![example workflow](https://github.com/vyos/vyos-rolling-nightly-builds/actions/workflows/vyos-rolling-nightly-build.yml/badge.svg)
# vyos-rolling-nightly-builds
Scheduled ISO nightly builds for current branch 

An official download page https://vyos.net/get/nightly-builds/

## How to check an image signature
```
wget https://raw.githubusercontent.com/vyos/vyos-rolling-nightly-builds/main/minisign.pub
wget https://github.com/vyos/vyos-rolling-nightly-builds/releases/download/1.5-rolling-202312191154/vyos-1.5-rolling-202312191154-amd64.iso
wget https://github.com/vyos/vyos-rolling-nightly-builds/releases/download/1.5-rolling-202312191154/vyos-1.5-rolling-202312191154-amd64.iso.minisig
minisign -Vm vyos-1.5-rolling-202312191154-amd64.iso
```
