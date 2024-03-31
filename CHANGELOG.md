## vyos-1x
- T6171: migrate <set service dhcp-server failover> to <set service dhcp-server high-availability>
   - PR: vyos/vyos-1x#3188
- T6171: dhcp-server: add fix for smoketest
   - PR: vyos/vyos-1x#3189
- bgp: T6106: fix test and verify()
   - PR: vyos/vyos-1x#3190
- T6121: Extend config-sync for QoS and system options
   - PR: vyos/vyos-1x#3193
- image-tools: T6168: compat mode update should preserve console type
   - PR: vyos/vyos-1x#3192
- op-mode: T6175: "renew dhcp interface <name>" does not check for DHCP interface
   - PR: vyos/vyos-1x#3194
- grub: T4516: correct a format string
   - PR: vyos/vyos-1x#3201
- T5872: ipsec remote access VPN: support dhcp-interface.
   - PR: vyos/vyos-1x#2965
- ipsec: T5606: T5871: Use multi node for CA certificates
   - PR: vyos/vyos-1x#3202
- T5832: VRRP allow set interface for exluded-address
   - PR: vyos/vyos-1x#3200
- vyos.template: T3664: add an environment variable for template location
   - PR: vyos/vyos-1x#3208
- vyos.system.grub: T3664: add chroot argument to the GRUB install function
   - PR: vyos/vyos-1x#3207
- openvpn: T6159: Openvpn Server Op-cmd adds heading "OpenVPN status on vtunx" for every client connection
   - PR: vyos/vyos-1x#3198
- dhcp: T6174: Add TACACS/Radius users to _kea group
   - PR: vyos/vyos-1x#3210
- image-tools: T6186: simplify image annotations fixing regression
   - PR: vyos/vyos-1x#3215
- bgp: T6106: Valid commit error for route-reflector-client option defined in peer-group
   - PR: vyos/vyos-1x#3213
- accel-ppp: T6187: use correct CPU counts adjusted for SMT
   - PR: vyos/vyos-1x#3218
- dhcp-server: T4718: Listen-address is not commit if the ip address is on the interface with vrf
   - PR: vyos/vyos-1x#3195


## vyos-build

