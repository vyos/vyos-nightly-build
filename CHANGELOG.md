## vyos-1x
- vpp: T9062: Enable DHCP/DHCPv6 client detection on VLAN sub-interfaces
   - PR: vyos/vyos-1x#5317
- vpp: T9018: Auto-enable promiscuous mode for interfaces with VLANs
   - PR: vyos/vyos-1x#5314
- udev: T9071: fix invalid ATTR key assignment
   - PR: vyos/vyos-1x#5322
- ci: T9082: scan C code with CodeQL (add c-cpp, build-mode none)
   - PR: vyos/vyos-1x#5331
- T9068: Add config manager module and refactor vyos-configd
   - PR: vyos/vyos-1x#5318
- wireguard: T8921: Fix false port-conflict error on qos dependent re-verify
   - PR: vyos/vyos-1x#5326
- T9079: Update on-dhcpv6-event.sh
   - PR: vyos/vyos-1x#5329
- router-advert: T9084: allow name-server-lifetime 0 in CLI validator
   - PR: vyos/vyos-1x#5332
- T8529: Add configuration CLI to enable OpenSSL FIPS
   - PR: vyos/vyos-1x#5139
- utils: T9008: migrate remaining cmd() callers to cmdl() and remove cmd()
   - PR: vyos/vyos-1x#5323
- wireless: T9104: fix CLI/OS race on interface removal
   - PR: vyos/vyos-1x#5336
- T9073: frr-exporter: add CLI support for optional collectors and collector options
   - PR: vyos/vyos-1x#5324
- T9105: confirm existence of config-mode file before use
   - PR: vyos/vyos-1x#5337


## vyos-build
- kernel: T8940: disable HYPERV_VTL_MODE and restore Hyper-V vPCI driver
   - PR: vyos/vyos-build#1236
- build: T9058: add a script for building Squid from source
   - PR: vyos/vyos-build#1237
- Kernel: T9067: Update Linux Kernel to 6.18.38
   - PR: vyos/vyos-build#1238
- Kernel: T5641: enable module compression to save disk space
   - PR: vyos/vyos-build#1239
- openssl: T9083: fix APT detected package downgrade despite identical versions
   - PR: vyos/vyos-build#1245
- Kernel: T8868: Enable crash dump (kdump) and debug info in config
   - PR: vyos/vyos-build#1243
- sbom: T9098: syft should run un squashfs instead of unpacked chroot
   - PR: vyos/vyos-build#1246
- Kernel: T9103: fix arm64 syscalltbl path breaking linux-perf package build
   - PR: vyos/vyos-build#1248
- T9099: improve test framework - add safeguards
   - PR: vyos/vyos-build#1247


