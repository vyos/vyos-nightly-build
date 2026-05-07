# AGENTS.md

## Project purpose
Public scheduler repo for the VyOS nightly ISO build. Runs `nightly-build.yml` daily at 00:00 UTC, builds a rolling ISO via the `vyos-build` toolchain, signs it with minisign, and publishes a GitHub Release that is linked from https://vyos.net/get/nightly-builds/.

## Tech stack
- GitHub Actions only (one orchestration workflow + CLA gate).
- Minisign for signature: public key at `minisign.pub` (verifiable by ISO consumers).
- `version.json` records the current latest build URL/version/timestamp.
- Vendored `minisign` static binary in `bin/` (used for ISO signing at workflow runtime).

## Build / test / run
The nightly run is automatic. Manual trigger via `workflow_dispatch` with inputs:
- `BUILD_BY` (default `autobuild@vyos.net`)
- `build_version` (default `1.5-rolling-YYYYMMDDHHMM`, e.g. `1.5-rolling-202604291200`)
- `SKIP_SMOKETEST_RAID1`, `SKIP_SMOKETEST_CLI`, `SKIP_SMOKETEST_CONFIG`, `SKIP_SMOKETEST_TPM` (booleans)
- `SKIP_RELEASE_PUBLISHING`, `SKIP_SLACK_NOTIFICATIONS`

Verifying a published ISO:
```
wget https://github.com/vyos/vyos-nightly-build/raw/refs/heads/current/minisign.pub
wget <release>/vyos-<ver>-amd64.iso
wget <release>/vyos-<ver>-amd64.iso.minisig
minisign -V -p minisign.pub -m vyos-<ver>-amd64.iso
```

## Repository layout
- `.github/workflows/nightly-build.yml` — orchestration (cron + dispatch).
- `.github/workflows/cla-check.yml` — CLA gate via `vyos/vyos-cla-signatures/.github/workflows/cla-reusable.yml@current`.
- `bin/` — vendored `minisign` static binary for ISO signing.
- `minisign.pub` — public verification key (committed).
- `version.json` — most recent build metadata (URL, version, timestamp).
- `CHANGELOG.md`, `README.md`.

## Cross-repo context
- Consumes the full build chain: `vyos/vyos-build` (toolchain) which in turn pulls per-package `.deb`s built via the internal build-packages workflow from the 14 source repos in `repos.toml`.
- The reusable workflows in `vyos/.github` and the `pr-mirror-repo-sync.yml` pipeline don't touch this repo directly — this is a scheduler, not a code repo.
- Sibling reusable build workflows for release trains live in an internal repository (`vyos-reusable-build.yml`, `vyos-reusable-vpp-build.yml`, train-specific reusables for `circinus`/`sagitta`).
- Release artifacts feed end-user-facing documentation in `vyos/vyos-documentation`.

## Conventions
- Commit/PR title: `component: T12345: description` (Phorge task ID at https://vyos.dev) where applicable.
- Default branch: `current`. ISO version strings carry the rolling timestamp form.
- Many repo-level secrets (the orchestration needs cross-org PATs, signing keys, Slack tokens, release publishers) — managed by ops; never committed.
- ISO signing key is sensitive: rotation is a coordinated security event.

## Notes for future contributors
- **Do not commit secrets** — all credentials and signing material flow through GitHub Actions secrets injected at workflow runtime.
- Skip toggles (`SKIP_SMOKETEST_*`, `SKIP_RELEASE_PUBLISHING`) exist for ad-hoc rebuilds; default everything OFF for normal nightly cadence.
- The published `version.json` is read by the website (`sentrium/next-js-vyos`) and download-page tooling; format is an array of objects (`url`, `version`, `timestamp`).
- Release notes pipeline lives separately in `andamasov/release-notes`; this repo only assembles the ISO and publishes the GitHub Release.
