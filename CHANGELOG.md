## vyos-1x
- op-mode: T5890: Fix arguments passed to generate_system_login_user.py
   - PR: vyos/vyos-1x#2746
- configdict: T5894: add get_config_dict() flag with_pki
   - PR: vyos/vyos-1x#2750
- T5897: frr should be stopped before vyos-router
   - PR: vyos/vyos-1x#2752
- T5169: nat: add option to map network and ports. 
   - PR: vyos/vyos-1x#2694
- smoketests: T5887: remove IXGB driver
   - PR: vyos/vyos-1x#2749
- T5900 dns forwarding: reliability improvements
   - PR: vyos/vyos-1x#2757
- dns: T5900: fix smoketests for serve-stale-extension and exclude-throttle-address
   - PR: vyos/vyos-1x#2761
- T5195: add timeout argument to process_named_running()
   - PR: vyos/vyos-1x#2764
- op-mode: T5904: add "show ipv6 route vrf <name> <prefix>" command
   - PR: vyos/vyos-1x#2765
- pki: T5886: add support for ACME protocol (LetsEncrypt)
   - PR: vyos/vyos-1x#2758
- image: T5898: fix kernel-level partition rescan
   - PR: vyos/vyos-1x#2760
- smoketest: T5195: fix BasicInterfaceTest tearDown() timeout penalty
   - PR: vyos/vyos-1x#2769
- pki: T5905: do not use expand_nodes=Diff.ADD|Diff.DELETE) in node_changed()
   - PR: vyos/vyos-1x#2768


## vyos-build
- Kernel: T5887: update Linux Kernel to v6.6.9
   - PR: vyos/vyos-build#482


