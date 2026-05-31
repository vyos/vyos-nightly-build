# About

Release/artifact store for VyOS nightly build images. This repository does not
run the build itself — it hosts the published nightly build
[GitHub Releases](https://github.com/vyos/vyos-nightly-build/releases) (ISO
images and their signatures) plus the signing public key. The images are
produced by the VyOS build infrastructure and linked from the official download
page https://vyos.net/get/nightly-builds/

## How to check an image signature

Download signature public key

```
wget https://github.com/vyos/vyos-nightly-build/raw/refs/heads/rolling/minisign.pub
```

Download ISO image and signature file (example):

```
wget https://github.com/vyos/vyos-nightly-build/releases/download/1.5-rolling-202312191154/vyos-1.5-rolling-202312191154-amd64.iso
wget https://github.com/vyos/vyos-nightly-build/releases/download/1.5-rolling-202312191154/vyos-1.5-rolling-202312191154-amd64.iso.minisig
```

Verify signature

```
minisign -Vm vyos-1.5-rolling-202312191154-amd64.iso
```

