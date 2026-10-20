## vyos-1x
- kdump: T8868: skip kdump-tools when no crashkernel= is set
   - PR: vyos/vyos-1x#5576
- nat: T9475: commit failures and weight issue in load-balancing, translation issues for port-ranges
   - PR: vyos/vyos-1x#5574
- wlb: T9472: silent daemon failures, ignored options and connections broken by commits
   - PR: vyos/vyos-1x#5571
- dhcp: T9108: silence per-run systemd messages of the lease-watch timer
   - PR: vyos/vyos-1x#5580
- GitHub: T9452: run ISO version step under bash so PR names apply
   - PR: vyos/vyos-1x#5577
- bgp: T9450: stop re-sending unchanged BGP lines to FRR on every commit
   - PR: vyos/vyos-1x#5578
- policy: T9394: reject route-map deletion if still used inside VRF instance
   - PR: vyos/vyos-1x#5579
- isis: T9485: only enable SR-MPLS when MPLS segment-routing configured
   - PR: vyos/vyos-1x#5581
- haproxy: T9097: add ssl checks-only for TLS health checks
   - PR: vyos/vyos-1x#5529
- firewall: T9474: multiple issues in rule processing (time based rules, fragment matching and failing commits)
   - PR: vyos/vyos-1x#5573


## vyos-build
- no changes
