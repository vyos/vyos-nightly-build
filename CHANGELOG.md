## vyos-1x
- static: T9278: reconcile FRR config after every DHCP lease event
   - PR: vyos/vyos-1x#5446
- T9279: VPP extend num-rx and tx ring descriptiors to 32768
   - PR: vyos/vyos-1x#5448
- image: T5475: derive the persistence path from the overlay upperdir 
   - PR: vyos/vyos-1x#5443
- smoketest: T9014: make configtest serial console image flavor agnostic
   - PR: vyos/vyos-1x#5449
- static_arp: T9268: Fix deletion of static ARP entries
   - PR: vyos/vyos-1x#5452
- T9269: fix container boot failures and two config diffing regressions they exposed
   - PR: vyos/vyos-1x#5456
- T9290: Fix typo for the image.py file
   - PR: vyos/vyos-1x#5457
- bond: T9269: keep the bond MAC when appending a member interface
   - PR: vyos/vyos-1x#5454
- firewall: T9157: add fib-type match for destination/source
   - PR: vyos/vyos-1x#5372
- vbash: T7575: Prevent re-declare readonly variable
   - PR: vyos/vyos-1x#5412
- monitoring: T9260: relay local frr_exporter metrics via Telegraf
   - PR: vyos/vyos-1x#5440
- http-api: T8989: fix X-Client-Verify header passthrough auth bypass
   - PR: vyos/vyos-1x#5464
- configquery: T8409: resolve op-mode config paths independent of edit level
   - PR: vyos/vyos-1x#5451
- podman: T9297: Encapsulate quadlet key/value parameters
   - PR: vyos/vyos-1x#5461
- T8264: add proper support for openvpn 2.7
   - PR: vyos/vyos-1x#5435
- tech-support: T5475: do not archive nested mount points below /run
   - PR: vyos/vyos-1x#5462
- ethernet: T9228: only warn about unsupported NIC features when node changed
   - PR: vyos/vyos-1x#5460
- ifconfig: T9313: fix removal of QinQ sub-interfaces
   - PR: vyos/vyos-1x#5469


## vyos-build
- T9245: podman: add libsystemd-dev to enable automatic health checks
   - PR: vyos/vyos-build#1278
- Kernel: T9298: make linux-firmware package architecture aware
   - PR: vyos/vyos-build#1299
- vbash: T7575: vyatta-bash 5.2.37 using build system
   - PR: vyos/vyos-build#1285
- T9294: strongswan: add security patches
   - PR: vyos/vyos-build#1300
- Testsuite: T7575: strip terminal escapes when parsing console output
   - PR: vyos/vyos-build#1301
- Testsuite: T9301: read the console type where GRUB keeps it
   - PR: vyos/vyos-build#1302
- T9277: image: further reduced installed and ISO image size
   - PR: vyos/vyos-build#1291
- openvpn: T8264: build 2.7.5 backport for the in-tree ovpn module
   - PR: vyos/vyos-build#1281


