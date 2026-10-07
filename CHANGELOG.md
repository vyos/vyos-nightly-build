## vyos-1x
- T9341: Fix consistency of legacy templates, xml_ref cache, and reference tree
   - PR: vyos/vyos-1x#5493
- T9365: add bindings for reference tree path from config path util
   - PR: vyos/vyos-1x#5513
- policy: T9379: prefix-list duplicate check in linear time
   - PR: vyos/vyos-1x#5525
- webproxy: T9371: fix typo in the squidGuard local-block-url rule ACL
   - PR: vyos/vyos-1x#5522
- pppoe: T9395: render default routes via FRR only
   - PR: vyos/vyos-1x#5532
- frrender: T9377: do not save the FRR configuration a second time
   - PR: vyos/vyos-1x#5524
- config-mgmt: T9399: read the committed config once in the post-commit hooks
   - PR: vyos/vyos-1x#5533
- op-mode: T861: add "show secure-boot detail" command
   - PR: vyos/vyos-1x#5537
- agents: T9348: update content in AGENTS.md to improve AI generated changes
   - PR: vyos/vyos-1x#5497


## vyos-build
- T861: Finalize VyOS kernel signing for UEFI Secure Boot
   - PR: vyos/vyos-build#1313
- Kernel: T9014: regenerate arm64 base config against Linux 6.18 
   - PR: vyos/vyos-build#1314
- Kernel: T9385: Update Linux Kernel to 6.18.54
   - PR: vyos/vyos-build#1315
- T9392: Keep kernel objects and don't create source tarball by default
   - PR: vyos/vyos-build#1316
- Kernel: T9385: Update Linux Kernel to 6.18.55
   - PR: vyos/vyos-build#1317
- Testsuite: T861: boot VyOS CA signed images as-is in Secure Boot test
   - PR: vyos/vyos-build#1320
- smoketest: T9402: stop navigating the installed system's GRUB menu
   - PR: vyos/vyos-build#1319
- agents: T9348: update content in AGENTS.md to improve AI generated changes
   - PR: vyos/vyos-build#1310
- T9400: Fix APT repository key for Debian Trixie release
   - PR: vyos/vyos-build#1318


