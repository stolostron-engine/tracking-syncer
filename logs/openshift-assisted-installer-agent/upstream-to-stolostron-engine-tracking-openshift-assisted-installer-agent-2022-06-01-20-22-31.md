## Fast foarding of openshift/assisted-installer-agent into stolostron-engine/tracking-openshift-assisted-installer-agent.

## Status Summary:

release-ocm-2.6 -> backplane-2.1: First run, created backplane-2.1.  
release-ocm-2.5 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-ocm-2.6 -> backplane-2.1:

New commits (first branch sync):

```
d4e7b0bf650547a7b83e867aa4b2a1510f05f641 MGMT-9505: SMART data should include only errors (#364)
ce3cdbfd27dd2939dd52d1e46ab4242f56357175 MGMT-10003:     If skip-installation-disk-cleanup is set path it to installer command (#362)
48096a20737f9aa74aa04a7226fd3c0b96ff66fd NO-ISSUE: update bluemonday/runc pkgs (#361)
dd1b1b3dfd0bcd64653afe2276d9f22794639b0f AGENT-204: Multi-arch support for OCP build (#356)
43e9639d6a23b08f3c6a4077297ec79136691924 MGMT-10514: additional NTP source failed to sync (#359)
c988e59b59b03f171c4d75b9abb6a3174d49cc52 NO-ISSUE: Bump github.com/hashicorp/go-version from 1.4.0 to 1.5.0 (#358)
cddfa074a8fb27507ebb0272d7a433d9f374c19c MGMT-10454: Run next-step-runner with unlimited pids limit (#357)
8f3dc7ad820fe8c8c0fe29b0439da99ae5fa9fec NO-ISSUE: Bump github.com/coreos/ignition/v2 from 2.13.0 to 2.14.0 (#355)
e8ff9836d99113886121431d84fdb5383505175a NO-ISSUE: remove redundant ok-to-test label (#352)
1da51c32de5c006daa71fd3558d9cac9738d0657 MGMT-9379: Validation should allow HA mode to be empty in parameters. (#350)
e7445c4e8a6181470277750f27b293322c34604c NO-ISSUE: Bump github.com/go-openapi/runtime from 0.24.0 to 0.24.1 (#351)
71823d6d96a1fc3049ab8a4a1d5d60da5e5a56cb AGENT-153: Add .ci-operator.yaml for OCP payload image (#348)
0ffdf98e17135adadeb54be4418916be5d964464 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.2 to 0.24.0 (#346)
89405454e4f080235a8dd06374bab49be1424231 MGMT-10154: Remove usage of command on step object (#344)
7ccc6d9c4397190337e7055d7abb09e00e8ba3f8 MGMT-10154: Remove an option to run custom commands in agent (#343)
9bb4db43f4b4aa45fb82eb347acdeea5cd288c53 NO-ISSUE: in ci pulling image can be too quick and we can't validate 2 running image availability commands (#342)
050a4ea5427565ab36a4bead6565ad8c4d82bf09 MGMT-10097: Move subsystem tests to new agent protocol (#339)
897f8b322bf8b849ec847b0a3264c8f2fe76ef68 NO-ISSUE: Create reply cache per session instead of global one (#338)
8a8c15a720cb1bf866dbbe76054f5a34bf16ec88 MGMT-10080: Agent subsystem crashes on panic when trying to register host with no DMI information (#335)
4aecb19f0df5393be0d85937a3ee5b09bfc269b4 MGMT-10070: Enable next-step-runner and tools to get the logger as parameter (#334)
906ee7b2ee495eda3bd7d79ac2a7bb6947226084 NO-ISSUE:  Add utility function that creates custom journaled logger (#333)
d8b4aee3d478cfc37dc280e7ffbacbe2b2213137 NO-ISSUE: Capitalize ValidateCommon to enable accessing it externally (#332)
f5b2ef7e297bf170a581f672263f5cc806644fcc Add ocp release support (#329)
a3ea5857ceb7521a7e367c1d2722e2873e165806 MGMT-9854: Eliminate use of global variables, and use context variables instead (#330)
7d17a9ff78ad08b377ae26d00fa1895d025e57c1 MGMT-9453: Implement params validation per each step (#328)
297942787b6107b90229c41c8d5f88cd7954f6b7 NO-ISSUE: bump assisted-service version (#324)
b1fe36c9cda47950a21b78f8e9f6af9a35d53a8c MGMT-9806: Enable unifying agent and next step runner (#322)
71cb575878faa64dcbe6113ffac16fec4818a639 MGMT-9807: Enable next step runner to run tools directly in addition to the running them in container (#320)
7dd64e88a5525cef98ea29d3c1ac3aa3007a2104 NO-ISSUE: Pass agent image name to subsystem docker file (#321)
36423c83ce8981080f53df71cab3f77c4ad9adfd NO-ISSUE: Bump github.com/onsi/gomega from 1.18.1 to 1.19.0 (#319)
00bdbb08435018a01f7e637f6d6375ebbf8a58c2 NO-ISSUE: Bump github.com/jaypipes/pcidb from 0.6.0 to 1.0.0 (#318)
aea5b4e5bbad3b541443e4d744ec3605c4a6e0d2 NO-ISSUE: Bump github.com/stretchr/testify from 1.7.0 to 1.7.1 (#312)
9805e89e362ee69a80eb555a2830db3deefdb087 MGMT-9451: Latest api fixes and moving to master branch of service models (#316)
2a729aa5f04125a5c8466bb7a80daf82deda61cc MGMT-9451: Moving to new service-agent protocol (#315)
6c0f1e19b1c086ab207d228c247e40cd16169780 MGMT-9451: Moving to new service-agent protocol (#295)
94f667c8d2b86074336d37a2f68d0fabd9f62f6c MGMT-9344: Delete Jenkinsfile (#311)
51582c5f52e9c22ca1e19fcdff122141ec1e4d2c NO-ISSUE: Bump github.com/thoas/go-funk from 0.9.1 to 0.9.2 (#310)
d05222663c08a61082e0b36e9832192443d8a9de MGMT-9358: update assisted-service after split to submodules (#304)
5f5b002736c8b8e7c7125756c748efdc30166db9 NO-ISSUE update container golang version to 1.17 (#308)
a9e4f3999510bf95e000a496c43bc37ea7457c3d NO-ISSUE: remove .ci-operator.yaml file (#307)
add5ab0b01cdcb8117acf4b574fc488c5c437c7b NO-ISSUE: replace .ci-operator.yaml to use local dockerfile (#306)
4fbd870ebd146094b31f99835841648c25a3b3b8 NO-ISSUE: add ci operator file (#305)
ad17f8e1a5607df93672271b680ec045c852c044 NO-ISSUE: Bump go-openapi/runtime to 0.23.2 (#302)
5de8ce7764d22435a031efc14b1370f19ff7626e NO-ISSUE: Bump github.com/jaypipes/ghw from 0.7.0 to 0.8.0 (#267)
e36b05c9c8251350eacbbca320c11ee5fc027631 NO-ISSUE: Remove small timeout subsystem test (#300)
7efd8892e3441bd9ede239720b4cfa7b4350bfa1 NO-ISSUE: Don't delete the subsystem_agent docker-compose image every time (#301)
9e035f47f2fac18e3487ac3768795558e269a37e MGMT-9481: Support linode serial/uuid (#298)
6a81a61b7445765d0fc484e3f030047b49ec237f MGMT-9344: Return non-zero exit when subsystem test fails (#297)
5dd71705eec88800d595c4805974402942571d20 MGMT-9396: Fix UUID fallback (#294)
b656f9eb2c3a1f45fcd9e58b3e8b1924c1ee1130 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.21.1 to 0.21.2 (#291)
ff0baa554db8fa8a3865c7eda74cda931e1fe591 NO-ISSUE: remove Jenkins publishing step (#293)
0830bd09a7d8a8472587872b9ee6051b57732a6d MGMT-9189: Publish coverage report (#292)
b79b5d775f6ca3c6a30bb35541752026cd7f87cf NO-ISSUE: Bump github.com/go-openapi/swag from 0.20.0 to 0.21.1 (#289)
f13de8989571f3a61a9ff194a83655620905375a MGMT-9043: Set multipath device as eligible (#283)
52b9970365d20c197cd19070b40398d6aac89fee NO-ISSUE: install smartmontools from stream8 repos (#287)
206307c1d777ed4179ab3c8b35bf6525216a2bc8 MGMT-7813: Reduce smartcl verbosity (#282)
d2a9f98291ab47a8af4f46f1927290711e621625 NO-ISSUE: Bump github.com/go-openapi/swag from 0.19.15 to 0.20.0 (#281)
93342ccd698829d38fa121f13b6567aadf40da73 NO-ISSUE: Bump github.com/onsi/gomega from 1.18.0 to 1.18.1 (#279)
42278a57f1ff6a255a10b01bba6856426ae2dd7c MGMT-8752: handle ocp router 503 errors (#278)
e4bebc1e7106236a8a3befdaaed0729a49920347 MGMT-9040: include only Luks section of ignition in response (#277)
0317df2d10914815855a5dd8e8f7dea85eaf259b NO-ISSUE: Bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5 (#269)
7c4cfd1d731bd5e994cefd4f9cb239ccc9f56787 NO-ISSUE: remove redundant GitHub Actions files (#276)
6ee312d9748e9164d4c80d7ebc18f23d43fdc83b NO-ISSUE: Bump github.com/sirupsen/logrus from 1.7.0 to 1.8.1 (#273)
36f5c7862951b4a1f95cc03ffee18bbe70c071f0 NO-ISSUE: fix dependabot commit messages to include NO-ISSUE (#275)
13774bd07b77b37e6d02963f63fa56fc64ea14a6 NO-ISSUE: Bump github.com/onsi/gomega from 1.16.0 to 1.18.0 (#274)
b7af0d13bdd2c0f2c7901b6295f7ec75d16cc0fd MGMT-8481: Allow fallback for generate uuid from mac for kaloom deployment (#272)
8919643674e6321515088fbff336a546e2de76e4 NO-ISSUE: Bump github.com/thoas/go-funk from 0.8.0 to 0.9.1 (#270)
439b28b50ea4205cd55d47a865b434b2d272aa7f NO-ISSUE: update assisted-service package (#266)
57baa621a1c04d5bae4b2a7ac1822317088c28cc MGMT-8847: Add bf serial value to unknown serials in agent (#265)
c7a3a430fecbef64a89a33d8a9739ab9bd802500 MGMT-7428: return ignition in apivip_check response (#263)
e37c4190854d860f46acaf3e7019e992a4dd9406 MGMT-8623: capi-provider-agent fail to add host to hypershift due to API VIP connectivity failure (#264)
487be214c7d0521f50cd540e1260eec6c022961b MGMT-8424: Add token and CA cert to API VIP check (#261)
55d9252ac2bb120f19a7779b8f5a23ef4c1fe048 MGMT-7428: apivip_check - Accept in request header (#262)
6f7459cf58f72e921c3d011b5da68840261ad0ac MGMT-7847: Don't check verify CIDR in the host (#235)
e72724636866f3421c9d5600867089b4c4e2a1ad MGMT-8422: apivip check remove suffix (#260)
51fca8bd01227bd82f6418084d7cf49811c1d04a OCPBUGSM-37106: List only physical disks on inventory. (#259)
1b51ecd2786c0f56ceb8f2051fe0af4dae1f7173 MGMT-8294: Adapt assisted installer agent to latest swagger changes (#257)
720bfed358fc01f827413c4e95ffc0cfc127b616 MGMT-7941: Allow forcing the IP address and hostname of the agent in dry mode (#256)
60e82d05d8259184efa4772dc60dbb87537fa67b MGMT-7941: Fix agent dry reboot condition in wrong code path (#254)
de31b85976055ad71cb9f689be2b6db73086e470 MGMT-8163: Logs sender logs should be printed to stdout (#253)
1e818b2737ca41b8cb6121ed718d95f7984a375b NO-ISSUE: Logs sender lsblk unknown column error fix (#252)
bf66b232529b5023f29eca554f9ed6c51b2a6044 MGMT-7941: Introduce dry mode to the agent (#250)
53b0eacfa1474d847ed6297dc234bafc34241305 NO-ISSUE: Inventory accepts Ghw Chroot path (#248)
ea4b2816abab5dff8536b03f2c56cb84a7a33738 Bug 2017502: don't return error from Resolver in case domain not found, (#251)
761e669621bbfb92fe443708d522b97910b639e2 OCPBUGSM-34971: container image availability command should not exit 0 if it failed on one of the images (#245)
dda746a296408e83e52a98d7db19b601d53c39c9 Bug 2012839: Agent should use V2 API for HostLogProgress report (#246)
37a5214e61853797883c5fe8e37a11d533943d24 NO-ISSUE: Remove user yuvigold (#244)
7918e3bf38a5001d60778d7b39f405b590026307 NO-ISSUE: Removing \n suffix from TPM version. (#242)
65d2e6db57cc2dc895baabc9ee3b12c195c19974 Bug 2011300: Agent should use V2 UploadLogs API instead of V1 API (#240)
669a2d7d699f2557a627eb949975d0e81ac1c565 Bug 2009241: Agent should support receiving InfraEnvID as part of SendLogs command (#239)
422b94c1f73118d7ecf272605a331b6c66f48fcc NO-ISSUE: Add lranjbar to OWNERS_ALIASES (#234)
05e460bca5e86feef4c48a772b3396c5ee8b1a49 MGMT-7761: Switch to stream8 (#237)
38b5a5f880866b695a3ddd9b80f056185a05b41f Merge pull request #238 from flaper87/flaperowner
763eaf7f5d263b4a3b013463329a4fd0e4d279d4 NO-ISSUE: Add flaper87 to approvers list
14870a7501549fa77bb04480d7c70caa036caee5 MGMT-7847: Add a deprecation warning for the VerifyCIDR option (#236)
4d39baf5fac3c28bb69458428335a3d540350904 MGMT-7457: Adding TPM version to host inventory. (#232)
d9a8a4aab778e0769abcf15eb9c16bd44bd2b683 OCPRHV-591: Add oVirt support to the agent side (#225)
60ac74ef05e45fd612222f3bd17f0b148d346d98 MGMT-7661: Add property called physical_bytes_method to memory (#231)
ad772bdcf765cc3a9aac387b769dc97b6651a39a NO-ISSUE: Add lsblk output to the log sender (#223)
e96269abbb1dcf3561dc414e4cf4da845709198b MGMT-5400: Get physical_bytes from ghw if dmidecode was failed (#227)
938df898fee740b2820d7afffde86b985506b24a NO-ISSUE - Add eliorerz to OWNERS (#229)
efe8ea006c178db1d8a6164262825219c9eb7fa4 MGMT-7659: Generate and update the agent (#228)
38136d7814a1c4f8ac498ffa5ce4c1598193d054 MGMT-7597: Remove ronniel1, and razregev from OWNERS (#226)
3d697f0b1a4988782205dd4cffac6b948d53d223 MGMT-7443: add removable attr to Disk (#224)
6c955e8319e0762c6c2b6f05baacd8b7d4c62d25 NO-ISSUE: Align IP protocol version number (#222)
b14d0a3e83e6da385006169aa6780e57b2f785b0 Bug 1990060: Host returns no routes with multipart (#220)
c1573868b0fd09f003d440c1834f4b41de6227ee MGMT-7407: Remove V1 APIs from agent (#221)
bda33e2f2fc9f6f04d46d6ac90d4f04a32604517 MGMT-7383: Add v2 APIs to agent (#219)
1d517b6cbfa1e9f71b41501b485de20f83121764 Bug 1975672: Parse GW nil as net zero (#217)
94d71302869c801daac992c811b6bb93e7b21269 MGMT-6977: Make sure that the image availability timeout is per tool run instead of timeout to pull single image. (#218)
38841dee2846214441576a19ded4f5a994f31312 MGMT-7210: Upgrade Go version to 1.16 (#215)
57afa1673f9328f840b102362aff8103f62740ca NO-ISSUE: fix OWNERS files to match group members roles (#212)
885f669df1d5b2ade50739fd0b78d0df0cd998c0 MGMT-6498: Remove filtering when capturing route information (#211)
8a8c4c4c4969b98286ed6ddb64c757f98b56af7c MGMT-6498: Capture router information in inventory (#209)
8d63a0ece1e669e679b1a44d1331213f3b8bcfb5 NO-ISSUE Add mkowalski to OWNERS/code-reviewers (#208)
2d07639aeff2c689390f6a48359505e66d181b1c NO-ISSUE: Add check commit script (#205)
30cdb974bb9f7e5dc1ae5bfe03ad6ed7cd071df0 NO-ISSUE: Fix linter errors (#204)
b04b05caf30f4b15ce4c2ed34cda3d4d36c00160 Publish tests junit (#202)
f5dd8915b1fda0408a1a74226050ca79d7f0faf8 MGMT-4966 Display a better message when media disconnection failure occurs (#197)
799e4bd24b12c56808d2898f87a431f53e481db9 MGMT-6668 Invalidate agent cache when there is a problem to perform get next steps from assisted service (#201)
5f5de4df21ae843517d1348adbc031c9b2c74c78 MGMT-6656 Sort connectivity check replies before returning the results (#200)
0827f184fbbf9302b31484441f5dd3e16d73fbd4 MGMT-6484 [WIP] Create cache for post step reply api calls (#198)
72b14c873597f3883eab9af308fb803b344af2d0 MGMT-4327 Remove old FIO tool from service and agent after the new tool is in use (#196)
3eb41884f8d7eee77e9cbac5647918149896f18d MGMT-4718 Capture network latency for L3 (#187)
ae01c7568822924689149b6c3827ada5faa9258b OCPBUGSM-27088 Filter out ipv6 local link addresses from inventory. (#195)
3d012cfc546213b4c064fef5bb4a4802e84fbbf9 MGMT-4142 Using ghw to detect GPUs (#193)
e217062c630886a821eefecaa3fc3ab62cc1a0b6 OCPBUGSM-27560 Duplicate installation disk. (#192)
42d49b73098ae12d1879768f01c390fa952d1cae NO-ISSUE Bump github.com/jaypipes/ghw from 0.6.1 to 0.7.0 (#190)
32ba879c3e0e7586a245618cdf45d7c041f9f25b MGMT-4397 Fix command args of disk_speed_check (#191)
299b4b3a8179a816403ee1882def3f5786979727 MGMT-4142 Detect GPU devices (#186)
7490d17a267d50522758ebcbe4666b8f85fc0e75 Use 'Errorf' instead of 'Infof' for step failure (#188)
4ae8931b8dad082b4907f270b738df7d9b2b6254 MGMT-4397 Agent changes - adding new tool for disk speed check (#185)
4b8a77a7db432763c508b11bdd23be556be2197f MGMT-4117 ovs logs gather (#184)
d28226138b29a122d2bae5108e81cebf693bb105 OCPBUGSM-26414 - changing the filtering of the network interfaces during inventory and connectivity to allow support for bonding and vlan interfaces (#183)
edbaff3f6b1343b6e51c64d461923ac592820476 MGMT-4048 change disk id to be the full path of the by-id link (#182)
0cf6d9f18cd2e4294a550bfeec0e2c7afdf0715f NO-ISSUE add michaellevy101 as an approver (#181)
363723f893eff0fb011a81c4522d048610a4971c MGMT-4052 Add id and by-id information to the iventory (#179)
3b8c3709294ea64e89c3663106c99d4ccadda204 Wait for image availability response in subsystem test to avoid race-condition (#180)
d0a02fa803847584117c2e6802ebb399207cb0c3 MGMT-3854 report log progress (#175)
3aab80c38d5779c4bfaf258e5924a5ba0112c7c2 NO-ISSUE disk unit test refactor (#178)
27aca022c9224502659a0cb5f80e53d3a12e5284 Fix ginkgo skip flag (#177)
7482b99b25be9b36c0731ea23be65e216194e385 MGMT-4346 Collect logs in Jenkins Post (#167)
bc4cadcd5542715d021ab5fa37e557ec5249216a MGMT-3869 - Add domain resolution command to agent (#176)
49e34b56a65942fc7b128fbc8fbd7897c1544db3 MGMT-4053 Add output of listing the 'by=id' and 'by=path' links on the agent to the mounts.log (#171)
dd888746f393a3a9716012d8cb63592e3615ad9b MGMT-2925 Clearer error message when next step crashes (#174)
566fb848f1edebd2d1f725d6ecf88d7ee6d05396 NO-ISSUE Add git_revision label to the image (#173)
4968d22704d8c5fe78dc71d373aff830eb3e870c NO-ISSUE Switch registry.svc.ci.openshift.org registry to public registry.ci.openshift.org (#169)
d0b71dd6ecee9068fd087804816580678ccd2ff0 Fix IPv6 CIDR based on route (#168)
957e2a5c6965169e830a1abba7e839e2475bed83 NO-ISSUE - Upgrade assisted-service to latest version (#166)
68618ca607d10d7edb4c653254b33f7bb52749c5 Update dependabot.yml (#165)
b628c66db1236dfe242a1dad36771e59130298eb Bump github.com/go-openapi/swag from 0.19.13 to 0.19.14 (#161)
7dde6be6720c31ac077081bad9908e661f903096 Bump github.com/onsi/ginkgo from 1.14.2 to 1.15.0 (#159)
184208775aefb0599766a9a00f33bd475ffb6cb6 Bump github.com/onsi/gomega from 1.10.4 to 1.10.5 (#162)
c0aa46cf0d287b079f7d12f43fe268292bf638ac NOISSUE: Change Auth Token missing message (#164)
a9cb0d28121ecff43f70395f48790abcfcd6dc3e MGMT-3526 Add failed_to_pull_timeout unit test (#158)
1dadfbf9757764ca3b3974ab7ff6cd3fe4f71469 MGMT-3526 Add container_image_availability tool (#146)
0bfedc461084f83c2f2b7464c25eda0ecceb4d40 Add docker ignore file (#154)
6710e9d2a6bb59237e00ef9051340beab2afc8a1 NO-ISSUE - Human dmesg timestamps (#151)
c69818898255f6870b425ff4783f4dd8077c55c4 MGMT-3315 Multi-stage agent Dockerfile (#148)
94cae07716c035bf81b46c9f9804c40c7c16ce55 Bump github.com/google/uuid from 1.1.5 to 1.2.0 (#150)
53bceb5ea502f28530697242f1e4e970a6ed3da2 MGMT-3390 - Added lint and format - for now, lint not performed automatically (#149)
5c709826070bb85a8e35b0d5fbec44c2ee083574 Move cloudctl/dhcp:ubi to cloudctl/dhcp:micro (#147)
ee0384801d487bcf26b746bc2a4d3a663af1e45c Add generateNsenterStep and generateDockerStep to subsystem utils (#145)
d9c79b7b6f69ed000eb835936b07eafead8b93cc Bump github.com/go-openapi/swag from 0.19.12 to 0.19.13 (#144)
3007163da5f4ca38adfde3539af862f88af2c8d5 Bump github.com/go-openapi/strfmt from 0.19.11 to 0.20.0 (#143)
c4dfdcc2f0598524331c5de0b0ed557eda45005f Bump github.com/stretchr/testify from 1.6.1 to 1.7.0 (#142)
dc3602e9c5179ba94043964a78271cd8ff27ab3c Bump github.com/google/uuid from 1.1.4 to 1.1.5 (#141)
36db835769867d760979703871a2a30d17daf603 MGMT-3463 collect full journal logs (#140)
a2fda3ca4d2ec8c3bb7730bed0e3d686ba16cec2 Bump github.com/google/uuid from 1.1.3 to 1.1.4 (#139)
21a4e3a1b35de93f989a69514a36f2df71ac4169 MGMT-3458 Send step reply from FIO perf check (#133)
f017b4226d79bcd0148fc1c3123a3269b3c9bc27 Fix dhcpd lease file issue (#138)
79ed6225e0bf5a8ddf3c78c4d2e4fad44b6eb322 NO-ISSUE - Add omertuc to OWNERS_ALIASES (#137)
e7dd7b18c3310acc25749aa02c5101ce1f1b319f MGMT-3456 - Agent will now report whether a disk appears to be an installation media (ISO) (#134)
eed3a59db39982a1394d279815afb7266bc81b85 Bump github.com/google/uuid from 1.1.2 to 1.1.3 (#135)
610f11613cc669f56a17428f5a9fc9825844f983 Get test images from quay.io (#129)
74e13887e1bd04dd61c9920d92bf372015dbae1e MGMT-3026 Add log of FIO result (#132)
2da45a368d3b99ea680b4b33e392a813e910be4b Check for expected NTP Sources on NTP Verifier subsystem tests (#131)
28672290ea3e5fc59f9bf279482ad416bb8d8de6 Change resetAll order (#130)
02fe461968b79755ea58cd78295b765290475ed9 MGMT-3194 Use nmap for L2 connectivity check (#124)
74c2c6013a2ec17214ebed8755f303ccdb785ee9 Bugfix NTP subsystem tests - reset agent (#128)
6f281de73f7f1afd196c9a5e6d6674817a4ed13d MGMT-3026: skip slow disks using fio output (#119)
a070b977d947bfaeea00db0975758e17427b0252 NO-ISSUE fix docker login timeout (#126)
571582f1d3b9c4baf0e542409688c6629f2ff52b OCPBUGSM-22485 - Agent will now consider Xen HVM domU machines to be virtual (#125)
855e2a5d713768f8f9b981d06efb93308a1653ac OCPBUGSM-22486 - Assisted installer agent will now consider AHV to be a virtual machine (#123)
aa8dba6e643ca316fd191b6104a07819cf1ebb0d MGMT-3291 - Show all disks - mark eligibility instead of filtering (#122)
e53fd3f80ed303b8c1645fb9b0c3dbb146a952a8 OCPBUGSM-21553 NTP tool reverse lookup for IPs to hostnames (#121)
1c694228073656d9e017a47f2d5d6b5ccfaed6c1 Add GOCACHE to skipper.yaml (#120)
6fc79c454f08e648cbf5f0a6277c3b461b789b15 OCPBUGSM-21366 Support comma-separated NTP sources list (#118)
c7b6b54cf117164febb52ed7cfcacabdd75f2104 OCPBUGSM-21434 NTP: Ignore adding server failures (#117)
7a3d06c5bc56de9a59c6e62dbea15b19f5d7303c MGMT-2858: coredumpctl - use priviliged (#116)
1152832b0b44e06e7a911b78545a86d28afb273d MGMT-3262 Remove app-sre images (#115)
7798058ea9e2fd0847f42776ffc10aa58a878afc MGMT-3257: discarding disks of type ODD (Optical Disk Drive) (#113)
e2dfdf0ed9420e7da5e58fc65a16d778b12e074f Bump github.com/onsi/gomega from 1.10.3 to 1.10.4 (#114)
96f221c34b18c8683e5834a19200bdaa4b807118 MGMT-3211 - Never ignore smartctl, regardless of exit code (#110)
9907fc1923ae3bcfc7d3a55656c954b5480ed6c5 OCPBUGSM-21377 - fix check api vip: in case connectivity does not exists, return code should still be zero (#112)
3824c62c7faf82968d1dc26dd727c3b39fc159d4 MGMT-3012 - Add mount and volume display logs (#111)
dbf9357a634a71eb3035665fd1d11e571b1850ad Bump github.com/go-openapi/swag from 0.19.9 to 0.19.12 (#95)
0fa8d77664c532958199b11c6a044e19df1092c8 Use quay.io/app-sre/golang for build container (#109)
f8070bf0fdeab765d88450a3621723b17293c99b MGMT-3120 IPv6 connectivity check (#106)
ff08b27ebd3a1b8c3462546cd31a6bb7e8cbf6cd MGMT-2858: send_logs - use coredumpctl (#108)
843a8cf20f2f2ec85516db4bd7c543b7a8b673c9 MGMT-2858 LogsSender: added coredump and dmesg (#107)
aebd94105b4ed6442f21a7a26ab4e40eafd936aa OCPBUGSM-19005 - Print step output after step execution fails (#91)
9b98329153609994da4d0080dddb21bac8b210a1 MGMT-3088 push images to quay.io when we build from branch for installer & agent (#104)
4eaac4b1a48688f5d68f38734966903a524e1f88 Bump github.com/google/uuid from 1.1.1 to 1.1.2 (#79)
e9d687e7adb341751304b8ecfca28a50df31a774 Bump gopkg.in/yaml.v2 from 2.3.0 to 2.4.0 (#105)
e829efc192dd3ffd76b54925c190449cb0baaae5 MGMT-2777 Adapt IPv6 network prefix by using RA routes (#99)
42c062876dd442702497b6541ab190debadaa7c3 MGMT-3033 - Use newer smartmontools from the Fedora 32 repositories in upstream Dockerfile (#102)
7b2f278d8e3c2cf45d3d1d04ef0f971b84ecd802 MGMT-2951 - Will log reasons for why disks were skipped (#98)
5f6903e972997c4fa4c3ec9666618f6a8f632d7f Extend wiremock setup timeout (#101)
fe23eb50d5579bf334d8096afa271d89fb9152bc NO-ISSUE: Changing the order of logs gathering. (#103)
618c94b98ab7e093d721cad756ea460e046f084a NO-ISSUE - Remove masayag from OWNERS_ALIASES (#100)
0a4da3fe7c21ea0c40141ac7d6498fccdfd72bed MGMT-3033 - Populating S.M.A.R.T. field in inventory host disks (#97)
8a01d229f32d575a18033611451fe8d5571bbabb Bump github.com/go-openapi/strfmt from 0.19.10 to 0.19.11 (#94)
8015175352d0bb8e11887a820203adc5953d3e13 Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#93)
262fc055ee4c1930f736568f69389310f9ec89c4 MGMT-2678: Supplying non-bootstrap masters IPs to installer-gather.sh. (#90)
6fa33e27761ea361a03c5fdb5067b92692df684d MGMT-2219 Set mac address as prefix for unique hostname (#92)
da9f50d0ad6b03674b2e8118fed13f3ae781ef9f MGMT-2322 Add ntp_synchronizer executable (#83)
c3194394a014cfaaaa7ab585f5fb7b833822914f MGMT-792 - Updated assisted-service, replaced lshw with ghw, populated is-vm field (#89)
d2b42027c0b1b9f4deab324cb8e64d460bfb8943 Bump github.com/onsi/ginkgo from 1.14.0 to 1.14.2 (#78)
30abab5d291715b06909a7dbba9b3c3257a81874 Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.10 (#86)
9307b0d10d128a446f2ba958a17749d556c94a33 Update dependabot.yml (#88)
e3ee9677c5a1a810945bf393d1f197c1c15c041c MGMT-2440 Fix the errors in inventory when trying to get BMC information (#68)
7ebf6037422d4e19958c9e1488704e74c28d643d MGMT-2769: allow bonding interfaces (#71)
6e22aca3b04b24a8981766c252733441a634ac6f Bump github.com/sirupsen/logrus from 1.6.0 to 1.7.0 (#81)
69ff13046658712013feee8329709e3322a59af3 Bump github.com/onsi/gomega from 1.10.1 to 1.10.3 (#80)
515ddbe7bc1fe551d92499f356e487c5c1a87557 Add label downstream-change-needed on Docker files (#76)
84aa6878fcf3b8df5c8876bd2bf13b10a337fb91 NO-ISSUE add osherdp to OWNERS_ALIASES (#75)
0f0760d0dffa5917d8b87f6aae338f1a880c3971 NO-ISSUE update owners file (#74)
a959f7eec75e2ff3b10f8f4538d9f92d57738167 Update OWNERS
c2aa5c2701a2e219dc4b1e726383cde74354e38b MGMT-2592: filtering media disks from the inventory (#65)
3aea65b0ba71f6634939e6233184445066bd93a6 MGMT-2447 Exit next step loop on flag from API (#55)
1d6d1c92aedcd8f88843caa3b2fe00f388ea07f4 NO-ISSUE: Adding to logs the output of /usr/local/bin/installer-gather.sh (#72)
39dc06ac7dcb5335dbd6771f4a12a2d90090a758 NO-ISSUE: Configuring privilege command to run using host network namespace. (#70)
27d45ae54bf9bf0cf12a88c60e3240bd63efc1de MGMT-2213,MGMT-2380 Bring back split into registration and next step (#69)
a85739e83d21a6868d372baef4c1caf3cd33a28c MGMT-2659 DHCP server changes the VIPs addresses after installation has started (#67)
ff21bc8686cdcf0a18d26264798afcc12a7d1df0 Create dependabot.yml
7c16bdbd1f410eff3ae47afe135fd9ddca76ebdb MGMT-2578 use centos which doesn't have the defect version of nmap (#63)
eb3ee583a779f7b9dea9c43a04783a64c8618200 MGMT-2347: remove output from log message if step type is free-addresses (#53)
85a88bb5cb18c3f065260a56222a3a4e4e2b82d3 MGMT-2431: Adding 'installer-gather.sh' to logs_sender on failure. (#64)
3ad7c4de1e09392dfcd59e12e87b297ffdafce34 MGMT-2576 Bootable info not collected in inventory - Add file package to dockerfile (#61)
3e84ac7bf47dd5c1995fccf2d9be63b0c9a236d1 NO-ISSUE revert to fedora 31 (#60)
cffd8954c255559fd56495c03f56c7e98c9877e3 MGMT-2069: handle getting 409 from server when host tries to register to a cluster (#52)
2e2b6a27b4a3fc9dd9de0f8b5891d1ebe03a58f0 MGMT-2479 Revert splitting agent into register and next step (#58)
d99ae31adf433d2ca5d6496a1cde66de8bf9480c MGMT-2420 Add bootable flag to disk in inventory (#54)
1616c72ceaddf82d0e8986367b045b02d32a5164 OCPBUGSM-18605 Clearer dhclient timeout message (#57)
5115e7b58fb8d8f708a6b0ac1cb2738f2bf48c96 MGMT-2380 Update README (#50)
22c33e020c803dbfec41e6875ed7e6a44883b558 OCPBUGSM-18606 Improve log messages for failed step replies (#56)
6fcfff8bfd66bcf05fb0cec2ca609be2c518a578 MGMT-2213 Split agent into register and next step (#47)
033928931edc70e675ac5a226018a70c365430ee OCPBUGSM-19005 add log with StepId (#51)
11c372356b59a0ddb086e4831b6526c898d47ad7 MGMT-2318 network CIDR verification to API VIP (#46)
855933ba95ec34b62197bba7131adf2c8aaaa010 MGMT-2398 Logs upload is broken due to new fedora-minimal (#49)
1bc57a6bf2f9e91746e0f982112d67e7a4f43768 MGMT-2075 - API VIP connectivity check command (#38)
fa2618ae5a8b5a3cdfeb99c7ee084f6f2dff512d NO-ISSUE dummy commit for DS images (#45)
aa52cbcaf97e03ce871fe023da7f64ebaada9682 Use gotestsum tool for testing and publish junit on Jenkins (#44)
a2898461413b5ba6ce6d9e08a985d3398da9067a MGMT-2279 If Auth is disabled Token is not needed (#42)
39e36047915225021fda98d95ae611a4157bf893 MGMT-2342 adding timestamp to inventory (#43)
382c69e29d29e74e495dc13ef392d6f5fce2fe91 Notify on abort (#37)
06a598d8c162761c4a02ce8a7801864bb106fc6b OCPBUGSM-17431 update assisted-service client to support 503 and 401 403 for all apis (#36)
28cdc326ceb0a58a06e6f2a9227edcb329c5b2cf Update OWNERS file (#35)
ff0732f58da697c2b7c35530b282750838461cec Add timeout to wait for wiremock in order to avoid test failures on weak machines (#34)
c20bd63e42036d0c116f82d9f97f6bd371f7a1c6 Improve logging.  Session #2 (#33)
fa7f3a7fa597aaa3098eb7a683453e64598f3bad OCPBUGSM-15958 Improve agent logging (#32)
1c5b2e8e0ce18b3151eb9f0c15b0a8aa05a0cc56 Add additinal timeout for getting inventory so subsystem test could work on weak machines (#31)
5672e2c5534f8b2b42237a199d3f3946a3ec3c92 OCPBUGSM-16626 fixing typo (#26)
50e6a55cf8932e17f11f07bcc803416e78f86fbc Add FOCUS env parameter to skipper.yaml (#25)
b2df63af339ae700faa0c30687f68261c3201215 Switching wiremock to an unused port (#27)
d9d34e690c294878721bc9633037b3abef9af8a2 Image build with network=host (#29)
1430b38aa8672f4e7b7c2d18e7e6fa5da7c74312 Update jenkins file (#28)
c786e23a9786042e7968d0ff47b1b039a1792679 Update Inventory client and test for 401-403 (#24)
7a45790bc3a82476a242cf7b9c654d7d6770b080 MGMT-1680 Adds discovery_agent_version header to agent API calls (#17)
4a3b33ccbb4112e3ccc6862c0dfecca2820801a1 Adding tar to assisted_installer_agent image (#23)
19e6e1f9a76de9795a31a2ab17a6180aa9377c4c MGMT-1912 Remove docker install from Dockerfile.assisted_installer_agent and add Dockerfile for subsystem testing that adds docker installation (#22)
a1cabadfb77c5880779f7f1a34c856256983fd57 MGMT-1719 create dhcp lease allocator (#20)
699cbbd0f40ffda29b3ef26cdc297b63222d03e6 Merge pull request #21 from openshift/osher/notification
fb4e77c398820073c75ddbc05a6cb58faf5d86d9 send slack notification
14be679db6cd6ccb649485f74800cfd77d83f940 Merge pull request #19 from openshift/osher/jenkins_file_notification
273b4d3fee0eac7c616181c59eded88e2c79c545 Igal/upload logs bootkube (#18)
25440f96dbe8e41278a43e2a54db0f2f638cddf0 add link to notification
0a05fca9b5e72dc6bdaaad6ea6d4560f8ddaa91d Avoid subsystem failure when running on system that only virtual nics have IP addresses (#16)
009ddae05f09ddcbfefd674ea50e9e4112312525 add notification when master fails (#13)
b27895b701481015f2c78720a58043712d9703d7 MGMT-1880 Change path inside archived logs.tar.gz to logs_host_<host_id> (#15)
634d5048eb4a08ec628892473971d46318d6a228 MGMT-1876 Add insecure and certificate flags to logs_sender params (#14)
8164292b43b502014958a4f5fb216398970d16f0 MGMT-1861 Remove the warning log from agent about not being able to find motherboard serial number (#12)
6dbef262aaf793d0f991cbe7ebaed2127f4a3612 MGMT-1713 Remove deprecated host and port parameters (#9)
fad95178306c817cba3a2f63f7626e02af201ae1 Merge pull request #10 from openshift/osher/agent_update
26393f600034c118850e841ae493ad3cb19b096c Update agent to vm
bc9c7b899b8ad392922794d32735909dfb266fc7 Fixing don't delete flag (#8)
78ece80bebbea7c71ae72ac93f5bf52cc2e153bd Fix for delete folder after logs are sent (#7)
fef78b81ce26868f7db1f9067b3766146cf4dc8a Igal/upload logs (#4)
9912d24f0bbdf56056d9ba9184d20535dfc96a7b Change README and skipper.yaml and rename build dockerfile as result of repo move (#3)
e577982ee8cf65e8b9971a5a7e985b2ff6a7da5a MGMT-1695 Support HTTPS transport (#5)
b95a4adcf90f3dc62f440091a8956f804fdbbd25 Remove space at end of image name
69b457ce9ab1a095952526e490c7bfe8703ac9c3 Update image name
5f5d7abef22ac8f8ecfcf4672919c9671a238d5d Fix subsystem docker-compose file to override firewalld network block (#6)
e417c3f1c4e586c7bbb80eab153fb328152bcbcf Added Jenkinsfile
121ae01642972ffa7e01ab2b4bf4fbae606507ad Fix imports after move (#1)
e551596e4ec62c612b3006883d061c9fc0a83e62 Merge pull request #46 from ori-amizur/feature/owners-file
f4df0b0ba838bceabeacbaecb6003a1a835b7094 Add OWENRS file
611d9a843fa1a5fcb4cdae3f0136da27760d309b Fix github files from previous MGMT-1767
ffcab4a55b02ba57476c7848cde3e8882d43790e MGMT-1767 Move git repo ori-amizur/introspector to opnshift/assisted-agent
2282ec0ee5f14edfedb98a39fbbdfcc52ade7b27 MGMT-1661: Ensure aws xvd disks are discovered
eb62f60ccc991dba791efbe706007ae1d97ba4c9 Merge pull request #34 from rollandf/pullsecret
e5182efba139ab7368aa7410a848bfca2de2e789 Add pull secret to Header
a86f2596df185a0988b3021ad424b87cdba8548e MGMT-1724 Adapt agent to new bm-inventory repo
bb04967f06959c173db10cc572bcd95f246c6895 Merge pull request #39 from empovit/vemporop/MGMT-928
fa5662f54abbb8f39e95d4354baa28aed2dac138 MGMT-846 Disable GHW warnings. agent log and journalctl filled up with these warnings
124b96e5a05ae8755ebb8de9ea9e2b7c8c756551 MGMT-928 Mark host and port deprecated
e768b1103b3d7cc5ed0d9fbac080968c48760018 MGMT-928 Add full target URL parameter
7fbd9c25093ab6699541f57c5e8535a01f320bf6 Adding SetJournalLogging to journal.go
1860afc38844686d9572f8ad3f8650dae24f6148 Making from journal logger pkg, to use it in other repos
127b97ce2a265e6e5d346cce955934f78eb01993 Merge pull request #36 from rollandf/skipper
ab9f234e8408b60985fa6dbdab8a8e0a59cc8928 MGMT-1041 fixes
5d4304734af4ac712176ac1c3d7831a413513463 Update skipper.yaml with configurable env parameters
ff9e172c472deb58c763ce2ed6335c076834e13f MGMT-1083 Agent and other commands should log only to journal
2a7d6a23201a15944674bee8152aa7d51114e6ed MGMT-1041 host will stop trying to register after receiving 403 and 404
cdc05ef12276c0a9e4130db3ab9db11089649269 go mod
2275c3d5e0a1c6086c50133d9c130ead0bb24d94 MGMT-1090 Remove the HWinfo host operation
24fd6f6ef88b663069ee47665bb417a4c9cea9d9 MGMT-1442 When running agent on vSphere VMs, all VMs get the same id
627be4a1e73ff08a84259810e748556008996ca9 MGMT-1347 test
909c47d71335b1c0c763e7236ba58b312907241f MGMT-1347 sleep forever if cluster doesn't exists
3b4cb2de35405b0b24667b92090b4ce42ba4bd7b Fix test bug
1716ee2358a515bf449b56dbe6850aeefe2c1bee MGMT-1207 autogenerated
e4bb4efaa9084e0c2086e7ae8784975026ac4644 MGMT-1207 next step timeout is sent in getnextstep api call
5f40f98c1115281b6304ea467ddf3d03f782d52d MGMT-1219 Add free addresses support in agent
b5d3aff8fb348ca26c67be1f0c8f9fcc9d01a824 MGMT-1144 agent return discovery agent version It will get it as a parameter --agent-version and return it as part of the register-api
033cd185fc6d7a990d50904f908cc2b62f6af2c6 go modules
fd7bde71f1c2d24a84bfc1886c07ca127948b30a MGMT-1145 Move all agent commands to execute
d297e69cfa617f5823f83f0e172e2ba9ca1a76b6 Trigger release workflow upon tag push
7702ef769ae20c125fdf4728fb48369e22460623 Fixed syntax error in the release workflow
df8cb97c8b0768c197b771b4c55c7f721154f80f MGMT-1160 Added release.yaml to github workflow This workflow will build the repository container images upon git tag creation and publish it to ocpmetal registry with the matching tag
6c797ea79d63feec917d0bccb8904d4b7cc6e9f5 Updated files to use latest instead of stable
1cc91500452bd52d0bb2328864c9536a299a3170 Push to master branch will build and push to with tag=latest
8ff840b2c8cb2cb4bf68fcd70bbc1fbf13eedfde Go format
d4e72cb83cca83f5af3bd6113bfb79b19ba39476 Merge pull request #19 from ori-amizur/ronnie/removed-label
626bd4a5834bd3b6384d3d20e126785ece0f518d Removed 'tests-passed' label handling from github action'
e34292732dfb5ccd3845b4ec2cdd03bf511e1afa Merge pull request #18 from rollandf/license
b9584a4d60d42b16d4f98e125a890e50aef2d9d5 Add Apache 2 license
c8bd0a7e64304d0de6f28d001f83e93ac7db0c0e Update README
81adf5d327dde36f555c20d8ac3bb5291b59b606 MGMT-777 Support journal logging
7c3deb672660ce7f5496cf51e2e8f670522f84d8 Updated subsystem to use an image from ocpmetal
f912fd980a4d0131dd9bbe6b4682ff67e959125b Get the inventory image from ocpmetal
fa941a3bde6bdd160194c6379fe730ba2ec5dd18 Updated makefile to use images from ocpmetal
551eafbb1581e8e73fbe7ac7ab5a9dd199625d9b Publish inventory image to ocpmetal
b05c3492c795cfec25ec78bfb4f296ff77e64f30 Updated image-push.yaml branch to master
99d8ef627a576165f9460cea7cdbef7ff11692eb MGMT-1029 Configure git action to build and push the agent to ocpmetal Added image-push.yaml to githob workflow
d89e6d873419efbad5f691d1a2b5107006704789 MGMT-688 - New inventory structure based on ironic python agent output
585119048068fac6dd8e4d65bb6ccc3d2e0fcdde bm-inventory changes for MGMT-688
c4fbba1b5fa22b7b37b08ec1ccd7a97b17cc51d1 bm-inventory changes
5ddff6ac1ba1d03f5b275a0c3007b17ab55d305c Changes as a result of swagger changes
1504f7b8f0b0d06908c50ac89560eaf13c6e9830 Go modules
10f3e6f0e5b48b8082f2cbca7c21c4bc46572e9c 1. Remove loggger from context 2. Add session object per query session that holds the client, context, and logger
42c6f093e472ebb0777a41fcffa5a7ce01f08a7b Go modules
b08470cef989d95d7a8c4ebcca8b2b69b1fd2579 Merge pull request #9 from ori-amizur/ronnie/action
075ccd6a7f9cd9f5b6ba41c7cbc54bbfdbf2808d Changed setup to python 3
3d987dff09132791ab84460a296d3fc0a94a49a5 Added github action for testing
0a4b7920d685850a6ecc4ac719c8eead423423da Update README.md
7206489716cf65832760a368613bdf5c4519ddf6 Remove uneeded function in subsystem
09a2dd339062b8c31fd94ed13ac28c619a7de752 Add request id support
586c191a800300b2de67a6d62630798ae58a6738 Additional tests
d629bc93d3f6f73bbf4efea641043c570256af8c Go modules as result of inventory change
ab33031be59daaa7a468485e7e9eb6e41f3b1aa8 inventory swagger changes
893a078cc39d2156cfd240ab6b9f8e70d5ee4d4a Change memory units to bytes
55d65a8c4e2a7a6ca498bf6b40e0c9e1bb56817d Remove uneeded log message
e05d994ac163367a38a5468e1e57d1f1f4a713e8 Additional tests
35a901b4a49bcd042d2f03d381aa16ebd08367c0 Go modules
72cd92dbc46535d6ae8e7083b7af40e610f4394e Add subsystem support
f4070955dbc4129de1d110e63d4da4d9958e43c7 1. Rename introspector to agent 2. Create additional contains: connectivity_check hardware_info dmidecode 3. Agent to call the dmidecode container and not directly to dmidecode
2cb5a819c336dc222e14a0d3ea471f90cfe1a962 fixes typos
e2f503e117a5305d8e67121264175bc7135ad312 change hardaware info to hardwareinfo
7a6b82d6326242e3ce3d564f4b9e4fb6e109a74d go mod update bm-inventory client
e721edda0aefd545d7a58ba5fac1d695b3549a19 New bm-inventory
70b7c0a0567df1a615f246cb488303eaa248a585 Adapt to swagger changes
2217ed35e12fb7739dd261ae129ff388c06e767a Execute implementation
936ab528b26f7abb1f98a3ba2a2fa5f644801072 fix makefile missing service env
d06748f7ed898c7daccfaf2798b03a3670dc4a8b Rename src/commands/node_info.go -> src/commands/host_info.go
bd47a235381083e355b5b5b26c7c223fe62a4a8a Change Node to Host
bed164a286dbd72e09a938acb16ca49f0787420f go modules
ac622b4e58363646967904cc7113720a61b1d632 Supprot chaning SERVICE target with environment variable to change it just export SERVICE=<your-target-image> and skipper will work with the new target
59ef3d58bbd677ff2f1b238d6b017d181dd9a112 Merge pull request #1 from ori-amizur/michaelf/skipper
5ac521fe338372f3fe5aa9776ba43a51def31f21 Default to building the build container in case it doesn't exists
d27f59640247c93c0f203952c9d40363d317842d Fixes to nics scanner and connectivity check
d20b7ce04c6835baf08eff9047cb625f05e2a67c Adaptations to swagger changes
123db1272d3d04c0b2134d9e3842da68c2f6298f Added connectivity check
164aa6f6c5219556e99d2211b5ba90c2b6da9804 Periodical commit
06549d6868718f22d46212ecac72bb0197bd5d78 Project reordering
e321184f3bb0f5e3166bc9320be83743a9a1278d Periodical commit
cd1a8f4767addeb926b1d6fcbff8fb23f4dc2f10 Periodical commit
e7e85fe4b8187de033be53988bcf10e13e72e67a Periodical commit
d87f3ad07ed1306363724f55ac88521345f60752 Second version
d53eb866bf9048c461ccc82c086fe1041cd641be First version
```

Status: Fast-forwarded successfully.

### Branch release-ocm-2.5 -> backplane-2.0:

New commits (first branch sync):

```
e292223d31c003f3249e77966a7299af59fe06bb Bug 2081282: Implementing new service-agent protocol on agent side - backport of MGMT-7530 (#347)
021d5e78200325efcdc9005d9181c5e10744b08d MGMT-9884: bump assisted-service version (#325)
94f667c8d2b86074336d37a2f68d0fabd9f62f6c MGMT-9344: Delete Jenkinsfile (#311)
51582c5f52e9c22ca1e19fcdff122141ec1e4d2c NO-ISSUE: Bump github.com/thoas/go-funk from 0.9.1 to 0.9.2 (#310)
d05222663c08a61082e0b36e9832192443d8a9de MGMT-9358: update assisted-service after split to submodules (#304)
5f5b002736c8b8e7c7125756c748efdc30166db9 NO-ISSUE update container golang version to 1.17 (#308)
a9e4f3999510bf95e000a496c43bc37ea7457c3d NO-ISSUE: remove .ci-operator.yaml file (#307)
add5ab0b01cdcb8117acf4b574fc488c5c437c7b NO-ISSUE: replace .ci-operator.yaml to use local dockerfile (#306)
4fbd870ebd146094b31f99835841648c25a3b3b8 NO-ISSUE: add ci operator file (#305)
ad17f8e1a5607df93672271b680ec045c852c044 NO-ISSUE: Bump go-openapi/runtime to 0.23.2 (#302)
5de8ce7764d22435a031efc14b1370f19ff7626e NO-ISSUE: Bump github.com/jaypipes/ghw from 0.7.0 to 0.8.0 (#267)
e36b05c9c8251350eacbbca320c11ee5fc027631 NO-ISSUE: Remove small timeout subsystem test (#300)
7efd8892e3441bd9ede239720b4cfa7b4350bfa1 NO-ISSUE: Don't delete the subsystem_agent docker-compose image every time (#301)
9e035f47f2fac18e3487ac3768795558e269a37e MGMT-9481: Support linode serial/uuid (#298)
6a81a61b7445765d0fc484e3f030047b49ec237f MGMT-9344: Return non-zero exit when subsystem test fails (#297)
5dd71705eec88800d595c4805974402942571d20 MGMT-9396: Fix UUID fallback (#294)
b656f9eb2c3a1f45fcd9e58b3e8b1924c1ee1130 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.21.1 to 0.21.2 (#291)
ff0baa554db8fa8a3865c7eda74cda931e1fe591 NO-ISSUE: remove Jenkins publishing step (#293)
0830bd09a7d8a8472587872b9ee6051b57732a6d MGMT-9189: Publish coverage report (#292)
b79b5d775f6ca3c6a30bb35541752026cd7f87cf NO-ISSUE: Bump github.com/go-openapi/swag from 0.20.0 to 0.21.1 (#289)
f13de8989571f3a61a9ff194a83655620905375a MGMT-9043: Set multipath device as eligible (#283)
52b9970365d20c197cd19070b40398d6aac89fee NO-ISSUE: install smartmontools from stream8 repos (#287)
206307c1d777ed4179ab3c8b35bf6525216a2bc8 MGMT-7813: Reduce smartcl verbosity (#282)
d2a9f98291ab47a8af4f46f1927290711e621625 NO-ISSUE: Bump github.com/go-openapi/swag from 0.19.15 to 0.20.0 (#281)
93342ccd698829d38fa121f13b6567aadf40da73 NO-ISSUE: Bump github.com/onsi/gomega from 1.18.0 to 1.18.1 (#279)
42278a57f1ff6a255a10b01bba6856426ae2dd7c MGMT-8752: handle ocp router 503 errors (#278)
e4bebc1e7106236a8a3befdaaed0729a49920347 MGMT-9040: include only Luks section of ignition in response (#277)
0317df2d10914815855a5dd8e8f7dea85eaf259b NO-ISSUE: Bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5 (#269)
7c4cfd1d731bd5e994cefd4f9cb239ccc9f56787 NO-ISSUE: remove redundant GitHub Actions files (#276)
6ee312d9748e9164d4c80d7ebc18f23d43fdc83b NO-ISSUE: Bump github.com/sirupsen/logrus from 1.7.0 to 1.8.1 (#273)
36f5c7862951b4a1f95cc03ffee18bbe70c071f0 NO-ISSUE: fix dependabot commit messages to include NO-ISSUE (#275)
13774bd07b77b37e6d02963f63fa56fc64ea14a6 NO-ISSUE: Bump github.com/onsi/gomega from 1.16.0 to 1.18.0 (#274)
b7af0d13bdd2c0f2c7901b6295f7ec75d16cc0fd MGMT-8481: Allow fallback for generate uuid from mac for kaloom deployment (#272)
8919643674e6321515088fbff336a546e2de76e4 NO-ISSUE: Bump github.com/thoas/go-funk from 0.8.0 to 0.9.1 (#270)
439b28b50ea4205cd55d47a865b434b2d272aa7f NO-ISSUE: update assisted-service package (#266)
57baa621a1c04d5bae4b2a7ac1822317088c28cc MGMT-8847: Add bf serial value to unknown serials in agent (#265)
c7a3a430fecbef64a89a33d8a9739ab9bd802500 MGMT-7428: return ignition in apivip_check response (#263)
e37c4190854d860f46acaf3e7019e992a4dd9406 MGMT-8623: capi-provider-agent fail to add host to hypershift due to API VIP connectivity failure (#264)
487be214c7d0521f50cd540e1260eec6c022961b MGMT-8424: Add token and CA cert to API VIP check (#261)
55d9252ac2bb120f19a7779b8f5a23ef4c1fe048 MGMT-7428: apivip_check - Accept in request header (#262)
6f7459cf58f72e921c3d011b5da68840261ad0ac MGMT-7847: Don't check verify CIDR in the host (#235)
e72724636866f3421c9d5600867089b4c4e2a1ad MGMT-8422: apivip check remove suffix (#260)
51fca8bd01227bd82f6418084d7cf49811c1d04a OCPBUGSM-37106: List only physical disks on inventory. (#259)
1b51ecd2786c0f56ceb8f2051fe0af4dae1f7173 MGMT-8294: Adapt assisted installer agent to latest swagger changes (#257)
720bfed358fc01f827413c4e95ffc0cfc127b616 MGMT-7941: Allow forcing the IP address and hostname of the agent in dry mode (#256)
60e82d05d8259184efa4772dc60dbb87537fa67b MGMT-7941: Fix agent dry reboot condition in wrong code path (#254)
de31b85976055ad71cb9f689be2b6db73086e470 MGMT-8163: Logs sender logs should be printed to stdout (#253)
1e818b2737ca41b8cb6121ed718d95f7984a375b NO-ISSUE: Logs sender lsblk unknown column error fix (#252)
bf66b232529b5023f29eca554f9ed6c51b2a6044 MGMT-7941: Introduce dry mode to the agent (#250)
53b0eacfa1474d847ed6297dc234bafc34241305 NO-ISSUE: Inventory accepts Ghw Chroot path (#248)
ea4b2816abab5dff8536b03f2c56cb84a7a33738 Bug 2017502: don't return error from Resolver in case domain not found, (#251)
761e669621bbfb92fe443708d522b97910b639e2 OCPBUGSM-34971: container image availability command should not exit 0 if it failed on one of the images (#245)
dda746a296408e83e52a98d7db19b601d53c39c9 Bug 2012839: Agent should use V2 API for HostLogProgress report (#246)
37a5214e61853797883c5fe8e37a11d533943d24 NO-ISSUE: Remove user yuvigold (#244)
7918e3bf38a5001d60778d7b39f405b590026307 NO-ISSUE: Removing \n suffix from TPM version. (#242)
65d2e6db57cc2dc895baabc9ee3b12c195c19974 Bug 2011300: Agent should use V2 UploadLogs API instead of V1 API (#240)
669a2d7d699f2557a627eb949975d0e81ac1c565 Bug 2009241: Agent should support receiving InfraEnvID as part of SendLogs command (#239)
422b94c1f73118d7ecf272605a331b6c66f48fcc NO-ISSUE: Add lranjbar to OWNERS_ALIASES (#234)
05e460bca5e86feef4c48a772b3396c5ee8b1a49 MGMT-7761: Switch to stream8 (#237)
38b5a5f880866b695a3ddd9b80f056185a05b41f Merge pull request #238 from flaper87/flaperowner
763eaf7f5d263b4a3b013463329a4fd0e4d279d4 NO-ISSUE: Add flaper87 to approvers list
14870a7501549fa77bb04480d7c70caa036caee5 MGMT-7847: Add a deprecation warning for the VerifyCIDR option (#236)
4d39baf5fac3c28bb69458428335a3d540350904 MGMT-7457: Adding TPM version to host inventory. (#232)
d9a8a4aab778e0769abcf15eb9c16bd44bd2b683 OCPRHV-591: Add oVirt support to the agent side (#225)
60ac74ef05e45fd612222f3bd17f0b148d346d98 MGMT-7661: Add property called physical_bytes_method to memory (#231)
ad772bdcf765cc3a9aac387b769dc97b6651a39a NO-ISSUE: Add lsblk output to the log sender (#223)
e96269abbb1dcf3561dc414e4cf4da845709198b MGMT-5400: Get physical_bytes from ghw if dmidecode was failed (#227)
938df898fee740b2820d7afffde86b985506b24a NO-ISSUE - Add eliorerz to OWNERS (#229)
efe8ea006c178db1d8a6164262825219c9eb7fa4 MGMT-7659: Generate and update the agent (#228)
38136d7814a1c4f8ac498ffa5ce4c1598193d054 MGMT-7597: Remove ronniel1, and razregev from OWNERS (#226)
3d697f0b1a4988782205dd4cffac6b948d53d223 MGMT-7443: add removable attr to Disk (#224)
6c955e8319e0762c6c2b6f05baacd8b7d4c62d25 NO-ISSUE: Align IP protocol version number (#222)
b14d0a3e83e6da385006169aa6780e57b2f785b0 Bug 1990060: Host returns no routes with multipart (#220)
c1573868b0fd09f003d440c1834f4b41de6227ee MGMT-7407: Remove V1 APIs from agent (#221)
bda33e2f2fc9f6f04d46d6ac90d4f04a32604517 MGMT-7383: Add v2 APIs to agent (#219)
1d517b6cbfa1e9f71b41501b485de20f83121764 Bug 1975672: Parse GW nil as net zero (#217)
94d71302869c801daac992c811b6bb93e7b21269 MGMT-6977: Make sure that the image availability timeout is per tool run instead of timeout to pull single image. (#218)
38841dee2846214441576a19ded4f5a994f31312 MGMT-7210: Upgrade Go version to 1.16 (#215)
57afa1673f9328f840b102362aff8103f62740ca NO-ISSUE: fix OWNERS files to match group members roles (#212)
885f669df1d5b2ade50739fd0b78d0df0cd998c0 MGMT-6498: Remove filtering when capturing route information (#211)
8a8c4c4c4969b98286ed6ddb64c757f98b56af7c MGMT-6498: Capture router information in inventory (#209)
8d63a0ece1e669e679b1a44d1331213f3b8bcfb5 NO-ISSUE Add mkowalski to OWNERS/code-reviewers (#208)
2d07639aeff2c689390f6a48359505e66d181b1c NO-ISSUE: Add check commit script (#205)
30cdb974bb9f7e5dc1ae5bfe03ad6ed7cd071df0 NO-ISSUE: Fix linter errors (#204)
b04b05caf30f4b15ce4c2ed34cda3d4d36c00160 Publish tests junit (#202)
f5dd8915b1fda0408a1a74226050ca79d7f0faf8 MGMT-4966 Display a better message when media disconnection failure occurs (#197)
799e4bd24b12c56808d2898f87a431f53e481db9 MGMT-6668 Invalidate agent cache when there is a problem to perform get next steps from assisted service (#201)
5f5de4df21ae843517d1348adbc031c9b2c74c78 MGMT-6656 Sort connectivity check replies before returning the results (#200)
0827f184fbbf9302b31484441f5dd3e16d73fbd4 MGMT-6484 [WIP] Create cache for post step reply api calls (#198)
72b14c873597f3883eab9af308fb803b344af2d0 MGMT-4327 Remove old FIO tool from service and agent after the new tool is in use (#196)
3eb41884f8d7eee77e9cbac5647918149896f18d MGMT-4718 Capture network latency for L3 (#187)
ae01c7568822924689149b6c3827ada5faa9258b OCPBUGSM-27088 Filter out ipv6 local link addresses from inventory. (#195)
3d012cfc546213b4c064fef5bb4a4802e84fbbf9 MGMT-4142 Using ghw to detect GPUs (#193)
e217062c630886a821eefecaa3fc3ab62cc1a0b6 OCPBUGSM-27560 Duplicate installation disk. (#192)
42d49b73098ae12d1879768f01c390fa952d1cae NO-ISSUE Bump github.com/jaypipes/ghw from 0.6.1 to 0.7.0 (#190)
32ba879c3e0e7586a245618cdf45d7c041f9f25b MGMT-4397 Fix command args of disk_speed_check (#191)
299b4b3a8179a816403ee1882def3f5786979727 MGMT-4142 Detect GPU devices (#186)
7490d17a267d50522758ebcbe4666b8f85fc0e75 Use 'Errorf' instead of 'Infof' for step failure (#188)
4ae8931b8dad082b4907f270b738df7d9b2b6254 MGMT-4397 Agent changes - adding new tool for disk speed check (#185)
4b8a77a7db432763c508b11bdd23be556be2197f MGMT-4117 ovs logs gather (#184)
d28226138b29a122d2bae5108e81cebf693bb105 OCPBUGSM-26414 - changing the filtering of the network interfaces during inventory and connectivity to allow support for bonding and vlan interfaces (#183)
edbaff3f6b1343b6e51c64d461923ac592820476 MGMT-4048 change disk id to be the full path of the by-id link (#182)
0cf6d9f18cd2e4294a550bfeec0e2c7afdf0715f NO-ISSUE add michaellevy101 as an approver (#181)
363723f893eff0fb011a81c4522d048610a4971c MGMT-4052 Add id and by-id information to the iventory (#179)
3b8c3709294ea64e89c3663106c99d4ccadda204 Wait for image availability response in subsystem test to avoid race-condition (#180)
d0a02fa803847584117c2e6802ebb399207cb0c3 MGMT-3854 report log progress (#175)
3aab80c38d5779c4bfaf258e5924a5ba0112c7c2 NO-ISSUE disk unit test refactor (#178)
27aca022c9224502659a0cb5f80e53d3a12e5284 Fix ginkgo skip flag (#177)
7482b99b25be9b36c0731ea23be65e216194e385 MGMT-4346 Collect logs in Jenkins Post (#167)
bc4cadcd5542715d021ab5fa37e557ec5249216a MGMT-3869 - Add domain resolution command to agent (#176)
49e34b56a65942fc7b128fbc8fbd7897c1544db3 MGMT-4053 Add output of listing the 'by=id' and 'by=path' links on the agent to the mounts.log (#171)
dd888746f393a3a9716012d8cb63592e3615ad9b MGMT-2925 Clearer error message when next step crashes (#174)
566fb848f1edebd2d1f725d6ecf88d7ee6d05396 NO-ISSUE Add git_revision label to the image (#173)
4968d22704d8c5fe78dc71d373aff830eb3e870c NO-ISSUE Switch registry.svc.ci.openshift.org registry to public registry.ci.openshift.org (#169)
d0b71dd6ecee9068fd087804816580678ccd2ff0 Fix IPv6 CIDR based on route (#168)
957e2a5c6965169e830a1abba7e839e2475bed83 NO-ISSUE - Upgrade assisted-service to latest version (#166)
68618ca607d10d7edb4c653254b33f7bb52749c5 Update dependabot.yml (#165)
b628c66db1236dfe242a1dad36771e59130298eb Bump github.com/go-openapi/swag from 0.19.13 to 0.19.14 (#161)
7dde6be6720c31ac077081bad9908e661f903096 Bump github.com/onsi/ginkgo from 1.14.2 to 1.15.0 (#159)
184208775aefb0599766a9a00f33bd475ffb6cb6 Bump github.com/onsi/gomega from 1.10.4 to 1.10.5 (#162)
c0aa46cf0d287b079f7d12f43fe268292bf638ac NOISSUE: Change Auth Token missing message (#164)
a9cb0d28121ecff43f70395f48790abcfcd6dc3e MGMT-3526 Add failed_to_pull_timeout unit test (#158)
1dadfbf9757764ca3b3974ab7ff6cd3fe4f71469 MGMT-3526 Add container_image_availability tool (#146)
0bfedc461084f83c2f2b7464c25eda0ecceb4d40 Add docker ignore file (#154)
6710e9d2a6bb59237e00ef9051340beab2afc8a1 NO-ISSUE - Human dmesg timestamps (#151)
c69818898255f6870b425ff4783f4dd8077c55c4 MGMT-3315 Multi-stage agent Dockerfile (#148)
94cae07716c035bf81b46c9f9804c40c7c16ce55 Bump github.com/google/uuid from 1.1.5 to 1.2.0 (#150)
53bceb5ea502f28530697242f1e4e970a6ed3da2 MGMT-3390 - Added lint and format - for now, lint not performed automatically (#149)
5c709826070bb85a8e35b0d5fbec44c2ee083574 Move cloudctl/dhcp:ubi to cloudctl/dhcp:micro (#147)
ee0384801d487bcf26b746bc2a4d3a663af1e45c Add generateNsenterStep and generateDockerStep to subsystem utils (#145)
d9c79b7b6f69ed000eb835936b07eafead8b93cc Bump github.com/go-openapi/swag from 0.19.12 to 0.19.13 (#144)
3007163da5f4ca38adfde3539af862f88af2c8d5 Bump github.com/go-openapi/strfmt from 0.19.11 to 0.20.0 (#143)
c4dfdcc2f0598524331c5de0b0ed557eda45005f Bump github.com/stretchr/testify from 1.6.1 to 1.7.0 (#142)
dc3602e9c5179ba94043964a78271cd8ff27ab3c Bump github.com/google/uuid from 1.1.4 to 1.1.5 (#141)
36db835769867d760979703871a2a30d17daf603 MGMT-3463 collect full journal logs (#140)
a2fda3ca4d2ec8c3bb7730bed0e3d686ba16cec2 Bump github.com/google/uuid from 1.1.3 to 1.1.4 (#139)
21a4e3a1b35de93f989a69514a36f2df71ac4169 MGMT-3458 Send step reply from FIO perf check (#133)
f017b4226d79bcd0148fc1c3123a3269b3c9bc27 Fix dhcpd lease file issue (#138)
79ed6225e0bf5a8ddf3c78c4d2e4fad44b6eb322 NO-ISSUE - Add omertuc to OWNERS_ALIASES (#137)
e7dd7b18c3310acc25749aa02c5101ce1f1b319f MGMT-3456 - Agent will now report whether a disk appears to be an installation media (ISO) (#134)
eed3a59db39982a1394d279815afb7266bc81b85 Bump github.com/google/uuid from 1.1.2 to 1.1.3 (#135)
610f11613cc669f56a17428f5a9fc9825844f983 Get test images from quay.io (#129)
74e13887e1bd04dd61c9920d92bf372015dbae1e MGMT-3026 Add log of FIO result (#132)
2da45a368d3b99ea680b4b33e392a813e910be4b Check for expected NTP Sources on NTP Verifier subsystem tests (#131)
28672290ea3e5fc59f9bf279482ad416bb8d8de6 Change resetAll order (#130)
02fe461968b79755ea58cd78295b765290475ed9 MGMT-3194 Use nmap for L2 connectivity check (#124)
74c2c6013a2ec17214ebed8755f303ccdb785ee9 Bugfix NTP subsystem tests - reset agent (#128)
6f281de73f7f1afd196c9a5e6d6674817a4ed13d MGMT-3026: skip slow disks using fio output (#119)
a070b977d947bfaeea00db0975758e17427b0252 NO-ISSUE fix docker login timeout (#126)
571582f1d3b9c4baf0e542409688c6629f2ff52b OCPBUGSM-22485 - Agent will now consider Xen HVM domU machines to be virtual (#125)
855e2a5d713768f8f9b981d06efb93308a1653ac OCPBUGSM-22486 - Assisted installer agent will now consider AHV to be a virtual machine (#123)
aa8dba6e643ca316fd191b6104a07819cf1ebb0d MGMT-3291 - Show all disks - mark eligibility instead of filtering (#122)
e53fd3f80ed303b8c1645fb9b0c3dbb146a952a8 OCPBUGSM-21553 NTP tool reverse lookup for IPs to hostnames (#121)
1c694228073656d9e017a47f2d5d6b5ccfaed6c1 Add GOCACHE to skipper.yaml (#120)
6fc79c454f08e648cbf5f0a6277c3b461b789b15 OCPBUGSM-21366 Support comma-separated NTP sources list (#118)
c7b6b54cf117164febb52ed7cfcacabdd75f2104 OCPBUGSM-21434 NTP: Ignore adding server failures (#117)
7a3d06c5bc56de9a59c6e62dbea15b19f5d7303c MGMT-2858: coredumpctl - use priviliged (#116)
1152832b0b44e06e7a911b78545a86d28afb273d MGMT-3262 Remove app-sre images (#115)
7798058ea9e2fd0847f42776ffc10aa58a878afc MGMT-3257: discarding disks of type ODD (Optical Disk Drive) (#113)
e2dfdf0ed9420e7da5e58fc65a16d778b12e074f Bump github.com/onsi/gomega from 1.10.3 to 1.10.4 (#114)
96f221c34b18c8683e5834a19200bdaa4b807118 MGMT-3211 - Never ignore smartctl, regardless of exit code (#110)
9907fc1923ae3bcfc7d3a55656c954b5480ed6c5 OCPBUGSM-21377 - fix check api vip: in case connectivity does not exists, return code should still be zero (#112)
3824c62c7faf82968d1dc26dd727c3b39fc159d4 MGMT-3012 - Add mount and volume display logs (#111)
dbf9357a634a71eb3035665fd1d11e571b1850ad Bump github.com/go-openapi/swag from 0.19.9 to 0.19.12 (#95)
0fa8d77664c532958199b11c6a044e19df1092c8 Use quay.io/app-sre/golang for build container (#109)
f8070bf0fdeab765d88450a3621723b17293c99b MGMT-3120 IPv6 connectivity check (#106)
ff08b27ebd3a1b8c3462546cd31a6bb7e8cbf6cd MGMT-2858: send_logs - use coredumpctl (#108)
843a8cf20f2f2ec85516db4bd7c543b7a8b673c9 MGMT-2858 LogsSender: added coredump and dmesg (#107)
aebd94105b4ed6442f21a7a26ab4e40eafd936aa OCPBUGSM-19005 - Print step output after step execution fails (#91)
9b98329153609994da4d0080dddb21bac8b210a1 MGMT-3088 push images to quay.io when we build from branch for installer & agent (#104)
4eaac4b1a48688f5d68f38734966903a524e1f88 Bump github.com/google/uuid from 1.1.1 to 1.1.2 (#79)
e9d687e7adb341751304b8ecfca28a50df31a774 Bump gopkg.in/yaml.v2 from 2.3.0 to 2.4.0 (#105)
e829efc192dd3ffd76b54925c190449cb0baaae5 MGMT-2777 Adapt IPv6 network prefix by using RA routes (#99)
42c062876dd442702497b6541ab190debadaa7c3 MGMT-3033 - Use newer smartmontools from the Fedora 32 repositories in upstream Dockerfile (#102)
7b2f278d8e3c2cf45d3d1d04ef0f971b84ecd802 MGMT-2951 - Will log reasons for why disks were skipped (#98)
5f6903e972997c4fa4c3ec9666618f6a8f632d7f Extend wiremock setup timeout (#101)
fe23eb50d5579bf334d8096afa271d89fb9152bc NO-ISSUE: Changing the order of logs gathering. (#103)
618c94b98ab7e093d721cad756ea460e046f084a NO-ISSUE - Remove masayag from OWNERS_ALIASES (#100)
0a4da3fe7c21ea0c40141ac7d6498fccdfd72bed MGMT-3033 - Populating S.M.A.R.T. field in inventory host disks (#97)
8a01d229f32d575a18033611451fe8d5571bbabb Bump github.com/go-openapi/strfmt from 0.19.10 to 0.19.11 (#94)
8015175352d0bb8e11887a820203adc5953d3e13 Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#93)
262fc055ee4c1930f736568f69389310f9ec89c4 MGMT-2678: Supplying non-bootstrap masters IPs to installer-gather.sh. (#90)
6fa33e27761ea361a03c5fdb5067b92692df684d MGMT-2219 Set mac address as prefix for unique hostname (#92)
da9f50d0ad6b03674b2e8118fed13f3ae781ef9f MGMT-2322 Add ntp_synchronizer executable (#83)
c3194394a014cfaaaa7ab585f5fb7b833822914f MGMT-792 - Updated assisted-service, replaced lshw with ghw, populated is-vm field (#89)
d2b42027c0b1b9f4deab324cb8e64d460bfb8943 Bump github.com/onsi/ginkgo from 1.14.0 to 1.14.2 (#78)
30abab5d291715b06909a7dbba9b3c3257a81874 Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.10 (#86)
9307b0d10d128a446f2ba958a17749d556c94a33 Update dependabot.yml (#88)
e3ee9677c5a1a810945bf393d1f197c1c15c041c MGMT-2440 Fix the errors in inventory when trying to get BMC information (#68)
7ebf6037422d4e19958c9e1488704e74c28d643d MGMT-2769: allow bonding interfaces (#71)
6e22aca3b04b24a8981766c252733441a634ac6f Bump github.com/sirupsen/logrus from 1.6.0 to 1.7.0 (#81)
69ff13046658712013feee8329709e3322a59af3 Bump github.com/onsi/gomega from 1.10.1 to 1.10.3 (#80)
515ddbe7bc1fe551d92499f356e487c5c1a87557 Add label downstream-change-needed on Docker files (#76)
84aa6878fcf3b8df5c8876bd2bf13b10a337fb91 NO-ISSUE add osherdp to OWNERS_ALIASES (#75)
0f0760d0dffa5917d8b87f6aae338f1a880c3971 NO-ISSUE update owners file (#74)
a959f7eec75e2ff3b10f8f4538d9f92d57738167 Update OWNERS
c2aa5c2701a2e219dc4b1e726383cde74354e38b MGMT-2592: filtering media disks from the inventory (#65)
3aea65b0ba71f6634939e6233184445066bd93a6 MGMT-2447 Exit next step loop on flag from API (#55)
1d6d1c92aedcd8f88843caa3b2fe00f388ea07f4 NO-ISSUE: Adding to logs the output of /usr/local/bin/installer-gather.sh (#72)
39dc06ac7dcb5335dbd6771f4a12a2d90090a758 NO-ISSUE: Configuring privilege command to run using host network namespace. (#70)
27d45ae54bf9bf0cf12a88c60e3240bd63efc1de MGMT-2213,MGMT-2380 Bring back split into registration and next step (#69)
a85739e83d21a6868d372baef4c1caf3cd33a28c MGMT-2659 DHCP server changes the VIPs addresses after installation has started (#67)
ff21bc8686cdcf0a18d26264798afcc12a7d1df0 Create dependabot.yml
7c16bdbd1f410eff3ae47afe135fd9ddca76ebdb MGMT-2578 use centos which doesn't have the defect version of nmap (#63)
eb3ee583a779f7b9dea9c43a04783a64c8618200 MGMT-2347: remove output from log message if step type is free-addresses (#53)
85a88bb5cb18c3f065260a56222a3a4e4e2b82d3 MGMT-2431: Adding 'installer-gather.sh' to logs_sender on failure. (#64)
3ad7c4de1e09392dfcd59e12e87b297ffdafce34 MGMT-2576 Bootable info not collected in inventory - Add file package to dockerfile (#61)
3e84ac7bf47dd5c1995fccf2d9be63b0c9a236d1 NO-ISSUE revert to fedora 31 (#60)
cffd8954c255559fd56495c03f56c7e98c9877e3 MGMT-2069: handle getting 409 from server when host tries to register to a cluster (#52)
2e2b6a27b4a3fc9dd9de0f8b5891d1ebe03a58f0 MGMT-2479 Revert splitting agent into register and next step (#58)
d99ae31adf433d2ca5d6496a1cde66de8bf9480c MGMT-2420 Add bootable flag to disk in inventory (#54)
1616c72ceaddf82d0e8986367b045b02d32a5164 OCPBUGSM-18605 Clearer dhclient timeout message (#57)
5115e7b58fb8d8f708a6b0ac1cb2738f2bf48c96 MGMT-2380 Update README (#50)
22c33e020c803dbfec41e6875ed7e6a44883b558 OCPBUGSM-18606 Improve log messages for failed step replies (#56)
6fcfff8bfd66bcf05fb0cec2ca609be2c518a578 MGMT-2213 Split agent into register and next step (#47)
033928931edc70e675ac5a226018a70c365430ee OCPBUGSM-19005 add log with StepId (#51)
11c372356b59a0ddb086e4831b6526c898d47ad7 MGMT-2318 network CIDR verification to API VIP (#46)
855933ba95ec34b62197bba7131adf2c8aaaa010 MGMT-2398 Logs upload is broken due to new fedora-minimal (#49)
1bc57a6bf2f9e91746e0f982112d67e7a4f43768 MGMT-2075 - API VIP connectivity check command (#38)
fa2618ae5a8b5a3cdfeb99c7ee084f6f2dff512d NO-ISSUE dummy commit for DS images (#45)
aa52cbcaf97e03ce871fe023da7f64ebaada9682 Use gotestsum tool for testing and publish junit on Jenkins (#44)
a2898461413b5ba6ce6d9e08a985d3398da9067a MGMT-2279 If Auth is disabled Token is not needed (#42)
39e36047915225021fda98d95ae611a4157bf893 MGMT-2342 adding timestamp to inventory (#43)
382c69e29d29e74e495dc13ef392d6f5fce2fe91 Notify on abort (#37)
06a598d8c162761c4a02ce8a7801864bb106fc6b OCPBUGSM-17431 update assisted-service client to support 503 and 401 403 for all apis (#36)
28cdc326ceb0a58a06e6f2a9227edcb329c5b2cf Update OWNERS file (#35)
ff0732f58da697c2b7c35530b282750838461cec Add timeout to wait for wiremock in order to avoid test failures on weak machines (#34)
c20bd63e42036d0c116f82d9f97f6bd371f7a1c6 Improve logging.  Session #2 (#33)
fa7f3a7fa597aaa3098eb7a683453e64598f3bad OCPBUGSM-15958 Improve agent logging (#32)
1c5b2e8e0ce18b3151eb9f0c15b0a8aa05a0cc56 Add additinal timeout for getting inventory so subsystem test could work on weak machines (#31)
5672e2c5534f8b2b42237a199d3f3946a3ec3c92 OCPBUGSM-16626 fixing typo (#26)
50e6a55cf8932e17f11f07bcc803416e78f86fbc Add FOCUS env parameter to skipper.yaml (#25)
b2df63af339ae700faa0c30687f68261c3201215 Switching wiremock to an unused port (#27)
d9d34e690c294878721bc9633037b3abef9af8a2 Image build with network=host (#29)
1430b38aa8672f4e7b7c2d18e7e6fa5da7c74312 Update jenkins file (#28)
c786e23a9786042e7968d0ff47b1b039a1792679 Update Inventory client and test for 401-403 (#24)
7a45790bc3a82476a242cf7b9c654d7d6770b080 MGMT-1680 Adds discovery_agent_version header to agent API calls (#17)
4a3b33ccbb4112e3ccc6862c0dfecca2820801a1 Adding tar to assisted_installer_agent image (#23)
19e6e1f9a76de9795a31a2ab17a6180aa9377c4c MGMT-1912 Remove docker install from Dockerfile.assisted_installer_agent and add Dockerfile for subsystem testing that adds docker installation (#22)
a1cabadfb77c5880779f7f1a34c856256983fd57 MGMT-1719 create dhcp lease allocator (#20)
699cbbd0f40ffda29b3ef26cdc297b63222d03e6 Merge pull request #21 from openshift/osher/notification
fb4e77c398820073c75ddbc05a6cb58faf5d86d9 send slack notification
14be679db6cd6ccb649485f74800cfd77d83f940 Merge pull request #19 from openshift/osher/jenkins_file_notification
273b4d3fee0eac7c616181c59eded88e2c79c545 Igal/upload logs bootkube (#18)
25440f96dbe8e41278a43e2a54db0f2f638cddf0 add link to notification
0a05fca9b5e72dc6bdaaad6ea6d4560f8ddaa91d Avoid subsystem failure when running on system that only virtual nics have IP addresses (#16)
009ddae05f09ddcbfefd674ea50e9e4112312525 add notification when master fails (#13)
b27895b701481015f2c78720a58043712d9703d7 MGMT-1880 Change path inside archived logs.tar.gz to logs_host_<host_id> (#15)
634d5048eb4a08ec628892473971d46318d6a228 MGMT-1876 Add insecure and certificate flags to logs_sender params (#14)
8164292b43b502014958a4f5fb216398970d16f0 MGMT-1861 Remove the warning log from agent about not being able to find motherboard serial number (#12)
6dbef262aaf793d0f991cbe7ebaed2127f4a3612 MGMT-1713 Remove deprecated host and port parameters (#9)
fad95178306c817cba3a2f63f7626e02af201ae1 Merge pull request #10 from openshift/osher/agent_update
26393f600034c118850e841ae493ad3cb19b096c Update agent to vm
bc9c7b899b8ad392922794d32735909dfb266fc7 Fixing don't delete flag (#8)
78ece80bebbea7c71ae72ac93f5bf52cc2e153bd Fix for delete folder after logs are sent (#7)
fef78b81ce26868f7db1f9067b3766146cf4dc8a Igal/upload logs (#4)
9912d24f0bbdf56056d9ba9184d20535dfc96a7b Change README and skipper.yaml and rename build dockerfile as result of repo move (#3)
e577982ee8cf65e8b9971a5a7e985b2ff6a7da5a MGMT-1695 Support HTTPS transport (#5)
b95a4adcf90f3dc62f440091a8956f804fdbbd25 Remove space at end of image name
69b457ce9ab1a095952526e490c7bfe8703ac9c3 Update image name
5f5d7abef22ac8f8ecfcf4672919c9671a238d5d Fix subsystem docker-compose file to override firewalld network block (#6)
e417c3f1c4e586c7bbb80eab153fb328152bcbcf Added Jenkinsfile
121ae01642972ffa7e01ab2b4bf4fbae606507ad Fix imports after move (#1)
e551596e4ec62c612b3006883d061c9fc0a83e62 Merge pull request #46 from ori-amizur/feature/owners-file
f4df0b0ba838bceabeacbaecb6003a1a835b7094 Add OWENRS file
611d9a843fa1a5fcb4cdae3f0136da27760d309b Fix github files from previous MGMT-1767
ffcab4a55b02ba57476c7848cde3e8882d43790e MGMT-1767 Move git repo ori-amizur/introspector to opnshift/assisted-agent
2282ec0ee5f14edfedb98a39fbbdfcc52ade7b27 MGMT-1661: Ensure aws xvd disks are discovered
eb62f60ccc991dba791efbe706007ae1d97ba4c9 Merge pull request #34 from rollandf/pullsecret
e5182efba139ab7368aa7410a848bfca2de2e789 Add pull secret to Header
a86f2596df185a0988b3021ad424b87cdba8548e MGMT-1724 Adapt agent to new bm-inventory repo
bb04967f06959c173db10cc572bcd95f246c6895 Merge pull request #39 from empovit/vemporop/MGMT-928
fa5662f54abbb8f39e95d4354baa28aed2dac138 MGMT-846 Disable GHW warnings. agent log and journalctl filled up with these warnings
124b96e5a05ae8755ebb8de9ea9e2b7c8c756551 MGMT-928 Mark host and port deprecated
e768b1103b3d7cc5ed0d9fbac080968c48760018 MGMT-928 Add full target URL parameter
7fbd9c25093ab6699541f57c5e8535a01f320bf6 Adding SetJournalLogging to journal.go
1860afc38844686d9572f8ad3f8650dae24f6148 Making from journal logger pkg, to use it in other repos
127b97ce2a265e6e5d346cce955934f78eb01993 Merge pull request #36 from rollandf/skipper
ab9f234e8408b60985fa6dbdab8a8e0a59cc8928 MGMT-1041 fixes
5d4304734af4ac712176ac1c3d7831a413513463 Update skipper.yaml with configurable env parameters
ff9e172c472deb58c763ce2ed6335c076834e13f MGMT-1083 Agent and other commands should log only to journal
2a7d6a23201a15944674bee8152aa7d51114e6ed MGMT-1041 host will stop trying to register after receiving 403 and 404
cdc05ef12276c0a9e4130db3ab9db11089649269 go mod
2275c3d5e0a1c6086c50133d9c130ead0bb24d94 MGMT-1090 Remove the HWinfo host operation
24fd6f6ef88b663069ee47665bb417a4c9cea9d9 MGMT-1442 When running agent on vSphere VMs, all VMs get the same id
627be4a1e73ff08a84259810e748556008996ca9 MGMT-1347 test
909c47d71335b1c0c763e7236ba58b312907241f MGMT-1347 sleep forever if cluster doesn't exists
3b4cb2de35405b0b24667b92090b4ce42ba4bd7b Fix test bug
1716ee2358a515bf449b56dbe6850aeefe2c1bee MGMT-1207 autogenerated
e4bb4efaa9084e0c2086e7ae8784975026ac4644 MGMT-1207 next step timeout is sent in getnextstep api call
5f40f98c1115281b6304ea467ddf3d03f782d52d MGMT-1219 Add free addresses support in agent
b5d3aff8fb348ca26c67be1f0c8f9fcc9d01a824 MGMT-1144 agent return discovery agent version It will get it as a parameter --agent-version and return it as part of the register-api
033cd185fc6d7a990d50904f908cc2b62f6af2c6 go modules
fd7bde71f1c2d24a84bfc1886c07ca127948b30a MGMT-1145 Move all agent commands to execute
d297e69cfa617f5823f83f0e172e2ba9ca1a76b6 Trigger release workflow upon tag push
7702ef769ae20c125fdf4728fb48369e22460623 Fixed syntax error in the release workflow
df8cb97c8b0768c197b771b4c55c7f721154f80f MGMT-1160 Added release.yaml to github workflow This workflow will build the repository container images upon git tag creation and publish it to ocpmetal registry with the matching tag
6c797ea79d63feec917d0bccb8904d4b7cc6e9f5 Updated files to use latest instead of stable
1cc91500452bd52d0bb2328864c9536a299a3170 Push to master branch will build and push to with tag=latest
8ff840b2c8cb2cb4bf68fcd70bbc1fbf13eedfde Go format
d4e72cb83cca83f5af3bd6113bfb79b19ba39476 Merge pull request #19 from ori-amizur/ronnie/removed-label
626bd4a5834bd3b6384d3d20e126785ece0f518d Removed 'tests-passed' label handling from github action'
e34292732dfb5ccd3845b4ec2cdd03bf511e1afa Merge pull request #18 from rollandf/license
b9584a4d60d42b16d4f98e125a890e50aef2d9d5 Add Apache 2 license
c8bd0a7e64304d0de6f28d001f83e93ac7db0c0e Update README
81adf5d327dde36f555c20d8ac3bb5291b59b606 MGMT-777 Support journal logging
7c3deb672660ce7f5496cf51e2e8f670522f84d8 Updated subsystem to use an image from ocpmetal
f912fd980a4d0131dd9bbe6b4682ff67e959125b Get the inventory image from ocpmetal
fa941a3bde6bdd160194c6379fe730ba2ec5dd18 Updated makefile to use images from ocpmetal
551eafbb1581e8e73fbe7ac7ab5a9dd199625d9b Publish inventory image to ocpmetal
b05c3492c795cfec25ec78bfb4f296ff77e64f30 Updated image-push.yaml branch to master
99d8ef627a576165f9460cea7cdbef7ff11692eb MGMT-1029 Configure git action to build and push the agent to ocpmetal Added image-push.yaml to githob workflow
d89e6d873419efbad5f691d1a2b5107006704789 MGMT-688 - New inventory structure based on ironic python agent output
585119048068fac6dd8e4d65bb6ccc3d2e0fcdde bm-inventory changes for MGMT-688
c4fbba1b5fa22b7b37b08ec1ccd7a97b17cc51d1 bm-inventory changes
5ddff6ac1ba1d03f5b275a0c3007b17ab55d305c Changes as a result of swagger changes
1504f7b8f0b0d06908c50ac89560eaf13c6e9830 Go modules
10f3e6f0e5b48b8082f2cbca7c21c4bc46572e9c 1. Remove loggger from context 2. Add session object per query session that holds the client, context, and logger
42c6f093e472ebb0777a41fcffa5a7ce01f08a7b Go modules
b08470cef989d95d7a8c4ebcca8b2b69b1fd2579 Merge pull request #9 from ori-amizur/ronnie/action
075ccd6a7f9cd9f5b6ba41c7cbc54bbfdbf2808d Changed setup to python 3
3d987dff09132791ab84460a296d3fc0a94a49a5 Added github action for testing
0a4b7920d685850a6ecc4ac719c8eead423423da Update README.md
7206489716cf65832760a368613bdf5c4519ddf6 Remove uneeded function in subsystem
09a2dd339062b8c31fd94ed13ac28c619a7de752 Add request id support
586c191a800300b2de67a6d62630798ae58a6738 Additional tests
d629bc93d3f6f73bbf4efea641043c570256af8c Go modules as result of inventory change
ab33031be59daaa7a468485e7e9eb6e41f3b1aa8 inventory swagger changes
893a078cc39d2156cfd240ab6b9f8e70d5ee4d4a Change memory units to bytes
55d65a8c4e2a7a6ca498bf6b40e0c9e1bb56817d Remove uneeded log message
e05d994ac163367a38a5468e1e57d1f1f4a713e8 Additional tests
35a901b4a49bcd042d2f03d381aa16ebd08367c0 Go modules
72cd92dbc46535d6ae8e7083b7af40e610f4394e Add subsystem support
f4070955dbc4129de1d110e63d4da4d9958e43c7 1. Rename introspector to agent 2. Create additional contains: connectivity_check hardware_info dmidecode 3. Agent to call the dmidecode container and not directly to dmidecode
2cb5a819c336dc222e14a0d3ea471f90cfe1a962 fixes typos
e2f503e117a5305d8e67121264175bc7135ad312 change hardaware info to hardwareinfo
7a6b82d6326242e3ce3d564f4b9e4fb6e109a74d go mod update bm-inventory client
e721edda0aefd545d7a58ba5fac1d695b3549a19 New bm-inventory
70b7c0a0567df1a615f246cb488303eaa248a585 Adapt to swagger changes
2217ed35e12fb7739dd261ae129ff388c06e767a Execute implementation
936ab528b26f7abb1f98a3ba2a2fa5f644801072 fix makefile missing service env
d06748f7ed898c7daccfaf2798b03a3670dc4a8b Rename src/commands/node_info.go -> src/commands/host_info.go
bd47a235381083e355b5b5b26c7c223fe62a4a8a Change Node to Host
bed164a286dbd72e09a938acb16ca49f0787420f go modules
ac622b4e58363646967904cc7113720a61b1d632 Supprot chaning SERVICE target with environment variable to change it just export SERVICE=<your-target-image> and skipper will work with the new target
59ef3d58bbd677ff2f1b238d6b017d181dd9a112 Merge pull request #1 from ori-amizur/michaelf/skipper
5ac521fe338372f3fe5aa9776ba43a51def31f21 Default to building the build container in case it doesn't exists
d27f59640247c93c0f203952c9d40363d317842d Fixes to nics scanner and connectivity check
d20b7ce04c6835baf08eff9047cb625f05e2a67c Adaptations to swagger changes
123db1272d3d04c0b2134d9e3842da68c2f6298f Added connectivity check
164aa6f6c5219556e99d2211b5ba90c2b6da9804 Periodical commit
06549d6868718f22d46212ecac72bb0197bd5d78 Project reordering
e321184f3bb0f5e3166bc9320be83743a9a1278d Periodical commit
cd1a8f4767addeb926b1d6fcbff8fb23f4dc2f10 Periodical commit
e7e85fe4b8187de033be53988bcf10e13e72e67a Periodical commit
d87f3ad07ed1306363724f55ac88521345f60752 Second version
d53eb866bf9048c461ccc82c086fe1041cd641be First version
```

Status: Fast-forwarded successfully.
