## vyos-1x
- dns: T8045: expose PowerDNS dont-query list as recursion-exclude-address
   - PR: vyos/vyos-1x#5409
- T9261: Python interpreter startup makes the CLI sluggish on low-cache CPUs
   - PR: vyos/vyos-1x#5434
- T9269: fix issues after recent GRUB serial console rewrites to support VyOS in container
   - PR: vyos/vyos-1x#5437
- T9231: Add reference_tree utils to return paths satisfying condition
   - PR: vyos/vyos-1x#5420
- http-api: T8989: add REST Bearer token authentication
   - PR: vyos/vyos-1x#5381
- T9273: Add Telegraf global_tags option configurable
   - PR: vyos/vyos-1x#5438
- sysctl: T9283: stop low-level Kernel messages on the console
   - PR: vyos/vyos-1x#5447
- update-checker: T8497: fix command injection via crafted update server response
   - PR: vyos/vyos-1x#5450
- static: T9278: reconcile FRR config after every DHCP lease event
   - PR: vyos/vyos-1x#5446


## vyos-build
- oci: T9269: compress OCI image and minor fixes to container runtime
   - PR: vyos/vyos-build#1286
- Kernel: T9272: update Intel out-of-tree IXGBE and ICE drivers
   - PR: vyos/vyos-build#1287
- Testsuite: T9276: RAID1 test sporadically fails due to timeout violation
   - PR: vyos/vyos-build#1290
- image: T9283: clean up warnings and errors during ISO build
   - PR: vyos/vyos-build#1292
- oci: T9269: mask systemd services for container startup and add healthcheck
   - PR: vyos/vyos-build#1289
- Kernel: T9283: run Accel-PPP depmod for the target Kernel version
   - PR: vyos/vyos-build#1293
- T9286: Update accel-ppp-ng to the 8cb6287 version multiple security fixes
   - PR: vyos/vyos-build#1294
- T9014: install flavor.json before Debian packages are installed
   - PR: vyos/vyos-build#1295
- Kernel: T9287: Update Linux Kernel to 6.18.50
   - PR: vyos/vyos-build#1297
- T9269: add OCI container image test
   - PR: vyos/vyos-build#1296


