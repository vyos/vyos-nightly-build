## vyos-1x
- http-api: T6069: fix allocation outside of thread lock
   - PR: vyos/vyos-1x#3089
- T6061: fix rule parsing when connection-status is used
   - PR: vyos/vyos-1x#3087
- T6096: Config commits are not synced properly because 00vyos-sync is deleted by vyos-router
   - PR: vyos/vyos-1x#3085
- wifi: T6095: incorrect country "uk" it's actually "gb"
   - PR: vyos/vyos-1x#3090
- T6075: firewall and NAT: check if interface-group exists when using them in firewall|nat rules.
   - PR: vyos/vyos-1x#3088
- conntrack-sync: T6057: Add ability to disable syslog for conntrackd
   - PR: vyos/vyos-1x#3099
- remote: T6104: fix logic of failure case in MissingHostKeyPolicy
   - PR: vyos/vyos-1x#3100
- snmp: T2998: SNMP v3 oid "exclude" option fix
   - PR: vyos/vyos-1x#3105
- vrrp: T6020: vrrp health-check script not applied correctly
   - PR: vyos/vyos-1x#2966
- http-api: T6107: add an option to increase the request body size limit
   - PR: vyos/vyos-1x#3108
- dhcp: T6102: Fix clear DHCP lease op-mode
   - PR: vyos/vyos-1x#3106
- firewall: T6071: truncate rule description field to 255 characters
   - PR: vyos/vyos-1x#3113
- xml: T5738: revert invalid change from lower character limit - 0 length must be allowed
   - PR: vyos/vyos-1x#3115
- dhcp-client: T6093: extend regex for client class-id's with DOT 
   - PR: vyos/vyos-1x#3117
- xml: T6098: relax description constraint to allow non-ascii characters
   - PR: vyos/vyos-1x#3110


## vyos-build

