## Syncing openshift/assisted-service with stolostron-engine/tracking-openshift-assisted-service

## Status Summary:

release-ocm-2.6 -> backplane-2.1: First run, created backplane-2.1.  

### Branch release-ocm-2.6 -> backplane-2.1:

New commits (first branch sync):

```
d4c02b2a7bade2bf62239416d9d66efbcd12deae MGMT-12405: Enclose API endpoint with brackets if IPv6 address (#4905)
ed9574025470ce4a16f14a37f809619ae9d85ed8 MGMT-11621: Allow subdomains in cluster name (#4910)
0ad5c7dc0a947d85f55abaa6a2dcec80f3241764 MGMT-12423: Watch for Agent changes in ClusterDeployment (#4885)
7cd0f7c0b65ca8f29158e3a57e7f8068eb0d6063 MGMT-13058: backport vsphere validation in sno to 2.6 (#4879)
6c9f6fc232d2e77aae6fc9a6e0ee269a75b019dc [release-ocm-2.6] MGMT-12794: allow to edit ProvisionRequirement post install (#4854)
472aec1137ec860486ba04bd46af202c6baaa37d MGMT-12379: validating platform type for SNO (#4788)
081373a5c26e8c770a9fda57ed98fb98aa603f59 MGMT-12866: Assisted Spoke install-config does not generate icsp with multiple mirror to entries (#4760)
7c51c9298fe5b9d05ff2c055b29e0fae18e6a374 OCPBUGS-2953: Fix regex to filter images by tag and by sha (#4785)
f839e3945f074775e5dd23a620d70cce3fe06ce8 MGMT-12635: Add icsp-file support for all oc commands (#4684) (#4700) (#4738)
b40765d9125de36f228f259131b786a13f7eb90d OCPBUGS-4493: do not mutate ACI post installation start (#4743)
37da8394789141ab4326b6127ea01feb12a2eaaa MGMT-12738: Validate storage requirements (#4686)
ca1896d902a8b0dd487f246d96849ec81786dc6c MGMT-12423: Additional debug logs when collecting Agents from ACI (#4711)
9128e8f630504fadac5ce0042f569ca26f3abb3d MGMT-12423: Add debug logs for counting unsynced agents (#4591)
f0c585799b20896afebb57df70b0cf349b4bf190 MGMT-12689: Day-2 agent stuck with status_info rebooting although the node is already part of the cluster (#4699)
1887a0503a1d557b027304f5a2979fbeb82b2eb0 NO-ISSUE: In 4.12 use 4.11 LSO and legacy security context (#4497)
ce70b2bbadf3af94ffde403c686b21e1675d656a NO-ISSUE: fix attach-disk failure (#4649)
5aaf9a983c335f1b5f2ce617fe7b9817c559a993 [release-ocm-2.6] OCPBUGS-3749: AgentClusterInstall remains in installed state when using ignitionEndpoint (#4609)
96b46896c97b221ff851151365d50961fb9afdd1 MGMT-11799: change all 'go get' commands (#4538) (#4619)
cc60dde37da83e3f648784681c2ac3cecbd4d7dd NO-ISSUE: In CI check status of Deployment and not Pod (#4493)
d6c890e9a6aafe7dc7977cf120bb2f503a49700d MGMT-12167: Make possible to mirror an index referenced by digest (#4533)
0639d0cba7c951b2d729a643d9f864a23c71d450 MGMT-12317: Add capabilities entries to install-config (#4532)
dd15431125b7dc5c028fafab40573a488af43948 MGMT-11642: Add Host Bind/Unbind Events (#4490) (#4515)
7a46ecbd7573b9ab5e56c5be8b610b009bf1cdc0 Bug 2135714: Don't set bootstrap kubelet ip in case of UMN (#4510)
f571793823c29ab07aeb09c8290285001cfe34b2 Bug 2131023: Allow arm64 sno installation (#4454)
99b3c7f44d5744eb209a10567dc1d9ac09368759 OCPBUGS-1482: Don't override schedulableMasters unnecessarily (#4445)
6bcafaac7051ae8d01575e0d48b99fc7678cfb55 Bug 2082979: Add node ip hint manifest for sno. (#4408)
977bbc6989a76e9876b047aa5467998dddfe4a45 MGMT-11414: support platform in kube-api (#4304)
3b50d80e662992e2516564f3594891432769e386 MGMTBUGSM-482: kube-api - improve error msg for missing OS image (#4355)
56d4db43cb446455733fd12cb03da2ab0e17b057 Bump mockgen to prevent dependencies removal (#4328)
e7b2cf99584449d151ed4643f8b3bfcf55a462c6 MGMT-11035: Allow noProxy wildcard for infraEnv, regardless of OCP version (#4224)
8f2dd40b3baa64339b6d4c752ce6e207ba6e5034 Bug-2118970: Create an utility GetIgnitionEndpoint function (#4289)
d5f3f71046ec066afa25752dcde6ffcd983d4f25 MGMT-11708: install oc from quay.io (#4288)
0e8dce55287d09c3e622cdb3c484575e6e0207ba Bug 2113954: Fix order when merging ignitions (#4240)
e612c65a7de06b27480aee8f4489ea3395070650 MGMT-11411: Fix image references for the release branch so that they correctly point to :ocm-2.6 instead of :latest (#4208)
32b7568048b41e38c0cfe7676d17a132b6d05fe6 MGMT-11020: revert usage of 4.10 catalog for 4.11 ZTP jobs (#4238)
6751dafe5fe0dbcf4a475c62b4fadf1a69b24165 MGMT-10960: [Staging] changing machine network cidr while allocate IPs via DHCP checked , show error massage (#4181)
162922dea5c2eede86295ef178f308bd3c3177e8 Bug 2112321: Stop reconcile loop after changing CR inside BMAC (#4201)
7c20d2dc912b417a95aa30fc76160186dcc8b41f NO-ISSUE: Fix conversion of disk size for device hints (#4205)
f28bdba712e8f28971d8e95b0daa67f9e8addda2 NO-ISSUE: Don't log whole ignition for InfraEnv (#4204)
852dd020dbe8d0b2c0d33c254e8affad57d61d9a bug-2109637: Agent validations out of sync with the host validation (#4196)
e8038fe184d79981cfddec040817945586e1cef4 MGMT-11362: Set api vip and not dnsname for day2 cluster (transform) for bm platform (#4191)
ab2e9bd8b9d3095d01ecf05fb433953a683f40fa MGMT-10734: Add more host reclaim states and transitions (#4139)
d295892559ab19e9e666785e30cfdbcac93a0b69 Bug 2099929: Detach BMH using dedicated function (#4202)
de2527037564396eadc7aaaaccc246e66a07eddb NO-ISSUE: cloud.md needs a little refresh (#4195)
6eee0a76dc03c067737fdcfec9a806d78d35fc00 MGMT-11334: Add API models for service-to-agent host reclaim (#4188)
eb992f68656589516ae04b3a0090ab1f34fa977a fix python syntax of string comparison (#4190)
1f7410a2d43220908c4ef1b136d2075ac284ec96 MGMT-11153: Add cluster tags support (#4187)
4e04230522992aad4d93551b8d935aa0d8b2ed0b MGMT-11092: Merge the format and the condition methods in host (#4097)
f118b7b814ac52496cd0b0ac476b1b8299043648 MGMT-10973 - kube-api imported clusters should be considered imported (#4155)
17617a7feaebf966bb4d64502da3fdb471de22ca MGMT-11309: clean up unnecessary grafana dashboards (#4186)
d0b6ccaf40bbd73e6c744d98e313186f5c7e5588 NO-ISSUE: Bump OCP versions release 4.10.23 -> 4.10.24 (#4184)
b4e75d4000007d48635c3f556c4dea149589119d NO-ISSUE: Remove leftover comment (#4162)
6b8401d3b0f0ceea5a837f33c17b9b1cd5ec52a3 MGMT-11309: clean up prom metrics to enable meaningful alerts (#4173)
58e7771c73ca45b263e2cb690ce3c3b55f199575 NO-ISSUE: Bump OCP versions release 4.11.0-rc.4 -> 4.11.0-rc.5 (#4178)
5147460a5dfcd06305e9b2cb81915d2f4e7bb90c NO-ISSUE: Fix set platform_type on cluster update (#4176)
857dca06b5875a17c8dd8fbae6ba336046b27092 MGMT-11262: Parse `/etc/kubernetes/kubeconfig` in day-2 ignition to disable DNS validations (#4171)
4e7e96d98937ea0cee26c37a868c9d68556e20e2 MGMT-10790: Always use APIVipDNSName to obtain API address (#4018)
fcab73ab6383eb08483d9bc8df3575acff279e32 MGMT-9506: Remove timestamp from host inventory (#3891)
b4662ae17568c0f1dd14a1485dbf1ea29c64b43e MGMT-11316: Remove unused `ovirt-platform` from swagger.yaml (#4177)
6b533d826e70a445d0fd501060675e44260de47b MGMT-11027: Add ENABLE_UPGRADE_AGENT env variable (#4172)
a775a4ed4d2a60fd3662ba537c62be74af8f386e MGMT-11027: Implement agent upgrade feature (#4121)
f7ab8b3d4ff7f12434c85624fca1ba3553a35aae MGMT-11174: Add Boot Control Kube API documentation. (#4160)
8e6b6c5913406433fd09098d1d37ee77a8f6168d MGMT-10852: auto-assign races (#4084)
1ea8c35ee89b824a4cf2cb0f970cafb8144fc891 MGMT-11131: Cache results of inventory unmarshalling in connectivity test (#4170)
73b77f57ec19287ec9682685dee1e387961425bd NO-ISSUE: Bump OCP versions release 4.10.22 -> 4.10.23, release 4.11.0-rc.2 -> 4.11.0-rc.4, release 4.9.42 -> 4.9.43 (#4169)
5bbb7dff3d57e4ab0f6669a11f590f7277904fdb OCPBUGSM-46053: bootstrap flag is not cleaned after changing role (#4168)
6977652f95ddacdf355ac37121058dc330d05627 MGMTBUGSM-412: validate pull secret in kube-api cluster deployment (#4131)
8b40b949f3795d0f2643d6cac640bdf0658cab26 MGMT-10861:  When removing/adding api* and apps records, it takes 5-15 minutes till host/cluster status is updated (#4145)
8264d400fc901b552bb9c2a214e6558493aca386 MGMT-10007: Remove ovirt-platform object under platform. (#4163)
4e69e146c67d4cc9482cfa162f4320da95b43d9a MGMT-10840: Change VIP DHCP allocation default to false (#4146)
6548ecc097886bd1c17271b45bfb92ff58cd1ced MGMT-11198: handle nmstate empty connection list (#4156)
2a5c40bd16be4961466483c34310cb1b91e42226 MGMT-10315: Remove deploy references to unused public bucket (#4164)
4ba9c5001e942101ac3f25df00e2bccb78592610 MGMT-11124: remove usage of IMAGE_SERVICE_SCHEME/HOST (#4157)
cca573243ca975d0bd4d6c4ec212586804bee833 MGMT-11174: Add IPXE boot control flag to infra env in kube API (#4151)
f7c6c3d57be5db17241522d55bc17daa20917bb0 NO-ISSUE: Fix failing static network config subsystem test (#4152)
a5cafb300700e5440504eae1de1cdb4ee0884619 MGMT-10866: Compile assisted-service with CentOS stream 9 (#4138)
c0bf41a099abe51d6153f5095aac6608f7d7ac48 remove OCP 4.6 from upstream CI and integration env (#4148)
bf9e0f714d7333b476b14bf8dc51ae3b77b91ba8 MGMT-9354: Define agent inventory labels as variables (#4147)
19e843c3df3681dfa4eb5ad6aa74d74597b81249 Bug-2106496: Do not perform refresh status on hosts after roles need to (#4137)
cbf4a2da590ec0ad543583ba6731fd92acafd1ca NO-ISSUE: Return bytes from `executeTemplate` template function (#4126)
98ac9c18986a889942839d3cf1d63f8c40ce792b NO-ISSUE: Use template function to generate data URLs (#4052)
564650feca372064314282d98d6fd9c6ee69bd2c MGMT-10973: Enable DNS validations if coredns or keepalived static pod manifests in day-2 connectivity-check ignition (#4072)
3782baf4165085d453768905e02ab9df9ddbee5d MGMT-10445: Add enhancement for automating returning an agent to the infra-env (#3849)
bdc942605d12956f40d84e0613d90776164fe7ce Bug-2106496: Make sure that updateInventory function does not use the internal DB object. (#4136)
a6d0cfb4625b407740369aa0a87297a90ddd641a MGMT-11161: Add "/boot-artifacts/" route to ingress-tls (#4143)
06a7ed0a6ac9979446d841bf19eddc64132226a9 MGMT-8578: Use host's role when generating day2 ignition (#4124)
ebc44e88d932ef0692074be1f31281d23b7b0f53 Change importing of Ansible's nth-host function (#4142)
e9b230109ce8c60c086baffca1078b370bd8aa0e MGMT-11131: Track hosts' registration times (#4128)
43cc03307d740741006b62b745f549121519a6f6 MGMT-10209: Pass in icsp file to be used for 'oc adm release extract' (#4115)
e15505fcb36ec7c44176bf39a0015470b37059d4 MGMT-10844: Add virtual interface metrics for SaaS (#4079)
7e1c51e312b8674303742dab6dbddef34512ec32 MGMT-10570: check that are master machine found before referencing them (#4108)
b95c3fcd89d2b012206a0266a23e717c3d7166ce MGMT-11161: fix rootfs access in PSI installations (#4134)
2fa0ae15a0a2205aad9de527db5431ba09d6c148 Merge pull request #4129 from michaellevy101/docker-failed
1f7b024e52f7644897d4b740c80f79e5e0a0e4e3 NO-ISSUE: Bump OCP versions release 4.11.0-rc.1 -> 4.11.0-rc.2, rhcos 4.11.0-rc.1 -> 4.11.0-rc.2 (#4132)
5e904658ff6244cd75a41df0c6110c8cef0b8f6b NO-ISSUE: do not print error message when docker doesn't exist redirect stderr to dev/null
d4be562ea1287b738259dc0b713d874cbdecfb96 MGMT-11120: Fix a misleading NMState error log (#4125)
616fc2cf84a479cfd8a4d32c62350c1c226c9f6e NO-ISSUE: Bump OCP versions release 4.9.41 -> 4.9.42 (#4122)
e1af4a57c4537ef6b44cd674d448012c8311ee10 MGMT-10985: add feature usage for static IP (#4123)
da8164f04040feae88de132de4cfe02447129dde Extract go test-tools - use small container for the CI instead of the huge builder container (#4116)
363e39a111961b0d8d33746db78ea98a27e9b846 NO-ISSUE: Bump OCP versions release 4.10.21 -> 4.10.22 (#4120)
4cff311dabfd24e6a777bb8df01a5eedb3a01552 MGMT-11098: Pass correct kernel args for multipath (#4119)
47a910fe9dee57370c0b153a6fe994e8cb2a824a MGMT-9982: Alter ipxe-script endpoint to handle boot order (#4012)
9b2224f816ec73896221af6925031a9fb6290549 Update postgres path - it could be on pg_ctl could be at /usr/bin/pg_ctl or  /opt/rh/rh-postgresql12/root/usr/bin/ (#4111)
dd79548c59fb0756b5a6536a8868ab29123dfcd7 MGMT-11115: Add setting bootstrap kubelet ip os env for installer generate (#4110)
876fcb41a2a0fd09dee886ba4935b89c847b882c Update OKD version to latest stable (#4109)
960e50e34cb5a8dfc99692fa46c52b884d309e98 NO-ISSUE: Bump github.com/aws/aws-sdk-go from 1.44.33 to 1.44.51 (#4107)
5106e25edd3193115ccb714841e1815e9d1309a1 NO-ISSUE: Bump gorm.io/gorm from 1.23.5 to 1.23.8 (#4105)
212a624e71d553be3fa16cbd0544a8bf0e088777 NO-ISSUE: Bump k8s.io/kube-aggregator from 0.23.6 to 0.24.2 (#3986)
1e547767e2fd508b13d8aa33c2529cf6f274ba06 NO-ISSUE: aws cli isn't available as a package in centos9 (#4100)
7a5050107894c6394405f599a9f9289addc319c1 NO-ISSUE: add CPU vs response time panel, unify limits and resources (#3909)
8b0d5eab415e5b06b8a54c33ea65b2d795a3c0d7 NO-ISSUE: Bump several k8s.io dependencies (#4092)
f3b99805406ddb2659f5cac787bcc46f000e83ce NO-ISSUE: Bump OCP versions release 4.10.20 -> 4.10.21, release 4.11.0-rc.0 -> 4.11.0-rc.1, rhcos 4.11-fc.0 -> 4.11.0-rc.1, rhcos 4.11.0-fc.2 -> 4.11.0-rc.1 (#4098)
9b5bb30c4e1c7ba42566f11eabb09fe16eaf3942 Bug 2104117: BMH  stuck “available” after changing a BIOS attribute via the converged workflow (#4090)
69a2c94c4c09e27d8d18d8ba6287b3c2fd975f12 AGENT-231: Agentbasedinstaller register extra manifests (#4083)
b64471ee0eee3edeb44daebaec56859f1f10fc0b NO-ISSUE: Skip failing static network subsystem test (#4094)
c78bdd568ad733a8291c43ff4f56f66d8871c884 OCPRHV-637: Set 'replicas' to 0 in the machinset for the oVirt provider (#3972)
e27247fe07ace5f6212ea5896871faa84e329fe7 MGMT-7741: New validation: TANG server connectivity check (#3608)
91533bab5c8ec075348b83786a25c92410599077 MGMT-10838: do not reset roles when operators are not updated (#4089)
86f181808eee8a04acbd5cedde0b1d28a59406a9 NO-ISSUE: Bump OCP versions release 4.8.45 -> 4.8.46, release 4.9.40 -> 4.9.41 (#4086)
9fab7bd07fbaa9de1bdcecc4563f17a815cc1c9b MGMT-10734: Add host states and transitions for reclaim (#4041)
81e8e04b9a75f353ec26d1e0ad9c1ac3ddfb3227 Bug 2100857: Fix master's manifest file pattern for oVirt provider (#3971)
b7eeb964297b80c1382868aff5b897a40c986342 MGMT-8890: Fix wrong release in the error log (#3889)
84ebdbf9138138d28bfdb2272c8c63247465ef80 MGMT-10921: Ensure that API address is not one of the cluster hosts. (#4068)
571ce5393a58307535b65da182a1024bb8047e30 Improve error reporting in ephemeral installer client (#4057)
54c1cbc719b9c2c6840b6f1e2bf7c8f71c237b36 NO-ISSUE: Some cleanup of `add_day2_remote_nodes.sh` (#3682)
4c059bcb7787f5a0d715e330f7fabae60edd7311 NO-ISSUE: added some logging in setup_lso.sh (#4081)
ec7fa62f824206746cba3f50600460801a7b8497 MGMT-10848: Fix double agent unbind when deregistering a cluster (#3964)
c7734c46ed9b9a105c7e77ed4afdb8352831abb8 MGMT-11026: Use image tag for metrics (#4078)
9d21fc4e3d71c4dae59c534e363a233fc68c9df4 Extract golangci-lint from mirrored docker image (#4077)
18e826f97bb72ce7b73f6eb5e8767f22c1902e9d Bug 2076333: Add UnsyncedAgents error in ClusterDeployment and ACI (#4046)
f1daacead01c1897fbf5953e946b2ec3b635db0d MGMT-10311: aci mutation hook (#4022)
c9d236c13d799acd5da7277146f5ad576f41af31 NO-ISSUE: Remove host ID from the `serviceLogicClusterHostImagePullStatus` histogram metric (#4069)
385dc7aff4c6e5b75b3b206a9048450312b5b423 MGMT-11000: Failed to update the cluster when select Integrate with vSphere (#4061)
dceb319f4a3fb17f3798c44a13095c7ba379b4de Revert "MGMT-10850: Message for Day2 reboot is misleading (#3970)" (#4075)
1de0c859c16db17c0700bea5f179b47bbefe9b63 Allow setting default ISO image type (#4062)
f436483d70e9eb1ffb2627e80b70edd4d64161aa MGMT-10991: Add forbidden hostnames to cluster_default_config (#4056)
e34274ae119fa9a3d5cd6786dd6de4716897729a MGMT-10850: Message for Day2 reboot is misleading (#3970)
8e323d766e72a00f100ffdcc0430b7529a4fd94b NO-ISSUE: Add @rccrdpccl as approver (#4070)
d347dc4d2f2fc1deab3d2b5e1ff8c08b449be578 MGMT-10678: Add upgrade agent OpenAPI enum values and types (#4028)
f40267245a6bc7e170b4e6acb368b7c41d8f0397 MGMT-11012: Add default route metric to inventory (#4063)
7f0a41b671297e987ae07a6e55d32f82a5c0c974 NO-ISSUE: Adding jhernand to approvers (#4064)
fe198c52d1a6da4bebc3f7874ea7cbc0b4cb04ad MGMT-11011: use 4.10 index for LSO installation in 4.11 (#4060)
09aaaab4b3e625bf56b22248c7878d412775c0ca NO-ISSUE: Bump OCP versions release 4.8.44 -> 4.8.45, release 4.9.38 -> 4.9.40 (#4055)
3a83d5abc438f555453ba24d1558ddeb698b7dd3 NO-ISSUE: Use `go:embed` for ignition templates (#4044)
bd2c5ea3632c68f195365c0a9556f31dd14a195a MGMT-10997: Use label filtering when listing Agents via K8s API (#4049)
3f7e555ac8714515f3031bb62a3f395717ff358d MGMT-10767: Add subsystem for converged flow (#4047)
31a8ea318d29b086888a1eedf30cbacd7316be2c Fix ui-ingress object to new API (#4059)
93ecf032a8fc9f0e2e372a3b68cab9ac08205a38 MGMT-10868: Fix duplicate `-latebinding` suffix in ZTP latebinding scripts (#4058)
8a7757a04c475b96f1c1b2f7f1431c4fa6e6a51b MGMT-10993: Validation failure on hostname, make messages clearer. (#4054)
400e890fbaa096253a63fa14f2dae0d99dcda7ac MGMT-10868 - Fix missing `ASSISTED_PULLSECRET_NAME` in ZTP day-2 scripts (#4053)
89f713bb0631558827fa207739a72ddc680cf2ef Fix oc-ingress installation method (#4050)
1f689a40a7688477fd2cf9c0e5bdf33e63e3daad NO-ISSUE: Fix onprem job (#4048)
088b584f2808f8f1c922d55531ec468bb6d3c8ca MGMT-10989: Missing condition status in case of unsupported image format (#4045)
437ba626e0d6a737148c11c286c7115f0d25832d NO-ISSUE: Bump OCP versions release 4.11.0-fc.3 -> 4.11.0-rc.0 (#4043)
e41ec722c2475a2878a1c9af55987dd937e1aedc MGMT-10958: UpdateHostName - Validate that the hostname is not (#4029)
1f30ed66d4084e69cff125b0a1e47a92a2939cb0 MGMT-10832: Add document for agent upgrade feature (#3928)
13384b19473f80b36b8c98b546f47797bfe3a60f NO-ISSUE: Remove unused butane utility (#4040)
53701f7b41730605ad0407b8b88adb6f2dbcbe4f MGMT-10868 - Fix unbound variable error in ZTP day-2 scripts (#4021)
9007d626a2684108bec60234acfdf6be89b1d64c NO-ISSUE: Bump OCP versions release 4.10.18 -> 4.10.20 (#4038)
c45f3699d83665a5e27a00939a9ff40907f39111 MGMT-8089: Force schedulableMasters (#4011)
bc7dde9ac107c70ec09ea0a62ea470e79d473807 Add OWNERS file for ephemeral installer client (#4035)
4f5e2c7952347d19fdcfd19d35cdf359e657cb8e MGMT-10914: fix ASC deployment reason on success (#4034)
eb6c54ee51b2a738e866ab4cb6e67a41bd1bcf78 AGENT-227: Don't exit when inventory not available (#4030)
09e500a682ea648bfd6b08be3741607f44951404 MGMT-10754: remove unused rootfs_url (#3996)
5552989baf3bdaab4a045ad23c7271179dbd5fc1 MGMT-9021: Set feature usage for ignition config overrides (#3791)
ad64755a3e283508b7f6bfb5343707948bdd3801 MGMT-10967: Set minimal ISO as default for SAAS deployment (#4033)
9e89b1e02fc5278b6631fc00611de1373973d890 NO-ISSUE: Gather service pods definitions in the operator CI (#4032)
4835e5f60e1d9b083b03c86c847183c34554682d MGMT-10956: Do not enable multipathd on OKD agent (#4023)
4bdeecd371d649b24c96b85cbd7100b9449120a8 AGENT-144: Use pre-generated InfraEnv ID (#4016)
84fd9ecc5451a920e9586be266ed131586f64579 NO-ISSUE: Bump OCP versions release 4.11.0-fc.0 -> 4.11.0-fc.3, release 4.8.43 -> 4.8.44, rhcos 4.10.3 -> 4.10.16, rhcos 4.11.0-0.nightly-2022-04-16-163450 -> 4.11-fc.0, rhcos 4.11.0-0.nightly-arm64-2022-04-19-171931 -> 4.11.0-fc.2, rhcos 4.9.0 -> 4.9.40 (#4017)
eba9079e61bb5022f788de9bc612fa53261b71e5 AGENT-227: Add host configuration support to ephemeral installer client (#4014)
f1d9851a1cafb72827d941f8a5962c5632dfa50c Use releaseImageMirror in GetReleaseArchitecture (#4005)
8306b067be6e8441739fd3897a7175dbb70f2f66 MGMT-10868: Add late binding to Day2 remote script. (#4010)
4d8bc262ebe546b7df9d6ee48e487043a5fd6779 MGMT-10311: UserManagedNetworking type change (#3927)
0b62c2873bd99d1ca3a8cb48750314ea8012fbb2 MGMT-10865: Machine network is not changing if list has same values (#4013)
c2406c9df83f8d52c1823200c659dcf44b5d7543 AGENT-224:  install packages for openshift-install (#3966)
cf0b54eab30151b3c20cc8be98b8b85e395c214b NO-ISSUE: turn on debug logging for golangci-lint (#4015)
6f2f295b170c39550e59e30b1d49356d128f5a67 AGENT-219: dnf install postgres for agent installer (#3944)
86037f622038d984fffa517dc2b4f4df97667f7a NO-ISSUE: auto-assign test with out the falky parts (#4009)
60b6b2d6b8beee88508974d3f0337dadae2f1c51 NO-ISSUE: fix assisted-installer-ui ingress format (#4003)
93321ff2278fd53bbb1c0a4ffd8b25be0af4c93b MGMT-10916: Change capi-provider-agent jobs to use the operator workflow (#4008)
02ed350a59ae3a8afb07612daf356960ac7baeef MGMT-10753: add base url to image-service deployment (#3957)
0f54e446da320c843d2d9a21fa71a6b7dce886ac MGMT-10493: Don't truncate CAPI/Hypershift logs in CI (#4000)
63fbbe64a0b5a007ef5651978610083963218f40 NO-ISSUE: fix MinimalVersionForConvergedFlow to include 4.11.0 nightly builds (#3998)
b421b9f6a8219882e7df26fce378be05cafcf58c AGENT-75: Add assisted installer images into OCP playload for Agent Work (#3954)
c307ab09df58e0e81bb558acbf485001233423ff NO-ISSUE: skip flaky auto-assign subsystem test (#4002)
910d5eded01b6dfc72b396ac57f97147786f6160 Merge pull request #3995 from osherdp/fix/umn-with-vms-supportability
a6527c6c9e877f57ae66e67a9acb6599f265ae44 NO-ISSUE: update networking api-version to v1 (#4001)
81cbcec1d8bbe1869a7e377c3fdd26ebe50c5bac MGMT-10330: do not change network manager config in case of SNO (#3993)
a43ea53bb2151bf70d715a016566934bde5c954c MGMT-10864: Collect CAPI data in assisted-baremetal-operator-gather (#3989)
d37d54b846d18096585c28f25e57939d10f69316 AGENT-215: Set release mirror for agent-based-installer (#3988)
02b4316c9fe29571a7dda220d9cd22ae73f3ca09 MGMT-10820: Make sure the PreprovisioningImage "Accept Formats" contains "iso" (#3994)
fa149799be86b9999b0db081cadcb6707ce487f1 NO-ISSUE: more indicative message when agents not coming back (#3671)
a76a87913bc1ac04bc5096e29aabdb5989898c69 MGMT-10858: Get Ironic image from the release image only if the release version is 4.11 or above (#3983)
fe02299d0b06189dc8eb9adabfe707a8fe8e5a9a MGMT-9720: Rewrite network configuration guide (#3892)
deda48c64e26d1fe4ad46c5860a71a1b00623e6b MGMT-10889: consider usage of CMN with VMs as supported
5d5320bfae959fc70b350d30144475f455f9381e MGMT-10488: Add assisted-operator-ztp job for the converged flow (#3991)
5435d5f860902a50467781a61f9375840cedde08 MGMT-10834: Remove ARM capability (#3959)
1d443f01ef736d29e0df2d2e73973f880e3b8320 MGMT-10855: Do not format bootable LVM logical volumes (#3982)
48e7076a57658b83816c045bb75252a4b7c85953 NO-ISSUE: Bump github.com/moby/moby (#3984)
8018e4399079bb2fcce0b078affb63b3790b68c0 MGMT-10637: Add default ironic agent for ARM platform (#3977)
4863910d0f488557fe92d11380e2f8c34285ca73 MGMT-8987: 4 nodes cluster deployment (#3669)
48f9c09ba0dd4561d0877a6e8164bd2a5eef0cc9 bz-2096106: Assisted service triggers the worker nodes re-provisioning on the hub cluster when the converged flow is enabled (#3975)
6e23b2a646d6b5ac0e32ab35597a7ce1b3447130 MGMT-10311: set user_managed_networking to true with sno in ci (#3947)
5fb6d505cac8bb660b6df62d8d5d47cad169ed5f NO-ISSUE: Bump OCP versions release 4.8.42 -> 4.8.43 (#3968)
1cfbfc7ece4cd6d6bf139347650afd552d30d770 MGMT-9682: fix default disk size requirement (#3973)
69d8cb716ad3675d287a9490aef6bdf1b0b7f303 MGMT-10597: Open firewall ports after DNS setup. (#3969)
3cf458c0af48b42940efaf19e2a2351ae79fc60f MGMT-10597 API address should be correct for SNO (#3952)
0c62d72dce509cbd7dce6a8187078096e63870e4 MGMT-10411: Allow enabling virtual interfaces (#3905)
6e18ff5b74e09e25d7fd0ba8586776f3e58c83b6 NO-ISSUE: Generate vendor directory correctly (#3960)
afdbab3426ddaa21201c28aadf58f2f4794ddf8c MGMT-10780: Explicitly pass OCP version to Hypershift (#3948)
c894572de9b27a5a50107d88a674ffdc84e04c9f NO-ISSUE: Adding paul-maidment to approvers (#3961)
4ca1437bdab5c7035cc152ed476174301ec7ac32 NO-ISSUE: Remove unused GarbageCollectors interface (#3953)
d98c44692493c07cbced0667b47ca48578a9cf0e NO-ISSUE: Remove code for deleting ISOs from S3 (#3955)
e7f1b2be6b0cc18e7fd0bc95203437ae5e40f333 NO-ISSUE: Bump OCP versions release 4.10.17 -> 4.10.18, release 4.9.37 -> 4.9.38 (#3956)
73fd2631a5c4fc60cca8b71548ac272e0801d650 MGMT-10656: Enable multipathd by default in live ISO (#3951)
c37d5543e1c6cfdb1d4b3ed13143268461ccf026 MGMT-10755: Remove duplicates: 'AMS subscriptions' unit tests (#3950)
00977c5e7667ed0d866cb4a0d0135d231b905516 MGMT-10801: Add necessary kargs for multipath (#3945)
c425e1c2aba5ad4aee83a9376914c3c8cb1b7716 MGMT-10783: Add hostname validation regex to validation (#3943)
e5476deea0625b2f1e7fee8ed5b6da72fbed3036 MGMT-10755: Remove duplicates: 'IPv6 support disabled' unit tests (#3922)
325e643291d12440b421d7fa9b6ad5b5c0bbd428 MGMT-9561: VSphere platform lacking setting disk.EnableUUID guidance. Change the host status to insufficient on validation failure (#3941)
208bbd5876a6f3b6c1bb290e8bc17c3e90972fdb MGMT-10666 - Single Node expansion feature support flag (#3886)
719eb3301bf2e6954d2c70c51625358252607eb7 MGMT-9710: Provide extended networking defaults in default-config API (#3586)
26df52ff4b516746d200ee92754718e948f9d76c BZ-2096460: Spoke BMH stuck inspecting when deployed via the converged workflow (#3938)
cd7ad2adb5cc7f51e893c277b4403148b66fee7f MGMT-10597: Libvirt DNS added for spoke cluster. (#3929)
cca3023940a8f8faad69419a5e53faa1d610ffaf NO-ISSUE: Bump github.com/aws/aws-sdk-go from 1.44.15 to 1.44.33 (#3936)
adfbf6c16ffa0714540cd92f6682cf48ec3e7be3 NO-ISSUE: Bump github.com/stretchr/testify from 1.7.1 to 1.7.2 (#3932)
994506f292c0cfe5fabad2edb4c1983aaba3d7cb NO-ISSUE: Bump github.com/prometheus-operator/prometheus-operator/pkg/apis/monitoring (#3930)
4d1cce21e4c4ccb3e7d16bc8245bc2ac3e1f44af auth: AuthUserAuth errors should be wrapped in HTTP 401 (#3933)
711bd1f12bd849d97ad250c3f77e03b3d6376750 MGMT-10755: Remove duplicates in subsystem tests (#3919)
9d50fb89dd33b119f6242c2b08c5235b36909842 MGMT-10618: enhancement doc - extract OS image (#3877)
06b1ab8c49415b89a824d40b81df70a14dc936f1 MGMT-9561: VSphere platform lacking setting disk.EnableUUID guidance (#3904)
98e1f4b3d1178f7850aed35d4cc164673f7ee4cb NO-ISSUE: Bump OCP versions release 4.9.36 -> 4.9.37 (#3924)
b3a63227a0bc04126a05abf7b7c5d1988eb38fbd MGMT-9553: Ensure that MaxHostDisconnectionTime is configurable. (#3917)
ee349efae3fd6170233b5f9413aa94d2b98f8edb NO-ISSUE: Bump OCP versions release 4.10.16 -> 4.10.17 (#3916)
5c9745d2283726f48d2d25c859b2ec5730d863f9 MGMT-10748: Define disk types in swagger (#3920)
55f604edd693fd72fbee7963309fe440a3d241c4 MGMT-8435: Fix V2UpdateCluster response to include hosts info (#3918)
ecd413df5fcf45dfa3e59f30e584cacc85f1c8f1 MGMT-10569: Remove cluster ignition_config_overrides column (#3914)
516ba0b2b0a3e50f0bdb222e8ec957de2a3cfca4 BZ-2089683: Disable ZTP converged flow (#3915)
ea98d35b303dd38229e448f5710f1492072256f6 MGMT-9388: Incorrect minimal CPU and RAM requirements for cnv operator shown in UI (#3913)
b8e888f0e704e25946b52b509bacf55f12876d9f MGMT-10722: Hostname 'localhost.localdomain' should not be valid (#3912)
c0fee5ccc185607b82a0bf996ce6df5b08b9a7fc MGMT-10705: Allow installation on FC multipath (#3903)
f2156d15d6f021c678bae68b8a8a074e25edad08 AGENT-40: Supply TLS certs for kubeconfig to openshift-install (#3836)
1259652dcd44957688d79ff08cd18a6dd640bb3f MGMT-10612: Allow installing baremetal + arm on 4.11 with feature (#3890)
565e5bbdbd3733831000b1e7378d8e3cd2509096 MGMT-10713: Soften IP-stack checks for host_network propagation (#3908)
fb68ca39091541be3f1947dc083456677c5134b4 Bug 2093503: Assisted service POD keeps crashing after a bare metal host is created (#3897)
f1dda992299a6a31a9ae33b4e904f294c62ee329 MGMT-10616: add release+OS images for OCP 4.11 (#3862)
0c1091d1c8946b632868d0c5bf384d3f5b8b3d95 NO-ISSUE: Bump github.com/go-openapi/validate from 0.21.0 to 0.22.0 (#3902)
85bfe005af0134e2f38844e9b40c01514272545f NO-ISSUE: Bump github.com/moby/moby (#3899)
38e505fe3b8099dc83f26d2165aa462024be8399 NO-ISSUE: Bump gopkg.in/ini.v1 from 1.66.4 to 1.66.6 (#3898)
02da5ad4567619ed157b74a124b176defb5e0eb6 NO-ISSUE: Bump github.com/ory/dockertest/v3 from 3.8.1 to 3.9.1 (#3901)
0bcad464f32ca3fafc7b072c9acd3a3bd6113497 NO-ISSUE: fix metadata for one dashboard and improve metadata layout for all dashboards (#3893)
2b56e8608e4b9d92faa9fc3763808f7160cfce03 MGMT-9175: Use an interface with a Mac address (#3880)
102b0a13b67f547e6676fde3c84a526507f537eb NO-ISSUE: Use Memory emptyDir postgres for faster subsystem CI performance (#3888)
2c282d859b9708eb846c278981141ca4913cb040 NO-ISSUE: Bump OCP versions release 4.10.15 -> 4.10.16, release 4.8.41 -> 4.8.42, release 4.9.35 -> 4.9.36 (#3887)
c7ae72f61192be33ac6b81dbc6acea0ff8277334 MGMT-10662: Add timestamp to get-next-steps and let the service use it (#3885)
a9170ed8487e828ebda0bf55ff62208580114e7c MGMT-10659: disable auto-assign test (#3882)
2811dad8750cff2995af50971b2323a1bc654bc8 internal/controller/controllers: label mirrorRegistryRef configmap for backup (#3884)
d1b3384663be5b48d9a57e0c1767419c86ef2dd3 MGMT-10643: V2ListSupportedOpenshiftVersions should not err for ValidateAccessToCPUArchitecture false (#3879)
cb07b9dc69f82143495b045d891c35e101386f70 MGMT-10631: remove Python dependencies auto bump (#3876)
b964e9f1f32c8bbac78672f034ac57bdbd53c42c MGMT-10633: BMAC should disable the BMH AutomatedCleaningMode in the converged flow as well (#3878)
18fcad2904816ba9023f2fec1550089989d5f531 MGMT-10632: PreprovisioningImage ImageUrl did not change after adding the proxy settings on the InfraEnv (#3875)
6dbae00c314345388407e8252591d226180d0321 MGMT-10281: Add documentation for the converged flow (#3873)
7c5da4c07d42c2b4708f3e7e2e12bc1c977548ed MGMT-8202: recalc suggested roles on host/operator changes (#3775)
d810eae0c15ec8a57570c541b51461f101ba2cc5 NO-ISSUE: Bump boto3 from 1.23.5 to 1.23.10 (#3874)
a09e3c459c684fb3e99eec39063cd2240ff7a987 MGMT-10195: ARM feature enablement for V2ListSupportedOpenshiftVersions (#3814)
4dae0b226c1dde6febb15d884449c6713fb854ce MGMT-10587: Revise wording for the message of 'non-overlapping-subnets' validation (#3872)
cc02f4ba1358b0de8244d77be26d7e3572296fe3 MGMT-10375: Get the ironic image from the default release image for the arch (#3868)
b5c877da797280fe7b25b5535f2a0805402233ef NO-ISSUE: Bump OCP versions release 4.7.50 -> 4.7.51, release 4.8.39 -> 4.8.41 (#3864)
15cca0fae0e3cc52cb8b083c0b2775a7b5ec5e87 deploy/podman: update OKD images (#3774)
096a0f99b15dbb9a5afb71c86c146617511f14d6 MGMT-10197: Adds ENABLE_ORG_BASED_FEATURE_GATES (#3727)
f66687d2b557bae350a58ca5b3e56ee20f099439 NO-ISSUE: update runc/ignition/bluemonday pkgs (#3865)
96765ee39dc83123a2c61b7212b8390a22760a3f Fix OCP image build (#3839)
eb83bb2f7df66fdb5670cf7e9c76288b757ed275 NO-ISSUE: Retry and redirect all curl actions (#3848)
284ef21780b9de4222bd4ca2a0e281f81f3ac321 MGMT-10004: Add UT for PreprovisioningImage controller (#3861)
47a40aa17cc04344095e89518a1ac13a608a1da8 Revert "MGMT-9259: Enhance the schedulable masters feature (#2861)" (#3858)
3c3ffb2a1991dcadd1050051fa06e897b7753b58 MGMT-10003: save-partlabel and save-partindex coreos-installer args are not honored because the partition is formatted previously (#3842)
eb82c28b3880a082fb8d0e61de7cd139478c569c Bug-2084410: Deploying OCP 4.8 on RHCOS with assisted-installer Failing validation blocks deployment with Insufficient error message (#3841)
4b0c4757f3032ea6038434ea55534cb6bedbcbdb MGMT-10473: Add interface type to Interface API (#3855)
a504baa6a35f79376709ecc78e50b3fb775a818f MGMT-10305: fix disconnect validation on bootstrap (#3838)
a36472aa756eb7a3675ea48edc093486209ea950 NO-ISSUE: Bump OCP versions release 4.9.33 -> 4.9.35 (#3857)
19ddb5bd0243a63ac5007b1979ef378e0df90068 internal/network: fix NewConfig to avoid throwing errors (#3859)
96b112e3b3f8d698eedc4198defa093e6d23a26d NO-ISSUE: skip vendor dirs generated files (#3854)
c2ce2d3480d8f18e803fb24c17f9b11473b7c10e MGMT-10493: fix gathering logs in ZTP flow (#3853)
5ae8f4d3d6b3638ea2724bf542bcf3ab828d4645 Bug 2089337: Fix the retry function to actually retry (#3843)
af26ffa209721231d40cb911b5afe88f039a9ed7 MGMT-10535: Set inventory+labels after inventory reported (#3851)
8cd065e97b8d2ce575ca7448ef7752a38571e75e NO-ISSUE: Bump OCP versions release 4.10.14 -> 4.10.15 (#3850)
fd41518b07cd7005ed8bce15777c42a72ad2f0d9 NO-ISSUE: improve readability for memory limits and requests (#3852)
e66b18b3ea9709616eca995eb091e66cb3e6710c NO-ISSUE: add 'generate-bundle' to the 'generate' target (#3835)
7d90320aef05b9bb7882186cafe0c838012638aa MGMT-10494: Make sure that SNO is considered when auto approving CSRs (#3832)
c978996463aaf0961cbd051c271287f432e1828d metal3 and ZTP convergence (#3815)
e45bc9bc1a92c28c86f4b774e7f435001c3c683b NO-ISSUE: Bump boto3 from 1.23.0 to 1.23.5 (#3845)
d8f86208b88d4f940c99c6f78360e0e0e1fd8106 NO-ISSUE: fix and tweak grafana dashboard about resource usage (#3829)
1611544bfc75d848b5c212cc1a73fabfaff750e9 MGMT-10253: Use a modern ignition version for our machine config manifests (#3773)
565a13bcd1ca10c7d66f2e305f9810be67e77345 Bug 2076333: Add clusterDeploymentRef as label to the Agent (#3826)
5126d93b1dc6e51ef84133780f50d131de916f9a MGMT-10458: Increase default timeout for agent service to 10 minutes (#3833)
27e6b7067bd30a37170710855a7f704b2afdc24a MGMT-10179: transient day2 misleading validation message (#3831)
4c5e3b3b7e1c39ff8cee5e78ed1e58890517a0c3 NO-ISSUE: Bump OCP versions release 4.10.13 -> 4.10.14, release 4.9.32 -> 4.9.33 (#3830)
3e8e1e863c7a091a0a4180279dd32509e0de256c MGMT-9574: Improve error message when updating static network (#3806)
c1eccd19b6f7a6bdd94639f074a675f6b4a43fcc MGMT-10264: In GetClusterInternal, do not bring hosts also from db unless requested explicitly (#3797)
ed1556c598732ff1621558a583bf61fa2011ab59 MGMT-10196: feature enablement enhancement doc (#3744)
367bc9451db75fbd5a8bbc13a5f1b98ef00800aa NO-ISSUE: increase memory requests and limits, and parametrize them (#3828)
fcbe615c34c6397ca11dedc42d521a05f3c936c4 MGMT-10275: When getting release image, let a single thread query it, and other threads wait for it (#3804)
2a05573785427cc77dbfb2a3557a193510021198 MGMT-8376: Inline notification for SNO text fix (#3825)
8f703827af15b3a585791a8e5d9dd0047c922819 MGMT-10347: Disallow capital letters from hostnames (#3821)
c821750cfecfbc62e8774289e8988fa8c49b7c9b MGMT-10263: Do not call refresh status from bm-inventory called from Kube API (#3796)
c3f90dc0fb25fd1b2497ceaf9348f625dd9b0c89 MGMT-9315: Create inventory cache during refresh status preprocessing, to avoid unnecessary inventory unmarshalling (#3813)
95758658dfe1ba70eeb1bbf68740646602568970 NO-ISSUE: Bump github.com/prometheus/client_golang from 1.12.1 to 1.12.2 (#3823)
b64fe2fd7a26cde5e27a1949e316f0ced82d1943 NO-ISSUE: Bump github.com/aws/aws-sdk-go from 1.44.14 to 1.44.15 (#3822)
7296f386338fe038eab9f7bf2463eac66eda7c63 MGMT-9259: Enhance the schedulable masters feature (#2861)
dbe941db78105d7cbdf827a6b1400686f4b0fe9a NO-ISSUE: Bump github.com/go-gormigrate/gormigrate/v2 (#3819)
1df12c082e044f862dcfe847d028918b76a16393 NO-ISSUE: Bump boto3 from 1.22.9 to 1.23.0 (#3817)
b50070f9c64138afeef7301a996f32854d767cc8 MGMT-9430: Remove v1Flag from V2ImportClusterInternal (#3812)
6382aa70347ac0e31c1dfbd6ed957be88d357acc Revert "MGMT-10174: Add node ip hint manifest for sno. (#3730)" (#3795)
cd9441ade2e2f52ce8b28d76e7df46628beb61da NO-ISSUE: Bump github.com/aws/aws-sdk-go from 1.42.53 to 1.44.14 (#3811)
b9ec6db2eb58e48022dd89c1d880ac7b1d934fd7 MGMT-9682: fix default disk size requirement (#3802)
7eeb0471742bd466d455f17ac19af3258effb9e3 Add .spec.[]osImages.rootFSUrl to example and docs (#3803)
8f7bc60886cbab86104063d54d2a0e99fd538734 Bug 2078531: Expose ipxe boot artifacts via HTTP (#3705)
ff812ad654f743c9c9a044c8b1e8cb6aca042d44 NO-ISSUE: Log stack trace when failing to recover (#3808)
fb997038c1495e1cd3b8a6e6c44300e15a718812 NO-ISSUE: Bump OCP versions release 4.10.12 -> 4.10.13, release 4.7.49 -> 4.7.50, release 4.9.31 -> 4.9.32 (#3807)
95b303964b3e2f16890d6c0930cb423c5d93ff00 MGMT-10261: For call GetClusterByKubeKey don't bring hosts (#3786)
f45e1b54d6a6b8b91f7127fb0937e7d08e8a187a NO-ISSUE: Add a retry in setup lso (#3801)
d11326d6e0e86f68566bf61432bd0ef49a5c0988 Bug 2083075: Allow cluster name to start with number (#3789)
424cea808c11a43eee184437bac03e851849f894 Revert "MGMT-9379: Do not pass "HA mode" parameter for worker nodes. (#3769)" (#3798)
c6655333325666f6456f5f1b044934d676a53dfb MGMT-8738: media disconnected flip again by the state machine (#3745)
ca348049145dd376158f693df0526e2a3ff6972c MGMT-9379: Do not pass "HA mode" parameter for worker nodes. (#3769)
e6407de4370b0106dca6a1d89dc1c799ea9944cc NO-ISSUE: Bump github.com/go-openapi/spec from 0.20.5 to 0.20.6 (#3792)
92b6c3b54b04afb665aa23959e86121c0844580e NO-ISSUE: Bump github.com/prometheus-operator/prometheus-operator/pkg/apis/monitoring (#3783)
218e14fdd6350915452413875cf9fb4927ace16a MGMT-10237: Add events and cluster metadata to cluster logs (#3778)
74612e15254732133a81085a8c8e91d21b745295 MGMT-9495: Remove unused isoeditor functions and isoutil package (#3691)
b15c0bd7598a36885d3c984272a6b359174ff484 MGMT-9452: Remove "command" from get next step api (#3779)
4f9bacfaa7ff3cac889921c97d090afbc9e51182 NO-ISSUE: Bump boto3 from 1.22.4 to 1.22.9 (#3782)
3fdefeeaf3848780223975cfcc28988a949635c7 MGMT-10160: remove cache for subscription access review (#3729)
6980ce2f1941950acadbebbf50ed85a72869d5e7 MGMT-9180 - Fix bad SNO OVN/SDN doc example CR (#3781)
12887492d6188b230d970413a236945e5769942a NO-ISSUE: Remove unused subsystem client agentBMClient2 (#3733)
f926daf41497b444d50112f6a3ec5497c2d0a842 MGMT-9574: Improve error message when updating static IP (#3767)
c1b6ed527e2de4f1110ef9ab840a318d9521599c MGMT-8796: clear msg about cidr range (#3732)
18a6a1f4dfded5222a902a26aae02c026769d4f9 NO-ISSUE: Bump OCP versions release 4.9.29 -> 4.9.31 (#3763)
1c3fbe4328a723a210af77a0821906b1c97c4c41 removing OLM operator must-gather from docs (#3776)
6b64affc50ca1ff771392af8850d853fac7c507e MGMT-10094: Update must gather images for the OLM operators (#3704)
2f82f2a21d94a21b39dab9909b51eb527afaf384 MGMT-9379: Service changes to allow day 2 workers on single node (#3718)
62465ab24f9b6ec01da8f0edaede4faeca0c6048 AGENT-104: Removed redundant command (#3770)
4780c78da601e3cee35a7488ec6a260f9aa16b88 MGMT-9020: Add install config overrides feature usage (#3719)
a125bbf9b5dc479f26b6d0f44ef5ed37bc3fdf24 AGENT-56 Client to read ZTP manifests and register cluster and infraenv (#3639)
5b655c143126bd0b90dcdce44d86fc553967e4f0 MGMT-9787: Add the built-in ipxe script endpoint to baremetal deploy docs (#3677)
31fc9396b44c70110905546005901e0e466ee6c5 AGENT-153: Add .ci-operator.yaml for OCP payload image (#3766)
398d2b2e4ccb69cdd57a2bbe827b03a823c9400d MGMT-10225: Update BUNDLE_CHANNELS to ocm-2.6 on master (#3762)
c74a8e331e06068fa3bfa2a6bc7fd35656a080ca Bug 2069976: Error with oc-mirror using an old outdated unsupported oc client in AI (#3598) (#3754)
84b83af19531313df8186ea4f075894fb518f9a8 AGENT-104:  Add Dockerfiles for OCP release (#3660)
876808b129e556ac56c904e8667e0e8ddc26457c NO-ISSUE: Bump OCP versions release 4.10.11 -> 4.10.12 (#3749)
763d20cb68010bd67731fc8db3e4a3af43aca5a6 MGMT-10141: On validation 'non-overlapping-subnets', canonize subnets from same interfaces (#3720)
142cf6e7a10508d47b8d99d08c2cb1011f26c734 NO-ISSUE: Bump gorm.io/gorm from 1.23.4 to 1.23.5 (#3746)
6272c78ae5cdcd782331b4cf0095b6c60368ba26 NO-ISSUE: Bump github.com/google/go-cmp from 0.5.7 to 0.5.8 (#3742)
6d637bc19ed5cd7ede00fc4de42bd0f925ae796c NO-ISSUE: Bump github.com/prometheus-operator/prometheus-operator/pkg/apis/monitoring (#3740)
c65a0eaabd5a3a62a2d6ff59d0a3d95b27499d26 NO-ISSUE: Bump boto3 from 1.21.46 to 1.22.4 (#3739)
e60395bd3ed7bd0e678753556337da6e914a6c11 NO-ISSUE - Add the ability to override image-service image when deploying the assisted-image-service (#3737)
40dce3a61138e2f602d3c6694df512146647eebf MGMT-8738: Media disconnection status doesn't updated (#3734)
a0ee380b3da1bb66ca674ae66638852f275b5722 MGMT-10174: Add node ip hint manifest for sno. (#3730)
741f59d4a7b4bbc7648aa0b3baf696fa2884bac5 NO-ISSUE: Use official Hypershift image in E2E test (#3735)
e973f877140823c4fc85ca73a003a21171529bfb NO-ISSUE: Don't use deprecated APIs (#3731)
178e8a358279f533bacd25620a4ce7ddfeae5069 NO-ISSUE: Bump OCP versions release 4.10.10 -> 4.10.11, release 4.8.37 -> 4.8.39 (#3725)
c9058f327ad8154edfe689eb5ce5f7372d81dbee MGMT-9227: Create deploy_capi_cluster script for CAPI CI (#3690)
3a25e0352232557768e99d2a486ba667e9fd8196 MGMT-10163: return StatusNotFound on non-existent infra-env (#3726)
2a4abf2d9177185d311d0d49a6c7f975e92ee0e0 MGMT-10109: return status forbidden for manipulation ops (#3723)
ddb6400f03c15526c39fa6a2b1bc1f1b7e6def92 MGMT-9060: Update arch doc with image service info (#3724)
4bc2b1407f988de8e1d8e93efe50b68ac0456dc1 MGMT-10142: EditClusterRole can delete objects (#3722)
5e5a31750330c06eab24193082e5a97c09ec0cf9 MGMT-9495: Cleanup unused code in s3wrapper (#3688)
0ad170900685838ba423d34db64faed81d4884a6 MGMT-9272 Automatic agent classification labels (#3721)
d3f6c4150c9ebbda01b380e1b6545920f677ad59 Bug 2068301: Upon modifyin DNS entry in DHCP server - SNO OCP platform does not update resolv.conf (#3717)
b31fbf34d02bf54e278276af53cea6a3e484baa6 MGMT-10029: remove generate-all target (#3714)
be92f28e10377f605f6f7be86028ca4e1c1dd67c MGMT-7274: Add Last-Modified to file middleware (#3697)
6f42cc283df155e341244589d10067cc669b5fcb NO-ISSUE: Bump github.com/pelletier/go-toml from 1.9.4 to 1.9.5 (#3710)
0680e64f9dbdde3f71096e414f1caaff92ef2cac NO-ISSUE: Bump gorm.io/driver/postgres from 1.3.4 to 1.3.5 (#3712)
6a06ad6e815dbe134a6e56461a45071a127a8317 NO-ISSUE: Bump k8s.io/kube-aggregator from 0.23.5 to 0.23.6 (#3709)
f274eaed6c230952d6cb483d364794a77a018319 MGMT-9561: vsphere disk UUID enabled validation API changes (#3666)
99c1b810143dc3402d5b7ab792e36a87fe4899c4 NO-ISSUE: Bump boto3 from 1.21.42 to 1.21.46 (#3707)
6927a94a20fb035ed2bcf3fe98fbec17812feab7 Bug 2077921: Operator deployment script doesn't wait after patching the Provisioning CR (#3698)
16809ba917115355b996e32138e14e0e624af48a Bug 2077162: Can not provision SNOs in a disconnected environment (#3700)
34b14e9447d0dd976a8a3bd62c8e3f71ca9cdcb1 NO-ISSUE: Bump OCP versions release 4.10.9 -> 4.10.10, release 4.7.48 -> 4.7.49, release 4.8.36 -> 4.8.37, release 4.9.28 -> 4.9.29 (#3699)
63c0e244c32af2078f6e0e8830ffb83de47ddda4 MGMT-9495: Remove unreachable image handling code (#3683)
f74ba9bdd99924146140c448982c3b925c2669d3 NO-ISSUE: create build directory for generate targets (#3696)
e185c6f4ceaa548403c1ac3702ba7a9643045028 MGMT-10062: Remove default service version (#3693)
881d46cc55bb8476386201fe85682c46b8618aa7 MGMT-9495: Remove imgexpirer (#3692)
2f0846ea8e5db9d3fb7c1157216f103050437887 Fix small typo in podman readme (#3673)
bdaedf995ba2e805bf0cd4b9850833a6b0d32478 MGMT-9460: Always use the image service in inventory unit tests (#3681)
0da8d3899d8e421a424a78816bbcc75b22683384 NO-ISSUE: Add a retry when fetching oc with curl (#3687)
9f463c8ac54821c57089dd68a86a27fce43b4e5b Bug 2076901: `pin-latest.py` script should exclude the postgres image (#3685)
ebe2d0c01995d7f8e739d5caa861ce66ccbe22b4 NO-ISSUE: Bump github.com/aws/aws-sdk-go from 1.34.28 to 1.42.53 (#3679)
2a5c18c6b49e617b88b4ca9c01f5c373a04374e4 NO-ISSUE: Bump github.com/slok/go-http-metrics from 0.8.0 to 0.10.0 (#3505)
b38ca2ad099174927f52e72fce7fd556c8f451d9 MGMT-8850: Don't copy http proxy to https proxy (#3678)
2721189702fdf8d4edda0d68bfdf5c0fe5418870 NO-ISSUE: Bump boto3 from 1.21.37 to 1.21.42 (#3676)
c8c713399f7dfb7c8883a4d8b9d67a6b4bc2407c NO-ISSUE: add a separate makefile for file generation (#3674)
42b015ea6262ad3c08fd735abfebc11d47469071 MGMT-9945: remove identity package (#3675)
dbb65071384ddda0b404648a3ec8560137faa43d NO-ISSUE: Bump OCP versions release 4.7.47 -> 4.7.48 (#3667)
78dea4c6d164e79f940da2f430c2d885b1da32bf NO-ISSUE: Add additional operator user guide doc (#3610)
8b65e2ea9cef88b60ce367ba1df4b9ce10557615 Bug 2073413: expose API/Ingress vips in ACI (#3663)
7b428ac914722b5ab7ebcb6d670751e42e050d91 NO-ISSUE: Bump OCP versions release 4.10.8 -> 4.10.9, release 4.9.27 -> 4.9.28 (#3661)
1d532a92ab339b44b1e1129f62edffb4b95eb171 Bug 2072728: ensure secret is labelled when it is being reconciled (#3658)
3e2fb637b89b27c6a48a81ad4b8ddab226724c50 AGENT-34: Allow preconfiguration of bootstrap host (#3627)
cdbb65b98076673d156f5a5b787bad9378528531 MGMT-5442: assisted-service should use official oc client (#3657)
01ee38750759ac1394e305466bfd2576f3031448 Bug-2072929: agent is stuck on pending input condition when configuring the network for a multi node/compact ipv6 spoke (#3651)
a785753f120ab0be9c46c0e883a751a32c706350 NO-ISSUE: Bump github.com/go-openapi/spec from 0.20.4 to 0.20.5 (#3653)
b71ea95444665a8ab9e13ed2f0652a492106aed8 NO-ISSUE: Bump github.com/onsi/gomega from 1.18.1 to 1.19.0 (#3656)
36a509d0075decdae0c0dc8a12200e0eed577088 NO-ISSUE: use upstream postgresql image (#3103)
96b2347f29be5076c8f154f7cbe4a75c06b76024 NO-ISSUE: Bump OCP versions release 4.7.46 -> 4.7.47, release 4.8.35 -> 4.8.36 (#3655)
3f8cdb3d13a8500a8b4da7c310e5a93e848a0901 Bug-2070838: Installation on baremetal SNO failed because 2 interfaces had overlapping subnets (#3642)
4eee641dccec201432e154189a67b09f719186e8 NO-ISSUE: Bump github.com/ovirt/go-ovirt-client from 0.7.1 to 0.9.0 (#3648)
5d948c72537caa755a5387147007ebfb2da879f9 NO-ISSUE: Bump boto3 from 1.21.32 to 1.21.37 (#3645)
a5203e397ec822e1f863e106027438f39372cabc MGMT-9799: Serve API spec on `/v2/openapi` and not just `/openapi` (#3644)
948402ec3d9ef7c91f65fea95329d02ac037dde9 MGMT-9934: Use compatible iPXE script format (#3638)
66ee39b1c1192e35dce7f9d4b3aba1c50336ca85 MGMT-9970: Upgrade gorm PG driver to fix segfault (#3652)
669dbe99e171fa75d6be3d5fc0e95c589c3fe6e1 add RDS dashboard (#3650)
ccc4f30c77f9d7649e5988eb3a58c79699996696 NO-ISSUE: move grafana dashboards to events scraper (#3643)
204c4aa79fd217622fb498256fe820e858517bff NO-ISSUE: Bump OCP versions release 4.10.6 -> 4.10.8, release 4.9.26 -> 4.9.27 (#3640)
423467bf8d78ae681726e09f78f12b43c812860d MGMT-9932: Remove unused events (#3636)
84fc7f0ddccb494bcf18d18a77aad65c55f793f8 MGMT-9778: align events authz (#3600)
497720b065a38612086a7badbec8382af450a6a3 MGMT-9758: replace AddUserFilter with HasAccessTo API (#3631)
88e2a3b85e38f036d71cd0cbc42087a611b2ca1a MGMT-9732: add user authorization to BindHost (#3630)
a14c20ca2c47f175df251634662c40960e9ad459 deploy: ensure that ServiceAccount is being created (#3629)
4cda26533d377f453f68783e8b2eae438734555d MGMT-9365: assisted kube-api SNO clusters should be converted to… (#3404)
63aa008800aedfd2e51d8c97cc54c1f8fccdfb3c MGMT-9810: check cluster update authz in RegisterInfraEnv (#3632)
72d13cb0c39f8deed221833cad100821cdf3396c unit-tests: support running psql for unit-tests in k8s (#3508)
53616082111984bbb43f4c848f7ce11c915f579f Bug 2069976: Error with oc-mirror using an old outdated unsupported oc client in AI (#3598)
ca4ceba382fd6d4e19f8f7819568da82a8ba4ee0 MGMT-9912: Handle a nil cluster_id with events that have an optional cluster_id (#3623)
ca0fd76bda34494b16b324fed645f1a82135d7e2 MGMT-8741: Accept full name OR tag for agent version (#3633)
96f97b3b46f4afd775d385f15612e1a9db60f8a2 MGMT-9673: Add HasAccessTo API to authz (#3622)
b42e7eb036f86770c55a94eed5cba8e4324c93c6 NO-ISSUE: Bump OCP versions release 4.7.44 -> 4.7.46, release 4.8.34 -> 4.8.35, release 4.9.25 -> 4.9.26 (#3607)
5cbb6f561811411036208f8e03941ac2c6ed56fd MGMT-9451: Move cmd commands from service to agent (#3554)
0cb3eb4601060c9a4111a3bc99da3c9cc086d115 MGMT-7340: add labels to the v2 update host api (#3358)
094b59997ad01891276aa020314d48212183ccaf MGMT-9747: adding image validation regex to steps  request objects (#3609)
fd010d669fa32b3fa0186e5c6a3e14db4d4861dd Bug-2061317: when using nmstateconfigs ISO is re-generated for each nmstateconfig (#3621)
2e392fa7c43116c2ed9b4a68508fa82d26399ee3 Bug 2069101: fail sno deployment with SDN (#3595)
6a28aeb0f6632a2e08d91b1984347cbfeee7a711 Bug 2030480: Handle incorrect rootDeviceHints instead of ignoring (#3606)
b365b892b2288e4c4914224e3e3a18db7e84f24f BUG-2063814: Set progress_total_percentage 100% alongside cluster status installed (#3519)
d784d4f8c8d5d3afb4df48a4e98585c04a3217ea NO-ISSUE: Bump gorm.io/gorm from 1.23.3 to 1.23.4 (#3614)
29236b32130c6d17c9f8dbabf38b342516f0eb36 NO-ISSUE: Bump github.com/openshift/custom-resource-status (#3617)
52e4ea26a46880e826d8d213f102dc4497acb9ab MGMT-9672: align manifest authz (#3510)
9799d7f81969b70c7f1a7f4654eec76d171868c1 NO-ISSUE: Bump sigs.k8s.io/controller-runtime from 0.11.1 to 0.11.2 (#3616)
af6b1e9cbd40822dbab63b6198abf9c3975b7573 NO-ISSUE: Bump gorm.io/driver/postgres from 1.3.1 to 1.3.3 (#3615)
5540f945bb7a6b4aa393ab3e28ddb8ec2e12c11b NO-ISSUE: Bump boto3 from 1.21.27 to 1.21.32 (#3611)
0bb6463a94fbeec912e0ea7de4d7aa5e61f57ffd MGMT-9673: Ownerhsip API to authz (#3550)
e54185050dd372cabd3167fd0667818fe1770cef MGMTBUGSM-216: improve ClusterImageSet sync error message (#3571)
87616d920e04325a92716144c05976d110ea0ec8 MGMT-9779: Call cluster-info with a namespace (#3585)
dc8f223569f42e02a053c6f547ea2eb41c20b00a MGMT-9453: moving part of validation logic to pkg to use in agent (#3599)
f509fa873795196d60462f0bea08afe73a5342bb WIP MGMT-9726: Wait for assisted-image-service when deploying the operator (#3597)
c28b509ea28fe92698b0d51a438c37fec87c045e MGMT-9793: Include an optional cluster_id for image_info_updated event (#3587)
9c27bb66abb97a9c4a946e484fde19ab8664cf2e Bug 2065034: Correct ignition validation message for day 2 host (#3562)
d7777c518a6c2a79c7a83a5a08e1d361a09f3e62 MGMT-9172: Misleading "No networks found for host" errors reported for hosts which don't have any IPv4 addresses (#3590)
597bd8209aebf12328768d85d1a5031e6d935f34 NO-ISSUE: added arm64 images for ocp 4.10 (#3566)
a9007bf76adf3503fe4a56a7a86670db85a5112a Revert "MGMT-9272 Automatic agent classification labels (#3516)" (#3594)
7b43bbd4c5eccf273205f2fbdcab04f9335da358 Bug 2066559: Host status change to insufficient when binding a host to a cluster (#3570)
264304b2c9958064aec808bfc956682dcf7ea07b NO-ISSUE: tenancy authz - added PATCH cluster test (#3588)
b8aa0b95615847c42434c46b6a08678b3d5d4476 MGMT-9532: Remove remaining references to ocpmetal quay org (#3559)
4a53caf5c08d8518efd8592f9f91462d39308423 MGMT-9272 Automatic agent classification labels (#3516)
6cbfba8c4be77b0a6c3a18c1c9dca9a959f8e65f MGMT-9532: Don't set openshift version in upgrade files (#3561)
9a8432287116458e0fbafdfc08311c06134a6450 NO-ISSUE: Bump github.com/stretchr/testify from 1.7.0 to 1.7.1 (#3584)
dc59fc0581c82393913628f8a734b662ba3a3ec9 NO-ISSUE: Clean up remaining references to onprem-iso (#3555)
d352a0454fcd7fee2dd4622bf43dcaef20c9b7d1 NO-ISSUE: Bump gorm.io/gorm from 1.23.2 to 1.23.3 (#3582)
900fd6ae4c53aae2e6a16fcab7623ba3570c6011 NO-ISSUE: Bump github.com/prometheus-operator/prometheus-operator/pkg/apis/monitoring (#3580)
afd8849feee8c450ba02085f16e723429ae32a6f NO-ISSUE: Bump github.com/golang-jwt/jwt/v4 from 4.4.0 to 4.4.1 (#3581)
6d6060682f65dae2f78781daa7d97448e6bf375a NO-ISSUE: Bump k8s.io/kube-aggregator from 0.20.0 to 0.23.5 (#3579)
a0bed03db9300df1b29ce07b5b99c1e6ba812984 MGMT-9779: CI - Retry cluster-info readiness (#3572)
429c4d9dc15a5a8dd2a9f37aeb0e694afaeb49d5 MGMT-7365: Deprecate single network configuration fields (#3560)
088945759dce3b0c360090c9bb020923b5b47f89 MGMT-9776: [Assisted-4.10] [Staging] multi cluster - installation failing (#3574)
a3236f55d33fceb4ad7616f504688ba44a67de81 MGMT-9742: Populate VIPs and Networks in cluster creation via KubeAPI (#3553)
ab1b628db7183d64371515e9729c995476f8a5c3 NO-ISSUE: Bump boto3 from 1.21.22 to 1.21.27 (#3576)
d553715a1f6296d50952917fb7b24b5cfc4dadf1 MGMT-9733: Allow updating image-file in UpdateHostInstallerArgs (#3546)
a314b89e470e47ccc91651ae6775f3727bf95870 NO-ISSUE: Improve `Makefile` & documentation around subsystem tests (#3491)
376863df26b986e55cbbe4014d76c6ac89706aec MGMT-9034: Allow all domains for CORS when deploying locally (#3552)
d7bfdd40e98136a8b6751a79df65cb77a5fd3877 NO-ISSUE: bump github.com/moby version (#3549)
d7f1f0923b2568047789eb8789fbc4e7de48c251 MGMT-9451: Move cmd commands from service to agent (#3569)
e3ec424115f9758e4094970eab739eeeed2b3de5 MGMT-9451: Move cmd commands from service to agent (#3564)
4fed6b094b39debf61d109e2b034c6091535dbeb NO-ISSUE: Remove docs site (#3558)
c9bac2133c96bd9dfbbe403bbd25029c863a8d9b NO-ISSUE: Change default release image to 4.10. Update 4.10 os image to 4.10.6 (#3545)
27ed29f80418d11952c8862ce5005771c11a308f MGMT-9559: Using vSphere integration creates extraneous machines and machineSets (#3530)
5a3e100e2b938ed7873e233eedaf73579011c1a7 Bug 2066196: ensure secrets have backup labels (#3493)
5678e83529a7500af2c8d44ae82491da2eeb1223 NO-ISSUE: Bump github.com/hashicorp/go-version from 1.2.1 to 1.4.0 (#3503)
eca0436925dbc650ea49e01f85f7d9e2fd355bf0 NO-ISSUE: Bump github.com/containers/image/v5 from 5.7.0 to 5.20.0 (#3433)
95a25559d1e2b720aa5669c75fd5651a7108dbd4 MGMT-9734: Fix networking issue while trying to get cluster's current release (#3548)
b89d3f657007a8eeed029c2efcc60368924ccbdd MGMT-9478: expose enable_org_tenancy feature flag (#3543)
b63ae39933e6e38a8b87578ad2bb5ffc100bd5de MGMT-9404: remove user filter from UpdateHostApproved (#3547)
f28bddc8d95a89a4804b77b362dda721e3e14214 NO-ISSUE: Bump github.com/thoas/go-funk from 0.9.1 to 0.9.2 (#3539)
57840eec840104a0b92377fe17e8fd62c4b2280e Bug 2065288: Add support for Ignition overrides for day2 worker (#3524)
6c91f0669c43876ce51a69fce79ad0d72767d804 NO-ISSUE: Bump github.com/golang-jwt/jwt/v4 from 4.2.0 to 4.4.0 (#3540)
38d14fc25507feeaad75be9aed0e711e38cb5201 NO-ISSUE: Bump k8s.io/client-go from 0.23.4 to 0.23.5 (#3538)
f0d92cd4e34945bbcdfe5c6752bceada03c5b9b4 MGMT-9684: Create a new API call to get cluster hosts by filters (#3535)
6b832323a408ae99bf8e185809a47e4561fbe608 NO-ISSUE: Bump github.com/golang/mock from 1.5.0 to 1.6.0 (#3359)
9ec1acc56abe92685897f3a35ade7f2f7432d751 Bug 2055333: gc api server when controller is done (#3532)
a97a9ccc95da83cd55149bef4f69b5e7d1fb4b61 MGMT-9371: added filter_by_owner query param (#3512)
0fc8657f923c9b92b06197aa3a308e3c0c934ad4 MGMT-8300: Allow API VIP on cluster creation (#3258)
6418537437e3bcb7b1b5174dde3741984032a105 Bug 2066786: Set the correct stopping state for a day2 cluster. (#3531)
1d5c5542cfa6accb320331ceff62f74f4fcbe959 NO-ISSUE: Bump OCP versions release 4.10.4 -> 4.10.5, release 4.9.24 -> 4.9.25 (#3525)
ee56de1f3eb3fb9e69010a0e9c3280a2d0c0fa36 Bug 2066917: Set boot artifact URLs in infra-env (#3480)
be71c270482f69acb81d541160195136a7e430db MGMT-9683: don't mark vsphere installation with Cluster-managed-networking-with-VMs (#3517)
7a3dbd34524b2a0744cf4cdbedc1a21558ed7576 MGMT-9511: Removing reset cmd as it is not used (#3434)
1d53d8135834d2905407dcfe0edce4719ccd08e7 NO-ISSUE: Reduce build image size with yum clean all (#3527)
3329e2b1a532bef406d8d544a884dd54a7b805b6 MGMT-9653: Update Assisted Grafana dashboards V2 (#3496)
ee3b8bf8f8180a35783d04c64953bbbd390a7f1b Bug 2035638: Stop BMH reconcile if InfraEnv label is missing (#3228)
916ac43d64dfe85dde2b0ca927ab424dfdee7452 MGMT-9687: mark CPUArchitectureARM64 as fully support on 4.10 (#3518)
da8c67894df55dc36197195dfcdba5be5d446346 NO-ISSUE: Bump boto3 from 1.21.18 to 1.21.22 (#3521)
176ca4ee2d605531e6c01ea1b37ae98126fe22d0 MGMT-9443: tenancy based auth. (#3482)
7587c104f0f6f378f20b8af082a926527778ab33 MGMT-9443: tenancy enhancement doc (#3473)
3cb261a2cd26706f5c8b4bb5bcbb6cf6134a9c15 MGMT-9403: cluster editor wiremock stubs (#3486)
22a28ccdcbe4117843feb52b5ac43e6b63340ecb NO-ISSUE: optimize build image size (#3500)
e251185323c16862f4898380895e0954e86180b0 MGMTBUGSM-181: ipv6 spoke cluster installation would fail when unchecking 'use advanced network', due to ipv4 defaults cidrs (#3501)
4f446b7d3b02b99fdfda89ddb680a294c3a809e6 Bug 2065661: `pin-latest.py` should allow a custom tag to be set (#3507)
96eaedb04edf2561ba50d0562f5f73a44f6acb60 NO-ISSUE: Bump github.com/pelletier/go-toml from 1.9.3 to 1.9.4 (#3431)
9065015fad447944459dbb48cc50689c0d27bbfd NO-ISSUE: Bump OCP versions release 4.8.33 -> 4.8.34, release 4.9.23 -> 4.9.24 (#3498)
044d6d694570abbdaa5ebee8f5c682c1e65a051e NO-ISSUE: generate CRDs in root and api dir (#3499)
e8cbce5d54eef0b322237374ff6d3d2985058b0f NO-ISSUE: Bump github.com/prometheus-operator/prometheus-operator/pkg/apis/monitoring (#3472)
f9bdf7e4a499a50a9ba76652a4faaf1a41efe777 MGMT-9369: filter clusters and infraenvs by organization (#3483)
608ee245463dcc15b131af2059853bcd11b3ef7d NO-ISSUE: Bump boto3 from 1.21.13 to 1.21.18 (#3477)
25546b98632214dafd8a5885a501fbc74be982ad MGMTBUGSM-191: Race between agent and clusterDeployment reconciler causes day2 host installation to ignore requested hostname (#3489)
c0c4d15bd32fac63c48e30908516d7cf92109b46 MGMT-9528: refactor code-generation scripts (#3490)
df53f0d41eed8b02e601c5c274ef0c7c4b97be27 MGMT-9539: Add presigned iPXE script URL endpoint (#3460)
cb48591dee6f39382362922d6354743574b7454b MGMT-9566: Improve UpdateInstallProgress performance calculating cluster progress (#3464)
f25794323bc183b060720a80428e98b764ac75a3 MGMT-9609: Remove V1 discovery-ignition-params (#3476)
8d81418a72d85143c1822df720877f6b6ea583d5 MGMT-9468: Add dashboards for events scraper and elasticsearch (#3488)
beb1c41cf66b5a1fd0e8e8e7f83af15f5f8c5d88 MGMT-9279: Remove assisted-service database timeout (#3355)
d45305aa6fd4423864c340fd66e068df0dc0554a MGMT-9314: Reduce the amount of agent updates in agent and BMH reconcilers by updating only agents that actually changed (#3462)
2bbbcb60eea4ea5a782bde995bdec3dd7dfc1f62 MGMT-9470: Make script to pin catalog compatible with python 3.6 (#3479)
241ad46db74add5f16e153f5f7ba0a5496fb06ba MGMTBUGSM-112: validate ImageSetRef in ACI webhook (#3425)
9afe0556239abbe491a45f9dcb8fb3c9b854c3d3 MGMT-7231: Deploy ODF operator (#2932)
f7a0e41f25b6121ea1862f02ff67a126ec0921fd MGMT-9584: Remove V1 middleware (#3470)
fade32b970bfa6f560b9dc623711f05042bcc935 NO-ISSUE: generate support rootless podman (#3474)
141adc8ae8f8cd993b04b6a804b91c4586a0cb38 MGMT-9277: Optimize connectivity check post step reply to improve load for large multi-node clusters (#3463)
91ecdf8db859a9ea0591cd0e645d5436c10e8c18 MGMT-9458: Remove v1 operation ids and definitions (#3423)
b2f4685e336d07b0a22816284e4bba03932fc1d2 NO-ISSUE: sporadic ci failure to get epel metadata (#3469)
73eae49ea594a6f2bc30d2d23774a9c9c32a6e09 MGMT-9577: Upgrade gorm to v1.23.2 (latest) (#3465)
4cc73ff81d0f0099af351aa9d697fb3cf0f4ac42 MGMT-9470 - Add a pin-latest.py script that pins catalog dependencies (#3468)
a0cd7ef3632b5dfb1877e90e1a20a10e221621e2 MGMT-8809: Fix e2e-metal-assisted-operator-disconnected CI job (#3445)
e574bc2de2fd3153c7454604e32d7ee7664c1d78 MGMT-9177: OVNKubernetes as network type with SNO (#3419)
2737156feb3dfcc304e8337a7548c05d84cdc9cf NO-ISSUE: Bump OCP versions release 4.10.3 -> 4.10.4 (#3461)
c77aa8147cb5fc553ecb32b882360ec5797da7b1 MGMT-8571: Deploy the image service as a stateful set (#3067)
2f81d62160a56a9a25581376fbbe556342aa44d5 MGMT-9550: Fix automatic agent inventory labels (#3452)
3ded92e519bafc816811607afe70bd53a85df738 MGMT-8824: Copy additional NTP sources to chrony manifest. (#3441)
29d721c7cc27721b87e2b04961ab33b33532ecc3 MGMT-9546: update OKD configuration to 4.10 (#3450)
b691fd46cc454c59a43853387f920231744ddcd3 MGMT-9334: Add an endpoint to download an ipxe-boot script (#3446)
737483a7cc47ebfe076ef62f0fbb1661af1af831 MGMT-9556: ZTP CI fix: increase the timeout clusterDeployment installed status (#3456)
2a6b243fce2d4191881b7d851ee5777560bda172 NO-ISSUE: Bump OCP versions release 4.10.0-rc.8 -> 4.10.3, rhcos 4.10.0-rc.1 -> 4.10.3 (#3455)
c183b5182bfed15e42745e9f7fd3bd4f21184bde MGMT-9540: Add iPXE URLs to InfraEnv CRD (#3454)
76f457bb292bcbcf590ccca5ca8d86a2e686c974 NO-ISSUE: improve docs: mention minikube tunnel (#3326)
bfd7e20a75c9f236964a1b7629141e5b6a7baccd MGMT-9221 Automatic user-defined agent labels enhancement (#3426)
23f7f03918bcea2111ed2686fae67f4d3190b71d MGMT-9467: Port authz_handler unit-tests to use V2 APIs (#3421)
f7055f0458c6b0aff62bb48bf24020e4b6cc1d0c Merge pull request #3457 from omertuc/empty2
fa85514c7f133a9b738cfd374be1308088328680 NO-ISSUE: Empty PR to trigger CI promotion
8e02d03aede63820ec4a8b532cd2f59cfebe30fb MGMT-9541: Fix mismatch swagger-codgen versions. Set both versions to v2.4.18. (#3449)
5d4d836747862f43fa2ec882e5871648bd12c780 MGMT-8794: refresh hosts on cluster update (#3424)
c5eacda676475f5a6de123678c1af353a2368bd3 NO-ISSUE: Bump boto3 from 1.21.8 to 1.21.13 (#3443)
d74a8a779760353c462068f060433f83c4c6905d Merge pull request #3442 from omertuc/empty
8a60446afa8c39fbf4bfefaa42296d5b09114bff NO-ISSUE: Empty PR to trigger CI promotion
2edbd071ab36b2904a97b46c048feaac69bef305 MGMT-9527 fix generate-bundle after moving api to sub modules (#3436)
1a370c7f9fa1a52dff33baeba972118c8c4c162e MGMT-9485: validate manifests names uniqueness specified configmaps (#3429)
0e229dea8672ef2e5275563c493a42867ea70985 NO-ISSUE: Remove mocks missed in previous PRs (#3435)
aab26021129ad5b8546c7ad2534a3281bfdc3d2f NO-ISSUE: Bump OCP versions release 4.10.0-rc.6 -> 4.10.0-rc.8, release 4.7.43 -> 4.7.44, release 4.8.32 -> 4.8.33 (#3430)
8c54328a19e2967cc1d111c3a2ad808fc978c546 MGMT-9357 splint api dir into a sub module (#3406)
6e1e9136084a6e4fce574000a0aab694ed3cb6d8 MGMT-9110: remove v1 UpdateCluster (#3427)
7324baa9dff91913dd393d1dc686259643d17f57 MGMT-9014: Fix OpenShift Virtualization disk validation message to contain GB (#3323)
94629d402d8789d6c051e238a141de486e531d30 NO-ISSUE: update day2 API doc (#3428)
877fea70eb4b3f341639e30bfd95c6da1c6e7e78 MGMT-9383: Add enhancement doc for iPXE boot (#3389)
0161c1881d103f08bfd403fdc53aa0517bde9ba1 MGMT-9409: Use AdminKubeconfigSecretRef if available to get secret name (#3411)
1e3df7d8791469f541e3268fb8d8f740b1897be7 MGMT-8879: Add ZTP None platform day2 flow (#3409)
a5ea1f489a477e939430558fd7a14982d2a00e0d NO-ISSUE: Bump OCP versions release 4.10.0-rc.5 -> 4.10.0-rc.6, release 4.9.22 -> 4.9.23 (#3418)
279813c706ee46cbdf9fd6446805b3686c59951b MGMT-9115: Remove V1 GetDiscoveryIgnition UpdateDiscoveryIgnition (#3417)
61c15559e0190a0c4800b877111d67bc31b02239 MGMT-9192: Unify spoke client to be a single client in assisted service (#3388)
1d025b8108f016038d6c2dcf444b9314aefdadcb MGMT-9206: Allow arm baremetal platform installation (#3345)
01aef1f8361609863f4e97cf7b77d0b18447150c MGMT-9424: Add to swagger api to transform cluster from day1 to day2 (#3408)
483d52644b50f652f6c96e6f614734e24f3353ad MGMT-9108: Remove V1 GetPresignedForClusterFiles (GET) (#3267)
d65126edf8b377d63f2074c535aaa702753a98db MGMT-9126: Remove V1 GetHostIgnition, UpdateHostIgnition, DownloadHostIgnition (#3412)
e32309591c61d6de29db0255ae56a2f419085eac NO-ISSUE: Bump boto3 from 1.21.3 to 1.21.8 (#3414)
f73f9a01ce9e599be135ea4f6a7b6641011f82d8 MFMT-9109: v1 RegisterCluster cleanup (#3405)
b4fbb246dc8415baf13fccbf37e48174d0d2063d MGMT-9376: Remove V1 ListClusters, DownloadClusterFiles, GetClusterDefaultConfig, ResetHost (#3393)
8abaf20cc108f84ad5a384c0848cee4ef53d1914 MGMT-9123: Remove V1 UpdateHostInstallerArgs, UpdateHostLogsProgress (#3410)
894879243da8e49662537983d0ee9a5d8f437c1e MGMT-9110: v1 host related UpdateCluster to v2 (#3407)
07f48bf9e875bee43df80a928210fe6a615ddb7a MGMT-9393: Close file before passing it to nmstatectl (#3399) (#3397)
ad327c2e5a795d07b508066256e8b0d99b2b3ad0 MGMT-9416 - InfraEnv should not use any NMStateConfig if no selector is specified (#3403)
6f0ef47baf6b8f349199188ee9758230ae4ca2cd NO-ISSUE: Bump OCP versions release 4.10.0-rc.3 -> 4.10.0-rc.5, release 4.8.31 -> 4.8.32, release 4.9.21 -> 4.9.22 (#3402)
ddeba91c7acbce35c8771dea3738b773d0dada5f MGMT-9122: Remove v1 DergisterHost, GetHost (#3401)
ff377867173422ac948814eb68c36782926ccd12 MGMT-9121: Remove V1 operationId ListHosts, ResetHostValidation (#3390)
fc17703e07cb1e8ea21116e637d8ee5f5a54e64c MGMT-9122: remove v1 EnableHost DisableHost (#3387)
d0366715fc9668190a075c64ba9402ecf7ab703f MGMT-9111: Remove V1 operationId GetCluster, DeregisterCluster (#3370)
dd87a26dbbb97c2ec2f57351edfa3fcba867bf59 MGMT-9393: Close file before passing it to nmstatectl (#3399)
67fb740bbf7bbd90a463f9042d03e404710f931e MGMT-9118: Remove V1 UploadClusterIngressCert, CompleteInstallation (#3391)
a20076169975941dc1a7c07cc66aab9aaecf1c4b MGMT-9132: Remove V1 operationId RegisterAddHostsCluster (#3325)
0b12240b7b71ecf12a50272db17b53bc6675849e NO-ISSUE: Corrected indentation in example. (#3398)
908283e3eba780ba8c799c37e839e56d7ee58b59 MGMT-8447: Remove GenerateClusterISO API (#3320)
ce4f2118ccec55e7f1e0bb3324a5096b83b65a29 MGMT-9356: Add go mod to models (#3385)
6de51fc7116f506d8cbdbd639d518603d14be4a8 MGMT-9125: Remove V1 operationIds UploadHostLogs and DownloadHostLogs (#3382)
f3d4112b9d1adbda8a36bae93c2b670612bf6d56 MGMT-9202: AgentClusterInstall - support multiple manifest configmaps (#3342)
d57892341f666016bdc3b22c5f7b0d28b1e9b81f MGMT-9185: clean openshift-version object in swagger (#3386)
c82bdc8f325b6ac5af11eb79fb93db779aa25adc NO-ISSUE: Set release and os images by a given version (#3380)
51f7d21bd33b8ebfe5b3a359fb5a41d7d4cbc7fd MGMT-9109: Remove V1 RegisterCluster (#3304)
7ada9949bf1db860148bb8aed4e842f2a8284b9f MGMT-9225: Change the format if field StaticNetworkConfig in infra-env to JSON (#3381)
8a30d0214521f3a3c61eb68f94e4072e52333a5a MGMT-9223: Automatic agent inventory labels (#3344)
f7548e590f8a6b09b40cd2c4c95c9e3b31f61472 NO-ISSUE: Bump OCP versions release 4.10.0-rc.2 -> 4.10.0-rc.3 (#3372)
10a74aeff67a9c5c3bd45504b8195511bfbe5817 NO-ISSUE: remove all Jenkins jobs (#3373)
744ab8b3b5b75da8675ef4438888dc1dc995f572 MGMT-9122: Remove DisableHost from subsystem (#3371)
c8086dc4d1c45872345f725b0788b45e4f3b5bbb NO-ISSUE: validate api/api-int when ENABLE_SINGLE_NODE_DNSMASQ is not set (#3361)
119eb1c1497accb87b7a96ea1d66757846def5f1 NO-ISSUE: Bump boto3 from 1.20.54 to 1.21.3 (#3375)
e0f9e1d46789981cba34ce6adf3504e900a1076f MGMT-9134: convert update hostname to v2 in subsystem (#3367)
10618e15b47e334695f6c648d94595114bf54178 MGMTBUGSM-98: Prevent nil pointer error when cluster ID is nil. (#3365)
49d11b7f9850ff545bca242db71c5e35495853ea MGMT-9119: Remove V1 operationId InstallCluster, CancelInstallation (#3363)
263f4ef94cd295d2bdc77536bb596cb31c8087a5 MGMT-9131: Remove V1 GetClusterHostRequirements, GetPreflightRequirements, ListManagedDomains, ListComponentVersions, ListSupportedOpenshiftVersions (#3364)
fe16c558e937d464429fdbb389c1ebe07cef293e NO-ISSUE: Bump OCP versions release 4.7.42 -> 4.7.43, release 4.8.29 -> 4.8.31 (#3369)
67e0bc1275f07acf46a2f4531f6984e6f7edb7f3 MGMT-9134: convert image_test to v2 (#3366)
bfcb3c0a7ef9a7c25d8f6d7615f7946ca823b167 NO-ISSUE: Bump OCP versions release 4.10.0-rc.1 -> 4.10.0-rc.2, release 4.9.19 -> 4.9.21 (#3360)
81e2525ab98d40d9d78f3311450493c581f49f5c MGMT-9120: operationId Remove V1 InstallHosts, ResetCluster (#3343)
b650b7d5671e7552ee0e190d675375e7b3e35837 NO-ISSUE: Add @vrutkovs to OWNERS (#3362)
14d13e635de6ae3731393d12f8cb58ef5429d676 NO-ISSUE: Guess compression tool used and improve scripts (#3349)
78f640c3ba3792eca41150fba58a43890807ef52 MGMT-8447: Remove assisted-service-iso APIs and implementation (#3331)
210136a4778324c3f78bb64bf08fae6209ddc467 NO-ISSUE: OKD: expand /var if its less than 6GB (#3356)
a0829e23af077bec76193fcbc1f212014dce84d1 NO-ISSUE: updates docs for running with podman (#3312)
e82a65b81f47032d1fbef700174727831d906e0f NO-ISSUE: Bump gorm.io/driver/postgres from 1.2.1 to 1.2.3 (#3351)
9eade0af2b2f6fdf7d7622439cede754bb373bc6 NO-ISSUE: Bump github.com/thoas/go-funk from 0.8.0 to 0.9.1 (#3354)
389594044fcfd5fc8e83830d779d66b45062235d NO-ISSUE: Bump github.com/google/go-cmp from 0.5.6 to 0.5.7 (#3352)
51129bc9f0128c757c4aff5176a2f790dd29666e MGMT-8582: Leader elector based on lease lock (#3335)
a4aa8cffed5368ac7ab88c4da27aee375fcd791a NO-ISSUE: Bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5 (#3347)
5a941dc79d1722280c4178b776d0b1ef2b62af07 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.21.1 to 0.21.2 (#3346)
ccd8534a7501c77c5cffb9da30561a0b8a6dfe58 MGMT-9233: set MachineConfigPoolName for day2 (#3338)
3ecf7c908ce0efd05ad1b9e6cf117ca2d361070b NO-ISSUE: Bump gopkg.in/ini.v1 from 1.51.0 to 1.66.4 (#3336)
305f006b44e9b94b1da70f92e7faf8a5177fc58d MGMT-8380: stop setting custom manifest flag for operators (#3290)
46bcdf323df44a48bc783be738b2e97f23497cba NO-ISSUE: Bump github.com/ory/dockertest/v3 from 3.6.3 to 3.8.1 (#3306)
2e54017e3a17eff608a99b09c66991893337ee1f NO-ISSUE: Bump OCP versions release 4.9.18 -> 4.9.19 (#3330)
20b836b79d3e58ba573078461359ed160a9ef6c2 MGMT-9109: separate clusterID and infraenvID in register host utils (#3328)
db120df6fe2b278b079661c059fe368685913727 MGMT-9124: Remove V1 UpdateHostInstallProgress, InstallHost (#3327)
736677e11963a01fb7980d22db707b8f5fdbd28a NO-ISSUE: Bump sigs.k8s.io/yaml from 1.2.0 to 1.3.0 (#3303)
3ea1dca46eda37425185b7fa74681f0559cd7671 NO-ISSUE: Bump twine from 3.7.1 to 3.8.0 (#3300)
c7b04102554aa8f884321c928fcdb053833bc50b NO-ISSUE: Bump boto3 from 1.20.49 to 1.20.54 (#3334)
4f3f3f52fd4629cdcd59fae93a7710094735fc68 NO-ISSUE: dependabot is a trusted app so no need to tag 'oktotest' (#3324)
82016621ee76ca2bb1ea6bc9cb59702ab8622c2b NO-ISSUE: Add example of manifest which preserve data (#3283)
82a6451617ad7e0d1c09450827df7a880def1f71 MGMT-9233: disk validation fails for day2 hosts (#3322)
c1a6e0476f7bd6c56018fbb5b42900cfa257513c NO-ISSUE: Add OKD support (#3297)
db0d9d767d27d32a9690b5362df3f6be817870c5 MGMT-8447: Remove DownloadClusterISO v1 API (#3321)
9c187edf97da5b81a6e98ca7d8ba640238bf3aa0 MGMT-8447: Remove template image upload code (#3319)
62bbb3e1d6c6ebde72840f92d79303837cfde364 MGMTBUGSM-85: Change occurances of "API VIP connectivity" to "Ignition (#3318)
38cf1812f651dc6418e04d74a4cecf62c2f2306d MGMT-9127: Remove V1 UpdateClusterLogsProgress, UploadLogs, DownloadClusterLogs (#3314)
133ed9cf68e36590f19901d71813399bb86b165b NO-ISSUE: Bump OCP versions release 4.10.0-rc.0 -> 4.10.0-rc.1, rhcos 4.10.0-rc.0 -> 4.10.0-rc.1 (#3309)
315721f475805f2fe7fb3c6cca4814587a74e30f MGMT-9129: Remove V1 operationId ListEvents (#3305)
a10a12b7b1652e2a6b6e0c7961d0af8d22b9d274 MGMT-9117: Remove V1 operationId DownloadClusterManifest, ListClusterManifests (#3315)
5411af1f838187238c41e8fa94741c29ad87b5c7 MGMT-9116: Remove V1 operationId CreateClusterManifest, DeleteClusterManifest (#3313)
b2907295956224410f3572858eb2e72a84586c0f MGMT-9109: convert update role to v2 in susbsyetm (#3317)
3d29b3e13633046c05ef7e5d65255caeb2a8f431 MGMT-8047: Approve the CSRs after the installation (#3169)
7ea3e5c083d0c1395804c037683970f4187d456a OCPBUGSM-35526: Failed validation: Machine network CIDR : invalid CIDR address (#3316)
7420042e7f7fc4f30967d360022833a0e7398668 MGMT-8853: Prevents conflict errors with machine networks table in database. (#3311)
9dacb8ca330c15fa9d2b0e1854f0a1bca72e9ab8 NO-ISSUE: Don't wait for CI to update coverage (#3310)
f0f29579dec2a28cab08f3a7798d6cc62e947092 MGMT-9113: Remove V1 GetCredentials, DownloadClusterKubeconfig (#3294)
dc571101abedf000a991816ab6be6b519a68c68b NO-ISSUE: Bump github.com/go-openapi/errors from 0.20.1 to 0.20.2 (#3302)
528bd44f189a377716e335439fabd75dbdbf62a9 MGMT-9114: Remove V1 operationId GetClusterInstallConfig, UpdateCluster (#3293)
f594f61e862b3f585d373fa3b4b0fd890b15a268 NO-ISSUE: Bump github.com/rs/cors from 1.7.0 to 1.8.2 (#3210)
8876083b11729681eb2e501252c9d451c76d2241 MGMT-8046: BMAC should not create BMHs on the spoke cluster if it sees that platform==none (#3180)
ebad1df4b84a64a08abd1a8b2ff9e0b9cf854310 NO-ISSUE: Bump boto3 from 1.20.46 to 1.20.49 (#3301)
74565a0b8b610c03d9f84f59cbabefb7e8bc7e35 MGMT-8744: Change image URL auth type log from warning to info (#3298)
0bfb371b28fb8f3d507dfd01be15ee1f0d8b22da MGMT-9128: Remove V1 GetFreeAddresses (GET) (#3277)
16e82edc52531f5aa5e7be153560f82cdd0aed9a BUG-1969933: Improve image_status_updated event message (#3278)
358826696cf4bdec7d31a612419b7ee1d362f619 NO-ISSUE: Bump github.com/go-openapi/loads from 0.21.0 to 0.21.1 (#3286)
cc8f35389bbf5179b66ed560a21296bce14b4d27 NO-ISSUE: Update prometheus/client_golang package (#3296)
3424047967ab2cda9fdb6328a1f084706b8bef69 NO-ISSUE: fix ut inconsistency (#3295)
af0bafb3f7f629932f8c3dc31ccddedfe6984926 NO-ISSUE: Bump github.com/coreos/ignition/v2 from 2.9.0 to 2.13.0 (#3287)
6ac2816d2e61dbc6f82d6df569dee692ae06767d MGMT-9069: Report unit tests code coverage (#3289)
9e6e787bc08f9e87ce41ea75269832b4a7e8ea22 NO-ISSUE: Bump OCP versions release 4.7.41 -> 4.7.42 (#3288)
9bced3f531b645565685a75494574b5cdf03f251 NO-ISSUE: Bump github.com/go-openapi/swag from 0.19.15 to 0.21.1 (#3285)
0ba10f4b6ace23dda8c042ebc167a9de1237f5b1 NO-ISSUE: Bump go.elastic.co/apm/module/apmhttp from 1.11.0 to 1.15.0 (#3249)
af605b2633785473075384aa761f93d2e98ee337 MGMT-9009: enable overwrite for hostname in ignition (#3282)
70cd21e2b64f0e28993182c29cae733242e359a9 MGMT-9009: enable overwrite for hostname in ignition (#3282)
cb6fb6f3480b520c706247a908e4ebf8c9836f86 NO-ISSUE: Bump github.com/google/renameio from 0.1.0 to 1.0.1 (#3209)
fa67982baa3993e864befb5eed147abbae200184 NO-ISSUE: Bump github.com/iancoleman/strcase from 0.1.2 to 0.2.0 (#3207)
54cf05edf22f461f6727568c8fa0ed7bb2975e57 MGMT-9077: refresh cluster after host unbound (#3281)
dcb1833f177b90ab41184d226ee3c073b485853b NO-ISSUE: Bump OCP versions release 4.10.0-fc.4 -> 4.10.0-rc.0, rhcos 4.10.0-fc.4 -> 4.10.0-rc.0 (#3280)
3d72ef8f7f8715cb7a7d7918e3b30cf8f257605f MGMT-8254: support day2 cpu arm arc (#3263)
4ec8aab09c12fae8f790876794c3eb7e3daeac58 MGMT-8823: Document REST-API V2 Day2 flows (#3262)
436a34cd9941ace3c6345a202bc76b7bbd274477 NO-ISSUE: Bump OCP versions release 4.8.28 -> 4.8.29 (#3275)
cc393b669778da38536f4cf51f3cba30f8173fd1 MGMT-7709: optional openshift_version in infraenv (#3276)
14b08ebe92a539ec08008115031624c88b2a1e1f NO-ISSUE: Bump OCP versions release 4.10.0-fc.3 -> 4.10.0-fc.4, release 4.9.17 -> 4.9.18, rhcos 4.10.0-fc.3 -> 4.10.0-fc.4 (#3272)
1d327257c3cc54485c3cd09b517dc56907873967 NO-ISSUE: Bump boto3 from 1.20.37 to 1.20.46 (#3265)
d6b24491d1eb3c47a55583cbbc91f1f2ef158e33 MGMT-9096: Add temporary solution to install baremetal arm on 4.10 (#3248)
f27fec32d016b4d9a77b86b5720cee7364dafe93 NO-ISSUE: Bump requests from 2.22.0 to 2.27.1 (#3177)
d2aecddfc0ae3132e56c7b6a307a47e7acc3cd6b MGMT-8943: Update documentation to V2 REST-API (#3253)
cdae36020d0b0d1e4f370cc44e533ce76c76aaec MGMT-8580: Add documentation to boot discovery image through iPXE (#3252)
94252a53b2ea269a951ff216be5d106e03abcbc5 MGMT-9094: Wrong default timestamp for install_started_at and install_completed_at (#3261)
99e4e06de8c7349d604172d7b9fbe9ac9f6b44d2 MGMT-8582: rbac permission for leases (#3260)
3198e3fde7bada1cd3dbf3511d13648b27415c0a MGMT-9070: ZTP versions are not compared correctly for sorting and filtering (#3251)
e290552f9b15aa953a7d23402202df0645aa503e MGMT-9053: Replace register_host_to_infra_env_failed with host_registration_failed (#3245)
5809ed01ec3779639989ec544e224b7f3aac5305 Bug 2034686: Expose a way for users to disable TLS verification in image service through the agent service config. (#3237)
09c188d065770766bff65b6436b8e90d0f87145b NO-ISSUE: Bump OCP versions release 4.10.0-fc.2 -> 4.10.0-fc.3, release 4.8.27 -> 4.8.28, rhcos 4.10.0-fc.2 -> 4.10.0-fc.3 (#3257)
3af7708f2644053e72a3c1a2c88bdc4dd8d4a864 NO-ISSUE: use OpenshiftVersion as key in openshift-versions API (#3254)
4b4f0f45d897430037039a9282225bf6bd02acfe MGMT-8844: Assisted-installer update SNO minimum RAM requirement to 16 GB (#3220)
40563cca4acc91e8400a62a96874b2408ef2a320 MGMT-9068: Allow /31 machine cidr in SNO (#3250)
ec8343b64d104854269754207258a9ebde6dab06 MGMT-8783: support multiple patch versions of os/release images (#3219)
36774ad9829f4bcc62effbf73981dc07e9261ae8 MGMT-7896: Add host's log's URL to Agent CR's status. (#3222)
bb585d6d7b40199427c29ae55f438f6624ed55eb NO-ISSUE: Bump github.com/onsi/gomega from 1.16.0 to 1.18.0 (#3231)
224c267c321d6fb1120941bbce443bdbb94961b3 MGMT-8744: Add log indicating that with auth none image url will not change (#3246)
a1c6df56391b517f4bbf167ba841ffe040950ebd NO-ISSUE: corrects image reference in pod definition (#3236)
ede52ddf6bc3ed4fc394294067faae6b14fab382 Revert "MGMT-8582: Leader elector to use configmapsleases (#3182)" (#3244)
5e03b29d72a246747ae5a44b55786430fa3cd243 MGMT-8582: Leader elector to use configmapsleases (#3182)
40b5ae791c3a5656e7cf47166f5c455b073266b9 NO-ISSUE: extends doc with podman pod config detail (#3233)
1ca00064d9b64ebb8806d31aa9bea9c22fd683d9 MGMT-9027: fix flaky subsystem test (#3238)
48ae00b5e1c58d5f5b3df43a98047af34d584352 MGMT-9035: Fix validation of CA bundle (#3234)
06441f0b663807dcc52438217a39ff5355476e35 NO-ISSUE: Bump OCP versions release 4.10.0-fc.0 -> 4.10.0-fc.2, release 4.7.40 -> 4.7.41, release 4.8.26 -> 4.8.27, release 4.9.15 -> 4.9.17, rhcos 4.10.0-0.nightly-2021-11-29-191648 -> 4.10.0-fc.2 (#3235)
8e01d8a9d79db14e1e26d723c3b4af217a6d3e73 MGMT-8738: Set Disconnected status for media disconnection during discovery. (#3225)
c94fd8327e67f1f7a3c9f299a876a0e729ba42d9 NO-ISSUE: Use agent's status role instead of spec (#3187)
6d32bfd440bc4dac2c65615721b3097952e59171 NO-ISSUE: clarifies prerequisites in README (#3232)
39a76838d91324220beda160d66b9878d8885c71 Merge pull request #3184 from mhrivnak/podman-pod
4fd1bc4e82fd37a2608a80c5b4ab4179fbac7a1f MGMT-8894: Catch FCs and nightlies when comparing OCP versions (#3226)
a9869850e72b002f4e9f89374da2bfd2e60dc43a MGMT-8716: uses Pod definition with podman
e656c13c6fc4d6bce5fe1b790d2ac2318e2b815f NO-ISSUE: update approvers and reviewers lists (#3221)
bc5eaa51357955fb2be9cad573be533777836c6d MGMT-8894: Simplify IPv6 Network Manager configuration (#3199)
b10718782935feacbc1b1dcdaa927089b8f089ff MGMT-8664: Fix ACI template breaking dual-stack configuration (#3217)
591395103fc1b2d509750b275e641baa00a99ed9 MGMT-8958: Proxy support in ACI (#3215)
202ce128d8a31fed5cf1bcfeeb2b3f14176ddab2 NO-ISSUE: Bump OCP versions release 4.9.13 -> 4.9.15 (#3212)
80170758e2463f3b0f7e1c0256f1ebf7be57d0ab NO-ISSUE: remove unused etcd pkg from go.mod (#3213)
40f4f8bfcd46cee44aebd277215baf8b62eb04a2 MGMT-8428: cpu architecture support in kube-api (#3170)
cabac577fbb8b6fa062cf9a4f440789966097403 Bug 2034582: Fix 'supported-platforms' endpoint (#3089)
650712aae8f387b97d69fae3afd208910aad7119 NO-ISSUE: Bump boto3 from 1.20.31 to 1.20.37 (#3206)
9bae4c3662e4755e80251284aba529318d76c8e9 NO-ISSUE: update static networking guide to v2 (#3205)
aa0761475953a625249d560f0b2110b980501bab NO-ISSUE: Bump boto3 from 1.20.26 to 1.20.31 (#3175)
f140a9ed60f1507e2cdeb71092e486918d50b6a6 NO-ISSUE: Add syntax highlighting to restful API guide (#3204)
db25501e204af3231c643131daf7a16d94ce7a76 MGMT-8893: set arm64 support as dev-preview (#3195)
bd5cb842fa5704093802f1cb2528895598b598fc NO-ISSUE: add vlan and bond nmstate examples (#3201)
760f9fa0d6b1c2f69e73f1e336ae0d9958ebdfd5 MGMT-8085: Change the cluster ssh_public_key field to text type (#3200)
dcfd0f0e48906580b05e9108c43b202f9f2b87f0 NO-ISSUE: Use the correct iso download url for 4.10 rhcos (#3203)
838183f4b392f2a6d27e54496489580ec7f99efd NO-ISSUE: Fix assisted_service_build image can't find minikube (#3188)
3ae28e4923b4acb3e830b3a8ce9a0214539942eb NO-ISSUE: Fix broken URLs in REST V1 to V2 doc (#3198)
94ce200b59e8bb3fa0032819a727aa85b532dc22 NO-ISSUE: Add support for OCP 4.10.0-fc.0 version (#3196)
563365cfc36d306650d5a4b1dd209be1f9bdebed NO-ISSUE: Add a middleware to optionally disable v1 API (#3166)
768ad93c9ec77973c137c8ba53b765e627463eb3 NO-ISSUE: Minor clean up to the PULL_REQUEST template (#3197)
a4467b48bf5c5edb82dcdb369cdb241dc0f6b41c NO-ISSUE: Bump github.com/go-openapi/loads from 0.20.2 to 0.21.0 (#3192)
644d6dc6035d830acbf020247e57e53e015b451a NO-ISSUE: Bump gopkg.in/square/go-jose.v2 from 2.3.1 to 2.6.0 (#3193)
a15ccf04daa671dcd818670422df92f8bdc705a2 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.20.3 to 0.21.1 (#3191)
09b4e90174765aac11cbabbbb018eb40a32b6af4 NO-ISSUE: Bump go.elastic.co/apm/module/apmlogrus from 1.11.0 to 1.15.0 (#3190)
16016ca51b4921f021a99c3c7003723386135a9a NO-ISSUE: Bump OCP versions release 4.7.39 -> 4.7.40, release 4.8.24 -> 4.8.26, release 4.9.11 -> 4.9.13 (#3185)
cf9fec69f9d8ad5d78965898f34c7ce278066407 NO-ISSUE: Bump github.com/google/go-cmp from 0.5.5 to 0.5.6 (#3189)
e59d68768b96b012690690041b7fb5fd49c25952 MGMT-8887: Upgrade OCM SDK (#3186)
c7ef67fe0e83d1fe27f9bfcca79aab7e8b316d13 MGMT-8871: updates Ingress usage to v1 (#3181)
5a3fba78d6e90760c3b33cb835c58fa3d41e25e0 Bug 2038903: Add proxy env vars to image service (#3178)
b2e35e7b72527cc23c8df5192a57e2adb0bcf924 MGMT-8664: Add none ztp platform installation flow with load-balancer for libvirt (#3084)
85c33c7b34f926f0548c5b7054753d5944f180d9 MGMT-5425: Removed logs when a cluster or infraenv doesn't exist. (#3183)
11413502e6ae30d4b146473bd6a44220398a7f33 MGMT-8851: Remove 99_ prefix from manifests (#3174)
01a262daf1a7066c1cce133979ab3e34065cdc8c MGMT-8510: Duplicate hosts status messages on events (#3168)
4a24d792ac8f9f73d2c3d94adb9118084771ee3a NO-ISSUE: Bump pyyaml from 5.4.1 to 6.0 (#3120)
a6038490573f831cfc4c03e207f2040ca70565af NO-ISSUE: remove redundant files for bumping OCP versions (#3172)
52ed1f7ff3047e631b46ebb43650194e80906a7b MGMT-8197: Deploy HPP when CNV is requested on SNO (so persistent VMs are possible) (#3131)
5a661f1fedd3e3e36aaee7d988d86dcbd73a5ece MGMT-7305: Fix ACI column (#3165)
e781cea7e66fb4a75537961d5569a917491be8fd MGMT-8765: Add integration tests to the MGMT-8280 code (#3143)
d30e3559593f17183d11c2730f1f5f7fc8a8cfff MGMT-8841: Container image availability check is not running in some cases (#3167)
8ce627129f7c2f5d3b25ce68f242b1dc08825836 MGMT-8755: remove mco image , must-gather and openshift version from (#3164)
8cecf2ff22ef3bad635e33cd8216c813dea3380d NO-ISSUE: replace docker usage with binary installation for conf generation (#3162)
dac91d8e96f40a2331570dde9f328167c3c8c7cb MGMT-8748: detect overlapping networks in SNO (#3152)
6278140aa99dca8d11f723b8d20694bdc9329e94 MGMT-8756: Make ImageSetRef optional in ACI for day2 (#3160)
cc29a54a2f633609e78992caa474affd365149b4 MGMT-7305: Add columns to infraenv and ACI CRD (#3142)
0b415976d5cd2120e4db2acf6cd1facd1dd084aa MGMT-8624: Enable downloading kubeconfig when it's available (#3134)
4fef8fdb08a9b6e97b2de592b9798e1216569338 MGMT-8755: Make openshift_version optional for day2 cluster in REST API (#3150)
d7580b33923b77f158e96eece5d65590ce16680e MGMT-7307: Tweak media disconnected message (#3158)
df41c55a30212aa74c64d15b3712a3c49b1c41ce NO-ISSUE: fix swagger UI link (#3156)
6ed9f692f7cbc873f7a66ee5b7ed4f08f156e606 NO-ISSUE: Change default release image to 4.9 (#3153)
ca9a803e06173cbfc6ec543ce31fa17a96ed35c0 MGMT-8498: fixing issue with not mounting pki due to old (#3151)
6d7285ad160cc6f3e9e462aeae49de4f9e3e50e1 MGMT-8607: Store event names in the DB (#3127)
b20a6faa5d1ec15ae9fa3752c970795eb82265ba MGMT-8741: Use full name when logging agent update (#3141)
64ef5f05576024baf270ac64047b9b0419da4f48 Bug 1994696: Clarify not eligible disk error message (#3130)
0b54b84ada3fc7bf05fa9d20701770d44d811c1e NO-ISSUE: Check events in kubeapi subsystem (#3138)
6759704d82f26b7d1ddba488ae29eb461c7ea40b NO-ISSUE: downgrade 4.7 version to test auto bump new mechanism (#3140)
ad8bb4c214bd74501cb76ad1caf8cb7f9a1babf0 MGMT-8513: V2 link in cluster's Href field (#3137)
df3de4ba4f8530d0ccfb6a8e1f437d4710b9c4bf MGMT-8703: Document adding additional trust bundle (#3129)
0a450c158036d75fbb4ac756c49887e9a5c74bf3 NO-ISSUE: Bump boto3 from 1.20.24 to 1.20.26 (#3119)
d01375012573ecd59776093bc025f40b94ec43d8 NO-ISSUE: Bump wheel from 0.37.0 to 0.37.1 (#3117)
52cedbde0b370d05d189ee35cb8989baa97180ef MGMT-8301: Add a V1 API deprecation warning in swagger (#3135)
c9e731244667da2c6dc4f2a6b5d5343d586f00c0 MGMT-8698: update status_info and progress bar when extra workers fails to install (#3133)
800f512bd143e0e428d34709d674970e82107ca7 MGMT-8722: Populate EventsURL in InfraEnv (#3122)
2fe4cee4049873bcf133ddd5e3c5a894c54b6892 NO-ISSUE: minor cleanup to the events generator (#3128)
40eabae5dfa3ca6b74b15c7c28a7a40f91090ade MGMT-7307: Improve the disconnected media message to explain what is expected from the user (#3124)
0e84bb731c9213ffcd071fcf7d26c04a301fe19c NO-ISSUE: fix 'yaml' has no attribute 'FullLoader' (#3121)
dec820d7265bd0cb99f0396cf6bda6cec14b7327 MGMT-8606: Add api-review label to Events API changes (#3125)
56f2e67a1b9a572dd2b4275387e75de80a3847a4 MGMT-8713: fix ovrit and vshere platform check (#3116)
2107513cd872f9e8e628ede9987ba1d7a04890ff MGMT-8096: Remove all VSphere platform properties (#3115)
6e940f003ced82b6fd3b6cddf338fb5cf7eb435d MGMT-8727: KubeAPI Controllers to use V2 Events endpoint (#3111)
0f95966867cfa6b1cf293aa7b1a5f8746e0a3282 MGMT-8364: use LabelSelectorAsSelector for nmstate (#3112)
b9f69f414fc9c565dc5cff0474f09da3e2732ada NO-ISSUE: Update to dev docs regarding feature-usage (#3114)
c8476c7dc6e242dbeaf9989f532538a7928d251d MGMT-8603: Add doc to install operator via OLM (#3113)
ec0d573b62a8f94fd26dbdb92321f7c1876ca660 MGMT-8724: use upstream postgres image for podman (#3110)
f00a9a0da255361695489199579a71c9fe349712 NO-ISSUE: upgrade moby to v20.10.12 (#3109)
15de04f35d77e10e1bf861c6dd0ebc54d1995ede NO-ISSUE: update golang-jwt package to v4.2.0 (#3108)
d42b27b5f28d3aa9288a527cdd867587111c3b84 Bug 2029876: auto-assign node fails SpecSync (#3069)
2521f15ca8e38c8ba65776d3e160d6850554bcfc MGMT-8498: Adding mounting /etc/pki to next_step,installer and logs (#3065)
9337a7662e01eff4af7d2aeb36517e3f7a0c0f05 MGMT-8721: Allow host updates when unbound or binding (#3104)
264a8dcfef5aafb58104fcebd362a2be64c81c22 MGMT-8663: Support none platform in kube-api for day1 (#3083)
d8c1bacc4d169e3e1ee957d8872948af94d5c095 MGMT-7385: feature usage doc (#3102)
52fe780cb49242dc1bddc2fcba490a9047ee17fa MGMT-8228: Fixed the error message when a host fails to reboot. (#3092)
27006a1db1fce79d0c1677e6b5c379b86c611d5e MGMT-8710: Assisted-service fail to get the agent ignition token (#3099)
a9110d598b75de655ca150e23b3c7e59a67adc20 MGMT-8709: Allow to override IMAGE_SERVICE and ASSISTED_UI images (#3100)
f2bf95ee08aa6b82fb1d940d6a0b1f09d14ab55f MGMT-8671: Fix V2ListHosts response when InfraEnv does not exist (#3098)
edf2f1d890cd6c8ac2caee3f88042a54446b0d4b NO-ISSUE - Add pyyaml to python requirements (#3097)
2117ce46e68089a6a31bb569a7ab8fd2eedb1bee MGMT-8095: Change 'ignition_config_image_generated' event type to infra-env (#3076)
76c1586d1a351af02e56205aece963298207ef76 MGMT-8677: use "edge-infrastructure" organization for all images (#3090)
c0808cde64b7afd07358f8fb9e7a11a28681ca20 MGMT-8477: invoke cluster validations when updating a host (#3082)
1f02b5ec6a19ded1c7a804ebd040b020f7da4b0a NO-ISSUE: Added doc on how to boot discovery image on AWS EC2 (#3094)
2315c61908dadd346775e710fa5afe5037be64c5 MGMT-8516: Allow filtering infra-env list by cluster id (#3095)
b53e85e1039d230961678416ab7a621bc277c8ea MGMT-8669: Allow /30 machine cidr in SNO case (#3087)
4d12b3a7381d783266ced616019e6e686b7c65ae OCPBUGSM-31072: progress bar alignment for day2 (#3081)
fb0cdf002d15ad88178426539146237b6bd9828e NO-ISSUE: Added example for tang_server JSON-formatted string to swagger. (#3091)
a38b90debfcd4ffdea45452b7c389d87ee902295 MGMT-7428: disk encryption validation for day2 (#3074)
59c4ae8da5924a2995a6d9b2dcbfb96e3a3a5d0e MGMT-8456: Add REST-API V2 documentation (#3070)
b8f972455c0ab7bbb874dbd24d8f47d38579fdf4 MGMT-8280: changing ignition fields in aci and agent from value to secret reference (#2972)
2c5c368632e2b5ba76ea0233433fd8404765b7ec MGMT-7330: remove unit-test logic from Jenkins (#3086)
6ff77427b52defd89dcb4af18c5ac479dc7983cc NO-ISSUE: Bump boto3 from 1.20.15 to 1.20.24 (#3078)
f4237fbc381eb2fb11c51cf98bcd5d1844b0d5a0 NO-ISSUE: Bump twine from 3.7.0 to 3.7.1 (#3048)
263cbed3c4f3fa7c462681308b076b8b4e38afb3 NO-ISSUE: changing sno dnsmasq name from 99.. to 50.. (#3085)
589d1530344dff8b803e1c8a79ecab4bf0170fb9 MGMT-8623: capi-provider-agent fail to add host to hypershift due to API VIP connectivity failure (#3080)
aa87618bd812c18d3dcc93f3aca8692d4f3bc26d MGMT-7428: added ignition to apivip check response in swagger (#3073)
b927d5c07d9b72fa986ade1befbc068342a3028b MGMT-8423: Rename api-vip-connected validation (#3075)
902d4753c6072bbd8016d1dec11625aa9a851e99 NO-ISSUE: Bump OCP versions release 4.7.39 -> 4.7.40, release 4.8.23 -> 4.8.24 (#3068)
8427f3c18cc4b2b34b4bd9ae342c4329f7b8c60f MGMT-7507: Add feature flag for dual-stack (#3057)
fd02c4be0afd1e72776e57578dcfa9433a1bf42d MGMT-8564: Rename the UI deployment template (#3056)
e925720cc7784aeeb2f85866cfbbdd5f44dd1168 MGMT-8178: Add InfraEnv GC to OpenShift template (#3058)
2cd050ec92f06a5b759be105330c8aad4b9433a4 NO-ISSUE: Allow short or fqdn for image in manifest (#3053)
374a46718aee28f974ce963e44d2e13f03e4d7a0 MGMT-7330: Make `ROOT_DIR`, `COVER_PROFILE` and `GINKGO_REPORTFILE` overridable for running unit tests in CI (#3038)
8a856a064f0306059d09930494b51258240f36a7 NO-ISSUE: Bump OCP versions release 4.9.10 -> 4.9.11 (#3052)
855d0c228be0e2cda5c93ea9a421bf36826e9e17 MGMT-8504: Fix InfraEnv image updated event loop (#3049)
e42bd72dbebbe637ce029875f51bdefcfafef96d MGMT-8300: Improve behaviour of dual-stack via REST API (#3042)
364b9d71b11250ae536787ef354c2d7cb516bb7c MGMT-8505: Fix logger for NotifyKubeApiInfraEnvEvent (#3045)
11486d01ab53dac3abbd1c7f24cf4954d2722c01 MGMT-8315: used values cached in cluster for AddReleaseImage (#3018)
2e5fc6d0c81a6a3db8a05d6cc45be37aff112cf6 MGMT-8472: Fix flacky test infraenv GC (#3044)
0082e14f443517b7d4a5c0e50630c497df623653 NO-ISSUE: Use .Equal to compare time objects (#3041)
3dd3df0acd914504743bc02d6d04bf3245fb59e7 MGMT-8413: Add new condition on AgentServiceConfig Agent object to signal the health status of the underlying operands (deployments) the infrastructure operator operates on. (#3031)
db8abd392bb181068cca37400070971b45bcb853 NO-ISSUE: Bump OCP versions release 4.7.38 -> 4.7.39 (#3037)
2b2cb010cff83cb555e03e12ea07330ad5938877 NO-ISSUE: Bump twine from 3.6.0 to 3.7.0 (#3021)
959ed85f7b5fb768df7f2aa1c5343084485382cb MGMT-8482: Add channel for ocs operator (#3036)
0e79e608f2b11a01ac40cc21bca72fddc5de8653 Mgmt-8424: Day 2 ignition endpoint check customization (#3027)
8996b3e2f89ab1434a0a968cec326d65da0be18d MGMT-8313: Update event on Add Host to Installed Cluster (#3017)
e525f26213d9c3ddade2c1d1385d65ca4c544672 MGMT-8415: Remove the infra-env image download endpoint (#3016)
30eab9b2f9915e88e567703b33bbea953cda0b6d NO-ISSUE: Bump OCP versions release 4.8.22 -> 4.8.23, release 4.9.9 -> 4.9.10 (#3030)
9928f9056c91bd5fee8f68d8da7a4b6322b54c42 MGMT-8448: Use the image service when deploying with podman (#3023)
c5992d54d734acf971d478831aa22eeb053af1a4 MGMT-8308: Fix vsphere provider db fields. (#2989)
72f1bf912689b50905915c372a9d750be42360e8 NO-ISSUE: Add api-review label to k8s API changes (#3032)
2fe4f0fc08876d8141e6d1118a55c0b46def74e9 MGMT-7330: Copy files for CI to run the unit tests (#3008)
bbff2371e9da8529281673340eccd2398f23d182 MGMT-7254: Deploy and use image service for subsystem (#2884)
1612598643d6472c55474fcd03651ff1d9e2fa64 MGMT-8461: Avoid panic in case nil is passed to GenerateError (#3028)
8e5c03ffbd0fdbbd310c5707c6e903b3aad21238 NO-ISSUE: Allow setting MINIKUBE_HOME (#3026)
90a9b30339ee2d001329640d7e5947e0846ebdec MGMT-8451: Setting VIPs support levels to dev-preview on all versions (#3024)
fb2c51618d44bf6ed3855b1ad53c1ddbbcf1dc7c MGMT-8178: InfraEnv garbage collector (#2994)
ea66ea918a923d6f23bdddcc8daa1da0fa0471c8 NO-ISSUE: Fix upload to pypi as it failed while uploading the tar.gz artifact (#3019)
818fb52b4cceca3d36e805c63c5fa476181f2a07 MGMT-8370: Replace the client on the service with the new generated one (#3006)
137a8603a46dfaf764f2703adbef10c042d41ae0 MGMT-7925: Remove a redundant cluster registration event (#3009)
5e759094ebf7e6a4f95f30c9404b964754079cad MGMT-7901: Kube-API import cluster doc (#3013)
b11287f4806461e4258add7fc71d1ddb38c0cdfe MGMT-8299: Subsystem refactor: Implement a global AfterEach func (#3014)
57178ae8a1cba1fdd779cf86c3097ded891ddbd0 NO-ISSUE: update assisted-ui repo location (#3000)
96c88b228cfb642385a391513e2f8db69a26d565 MGMT-8355: Fix flaky subsystem test - host next step (#3011)
0d3dbb71dcd8043e41972e0ddcf0d7fc7d36133c NO-ISSUE: Bump OCP versions release 4.7.37 -> 4.7.38 (#3010)
03371a059d91942126f8e56c3bb20e2612341596 NO-ISSUE: allow setting HTTP routes with DISABLE_TLS parameter (#3012)
e663286f78b811d5db22d05bd213559fdaa542da MGMT-8180: day2 - fallback to default ocp version (#3002)
1d44e57368014d8bf00741760afcf859332e7af9 OCPRHV-635: add tests for ovirt provider (#2911)
1439a827f959233a8d303016238bec127ac59b6a MGMT-8203: DHCP server failed to allocated VIPs when VIPs are manually cleared (#3007)
b9ab5d3c77580ab93c29bb43cb78cc6b02d54e88 MGMT-7943: changing message for image availability validation failure (#3003)
74fac6fd951194e6b954789f77904171d840dde7 MGMT-8302: Ignition endpoint token should not be returned (#2998)
ec5584d951c10cd273f31887a92be0b3a149a625 OCPBUGSM-36598: reset progress on re-discovery (#3005)
cfc506caf82065c0cf8a7ef4aad4806417c2a085 NO-ISSUE: Bump OCP versions release 4.8.21 -> 4.8.22, release 4.9.8 -> 4.9.9 (#3004)
fa4b690782dd01cd8910a29d5e19c4c1f2a84a08 NO-ISSUE: upgrade git on build image (#3001)
08c3627b1551dd5a8cf63629990bcac0fa2fb48e MGMT-8334: skip unbound agent recncile if bmh host is not detached (#2984)
14ada2f9c7388ad31bf339e77b8ab1c48aab7cc4 MGMT-8372: Removing data from "Custom manifests" usage (#2997)
e577680a7f6b87338e06bf0b9ac00d664c9ead0a MGMT-7330: Create a job in prow CI to run assisted-service unit tests (#2916)
bd9e790cfbd8a53e7e799c8277e51e74a30aa19f NO-ISSUE: Bump boto3 from 1.20.10 to 1.20.15 (#2995)
21a0b6d0ce008343ca5eaf1cbe467b1cd98940a0 MGMT-8337: Remove unsused hostname from Agent CRD (#2988)
4c3f37a643153a29becb97312f7775a6fb7fca18 MGMT-8351: Hosts table primary key has to be migrated from (cluster_id, id) to (infra_env_id, id) (#2992)
778362afc3b57dcb89575931311e2e77b1581eb0 NO-ISSUE: Fix typo in error message (#2991)
314a8b88529b56364a3d91120750930c055f6bd1 MGMT-8178: Add InfraEnv package (#2981)
a3b408e7daa880778f6ecd1e7202df8f1ba8af10 MGMT-8333: Cluster failed to update console operator status (#2982)
4d4f9a6a64c9592c0c8cb214ab5855d1fbd69b4c MGMT-8346: fix iso url when using image service (#2987)
81908c7aac5cf4c41cf124f3b3f71da32b77f36a MGMT-7929: Host status update events to include optional cluster ID (#2980)
21dcc3424acd5a4bd351cbf439e0330f77ba6764 MGMT-4502: Put unit-test pgsql data on tmpfs again - the path changed (#2986)
1b137112f1a4b5b7944748c6a9353e41573f2c7c MGMT-7716: Add IMAGE_SERVICE_BASE_URL to template (#2983)
806932db60d8f4ccc3c466d3fc2cf1f137eb9e52 NO-ISSUE: Bump OCP versions release 4.8.20 -> 4.8.21 (#2979)
d82437f6773b6b967ab3edeb294563f0c4fffcd0 MGMT-8088: validate hostname before transition to known-unbound (#2946)
684c9c6311cf9ae9bdcbea2cc3a6798680d05e96 NO-ISSUE: AgentController move log to debug (#2978)
128a0fbc34429da7ff5aeb8806656c5860606e72 MGMT-7817: Rename env var for operator upgrade (#2976)
222cf111b23f74f21243f25cd09d280580757065 NO-ISSUE: Bump twine from 3.4.2 to 3.6.0 (#2930)
7a231c4354a24c65d35a20e1743007fa3ca65743 NO-ISSUE: Bump OCP versions release 4.9.7 -> 4.9.8 (#2973)
386f864a87417eed80c91e3a41133a432006e096 MGMT-8222: Fix flaky subsystem test register_same_host_id (#2948)
0ca0a5ae7db26a5ccd7f141a8830ddb33d260fdb MGMT-8279: kube-api - ensure release images exists upon install (#2970)
c40d0c169da4c565d50281ef56e88f4c7c83436c MGMT-8307: fix flaky reset log test (#2971)
2b8721f61710d9a3ef2872f418b5a19fd45c0c61 MGMT-8281: subsystem print resources when subsystem tests fail (#2958)
56268a27f154f6c3068a5f1223d7b1cf4598443b MGMT-8296: Ignition token is not updated in UpdateHost API (#2967)
244ae5b5c86ecb9c509a8a7da20b28146468cdd1 MGMT-8305: Ignition token passes extra colon (#2969)
908ddcb55f0803c5e3d826cb9091534ab84ba0aa MGMT-8298: MCP can’t be set until the host is day2 (#2966)
116f3b15f90e520d67c00ec904bbca570665e04a NO-ISSUE: propagate GITHUB_CREDS to OCP bump script (#2968)
0ec868488942628cdb866e70b4b2cd7ac1311dda NO-ISSUE: only inspect netrc file if this file exists (#2965)
0d08087cda37aebd7034ed24fde4b9f05ec734ba NO-ISSUE: skip tickets creation when bumping OCP versions (#2956)
325aa5ed78578776256aaad6ff511e382ca1f1c9 NO-ISSUE: clear host's log timestamp before installation starts (#2435)
b74db8f3d364b01a04baeed4f3d8cc222c22b51e NO-ISSUE: make openshift-edge-bot author for OCP version bump (#2964)
8f48227b669895ffd2f33b5dd3c97ec5b6c319b7 NO-ISSUE: Bump OCP versions release 4.7.36 -> 4.7.37, release 4.8.19 -> 4.8.20, release 4.9.6 -> 4.9.7 (#2955)
104df463920b09bab909d99de805249060af4f8f MGMT-8278: Allow updating agent properties before binding (#2951)
08bf4307df7fbe598769acd4835097a2d4f28dcb MGMT-8295: reconcile fail in case agent spec.IgnitionEndpointToken isn't empty due to null pointer dereference (#2962)
afc00380866f9be26c252b189c527c76e9889887 NO-ISSUE: Bump setuptools from 58.3.0 to 59.2.0 (#2959)
2c0b10ee076f3087d442d4af74ed3e63790ce110 NO-ISSUE: Bump boto3 from 1.19.3 to 1.20.10 (#2960)
8a08c76ba792ac9a732f21090478ab95def02425 NO-ISSUE: Bump mkdocs from 1.2.2 to 1.2.3 (#2790)
7961cb3700a35b688d8a5ab3a3cd77f4ed2cdbef MGMT-7401: Add cluster progress to ACI (#2940)
dd6eb94f5e87e6dff909b89030a9d32c3b9d7a40 MGMT-2086: upgrade to GORM v2 (#2908)
fac2d434a754811797e8916fa4cd967c4e7ed641 MGMT-8243: remove log msg about user issues with tokens (#2950)
09d8c4904900ad26485487224cbee8b42a58e9bb NO-ISSUE: there is no need to base encode an already base64 encoded ca.cert (#2949)
fcd1962e39d9c87595fc2d1460f151832da820cb MGMT-8225: Bump OCP versions release 4.8.18 -> 4.8.19 (#2922)
5b76f6eb37f14e252ce16f7a80b6064c58e0b97d MGMT-8276: Add Day2 state in Agent conditions (#2947)
aed9cd986e48489a3aff0b5a13586fe1d953bad5 MGMT-8127: Webhook block unbind if Agent is installing (#2942)
b51d4bee708a0d2a72a84dc529d83b0cde2fbac0 MGMT-6893: Fix ignition endpoint URL validation (#2909)
b2f12a4812b183ab3c072c85b3c0ea101d23c46f NO-ISSUE: remove default_ocp_versions.json (#2941)
140fe0cc2726d73077e6737a8a65f178d2ea6875 MGMT-7231: ODF docs (#2945)
26714eaebe4a723e9dae22e1928b5b9ef59b5696 MGMT-8205: Add endpoint to regenerate infraEnv download URL (#2919)
66174d092f8e1e04c303084bb0390165ecfc23a7 MGMT-8067: Adds disk encryption feature flag (#2915)
2bab992917261c93b78fe3d633b52ceae9a1f98b OCPBUGSM-36861: progress bar goes to 10% after pending user action on reboot (#2938)
7513e6e85fdaaf344445ced0e49447d3807901a0 MGMT-8237: incorrect api responses for cluster managed networking with vms (#2936)
3c6c20c6f897a2a0378a6ff41c141028c52b8a9b NO-ISSUE: set PlatformType on ImportCluster (#2933)
4d9a92a5afe5f79505024dbbc5a81cf2b0631db3 MGMT-8079: reboot BMH on unbind-pending-user-action (#2912)
a65d79dde664c16794a925c1ad36db0e203d31bc NO-ISSUE: align spelling of infra-env in swagger descriptions (#2924)
07253f323a55c137b16d56859116d22a805118bf MGMT-8101: Add subsystem for return host to InfraEnv (#2923)
1b0a65263d27d00903f71ec8de65448380f739cc NO-ISSUE: remove openshift_versions support (#2875)
62b1de9d84e0b3058f0036e0059f8516454d8955 MGMT-8229: All host registration events to include optional cluster_id (#2925)
bfe669325f8e644cce661e7d70ef15e79bdde297 Bug 2014262: No cache no client cause hub gotta speak to spoke when retrying (#2920)
a82cfd056626f9c7322e881b8d675a79480c739a MGMT-7693: More V2 subsystem tests (#2886)
177046427e7cef7b856ac233a64ddc2012884722 MGMT-8200: Fix controller crash when import installed cluster  (#2921)
03e48d22c2d297fded8d9bc6656747a50c4937e5 NO-ISSUE: replace occurrences of cloud.redhat.com with console.redhat.com (#2917)
4883d1f5e08df14554aa05fe5ca6b5c0a2a07851 MGMT-8206: Bump OCP versions release 4.9.5 -> 4.9.6 (#2910)
e76f930a20227e0ebc63308f866decf3da1e74e4 MGMT-8207: Worker logs does not collected while cluster in status error (#2914)
67e1d0cf8378498753fbfc05c73d914ba3a936d3 MGMT-8198: Rename host_cluster_registered to host_registration_succeeded (#2913)
f2f7a27ea69ac7bb6fce77cff87359dffe1f33bc MGMT-8196: Use postgresql-12-centos7:latest image (#2904)
6a0dcf6dae2e2ffc0a936fd6b8becd674a0fac71 MGMT-7897: Add Image-Token authentication (#2824)
c48bcdf24e33c114545089df0ae90fa27b926e24 MGMT-8099: Late binding doc update (#2905)
a18c6150f0d88ffec5e8c9ae5d830c1660a1568b NO-ISSUE: Update webhook doc (#2906)
8aee9aca678416b729ba136b708ac9abe346cb43 MGMT-8192: Logs_cmd command fails if insecure flag is set to true (#2902)
ca65aa3a0e71526bc94731de6a26e79c694a725b MGMT-8129: Upgrade go-swagger to v0.28.0 (#2872)
cc827d7553ff12a85662e6973e28ebce9e3be082 MGMT-8188: Update properties order of host events (#2900)
c3bea6489271e79955f3411afeb56028ef4c81f9 Bug 2021215: Skipping disk-encryption validation on day2 hosts. (#2901)
68127da721ba95f87d5eb44d750e186c9a163f3b MGMT-7423: KubeAPI support for disk encryption (#2890)
9495cf9737253d6db2d8846197de2e5c841f362a MGMT-8144: Bump OCP versions release 4.8.17 -> 4.8.18, release 4.9.4 -> 4.9.5 (#2874)
6ea85fed882d82d2d18f66043679503f6d62425c NO-ISSUE: Graduate hive CRDS to apiextensions.k8s.io/v1 (#2856)
84c9c1f11f51132ad8ef34bf75fed04e2875ed12 MGMT-7834: create webhook for infraenv to make sure clusterRef does not change (#2851)
1ecc16b2160b843cde1650161954eb4d95f40b6f MGMT-8165: Enhance message when hosts' clocks are not in sync and have more than 4 min gap (#2888)
8098abf4cd63feae5e88f237f7ae255ec76ae53d MGMT-8131: k8s user can specify CA cert for ignition endpoint (#2883)
5ec1587a4cdd30fa97dc082f6a845ce67647ee2d MGMT-8130: Unbind hosts on cluster delete (#2871)
c5480d217030409a4293ad7a81e9860058963d62 Bug 2019415: Cluster installation stages missing from cluster event logs (#2868)
7ec84480c31c16cc0e34a379dc8c5a08a6311b09 MGMT-8169: Ntp server set is failing on upstream due to chronyc client version in container (#2893)
0dcedb3867bfab73226ff833c36c31e67bbe4eb3 OCPBUGSM-36598: clean progress on reset (#2854)
c7a98ee79bf967ef9bd3b5a202da9450e52de86d MGMT-8166: updateClusterData should handle updates for Tang servers (#2891)
a3923b08fe52a0fad469db5d3d3cc6eaa7cc33e2 OCPRHV-589: Initial oVirt provider support (#2745)
88348c8d319ff1cb2173f21d9843bb91aff06e45 Bug 2020928: Changing the condition that check if disk-encryption is enabled. (#2887)
5e05b2e4dabb782ac4dea25433af5d34af968657 MGMT-8078: Agent conditions for unbinding-pending-user-action (#2859)
e6f9e3060662221607d64c2b8e63336cfb50e957 Bug 2011745: Document ignition versions (#2879)
acb52f84154c4f45a057f7c5cf6aca8581c95c15 MGMT-8129: Remove required attribute from current_stage in both (#2880)
9a1af8bb6883d9869883415e39fe4c5490b7bf5b MGMT-8126: Exposing feature_id in swagger (#2876)
52e1207ffbad78ffdac1f10290fd93598a38dd15 MGMT-6893: Support custom Ignition Endpoint URL and Ignition token (#2849)
e125b59fd271dbeace653e02631a03d8d57ba98f MGMT-8074: Make the assisted-service more dry run friendly (#2822)
90235ad12442f8ff60a1fd677283179ce3a2e54e MGMT-8149: Add OPENSHIFT_VERSIONS template parameter back (#2877)
012938680cdb94b43d65ac06b8286ef879e46868 MGMT-8090: Add state unbinding-requires-user-action (#2844)
56130849043f9e3218669133236ab457ac40c525 MGMT-8062: Update doc for agents-back-to-infraenv (#2869)
a10efdb7f493ffa00620183472ecacf9abb2bf93 NO-ISSUE: Expand operator CSV description (#2873)
93587459537a2b8ae93a4b2c6a26a8e7f402b88d MGMT-8070: Adds V2 API: V2GetPresignedForClusterCredentials (#2821)
2e6d080de5ec4ee8df2c68359c9707c8e147a554 MGMT-8128: Fix wait_for_assisted_service failing on multiple tests (#2867)
f5eb147497227cdf89204f57189e0d47246be361 NO-ISSUE: fix usage report on SDN/OVN (#2870)
79b52d6579bb4a9144e3f9673cbbcb4efcd63e74 MGMT-8098: Bump OCP versions release 4.7.34 -> 4.7.36, release 4.8.15 -> 4.8.17, release 4.9.0 -> 4.9.4 (#2843)
843ab6e6a35cfffc8bb4d430a393df149658b553 NO-ISSUE: remove '/test all' that just breaks all jobs (#2857)
793f318b97412e2e6b18a1e43723d16f28dfd2c9 NO-ISSUE: Add event name documentation (#2863) (#2864)
328d67ad14dcf1d9adc8f1d0e5d40519fd02d99c NO-ISSUE: Add event name documentation (#2863)
15b6f0360d96f8f05caf0ae86124dc986dac5ed1 NO-ISSUE: Add more AI links to CSV (#2866)
8619f7c412b5fd3bf0f5d82742dffb6eb9f61652 MGMT-8108: Clear Progress in Agent status (#2855)
130c2bf20e4a2e0c8ec41d550b8ab4a8ab814f47 Bug 2016178: Add ClusterOSImage to Baremetal platform (#2862)
6be4db4fd7200ea7ee1976307eeafd8c95532698 MGMT-7915: create V2 API for Importing (Creating) Day2 Cluster (#2813)
e00b346c1e89dd444c4a317666c69855678b2954 MGMT-8113: Update the postgresql image in the operator CSV to the new org in Quay.io (#2858)
0060ea38e4006ba09a503c7f9d3602d4516d65c0 NO-ISSUE: Renamed events to a uniform format (#2820)
4d7bb12f20f9728cdb3e44c1626466e49910cbe8 MGMT-8120: Change Events subsystem tests assertion (#2860)
3afd149a1e014a9c8ad12e17bd552a46d9a49f76 Bug 2005259: Progress bar out of order in SNO (#2848)
5d1e72b903c82d4471e6f620306cbbbc281165a2 Bug 2017866: Populate requested_hostname in V2ListHosts (#2846)
cf17896cee7c04bb64a59c5634d22da120390ad8 Bug 2014081: Add user filter for /v2/events (#2798)
c775a6486a9d44e6cc1b7c73ab17186efb27006b BUG-2016158: fix links in hive-integration README.md (#2842)
f3fe241b7abb5efa16fb5aecd9969999a6c35ea0 NO-ISSUE: bump OCP versions based on fast-channels instead of stable-channels (#2841)
bff1eb2c76d65071b000bc11f01eb8787d7b03dc MGMT-7789: remove deprecated default_ocp_versions.json (#2783)
690e415d461f2fb8c4908450a07c944cb578bf9b MGMT-8062: Enhancement doc for return Agents to InfraEnv (#2825)
4a6cc531a15f6575ac6097d49d5621afeff6e7e9 MGMT-7439: Improve validations debuggability (#2328)
38a9d0398b96e81ef494029277e362a7256df44e MGMT-8094: validate OVN with VIP allocation (#2839)
4f4791a8a27a96e50892d9cd83d424d604ce621b Revert "MGMT-7330: Create a job in prow CI to run assisted-service unit tests (#2830)" (#2838)
b227df11416eb2729a65a2eddda89602d235e9bb MGMT-7330: Create a job in prow CI to run assisted-service unit tests (#2830)
e3f3e867f7dc757492110c770951aa77cb6c086e NO-ISSUE: Minor bump to olm-catalog (#2836)
1fd98239182aa20dd8511c24967075d497b6a23b MGMT-8093: Bump OCP versions release 4.7.33 -> 4.7.34, release 4.8.14 -> 4.8.15 (#2834)
bba8ede61f10cc26cdd7d1ae632651a5caa0d502 NO-ISSUE: Improve asc field descriptions (#2835)
cb8576bd58d8e7fa8b45107352e74c0da88aca1b Bug 2014074: Add hostname to host event message (#2819)
c6f4efcfc965a9301942aeee2459d7e09706ac6b MGMT-8092: Change ARM feature support level (#2833)
81155724b20ede16be5073788d8a90ecec8daee3 MGMT-8027: Replace generic events (#2799)
f3f9836fc4cd54e1ade73da5f5747a5c79f5adc8 NO-ISSUE: Update asc description (#2827)
6359985a800e528f06ddba2a0048b1703148a6c2 Bug 2017444: Create BMH before the Machine (#2826)
190af85f3154250009c953992aa8f492a56cd5f4 Bug 2013671: v2uploadLogs to use V2 Events API (#2767)
38ffae0ebfe4a27227f483fe2500fa6dfc4e0bb0 NO-ISSUE: Update operator description (#2823)
f5b56b1923b534c16a13c17ef29bde902466e4cc NO-ISSUE: Bump operator channels on master (#2817)
36b5951109e426301eb2797ab0b68950df4ad4d6 NO-ISSUE: Bump boto3 from 1.18.63 to 1.19.3 (#2818)
b72f99ab6d86fc8ae9cfeefae8bbf062911764fa NO-ISSUE: Bump setuptools from 58.1.0 to 58.3.0 (#2815)
d76d75279fb4cc587701852bed8aea52cb433c0c MGMT-7897: Add sub claim to image service cloud auth enhancement (#2805)
9bdce9e8b651abed1875ea198cd6b4ab062fba4e OCPBUGSM-36145: host count validation message (#2814)
aa26479f2cf184a0a2d6d6ed4d439e2595e17780 MGMT-7932: added PodDisruptionBudget to template.yaml (#2754)
e4dbabefa15f1646401575d7585170ac234f5ee2 NO-ISSUE: hold OCP bump PRs by default (#2810)
ecfe5282f3f031546bfe5746bb3a1b5ef95d85e2 MGMT-8056: Bump OCP versions release 4.8.13 -> 4.8.14, release 4.7.32 -> 4.7.33 (#2809)
d4e9a87d4d43f2398b1c2e318e6b8151af79c14d MGMT-8508: Update Operator CSV to use images in new quay org (#2811)
c9b4a787e8c9cb5ede72be9b5b5c4a68235c2244 MGMT-7148: Add webhooks validation for ACI (#2224)
8183d673054b6cf188c906aca1301aca028e2e2c NO-ISSUE: use appropriate image in operator upgrade (#2808)
489c729935f3e8a49e2bc7825148e4af05d9b203 MGMT-7876: auto-assign select weakest masters first (#2795)
3b9af4fb82721fa63043ee806e2a06e4784d5856 NO-ISSUE: Bump boto3 from 1.18.44 to 1.18.63 (#2789)
df1f2e38e095c9efe828732a6e9f6d356ca308bc NO-ISSUE: use aarch64 path in default_os_images (#2804)
e5fb301bdcb671f053eaf8325b0f96903c81a3fb Bug 2012067: add <TRUNCATED> to truncated error messages (#2797)
f0853cba9b89df3461056ffc52176d20f864780a Revert "Use 4.8 redhat-operators catalog on OCP 4.9 (#2688)" (#2802)
18d167a2ecdd039de649350e18d078eaa4453185 MGMT-8029: Gorm creates wrong field name for https_proxy field in infra-env (#2793)
246752a248ade24385ff9a32ff2091d52834b01b MGMT-7148: Docker file update for webhooks (#2801)
1cf74edb2726a2affb206e23b5b5b2246a3b601e Revert "MGMT-7716: Add a template file for the image service (#2762)" (#2800)
713c8942d420305bca08147fabfa4afe6479376d MGMT-8021: Move authz out of the authentication handler (#2780)
2b354214d78d722a8a78cc06fcc1907e75aa4ede MGMT-7923: Image service cloud authentication enhancement (#2733)
0d4e88137447e9ddf4dcbab5caa005e25c27da44 MGMT-8024: Bump OCP versions rhcos 4.9.0-rc.7 -> 4.9.0 (#2792)
2d302407f3bc484b9c9df976fd154c1709e7dfa7 Bug 2013640: Generate bminventory package events (#2717)
464f6ac78fe7641da40df85d267e7550ce8759c9 OCPBUGSM-35151: validate HA properties on register cluster (#2765)
38f02fb2357feccb0abca67dbf93c30967f1d6ed NO-ISSUE: update default versions - support new stable (#2791)
a24170a8f09a8f4be62060689f3303fe40407ee2 Bug 1991953: Adding timeout on finalizing stage (#2785)
8545671c7edb8ad9476719792b090a9689e79c7b MGMT-7998: Fix nil pointer dereference in subsystem metrics tests (#2784)
b02abb30d18d2de501527d93a71d70e6ebcf3897 Bug 2013419: fix status_info in case of day2 host (#2782)
7a3c1197bd9a38cbb79cafda5adeb15235c4e16e MGMT-7973: Bump OCP versions rhcos 4.7.13 -> 4.7.33, release 4.8.12 -> 4.8.13, rhcos 4.9.0-rc.4 -> 4.9.0-rc.7, rhcos 4.8.2 -> 4.8.14, release 4.9.0-rc.4 -> 4.9.0-rc.8, release 4.7.31 -> 4.7.32 (#2781)
cc39df66bb6431e7843d3be828fdc9e4a731939c NO-ISSUE: Use ansible_collections instead of ansible.plugins (#2777)
09449e394e647efcd86be6dc02dd60595e5cd40b Bug 2013791: Delete host from DB if Agent creation fails (#2771)
4ef488475f3675e717c0bfb366470eabb9e59a26 Bug 2014140: Adds host_installation_started event (#2774)
8fc5c739fcff5a3fa7ab2518fd1b13b2cc7428cd MGMT-7817: Rename and set env var for operator upgrade (#2729)
ec34821a23582da82242297923f647fdb6658b01 Bug 2012811: Unbind host from bound InfraEnv conflict (#2766)
e4ecba5f6601990d7ee58cc2bedb8939d36c010a MGMT-7408: Expose support warnings from backend (#2728)
ace332361745cc50d1c7ffa09eefb00153e13847 OCPBUGSM-34971: make retry-able container image availability (#2752)
18095889fd1de8516ac6f511095e90e77847afe6 MGMT-7716: Add a template file for the image service (#2762)
0ba6d8eea8bf5f7c50fbc929536b455b57be6176 Bug 2012796: Add LivenessProbe to Image Service (#2751)
5933d3ec7a43bef8012135a44172c982cfd583b7 Merge pull request #2764 from slaviered/auto-assign-feature-flag
934ddc8caafd769bfb94e027bb1403d5549999a7 MGMT-7181: CNV operator cpu architecture validation (#2760)
447ffcd02943354d0bf73d3b84eec800558675c2 MGMT-7956: ENABLE_AUTO_ASSIGN env variable
be61459525f905dd60131d25511b21908fd2c780 OCPBUGSM-35106: pre-network-manager-config failed due to timeout when static config is used (#2763)
8083e57a0642fe0aec81342547db9a30114a2583 OCPBUGSM-35978: Add cluster_id and infra_env_id to logs in more flows (#2744)
443f84321bde9cbd7933fa6da265ec079a04c7bf MGMT-7874: Use suggested role in Status (#2646)
285c3de61264d9531becc98c8324a8873930dffd MGMT-7710: Adding TPM requirements for preflight requirements API. (#2755)
eb6166ff50b3966387938706a6069ff688968a9d Bug 2005651: Add maintenance to release-image support levels (#2749)
52fe342ef02e84f69c952b123181557d2ae09e96 Bug 2012901: Allow Agent/AssistedController to authenticate for V2DownloadClusterCredentials (#2750)
adf8c73bde2c01d51a7623b936fdbedea8ddd1eb OCPBUGSM-35987: Adding default value for disk_encryption in cluster registration. (#2743)
19dafda106a632994ba09689b6d7af59b9f32917 MGMT-7801: update docs on os_images and release_images (#2735)
1094250f72756f6e3ff3aae8fa4e4bf1b88337aa Bug 2012534: Late binding doc example (#2753)
80d21a05921180b02b92b7804f68b9fe5320dfc8 NO-ISSUE: Remove user yuvigold (#2748)
94853fdf095031fb2bd791f78e0ee3c4ef78c22e MGMT-7779: Delete Agents when InfraEnv is deleted (#2726)
41c28d579e489e31a3494e189a4c3c4e49849639 Bug 2005651 - register cluster should return BadRequest in case the release version support level is maintenance (#2742)
fc5847eac0b599fd3a2a880bb3e3527aba2c90fb Bug 2005440: Use current and new cluster data for dual-stack check (#2731)
aafa5c8c407e43f27b7fd165cb046d51283b1f1d MGMT-7190: Added ValidationsInfo to kubeapi (#2692)
581ca9a9c07885b408ccfd4e632bc2a38f726c1c OCPBUGSM-36009: Fix role selection query (#2738)
beebeea1d06d887524973327583f6cd78404ed40 Merge pull request #2741 from danielerez/versions_tests_fix
84a9ab88a5778366344551c4e535e08c93cc8bc9 NO-ISSUE: fix versions tests
50d8b017d89f156595c35e5086af2182b5f94066 Bug 2010384: Adds /v2/events (#2608)
8d28eedb9bf305fadcf515d925efa1c9a3f27f53 MGMT-7180: Add support_level to release-image (#2734)
6579cf41317b5aab050c87a69cd33e83bf60f484 MGMT-7705: Use os_images in deploy/operator scripts (#2708)
170c324f876ec498641d65940c1ad5848a81d79d Bug 2012534: Update bind agent cmd in late binding doc (#2737)
cfe2dd1bb43c535abcda7907c7fe68f6b096006b MGMT-7899: mark required fields in InfraEnv (#2719)
050a186ffa8a196df7c91fc8a116bc657d4f147f MGMT-4475: validations to consider effective role (#2587)
38b6857f11c7d5afba6ad5dbcdfc63c6e3ce3008 Bug 2011976: operator should handle rm nodeSelector (#2730)
697ba620ddcb396d99c99c391e481c1188c3aa48 OCPRHV-631: Enhancement, "Define Providers Interface" (#2272)
03a7180e1f5af90a100fc8ae5aea8b995081dbc1 NO-ISSUE: update arm 4.9 rc.4 release image (#2723)
22868a6af177aec0d40fef1ab966cf2d8a918015 NO-ISSUE: Fix catalogsource when upgrading operator (#2724)
38d5ad33be4ab091664a8638073a2f7a7c5ea61a NO-ISSUE: Changed 'Platform' to 'platform' and 'Proxy' to 'proxy' in the install-config.yaml (#2721)
10dcf01527da7cf81911741c3db6001caf21e0df NO-ISSUE: fix reviewers and watchers for OCP version bump (#2712)
5ff11a4225d7758fbcaa077028563429280a9541 OCPBUGSM-35727: Fix calling 'supported-platforms' just after the cluster creation causes a panic (#2706)
0b5235fd9543e3e00f2e4b704244377f4a07e493 OCPBUGSM-35272: empty cpu architecture implies default (#2693)
aa208ef44c1b435aa4cb790bf43c34fd57f3a975 Merge pull request #2679 from eliorerz/bugfix/OCPBUGSM-33932-image_info_content_differs_in_response_to_GET_and_PATCH_in_/v1/clusters/UUID
60368e521eea91de7541713cba9493dd512d0a95 Bug 2005656: UpdateInfraEnvInternal should not log InfraEnvUpdateParams.PullSecret (#2718)
aaf082709521945b0c2fa2600113caa553071398 OCPBUGSM-33932: Fix image_info content differs in response to GET and PATCH in /v1/clusters/UUID
f23aeffb12d2f2ea3de0754e0b133b12a0172e01 Bug 2010319: Use V2 in log URL in ACI (#2700)
f7da12dc682adaa6ae8a46cf71e074d1a1f5139c NO-ISSUE: Use correct catalog source name (#2711)
098c55396a0197a18793c8d319e31a980e7c04c6 Bug 2010479: Reduce open db connection limit to under the max (#2705)
1afa49524f1bb5b369829f9fd1affd62868f1727 Bug 2009255: Add infra-env-id to the send logs command (#2709)
6d349494f9b7a39897156bafd19b8838b3398314 Bug 2007781: Multiple concurrent request for initrd download crashes the service (#2677)
7102f39b1edacbdf2e7faee1bb22f900634d60d2 MGMT-7708: Generate openshift_versions API from RELEASE_IMAGES (#2674)
faf9e0916b8a486250378da4b872f4487519564d NO-ISSUE: Fix typo and incorrect if condition added while improving operator upgrade job (#2703)
e757792da509d137a5d47d4f86d1bc1ae6a68f34 Bug 2007106: Extend dual-stack network subnet validations (#2660)
042afb35e346cb0c35ac942fd79871bbd2a98f5a Bug 2009412: when unbound host is bounded to day2 cluster, it stays in insufficient state (#2694)
cc66413c6368c9759148f38e3df75cbdc2251054 Bug 2010168: Fix nil pointer conditions search (#2698)
e93b52cdcd08b2eac2dd37f1fb504c9109af21a4 NO-ISSUE: Fix tests url on dev testing documentation (#2697)
badfb5d77b0642688c06743cb5e304e6a29c62be MGMT-7708: set default release image (#2690)
198ac9ceaf60b2cd4ebc12ed2f54f0b110cb280b NO-ISSUE: fix ci-approvers list (#2696)
3ba1cccfbb13815b884d5840c26d5b0dfc07dec7 ASIC-58: Add --no-cache flag and remove old Dockerfile.test (#2695)
f2d1db6f3a410a995def24d45842e00110c5311d Revert "MGMT-2391: Deprecate host stage_started_at and stage_updated_at fields (#2681)" (#2691)
b26b8d43dd6678ca4ac4333ffd389a680d7ab740 NO-ISSUE: Use 4.8 redhat-operators catalog on OCP 4.9 (#2688)
ebeabdc696809f37ef89f2b3a23070145d52989a MGMT-7890: Bump OCP versions rhcos 4.9.0-rc.0 -> 4.9.0-rc.4, release 4.8.10 -> 4.8.12, release 4.7.28 -> 4.7.31, release 4.9.0-rc.0 -> 4.9.0-rc.4 (#2685)
b77227c5cee64fbe4d393b4dfcdddd4b732ab6dc MGMT-7817: Improvements for the operator upgrade CI job (#2661)
a4e1eb6e623032813da3a68a5e075117fc234c70 NO-ISSUE: Bump setuptools from 58.0.4 to 58.1.0 (#2664)
90aaec0a14535c30b0d574533d4a6565846cc1ff MGMT-2391: Deprecate host stage_started_at and stage_updated_at fields (#2681)
cacce54197fa8407197f5b05f14d0a3c5fab83d7 NO-ISSUE: changed creds used in ocp bump job (#2680)
b83e81a1cf68c0d281d70f588e35071945f92c95 Bug 2009204: Add error msg to InfraEnv condition (#2675)
30af7f2d5d86333f48b5766f96beb9ac33916088 Bug 2009349: Adds InfraEnv Register Deregister events (#2610)
0be2147c0e5128c664d0223469816047c2c94399 NO-ISSUE: use /cc command to set reviewers for ocp bump PRs (#2676)
1af6bd6250eba38699c2478056762352fae1bedf Add Providers Support - enhancement implementation (#2546)
a94e949059b85cc17241b773bf2ed914b0820145 MGMT-7871: added default arm64 OS/Release images (#2671)
0a010b16b32bb5e1f0c4152babda3c58588ab8dc MGMT-7599: Add documentation on the repository CI (#2584)
8369c23466c2c853b485e8bc9583155fcf9ada42 NO-ISSUE: fix OCP bump by updating assigned user (#2670)
73b88bcc23d5a34603bd585d832062e89bc74d78 NO-ISSUE - Increase operator deployment wait-for-service-pod-ready timeout (#2669)
824eef89ac58cf89a474d9272e9d54b4b353c911 MGMT-7867: Use default ImagePullPolicy behaviour from OCP (#2668)
d3264105f8a3d6f7edfb3fbab269624e53cb7f74 Bug 2007515: Fix regression introduced by copy-network bugfix (#2667)
8cf51023fecb0ef0d213b8d0d216176f903f0190 Bug 2007515: Pass copy-network when infraEnv.StaticNetworkConfig is set (#2662)
93806847727b74362d4e102a64e025a5f043c6a5 MGMT-4872: Generate event for operator status (#2638)
eeb24d2705ec694948ff8708eab024e7cf11c1cc MGMT-7282: Update operator using subscription channel (#2659)
9f25ce68c11919bb0a9ccdc7d825f09f6691d9c1 MGMT-4872: Generate event for disk quick format (#2639)
d868786dbe448613237e386840a957fd7a599c1e MGMT-7732: Late binding - support move agent (#2599)
ee20b7d438597371c510a768662a36906440dd6c MGMT-4872: Generate Image Expirer Event (#2637)
b537ae8363807330936db74eddeb447d2e0f1b76 Bug 2006549: Pass CA certificate to the UploadLogsCmd (#2656)
2c989772dba9ef9efc7aa1bbbf1d494f27575e68 MGMT-7282: Use community operators to install AI operator for ocm-2.3 (#2657)
de149acd018268795c22e7563643e2bc6f9ecd47 MGMT-7687: Propagate Infrastructure Operator node selection and tolerations to its workloads (#2640)
be02b47c11302ccc927f26f7130c196504abafc7 MGMT-7223: Changes for adding remote worker node jobs (#2649)
967ff04c03836a50afe36ffac7035ff7cc140181 MGMT-7315: Allow providing machine networks for multi-node non-DHCP (#2635)
0eed5f33402d9e6ec98d2f8db3986853a1934cff MGMT-7258: Use image service in assisted service (#2628)
7dcb60579fdf27b5d1a34f3ffe89eb50675da0b8 MGMT-7852: Implement V2 InfraEnv Host download Ignition API (#2653)
f4303654b85b75ad9c8658ae27cae9e2b50d9313 NO-ISSUE: Bump boto3 from 1.18.41 to 1.18.44 (#2652)
69fdf61b2d24523cb1bf9c28fd76f6c24292d0d8 MGMT-7847: Remove SUPPORT_L2 env var (#2650)
51c724621cc833b1dd9c5987c86cd2d3f08d679b MGMT-7421: Adding feature usage for disk-encryption. (#2641)
413b69ca0b66f4cc57f22a5362377bb4d373bf74 MGMT-7282: Operator upgrade readme (#2632)
09bd0816a90196e5c203b32c4ecbd23c0bb8852a NO-ISSUE: Print resources for easy debugging of operator installation (#2636)
5b1886c1f78a08b79d770755e63baa6699b4b170 OCPBUGSM-35242: Set x86_64 as the default architecture for OsImages and ReleaseImages (#2634)
48161f4ddd572aa29a37c9c6eb1f8169d0787193 NO-ISSUE: Fix olm skip range (#2651)
4b3e6c606f7754f9ba12500bdaedc4f14ab72a73 MGMT-7698: KubeAPI subsystem - restor upload logs tests (#2648)
d3bea25d540ef4406a002727260aebf8d95f918b NO-ISSUE: Fixing default values for disk-encryption on cluster creation. (#2643)
fd66b0719a6daad36c2f8d4e93c5dbbff2e05752 Monitor logs (#2647)
d78e59b86e754c1e5114a3403ae3e0fbf5bab040 MGMT-7840: Document events usage (#2645)
48a7ecedcb85f731c25e2f23b692c18fef93a9a6 Pushing all V2 APIs commits in one setting, in order to avoid multiple rebases (#2642)
aa4db9435bc5b734abe64cd7cdbd487479746895 MGMT-7780: Late Binding Kube API documentation (#2644)
77b37428298e7ccc7806277e8b876326dbe3a1fe MGMT-7806: Change host events API in order to solve segmentation fault (#2620)
10cfb3452bf91916f0b416fe43ad1572ced52145 NO-ISSUE: fixing the name and the message of the status info for UnboundKnown state (#2622)
cb15c3ab5c9d4ab289acc49ba4d699e15693cf32 MGMT-7790: Set SUPPORT_L2 to False from the oeprator (#2585)
e98d697d36e44baba984889f40f408c5f4fb4382 MGMT-6763: Add support for dual-stack CI jobs (#2631)
d8888171f88fd2ab69920e2088f742fd35fa92ee MGMT-7613: Move get cluster logs V1 API to V2 (#2603)
9ca0d69ee4d97e502e51e8f572f7edd973f4d084 MGMT-7666: Move list monitored operators V1 API to V2 (#2535)
34c986435c1e85776b2bcb0544eab2e6e77a2c2b OCPBUGSM-35037: Fix osImages refenrece passing (#2626)
f7c3e44a7774262b592673edb098c2c862dead5b MGMT-7282: Rename env var and move upgrade scripts into its own repo (#2627)
d6d04d46541dea66362cf91424c52351d7f95665 MGMT-7282: Operator upgrade (#2577)
81f0d7aae706b9584b36c5bee1c8cbd4bab60f23 OCPBUGSM-34323: Use the hostname in the Spec if present (#2586)
56e04f4305f0514451a4b3ca9b47e70636344dbe Revert MGMT 7639 podman transition (#2621)
eac427b0b815af5e87bfbbfa144d128ed897f63d MGMT-7772: move specific V1 APIs to V2 (#2607)
b4ef293775125c7f52715b5d5ecacce6ec1c547c MGMT-7608: Move cluster default-config to V2 API (#2509)
5c005bce5b74d4ca9000329bc466a4360e8980aa MGMT-7728: Add NTP configuration to ISO (#2595)
d32509441d865592c48c8073e218de03e3fd81d5 NO-ISSUE: Bump boto3 from 1.18.31 to 1.18.41 (#2617)
e8d1dbdcdc9b3c83a07ad1213a6e95004b1be4b0 OCPBUGSM-34901: Add register successfully event (#2616)
8ea305cc6eec1341f9da2aad13d1a676e4ad9835 MGMT-7796: reset host data, set by the cluster on unbind operation (#2597)
7400d650be9138b57a15f9db6319c6e6e12e5a7a NO-ISSUE: Update operator-index-build to use podman
34ee58a1333634a0f1036eb0d0a432b601598fb8 NO-ISSUE: Bump beautifulsoup4 from 4.9.3 to 4.10.0 (#2613)
aaab065d4d8cae001644b80ce9c32c630173f268 NO-ISSUE: Bump setuptools from 57.4.0 to 58.0.4 (#2614)
a96c596238d8177bdaa33541ff16d352f91b7be3 NO-ISSUE: added OS_IMAGES/RELEASE_IMAGES to template (#2611)
73e4b5247468179cd6f6844750648ac63ca1b837 MGMT-7798: KubeAPI: Adds InfraEnv debugInfo.eventsURL (#2606)
d4382db81e24c89fe8b56c3d17a14f30d0a90cc7 NO-ISSUE: install epel for centos8 stream (#2604)
01127b60fd52ef985cef5bde78bdba80a0799350 MGMT-7785: support AddReleaseImage in Versions (#2598)
006d1162ddd1ba40fff3819d7f5086ec57bb186c MGMT-7799: Adds infra_env_id to event properties (#2609)
0d559c3a98321e0d83a74fe20124e7f73147ca86 MGMT-7576: Implement V2 DownloadClusterFile presigned (#2429)
98eb2f2800d1812cf93241ee42010eeeaa75126e MGMT-7667: Move list managed domains V1 API to V2 (#2537)
286b9294e4d8fe3e8a8cc3d2ac46b2831528d98e MGMT-4872: Generate host package events (#2529)
5600072078a351bc9bf595bb4aa10cea780d39f6 NO-ISSUE: Fixed a flaky subystem-test related to disk-encryption. (#2594)
300f0564c33cc485dbddf830dcfa027b8a41e69e Bug 2002495: Deploying OCP on RHOS with assisted-installer Failing validation blocks deployment (#2592)
7fb78b2048199211c6f2f475b68b1f42a6d16e9f MGMT-7774: convert V1 APIs to V2 APIs (#2589)
f98a97f809d61a59ec38fb3e24048744ec727e3b NO-ISSUE: adding podman to the skipper builder image unless the opm index command failed
8665edbe178483df6cc940b91d26d64e89379a5d MGMT-7726: Handle non existing cluster in Agent controller (#2569)
124ebc9bb477da66b34014c07d4a8772ee6ee870 MGMT-7639: Support using podman in the deploy-test make target (#2451) (#2591)
c3745ae0b4dba505dd9513acb3bce22499e4c8b9 NO-ISSUE: Skip cluster progress update on day2 clusters. (#2590)
c21027e12b4f69b19d13d84917bd08d91b3c296b MGMT-7777: Bump OCP versions rchos 4.9.0-fc.0 -> 4.9.0-rc.0, 4.8.9 -> 4.8.10, 4.9.0-fc.0 -> 4.9.0-rc.0 (#2581)
b87833716a4b05c0ff5b228e2aeb8164dc2e125f Revert "MGMT-7639: Support using podman in the deploy-test make target (#2451)"
bf551bc0c13e6b71dde96bfc8368488c74c08892 MGMT-4321: Extend network validators for dual-stack support (#2452)
c7ebec57586ce689db1a90cfc2c74ef96fce6094 MGMT-7639: Support using podman in the deploy-test make target (#2451)
3b1d4bd293e88a27c008a715d68a58202d0ff82a Bug 2001029: presigned files access (#2583)
c4d12fd81f3366cf286d735d1446c23c7c119ac1 MGMT-7775: IsDNSWildcardNotConfigured should not be part of unbound host validations (#2582)
88829d7bf7573fbb2289cace1a576cf47fc2d709 MGMT-7611: Implement V2 Cancel Cluster Installation API (#2533)
9afe29ed4edf54c6faac9adde284154e8bea5f06 MGMT-4475: add operators host criteria to canBeMaster (#2575)
80bc8bfef640f741d73b8fa430a1d5db6b4466ab MGMT-7643: support pre-releases in update_versions (#2559)
97c9aaa73e3cf4413ba566b1ede88ff13611dd76 MGMT-7633: Update CD controller to use V2 API (#2567)
97824b774469328cf7b305b61c46ce8f59396580 MGMT-7395: Improve error message for DNS validations (#2496)
0cede0e423ffbc3bfedaa11aef43e18c3e6b0d01 MGMT-7730: Add Bound condition to Agent CRD (#2565)
dced33947c05954180a31ad47f0330737f3d12e1 MGMT-7768: Handle Host's Kind field during bind/unbind/register (#2578)
2085cd7c4c573941b28691ad4bcd70701088674c Release 0.1.0 (#2574)
48f58845a3b0e7381efe1d56988639af9dfb27ff Bug 2001973: Add more validations for Disk Encryption settings (#2573)
86adabf1034b2dc81ceeaf3dbede18ce33e20b9c MGMT-7754: Support iso creation with EFI boot only (#2563)
1503d374d6196d0049cd6905b9b9e59c05af9d6c MGMT-4475: calc suggested role in monitor (#2541)
2e5368d7f3bf698126e25a913c68f6b6e7a04a32 MGMT-7601: V2 cluster update API (#2464)
c30a99612382d8c7125151b42a929ab1b971e73c MGMT-7253: Add assisted-image-service to AgentServiceconfig (#2480)
8e1218d2bb1145feb9cc5e06fd06d3fbfd3bab12 MGMT-7090: Bind and Unbind Agent (#2477)
ae1fe9b323a2ba70e32cde08bde87aa93d707897 Bug 1979950: Fix minimal requirements for cnv (#2550)
f41d4779ea8c70b3c809441551d373244a0395a4 MGMT-7593: Added custom manifest feature usage (#2504)
418eebe6c858fc5f6184b7631bc4dd65d5beaa18 MGMT-7643: update ocp to 4.9 in operator/common (#2566)
3f3e964827a3201a4ca60014b068f745a25b71f8 MGMT-7752: Bump OCP versions 4.8.5 -> 4.8.9, 4.7.24 -> 4.7.28 (#2558)
b574045556063943442e9c8a380117c123a08c64 NO-ISSUE: Change wording for the preMigration section in docs (#2554)
c461c0e492bdbb335ec11c20ceafbe0974e3dd14 NO-ISSUE: Bump boto3 from 1.18.21 to 1.18.31 (#2514)
7b91e4c29bc40f5b27ccfa0d72e3d67236b58599 MGMT-7751: fix unbound host not reaching discovering-unbound state (#2568)
2b2a0f9a99ef2f0bd87bd3463d564c8baea32113 MGMT-7686: Support unbound status in conditions (#2522)
7e2bdee7eac37b6afc5cf402f65f9c8b9051c655 MGMT-7742: Fixing host getting stuck in "binding" state (#2561)
56f78c351bf7e4d92a4806ec40e0e1a4407445c8 MGMT-7725: BMAC add test for agent without cluster (#2531)
ab08d4b01d211feea1eab31816c9b02ebda1c555 NO-ISSUE: report OVN and SDN nw types separately (#2557)
63b910220beb5dcc9626078fc085f2e788a99a35 MGMT-7457: Adding validations for disk-encryption. (#2482)
bb4e8cf7fa547570ca84792d4eae72fa6a9f3f46 MGMT-7753: KubeAPI Docs - Update Diagram (#2560)
e100b7e6dbadb96b3fd71da210d5aec4d117e53f MGMT-7472: Fix log to print infraenv ID (#2548)
c5856d40f5b1e9bdaee817631d127eb50d464a17 MGMT-7610: Implement install cluster V2 API (#2530)
f6a69317500350c0c90abc722c5410e1795ca940 MGMT-7736: Do not blindly load the whole database in InfraEnv migration (#2536)
1ccfaac7774b43658c308618bdb152399456b2e8 MGMT-7498: Add missing backwards compatibility for network configuration (#2485)
3ed387eda54e012ac597bf48df8c9286b35d13fc MGMT-7749: Bump OCP versions 4.8.4 -> 4.8.5, 4.7.23 -> 4.7.24 (#2552)
a3ca9f18329c2a848cbea5be822d41b42bde8985 MGMT-7568: ocp_version_update - clone repo before updates (#2542)
e3c3d28e81587e5930d20396ecd6210903042bfd MGMT-4505 Fixes RWN creation when no hostname annotation is passed (#2549)
e1f6833d7b9a009ddf60ac8dabcc758f0934135f NO-ISSUE: Fix typo in log (#2547)
01236fe7da1dea93b53f4858b0b6db2640fb2f87 MGMT-7724: Remove notification CD to InfraEnv (#2532)
474b3a4480626e7e4c88dd6434bf48899761b5e6 OCPBUGSM-34158: Transition day2 hosts to Done (#2476)
801802e8833013278c20934d5f816416cc9d4660 MGMT-7643: Add support for OCP 4.9.0-fc.0 version (#2540)
76f1a17949d2e22cc9f9022029371808b689f261 NO-ISSUE: Move events.yaml to docs (#2534)
576f2c127c095d3095a1c8bbf8494c7b72125b56 MGMT-7704: Fix disk validation for infra-env host (#2517)
86e5c2977613d915134edcceeace9028288f3ab8 MGMT-4872: Update events requirements (#2497)
d271e2bd73701c2dde93ec1ec6d1e9152134cfee Bug 1999297: Trigger VIP reallocation only when the primary machine CIDR changes (#2527)
d15dc93a96b2d6c3c4906c4174cdb72c9e7a5ebc MGMT-7568: ocp_version_update - support os/release images (#2525)
7c519c97806ede146c73b9dd5a272fdfcfd1b747 NO-ISSUE: Update cloud.md how to get JWT_TOKEN without ocm client (#2528)
5517abcbfc7144a2296c6971cc59f856fd3541cd MGMT-7609: implement cluster get/update install config for V2 (#2519)
cd276798caa666141f484607a5df4c868fa73985 OCPBUGSM-34182: skip IsDNSWildcardNotConfigured validation in day2 (#2526)
2cc28dd1f21cd84e6afc95371fe71560b824aa57 MGMT-4475: add suggested-role (#2508)
7e1b1109b23e98c9d866d6b1a5528f00319d4105 MGMT-6670: Fix handling of empty network in various network params (#2512)
d3df122596992f30b945532cc98254b5ed779b72 NO-ISSUE: downloading kustomize release directly to handle rate-limiters (#2523)
6830bcb730b0a593501ef0e954b2a6eb09ab43ce MGMT-7714: Allow downloading kubeconfig-noingress while cluster is pending user action (#2521)
5273cfb4e4640cf084eca523d08533e76a36af83 NO-ISSUE: Create initial docs about network configuration (#2428)
3b7fb154c738c0ab57d004a69df931abf812e607 MGMT-7292: Revert Add custom_manifest.yaml to not break tests (#2520)
ad8e599e0c910c854fec82b480f497ab245bc763 MGMT-7606: implement Get/Deregister cluster for V2 API (#2500)
8dea319859354e10cbd313d367b6fd1695227e10 MGMT-7690: BMAC agent reference to CD is optional (#2510)
364ec237c5cc5e564e0e3272155de8d56b8e90bc NO-ISSUE: Update swagger-codgen-cli to it latest version (#2505)
bd2c1dce47c2187e9bceec4c8b9cc34234271948 NO-ISSUE: Fixing disk-encryption definition in swagger.yaml. (#2493)
f9d35ddde26443b283a43103c80862b1ce063226 MGMT-7479: support OS_IMAGES in AgentServiceConfig (#2503)
f9bab51220f7fe745a627a9900f2ac7f0f3e28e5 MGMT-6670: Fix BelongsToMachineCidr validator message (#2511)
51ee4ce418dd208fcc902a4e54064bc74dbbd57b MGMT-6898: Fix MachineNetworks validation for multi-network setup (#2507)
dfe652d0b729dd954cb802744393f8b539461597 MGMT-7592: implement Register/List  Cluster/s for V2 API (#2499)
4115a5eacb44a4f6160e2b780197517b5b10bd5f NO-ISSUE: Remove manual sleep in Makefile & Extend sleep interval when waiting to the service (#2498)
64d7ee9b50aecb9dd4fb010bee7e1344726a8c3e MGMT-7484: validate UserManagedNetworking for non-default arch cluster (#2502)
f129981dc2e7e414cec9d23e6e572ddf6b3e024a MGMT-7642: Use GetOpenshiftVersion in GetLatestVersion (#2501)
3fc865dd4739351424c08b19c9cfa61c34e5a26e MGMT-4872: Generate cluster update events (#2467)
b369673e5cb4ae9240cfec96337d102ee8bbec23 MGMT-7234: InfraEnv Controller migrate to v2 (#2379)
81d8a9ca6df026b065d8c5f9b3ec97e09ba91e76 MGMT-7695:  remove a ClusterID option from InfraEnvUpdateParams (#2495)
8eedf068bcc104c66a1334a94e54598aa507b9ee MGMT-7692: add subsystem test for infra env V2 scenarios (#2494)
2bede3fc24fee89f5b9b5830c0588ae7119c2ede MGMT-7187: support multiple architectures in uploadISOs (#2454)
f9b2f3d3246f91f7e80eab0b85eb9c34742eaa46 MGMT-7549: extract openshift-install for none platform (#2456)
4a3649715c6e71771a9d662d622732e6bcca120b NO-ISSUE: Deprecating /v1/clusters/{cluster_id}/host-requirements API. (#2478)
9d64b25d5fcd2c90c360cab28b15b32288124c7e MGMT-6670: Extend validator for L2 majority groups (#2414)
68e5678e73cdf08144b1bb6ef2ac661bd1c51774 MGMT-7688: Agent Controller V2 Ignition and Args (#2491)
d78b955a9e1e5b0104f1ad87ee73ce3c37dc03cf MGMT-7685: ISO should not be generated in case InfraEnvUpdate has not changed its params (#2487)
bc54dd0788fe73a51bcc2c95490e8bd1ddedbb75 NO-ISSUE: fix typo in the word requested (#2490)
253e388e2a31bd06e2160cfeaf5a97480a0a36f3 Bug 1992138: Handle possible NULLs in user data migration (#2488)
4cf673eabed9ef0ac7e47332ae259ef18bbcbe41 MGMT-7680: Use V2 Host Update in Agent Controller (#2481)
eb7c83ba5fe69b55cd5a9f432de8c7bbafdc0701 MGMT-7646: Validate ignition on InfraEnv Register (#2461)
304c71315ef1529d023ec47532c6896503ec9fc9 MGMT-7684: Assisted service crashes when there is an unbound host that has a failed validation that used to succeed (#2486)
0161f74b890e45c21421b4a06f698864fe23d667 MGMT-4872: Generate cluster registration\validation events (#2444)
f5a7dcc55610ebe9fb696339ff42d604d211d90a MGMT-7656: include host calculation in waiting loop for the service (#2484)
45dc5dd6046e9d7f4519a94ed1b8e0b7c13c0664 NO-ISSUE: Change users at the OCP version update (#2483)
dabadc7587577c9348a3bb8c143111f352b7011d NO-ISSUE: Remove push to app-interface when updating OCP version (#2479)
da115d03cbd81b752a3777f4bd5d34459beaf089 Bug 1992138: Check ownership of cluster and infraenv in rhsso auth (#2471)
13edb3cf14547a7beaf714ee8130ee2416e0afef MGMT-7676: Remove ENABLE_KUBE_API_DAY2 from agentserviceconfig_controller (#2473)
2200f5dc278b9257891aa5bd303f7d7706dc0353 MGMT-7602: implement V2 Update Host API (#2466)
dc302e2d14b2df545c264bdd6db8e48d560c0cac OCPBUGSM-31544: Make sure spoke BMH inventory is populated (#2410)
ddd633ccc73e1e016c1752985c9d50a618fff894 NO-ISSUE: Add more info to the 'Test' section in the README (#2114)
56247fd7d2d97d6a99eb540ca43404ee84512566 MGMT-4321: Bugfix flaky auto assign machine cidr deadlock
68e0dc8d4c7e3ff890303d7f30fbc4580f0c58c2 NO-ISSUE: Bump jira from 2.0.0 to 3.0.1 (#2457)
a2c9340f056d50675a7d28f57db3afee645ffbf5 MGMT-7661: Add property called physical_bytes_method to memory (#2470)
860bea3122a2256a3d7d393f1c68c6d4587aa64b MGMT-7650: Align GenerateIso error handling (#2465)
6dfb1b6baf3a4d222633443b3da4edf2c173c735 MGMT-7642: Select latest version in InfraEnv create (#2460)
446becc0f8501ee4e00d8be90a872ee219a40fb9 Bug 1996531: Reduce singleNodeRebootTimeout from 120 minutes to 80 minutes (#2453)
8e047e6719c316cf16886d0a92cc240f0336f59d MGMT-7574: Add V2 endpoint to download cluster credentials (#2418)
65d8817c2bc5cc7e7d938fd7b4e0d0be207640de MGMT-7675: Update StaticNetwork in infraEnv update (#2472)
6ba8da87d7880524f2e1b5bd0d86780d7a828efc MGMT-7420: Introducing disk encryption to cluster properties. (#2333)
48b20e5f010bfc2213940651cac9228a3337142e MGMT-7648: Notification on event for binded Host (#2462)
3ca606e5d625b4a83f770aced4391b63b77bf1af MGMT-4321: Bugfix flaky auto assign DHCP machine cidr (#2468)
7dd390d940ed0739d7298848abf799c8bbf67b19 MGMT-7498: Migrate multiple networks (#2445)
bc6450e3a8b0c24a52a17fd7d47edc5e6406ad90 MGMT-7114: support CPUArchitecture in Cluster (#2443)
e0c3b90738c14979e594165509495cc6c51026a3 NO-ISSUE: expose the assisted debug port and remove the liveness port as part of the patch-service make target (#2415)
e839989f5047d1a8cbafcbaf771f2b70fec36ade MGMT-7649: Update inventory should not try to get cluster if host is unbound (#2463)
2f2c8a545e3d29fc7aefda156d6819d8155ae736 NO-ISSUE: Refactor agentserviceconfig controller (#2421)
bdfa49098aa5fbebf90a974bfaa4c59cb64050a4 MGMT-6911: Validate that DNS wildcard entry is not configured. (#2298)
97f466dbce8aa486620fba3c2b1fa7a0ab375863 MGMT-7529: Migrate local auth to use InfraEnv (#2446)
ed04399172fae3d032a7c679ca6c592313afac7b MGMT-7498: Add backwards compatibility for network configuration (#2455)
19862722d98eeb462df942b8379768033f03cc96 MGMT-7566: Fix day2 printBelongsToMachineCidr validation message (#2440)
7fef5f7994d2b6cf60b7fab1c3871c068db4578d MGMT-7638: implement V2 Get Host API (#2450)
6db43e509f77df790830a2ce837e06f1b379eab7 MGMT-7637: Bump OCP versions 4.8.4 -> 4.8.5, 4.7.23 -> 4.7.24 (#2449)
a40e053cbbb5a342be9f49d496526ab41b2b90a7 MGMT-7464: Pass multiple machine networks to install-config.yaml (#2432)
a0c71cbaf924eb9666e7dfa69aea776e957ceb25 MGMT-7620: Change download URL in InfraEnv to contain V2 URL (#2442)
bff22ab3ab4a469f4f9d40c676a45f6976f21449 MGMT-7582: Fix hasMemoryForRole validation message validating by UsableBytes but the message showing PhysicalBytes value (#2409)
f5a1fc626488e7cc3460b027374b6296b5de6bd7 NO-ISSUE: OCP update only to github (#2441)
cffd89ed125d5d376b1e7a0cc0dbb13645f2e846 MGMT-7588: Replace the type of the generated clusterID and hostID (#2438)
14c5a90bda219002b2210a5de87a998663ef7f02 MGMT-7595: add UserName, OrgID, EmailDomain to the InfraEnv model (#2434)
0784d3fb3cfcd42870fbb06a99bca88d1c406d0a MGMT-7206: add RELEASE_IMAGES env var for listing release images (#2420)
7088bc266b5953eae1764afdd5f6c373963e36cd MGMT-7597: Remove ronniel1, razregev, and sacharya from OWNERS (#2436)
e807a51dac6d4e9bfe4336b7e2e61c4641d15ddb NO-ISSUE: Mount k3d binary in skipper conf (#2437)
e62a93abe62a432b054d3b2e39574d3879c9b0e7 NO-ISSUE: Create a direct link to user guide in the main readme (#2430)
1a9a6fc77d34510119e2a81a8589f737c087e5f2 NO-ISSUE: fix typo in overriding OVNKubernetes via install-config (#2433)
3700d7726ae1bf36ba3f6f82486ba3db58d42e83 NO-ISSUE: Set machine network only in case of SNO. Remove unused VIPs from cluster deployment. (#2386)
4e5d1be248533b0781436dc01b3bb094bcaabaff MGMT-7588: Fix event wrapper to notify kube-api (#2412)
135b43cc5dcc8da1b5a48995e7e52a67de2ec7ce NO-ISSUE: Bump build tools to latest released version (#2349)
b07781b132e231247608caa761f97b59642a886b NO-ISSUE: Update ztp readme file (#2370)
261a4bfdc0b3ea6129d5a336a854386888999749 MGMT-6670: Create a getter for Machine Network CIDR (#2416)
1c6533be79709a99012366d90a3182a691511ac5 MGMT-6670: Create sample ACI manifests for dual-stack OCP (#2424)
344d88cbb586e85870c014bea74175f69a348127 MGMT 4321: delete networks records on deletion (#2423)
70948d198a7d0de87012a691c3ed1b1207922c0a MGMT-7600: log ignition generator user request id from the api (#2426)
f3d119ef9e7017d712d2248eda91c1ee78457d28 MGMT-7497: Remove KubeAPI EnableDay2Cluster flag (#2407)
577382f491b06a18c61c04076c1eba6c2e71cb4d NO-ISSUE: Bump boto3 from 1.18.16 to 1.18.21 (#2395)
a5958d9b0451dc283581759f2a753ee0dad5dde5 NO-ISSUE: Bump wheel from 0.36.2 to 0.37.0 (#2394)
05a09797ade2148690bede4fee3630d106ace6d7 MGMT-7510: Implement V2 Infra Install Day2 host API (#2417)
a2ab64387bc2594e5e5bf9fc0dbffda6d9d6b120 MGMT-6670: Extend validator for host in machineNetwork (#2403)
3e44b0733ea80db230ef845441e45acee25684d3 NO-ISSUE: clearing logs timestamp when node re-register (#2374)
fd2dcd0accebc65ff380acd35034dfccc422dbd1 MGMT-7509: Implement V2 infra env download image API (#2422)
e63a7441d87e698d0e1edafe8246b41de23fd389 MGMT-7315: Make ACI CR accept multiple subnets (#2360)
2918f97ec767541838f0b200f6bdca5b3f80d16e MGMT-4321: Service support multiple networks (#2340)
2fb8fbee61650c56cacc0c406e499a6f95bd38e8 MGMT-7583: AddEvent function should be used with InfraEnvID (#2411)
a8d16c6f383ff786178a218f6e37e0b20a3a66e2 MGMT-7569: remove release getters from Versions (#2408)
edadd5e39538d7967ffdbcced14b3b4744f3819c NO-ISSUE: Add MINIKUBE_HOME to skipper.env (#2413)
64ddc32377d0bf2de9fee60cb08b1c8da8fc3a9b MGMT-7511: V2 Infra Env Reset Day2 Host API (#2391)
fad08956ebcaeac2ba61b4838f1648290eaa79fe MGMT-7251: Add minimal-initrd endpoint (#2342)
dd747a45db6b1eed368d9a144b85339d19478687 MGMT-7564: cluster credentials should be accessible only for cluster owner (#2404)
7128496b7ca0a05246d4208c9f882023f8e72188 MGMT-7505: Implement V2 HostLogsProgress API (#2400)
8eb3afe5103e7ae8ff6a5b7be8b169232790c4c3 Move the ocp version script from assisted-installer-deployment to this repo (#2398)
6ce0bc18de56560ab08e5e6e31f1763fba455911 MGMT-7528: implement V2 download cluster files API (#2401)
156fc6bab6410ffe575d7c80d3b4787577c2856d MGMT-7178: Adding new worker status, waiting-for-control-plane (#2399)
d1823eb72cb4ac6e05188eb2d17087d3617d7292 NO-ISSUE: Run subsystem waitForHostState in parallel when possible (#2396)
11926ec01f3f976fff875fe093f397d19d8f04f5 MGMT-7512: Add V2 API for reset host validation (#2389)
a48ec18d407318128d221266376f52cb9a025f18 MGMT-7444: Support OS images listing in OS_IMAGES variable (#2369)
24530bf6f048f41badbc36fa44ef9426f96583ad NO-ISSUE: Removed obsolete installation-timeout from the install command (#2355)
7e666d615c9add654ab02aadcfd3c82f9467cc58 OCPBUGSM-31544: Spoke worker BMH does not join cluster because CSR was not auto approved (#2325)
4962ca4227557d3f7953cbfb999e012cc59215cd MGMT-5443: Reduced reboot timeout to 40 minutes (#2357)
69b7616e512dec23ae5268e750d5abc58b809fd5 MGMT-4872: Add events creation with events generator (#1854)
c54d877e449520344f407ca5c1249f5d0fb4979f MGMT-7567: Check cluster owner for file downloads only with rhsso auth (#2392)
9ef1ab0f8d6ba15f84600606236682c2cdb12726 NO-ISSUE: Change IP version to golang's unix constant (#2358)
4a64c7cfd108119fd21b85ea0e5030ac088275a5 NO-ISSUE: Deploy multiple versions on CI only (#2390)
1295cfa455f6a754603d0c69b93b575d80ac9134 OCPBUGSM-31544: Set the BMH's hostname to the desired value (#2382)
52a10eaf077bc563e4a9f3603f5f3d2e3c50e2cf MGMT-7502: implement V2 API download infraEnv discovery ignition file (#2383)
b9de3c8b1204549a41bfd53df962697ce96514f8 MGMT-7443: skip removable disks format (#2378)
8f07564515cf2f91d6caf24938dcdb994a0485ca MGMT-7220: CD controller to transform day1 cluster to day2 (#2291)
6b7f79ea03fc74e65122ed6b600dcc3fef47e64e MGMT-7534: Bump OCP versions 4.8.3 -> 4.8.4, 4.7.22 -> 4.7.23 (#2387)
2b4b369e133ff997c37c2f49728b20448a77a86b Bug 1974077: Improve validation message for network latency and packet loss (#2368)
1437673a37e30917830cdd09ec45a719638e5315 MGMT-7513: Add GET method to host ignition endpoint (#2381)
e08b7584238b7a37f75e81b46803ec67345270fe NO-ISSUE: Use variables from env if set (#2385)
165e849305ecb67cc6b1b24ccb76137c10693f53 MGMT-7475: allow only cluster owners to download sensitive files. (#2384)
63d3a9be36f32fe4557d6e51a7217852d1763240 MGMT-7520: Update ignition as part of infraEnv update (#2380)
41fdc6a6285e5aaafc8d5032ffe98c0ba91a9d41 MGMT-7472: Create Agent CR without Cluster (#2365)
23f3601c07a3a0faa69ca62035b48694ea6133f3 MGMT-7234: make clusterref optional (#2377)
d76ccc1f517c3e5b6b0fb07ce409d9003c586019 MGMT-7485: move infra-env generation for V1 to cluster generation (#2367)
c74275d6d710e11a0883bb23f570e868102fa3e8 MGMT-7384: add usage to schedulable masters feature (#2376)
5ba7a42f4bfbde90b637a58123d3804502a98b24 NO-ISSUE: Add CRD update in README (#2375)
d97299c5cfd8a4264823b4136bd098edcb24fd85 MGMT-7292: Split custom manifest in custom_manifest file (#2266)
4f428149bd83d08cf7ba6e8068634d66acfb90b2 MGMT-7470: add Internal interface V2 API (#2359)
e6cd01336fbc1aac6984bba490a0a2ae2b5ba6e1 NO-ISSUE: Add default test values for IPv4 and IPv6 networking (#2364)
e17eb7d30ff1b96a80b2049317535bd1f761b528 MGMT-7069: Adding latency metric to cluster to assisted-installer-basic-cluster-operation (#2362)
3e751246329f9c8f56744b3b5e4d5f986097c189 MGMT-7487: Add list infra-env hosts (#2361)
d5e953b1e8d68fa3470c433fc8141d882bc3e01e MGMT-7309: enhancement proposal for ARM64 CPU architecture support (#2305)
789a0cc47099d0e194d838322b8d4fd58d82d63e MGMT-7468: Bump OCP versions 4.7.21 -> 4.7.22, 4.8.2 -> 4.8.3 (#2352)
da0af6543edf3e761bd243968fcb5605050e97c2 NO-ISSUE: Bump boto3 from 1.18.11 to 1.18.16 (#2356)
e8d0b0b46baf9b240afe0416e2b05ee80045d5f4 MGMT-7091: Add unbind API (#2353)
77213c8ec9a48834a7065aad85576ccbb0c25cfa NO-ISSUE: Remove host ID from upload logs log (#2351)
ac0225db1dd8652fbc1dadaa784c8f81957ebd4b MGMT-7437: Add infra-env-id to the install command per host (#2326)
42098a3a907873ada698f7a3fc9affc770ee68e1 MGMT-5444: Set 24 hours timeout for installation to complete (#2350)
6500593a80ba638f6f694549d3f5fa26c9f7fa2d OCPBUGSM-32941: Cache kubeconfig admin secret and BMC credentials secret for spoke cluster. (#2335)
0e701017abfc43eb08b4e45a2dbb8613f76c1f43 MGMT-7089: Add binding host API (#2346)
196700b78db77df32d0e40ce3824126033411857 MGMT-6897: Swagger support multiple networks (#2339)
bcf2b573c576ea309cf278f73262f674a1896a9f MGMT-4893: Add default values and doc to MUST_GATHER_IMAGES in kube-api (#2348)
c5d39e4a084f7b2d60f1afde1e30159bb283fecc MGMT-7413: Change post step reply tools to use V2 structure (#2344)
b8154c04943242ca799f12abdbe84f32cb819870 MGMT-5443 Set host status to pending-user-input in case of reboot tim… (#2343)
7b62a88d5c951af05dba26893c1acae45fc5a85a MGMT-6537: Fetch operator version from index image (#2233)
54087222c6ed238f81000bf4aa0c0fa79a207f36 MGMT-7427: Add support for hosts that do not belong to cluster in host monitoring (#2331)
4afc4b5ae51575fdf4cd30f437e11e0bb604a293 MGMT-7466: add V2 update host progress API (#2347)
1b4022329e3f7e9eaed491f52a358e92bffaddeb MGMT-6768: Add NetworkType to KubeAPI (#2318)
72eb9bbab8e16f718bec99441af9550e4841a0ed MGMT-4893: Support must gather images in kube-api (#2338)
04326d154f72cb71ece287dad19b7f016464ae88 MGMT-6735: Update ZTP script to allow for multiple baremetal hosts (#2336)
355bb8b0e0bfbc3e9711e954bfb12e044b798c05 MGMT-7426: Allow installing on OpenStack in case of userManagedNetworking (#2323)
e9a2f4bff648892d06c6ab9f1ca0e990d61deeea MGMT-7445: During update-cluster CIDRs are checked for overlap even if they were not provided as part of the update (#2334)
6be15cf10a89f20a48cb79694c669938ee7f8d10 NO-ISSUE: KubeAPI subsystem cleanUpCRs to assert via Eventually (#2332)
557a32bde447996e04fab2a57838d42c2a8c713f NO-ISSUE: wait for the 'stopped' condition to save time on early failures (#2330)
1ab926b16bb2f2009b0be4f61e98ede1da4b3463 NO-ISSUE: wait for 1.5 hours for installation (#2329)
7ba97cf76e389175de6a3f6efdea14c41101274f MGMT-7331: Validate host platform (#2274)
7d7068fb8d3afe372ee101d096c124a53795061b NO-ISSUE: Making agent discovered message more informative. (#2327)
1361b088827104aeef4fbe45005ec3a6c8706918 OCPBUGSM-32618: Create worker's spoke machines in the "openshift-machine-api" namespace (#2313)
78deb9507248ce999521347c215641f2c67bab5b MGMT-7424: Remove undeeded network validations for day2 hosts (#2322)
31f003d63d8b9573723a4234580ab336427e6eaa NO-ISSUE: Bump boto3 from 1.18.6 to 1.18.11 (#2321)
f2fc7f08f107c4787ceb067f64e5f0a9c530e01c MGMT-7088: Add InfraEnv CRUD API (#2319)
070566890afc5c579f8ef9f68f28fc9e8a4a1aec Bug 1985449: Use report variable to unmarshal json (#2282)
f2010a32179f4cb64e98749ec5ef24aa20549a86 Organize update network params (#2307)
8f89ccc17c91559b00d9b5e49d4dacc1d63ad526 MGMT-7321: Move the AI code to address the host using its IfraEnvID instead of ClusterID (#2314)
4b7bb08bc2808919e20e3dc50a01ff7a117f8177 MGMT-4893: Add Must Gather Image map (#2247)
a069d6f02a5eadbfd1b74a153ec789fc7feed9a7 MGMT-7280: add API for getting the hosts supported platforms (#2306)
80da5d4570865c34e4885c13cf8a523a1dc996e9 MGMT-7389: Create cluster with a platform (#2297)
174c814fc662c50d2e8be7ea389bb32159ff207c Bug 1987250: Remove diskEligible check for OCS (#2308)
ee5ef6fce43dcabf06492f7d46e8ca24d5fdca71 NO-ISSUE: fix gathering after operator rename (#2312)
64521edf6685aafcdd632c9adba6fbca82d95ffd MGMT-7250: Generate discovery ignition on demand (#2267)
7579a527b8b92e4cec0dfb51722a82b7139ddd7e MGMT-7398: Bump OCP versions 4.7.19 -> 4.7.21 (#2303)
1bed633debeae6a1cdbfaf156e02a5c9b9f24278 MGMT-7362: Change to infa env id from cluster id in discovery ignition (#2310)
27cf03cb7ff56fbe21e5366a41b5498b4ae79a07 MGMT-4893: MUST_GATHER_IMAGES env var (#2263)
5fbf9ce9de8f631513e60b88a82c7c66c57c422e MGMT-6735: Add configurations for multi node spoke in ZTP (#2290)
b33b6f69330b3b53524cb0118a754d9f3892f7d0 MGMT-7093: implement pool image state machine and instruction manager (#2296)
bb1e7b10d36fe65007f668433702ecda34e4735d Revert "MGMT-7280: Add API for getting the hosts supported platforms. Return the intersection of cluster's hosts platform (reported by the agent inventory) or all supported platforms for an cluster with no registered hosts. (#2236)"
76a359fcf20976cbb9e26e65b6e35b5d5f90be96 MGMT-7333: Add a HoldInstallation flag to AgentClusterInstall (#2293)
20aff0d544bf797166d6f53bb70d91aff1b2a3ca MGMT-4492: Removing WITH_AMS_SUBSCRIPTIONS env variable. (#2294)
f3dad1af1e21f9b51863a0d1cb9cca247d8a6482 NO-ISSUE: Move 4.8 support_level from beta to production (#2289)
a0abfc7cc065b5a4ba3a56b77a09094651d634ba OCPBUGSM-32293: Cache only required secrets (#2286)
dd818a5650a66ff6693f632ddb83d48d29692755 Bug 1975383: Update the defaultChronyConf (#2295)
0ea3ae4b5bd5d542aec8103268106637bccc519a MGMT-7280: Add API for getting the hosts supported platforms. Return the intersection of cluster's hosts platform (reported by the agent inventory) or all supported platforms for an cluster with no registered hosts. (#2236)
6e91d6ea27da64a19df9988e01caef150d209d01 MGMT-7382: Delete clusters using REST API on subsystem tests (#2288)
3889757c6131e30096f5f178238253dce5cf3f44 NO-ISSUE: Adding BE progress for day2 hosts. (#2270)
2c8edc42d272f581837cf05ae23444142fc605e2 MGMT-7377: Remove auto-assign param and set the default to SDN for network type (#2284)
40c23ccb2b6678d5010b70c5b9a767ed064d0bdb MGMT-6425: Add DNS domain names host validation for user-managed networking (#1884)
46cad54746e1c3d6ca12fb787f629a458c5ca4bb MGMT-6750: Automate community-operator updates (#2255)
54ce7f8b79b74bba98067663bd58e13e4a4d4856 NO-ISSUE: Deploy MinIO as a LoadBalancer (#2287)
f8b30e49cf282054df570dbd44d8ac3ac6be3aca MGMT-7268: Remove SupportFreeAddresses (#2276)
4111a6d9dc04410da74fdb904beec3c1b8b9271a MGMT-4561: Add MCS certificate to workers pointer ignition on installation start (#1661)
de933099cbe07917a1f5fc3d7e19ef39dc158bef MGMT-7374: Issue a single cluster log collection event (#2277)
f96503bcd069b1d8f008c4752df6ecf79b32078b MGMT-6897: Add network_config field to cluster (#2281)
77cb9d3348dafd2abd61fd7c8066e7e7a7805d95 MGMT-7356: Bump OCP versions 4.8.0-rc.3 -> 4.8.2 (#2268)
345587bfcf6e5f5f13b94ed83f6374d26f42ffb6 NO-ISSUE: remove unused params from cd controller functions (#2285)
3973dd76172d5001e53281f1a7026f9e34bfb9a4 MGMT-7343: Increase s3 pod volume size (#2278)
84050d56334b4fec93996a4b70946929f8f25037 NO-ISSUE fix panic in host reference (#2283)
ef0ac723185b9ae33df9f46287c583774241bda7 MGMT-7358: change host validation to support infra env (#2275)
0daa74d48c2fd1d94864c9594ca2aa8a93863016 NO-ISSUE: Bump boto3 from 1.18.1 to 1.18.6 (#2280)
45a5faa15f5a58345810225deacec430d395934e NO-ISSUE: Bump twine from 3.4.1 to 3.4.2 (#2279)
e809201cb80d359315ebc7a515c404a17ffbe578 MGMT-7087: Add support for register host in v2 API. (#2269)
da15b31996c6b0cd449c3a86255c6f1fc148106e MGMT-7219: Add internal API to transform a cluster from day1 to day2 (#2265)
fa49588aa60a275a2e9d6bb4f11ab9320e99f40c OCPBUGSM-32244: Bugfix ListClusters for admin role (#2273)
1fcc27d863f2e330bf0eef736922c1c0d279299b MGMT-7319: remove ntp validation from kube-api test (#2271)
d1ebe268cc0cec00094a08a1d3e9c54320846d95 MGMT-7197: Implementing cluster's installation progress bar in BE. (#2208)
ba311bd8e4989cccddc4c6903120c89c7ff3e4a1 NO-ISSUE: enhancement proposal to avoid agent reboots (#2144)
80c58311ebb8c07dd46abec77ad9897cebc02eda MGMT-7262: Create a ServiceMonitor when deploying Assisted Service (#2234)
dd03fda6f83b5dffb17d14340ad12934fb9580b6 NO-ISSUE: Fix validations package mocking (#2262)
adf74fab8fa3235d3c90017d550c23d519d0389c MGMT-7085: Add metrics for networtk latency and packet loss (#2187)
9fe1c244323d5e0c624a1e256fbd671513334366 NO-ISSUE update ginko version and add logs to kube-api subsystem tests (#2264)
581f79c8b3b42dfe92467bfeaf644fde404fd2e4 MGMT-7141: Add VMWare to feature_usage (#2257)
f8d40472fa83a3f21288e5f08a78f099ef1b7255 OCPBUGSM-31996: Preparing for Installation failed with message: Failed to prepare the installation due to an unexpected error. Please retry later (#2261)
05657c9979f66eb9a3e4ff777ac7aeb4d52e2056 Bug 1983412: Wrong validation status for network latency & packet loss (#2251)
92bfccfd261d2edcc8ad3bf4209594d8f21cd109 Bug 1974077: Missing source host in validation error (#2248)
384748ec5aa3a5f107681ed360f81549d6a461e3 OCPBUGSM-31406: Validate log collection before displaying LogsURL (#2241)
6a1acf885c5644d8a7242ebfe446e8941923dc75 MGMT-5171: Mirror OCP release image to a single repository (#2259)
85d1df22822ae0523539f98efeacba2cd4c4a99c OCPBUGSM-28683: Enable pprof when running in debug mode (#1679)
3f35d6cfad5156591fd76eb74dc37ffc5856a965 NO-ISSUE: download binaries instead of using docker-hub
642d924ab2d0948a69f22cc7e7871d8088c59057 NO-ISSUE Enhancement for late binding (#1838)
ced7214ee9c721f17004c5d29b49e5d7da79edb7 MGMT-7294: Remove v1 from swagger basePath (#2245)
34f0b498741ec92efc09755a6a8bc4f8d39587a9 MGMT-7235: change AI implementation to use InfraEnv instead of ImageInfo (#2232)
874bddad7d8e90de24fdf01750cde510a536f964 MGMT-7308: Increase timeout for agents in ZTP flow (#2254)
b3b645c522896e1558d4ee277f585ca9242a15cc NO-ISSUE: Filter out Clusterdeployments from non-relevant namespaces (#2252)
78658ffcef94ec6b2a8fefe8d8bb64dde8f41112 MGMT-3934: enhancement proposal for image service (#2172)
108a211c03cba7017675f682db9dad53e8c7ac15 MGMT-7306: Use local CI image for spectral if it is available (#2253)
061bdace8ec78616bb6715b39a5f087223ade971 NO-ISSUE: Bump setuptools from 57.2.0 to 57.4.0 (#2250)
15ddfde049517bf8bc41e4eed241fecfe7b75749 NO-ISSUE: Bump mkdocs from 1.2.1 to 1.2.2 (#2249)
af7c6cbbd6f60b27cf818443081faee90d265eae MGMT-7297: Add view agent logs command to the agent message of the day (#2246)
39644f16fc9b76e857d3466e65d490e287a20257 MGMT-7104: Add new API for updating VMWare credentials in the assisted service (#2175)
40c33eb3024bcb4bd8972f7db6ba855d724491ba MGMT-5302: Removing deprecated /host_requirements endpoint and related model (#2235)
e459dc408a0acb3a1bffd14d28947694990c1770 MGMT-4540: Support schedulable masters cluster property (#2075)
5c51d15b384df83ada2d2f8ccf0b4773ac849583 MGMT-7287: Monitor user selection of networkType by setting usage when user select (#2243)
279aa303836734a15f25b06c75e2f3722544145a MGMT-7086: Migrate data from Cluster to IngraEnv (#2244)
8758e8197b6bdd44bfa2e652f344ed6c8e3485fe MGMT-7288: Add degraded cluster event for failed OLM operators (#2240)
a415142ac645b35073d8f0c193d0a6c562e81e3c NO-ISSUE: Bump mkdocs from 1.1.2 to 1.2.1 (#2216)
93ef80a1dc0573674e99fbccc3df0003316bca10 NO-ISSUE: Bump setuptools from 53.0.0 to 57.2.0 (#2238)
12d033890f5ff671d78c990e32af7071f7bc1df7 NO-ISSUE: Remove unused srcStatus from updateLogsProgress func (#2231)
06e94a6f7c0dc52e9c00d3a4f1900573fd21293c MGMT-6768: Allow users to choose between SDN or OVN network type (#2113)
d90cbeb1e19bb8fe2623513c006a10b834e18770 MGMT-6977: Make sure that preparing for installation timeout is more than the tools timeouts (#2221)
bef83a8bae6684a794d4efc7eb821d086cafaa7e NO-ISSUE: Bump boto3 from 1.13.14 to 1.18.1 (#2239)
7eb89562b6d95070493c8f30bceeb3f90d2d6c76 NO-ISSUE: Bump twine from 3.3.0 to 3.4.1 (#2218)
29d4be31efcc57e44f66fefc7786d1a9502ec9d7 MGMT-7286: Bump OCP versions 4.7.18 -> 4.7.19 (#2237)
f63b542baf99895af6ecaee8337ca832732f145b MGMT-7210: Upgrade Go version to 1.16 (#2203)
d273fa3e4ae599f19e6b665b4e1ab42480cfb3d9 MGMT-7086: Migrate data from Cluster to IngraEnv (#2229)
9f1ecf08fa418ad5c8f6a09805ac7c83486da0e9 NO-ISSUE: Removing Install() method from cluster's API. (#2228)
9868189234b057ef0d07e3dfd3392eed991e6a12 MGMT-7054: Use a network LB to avoid download issue (#2226)
de2698f070e6207d0d5cd69d8874e1769cd38256 Bug 1975672: Gateway is '<nil>' in route (#2223)
234fc30c5d20491f968587656ab6428beaaf18a9 Bug 1974085: Worker host IP appear in master validation message (#2098)
48cdd53a6ec96f39b67c92d24ad0cf3e5ab2a8cd MGMT-7214: Add InfraEnv model (#2207)
41f818e1fc1dd6e1471321aae2441324f0839c37 OCPBUGSM-25122: Unexpected host api-vip validation before setting network parameters (#2209)
0c11996a702c2efdbef4c847260b6a8ea8be169a MGMT-7154: Flaky test: Host tests next step - DHCP (#2227)
98108bf15634fd83e3ffa7eb8567250c20e7f881 NO-ISSUE: Update document (#2225)
65aec4450d787ed90d5e0932342cc960bb56e88e MGMT-7228: Add AgentClusterInstall shortName aci (#2220)
b87894c7f47091a88ca8f26ecd8018a00349e37d NO-ISSUE: Make dependabot commits prefixed with NO-ISSUE (#2219)
a562cb03837d2bd36feb26dbf7922246eb7d8247 MGMT-7111: DISABLED_STEPS environment variable (#2210)
baabb97ac646acdd839294b4d08d95b3c4d82838 MGMT-7195: Add calculation of L3 majority groups to cluster monitor (#2196)
54ba4df05f13a54faa7e86a28304dc042317fd7f MGMT-7212: Fix crash in PostRefreshCluster (#2206)
88d03a2e1072b685d2bc5eccbe1118d172c2e587 NO-ISSUE: Add dependabot.yml file (#2211)
d9e97760130c3923a643a292a939398c094f974e MGMT-5171: Mirror OCP release repositories instea of namespaces (#2205)
6fef45e608dc9a33f8acaa55eb0160d5842822d8 MGMT-5171: Mirror only assisted index image (#2197)
8852a552c2751544eadb4a080b0bee0a4a7f8dd5 NO-ISSUE: Remove deprecated IMAGE_BUILDER var (#2201)
87aebd077d299c26ae93c254c706ac41b4f72a09 OCPBUGSM-30272: Clear ACI LogsURL and EventsURL in ClusterConditionsUnknown (#2194)
1f1460d8b429ce58d5aa6f6c36d9e1760fa402a9 MGMT-7136:  Add metric report to all installation complete scenarios (#2183)
d5a9a26ec83379b7f1d32621e6f839df68ce8868 MGMT-7170: Adapt connectivity groups to support L3 connectivity (#2193)
8e281ff3251ffac35ac7f58ee280678ae6e6a9ec Bug 1966586: 200 OK returned when setting invalid Base DNS domain using API (#2112)
ea07b14e274005ac7d941f44b63fcdffaaeca917 OCPBUGSM-31903: Match 4.7 rootfs with iso version (#2189)
2b413b3adbb016dad58f9b687d2b6616aca393f1 OCPBUGSM-31691: Add Machine net CIDR to ACI status (#2171)
659c6f91f5be932e3023aba3e1ebdee0bad10d27 NO-ISSUE: Use spectral image directly when needed (#2192)
e399ac41aefb1b26afc955603414f01b0dd4dcb5 NO-ISSUE: Don't lint swagger for now to make tests green (#2190)
15aab32fd5d68aaa73ef20771b34de98398de430 MGMT-4179: Move KubeAPI types to under the top-level directory (#2186)
62537db0a8854f9b8f31b6f5fb524a4efe45659c Bug 1978691: Fix osImages reference passing (#2184)
951b9a9b9b1531d45856a03da1808c7e2bb6fe71 MGMT-7121: Add vsphere platform support to install-config.yaml (#2124)
34d3dd4ad85391b5a48dc420c8305c29741bc740 OCPBUGSM-30766: Removing "Unauthorized access to cluster *" log. (#2170)
973880c9591447a8a4f0e798c48e832c0ca1d10d MGMT-6961: optional argument to cluster_list REST API (#2160)
c28ba5e4ff237cfdbb9f187baa9c9e5dfe695b12 MGMT-5171: Mirror all available ICSP on script (#2185)
9f68e6646bdaaffbfa30242854dda8189ce926d5 OCPBUGSM-29517: use UsableBytes instead of PhysicalBytes (#2115)
1e981d62390d108e5e938f27f57061165bb56099 Bug 1979169: Clarify documenation about automatedCleaningMode (#2162)
3d61b82ee22efd9d4c67acde00358d3026385f89 MGMT-7189: Bump OCP versions rchos 4.8.0-fc.3 -> 4.8.0-rc.3 (#2178)
b425c9e13270bdeae2b4aca519f97d03c62e7aa2 MGMT-7054: Mark iso download tests as pending (#2182)
35dc5c7889203d3cf36f4a8e23a03a6c93a83749 Bug 1978739: Fix requeue logic inside mapInfraEnvToBMH (#2173)
ceb643965e0a2aed57f4505168712f44c9505a05 NO-ISSUE: Fix CRDs description
de9da0b521aac6ba593cd975f2678c6ea8adff2e NO-ISSUE: Remove -u flag from go get commands to use fixed versions
fdf3c3e3d59b941678b1d0fc184ce2ce49579937 NO-ISSUE: kubeAPI subsystem tests: decouple ACI and ClusterImageSet Creation (#2169)
364ac6828d1b9b86adcd402e3d905b8c08534d23 NO-ISSUE: Enable Day 2 cluster in kube api (#2159)
b7bb45784ec102fe5bae3d62e52ddb4ed88cbb40 MGMT-7083: Add additional timestamp to trigger monitoring and replace updated-at field with this timestamp for selective monitoring (#2091)
5366b48f8d790cd1ddb096138b67e99b62b936ce MGMT-7163: Bump OCP versions 4.8.0-rc.2 -> 4.8.0-rc.3 (#2166)
b79b701ec048cddf663f9d9d81075436edb03cc9 MGMT-5171: Fix quotes on setup_assisted_operator.sh (#2165)
84cf6f51776b5c6ed50e9cd898ce7c3390c0643e Bug 1937696: Use hostname for BMH resource name (#1992)
3528c60948c76f3b7ef13eca788820fef080ef0a MGMT-6663: Make an event for any operator update (#1879)
a2423cfdd1a369ae21224c76d21bddf005277ed0 Bug 1965117: Keep assisted-service configmap mount updated (#2137)
51aa0877efa331ca8eb8d8a2eec264b70150df3a MGMT-7142: Bump OCP versions 4.7.16 -> 4.7.18, 4.8.0-rc.1 -> 4.8.0-rc.2 (#2153)
e663324dfefe17c11b3cd04f6314364a93b6053d Bug 1975529: Remove unmet requirement message from log (#2157)
48ab6731761a88f32ae64fe2339a535d68d631f0 MGMT-7152: Adding verbose printing for ginkgo. (#2163)
9d46226645378e553afd2fe469f53dcd050bfc2f MGMT-7144: Add verbose flag for tests (#2164)
7bc89fcbdb3cd412e40df1dc74a520f1a5bd5399 MGMT-5171: Call set_ca_bundle.py script from the correct path (#2161)
6ef5bdf85aa856c1b8d06d9ed483036f8bb0b4cf MGMT-5171: Disconnected IPv6 full worfklow (#2148)
228443466618eb316c1698b3b53371a0f103c8ce OCPBUGSM-31176: Fail the installation if there is only 1 installed worker. (#2154)
80ccebee5062b6407922e8b7bf5225880c33a968 Bug 1977354: Move agent to different cluster same NS (#2145)
edf25fabe0468d16073af7330528e62c49824183 Bug 1976983: Add docs explaining automatedCleaningMode overrides (#2146)
15cf33e489445315457e8295e708870d251f64f8 BZ-1975491: Added network latency and packet loss to /host-requirements endpoint (#2132)
c9b09ce3f96fa925a47d0197ecd402b554f62964 Bug 1975452: Fix spoke BMH provisioned registration error (#2141)
c704f8497a4369d951a981e691a076db48f4685a Bug 1970063: Don't force ca-bundle.crt when mirroring (#2081)
cf608969436d5387e8ad6976a093ee56f8ea3c8f NO-ISSUE: Move live iso test out of image type loop (#2150)
687ed5f0379139a448075b17ae2c2714515a10c3 NO-ISSUE: Show full command on release.go execture error (#2139)
8f954e7ac2a2df0e4def48c85de27cff4ab59364 NO-ISSUE: Add common module for operator deployment scripts (#2140)
3ed09f53cca4c011da2004059d1bbe8638f9383e OCPBUGSM-31584: added columns to Agent CRD (#2131)
648ab504beb14171ebe480c7f5faee2331262524 MGMT-6908: Adding enhancement for installation-progress-bar. (#2042)
6857095decf2bb77e99099a1ce09a38c76631355 OCPBUGSM-31522: Bug 1976776: Change agent's ReadyForInstallation condition into RequirementsMet (#2135)
b1ffbf6925eb9e5ef249cc2298ea0a97be065f03 Bug 1946178: Fix OCS validation message (#2055)
4e8047dd68a2da54a9e6a0b59b76552efb556b4a Bug 1959869: Set OcpReleaseImage for RegisterAddHostsCluster (#2095)
0b0e3677ae83799151d11f1267cbfa39bb0c6f2e Bug 1977444: KubeAPI getting started guide (#2133)
dd9644ca25fd4ffb62944414d1323d3e0000de84 Bug 1977449: Fix flaky test: invalid NMState config YAML (#1847)
bf201b6a37d2101c81d1c84833396db31fbbfc5b MGMT-7116: Bump OCP versions 4.8.0-rc.0 -> 4.8.0-rc.1 (#2121)
8edfd26f2d007e17903d2d780d7e8dcdcb83d7b7 MGMT-7082: Spoke namespace should be different than assisted-service namespace (#2120)
32a85579ce96247ebe1636036ad93f6b3408bb67 NO-ISSUE: Fixed a broken link (#2130)
a3176636c377aa2d3669c6d5bd7166f588fc1a9b OCPBUGSM-31519: Adding api.<cluster-name>.<domain> entry to sno dnsmasq (#2123)
0fa7f1ff026dcd26291787a499e49f168b86f107 NO-ISSUE: Add an issue type section to PR template & hide explanations (#2122)
e562e51479e30742be983d064309d3cb57eb38e2 OCPBUGSM-30214: add controller for AgentClusterInstall (#2067)
cba772327c6623f3358d43ed4b35cb859f18a329 MGMT-6808: - docker push command hasn't the --tls-verify flag (which is a podman flag) (#2107)
0f3e4f04f142ac0a4c4ba4da520f5ccaa365c929 NO-ISSUE: Add more troubleshooting to BMAC docs (#2100)
cfb4c45af79d59491abc2670c811ae93f83c3b5f Bug 1968448: Add CVO progress to condition (#2110)
c64412c50327d024e09550c7d6e93d882324b4e4 Bug 1968572: Assisted Service does not escape backslash characters on public SSH keys (#2060)
0834ae92462120ac29600197f02e6168175d3168 Bug 1969391: Fix InfraEnv missing ACI msg formatting (#2109)
1e984c12b4d805da12e67720fdf106cd946e66a8 NO-ISSUE: Remove AgentsLabelSelector from ZTP flow (#2108)
37948fe810690b6bceca694d441f83061a77590e Bug 1964471: Add AdditionalAgent Reason to condition (#2089)
549a7faecbab833bb7d2422cdbc66b5caedcef04 MGMT-7084: Validate clusterDeployment status becomes installed (#2104)
0bb4771d8e36b3dd6ccb3f7432e1839d45e6de9b NO-ISSUE: Move baremetal-agent-controller doc to docs/hive-integration (#2105)
0c43c1dd9d1ea4a85cbd145b881f43b2967d36c1 MGMT-6500: Add host validation to check for default route (#1785)
4752fd82a8a6313dc63b528e7ec7b1a2fc77c32a Bug 1972598: KubeAPI: Adds install retry doc and reorder existing docs (#2076)
bc8b9c1095056c35ec6587aa61f2c690bcc4f371 MGMT-6860: Add config for the spoke cluster in ztp flow (#2090)
cf50f3cb4abc10ae37c40e56bcc3d64d9f33f147 OCPBUGSM-31346: Production logs are spammed on "Found unpreparing host" (#2084)
4f6cea644a1163d107009b99cec1334a5ac2819f MGMT-5171: Support IPv6 networking params on ZTP spoke cluster (#2087)
1f8bc81218f5093b3b47cc2558a7c9d033af2e71 NO-ISSUE Add skopeo to image and log image information withouit running a container (#2029)
fb6a48d2d4d8cf2880ed824dd4a5132baa2e7b38 MGMT-5171: Fix setup-disconnected function if condition lacking a semi-colon (#2086)
e35d52acdc33fc1e2cefc7b2c38b5abef2a0d1ff NO-ISSUE: Create infraenv in assisted-installer namespace (#2083)
e465669ebf558da81537e33889019b1cf88f5636 MGMT-7074: Update OCM sdk version (#2082)
181af442b23c8d577d51a96dac6166584e2a3c6e Bug 1975218: Move conditions const to CRDs (#2078)
c1aa988f5c732893d6e5adaad90a06e2afa3cd04 MGMT-7054: Use Minio over scality (#2071)
23735a3f1a0b6faa0cb9bb5f9cec33258944cfda Bug 1970567: AI Pods throws errors cannot access the media (ISO) - media was likely disconnected (#2061)
6e910fee3989d899ded2362854cbb1d67d236d67 NO-ISSUE: Add pawanpinjarkar to code-reviewers (#2034)
f0584c49e53c2b11ce7d18dc19d3b6b6e85d653b Bug 1968552: Wait for ISO for 1 minute before using it (#2032)
08cc95e60231b99ac0106674513426586c5a0fd8 OCPBUGSM-30075: Update error messages on invalid OCP version (#2027)
6eb74f293cddfcf085134546761a7019de001873 NO-ISSUE: Remove duplicated transition tests (#2079)
af1927b8008426069c82a382498dd2b1612a3bfd Bug 1974501: infrastructure operator rename (#2070)
642c98a17c82b48cb5e78afe4d2b4ac349f280d6 OCPBUGSM-31316: reduce poll interval for check NTP source (#2077)
599b72dda698d6269d57c80b903109a79898ab9c NO-ISSUE: Elaborate assisted-service tests documentation (#2085)
7f45389cd2117f319853098ee662e6be78aef3d6 Bug 1968423: Document kube api teardown process (#2074)
b5f9a4240adb4a71803bcec9c59f947f52122c49 MGMT-5171: Deploy assisted operator in disconnected ipv6 env (#2052)
568c24282c8b22588c1fb5fd6200812c4e05a993 Bz1974085 wrong ip network latency validation (#2053)
108ffe26acf93b439ed12aa71a9f11c9dfcebdb6 NO-ISSUE: Fix a PR template typo (#2047)
099da76cab157e12d77d13bc473a0c7659789b29 NO-ISSUE: increase timeout of waiting for pod for disconnected flow (#2044)
bcd041742cc72a8565b0d9783730122b8a3db6bc NO-ISSUE: Update BMAC documentation (#2069)
3def39ed6c582aaf96fcabdff9b496da49dc2bcd NO-ISSUE Adding sagidayan as a code-reviewer (#2062)
425735e21f5e5e8508dbc83b339980e825e06884 OCPBUGSM-30203: remove cluster_id from prometheus metrics + update tests (#2045)
6a6d635897111f52486220c0353ae7b9d20ff087 Bug 1969547: Create KubeConfig Secret when install starts (#2041)
2ea77054c7eda0a6cb3e05fb805329ddbe557fce OCPBUGSM-30296: Delete unregistered hosts agents by namespace (#2018)
ad7260c5a8583fd945fd58096d617cb5ebfec669 Bug 1972525: CD controller to notify InfraEnv for backend cluster registration (#2046)
3e4168fdd46990aa85a62a02f9d71b7705a9b3d5 Bug 1964623: Tune FS disk usage log messages (#1888)
89a3b0669b6aff875eb4c42dc949cbe99982d3e8 OCPBUGSM-30844: NTP status is Unreachable after disable - enable host (#2051)
c5c6125a31b2f8691b919af4cec077b01ae5a23b OCPBUGSM-29588:  ACM/ZTP with Wan emulation, several clusters fail to step past discovery (#2009)
0cedf4ab3e4e7de4a66d11eb4a47e3134281d76d MGMT-6806 - Enable remote debugging on Beaker hosts (#2039)
ebe50b8caf2ef2fc8890b917339b1f74a2ed09f9 MGMT-7045: Bump OCP versions 4.7.13 -> 4.7.16, 4.8.0-fc.9 -> 4.8.0-rc.0, rchos 4.7.7 -> 4.7.13 (#2036)
f9823d44577607ceada66d4d83aa58dda95740ce OCPBUGSM-30324: AI KubeAPI AgentClusterInstall confusing "Validated" condition about VIP not matching machine network (#2023)
b93f86c2fdf84f9a542fa93c5fb8ca88ba245479 MGMT-6764 Apply timeouts for waiting for amount of agents and waiting for agentclusterinstall to be completed (#1885)
ede9f21da7d534d4fa7c21927f6cb2ec54b74ef0 OCPBUGSM-30089: parsing error indication for config override (#2020)
ee3da07fb0c0ee6c8ef952db870a3b64ebb26e35 OCPBUGSM-30887: InfraEnv should always requeue on HTTP 409 backend response (#2022)
59b3ded8a6acc0521a74509d100730e74973b3a7 OCPBUGSM-30258: Fix empty cluster name after applying InfraEnv.yaml (#2040)
5904203764b98b484b5e53b382c106939118f6fd Bug 1968425: Apply labels from infraenv to Agents (#1998)
6eaed6fe36c00d45505505bc7c099684d4372162 OCPBUGSM-30121: Add Image CreatedAt to InfraEnv status (#1975)
e3418973cb0c2e08cd63fafab85afa0c3e0cddc8 MGMT-4585: Enable flexible scaling for OCS (#2005)
c0c0ed9239c495118883573dde2ef9328a86eb4a MGMT-6712: Enable host validations for network latency and packet loss by default (#1853)
6b5855e7f8ec770bab1d8373e4c0d373cf7202e9 Bug 1972096: Use .invalid domain instead of dummy.com (#1993)
eb92c757899bc07d882ec82d00eb074249b2a198 Bug 1968124: Clarify "Mirror Registry Configuration" doc (#2021)
8fc159f621f32e7389cd0ae7cee6f52a22414cf3 Bug 1967956: Propagate proxy config to service (#2026)
3c5e4c5ed6f86fc785021c4c9061e5e6aea24ec9 NO-ISSUE Add results to cluster.installation.results internal event (#2028)
f616be5ba6034fd3095eb4c14068a3ed1a10724b MGMT-6806: Rename DEBUG and DEBUG_PORT flags to DEBUG_SERVICE and DEBUG_SERVICE_PORT (#2019)
39b088d1e294fe4f5df0e7c1e2bd06f3f855c493 MGMT-6942: Bump OCP versions 4.8.0-fc.8 -> 4.8.0-fc.9 (#2012)
687c744aa6d39dde1d5f71ce7cc51a343bda8829 OCPBUGSM-30350: Add Progress info to Agent Status (#2004)
3fa664372be25e43957e23c10a4f310d06c020ce Bug 1971162: OCS check if the disks are Installation eligible (#1999)
ef553a48488e1295c6eb79650076cc37f0acbc60 OCPBUGSM-30211: cache image fetched from release (#1997)
5be0659d69485fb2bf371d992cf2ea301e8754cc NO-ISSUE: Add lranjbar to OWNERS_ALIASES (#2024)
0dfa60bb973cf336f79f78bfc7c4e387c7c04498 MGMT-6628: Exposing the deregistration time on cluster API. (#1995)
081036c9f0f11c4725565a627ffa39fb3d065a13 MGMT-6286: add image mirroring in operator installation on CI (#1950)
c0c6711019d2fe86466e9a91ae721674080f184c Bug 1968125: AgentServiceConfig examples in operator.md doc should each contain databaseStorage + filesystemStorage (#2002)
95e05344b12363b461c6a188a96f7b1b5ed69bfe OCPBUGSM-26021:  Can't proceed beyond the first wizard screen, if a cluster already has VIPs but no hosts (#1990)
9e6c76214c3be6adf7cde2c6b4ecca3070396153 NO-ISSUE: fix hive installation to create namespace and OperatorGroup (#2017)
2dfc8976cd95a7122f302dbd793c5485b666d7bf NO-ISSUE: Make operator deploy.sh exit in case of error (#2014)
124ac4b1f5d7b33516f1fefd1e0ee4c5bc3484bd NO-ISSUE: gather hive logs on CI (#2006)
5ccdf83ab301eb668593296d53c02c647deac3b0 Bug 1966199: disable /etc/resolve.conf handling by NM during bootstrap (#2000)
f777531f522b8e2b4df4b6963729683f73a5ad41 OCPBUGSM-30076: Add role, bootstrap and ntp sources to Agent CR (#1994)
d07966e3b06a70b18b6369cc2b2fd52c41a10b90 Bug 1969796: Fix logline containing ConfigMap for AgentServiceConfig (#1996)
0fec37e50a8f7da1ec85f27edf8f0f49f705f18c MGMT-6024: Merge setupNewHost subsystem utility with registerNode (#1865)
eecbcf83cc9ff5ce8b8b507c4d638cdb3abbf2ba NO-ISSUE: Use /cc instead of /assign to link PRs to users (#2008)
54318fab4c9664b0e9a6b029fddcf8679dea2876 NO-ISSUE: Change default value for BMH_DETACHED_ANNOTATION (#1974)
06d15ca786a452d4940f213314980a90ee59e6ec OCPBUGSM-30853: Change default telemeter server of installed clusters to prod. (#1988)
209338620142cdbc36b42e0910990b36f77c16bc Bug 1967773: Cluster folder should be cleared from FS (#1932)
ca2104fc8f6d23815b01a34cb9ed46f3b341587f Revert "Revert "MGMT-5430 Move assisted service image to stream8 (#1763)"" (#1788)
c74f617e00afd9a1dbc79472541f52297da8dcfb MGMT-6647: Allow wildcard no NoProxy with OCP 4.8+ (#1957)
6fcaf82efd6f8329b46f02145919235af9a88d4d OCPBUGSM-30146: Fixing the issue with missing data in /etc/resolv.conf after reboot of SNO host (#1971)
7a7082140c8db6a48762198017ed3e3028c934e0 OCPBUGSM-30179: Remove unused fields in CRDs (#1982)
8c3e92a887345ad011cb16abda663bcca79bf9fa MGMT-6747: Media disconnection: Mark host as failed and show an Indicative error (#1867)
52dd09d9b935b35a5a92d146581bd142e3339940 NO-ISSUE: ZTP CI gather more CRDs (#1983)
091ce1d391ffb80a9c601a43e092a06c3b969ce6 OCPBUGSM-30056: host namespace on agent update notification (#1941)
b1f2f40d742fb8967fde6a611d264e931acfd096 OCPBUGSM-30346: Populate State and StateInfo and move to DebugInfo in CRDs (#1972)
0b3a8e5d260cd1b8e1b0292b7820afc77a96fdc5 OCPBUGSM-30278: disable metrics event when deploying via operator (#1980)
add3131fb4f28c1f49ce36617cc8727b23ea0c10 OCPBUGSM-30082: Don't reconcile BMH in a detached state (#1943)
d35ba1c854f4c4d43655ae2d3ee7778629501b08 Bug 1969304: Don't queue BMH reconcile if the InfraEnv URL hasn't changed (#1862)
d6a893f4f1e25d7666c0e5d631806ff72df29201 MGMT-6607: Fix OCS Cluster Validation and remove minimal mode (#1807)
492b191caec3d25b9250cb2744339b77c8b07dde OCPBUGSM-29458: Check the response status code from http.Get (#1958)
26ec28b940cbb44321170f5438ba2e07eff46945 NO-ISSUE move check-commit from tools to hack directory (#1973)
6e674cd792023e987e864e610844eaac83eae0c8 MGMT-6707: Move cluster status update to central function (#1969)
d88078bf8db55b6c891c010eae06adec04a1fe89 Bug 966545: Installation fails after cancel and reset of installation before node reboot (#1964)
3cab52dfe9474282b7a7d71139e7447f7ae827c2 MGMT-6848: Bump OCP versions 4.8.0-fc.7 -> 4.8.0-fc.8 (#1954)
86ad71a59b8ba374f8564323f5fa9098a3ad4e07 MGMT-6849: Remove vmware vxlan tunnel offloading patch because it is done by OCP (#1955)
13c2dfc4588e507637d9cb3eed6ce28d701a5690 Bug 1968631: Missing request ID field on image uploading logs (#1961)
137fc5ad3b67046c4eaf58ea08f11051ce497531 assisted-service-operator: bundle versions (#1902)
972a2f080f22ff0bb89ff6a63522f30b231b746a NO-ISSUE Use `annotate` instead of `apply` for AgentServiceConfig annotation (#1967)
3271d7abdec0798ca1c53520adf7e98843edd751 NO-ISSUE: ZTP flow gather agents CRDs data (#1963)
6a027509253edf10483dae98a9d6c8363b640b39 NO-ISSUE Doc update: add example to print ACI conditions (#1956)
20c61e40a55badf19864e62428a43391e364187d OCPBUGSM-30087: Fix doc for installconfig on ACI (#1959)
81a252cd6ee42175410e7da038a5ac4d237aa71a Bug 1966989: asc controller log line (#1946)
434ec717f59cf24fb900168c5611e4877ad3b1ff OCPBUGSM-30084: Always disable inspection and cleaning for BMH (#1948)
f53ecb77179b97aca4a34a32b9b19086a411e6ad NO-ISSUE: enable AlphaAgentInstallStrategy feature in hive (#1947)
2a818e2c18bbdaf40581a790038c32b5a9693879 OCPBUGSM-29808: Wait for REST api before starting controllers (#1937)
aed2da2b4a1608cf0b87520ce9a44ee9e49a57f1 NO-ISSUE move provisioning configuration for watching all namespaces (#1930)
48d7b50096886a0b1d2bd923443a734efba30e15 NO-ISSUE Add CI to the list of environments for the PR template (#1935)
9c2445efd59b042d11f085f79d6fa7c7184b2ee4 NO-ISSUE: Add djzager to ci-reviewers (#1921)
0df53cff6eeb960c7722015aa5449cb41f039b2c NO-ISSUE: Fix  grafana dashboard annotation (#1940)
1eed78b4673ebddcb7b3b89ed813cce1a220d903 OCPBUGSM-30068: Revert "Bug 1967121: Docs should clarify that the pullSecretRef is currently ignored (#1898)" (#1938)
5633679707b87fa2563a79a718ec361181b3403b NO-ISSUE: Add to deployment status dashboard installation status (#1936)
781ef2173e8732606d526a1eba047f7c64d09801 MGMT-6832: Bump OCP versions 4.7.12 -> 4.7.13 (#1928)
717fa9ef72985f3000375f2e122086bcd523004d Bug 1967423: CD ctrl reqeueue after 1m when failing with AddOpenshiftVersion (#1912)
60ca54b2658ecefe9c28f352ed6b7cf484fe5837 Bug 1966546: KubeAPI keep day1 cluster after install (#1900)
4d4cfed06a285649979e23866bfe6fcae4219875 MGMT-6775: Bump OCP versions 4.7.11 -> 4.7.12, 4.8.0-fc.3 -> 4.8.0-fc.7 (#1890)
96af3672cacd33873f7053a719efda54b7b65d4b Bug 1968067: KubeAPI add all none-success validations to conditions (#1926)
c54fc0932edd7553fedb333f25206a8b3aad4e1d NO-ISSUE Add mkowalski to OWNERS/code-reviewers (#1914)
f33eeda865b4f98c4bb89e40109b0ba2d313c0a1 NO-ISSUE Fix spelling in the PR template (#1910)
aa8b4ee6985547dfc47aa70cdbf19164f6e2e63b NO-ISSUE: ztp flow download log as insecure (#1924)
403985c8d95b5bef173a11326b3de7aec3fdef18 NO-ISSUE: ztp flow output log to file (#1923)
481b03a775007b927dd0ed108f22f98b7f76db9d Bug 1967842: Removed log messages from OCS cluster validation to prevent spamming of logs. (#1920)
1f0e02b44f242dd69bd6b1f3ed3f9ea265447b41 NO-ISSUE: Fixing metrics subsystem-test's spamming. (#1908)
b483364bcf6a7c9f604966537b4e747b277f1d5b NO-ISSUE: fix docs to make use of 'EXTRA_WORKER_<X>' configurations (#1915)
716e676ab9e38f51388c7f753cdb42a3aff02400 MGMT-6533: Skip "Token used before issued" validation in jwt-go. (#1846)
8debcb9c2f9934df079b415b58afca83b57f88d9 OCPBUGSM-29525: Assisted installer chrony manifests missing index numbering (#1906)
23664754a758248f7e5ee9211762c57d7940dc6b MGMT-6607: (OCS) remove resource checks in ValidateHost (#1873)
ef7016f687618279f770dcbabb8d64c597deff4e Bug 1967102: InfraEnv should log the amount of NMstate Configs baked into the image (#1899)
2f31208aae6c9d2002d0ea64074c5a9c7f420677 Bug 1963684: Return zero for DiskSize for OCS GetHostRequirements (#1872)
1ceca5f22d3b20fdb4128b28553b7e6aa2581969 Bug 1966892: SNO node cannot transition into "Writing image to disk" from "Waiting for bootkube" (#1901)
00f62014822a8387fa2f574af16f69efb3a85a4a Bug 1965356: Change install config override example to OVNKubernetes (#1909)
8a9f14ef82d4716b30d5a588bca2e777a9329164 MGMT-6286: install AI operator on disconnected env (#1895)
6822283ecbf84a6376b04599596b658763707244 NO-ISSUE: Extend waiting for pod to 20 minutes (#1907)
0ced328781d5683f5f464b8c095f3bd99d358bcd Bug 1967121: Docs should clarify that the pullSecretRef is currently ignored (#1898)
0d10efc9109d91dd092ce1e8d520215757e7413c NO-ISSUE: Fixing typo in stage telemeter URL. (#1897)
d19e94a28a5f495d25d287a3f77f272e5503a208 NO-ISSUE Remove context log for Periodic GC for spam reducing reasons (#1889)
960b1cc055e7eda725d354b11cc83eaf58ad65a2 MGMT-6765: document how to run ZTP workflow (#1880)
72f7a8848f0286d873119948643cdc80c05ba2da OCPBUGSM-29623: Configure IPv6 DHCP in dual-stack (#1864)
2bd1cedff41fbc05aa545d5bdea0d5ef75a43a51 NO-ISSUE Enhance subsystem waitForState functions (#1887)
852c9591dd6b89a675e00787e58467a9ad41128a Bug 1966485: Wait for deployments to be ready before marking as done (#1878)
2224cf88be009b4c4da0810668cbf1b2cfa0f389 Bug 1966268: remove default.nmconnection as a WA for NM priority issue (#1870)
708eee70ca31d785cb903a67ffbb35b9f72ac9dc NO-ISSUE Add a PULL_REQUEST_TEMPLATE for assisted-service (#1842)
10d22e2f747f0c217a537eed74d5377f24e7651e NO-ISSUE Add a PULL_REQUEST_TEMPLATE for assisted-service (#1842)
db02af76e788bcea89ad01023e184daa34500f37 Bug 1965356: Fix InstallConfig override example (#1886)
3a302b8a985feb63fac313a49c744fc273284acb MGMT-6014: Missing VIP values in SNO cluster (#1811)
a532243a2115301418b52267172e60b228d3bae7 NO-ISSUE migrating gathering logic to assisted-service (#1875)
b08a72e08efd6f4c11b61e4f6ee79862b728110b NO-ISSUE Fix host metrics stage label on ELK (#1883)
ee45809f87d30f1b04bd913ffc11276807cadde7 NO-ISSUE enable defining public registries that should not be validated (#1874)
1d66593ba0cfe317d6fc005f96695f4bfbdbdc88 OCPBUGSM-29621 Unify client Scheme registration (#1871)
1d9e078f900e159d0b7afc09b9eb78f6d58648d6 MGMT-4189 - block in update cluster setting API VIP DHCP allocation when user_managed_network is set (#1866)
03af71f3106f1477e8e40e133c45cc67186dbc60 NO-ISSUE Check commit for bugzilla prefix (#1863)
0bd87b825bf37d00780d0895bb1c22ab976400d7 OCPBUGSM-29721 Keep Image URL for existing image with auth=local + S3 (#1861)
04379123dcd2b37b76d3d733ab178abaa4435ae0 NO-ISSUE Add HostStageWaitingForBootkube ad HostStageWaitingForController to the list of bootstrap stages (#1882)
3ccf42606b012909e9df4b1fb874b3e4933dbd74 OCPBUGSM-27422 Kubeapi cancel install before delete (#1855)
0c71f5496d98db778d673dc2b034451cb7e9a7f9 MGMT-6605 Create disks with WWN (#1819)
80ebb6273a1fd126d39de1cedd05eb120b37d57c MGMT-6550 Move SNO requiremets to versioned host requiremens configuration (#1818)
8d7a33e3ad8d5c4e24050a813d1175ba435ff2c8 NO-ISSUE Periodic GC log to debug (#1860)
c9d05292424005a4c16a2db82f0f8bc319222a62 Bug 1964591: Remove AI Agent image in case of service failure (#1836)
846f2dc89d10b74ed95cb99a6a8888902fb11497 MGMT-6653, Bump OCP versions 4.7 and 4.8 (#1831)
e5c131d1c307adf6afe9710e5e0b850415dbadae MGMT-6549 Remove HW_VALIDATOR_MIN_* references in template.yaml (#1827)
2bea4d65ed79b476bd8fb040cd0211ddae529db6 OCPBUGSM-29444 added comment to README about the 'Deploy Monitoring' target that is for devs use (#1856)
f5a57dc029e010df6aaf236797c800ab160d584e MGMT-6464 Deprecate default_ocp_version.json link (#1852)
6bda34bb1df401c42b6d8894681e92ee1ac975dd OCPBUGSM-29535 In case of timeout in preparing for installation add event (#1850)
6bbf952d3ea9b207e271223dee8b2ec97a77d170 MGMT-5422 AgentClusterInstall - Added LogsURL field (#1851)
d55b0d75c55ca175a8b57d3b1cf04fdb6df3553a MGMT-3560: Add support for multiple SSH keys in the ISO (#1510)
29adef27f3e796f8c7a4e0c7ef77e58a367f4c52 OCPBUGSM-29066 Remove cluster resources after clusterdeployment deletion (#1801)
53d74088d7976bb796c595a7b9ec69e0ffc429c1 OCPBUGSM-29655: Exporting the variable that supposed to hold the data. (#1849)
c57163cedcea235f34752f0f8e647aca99f104b0 OCPBUGSM-28683: Allow to signal when the Reconcile should return (#1678)
77260e41c79a7fcaf288efa6108bf1cea0c3a17e MGMT-6487 full ZTP installation code (#1832)
b4d6a5047a785c8a994ccc18c7c32e6e93fbdb97 OCPBUGSM-29645 Reset host validation mixes the parameters of cluster-id and host-id (#1848)
b8d2b08481e1d45d2ed89336d7bd08266112a89d Bug 1962957 - Check the response status code when downloading files (#1787)
c645e58e123ec62a8c1c49b6626ca9a52f1ec627 MGMT-6514 Set invoker for assisted operator (#1834)
8a939f06960b275775ea23c6167b9ff7e19ed4bd MGMT-5451 Document how to install on OpenStack (#1695)
4a9894def82bf353cc0c7f145c93aeb9880633de MGMT-5244: Only include 4.8+ in operator manifests (#1823)
66357483f48b09c067702d6bba0230fee41d6eea MGMT-6848 hyperthreading doc (#1843)
1401e62482d1c78459ec92081d4a8211e74138ca OCPBUGSM-29476 Trigger BMH's deprovision when the ISODownloadURL changes (#1808)
87c7fbc115db800f879ce2eed0cef12ea87efa19 MGMT-6457 Remove boot files download and upload (#1733)
98f662c53671b5588bcde8468cb7c0e94dcac576 MGMT-6552 Remove duplicate iso download endpoint (#1841)
bdac06c3f57bf9eef80beed1cdfa295ff28ad7ef OCPBUGSM-29619 map clusterdeployment to infraenv from all namespaces (#1840)
3c13d4e5680ddecdec1e4c3c0dfb926fbfe344c4 MGMT-5251: Print OpenshiftVersions data instead of memory address (#1839)
feb0071f5e8e4c63503ada14597c088fab477a37 MGMT-6650 Example CRDs update with clusterImageSet tag and SNO cluster name (#1837)
a883da053afb27546ba0f6dcf81ff9f31d46e0be Revert "MGMT-4627 Match version key to image repository (#1339)" (#1835)
80d9b5f6e69bdebeae8e1ed921a7956eb3b45235 NO-ISSUE Add logs on error in controllers (#1830)
701d70b9a77008b4de9e9553c543e4b1cd710754 MGMT-6609 Add name field to AgentMachinePool (#1829)
c91bf1b304ffbb309e599781426af41d59224484 MGMT-6005 conditions for ready and approved agents (#1782)
14863710440853f28c45f59b1ed2320bfad66aea MGMT-6497 Extend swagger to store route information in inventory (#1752)
9ffe453f7ccdd8506492ff95d042d02567f0f083 OCPBUGSM-27828 - do not output Status field to the BMH on bootstrap (#1833)
d7d1d76046a782f79a4515a823e04acd71933765 MGMT-6486 Add events URL to Agent DebugInfo (#1822)
888865cd92cc70e478ad6e249b59e0e067f52b1e MGMT-6634 Increase kubeAPI event channels size to 200 (#1816)
64472c3ec242367c66ffe74c123e8a5550f590c4 MGMT-4823 Remove spammy logs from the service (#1803)
ce6dbcdc18af4cf24cb91c3b1af6b18af21d7101 OCPBUGSM-27700 Fix NMstate requeue (#1696)
9103af060a340f1acd371f917cb848ddda1e9bf4 NO-ISSUE: Bumping ocm-sdk version. (#1826)
5d0ab50f6deb47f9985db722f56ff3bed8552896 NO-ISSUE Update GC times to 20d for deregister & 3d for delete (#1824)
01d2130465b26399a8e8599ccdcbd8f272b00cec NO-ISSUE - Add documentation on how to use the API to set the discovery ISO type (#1820)
a71e3e083bcdfbeb84b21caf6f2b11ccde447ad9 OCPBUGSM-29119 Can't change Installation disk - subsystem test (#1775)
e4dfae471bc68f1aa05368cc8e0bbddf5b97b156 MGMT-6483 Selective monitoring for cluster and hosts (#1754)
6c126481403fb03a14da27ed3fb79064867bf68e OCPBUGSM-28856: Increase the minimum disk size required for OCS from 5GB to 25GB (#1680)
443ebb797d25163ebf9c7112efa623da97b29be3 MGMT-5999 Add a flag to enable day2 in kubeapi (#1745)
cf99d1fca3fe29869a9245dc7b0b2400eaf11fc3 MGMT-6639 kubeAPI docs: CD and ACI cleanup (#1821)
f00aff7b113a97bc93e98a28f786775073cff1e1 NO-ISSUE add OCS team to code reviewers (#1828)
0a6dd66f345e6f27be33cd324f9550e356192f6d NO-ISSUE fix indentation issue in openshift yaml (#1825)
19d9e9339f2530a8d7e7fefff73c7a8a80ac439b NO-ISSUE Use a ClusterIP service rather than LoadBalancer (#1613)
79d0d395623c63654f7196df4735b42029293d8c NO-ISSUE KubeAPI docs: fix a broken link to agentClusterInstall-SNO (#1817)
c43ab4572f0d0ff1582a52463f3a0c502497c532 MGMT-5255 KubeAPI clear events URL when "installed" (#1815)
dd4b9e82d1b8707c03050646f1c29b85c1143cd4 NO-ISSUE: Adding subsystem-tests for telemeter manifest generation. (#1813)
4a3b6548ac7616a0edf8b75c4f6fe7f6489a9e8e MGMT-6633 set db connection pool (#1810)
bf6ad2ab22c4880907ee0db05e64bd69f436deb5 MGMT-6549 Removing support for min CPU and RAM env variables (#1779)
1a82a39964c63845605cbd4ecbc99963d011dcf9 MGMT-6547 Remove OCP version validation from OCS code (#1769)
0404f3865b9a30e1cfabaa0520ce05198e1168b1 MGMT-6455 KubeAPI Controllers Debuggability: Add Logger Fields (#1741)
69669e40206137ba2ecb9b80f8711ce8ff53ef24 MGMT-5255 Disable check for clearing events URL (#1812)
57a9a922259d9f25cccd3ce952e8c500185b8d6b OCPBUGSM-28872 Requirement Conditions for stopped state (#1802)
af46cb3ac88e5543c5c05b2eea0620927e4b0585 MGMT-6437: Redirecting cluster metrics to the correct Telemeter server. (#1773)
90de5696bec061a73e9c39ca0162525ef1a81183 MGMT-4758 use InfraEnv namespace to create the Agent (#1670)
3f6e0e264c2449faecc9e467a96993d678369283 MGMT-6531 agent conditions: check if approved (#1809)
77f2b96f5068ec867eee8bfb58e4ff27732055a3 MGMT-6562 Agent CRD Validated fails on pending-for-input (#1786)
92daefb8e32282735b148dc4d711a7ce69319c5b MGMT-4261 Agent CR and ACI cleanup when deleting CD (#1606)
7ed84e4e20aacb418ca09b2bfcc85dd45e52f126 MGMT-5255 KubeAPI Update event URL only once (#1804)
b5ff39d64d3f6ecbeba0312330477f1246b3f572 Revert "MGMT-6576 - Bump 4.8 OCP to fc.5 (#1791)" (#1805)
7060ae6a097301044681d4f81a70137760dac9ce MGMT-6584 Add host progress stages while waiting for control plane (#1797)
d7484ff0571b935f34ccfb4bfaffe63cdd766413 MGMT-6577 Production logs are spammed on "Failed to determine installation path" (#1796)
ae33443e7dcf5017dc6da14b54ef4de7a7e83a95 MGMT-6025 Enable day2 subsystem for kubeapi (#1800)
6bfc86be314a1d5714a5ab9c3d27b54afa1a6a12 MGMT-6410: Adding documentation for OCM integration. (#1795)
61ec9d87819933341d91346eef357c1c226f92c3 NO-ISSUE: upgrade operator-sdk binary (#1790)
93d6942134827fdea26de936526f6ef2b455ffdc MGMT-5274 Setup assisted operator ConfigMap (#1781)
916d2a2ed5ad7cf6609e3a9d54b866ea4f0a8634 MGMT-6413 fix  installer-deployment-overview configmap, (indentation issue) (#1771)
33b6ee0e3b87af02fcfa4402bbdd7b806a9207d6 MGMT-6022 - Hyperthreading support in AgentClusterInstall (#1783)
f46438444136d65086cfa7c61264452203843361 MGMT-5255 Add events URL to CRD (#1776)
76ec9d1b9abff8e7009365675d437f81604dd3e0 MGMT-6576 - Bump 4.8 OCP to fc.5 (#1791)
c1fcc80241094823f3bea9651d68880bc9c753d1 MGMT-4668: Generate OLM opeartor manifest to bootstrap ignition (#1609)
38f11f4d741acfff11db1d76a757b836f63bd4a8 NO-ISSUE: Fixing doc typos (#1784)
5950acaebb2e36aee273d530f9c78c56c113ac5c NO-ISSUE Extend BMAC documentation (#1772)
305e5a0518a5c3be2ddeb555e7c95201d94e0885 MGMT-4966 Mapping /run/media directory to the next_step agent (#1780)
a47e966fadf90a8b40f85c5359d7145df0b313eb NO-ISSUE Add note about Skipper to the operator build docs (#1768)
d13495329240c1fb99051ab0ccd30eb441826fde MGMT-6411 Discovery image deleted on cluster removal (#1720)
ac871fdfb3e50506e119c33bc0ddec2556f70a3f OCPBUGSM-29306 Allow creating SNO cluster with any 4.8.0-x version
aa245bfcb31782da259ec7536305422e038f2dcb MGMT-5274 Check nodes disks before attach/detach script (#1777)
90180311933a6ef9f2d08fc5014aa81560f42189 NO-ISSUE fix case of AgentCluster (#1761)
de21d1fed9f4730a61b8bbe690ee0af5400ac519 OCPBUGSM-29119 Can't change Installation disk (#1762)
b5f4d917a9d2a72f64675738ed84a41b60411095 MGMT-6284 install hive without OLM (#1698)
e105c66d9a3bd2c6573befae044bc6feb0648b03 NO-ISSUE: don't overwrite bundle metadata (#1766)
2eeea5e8a06b4572e0cf8c7c3d79b0ca1b481da6 Revert "MGMT-5430 Move assisted service image to stream8 (#1763)"
d12b068c02dc0e19b283f4cb71b3ab691516c91b MGMT-5430 Move assisted service image to stream8 (#1763)
7dac3fb956cc7c477cf79aa024ba4813ac85000e MGMT-6495 Parameterize OPENSHIFT_INSTALL_INVOKER (#1756)
a714f40bf720c30d8e491bdf54e847fb468c0654 NO-ISSUE kube-api: full format for release version (#1760)
a0ebf014d9fced061a9d6434eaa4100d5a173a86 MGMT-6473 - adding mirror registry documentation (#1759)
986a2030838e96e689d36d48da29cdc98a043cb3 OCPBUGSM-23667 - add validation for mac/nic uniqueness for static network (#1742)
6a9be30757f8b586345bf053655d0ae0674dd5bc NO-ISSUE make cnv subscription configurable (#1421)
be79cd3f63c2996bc82fdca54a86763ce487a11d MGMT-6063 Minor improvements to DHCP kernel arg (#1749)
5ca7722f6a1f7838dc5a7c613dc5c399f0df3fde BUG 1941606: add IMAGES_BY_DIGEST to generate-bundle (#1743)
9e1f1680a249925e9a020485d410c4507a816c09 NO-ISSUE: Add docs/enhancements directory (#1227)
f39d8d962348a04ab830579c2108e81bb116bafd OCPBUGSM-29303: fix crash on undefined pull-secret (#1755)
a16c1c153eecb6e668d69657629fbd5eb1c3d6b5 OCPBUGSM-28663 Create an iso download endpoint with .iso at the end - bz-1956421 (#1744)
a09c64feae8ac474a9cb5fb6ef2baef762b726e2 MGMT-6469 Delete Day1 only after the state is updated in CRD (#1753)
5cbfb1f8ce69415af7f67f07ae7f502aeb181419 MGMT-4658 Remove contents of Hosts field from payload (#1731)
6055d2f9e0e5be31dbffc65a107a596c9c3260f1 MGMT-6420 add owner reference to AgentClusterInstall (#1704)
7008e6bf06dde1c333c9959e77f8f507dbb290df MGMT-6413 Move dashboard under assisted-installer folder in Grafana (#1757)
dd25dfa8db383cae11ea9285cea2264f73de11f3 MGMT-6438 Remove references to unused env variables for hardware requirements (#1746)
28bff58124cb0da8b9fa80e1549bf49b41a921ab NO-ISSUE Remove kube job references and combine job types (#1737)
df3cd0b8e46ab338f346e0f0dbf9e038ce6ec615 MGMT-6282: Split openshift_cluster_id and status 'Active' update in AMS. (#1718)
578911c166e1b5785eaf12ea770405136851442a OCPBUGSM-26546 Validate length of base DNS domain (#1675)
86e955ab315e987e61e853375aeaf2f658a46d96 OCPBUGSM-29306 Allow creating SNO cluster with version 4.8.0-fc.X (#1748)
b5ae673a279353d0c76f7544ddef38c35f664d14 MGMT-4327 Remove old FIO tool from service after the new tool is in use (#1701)
51657071fb39d778d19c5f8d3cd68bfd31285ae5 MGMT-5430 use the nmstate RPM (#1585)
9214f6a1ceb44493c93709f96b82b689b2026b04 MGMT-4878 Add host validation for network latency (#1432)
f7f9b8090e4f4948643bbd01c22a07d6766025e7 NO- ISSUE Revert "MGMT-6451 Skip flaky subsystem kubeapi test deploy clusterDeployment with agent (#1714)" (#1750)
298592298ece31ef8134470a055c0cd484c63077 MGMT-6413 Add current deployment state dashboard (#1729)
49567c1c7d941313f03833a1759aadd345f8900f NO-ISSUE Add examples to the contributor guide (#1711)
ac62c8b49e1a2d5295a80a6c518fd51098e38e70 MGMT-6465 Move default_ocp_versions.json and default_public_container_registries.txt to data directory (#1713)
32486e60932efd02786824fa1742066851af26b5 NO-ISSUE: Bump operator to 0.0.4 (#1735)
1709a50d59bb8aba03713ade2f4869f86a43b8a3 MGMT-6456 fetch OpenshiftVersion from cache by ReleaseImage (#1719)
f7facf46a636c0fd5ae9fb38ef8e514b6b2b593f NO-ISSUE Add Elastic APM agent (#1707)
c7c243a52505e4f3a578f2ce3f8318da8acc48c6 NO-ISSUE Fix HW_VALIDATOR_REQUIREMENTS value for the operator deployment (#1736)
a2db71578907dfdf1795662a3bbf52af5202a571 OCPBUGSM-28708, OCPBUGSM-28573 Disable OCS installation on OCP 4.8 (#1734)
b1062a062e14f1bbfbb873ce0223488db47706b5 MGMT-5302 Restoring /host_requirements for e2e tests (#1732)
51cc786886b6a2db0f378ec9aece8793e0ddf1fb Bug 1957227: Allow overriding defaults via provided ConfigMap (#1699)
236bf216773f49eb49f264ffd5cb884995acf57a MGMT-6451 fixing flaky subsystem tests with bmh deployments (#1730)
4064240c62b102a24346575a9732d4af5bb1949e MGMT-5847 Move InstallConfig annotation to AgentClusterInstall CRD (#1648)
2c13627739e41ea85f69c371fa08508bbce9d82f MGMT-5399 Add support for conditions Failed Stopped (#1644)
271667eb988819be430e6cb13fc96593465dcbd8 MGMT-5412: Add OSImages to AgentServiceConfig API (#1592)
338b51c205609e3aaef6d335421bbf9fca5956ba NO-ISSUE Add documentation for overriding hardware requirements (#1728)
7acd467ff179b3912df7bafd7684e070ee5afcab MGMT-6438 Removed deprecated requirements env variables. (#1715)
0b6b6cf9fef664291faaa7caf4c6ddfcacec9f9a MGMT-6458 - Don't override hw master requirements with sno one (#1724)
60c9b8e6f013ec011c2505117ed1263a4adc7e30 MGMT-4942 Download rootfs from mirror.openshift.com (take 2) (#1697)
49683ef8749114c5aaac1944cb821edc6ccdea4d MGMT-5396 Remove unneeded yaml - rebase leftovers (#1716)
66be7eef365048c0b53ff4cf664367ee1990379f NO-ISSUE Add retry for any curl command (#1710)
f8129a325080306a09f2ce426764cdd1c8242ca2 MGMT-6001 Misleading status after prepare-for-install error (#1706)
707969546c75b8792355034a80941ff2a6b1ce85 MGMT-5415: Adding filter to GET /clusters API. (#1705)
d6af0506bfdcf0b189caaada53b3e94d02a89acb OCPBUGSM-28332 - Fix enable/disable host operations returns cluster resource with only enabled hosts list (#1702)
85257f61af2f8c2299d0b4be39d9f8ec22f15c86 MGMT-6451 Skip flaky subsystem kubeapi test deploy clusterDeployment with agent (#1714)
db5cf00dc8b154c747a6f5e0cb261dada718f69e MGMT-4261 Deregister Host on agent CR deletion (#1642)
3d3b762caf576bafd20a62d6e50824948e0cc238 NO-ISSUE add /etc/pki/tls/certs/ca-bundle.crt volume mount to skipper.yaml (#1712)
d3657fd59d41d5a9301bf96d2adea27974763a8d MGMT-5398 Update kubeapi docs for AgentClusterInstall (#1636)
45105c16a7c833f84132cad02c4940106cceebb0 MGMT-5302 Removing deprecated /host_requirements endpoint and related model (#1549)
0270af0fcce1e909138dc2fd96e919f0917c5b4d MGMT-5274 Destroy test assisted-service test catalogsource (#1708)
bf56f4a5a7fbf4ea5f9f7171e263ac1cf62f1207 OCPBUGSM-28705: replace MiB unit with GiB when ocs host requirement fails (#1667)
b99b31532f016280c19b52804f5a693cb696ec58 MGMT-5270 handle_ocp_versions: ignore default key (#1700)
9a7d3ab896aec432c207328ec28c96f59573abb2 MGMT-4640 set default OCP requirements (#1458)
133abc1b82477e9ece0ae8fee98fb58c3f24ec7d MGMT-6063 Define DHCP argument per NIC
e59435198292e944d0999a18f748b42f2baad3b4 MGMT-5396 Migrate to AgentClusterInstall CRD
7487e12585ff3819fb05d48ca4ef6bc92c7931fb MGMT-5243 - Bump 4.8 OCP to fc.3, along with 4.8 fc.3 rhcos (#1688)
cb8f56516e9b29b1904b9bcfea225faaa1e004cf MGMT-4134 Fixes to usage dashboard (#1694)
02dfcff43cc0f4e852476e115150472423a1f024 OCPBUGSM-28683 Stream file content upload (#1676)
bf9ad32739a0a97b1667e951007c971b5e865452 MGMT-4943 Watch the ClusterDeployment resource for BMH reconcile (#1617)
6eb500bcfaa3ef6e0665dba88ef27564a070daae NO-ISSUE Update and expand BMAC's documentation (#1608)
1e9a56ba4c76a165ec8925b2673b65f7be264802 MGMT-6422: generate operator OPENSHIFT_VERSIONS (#1693)
951ccaeb29cf8f8019d6b4eddede7266ca70cb14 MGMT-6281 mirror LSO packages to local registry (#1684)
f5959dd4936077e30fdfab7a6346ba8d96c3a73a Revert "MGMT-4966 Map the /run/media/iso directory to the next_step agent component (#1685)"
a652d78524723e9586dcb4ab9b1dcde9ec233f04 NO-ISSUE Fix apiVersion for AgentServiceConfig (#1692)
94f5703fab82cc93222bf77afa667f8a57708211 MGMT-6075 Implement ResetHostValidation API call (#1689)
5eb1f097dc4ef4b731b2d671e61a933a7028ee49 NO-ISSUE Fix incomplete Hive installation manifest (#1690)
b67b98aaaffb5eb5bd2308bf39607c8e00c39f70 MGMT-4477 adjust OCS preflight requirements (#1543)
70855d4fe011d2f84d336119e07ec1354cfa71fa MGMT-4966 Map the /run/media/iso directory to the next_step agent component (#1685)
176f21cab4cde3330fb142ac5c0e5b22e2fc618c MGMT-6067 Add a cache for the local authenticator (#1683)
4f07ab7ea86cdf723d04b9e8a70e30b8e0f627b4 OCPBUGSM-28017: Unify operator manifests and move them under config (#1557)
594bd1b6123b3ec7a4d769e05b513455d19fcb92 MGMT-6090 - fix erroneous mirror CA is set in the master ignition (#1682)
e7d8e406d85bf098b6a27a8d64cb1259ec1f6ce1 OCPBUGSM-28762 cd controller: trim ssh key before update (#1674)
1fce78c4dd59586d5b6ad37676a5a1fcdb53a754 NO-ISSUE allow GitHub-created reverts to be used (#1687)
f0b5937dc557e4ab38c9ace5efc19180c976ee3a Revert "MGMT-4942 Download rootfs from mirror.openshift.com (#1669)" (#1686)
683cfc08e98691c0e5669866fe4375c386d52526 MGMT-6028 host metric events subsystem tests (#1668)
f8d9f5a7553e4e05a862839f886dca69e3dbffad MGMT-4942 Download rootfs from mirror.openshift.com (#1669)
be800a7c26851770258f546054d1234c24b14963 NO-ISSUE Fix call to_url helper function (#1681)
3ac57e6caf1afb638f667c08e0f29e49c2aba433 OCPBUGSM-26820 Add database connection retry (#1673)
575df68975a5079238480b1fa5847088f545de8a MGMT-6010 kubeAPI subsystem tests should cleanup the pull-secret (#1647)
f4fc64b827be1213f7c98a9c4b207c0aaf1de32b MGMT-5348 cluster specific disk eligibility check (#1555)
2fe744720eb02a67885da41349aea35a5e05decf MGMT-5449 Provide Minimum HW requirements for SNO (#1665)
27c686862fe93b2b8d4ad3a194890f2c1bd2494d MGMT-5331 Subsystem test for filesystem usage metrics (#1659)
71ea698dab9e77d300c36c532f1fc23ee65a790d MGMT-5274 Make deploy operator scripts executable (#1666)
d42b8c859f82eb4938142dd0ca32d7357df435af MGMT-6034 fix enabing mirror registry certificate in Assisted Service pod (#1662)
16b6de6ad6cd3f0f232058b0b329ade5eda23fcc MGMT-4292 Re-enable image availability (#1645)
9278a97dfd5efcbb7fd6c23805fc291d8f32124a NO-ISSUE: Tests for agentserviceconfig_controller reconcile and (#1619)
43cb84208b7e3e891176ef78453810b247298007 MGMT-6023 kubeAPI subsystem test - wait for URLs (#1652)
20013eec04d2a998ed9713a312a0f7eb029fe5fc NO-ISSUE: Change the memory unit from GB to GiB for ocs (#1601)
5c0db398d66d0ad82a4a640779edc8e6ddc9a2db MGMT-4529 convert host and cluster metrics to ELK (#1560)
262e28709c491f58c2ddadd0dec24c9ce6b5e93d MGMT-6026 Update default OCP version 4.8.0-fc.0 -> 4.8.0-fc.2 (#1663)
1ba73150c4170ef74c0ed6c3ec8f2a9b2cae768d MGMT-5456 docs: hive integ - z-stream support (#1625)
39cad914f0f7514e999862486339f269d674a6d7 MGMT-5274 Order alphabetically operator env vars (#1660)
7e03c417acd6629a198782d9dac331933d6d66f3 MGMT-4736 Calculate SR-IOV NICs-related memory overhead (#1527)
9ed8cef5280586afa74aa996a521af5c3511ad84 MGMT-5390 Additional improvements to host monitoring (#1658)
d5906143413f5d5632082ba955e97aefcbe7e262 MGMT-6027 - documentation update for deploying via Operator with mirror configuration (#1654)
0599859fdfedaab16fb9a9e9ff8b4081267440dd NO-ISSUE Use correct validation ID for CNV host validation (#1623)
3fa886e6046e50496c38d3509b61cb97afa86386 NO-ISSUE support using a local registry (#1611)
e05f77a285fb3df77c2c91af43a24c317085d9c0 OCPBUGSM-27416 Handle AAAA DNS records in Route53 (#1538)
53e8a096a02ce6ba652d7977bd4e1e77dbd6ede0 NO-ISSUE Set release_version when overriding ocp image
620d9b0be76d935e1cb8342d51ff9808c5820e33 MGMT-5441 assisted-service should use oc client with ICSP support (#1655)
e16b630acca150931ffa0d305d368d2976ba5949 OCPBUGSM-27596 Update KubeAPI docs for nmstate (#1656)
924737701cc9d6547a474c0a241f7d17957eb2c7 NO-ISSUE Verify release_version as part of handle_ocp_versions.py script (#1653)
732ff1aabf3b3816f1b01d46393ddc03ae8a128e MGMT-4795 - operator should configure Assisted Service deployment to include mirror registries configuration (#1595)
b725f51b6801ef3075da6b5ca0ca2da241cc2bd8 MGMT-4849 Watch the InfraEnv resource for BMH reconcile (#1586)
c32581530b1887661e3cb5f7dc92b8dc5dcf1271 MGMT-6011 Add monitoring for duration and number of clusters/hosts for host/cluster monitors (#1646)
5abdef837e2f3b77756e1089cb74e0dd86d545e8 MGMT-5274 Adjust operator scripts for test-infra usage (#1643)
605a713c5a3414cd434152bfed808dbce50eb26a MGMT-6000 Updating versions to latest releases (#1635)
4b6e8814cc91ffa75c0fdf1c892489d7855ea897 OCPBUGSM-28382: Accept cm annotation on ASC (#1593)
1bc905585b9d7b2dee4728b1c7a26d95d5741191 MGMT-5390 Improve host monitoring performance (#1640)
3823630a0900c7f7a7113d7be4ff5a404a35186b MGMT-5419 Move disks creation code to assisted-service repo (#1620)
eef8f8f9f9b9375691a2e97a7171052fad26df91 MGMT-4356: Deploy only single openshift version (#1412)
ff88aad496daac299a761b703f7dad6f00b2dec7 OCPBUGSM-28168 update the ignition config run our service after the NetworkManager (#1630)
f3692b6ab7e088ab8bad1b4bc29d1f1026215df1 NO-ISSUE remove redundant call to upload files (#1626)
b391548c68aa89310eda20acd0ced20fe37d36f5 NO-ISSUE: Fixing OCM-Operations and Validations Grafana dashboard. (#1627)
92855ca765c8ffd07abc212d0acd94c4c632c723 Revert "MGMT-5441 assisted-service should use oc client with ICSP support (#1615)" (#1629)
169af55fcfe240ce08e4f7714f1a6106a6c89d58 MGMT-3512 Decrease verbosity of filesystem logs (#1589)
87496ec795087d46bbb106b88bce26e4e4000bc7 MGMT-5420 Always return 401 for local auth errors (#1622)
f45f38dc7eaae3ca509cf49c2c830fae60544b5c MGMT-5248 - add configuration of mirror registry and its CA to AI deployment (#1563)
926de34393b0dad4d606f153b5df30c40b4bf74d NO-ISSUE enable providing SERVICE_BASE_URL in operator's installation (#1618)
d0f1527569d494fb044519664c0e60dc042261eb NO-ISSUE Remove unnecessary mock controller from service config test (#1612)
8a88636a149efab5abfdc9ba1b599e64b3e82010 MGMT-5408 Warning if day 2 host is dual stack (#1621)
4dbccf5a573357dfa2055d03338815f5b195dcfa OCPBUGSM-28374,OCPBUGSM-28418,OCPBUGSM-28414: fix host requirements for ocs (#1596)
1540cc81725da243c9318837562200677df206b0 MGMT-5216 Add detached annotation to hub BMH before creating spoke BMH (#1552)
ba97a30c7fb69bcd19059342ceae5f2f97e5c5a7 MGMT-3700 Add dedicated subsystem tests for BMAC day0  (#1584)
6e82978d67663c05e232388463ee0d8dbba0b56d NO-ISSUE Check that CD PullSecretRef is not nil (#1616)
317f122ee4e78cfa98af2ad32403349261e4bccd MGMT-5441 assisted-service should use oc client with ICSP support (#1615)
b9a9708f9c5f10ad2b32fb7e3db890fa577eb946 MGMT-5408 Fix kernel arg for dhcp in none-platform (#1591)
bb47e03beb9fff41e0b9bf93a415d19a7ebd64ed MGMT-4741 Use the ingress cert to ensure trusted https connections (#1537)
5ddcfc1625de87be709c08f42bc83c73753962ca OCPBUGSM-24075 - fix events using English spelling canceled (#1610)
1c63392ebdbeabd41d4dd7e061aa058c4ae6bcaf MGMT-5359 Fix comments from recent PR (https://github.com/openshift/assisted-service/pull/1573) (#1594)
45be301ad9bc434e01dadebd0c7266df349d7176 Igal/mgmt 5323 allow adding costum manifests (#1567)
989d3b704bc9f2115eb5cf860601ab66743ef578 MGMT-5373 filter events by category (#1569)
7c6858801bf03f083e93df1bc4919fb9539ca33d OCPBUGSM-28289 - Assisted installer fails to allocate VIPs (#1602)
63e9996b1a7973798a2de92aae4df7c3981cff28 NO-ISSUE - Improve the docs example script for changing discovery ISO password (#1607)
09f2d7d9a2de4c1d496e408b22e37169eab028f0 NO-ISSUE: Adding debug info for failing validations subsystem tests. (#1605)
2ea0afa46b4107152f98d40b12d42efa02069021 OCPBUGSM-28353 Modified LSO Subscription manifest to use default channel (#1597)
a5b69eb813a09404a13cc380024816762b57b8bd Mgmt 4967 Create a standard way to run a debugger on the service (#1576)
969585a03de319aff80a5662800f6ca3a2ef64c1 MGMT-5362: Add CapabilityReview to OCM's cache. (#1574)
355ce62245a708e482e57809036fafed2c2144e2 MGMT-5372 added scripts for operator installation (#1568)
d10163ac70e0ccc10ec5de295db65a17b09978d8 OCPBUGSM-27380 Fix confusing host registration error (#1590)
a1689816f9b7810d3e6663515267f644abc2d0b1 MGMT-5174 Subsystem tests for epic MGMT-3563 (#1526)
99b248bd71488ebdbbdb69166a496f08283ba7c2 MGMT-5295 - Use AI configuration to configure DiscoveryISO and RHCOS with mirror registries (#1561)
4dad93a50b65f53d36f5aa883aab7b4a5c139692 MGMT-4186 use z-stream version for ClusterRegistered metric (#1588)
6c8d2aaef8599c4f4729cca4d6e016c7af2dfe2f OCPBUGSM-28006 Fix vxlan vmware incorrect checksum in assisted installer (#1580)
ff2a15b17ee262bfede94a90116852a3be1cabbf MGMT-5386: Fixing OCM-Operations Grafana dashboard. (#1583)
0d0f478724fe71db66ba3f20e218e577b5f6f7ab MGMT-3512 Skip garbage collection jobs in operator deployment (#1582)
1c6f3dccc0628e8ef5278b803c0af8bba845da30 NO-ISSUE: Docs update (#1575)
0474715b5bfc65fc5b16a425ec5bc81bdf55f492 NO-ISSUE Adds BMH detached annotation if Agent installation has started (#1540)
4c3c6dd07216e079ff95c62a9bdcd6b581fecf66 BZ-1937293: Disable container-image-availability host validation (#1554)
5513109631e79cea530a951971abb31a1e0b7e32 MGMT-4930  Add notifications from ClusterDeployment to InfravEnv (#1550)
d599757baf987e31b4f28695fea8c53fe5c416fd MGMT-4185 add release_version to default_ocp_versions (#1577)
8b419f64867cc968475942fd7cd99a310284db38 MGMT-4554 API for supporting a custom OCP version (#1319)
c1a701d7691d0e14e4728d8da55c3b34cd6b805b MGMT-5359 High CPU usage of Assisted-Service with 500 clusters and not hosts (#1573)
1052124277fc13f3e3c032a995b7fa62bd1aded3 NO-ISSUE OCP version update 4.7.7 -> 4.7.8 & rhcos update 4.7.0 -> 4.7.7 (#1578)
4780dc7e941c224a79d8ea8f1e6d5797cff2259b MGMT-5274 Allow override SERVICE_BASE_URL for test-infra port-forwarding (#1572)
0efa08d1741f14f4cb393e6cbac2c0e5901e1b94 NO-ISSUE Updated logging in release.go to reflect cases that `oc extract` required retry (#1571)
e4fbed2423e14bdd3be50e65af112a68732acd92 MGMT-4843 Update CD CR with api and console url (#1565)
43e811cdcb9b5f633ea44478656bedd7b5d830de Mgmt 4967 (#1548)
24e86c347e58a13dee939d8d348f4b91a2effc5e NO-ISSUE Refactor kubeapi sub test InfraEnv condition (#1570)
3b2f9472c81a7a6318e3840e5c58475113721ba0 NO-ISSUE fix some typos (#1566)
6b98bf164a7e765d30709f5bb2a346df6666b31a MGMT-5306 Handle dhcp karg in case of SNO (#1564)
e36e9475e7d752a96ccf12f1dc25b17f046fc963 MGMT-3879 Add ClusterDeployment Conditions (#1524)
f9dd444e20529ea1d642b1698b9ca4c19a25b912 NO-ISSUE remove dependency of common in s3wrapper (#1559)
68e69e9893874f7a9be0096c07296c295a4379e7 MGMT-4563 Skip host connection validation when host is installed or post rebooting (#1493)
f1f087f53301a543d77031b473f9616e99f664c6 MGMT-3879 Enhance kube api conditions docs (#1553)
5e053393579651c9ef9a11f5648d8ada32185456 MGMT-4444 Update SNO example with machinenetwork (#1562)
928765c75f141cfe05fa366ab4ca5a31ff79f13f MGMT-4463 Support IgnitionConfigOverrides in the Agent (#1502)
9385acfe05ade0450d7147fc5501a399ec072c62 MGMT-4494 Fixed unit tests.It is based on the work already done by Sudarshan here https://github.com/openshift/assisted-service/commit/7601896f469af6e186c5492df18105d4ae7c1aea (#1541)
951f02d9f5b4db91a118672fee8a2f7b37c6b698 NO-ISSUE set feature-usage to nil in old clusters (#1546)
782861ed732a8365a682b5808800fb8b23fcd2fe MGMT-4740 Encrypt traffic to assisted service (#1506)
d37ac44051be76e95676f33b8361c04eae290357 MGMT-4273 Create secret key to enable local AUTH_TYPE in operator (#1467)
897f4cd78a071393cde014e060366574a635546d OCPBUGSM-26846 Fix DHCP failing silently on reboot (#1420)
961906c4c288ea696ed069c101186c95da3126fd OCPBUGSM-28144 fix reconcile error of installed SNO cluster (#1551)
afa06da2391af5392d01ac09b0a50d0e7a98f310 MGMT-5324 Skip flaky subsystem kube-api test invalid namestate (#1544)
31329e72633ddc6c83729cec7f864e63b37d1a47 MGMT-4444 Enable machine cidr validators for single node (#1239)
210d1b47255dc3b72415cf563ba2999136ade3f6 MGMT-4526 - Extended Event API (#1532)
480208622cd30a77922f3c2ef1948780b241f312 MGMT-4557: Add Host Validation for OCS (#1456)
09e87befc06414db95ed33d2b54cbae701bddff6 NO-ISSUE - add kubectl to the build image (#1539)
ef4487249cc347f18027f2487367c1289b6fdae6 MGMT-5282: kubeapi: Added info log on reconcile entering (#1536)
2a0534ae18ce8526acc8f492ed76a859bf207638 MGMT-3512 Be more efficient with disk usage (#1443)
43fc60875a2a52f52ed635a9cb4226470e66c2f3 MGMT-4477 Preflight hardware requirements handler (#1515)
89e2797e57d0b77d4fafb151d40cf8fdb6aedd06 MGMT-3512 Report FS usage metrics (#1491)
fc2838bd830140fe6bba45dab2be43da6a8eb759 OCPBUGSM-17327 Handle asterisk in NoProxy values (#1409)
0349a5ce148949f27edd33e6ca5cb180df1d6a85 NO-ISSUE Set `online: true` and disable autoamted cleaning in the BMH resource (#1512)
69594371fa01cd67db43093542ee5f6fbd449134 MGMT-5288 Handle NOOP transition for host "preparation-successful" state (#1535)
d1873486e7c6a11656b190f35b6e5135925a9905 MGMT-5268 SetStatusCondition causes controllers reconcile endless loop (#1529)
1c3c775de2bb6d0c2eae74fe47cd324eeb06db8b MGMT-4914 BMAC sets IgnitionConfigOverride to agent (#1476)
ad13a763f109c191c63f8cab73fb1b76038c6c17 MGMT-5280 move installcfg package to use interface as an external API (#1534)
e368f8f5b4c33d0802f7256c6592c42269b564f0 MGMT-5266 Add API endpoint for resetting failed host validation (#1530)
64d01f6d69d4ab7c811025c7de7b1e2b338e516d MGMT-4965: Fixing OCM-Operations Grafana dashboard. (#1533)
9a2c09ea46159c0ec18af0140e461ac80d5d2345 OCPBUGSM-25356 Handle net prefix for single node (#1525)
9956a7902e8cf115e7329d6784b465c88c0c7bbc NO-ISSUE: Fixing validations dashboards name. (#1531)
e0a3942e849a1a594f9183700f0ef115e1d48285 MGMT-5265 Add the ability to disable host validations via configuration (#1528)
46149d3e3e58622b38e1ccce7c78643d9ee7a71e MGMT-4477 Pre-flight host requirements API (#1508)
a1e013fc51d0f6272c1b0ae386c0b1a67f701696 MGMT-5188 Deprecate UpdateClusterInstallProgress API (#1509)
2d6fdff6c769f8d79f108ecfd33e49827694023e MGMT-3443: Adding Grafana dashboards for validations metrics. (#1496)
5e7cc60663b4cc3e6aa2d0f19a5629fefdae1ffa OCPBUGSM-27929 - Make transition for cancel installation from known state not to fail (#1523)
7366b6251ac4592fa04e2bba96897cc94c60ba91 NO-ISSUE Replace gorm.IsRecordNotFoundError with errors.Is (#1521)
ea60bddf0d3c5cc7e1e736398879b934b34c4f42 OCPBUGSM-24075 - Correct the spelling of 'canceled' on canceled by user event (#1488)
984e7803bfdad084b5ea9387cc20959e92bae5f6 MGMT-4143 Usage API and metrics (#1361)
0ec56929f077cd512e4ef91e3a242ad20d3a7bd4 NO-ISSUE: Update doc: nmstate and agent conditions (#1507)
5a066026615a1b9c801eb2ffbce1513613c6e48c MGMT-5249 AI controller will install only OCP 4.8 (#1520)
82c8e57eba2ad00b8b665fae32dfa0ac4d2513f4 OCPBUGSM-26430 - fix dns resolution for bootstrap node configured with bond interface (#1516)
4d7751148e3035648e0701e9916aa247cf7882e5 OCPBUGSM-1948449: Update Standard Deployment RAM and CPU requirements (#1511)
054f70c32fb0505de21fe52438cb3df717226bb0 NO-ISSUE: Fix CLusterDeployment example (#1519)
aa5920b8a6cc15c97be478e241fc0b4ff435b4ae MGMT-5240 - Add recently released 4.8.0-fc.0 to the default versions JSON (#1518)
3da6af49c84f10d87cfafcf8c62ee821cf13826b MGMT-5176 - Fix support for disabling hyperthreading (#1500)
55bc6bf876425b9a5f1680af4f37767e2c043692 MGMT-4981: crds and dependencies for custom version support (#1492)
e8dc228514c36cc0e8d7b85d3ab09f08c070470c MGMT-5237 Update ocp version 4.7.6 -> 4.7.7 (#1517)
e78c2a16167c1ddf47391911f4b03e96e1286c01 OCPBUGSM-27640: localjob when storage=filesystem (#1505)
c2f46ea176bd29f66f94a8518e30f14a4e764e74 NO-ISSUE: Update docs for BMAC deployment (#1513)
7c2aa0421ea6e46178c3104bb5841825b2390dff MGMT-4921 Rename InstallEnv --> InfraEnv (#1485)
54baef6c24feb4e7f29d7cbd32739d3fc3bc8889 MGMT-4494: Create bmh in day2 cluster (#1424)
5f578feec1fb59871803dc6bc29080d74e9b18a5 NO-ISSUE Use logging instead of print in tools scripts (#1395)
d8e43d42dba1517b6994fb701eee9b5d19d90203 MGMT-4996 Bugfix Wrap REST error StatusNotFound when gorm record isn't found (#1498)
b1d97ea3fee06e5b72078c335e50b52d61e44fe7 NO-ISSUE making subsystem for ignition override less flaky (#1499)
11e32547a904a2ba49562b4b0ba3a63e09d50d81 MGMT-4711 Move to new installation initiation flow (#1464)
b5659ee1aed45406c9effe019b451bdf250f4607 MGMT-4467 Add conditions to Agent CRD (#1457)
a5a1eb6d27cd2bce87a55f76a4f0f767c25a8acc MGMT-4991 Allow the service to serve https traffic (#1495)
8880093ef5ce041d4c1951ffd5ea1096991ec3ee NO-ISSUE documents how to configure baremetal-operator to watch all namespaces (#1504)
5cb346d1914eef705c9fe9b0bac8e51386094285 OCPBUGSM-27612 - Fix typo in dnsmasq description (#1501)
d0a98b014073959e91dcd5915a92479e2af75b24 NO-ISSUE Remove error log when iso template versions is missing (#1497)
d54cb5e62f500e22ed3952ef8f4acd16a09b8a3d OCPBUGSM-26455 - Change misleading message indicates we can support more than 3 masters (#1487)
235d3df474d423157851ee9363cc9fb2b7c9e1fb NO-ISSUE improving doc for installer args override with crd flow (#1503)
bd4f980be7891a2c10c8da0389cd77759bc4c050 Igal/support installer args (#1494)
3beed1168bd165abc59c0568871707c6be452865 OCPBUGSM-27561 Updating the host get to wrong boot order event to contain the disk name in addition to the disk installation path (#1490)
913aba63aae8923400e8ff4e040c8cfc0d59897e MGMT-4638 Rename Group/Version to agent-install.openshift.io/v1beta1 (#1363)
26ba876ae143d2eabf2b61047a2f832f52baf9ec OCPBUGSM-27559 - fix pip install of the pycairo package. previously it was using --user flag, which during build cuases it to be installed as a root user package. When running in non-root container, it cannot be accessed by the executable started by a non-root user. (#1489)
659b5dab9f676d4bdc70675c20f0b2d1111929ce MGMT-4937 Events doc (#1484)
4a57d53684600660d7d577e2e74b2d7e112503fe MGMT-4955 Update OCP default version 4.7.5 -> 4.7.6 (#1483)
a81be5ab075267a95852dddc1fd6dee912d85a0a MGMT-4739: AgentServiceConfig controller cleanup (#1475)
b6c21875ef86bad2ea7c5bcf38eb95128d611799 NO-ISSUE Updated Minimal Deployment RAM Requirements to 57GB (#1477)
03c1282f95cd6f3de3fc84c7efc853de444821a6 MGMT-4704 - add CA and mirror registry to install-config. (#1433)
5d0580a34d9f32a3135dde39759c16e40e35a6cb MGMT-4363 mark the default ocp version (#1427)
1743a8b4c8a54e7d06764d53cfeb03e19b49f977 MGMT-4734 Adjust GPU data model (#1474)
e05c824dca3de8beb436843cf047018a98342e1d MGMT-4314 KubeAPI: InstallEnv support for nmstate config (#1316)
08a4b8b94ee1abf2dfc16582d6b279439ea45cc6 MGMT-4848 Return the newest agent in findAgent (#1471)
902a54d507dc4661d0ca2977114dc8500f52ee05 NO-ISSUE Pin k8s.io/api to v0.20.0 (#1482)
c1ee2606c6e4656206cdb19536733cc9443ebc42 MGMT-4929 Add Agent Approval event (#1472)
b764fe71248920344d49414825520152e2be8ce3 NO-ISSUE Publish susbsystem reports (#517)
ad8dd423c0d5de107a5915b847865f2f8cb94666 NO-ISSUE: Fixing update of console URL in OCM. (#1460)
00fa5a35ad936e120d8a398e09a827eff2891390 NO-ISSUE Replace envconfig prefix in-line string with a const (#1400)
834faecd31fbccaa9716ca020da405a2d13296f8 MGMT-4762 support head for iso download (#1430)
fc4cfa4c724a38a75f5d41e6c9f683acd5a84cb5 NO-ISSUE Increase operator resource limit/requests (#1473)
35f8de874c50871610310ad457c24017d583b6ec MGMT-4910 - set hyperthreading configuration to install-config based on cluster configuration (#1470)
a1b6109c4edd9cac5ccd9c33a9ad60593c286dae MGMT-4834 Reconcile on backend events (#1445)
6b0ef1946499e5beed48d2f562d0ce840ab21a11 MGMT-4909 - add hosts' hyperthreading configuration to create/update cluster API (#1462)
eb983e2b92936a03190c81077aa04e43945157e1 MGMT-4737: Add AgentServiceConfig controller (#1422)
0f2a31f93b162107f84441af0efcc6161c848837 NO-ISSUE Allow @pkliczewski's team to lgtm PRs (#1468)
ae9adf106926aed1cffd6224ac5108f3feeb97fa MGMT-4922 remove flaky call of updateAt while static (#1466)
82ffd2b9d344f89d336785b9cbb1d3a6c5021e7d MGMT-4733 Take supported GPUs memory overhead into account (#1418)
3259b5dff2d0889e48d2723a4359611ec2db7446 NO-ISSUE fix kubeAPI doc syntax highlighting (#1465)
e08fc9c230ad0cf4b2a149341ff0d961dad329a4 MGMT-4850 set InstallationDiskID based on RootDeviceHints (#1461)
07c7e8ab0483fe57b686a5868414cb616f65c5e6 MGMT-4523: Exposing ams_subscription_id field in API cluster model. (#1451)
5bc8d7ef053110bb3da7be9460284e930eb03b1e MGMT-4891 Validate hostNMConnections is not empty (#1455)
18664ae19d600e452848c6ea353d9f0b5094fe6c MGMT-4580 InstallEnv should only accept a single optional SSH key (#1438)
2f36f8a677d2b8d28d4ff1318de9513b28c822dd Mgmt 4801 - Use common GetHostFromDB in the server (#1453)
35cf3471a9f655a7fee5052aa72577cf518faa14 NO-ISSUE Remove skipper dependency from build_images.sh AppSRE script (#1454)
b6f67f34cb948a9a520e92be984025d78ddc4301 NO-ISSUE Fixed markdown Heading in Kube-API-examples.md (#1452)
a1d20aa3375fdcf05baf667d53b4d86be83434ef MGMT-4822 Skip un-needed cluster status update (#1423)
0d2c0170ff0ada57c7803246c0c961313baad860 NO-ISSUE Architecture document (#1444)
d7af0b3992665729ba4e7421f5a4b177f5ecb419 MGMT-4866 - remove code related to local day2 cluster flow (#1446)
731396c3b17a141c021e390a4bafdfdc8e39ecfb MGMT-4443: Adding console-url to AMS subscription. (#1358)
fbaa9d1c72e98dd6f4badfb5f6096bd0c9d23824 NO-ISSUE Remove minikube code and PROFILE variable (#1336)
97823f3cc6fc07a219f88c4922d3c5101d525796 NO-ISSUE - Jenkins slack message distinction between failure and user abort (#1435)
b5bdb320c77a509320a284e3b59033ea2656b8c8 NO-ISSUE Add an "about" section to the README (#1434)
dfec6b83424beea48bac5daaa4cb7c963c619479 Retry extracting the installer from the release image (#1439)
a6aa68d95abe053b0f2566dbecd77c87e1e59e21 MGMT-4543 Updating versions to latest releases (#1436)
255c478d7c2bddf9b41802bd36865850fa3eff54 OCPBUGSM-27173 Set operator status_updated_at field on operator status report (#1441)
0a86d5d4670e9e40ec00a72a36ab9a4dae6eeafa MGMT-4647 Remove HTTP409 event for GenerateClusterISOInternal (#1440)
7c90a40ce661ef882e97fc05e63ba11b540bc1ad MGMT-4587 Allow install-config overrides using annotations (#1417)
03523094ca3ec10fb97ec284a416a757750dcc28 OCPBUGSM-27182 Backward-compatible IsOperatorAvailable function (#1437)
bd083f15dd68b96316d6dbf54439187e53ed7ccf NO-ISSUE Extend Hive integration doc (#1429)
030f62fc3ac387c40060e4281e3a3c557264ba25 MGMT-3697: BareMetal Agent controller (#1279)
ed229bafb7d13350d0858a58dc72cc0fa51912cf MGMT-4640 Versioned OCP requirements (#1413)
b1f73ba306f40bcc4b27b066305ca2166b7049bc NO-ISSUE Remove APIVipDnsname handling from CRD (#1426)
dcbeb0a977903762d25ddf903639c3845afcdfc9 NO-ISSUE: Index build needs to use the publish tag of bundle image (#1428)
96a04f369230af2af24e3cb45009792db8f9746b MGMT-4715 Auto install Day 2 hosts in kube-api (#1404)
669010181cbf3fd45d71fa8701534276326fa658 NO-ISSUE Remove subsystem steps from Jenkins as they run on OpenShift CI instead (#1425)
abcdd8ac878da088aca62b326c488eaa469da2ec MGMT-4623 Publish index image for assisted service operator bundle (#1348)
a3e25dcffe5b317cdfd87431a25fd3adb59e8426 MGMT-4070 Capture network latency between hosts (#1376)
3f6af40f0b5fb621092f42544cc99c55ad43c3e1 NO-ISSUE Fix boot file upload race (#1419)
3d25caf63989c2b4a98ad5b3af6a676e79ed358b MGMT-3453 - Add support in requirement API to retrieve the value of installation_disk_speed_threshold_ms (#1370)
49de7f18c4411af163c19aa6ca8307217b7c37e2 OCPBUGSM-26495 Resetting a cluster removes user's created manifests (#1367)
1d34f4d9f607167d8faef08475c60a6dec469310 MGMT-4749 Add cluster id to logs on cluster create (#1414)
7725311bc8855171cde95210a3ec92459704dcaf MGMT-4703 - add CA and mirror registries configuration to the discovery image ignition (#1410)
fd1e93ec8b8614ac358241cac4761fd62128de00 MGMT-4663 Add host count for list cluster (#1357)
abe30f5143b741e1a6807a3d395432d9dd48030d MGMT-4773 Use local auth with kube-api subsystem tests (#1399)
e231612a06de5d6bb49d586729676f8474c7ba5d MGMT-4117 - add ssh keys to logs_sender container on bootstrap (#1340)
790c68adcee8c8e34af6708868121b649d0a2129 MGMT-4734 Add device identifiers that can be used to identify supported GPUs (#1403)
ce863c13aa64031b8dc2132e1fd5d57a55212bd9 NO-ISSUE Add skipper.env file (#1265)
fcf72643c19714e0cc2f052a3603c480300d416e NO-ISSUE Add the local auth secret to the operator bundle (#1405)
929ec81f06c92d149988f5cf96d908b5389b999e NO-ISSUE Add cluster and approved columns to Agent CRDs list (#1401)
954fabf7fc2c0334f7b369435d3de2f356268837 OCPBUGSM-26901 - Fix add_hosts_clusters endpoint returns host_networks and hosts as null (#1407)
51c393a002abecddb01bdd6970dc5adec7d8c5d7 MGMT-4049 & OCPBUGSM-22823 - Changing the disk identifier to be ID instead of path (sda) (#1314)
1ba0fa87e41e8e95ddbdf7ec3a00dc59c8610001 MGMT-4639 discovery ignition should be complete (#1355)
cda12e9a9f103a410512dd50e597d9d4484d1a99 MGMT-4422 Add log and events for customizations (#1406)
7ce86d9c8b14910397dce8234f7a828dc9a87fb4 MGMT-4237: Introduce AgentServiceConfig API (#1382)
bf03668c02ea90117700d3e5d470be2bae9def4d MGMT-4743 Assisted installer clusterDeployment uses same netmask to parse all networks (machine/service/cluster) (#1408)
5953df7b38064e59ee4f56049b2c9e86878f8ef8 MGMT-4630 Upload to filesystem S3 atomically (#1402)
29de006ac14fc31c5c17998632c95ecf5da541b0 MGMT-4733 provide host in Operator requirements API (#1396)
00f9529e8760959d8e35b38ba6972d18a07be4cb MGMT-4702 - add mirror registries configuration option to the discovery ISO image create params (#1383)
2fbf31d04dfc08f2c333ac21c3e51a4440ab9a7c MGMT-4509 Display memory units accordingly (#1294)
048556ec7445eb1a41051f2399225cb0550a34fb NO-ISSUE Render a file for the local secret (#1397)
a475385fcac1a6ec0319c6fc295ada5772174151 [BZ-1942521] Revert memory validation for host role to use physical instead of usable (#1398)
54379495aff6137526c2824e2f59c0d329c9fbc5 NO-ISSUE - Migrations unit tests database cleanup (#1394)
51105f8f8f34e6372e986422b563cf4a80181caa NO-ISSUE Update RBAC for controller (#1391)
8e7679c548e1b2f35974e2d9fbfe64bde59391cf MGMT-4760: Updating cluster.GetCredentials function. (#1384)
30b2883c28d888fe0f2e60167e1578e5eac9f04c MGMT-4673 Sort ValidationsOutput to prevent uneeded updates (#1373)
8143fbfe055d67e0cbc1c74c1ddb47f53177cb08 NO-ISSUE Update clusterDeployment CRD imageSetRef name to openshift-v4.8.0 (#1392)
6dc4044ffa6c95da7bb809f8c6265474d3f7396b NO-ISSUE Split Jenkins stages for REST and Kube APIs (#1386)
7db4bd0640e2f3637439e6a92938e7d387923d72 MGMT-4072: Remove coreos-installer dep (#1177)
e2a0806ebc450c68eb0efa6de4486c5e2659c7d1 MGMT-4358 Deploy the local secret when deploying the service (#1318)
9d91b6559d5ffa40ae354cb1fa2070a808a2da5e MGMT-4693 Make minimal iso boot with UEFI (#1372)
3cd57e6e7df6d377914ec09f2f484d712028e8d7 NO-ISSUE: Removing flaky test on cluster validations metrics. (#1390)
e0f9c4eb752afe9061eabbac11283e10ff9830c7 MGMT-4765 Bugfix Resolve OLM dependencies on cluster creation and update (#1388)
2f2a727ea957f446251db7fd5cda46b05cca2c70 NO-ISSUE Update CRD examples (#1387)
850db5669bbe0d1246db0be4ea28489ee3de0115 NO-ISSUE generate random db names for unit tests (#1380)
0000d7eec1a911ba267404d60f8ebc2c9bf76a6b NO-ISSUE: Add ocs operator unit test for standard deployment mode (#1320)
f57bd91bc9db25cd0db21ab395df600ffed21d33 MGMT-4734 Adding GPUs to inventory (#1374)
45c2d1b489f15ab12cf19229390245e45dacbd3d MGMT-4079 change subscription channel to stable (#1385)
29a017139b6b59cdae3ba7e9aee6e1ff7379ccb9 MGMT-4163 - Return error on update cluster when APIVipDNSName is set for day1 cluster (#1371)
8018c20a6f0286de356386a81208881c33c36c1d MGMT-4694 Adds KubeAPI CRD examples (#1381)
f9a6f57080dc965614d13034433028067f18ae5c NO-ISSUE Update QE grafana Perf dashboard (#1288)
4db0ab2a6eaae57ef74a37b5a8423ae9a0173ce3 OCPBUGSM-26879 Fixed indentation issues in OCS manifest generation along with unit-tests (#1379)
d610a3a0d201f86b660e4894fb75034adf5819c0 NO-ISSUE update hive version and clusterdeployment crd (#1378)
31d2d135d153874981d4f77f241d9ca2ae58ff97 MGMT-4742: Removing flaky subsytem-test on cluster validations metrics. (#1377)
8046155358e09db4444189c0b1dcd086e59afe5a MGMT-4626 - KubeApi create day2 cluster after cluster is installed (#1364)
061b21f59941c8dece456dc39d4e01ad801c8f6c MGMT-4531 Remove Get*RequirementFor* methods from the CNV Operator plugin (#1341)
075ec70efd1aced697e35fdb3a991e0079349b33 OCPBUGSM-26705: multi-version support fs client (#1343)
94f6b423708d11f07d3ba8f4a6afdacf84853c9f NO-ISSUE Fix subsystem image tests (#1375)
a8a132af8dce6d856d47969676bed786039b2939 MGMT-4425 Add presigned url authentication (#1347)
485d55be7aea9221f4dafdda14e43f7298aba691 OCPBUGSM-25994 Fix for unbalanced disks on  OCS StorageCluster (#1359)
b3636dde03e3776b58dde8d6cbcbe11647657940 NO-ISSUE Fixes in kubeAPI subsystem tests (#1368)
a71e7680248b600b6478d78b7c7d17273428407e MGMT-4531 cluster host requirements handler (#1329)
d8ce8ec53d9641be697f25b2f218f39b59c460d7 MGMT-3431 Bugfix pass CHECK_CLUSTER_VERSION value to other components (#1369)
fabfeccc3eb4b536e52063b329fb649817f5dca2 OCPBUGSM-26541 Verify file name does not include folder (#1365)
1746ce0a3786ffef33c330b9e639f9e0c81c87ee MGMT-3659,MGMT-3483: Generate metrics/event on cluster validations failure/changes. (#1198)
47af00a32c255cfa4a1d58f99edb7e5bb3c5578f MGMT-4568 Block IPv6 input when not supported (#1334)
6308541f16424912cc730e9b2e170179c38739d4 MGMT-4398 Handle post step reply changes for new tool in assisted service (#1354)
db2b7e0c1b14f51df3599b79cb7f88b1d8985487 NO-ISSUE Transfer assisted-installer-deployment repo under openshift-assisted org (#1353)
ba7b76276d98eb84a1a3fdf93154c07dd3cf6362 change single-node ocp release (#1349)
70ea7d35f5e5099a888c127981a032253a4b38c5 MGMT-4627 Match version key to image repository (#1339)
7eb0bfa656fdce30cd4048fe0c912bcc0306a5e7 MGMT-4386: Use latest available rhcos for onprem (#1338)
268bcc7bf5278aa4eb3fd7ef089ac997e6bfd306 NO-ISSUE: Add retries to Agent Update in kube-api (#1362)
609cfd8221f65bc08980e9bd23af4ea9f12971b2 MGMT-4644 Enable IPv6 support by default (#1350)
1d0ba083aa696ffa1b03260937afc7590aacde00 MGMT-4576 Check manifests content on creation (#1328)
6ce37db0a707d494266b64b9c2bbafe38b5c2e8a MGMT-4583: Refactor ocs code (#1308)
3f303c89a6cbdbf44178fa678005f354942e21d1 NO-ISSUE Update create manifests example (#1344)
73440529c68424ea318362ded9874042a9d2de8e No issue enable kube api for ci (#1331)
15cd03c7e548767786d9649f986730348b7e7321 NO-ISSUE: Fix typo in the documentation (#1351)
5f248570800f834047213b21e0c536e825772dc4 MGMT-4558 adding joined state for workers and bootstrap (#1346)
a498c33a7e89305ee42f31bae5d7495a53c8b453 NO-ISSUE: Add flaper87 to OWNERS_ALIASES (#1356)
5fcb7e4afe7967f585b1e618a4af9d71564556af NO-ISSUE Add retry to update agent in kube-api subsystem test (#1352)
3252844b4e6379c28ee6bc7e550076955a5dc379 MGMT-4300 Deregister inactive cluster (#1248)
f1fe0aa81503917899fb9c3aff12e9824f59a119 MGMT-4205 Wait for OLM operators to finish cluster installation (#1337)
29e74e7c7af6c2a65c8d99f90b2a5a2950058a4e NO-ISSUE Agent Reconcile need to create empty array for inventory (#1345)
467f5df8252e190c7b156dc31337a60bd45f62ce NO-ISSUE Fix Secret create role (#1342)
1434a2dc58134c776b5ba5eb46f6a59d8c115081 MGMT-4628 InstallEnv ignitionConfigOverride should be optional (#1335)
d44545f4bfec2fbf74f217dc5bee97b24bd388f8 MGMT-4217: subsystem: run kube-api tests after rest-api tests (#1191)
450a2239c98ae5fdd8cd20d0a0bba6bc759921f7 NO-ISSUE Agent Reconcile do not update if installation disk is empty (#1333)
ac59176add3f1a5f89fe47e1df021d9c9ab7589c MGMT-4205 Add degraded cluster status info (#1327)
e400a0e43bc9f979e48809c8b5cc02262ee4c9eb MGMT-4234 Update ClusterDeployment CR MetaData (#1303)
29f9831ca4e4a007cf5ebea83b11e063b237efa4 MGMT-4312 Remove scality from operator deployment (#1270)
c958b909c9c6e74ba6c7c7db9c7e61b8a93f6257 MGMT-4210 Refactor ignition code (#1242)
668e7c9226b79856fc6f0c7f8b64965e70588bf8 MGMT-4420 Make dnsmasq manifest for sno optional by os env (#1237)
3bcaca8abef5173b0e2175b5d0b722e851e39cee MGMT-4517 Update static network config in  RESTful API user guide (#1325)
ce0ea5ed742e623574c971b4ee1e10553c99d3a4 NO-ISSUE Update ocp-metal-ui proxy-pass URI with service route URI (#1321)
f3bc0422761ec94c96fb0d0c55d14676e3ea69b3 MGMT-4480 Get must-gather image from release (#1322)
e0df002062f80149769707e72e5952da16897aef NO-ISSUE Add icon, additional metadata and annotations to operator CSV (#1326)
bf0d68c9650e2ab5ede1c099a92219868cd0057f MGMT-4531 change ram_mib to ram_gib in cluster-host-requirements-details (#1315)
eb2fecd49c994f190fa58842b6bb8f840867390f OCPBUGSM-26476 Set portable to false for StorageCluster CR (#1323)
bf120e7c49ae7500d23e964bb472e941e3d6d753 MGMT-444601 Verify CPU virtualization flag for CNV (#1295)
95c7311363160c1f92377978a87bdc3a0281e589 NO-ISSUE Download specific version of operator-sdk, turn on publish (#1312)
1958784db1d5922a6b2d7477b536a12bdecc433e NO-ISSUE - Operator SDK should have a pinned version to make sure the environment is consistent across dev machines (#1317)
731c25c14717a8c6279b873f49344f3237547257 MGMT-4513: Don't do anything if we update host with unchanged info. (#1302)
b30460b30aa6f7fe25b736ef7e969465e0f792d6 MGMT-4079 Check whether inventory available (#1301)
ea463fe84d8fd795ea108efeebc1b22760295c90 NO-ISSUE: AUTH_TYPE missing in onprem and liveiso configurations (#1306)
e864cc856c7c9faba26a2411018ae1c683b85841 NO-ISSUE moving conversion helpers to separate package (#1297)
8d29b4ea2fb80fbf6be058bff2b62434cc312658 OCPBUGSM-26398 Fix OCS and CNV manifests indentation issue (#1311)
dc2f655b6aebece397962e55012ec9b37665b441 MGMT-4205 Cluster completes on monitored operators status (#1276)
4d227544d0fa9dd08f0f44f4c83cb8f3e295ca25 NO-ISSUE - attempt to logout from problematic registries before running CI
22c7915c629659059941abcc7a2707e57963286c MGMT-4490 Cluster-dependent host requirements API definition (#1278)
8ea5db7cb88596de36c9921511ff76fb0c37f803 MGMT-3550 Add flag to disable IPv6 (#1250)
3e7dcf0c735e5a8e8b27839bd9051f3609306aed MGMT-3109 increase timeout for cluster logs when logs requested (#1307)
a93b5bab755f720baea0522dc27cef3a6b460fdc NO-ISSUE - Remove erezalster from OWNERS (#1299)
2f24eac790726cec10a6a664e857982a74453b1b NO-ISSUE: Move tests for ocs into ocs package (#1296)
62f6a12f9790dff75397c65cfd652215ab83a088 OCPBUGSM-25786: Fixed pull secret validation message (#1305)
97870855c454fd8094dc01607c956bb7176124eb MGMT-3811 KubeAPI Minimal ISO support (#1256)
82fa8faedb66fc572b34c20ce76d2c8f8ef71285 NO-ISSUE: use swagger-codegen-cli from quay.io instead of docker hub (#1304)
bed493098c712a9bafe627cda1e1ec52e35a65d1 MGMT-4501 - Remove unnecessary steps from Dockerfile (#1284)
a612109d98d1a676856a60fd7acfe6dd1408e4ea MGMT-4413 Updating versions to latest releases (#1289)
084723e740441ad8ecac0c2031a93558c97c5d05 MGMT-4502 - Improve unit test performance by putting DB data in RAM rather than disk (#1298)
64233f6b64218eb330cc0214f97c8d5089e45885 NO-ISSUE Revert PR#1285 adding operator-bundle to build-all and publish (#1290)
b8fd8b61bb294e86c9715bdf760f11220611356e NO-ISSUE Add customizations doc (#1268)
59de40f1b35dc87048df558933d2eabb9ef8838a MGMT-4382 Sets minimal-iso as the default for operator and updates docs (#1277)
98cdd8e40907625ed0a918856b8a86e0c77606b2 OCPBUGSM-25828 Use ubi for assisted-service init container (#1287)
229c20817d1f429ce3b17ce2f6a16bb9854a1223 MGMT-4274 Remove ENABLE_AUTH (#1263)
e5546584aa72f86dc9cfde58eed2546d99493963 MGMT-4448: Updating host validations metrics test. (#1293)
7623d78759009f4a00e43d09ecb605e7b31f6c1d MGMT-4450 Operator bundle should not include experimental ISOs (#1271)
da684325f45b6a050fe69e1a8963ff889e611c07 MGMT-4204 Return subscription data in monitor operators (#1283)
9af038b12538bae6c83c0e0f86bf17127f457586 NO-ISSUE: Document the need for a scality PVC (#1252)
df6988c73f2f3a888fc199eec84d1fd3940d131e MGMT-4518 - add mac address format validation for static network config API (#1291)
6c62380b24e7044b50e91f36302573496f915231 MGMT-4461 Use mac-interface mapping alongside the nmstate yamls (#1274)
3b0e77e1ed5f7559ab1d0793ed9b23f8cc766aed MGMT-4471 Generate an agent auth token for local auth (#1269)
9d92a37f2dfa009f86e1dfeddea8006c66c7b5f3 MGMT-4219: auto assign machine cidr from cluster monitor (#1162)
b907fe64df8167dd8b7b7d3741b0968182837add MGMT-4460 - update REST API to support new format for static network config (#1267)
709ddcfd8921a44980c780192f4815fdb6a88546 MGMT-4066 Add enabled OLM operator CPU and memory requirements to host validation (#1167)
f30d42d8d76f66bec73f9e830b8f0b27996eb2b5 MGMT-4428 Adds operator-bundle to build-all and publish (#1285)
ecfba837e6075a4b047e6e4d0379d9a2d96d5012 NO-ISSUE: remove bundle from publish (#1281)
a17727b781808d5ed35ce3293acb9c360f895534 MGMT-4442: Added cluster name to OCM subscription. (#1273)
e9d80468e4df9528dec6e00bf0ecc18ca0b2d380 MGMT-3541 support ignition override in kube API (#1241)
d07b813b121a5e012d6017eb69a1632b80bdb99e MGMT-4428 Create Dockerfile to build bundle image in prow (#1230)
c50b6b9ce424f8c3931412aa6dbcaef47db465ac MGMT-4275 Add local JWT authentication (#1228)
31aa5859b9a1d0b58bfee2bb978c734f5921ba14 MGMT-3667 fix Logging image to best scenario output (#1192)
8bb1445f29971a796d2981231f9d4a9632224c9b MGMT-4188 Use manifest API to manage operator ignition files (#1264)
a5b6e4f41ac39a431989b22183fe62c6bcbe7e2b MGMT-4483 Add InstallationDiskPath to Agent CRD (#1275)
f60ae14adc85af9b0847417644e2b976b5f17beb MGMT-4204 Rename prefix_name to subscription_name (#1266)
a14e4d7fdfa198665ef17484a4584cc062584d6f MGMT-4423 Add Host inventory to Agent Status (#1272)
6299abc084c67a9cf0d08e4bcf085a8439ad4c97 OCPBUGSM-25057 added image type to events (#1258)
37982a5723ad6011a1695c2048205468ea995e5a MGMT-4430 Fix for flaky subsystem tests (#1257)
806f747006607e5b1169a368783e9b2feb785a04 KNIDEPLOY-4234 Add option for s3 client to use local filesystem (#1129)
2e48cadee4c7f6d6f3e596aad34c0a9715956b66 MGMT-4366 compress custom ramdisk archive (#1260)
a6c2ab87d50669e626fd0500dc0d836d1d512ecd OCPBUGSM-1936338 Fixed the total disks to be used while generating OCS manifests. (#1259)
bf01e736cf8a8dd0003c7d5337fcdf7560d5a83b NO-ISSUE set MinWorkersNeededForInstallation to 2 (#1255)
78803bf31d071c9f53b2c2047b3f961a337cc1d8 MGMT-4274 Make ENABLE_AUTH optional in the openshift template (#1254)
54a71d95ae16b71477a3cce6d1539c83cf90a979 MGMT-4468 update cluster from installenv (#1253)
acfb688a2cabde1ae885bcff1a309c68ca445b67 MGMT-4430 ListOfClusterOperators and ReportMonitoredOperatorStatus operations (#1245)
a6941a4115ac0ddc9dcfb8800b18e607dba7d4ac MGMT-4365 validation for custom ramdisk size (#1251)
9c3609bc4336bb99d2888e7bc6c8f5a49316893b MGMT-4447 SNO - if machine cidr was not set, route53 fails (#1246)
dfc03a6c155ba27070874850d5942c26c5a52d7a MGMT-3697 Fix typo in the role verb /patc/patch (#1209)
6017a4713eeb3296ea0d350dc4766810f03d5f00 MGMT-4385 ClusterDeployment controller start install only if hosts approved (#1235)
5c64d7b843e9d024826d172cfd02545b8a889813 OCPBUGSM-1934562 Added the validation to consider OCS disk of size >=5 GB (#1243)
164865da6f9f21551a137f8a35b333cecd0bccca MGMT-4414: Adding DB update for each change in validations status. (#1234)
efe87086001509d60f0a4ced00fa85b082619597 NO-ISSUE update OLM plugin dev documentation; simplify monitored operators (#1219)
41076d3c46b945ebcb74c5600991e1e977e004c9 OCPBUGSM-1934722 Included the size unit in validation message (#1244)
b7b19b0d2696c8eb71b6774b2e83cadf8d6df42e MGMT-3998 Get installEnv params when creating or updating cluster (#1170)
4d079a4bc716c1e4317aa17c804f12ce93436088 MGMT-4415 Remove cluster_ID from validations metrics (#1238)
e1993f0f16f224b1b9214539ed3f05f2d4444996 MGMT-4079 CNV update (#1229)
225a4fe062a481fb26c5b4517d944637c30b38f0 MGMT-3854 log info impl (#1180)
0e7803337105e35ecd6001caffe842700ffbd969 MGMT-4049 Add id information to the inventory disk (#1225)
d41508fc3c2240e535fa05599b77a14a554ba5bd MGMT-4123 Allow the user to provide the machine cider of the cluster API IP (#1121)
62c73733330e1807fa1bac330a451c666a7844cc MGMT-4424 - vaidate the interface name parameter format in case of static network configuration of HW interface (#1233)
fc9984ebe051c2c60b7850aa72b0d4e438ba693c MGMT-4079 Deploy cnv (#1176)
5637efa4116db08151d5cf44671a48b4ef962298 MGMT-3979: Embed ignition and ramdisk into cluster iso (#1151)
6aaa8f67ffb82c9be4033a9bf20beaba88006ac7 MGMT-4274 Make AUTH_TYPE optional (#1226)
cc44cb6f76ef4810b9765408ee5cd2860f2bb357 MGMT-4170 - Add --skip-existing flag (#1224)
384aae73beec2286b8132fcf59318a22c4365672 MGMT-4348 move cluster-deployment crd from internal (#1217)
5f67627c0c836b21cdb81fd98b64b09bcf495fdd MGMT-4165 handle minimal iso templates update (#1208)
28161b09903d9c1877a365f50489c5eefee03d36 NO-ISSUE Remove unneeded fields from Agent CRD (#1220)
4a927656ef7ac7e860fd1223c3969760fbfea853 MGMT-4274 Allow for additional authenticator types (#1201)
47b03ddff8907487f1b58373f8c561d8301a0deb NO-ISSUE the build failed on MAC by a weird networking behavior (Docker desktop) - please see the long comment in skipper-mac file (#1221)
e7b15d761f9691e2c60d14fd13d87c225ba3eac5 MGMT-4318 Dns manifests for self managed dns for single node (#1182)
927f8bbdf395e2ee830749eb672283d1089396b8 MGMT-4339 Add indication for discovery image generation (#1206)
ba91bad8f1932eb4d1fa1bdc216f95500788df05 MGMT-4065 /supported-operators handler (#1197)
70dfd4606447324189a1f01d500b2ea5057ad694 NO-ISSUE - Support make build without the skipper on MAC (#1196)
c1788d95393e0fb0f195fbdf7868f2d3ff54b0fe MGMT-4170 - Create assisted service python client as a library , make generate-python-client now creates python package (#1168)
0e882fdaedf7069eed4e748049df051a6860899e OCPBUGSM-25682 - set image type to full-iso during cluster ISO generation in case it was not set by user (#1212)
d8c9bd8ea0efa610b0d71972010b67caaa1cedd7 OCPBUGSM-25741 Fix for bad validation message when total disks on the cluster inst multiple of 3 (#1215)
b307df44fbfee4eed760e3be468dd1b5a27244a4 NO-ISSUE update hive version to master (#1211)
e02fed26635ce005fd7dcec98f5426f5fd9cbd01 NO-ISSUE Performance grafana dashboard (#1207)
247de06c92375c249aa374aff19e361faa617dcf NO-ISSUE Delete assisted-service pod before deploy-test (#1210)
d2a13e1c9799b0e683cc2d3db3b486ac049a6712 MGMT-4204 Implement generic operators API (#1094)
9ef20b79c07cf028d21193587aafda065f4ccda7 MGMT-3371 Documentation on adding support for a new OLM operator (#1205)
394c41250d839240d315135ad7bb62e1ec74eaa4 MGMT-4259 Add Approved field to host/agent (#1183)
a74318d074be9643eceb2d36fa61d49856db2185 MGMT-4315 Api changes and code generation for additional state for checking disk performance (#1172)
b358efd55639da29fd23e70cd8381772cb08a045 MGMT-4095 - update minimal iso flow to work with nmstate static network configuration (#1178)
6b56b6707c4d5b43e024a56a5827a231632ec531 NO-ISSUE Organize common db functions (#1200)
0edec75edffd36b5402a151b6aa789fdf07bcce7 MGMT-3854 log progress new API (#1199)
97753cfd953da1e1d157453afe85178f4b6d51e6 MGMT-4345 Removed setOperatorStatus from OCS validations code (#1194)
58145a52620acc36a89dba98076d098441ce5ed0 OCPBUGSM-25000 Unclear error message when saving wrong service CIDR (#1195)
e140902bca3a4630400a4d430228f94c62dc6998 MGMT-4361 Postgres init container should not hardcode namespace (#1193)
8f947b853e8be1554ad8b3912d27802781803e38 MGMT-4052 - Add disk by-id info to inventory - Adding by-id field to the disk model (#1186)
c40843e8384e5e20e1e0e203747fa76cdb9a4263 MGMT-4343 Document how to set static network config with curl (#1190)
6fd80659c71da466a167da9b7db67ca5b444a186 MGMT-3854 convert log info on cluster to ref (#1184)
1478f67a797f5413eccf04491517cb9840c15c7d MGMT-3982 Store initrd metadata in system area (#1171)
75540b2d2bafcf83780f95ba1266ea14739abb32 MGMT-4347 Fix pull secret format to dockerconfigjson (#1185)
f73f3d5e40299f268d991a7aef46702af2036653 NO-ISSUE Add docker ignore (#1188)
d2945485c000062515bd7ae5c70abb763e958b13 MGMT-3865 Block VIP DHCP allocation with IPv6 (#1152)
a1290a566fabdaf16d83a636e9210d5e66723bcc NO-ISSUE add skipper mac file (#1116)
4ae4764c49fc054b2c87bb2c199e0eeec495c62a MGMT-3976: Embed ramdisk placeholder in template (#1150)
cdd3806e2b8d3e0195e7588135992e56ab441c3a MGMT-4281 Updating versions to latest releases (#1160)
10bd870d5a010c119b3293d2c0f9294760ade8ff MGMT-3854 log info API (#1148)
6b21007a7474307ebcca270a378e4785c407814d MGMT-3598: clusterdeployments_controller.go: Update host prefix only if > 0 (#1169)
23d0a32ac173439d75f16d30067e52dd08b58aa1 MGMT-4090 Use nmconnection settings relevant to current host (#1138)
bd190cc6e47c0065d58c3563d6de33111f74656d Igal/mgmt 4325 (#1175)
854f1c49e3eeafffd0d33f9df403884d7d2f6a3c MGMT-3360 Agent controller spec reconcile (#1164)
23cc1d598f1602c29dacf5eec0fc8a7a1987d8f3 MGMT-3371 Introducing generic OLM operator API and migrating OLM+LSO. (#1140)
1cfae5cd9ad2f41419a18abccabb972110cae3d7 MGMT-4323 - fix the nmstate lib installation in Assisted-Service container (#1174)
8fc0918fae08b8de12174fbe4e9ca0688210536a MGMT-4282 InstallEnv ctrl to update installEnv status in all error cases (#1161)
94c666f95a6593a607e459597bef04ec7e7da733 OCPBUGSM-1931840 Removed channel from Subscription manifest to allow OCS to install latest version (#1166)
f1d6ca21ed062d1d90b085c399a615daa8779f28 MGMT-3856 - Fix weird domain resolution auto-generated swagger name (#1157)
98282aeb19b8361d0733ac64767f6135b40a5b61 OCPBUGSM-1928868 add ocs validation for autoassign (#1139)
9abdf4cf5a8f8586fa3a4567ad1192f9d1800d63 MGMT-4297 Nuke Image and Cluster CRDs and Controllers (#1112)
ef9e854a1ceb54318e93141ba365e9e0770302e4 KNIDEPLOY-4151 Operator deploys the assisted installer  (#1073)
cfd55e06f3f19a0d1da14cf41e5f19be74460690 MGMT-4295 Verify that a host is valid to be master not only if it is in known state (#1165)
c88304e5aaf70e023bac9ba3e4bca46167c9d733 MGMT-4089 - create nm connection file in discovery ISO using nmstatectl (#1143)
48a01839c1555a8282e7ed5d052ecfdb2d40d561 OCPBUGSM-25447 Disable image availability (#1163)
01afeb5e832316322d7239dfdbc2856e8ca1d664 NO-ISSUE Organize DB preloads with common functions (#1158)
40846415a31fb6f8799e124a706ce2c70aeaaa7e MGMT-3667 Print git_revision label for every image on deployment (#1137)
b32b6289d1fcd0d0d3f4e44ba57efc7cbaad5fed NO-ISSUE Call build-minimal when using deploy-test (#1155)
6adf01fe23a84523562ea813470f3aecb5438f53 NO-ISSUE Log each time uploading a new file using S3 (#1156)
7eb0985891c4d702464ea492b02cdbdc474c11c4 OCPBUGSM-25360 Create of SNO Cluster will set vip_dhcp_allocation to false (#1154)
cdb72892a7ea5c9be6c740d2f0895f2ce546cce4 MGMT-4242 Install Config edit fails for single node clusters (#1153)
d6a877ccda8580587c9850ede85b5400156daaa6 NO-ISSUE Fix typos (#1119)
0372c7aeb81112b92f2c59ee9b2c5e8abfa4170a NO-ISSUE: Fixing a typo in OCM Delete subscription logs. (#1144)
5728b6fe12ee6f3f3ac69a57287457d9c68a9108 OCPBUGSM-1927631 Modified the ocs validations to use all HDD or SSD driveType disks except installation disk (#1128)
1d46d080152598d42668a4716441ff3ccb00f6b6 MGMT-4182 - Add 4.8 sno to OPENSHIFT_VERSIONS in test deployments (#1120)
d60432e3a4b392e92f22b15f725732ba632e0eb7 NO-ISSUE: Adding WITH_AMS_SUBSCRIPTIONS to deployment template. (#1145)
122a453e19a6479a64223c63555ccf2e1df75934 MGMT-3970 Make the iso editor scratch space base dir configurable (#1063)
32abc2f211a3ec31a40dfc73e22f852e8d69a9a0 MGMT-4191 Clean up ignition package naming (#1124)
f388657436085b1f4032de4a87337ce37dc4d39f NO-ISSUE Fix bminventory unit test with AMS mock (#1141)
b41e2b6afd655251674fbf277505e05e0c115949 MGMT-4088 (#1097)
2ce170b7153a5a50267c1e6d2e93fac44738f0f7 OCPBUGSM-1927459 Added ValidationPending Status when host inventory is empty (#1118)
8d81d01fe6d8672e59ffcc5e3733d58154009df4 OCPBUGSM-22593 Validate SSH key when generating cluster ISO (#1136)
bd0a2170249c8f3dfcdc4258f13a7ec12b1aa632 NO-ISSUE Organize bminventory test mocks (#1134)
02fc8a3c0010ca3bc7c1c2e945afb2652ccd53d6 MGMT-4211 - Single node clusters will now use default master role for hosts (#1133)
63df040cd08f4688132d87a8617fd952ccac3f0c MGMT-4161 Updating OCP version to 4.7.0-rc.2 (#1110)
cd59b9ebf4882c83533a80381ad7eeb2d198ffc2 MGMT-3918 InstallEnv controller (#1029)
d83477ce6d66fef7ac608efc0acf431a5a9f6ec1 MGMT-4017 Create agent CR on Register Host (#1065)
c378e15dd699b3604a0a39b803e049b7446b96a5 OCPBUGSM-1928474 Fix for memory validation, when using additional disks (#1105)
445721969c3f307ce20f1ee817b8a0c0e66736ae NO-ISSUE add target to deploy-resources (#1130)
8f5dccd41f770910221025f3d13c8ed3a358136d MGMT-4087 - add REST API for static network configuration (#1096)
f6e502ea29e461cf10bea76a42da37b2fb494c96 MGMT-4168 SNO cluster will be created automatically with OCP 4.8 (#1127)
3fded7a5546d7dc5ad2375d6056fe2d51874faf9 MGMT-3371 Move all additional operator-related code to dedicated package (#1074)
148a58243d8cfc84344bacaf415c68418ec82845 NO-ISSUE Log format fixes (#1125)
2075a7fbfd8a2dea49500ef6b3c7fc111eaeb6d7 MGMT-4190 Fix bootstrap in place master ignition version to match the bootstrap ignition version (#1123)
5a5967b7986826651e9220a77db10e96d0af4eb8 MGMT-4181 Generate service image URL for non S3 enabled deployments (#1111)
411f92d0d1afcf40818b9dd7763d384308236102 MGMT-4180 - add HostStageStartWaitingForControlPlane to dissconnection validation (#1117)
cbb4544f048723eb6b169735ebcc63c50b1530aa OCPBUGSM-24964 Change sufficient masters validation to include insufficient, pending-for-input an known statuses (#1114)
f1627bb78a5b77300fecf929b45116b8bd41112d NO-ISSUE Remove onprem step from Jenkinsfile (#1115)
a938d4cf51e453d0d2dae7ce0068616fa4acdbb8 MGMT-3370: Added error logs to RegisterClusterInternal (#1113)
38fda234ab163861ca0d5209d47f88523071b413 MGMT-4167 Support both 3.1 and 3.2 ignition versions (#1109)
b8c28e41fa42b0f2457e5bb3ab73379ae9b8b3ae NO-ISSUE: validate PULL_SECRET value before using it (#1103)
1857813bd65760573bc065bd8313bb6758f4a757 MGMT-3370: fixed typo in AgentPlatformStateInfo value (#1099)
68cd8166b21fc9f5a6372396db5ccc31066f7c04 MGMT-4155: Fixing integration with AMS when auth is disabled. (#1106)
1a79cf35d01790c30c343ee633a394c3e31aca94 OCPBUGSM-25012 Fixing bad bandwidth subsystem test (#1107)
b699998e99e2269926b4076995d8f57e7e55571c NO-ISSUE Switch registry.svc.ci.openshift.org registry to public registry.ci.openshift.org (#1104)
b02d18ae8d96187699c578f4ea798dd25b1b1d38 MGMT-3137	 OCM Cluster list - Integration (#771)
9ab93cd0f79f9ae6bf3ebeefdcc9c67001e13c0b MGMT-3999 minimal-iso proxy - capital env vars (#1090)
b5f913fd111aebd7111fe7976792d714f5465f05 NO-ISSUE: checking hosts' status before checking status of the cluster (#1092)
eaffe5d4eed02270b9e8f92a00aa03963d3738aa OCPBUGSM-23207 - Fix GenerateClusterISO sometimes return null in certain fields (#1082)
b97c64008b926d442a9fab2ad519e5f6c9cfb803 OCPBUGSM-25012 Check download rate only for an image with a positive size (#1086)
97d699cd7a289d2d5993a02003014dddaa5d392d MGMT-4114 Refactor and use clusterDeployment (#1084)
478f7041d75d5f40346396df241ab2966425bef3 OCPBUGSM-25004 Avoid printing empty image status measurements (#1089)
aec2f09057eb93414d4a8114e1b4e2ea1910dd42 NO-ISSUE: use 'safe_load' instead of 'load' to remove deprecation warning (#1088)
c306ddb915c1f31f6d3894c0b359e31121de6cb2 MGMT-3999 http proxy support for minimal-iso (#1075)
ae0aee1a603327557d4f6f10f1ce650845ca0085 MGMT-4092 Update AI to set bootStrapInPlace option in the install config for SNO (#1087)
f3dba4e67b1926a629c4dcf3d64e005ebfe6380c NO-ISSUE log the params UpdateClusterInternal (#1080)
a934da08f5a2cbbb3638595f0443ad4e37f587b6 NO-ISSUE add the profile name to the minikube status command as well (#1085)
894ba57f721bb066514737930eb6d6b71fb762c8 MGMT-4111 Return BadRequest in case RegisterCluster is called with noneHAMode and OCP version < 4.8 (#1081)
70cbcae96f5a66e08baa9567f755fd22bf758e5f NO-ISSUE add profile name to the minikube update-context command (#1083)
ca8cc1b60e8b885f8341908f6afa21fae6cdeda1 MGMT-3966 - create system-connections-merged using overlayFS and add route-metric to the staticly configured interfaces in order to support OVS configuration (#1064)
7d53cb0a8ece947fc63d15756ea2b0eb787a7370 MGMT-4059, Bump OCP version from 4.6.12 to 4.6.16 (auto created) (#1066)
59a269e64d9c760286e37dbb82e5a3a65355870f NO-ISSUE standalone build performance improvements (#1059)
442658883158f6f7fedab065decbe483263ea478 OCPBUGSM-24603 Remove the cluster-id from http request/response metrics (#1053)
d6eec2449f408dd7ec0008999f310a5706ca8c01 OCPBUGSM-25002 Start image availability event with hostname (#1078)
d340c220780511c231a83fb122b21c0732b593de OCPBUGSM-22823  Disk formatting event is missing host name (#1079)
59ccff6c37d15d7ef220443d500a594f4624af4f Upgrade golintci (#1077)
6d0791fe2c461018d1a2e8d2e5a92e16a9be7f2a NO-ISSUE support macos see https://github.com/ory/dockertest/issues/212 (#1052)
47d8cae06d4731b01fb2529df701bf12dc243d14 MGMT-3890 - Add default-configuration GET API call (#1021)
597087507e6bc04d6244e6d5d42681544b428144 NO-ISSUE: Update OWNERS_ALIASES (#1068)
3bc73c1259d48b711077f5ef7de0c1fde8d066d9 MGMT-3990 Single Node integration environment invalid IP address DNS installation error (#1069)
a87c01f106c5d02e532182a64f755dd17112cde1 MGMT-4013 Add generate-all Makefile target (#1062)
758b4373e1e0551294c480c2dca02594a79d5b91 MGMT-4061: using the PULL_SECRET env-var to access the OCP image (#1067)
b6e37b73a6377032816f9b21ad7a921a1da38260 MGMT-3980 Update go-diskfs to expose file offset in iso (#1047)
6fc4618bea5c770541172acbfec4f8f7b39b1944 NO-ISSUE Update ClusterDeplpyment CRD (#1050)
e66d4d87cf26259457c36ad099048d422cd7f075 MGMT-3911: Fixing 'belongs-to-majority-group' validation test. (#1061)
e4e25032839a8c42e76dc4129d1bf77e5ae70914 NO-ISSUE Added michaellevy101 to code-reviewers (#1060)
3177aeb0e10434e8af0c26dd7a7b12c9f2a53ae8 NO-ISSUE generate-from-swagger should regenerate KUBE_API manifests (#1003)
3847fcde73d20b541f5f953f4e1ddccce95a269f NO-ISSUE fix ENABLE_KUBE_API condtion (#1058)
9bafbf5f4531faf1d92a9629c7e57b4be7669003 MGMT-4033 update OCP release to 4.7-rc.0 (#1057)
4f438597e04a8f757d883dc0dbfe9fad3bdc0327 MGMT-3844 Limit concurrent minimal iso generations (#1032)
e2962c0bf7157284980e5bdf7d2fbeaafe986781 NO-ISSUE Get cluster server and verify cluster instead of specific minikube (#1040)
9cdb683235b2cd759d9380da6af605d0be2d0033 MGMT-3959 Remove OCP override flag references (#1041)
e4596a18fa64beda9d62bad66234b2fd5e39cf64 MGMT-3857 subsystem test for stopping installation when host disconnected during installation (#1038)
3514b70a801124b88f54de3ef5960905a3c031db MGMT-3370: add ENABLE_KUBE_API to skipper and configmap deployment (#1037)
b1df0e72afd7c30a83cb1b89529642ec36ca068f MGMT-3432 set high_availability_mode on cluster creation by ProvisionRequirements (#1036)
79033a8d90f27771ec5be902b2d49d6d3e41ba1b MGMT-3959 Support overriding newer release images (#1034)
129815d0020f66852e42dba22ea04ed7b37142a2 MGMT-3884: Modified OCS validations to use all disks (#1012)
740151c59423e8de440a65da15724eaf9fd8610a MGMT-3920 rename host crds to agents in kustomization.yaml (#1033)
196656c95aa43442df8182b643c8ab186a1f6487 NO-ISSUE Don't recreate the s3 client for local ignition generator (#1010)
27fab2c5e6364ffe84173d533164b83fdb67fac4 Revert "NO-ISSUE adding gitattributes declaring generated files (#520)" (#1028)
3659054f585e10e2b71f07e3ad1f485f545454c3 MGMT-3526 Add container image availability step (#983)
ce7fc1c106e678830a0c29b583e9c3597f325366 MGMT-3920 Rename Host CRD to Agent CRD (#1023)
f929c57e965d5a0d9a613e7e8f031e676c5ee1bb MGMT-3719 First pass of InstallEnv and NMStateConfig (#969)
10a0fe52c90697c890de78dd459a2638dbb39398 NO-ISSUE add swagger changes validation to the build (#588)
ff99a3a9e9405a02291fbddb1d349714fd9551f7 MGMT-3908 Port mapSecretToCluster to clusterDeployment controller (#1019)
d5a4c9feb1b5ddd86c1cb29f97e91f628a28938e MGMT-3910 update OCP release from 4.7-fc.2 to 4.7-fc.4 (#1020)
02900f9992aa508c46883f2137c974020efd916b NO-ISSUE: Temporarily removing a flaky test until the reason is determined. (#1018)
e690cd970825bf65466205f6f8e77242241c3c8b OCPBUGSM-23207 - Overwrite the default value of host_networks (#1017)
c92f8abf571ddfa833481b2f9e2cbdce9a1df569 MGMT-3826 - Versions JSON validation exception for specific single-node version (#1015)
805ea554630242760fb3af89e2c3478a9bf5f7b9 MGMT-3576 Fix logs_cmd timeout test (#1016)
9a6c4e01d2a2edeeceebee1fa6d0443f392983f1 MGMT-3721 ClusterDeployments support cluster installation (#1014)
19e3b6fd0a7ce1c737a5dc494897262a8cbd2e0d MGMT-3576 Add timeout to log sender (#1008)
139c5878b178b1cad82569a6d0f2983d3dd556e6 MGMT-3856 - Add API for domain resolution step (#1002)
7fdfccd2a49c6b0f7ed33b89882198b955a2301a MGMT-3721 ClusterDeployments support update (#1000)
c482fb86422e08737f0a942dc178a90fcdabd348 MGMT-2424: Added ocs-validation code (#637)
2a767c42181ecc0721a7559e52e5c5395afdec4e OCPBUGSM-19591 Host connectivity validation fails when only 2 nodes booted (#1007)
972e06f3d8bbfa5f49c7ee4267b50fa7e1348fe4 NO-ISSUE Add generateEssentialHostStep function for subsystem tests (#1004)
18780f52540d6c632c196b1e97bff09293927cb8 MGMT-3658: Generate event/metric in case an host validation is changing. (#952) (#991)
750cd8bda6b2192d4f42a339729bff4762b429b6 MGMT-3862 update KubeAPI Image with recent StaticIPConfig changes (#999)
539659539e62528ce6889e3b0d683d20e0d1762b MGMT-3872 Fix s3 url for boot files (#1005)
6bc4eea791abe7a1c256b25acff98344bd5970f1 MGMT-3358 Image CRD to use ClusterReference instead of ObjectReference (#978)
feb665a272b359fabd92df1c932560a22e513ce5 MGMT-2662 re-enable the baremetalProvisioningConfig (#980)
61e7c4b014afdc14ffe5d2d1ebb63c2a498cac16 MGMT-3721 ClusterDeployments support creation (#996)
2bc0848a390a9eb4f0d21770ff8f795507723adc OCPBUGSM-23927 - correct openshift version recieved for day2 cluster to be of the format used by version handler (#998)
511e6fda3729063e1a96c6772f44b8455b3736f8 NO-ISSUE Add cache of dependencies before compilation in Dockerfile (#997)
8ed142df83bbd5c62b7d58ad3b7825a8edf71342 MGMT-3802 + MGMT-3299 Cluster fail if host is not responsive (#985)
55e26af2de8854faab60e4fe5c5b15cbf6e8e145 MGMT-3721 ClusterDeployments support delete (#992)
39ce457fa2ad769f66b989f1847941142160ccc6 NO-ISSUE Substitute OPENSHIFT_VERSIONS parameter (#993)
09499d78c7d785ad7e7ecc7df2d69ef14c03c76b MGMT-3510 Set static IP during boot in minimal iso (#986)
13e1bb9dcf3cb8d30a7d7f2101a92e7637cd33b0 MGMT-3797, Bump OCP version from 4.6.8 to 4.6.12 (auto created)  (#976)
f85ee27006201b234bf6b70d98e4fb63d2e50075 MGMT-3362: Subsystem for kube api with basic installation test (#968)
022aff48f7c99c7f9984dce0f163acd6cb5092e6 MGMT-3837 Add cluster deployment controller (#990)
2915b9e7851db6f7600ec18d722e38ae5ab8c374 NO-ISSUE: removing 'role-defined' validation-id. (#989)
d72bcbbf54b00ad6d0b5847a85b92d4060baa7f6 MGMT-3608: Added cluster deregister when CRD is deleted (#977)
72c80921e3d50e2af96555e0f0d80a03ec3786a0 MGMT-3750  -add VLAN option to generate ISO API (#979)
3b47299becf99e48823fe380187cf8220d416b17 Revert "MGMT-3658: Generate event/metric in case an host validation is changing. (#952)" (#984)
fc5b403fa34b83422cbe28f6a882e73c830dcfef MGMT-3523 Reconcile Image when pull secret updated (#939)
5cdc032bdfb646efaea59b3558edb0a387bb4f22 MGMT-3684 None-platform set machine network CIDR from bootstrap (#967)
e06fdb6e35627d5402bb49796c96437f652f6c75 NO-ISSUE Update go-diskfs to include temp dir leak fix (#975)
c75aa06849c60353fb80da07624784d47184e0a8 NO-ISSUE Merge all agent sub-images into one (#974)
2f49f536115b44b4a2270e78968818d36f8230bf MGMT-2622 - Add disk and user to event when booted into the ISO instead of into the installed OCP on disk (#972)
c31a1b85255d514c61f0088fef78b3e7de1ac4ef MGMT-3658: Generate event/metric in case an host validation is changing. (#952)
bf9a813acdbb5140c9ccdedd9f79e709a9c6ff22 MGMT-3763 - Fix misleading host progress error when cluster enters error state (#971)
4ebd038f20035f3e4aca93c73d96430e2e7417d6 NO-ISSUE Fix format issues found by gosec, update format-check (#950)
a3176c0a0d104afcc6f7d76f443adb84ebddc796 Revert "MGMT-2662 re-enable the baremetalProvisioningConfig (#709)" (#970)
9475ac14a769edb18b77e2e0a9c38b7cee360bd5 MGMT-3510 Alter the static ip config script to work during boot (#958)
d13d1ea68297f0102e829605b2bb929f51465be4 MGMT-3526 Add timeout, time, size and rate for the pull operation (#961)
e34aaf449571b4556df7cba50c97d424a7695f9d MGMT-3747 Filter ISO Generated data by openshift version (#960)
2d767454c5cedc15ffbd4c5b8476646e1965c8f6 MGMT-2662 re-enable the baremetalProvisioningConfig (#709)
5514de248df6ff2903e5c8916eb5afdaf2095897 MGMT-2977 Cluster specific minimal iso (#932)
a9ee7f68f6d0a9c1ec2719d789119b858e4959af OCPBUGSM-23568 Generate default no proxy in install-config to avoid passing internal cluster communication through the proxy (#962)
057f7199530f65369315c17a04de32122bdda144 MGMT-3357 Host CRD (#861)
76755d41f70c1d57a6b4c92b5b8505a61c45739d MGMT-3538 support cluster installation with kube-api (#955)
092917cd9f55598bcacd963e13ac4806a848976c MGMT-3690 - Fix tests that never ran, add lint to prevent (#945)
7999bf990196d3ec2076855f1cf4846ba2333dc3 NO-ISSUE Extend onprem installer startup timeout from 1m to 3m (#956)
432f69c82c537cc159e7a7379f398b0b26c9298f MGMT-3717 support IPv6 config for DHCP in static ip scenario (#953)
681ad45cba54bd05a499e17951e1d7770e528ac8 MGMT-3714 Adds emailDomain pannel to cluster overview dashboard (#949)
c9276b8caea3d6490e258e3ed58f6c620ef5983f MGMT-3701 Update AI to use latest release image that support SNO (#951)
c43b027de9d6c743dc8f1f6f63f81f957215239d NO-ISSUE Move commands to hostcommands package (#948)
1ac1cd91e12d5c68af969f2ada24c1a276e54b72 MGMT-3691 Move IPv6 single IP configuration after pivot to use ignition instead of manifest (#943)
f5570061665f7e1b941fa327cf0c2994d7b0e2d9 MGMT-3526 Add image_availability request and response objects (#928)
2e95157c85cc8da2c61063069d3af78059a5d1a6 NO-ISSUE Add info logs to install and update progress apis (#947)
c1d21523582f8351ce38778a0fc0ddc9a91e0be0 OCPBUGSM-23132 - Allow read-only-admin to call openshift_versions call (#942)
ec8ac1605bbd5ef8eb261cf9b6b7a0bc6094e199 MGMT-3431 Support update CVO flag from env param (#944)
9f64a52993165ebfa1ce548f95190f2c8531b61e NO-ISSUE: Removing metrics unit-tests. (#941)
564bb6a911b0c3b17fac49ce0c179b95bdeb782f MGMT-3680 Make IPv6 configuration be sent by ignition and not by manifest when not in single node (#940)
163ecc87b6e6575288969e242f0f8141316012b7 MGMT-3446 Update Waiting for ignition timeout to 24 hours (#937)
6c94d4a38dcd618e05b2acaf2406f919a8931267 MGMT-3482: Report metrics for host validation errors on cluster deletion. (#885)
f0fcd4f37d322b9c2f0f3ace4e1bd5fcbc42ec12 MGMT-3201 - IPv6  installed hosts get a different IP from DHCP after pivot than the IP received from DHCP during discovery stage. (#927)
55ea7af5e82f8d67176467bc5a642f0b78c14049 MGMT-3491 add swagger changes for additional OLM based services - fix (#936)
79a30b7646fc001e3c35ec12f476881b75696308 MGMT-2623 - Remove cluster name from event (#934)
9ac44a925c25ddcba33bd20dc45ca806998da551 NO-ISSUE Set get spec endpoint test as minimal set (#935)
cabc352e0286fa6590d95943fabea25856f0ee89 MGMT-3630 - Fix missing validation for minimum host valid disks (#925)
910f7a73e7718ccb2b09a2d0b3ea08f942609b4c MGMT-2977 Remove coreos.liveiso kernel param for the template minimal iso (#930)
8af11f509d37584c3c27d9f2a4643ed73892753a NO-ISSUE Removes some extra whitespace and contexts from tests (#933)
9dddcdc75c5d53a1c1dbbc3445dd371da1bd010b NO-ISSUE Add format-check to Makefile (#929)
37372ca5e0db562cb4d34cd8cea454dfbc92f273 MGMT-2977 Allow downloading and caching from the public S3 bucket (#931)
964357bf69967e9b0f7ea80720b78c5ebbb04acd MGMT-3620 Add RHCOS version as build id to be part of the S3 object name (#924)
54ac972437d94a3a6ec8f55129c1908fcf199ea3 MGMT-2976 create and upload minimal iso template (#911)
a9d0941b91751a756a4f420772abfa38c2f1077c MGMT-3327 - Remove backwards compatibility code for listing ineligible disks (#919)
2561c0b7c9d0adf9f3b1550d11ad4d6d44aefa12 MGMT-3618 Add progress info to event (#922)
c1b0182702fef639233e330d1fddc43bb071fa42 NO-ISSUE Bump RHCOS 4.7 image to use 4.7.0-fc.2 instead of 4.7.0.-fc-0 (#921)
a8561161562f1fba5960f9b4b1cbf063e4486a51 MGMT-3615 Set machine network CIDR as a pointer in cluster CRD (#920)
d23045a722b9bd8b44903701f8565c2460ea6c2d MGMT-3431 add CVO check flag (#917)
5a64589330cbca8417c141842a5def999d619865 MGMT-3491 swagger changes for additional OLM based services (#913)
7aa360c9ac4ad66c1afddaf20b18a484a1070268 MGMT-3434 Support cluster update with k8s API (#891)
33f5d40fb19174b1c9a455f6869ad43a626d5611 NO-ISSUE add Elior Erez (#916)
d95d615fa2bd194db169318ccae7f34f288f0dbf NO-ISSUE fixing leader test on aws (#915)
b7bd0ef101ff5de0b67156553885a83d6aff5cbe NO-ISSUE Bump RHCOS 4.7 image to use 4.7.0-fc.0 instead of 4.6.8 (#914)
bf8816e60d0413f721eebd7f5eab1b4d399cf4b0 MGMT-3583 user-managed-networking must be renamed to user_managed_networking (#912)
6f4f66f1edb45abeb0496f9c6907600fd54969d3 OCPBUGSM-22643 Replace NTP pending with failure (#910)
f59780720aa0940ac6b42eeffcf2014aa0b85dbf MGMT-3568 - fix formating of boolean input arguments in Install command (#904)
36085329a6cd8bb677c14d510e2bd5b2cc64882b NO-ISSUE Remove [only-k8s] tests references (#909)
cfaca2044fab8359a079e23264e4feb826129467 MGMT-3572 Modify image_test to run against the supported OCP versions (#908)
38c8b884738e2bfe2c9223b7c442361f66f48e74 Mgmt 3539 get clutster by k8s key (#907)
dc8d4c550e0c9c21bce579663d33caeaa5e949d9 MGTM-3552 Remove default for user-managed-networking in cluster update params (#899)
9798ef64019cc26885e3fd5c8795df795c42dee5 MGMT-3356 Cluster CRD - align with K8s API name conventions (#887)
cea7582a40e0acd092d9013b4d179730e370929c MGMT-3508 Update general-overview dashboad to be filterd by oc version (#879)
5cd03575eced3a287fa1912d2747d75d6211fccc MGMT-2977 Enhancements to isoutil (#901)
7f121f4c8b5896482d2d137575e5bc27382e7b3e MGMT-2977 Add a cache for downloading files from S3 (#900)
4ec616b70864668d8b497e266de46dc0ba61acd8 MGMT-3200 Add IPv6 static IP (#850)
85505540de611d32d7e3aebf2095c012f8db5cec MGMT-3361: Image Controller (#865)
8fde13ca421e89d576f9b67729bac3d9848c78de NO-ISSUE Add Cluster NTP metric on PrepareForInstallation (#896)
bbfbdcfc6fb6a646669346f909ce23e25722e927 NO-ISSUE missed run of make generate-from-swagger (#894)
33a1fc8c9e86b2f79d30a78c49d07788ebd5d8f9 MGMT-3551 add name to FIO check container (#897)
7aa29748bb9205632ff051ec15b322f3e94d8247 MGMT-3507 Openshift version is sent to relevant metrics (#870)
5eb2efd5ce94ce408b2dfc1457c0417a753dca7c MGMT-3026 update openshift template for FIO check (#895)
da8c6a83446d821704c282d1141db7e1acc0a7ce OCPBUGSM-22671 Remove IPv6 networks from host networks. (#889)
905341e9954fb988910771bb508d8e53cba40c2d Revert "OCPBUGSM-21433 Enable NTP validation as sufficient for installation (#798)" (#893)
a9621b822cc38047aafd488a7a8b7eef4c85ee06 MGMT-3459 added metrics for disk sync duration (#888)
e3dccf4a6a1bb2c32b3277a6d24f87976ffea960 MGMT-3353 Update ocp template (#890)
7ae02387cd42afab358558ff28cb690b7f41836d NO-ISSUE Enforce description format in swagger lint (#886)
56fcb64109c97be0688691302677e442b970d339 MGMT-3458 Pass REST API params to FIO cmd (#860)
715f2c17a16638c58a7b73b22dbb2402b111c765 Avishay/fix onprem wait (#884)
dd4f2c7e61a354e6c78833a7a748a1d9da86ea4d MGMT-2712 Validate cert in install config overrides (#662)
286f05725d1d277818f195f6093d82abe19a71ee MGMT-3514 Add extract and create methods to the iso handler (#803)
b29e45500f5806b5672003f9ea65eb8d242a404c MGMT-3489 Support None HighAvailabilityMode  (#883)
bb4e14cb17275450db923de4a34c90478bbc96ea MGMT-3353 RHCOS per version (#869)
b981df4845576636704d2c9bacc55ce6ed56738a MGMT-3502 Add linter for swagger (#882)
0af263b609e991af2887ad3f8b98f5823341016d NO-ISSUE add goimports to fix auto generated controllers code (#881)
b18e08ae96844c5c2743c1a27fc0af7362ed7834 MGMT-3476 - Service will set hosts installation disk path to the default installation disk (#864)
ac5f5d85d8bf06cef1fb2b5286dd30dc2fd4cac2 MGMT-3297 - support static ips when rebooting nodes woth RHCOS image (#872)
7198539ba83b22c1a3a8afe08e1d9ee1b69b1a50 MGMT-3330 default OPENSHIFT_VERSION  (#847)
76aeb9b85ac13dc38ef377e4cd44d453fd23bfb3 NO-ISSUE - make format target shouldn't format anything the linter doesn't check (#876)
9b5c6fe5535a9e228279560f367784c39bb12d77 MGMT-3356 Rename Pull Secret in Cluster CRD (#878)
ea757d4217ffa2c4aa3d00b5444bf82b3c74e4f9 MGMT-3489 Update create ignition-configs in case HighAvailabilityMode is None (#877)
c6b3742bf22dd5274271173fdb51b8c357d96a4e MGMT-3358 Minor fixes to Image CRD (#874)
3c2dda0ec144936807c706449f05605908c57e5b NO-ISSUE: Fixed typo in spec.channel in lsoSubscription manifest (#866)
209a9c80708290b915454f30b53b80743ca90c5f MGMT-3511 Wait for service in onprem deployment (#873)
e95d0de4db3c70204861bdf5de6055fea8318a22 NO-ISSUE Stop trying to push the iso create image (#871)
b59b8e02ffacc231684afe86febb11a23e6a32bc MGMT-3489 Update create ignition-configs in case HighAvailabilityMode is None (#867)
37c09c4896465cab81544ba8bd55cafd313a0166 MGMT-3456 - Will not attempt to format bootable disks that look like installation media (#862)
6dbfbda0da697ccfa59b6d4395f223d0a145a5d6 MGMT-3488 Move cluster_mode set to register cluster (#863)
a7f51de15781d8a56cc7ef19b4591b7eadabb5ad MGMT-3433 Create cluster with CRD (#857)
d086d8c2b880925d00cacac335f29eb90f8b76c4 MGMT-2245 Extract OCP version from OCP images (#856)
36093cae672a5cd59845f607d2935742267f6e3a MGMT-3100 - Add missing generated files (#858)
c8fa79127d0ad394d3bf511c5320f1268622ed93 MGMT-3407: Add cluster controller test infra (#849)
0b17558aee9e3420305d28201cab00a6286b0187 MGMT-3358 Image CRD (#844)
4eadfef3f66e5e9ec4c1a3a450319ec9af44e49a MGMT-3405 - block role and user network mode update in sno case (#845)
36b517f589451192591948bf60e7f8537e62b1dc NO-ISSUE - Makefile cleanup target used pipes instead of conditions (#853)
5bb6c1d46841d13add5d4b6df01b94b84ad78e44 MGMT-3437 Shell escape for installCmd (#855)
8f47ccb9472b3e6de5fb79ab5a2193b97bbdfef4 OCPBUGSM-22592 Clarify disk format event (#852)
cc83daa38bff666b526055cacda3063cc2c9ee1f MGMT-3452 Collect logs from onprem on AI CI (#851)
38fda0e75b9583ee48d1316836365ba81dcc43b1 MGMT-3407 Add host and image controller unit tests (#854)
95d091d3609710680d5ea022e628de637409396b MGMT-3100 Upload/download PXE artifacts (#755)
8cdc19b60d3a81e7e1d7aa7a82c46c8fe48d2e1a MGMT-3026 increase FIO check threshold (#848)
058d6fe6020324dfeafcd1961cf3b13e1e243fc7 MGMT-3356 Create cluster CRD (#843)
fbdbfdcab3b3669c66f108662430802d3b11c56c MGMT-3410 Add HA mode to install command (#842)
ef465b6a394fc37031c65a8e978f8316f50e3b6c NO-ISSUE Add userAuth to DownloadHostIgnition (#841)
cdd01d086744077320c0778bd825a3f6062c87fd Revert "MGMT-2245 Extract OCP version from OCP images (#820)" (#840)
4c883a96efa6bfd53ae9a1db05b938ea6bdf1f33 MGMT-3355 Add controller generation call to controller manifests generation (#837)
cc6eec50adfd986b3c0409b7e9b7d8ecb4db5381 Revert "MGMT-3410 Add HA mode to install command (#835)" (#839)
f217cdfc9b0b10d425b7b545491e083ee2cf5ff6 NO-ISSUE Change log to log format (#838)
a23bdda5389fb3641f096f4575920c927f98d1ab MGMT-3330 remove requirement for OPENSHIFT_INSTALL_RELEASE_IMAGE & OPENSHIFT_VERSIONS (#836)
9ede34392f7d21ee7fccc9e613d582f90e6c74d1 MGMT-3410 Add HA mode to install command (#835)
b3a51f40d3bd4049f76cdf26eb5e2dfb20759e2f MGMT-2256: run tests for openshift ci deployment (#832)
4634b379daba648d2ce3b649bec28ea067e53a85 MGMT-2245 Extract OCP version from OCP images (#820)
cd77b8979be81721da1e7fc4424d0c0865747a1f MGMT-3419 Verify OCP versions on CI and on deployment (#834)
1e460d77b591216b140dad7ab0d48fba1a6ad397 MGMT-2256: modified Makefile and scripts for openshift ci deployment (#831)
f547044473d41b231aff347fd4c83336914c7f1a NO-ISSUE log OCP & mco version (#833)
f93cfaf76102041c0fc63b4158c254359ba40573 MGMT-2966: add a single node mode for installing SNO clusters (#715)
697a281f3a06b8314d7ed74e9a8985d6e142b8f3 MGMT-3355 Run controllers along side rest-api (#829)
d0a1ba34a37c86f6b7468081dd8a3601c34adcf1 MGMT-2782 - IPv6 Phase 3 changes (#818)
faaee376745c04431bccb8f39f9c506099032a29 MGMT-2470 silently fail if free addresses container already running (#728)
250e579c7b24ee2791f2e3567ef23c5cc11ff00e MGMT-3026 - invoke fio from installcmd (#806)
613ee6887dab1368cf5b4b6faaaf4a8c45d3f0b5 NO-ISSUE reduce main cyclomatic complexity (#830)
09e1d3707c5ca3a36b2df25072bea69c1ea926e1 MGMT-2256: placeholder makefile targets for openshift ci (#824)
debe818dbc42df14faed5360e900f406c40c9571 MGMT-2245 Bugfix OCP override image (#828)
cd1bd81516fa2014b96f392eead13ff1de827792 NO-ISSUE Extend wait for assisted-service timeout to 30 minutes (#822)
47be818b6104ffb4524faec5061748fb2697049c MGMT-3078 - Add disk filtering reasons to the API (#804)
2b8f842a0a37e76b81599029d1ce9401f4b5637e MGMT-3295: On installation delete old cluster logs (#821)
06b0bdd66b3939ae0130782ec7801c5deafccb39 MGMT-3303 update OCP release to 4.6.8 (#815)
5138bfe5e29b0b8e6ae228719fef0640c78a7f3d MGMT-2245 Bugfix add default 4.7 and create default_ocp_versions.json (#819)
ac76ddc0717862359951eec05d621eb161ca682c Add host count to InstallationStart metric (#799)
e805401970e98676bd145343952dea949ca5b4a3 MGMT-2636 Remove uploadBaseISO job (#645)
3ee4b32afa41653849c4ca0608e5776ee2d6e297 MGMT-2245 Support OCP multiversion (#805)
137c9639306406b166ec4a0ed3f615d759fb1ecb MGMT-3117 select boot disk (#814)
256bb583ae9ef79ac0ab2478347019b850ec84d3 MGMT-3296 support static ip provisioning for discovery ISO (#812)
bc59e3df5a1573be678f729214ed2de891e51948 MGMT-1263 Add --image-url to the installer allowedFlags (#693)
8ca5c20f9f90321b8af6e231ead983ce4714174b MGMT-3062 Allow cluster progress updates for two states (#809)
c22520743a9e6490ee2c90678745ccb8a0652dac NO-ISSUE format mocks (#813)
29a24ac99ee0b95e856f8146d2853d84e3c05f09 NO-ISSUE Default of a single service replica (#807)
1314760d5e8f90c7f161c59343d6f22599c3cafa NO-ISSUE hardcode SERVICE_API_PORT in onprem-environment (#810)
8494d8fb48d6a20195b2c5c17eaa01a8bced3a26 OCPBUGSM-21144 Document stand-alone mode (#774)
6c832e0d484b4dd535a6558044beb42bd61da6c8 MGMT-3287 Add none-platform label to startInstall metric (#808)
d527a1a9fc3d7784573a5fb4e4e0b2c196f03299 OCPBUGSM-21433 Enable NTP validation as sufficient for installation (#798)
7fa60b0f3839f2227412bcdf1afb37d4f2fd7405 MGMT-2991 None-Platform logs commands IPs (#792)
247205470144d6c058bd6da8251f8ec881825fa3 MGMT-3117 Add API for selecting boot disk (#787)
dbe992eacbddea5eda32ee5a71f69481842b2d9f MGMT-3120 IPv6 connectivity check (#773)
fd704de04f287523a18e3c576ee1cddd37856603 OCPBUGSM-21213 skip cluster validations when cluster is not in discovering stages: ClusterStatusInsufficient, ClusterStatusReady, ClusterStatusPendingForInput (#777)
b23f84e01fb6d51f88bf50984bd138025254cc29 OCPBUGSM-21366 Support comma-separated NTP sources list (#801)
33090c305040b9202c7f84b4be9489568e79c84b MGMT-3262 Remove app-sre images (#795)
7c2f6f30853d3190981e3d4864f34ffc25ef087a OCPBUGSM-21552 Bugfix trailing parenthesis (#802)
faa41eb215e73b7af643affe802bf22c0c4bc2b3 OCPBUGSM-21583 Remove RHEL default NTP source (#797)
218d098cb83eb94a2f5bf6e0747e9ad86aede2cc MGMT-3078 - Reverted #772 (#800)
45ecdba76cf9766a9e4b67541efa48d2442b533b OCPBUGSM-21552 Add workers chrony manifest (#796)
ee98d122d64cbb2ee02cc24e0acba0ccc04a0a28 MGMT-2424: Support for LSO(Local Storage Operator) installation (#762)
a44d335ba6dc7bc4f3367e02c72ba4cb65d1dbbf MGMT-3078 - Add disk filtering reasons to the API (#772)
b0ef94269de6a08d5ebc0b61a053e0717755bca6 MGMT-3261 Add ISO Generated metrics to weekly and general overview (#794)
fe1e8664be06e5f6898e7381afaeb9a799023271 Osher/ocpbugsm 20497 (#793)
2cf921c2df5762ab952f7cdb4f3988480e7b11e7 MGMT-2758 Remove image from s3 when editing the discovery ignition (#765)
45182691e179915d719aeaee2af0a916ec713d08 MGMT-2765 More robust curl retry via shell script (#790)
c41faa699553e033b00f87ed77877c14cb131318 fix podman pod create format (#791)
1856df753deaf1bb5de79a854b0fdc485a0b093d MGMT-3064 User Managed Networking cluster params conflicts (#786)
413c3d82572308c2d798f961328bfb34a6e3f982 NO-ISSUE Add 4.7 support on swagger (#788)
02e048c17284e386d2c7278412137e3dac7bcfec MGMT-3220 - Modified ISO password set wording (#785)
b64284efc7de8d3e5530dceff7dfe98582c3599d NO-ISSUE Added Omer Tuchfeld (omertuc) to code-reviewers (#784)
be8f43281f605e3947b19bd1a8ff220faf3ce65c MGMT-3220 - Add documentation for setting discovery ISO password (#783)
13e1d3350077fbd32909cbe48d7d652c03dd8360 NO-ISSUE Fix + update weekly overview dashboard (#780)
18cb025addae9c087c9dd473bd52fbd5763d1eb5 NO-ISSUE Adding Richard Su and Sudarshan Acharya (#781)
bab0090a96a2397efcec070ed69b95a1bd2583b4 MGMT-3061 progress_info should not be a mandatory field (#779)
465f4e2da6c580bae145f2799c7b073e86e08763 MGMT-2254 Migrate Grafana additional dashboards to assisted-service codebase (#778)
3a363c9721b6046f81774f884290d3d8122ab38f MGMT-3061 Add cluster install progress (#748)
15cf6a5290b9671961bae027157c3170ac205278 MGMT-2254 Migrate Grafana dashboards to assisted-service codebase (#775)
cfec44c3901a16169cc17cc132f4d4924f5004ec NO-ISSUE add cloud README (#776)
bd823a09ab6e30ea200231dc272e057134b2bcdd MGMT-3153 - Disable password login for discovery ISO core user (#764)
fb1565479df6c97845e7359236fc3aad02fecc78 MGMT-3182: remove duplicated refresh status on cluster error (#770)
223ed05ff82eec4f3b37cfe46eb2eac6f68b7331 OPCBUGSM-20841: Wrong boot order hosts will be set to error when cluster status is error (#769)
afd525b8f59a552039162ac605cfc2d7e573ddc4 MGMT-3130: Change unit tests to use httptest server instead of http server (#768)
b74376fcb143d90e859c59f6b1eeac521fc91445 MGMT-3086 - implement InstallHost per specific day2 host (#767)
cc653e4e35edea383391f2b41e611c82e5161cfb MGMT-2277 - remove references to the unused ignition-generate-image (#747)
22a3d2fdad365eb2c5f716b789d4835a50ed91f1 NO-ISSUE add helper method to updateClusterData (#766)
92e3dada0586054039cb53f468635c1b3501f01a MGMT-2573 Extract and use MCO image from release image (#648)
dcae87ef02533706758fda476dc999e065539a7f OCPBUGSM-20856 Remove ssh-public-key length limitation and migrate DB (#763)
f99dd73db60cf54121086e49313590beb1cce465 Add a migration generator and documentation about migrations (#596)
47280c3e972150076d1f6cc4c0d7ad94d29732e9 MGMT-3054 Add host machine config pool (#760)
0c67ae8711ea8a0fa8644d5a03950d088b7f1897 MGMT-2738: installcmd.go remove MBR sector from bootable disks (#761)
b49914fce0793cc3ebca2fb182a25212c3ec8950 MGMT-2780 - Changes for IPv6, Phase 2 (#756)
6af24346590c704b208a69eee900603f3f1d37e9 NO-ISSUE - Remove romfreiman from OWNERS_ALIASES (#759)
eae1c5a0cafb67fca6ce1457abef19c8deacb401 MGMT-2964 Skip Machine Network validation for none-platform (#733)
8fdfae0165d3a7ccbd00568f0d44d0249aaec89a MGMT-2892 Add openapi endpoint to return api spec (#758)
272472df2fbc8952d37f7b1814def909dabfe2ac MGMT-3128 - extract ssh public key from OCP cluster (#757)
724793e12443537f41368603738166775946db1d MGMT-3027 Wrong event when timeout on writing to disk (#753)
3aa4b384dd435a89d2cb72615a1a9beb06992f3e OCPBUGSM-20982 Bugfix List manifests onprem (#754)
00b4936261245ce6fef618f22948b493d5062751 OCPBUGSM-20944 Clear kubectl objects with force (#750)
ae77333260376c6f542c9878c841bc72bdf43c20 MGMT-3103: reduce image expiration time and interval for local e2e tests (#752)
6817194e17133cce33ca6e2c1279513a270c6bf0 MGMT-3024 Update OCP release to ocp-release:4.6.4-x86_64 (#726)
b429c48f1e0a5b2d1715c57640832ee7597a7f4f MGMT-2322 Bugfix Default NTP value (#751)
412e86f257a67cc5b57672dc1b9a722f657fc637 MGMT-2370 Bugfix create chrony manifest with no ntp sources (#749)
9feb42c785968109e5df62a2bba5295bbcc77a6e MGMT-2370 Add chrony manifest (#743)
f3fe28fd6e732f3b6a64cd5c7658040813797a8e Revert "MGMT-3078 - Add a unfiltered_disks list entry to the inventory API (#740)" (#745)
1ac2c61ac6978b9535badb56181f5036a8b8bb3c MGMT-3078 - Add a unfiltered_disks list entry to the inventory API (#740)
a193262fe85bb3407c86011f4d499fd781c2b946 MGMT-2955 add retry to live.iso curl download in deploy-onprem (#742)
16ab19ad6150e0955392f20803273a429d43ecf9 NO-ISSUE - Remove masayag from OWNERS_ALIASES (#741)
0290a5089dc07c4dd79f94d15cfab87a3206995f MGMT-2322 add ntp step (#675)
66cabb26873231064f6a2a715e2e9a44581cc230 NO-ISSUE - Added missing env forwarding in deploy configmap (#739)
174b2623f0d61f5dca6184ff5c7888722ad41e04 MGMT-2943 Expose discovery ignition separately from iso (#691)
632752de76c462c48c310b760ba26e32d95f31b6 NO-ISSUE Remove docker objects cleanup (#732)
fc89b94631c24ee7ad4f20b62b6e7c0e53e9e094 NO-ISSUE Merge RUNs of curl and chmod for assisted-iso-create (#729)
9ba664cd7ff4b7fd330dc02920f493ef77e2c193 MGMT-3033 - Added S.M.A.R.T. field to inventory host disks (#727)
82bb414b2ba481cd2bab480aa9e972e7c6386130 OCPBUGSM-20820: Removing workers IPs from logs cmd. (#723)
ea25e6b734dd73d25d1583e5bcf2210d6a1b9383 MGMT-2411: Added error_utils.go (#721)
e74d8c879ddda35179154fcb7f57907c84d0a956 MGMT-3013 - fix the IP format in BMH annotations, fixes the link between Node and Machine (#725)
e9a95fe03723083c392c6740dcc467ab9547a5dd MGMT-2989 increase timeout of writing to disk from 10 minutes to 30 minutes (#718)
eb8c88e25b5d552be023ad689436532535191595 OCPBUGSM-20151 - in case day2 cloud cluster already exists for the UUID, return 400 (#722)
574ccd0fee676bd74be2af280fb087ff4adfb39d OCPBUGSM-20425 - failed day2 host should be able to be reset and to re-register (#719)
c88428c2fc38417b48957ae0b3eef1b1b8de4c46 MGMT-2678: Adding list of IPs to logs cmd. [NOT-WORKING] (#704)
46568eab73cbbae267932a19f4c7b9b895090ef9 MGTM-2834 assisted-service on-prem reset doesn't clean old cluster state file (#711)
f5abfee7a18b6a5dcefe937c0706fd86b255022d OCPBUGSM-17591 [1879103] Failed validations on the cluster after installation completed (#713)
48cf48352bd9c080d650eae44a9143d3865c75f3 NO-ISSUE Regenerate files after swagger changes (#707)
10908528c1710e555b67df96851aa7421512d651 OCPBUGSM-20497 limit cluster name to 54 characters (#699)
89c1250f6d6901775c6d92d078f8f25cfbd33e07 MGMT-2403 increase upload log capacity (#705)
0d610b28d817b91b55cf67d3d6ab6e463e03d567 OCPBUGSM-17327: allow "*" as a valid NoProxyFormat (#642)
6eac158645777354c302f9658be45b2d0cc78ec2 MGMT-2393: enable filtering clusters by Openshift cluster ID (#686)
ec5d62448f049f56c5c221a36ab8978194ee47bf MGMT-2965 Reset fields when enabling host (#701)
89b1e7f30ae4bb199fee8e296dd22c7b2c8d9405 MGMT-2982 Fix image build race condition (#702)
df6fc7a9e07366aec892579bf807a9c5d2bc762e MGMT-2765 Run a subet of subsystem tests for onprem in Jenkins (#692)
f3ca1daecb7d5543f62a4ba1cd745bdfa490c1a8 MGMT-2465: day2 - single replica for ocp (#700)
8097c1bd96194c4041fb4162b77bffb017bdbd0b MGMT-2752 - Add user-managed-networking to cluster (none-platform) (#674)
ccdd5661e8f23bcc7b0a7c11b121acfebaf9cccf MGMT-2947 - move day2 ignition from general to per node ignition (#690)
2f02ec5362ef55c07c42a5209d4bef9fe905a6e9 OCPBUGSM-20496 Add hostname to host enable/disable events (#695)
d789e964e1c6201955b979a8819246432e808a3e OCPBUGSM-20563: Allow registering an unregistered cluster (#694)
e97b039ef0c051029dfd5d2848ea018064ea75ec MGMT-792 - Swagger - added virtual field to system_vendor (#688)
4666a6791799f3939851994e945c232699d51695 OCPBUGSM-20532: Allow register deleted hosts (#685)
65aa5066d9633999f9f0f8c2c07dcf708668828b MGMT-2936 - extract machineCIDR and baseDoman for day2 on OCP, fix api connectivity check for day2 on OCP (#682)
0f6dbe96a56aa0191d07a472f802b3ef07ff5193 NO-ISSUE Handle ISO generation cancellation (#684)
2b452edf98014ec45b4382e68fc48245156b833a MGMT-2652 Inform there was a disconnection when stage is timed out + test (#680)
15c76d5a1622f3d749b3b06b64ec8e9f156ab4c3 MGMT-2694: Allow additional installer args per host (#626)
3b458aa3ef5c8b265a01bcde2e88cfc9f343b112 NO-ISSUE Add unit tests to ignition generation upload to s3 (#683)
bb99c1704bbc7464ffef431101c141774473edd6 MGMT-2888 Add marker file to bootstrap ignition (#672)
7dc7674fe0ec3ae6539338af66b645d84e679d2f MGMT-2384: Add OCP cluster ID to AI cluster entity (#663)
7eee80c8cbcf48e1c88a0a78e3bd9b7407f7e8a6 OCPBUGSM-18132: Added AddForUpdateQueryOption to cancel/reset (#677)
ef59391796e61186e545f55662a0e8b593c60b60 OCPBUGSM-20495 ignition generation should skip upload files of dislabed hosts (#676)
be82d501cee20799a4e0d4d95527878886ca6a92 MGMT-2208 download live ISO for running AI on-prem (#599)
3384da12377ea23d9236f8eb9c527172394d5f13 MGMT-2889 Allow registration of host in error state (#671)
64b64b458a5be660785585999d7c34da3fed1e79 MGMT-2633 Stop sending the hostname to the installer (#670)
66ab7e7ad61f528b74fda9299538edabee6439b9 MGMT-2624 removed proxy URL print when proxy URL is empty (#656)
00c91582b69e9a2f6ca43af30b774a76a9070094 MGMT-2464 - update state machine and instruction for day2 OCP (#665)
a5c605b2f4439b265101a36aa4c5fff038f43a6f MGMT-2871 Revert "MGMT-2472 Format bootable disks on Install command (#593)" (#668)
c71f127ba6f2eb01ced3dbca9c744789919c9c4d NO-ISSUE Clear created images after Jenkins job (#667)
3251ed6ad99f179749a2d7e5a173aed7e93f919b NO-ISSUE Update OWNERS (#664)
3613e9673e4732f04658b8325a2db09c9e84da60 MGMT-2868: refresh stage_updated_at if cluster is pending-user-action (#666)
eb35b40acdf8d43f48aca4736475814794de7aef MGMT-2456: new cluster installing-pending-user-action state (#651)
53f73480799d28c231331c2a0ae72a8a22f01bd3 MGMT-2857: Fix image expiration (#660)
e78a899457c09cd214dc3d76a1a9917450870ba3 NO-ISSUE: Generate and verify onprem configs are in sync (#594)
af3b34fe7973c8d8ff285a09a1cc3a90a6be42ff MGMT-2846 - half dummy inventory should be created for day2 ocp cluster host installed on day1 (#659)
28a947ed491a81134cae02984fbf85246fbffaba MGMT-2831 adding failed validations in events while statusInfoInsufficientHardware and statusInfoPendingForInput (#657)
ff39405ce2534b0d1c36472c60edec68324d2b27 MGMT-2137 Exclude quay.io from pull secret validation in onprem (#658)
32d8818fcbab554964a4e14ab3b9867fc0d85e09 OCPBUGSM-20065 require pull secret in swagger (#655)
bb2f4a5dbbd8357716edeacc0ffbc540fa1e1757 MGMT-2629 Added secretdump package (#653)
e95d2c24a4233aece09c9878ef0b9d1b898957ac MGMT-2821 - fix the getting secret k8s implementation (#654)
7c8f588df79a4ad24bd9abbf6ea78df8b3448dd6 MGMT-2322 Add NTP API to swagger.yaml (#652)
c1742107cc55c463f561eff2aa3ec360324a2555 MGMT-2611 - Event on failing validation specify the validation (#650)
9c70982f49a68550c8c4c2dc80526504b83403ff MGMT-2821 - day2 on OCP should use pull secret extracted from OCP (#649)
e38d6da6e0a8e145e73db94ead1b799a78096b7d MGMT-2462: deploy on ocp - copy livecd (#644)
be1bc532930e1d07bcf4a5f24936e2ed96776e80 MGMT-2788 - fix installing hosts on day2 cloud cluster, when there is already an installed host present (#641)
bc684252bf7c07e34f05e1551930e00143473bfd MGMT-2657 Fix StartLimitInterval in agent service config (#647)
dec25d5b3b0edc1c3658b5017bc12ed32d0c2241 MGMT-2704: added nodes to ocp clusterole (#646)
a953e37cfc35147e770d80101927893c5b204f63 MGMT-2592: adding mounts to all required files from host for HW detection, and direct ghw library to the new root directory (#627)
28ddb8ee9303340e5c437c1ef2873624ad1f6f7d MGMT-2331 Host ignition customization (#568)
485aa0797b4b396e948fea55f6c8ee36f66bcd14 MGMT-2770 add inventory to installing-in-progress (#639)
9fbcf52e8938aea05e3dd9f47f920201197ca1ba MGMT-2137 Exclude quay.io from pull secret validation (#640)
3fb6d9fd0094613522f73693bc9245179373fa09 MGMT-2221 Host-specific ignition files (#466)
384ae08c64a9d4cb65ecbd412a96e33103ed0389 MGMT-2575 - create installed hosts during day OCP cluster registration, allowes smooth validation of hostnames (#634)
eaefddf5e49302d2b0d4e353c88c0627debef821 MGMT-2137,MGMT-2134 Verify that pull secret includes required registries (#609)
fc512e8d51427ee2a479049b91abfd4e32689149 NO-ISSUE Update Makefile for onprem (#631)
232760d59757d3282add2365a9ca1d66cee8073f Validate user is not installing on OpenStack (#633)
24c4a117a6b5a497982118e02b223d81b6db6520 Raz/mgmt 2746 unregistered cluster fixes (#636)
d6f38eff3369f2f73bed6d58f97d47d164f7cd1d mgmt-2320 expose logs deleted clusters (#525)
7d1df8a9510c88e2c0c6e4e0cea302f034fa35d4 MGMT-2450 Add email domain label to cluster and host metrics (#614)
0b5f50d53dffaf2d8712e7e806e497919bb8334c MGMT-2659 DHCP server changes the VIPs addresses after installation has started - code changes (#629)
b435e08835b8c4a84f042aa9787346633002dbac OCPBUGSM-19651: fix installation's event message (#632)
3f7784f45d1f43889f65346df7f134ee1e87a90a MGMT-2734 - fixing error with go get command (#630)
30186e36bcd00bc3d6036844d9458a7e877feb4f MGMT-2659 DHCP server changes the VIPs addresses after installation has started - Swagger changes (#611)
6bfedddded7fdfe1fcad3c1fa92aff7be2ccb600 MGMT-2377 - Exposing grafana and prometheus as NodePort instead of clusterIP on Minikube (#284)
2e91045d192718575e67849cbe7daae0a3301cf2 MGMT-1992 - User guide added for iPXE use case (#402)
e1fb12594285c9f97479496e8432a292598afe75 MGMT-2612 Fixed 'base domaine undefined' validation message (#625)
3b1fa04a3bb93c2e290f15c6c9f50d29c9f51478 MGMT-2320: added ADMIN_USERS definition env to openshift template.yaml (#624)
da122b778fe322647f3660fe18cd1daac2c75f21 MGMT-2462 AI on OCP cluster (#602)
17a14385b8b6ac9c4799c6a79a332a3fe5533436 MGMT-2320: added ADMIN_USERS env to openshift template.yaml (#623)
61b1ae8c94366ce76f31104035510fba7d7f4455 NO-ISSUE fixing logscmd test db issue (#622)
53218f04d3d8c90af698c392a221b8dc0638f135 OCPBUGSM-19500 - enforce worker count with auto-assign (#615)
6ea925a3300d88831cd90e4af5dd925a90ebb2b8 MGMT-2704 - adjust role deployment for assisted-service day2 on ocp (#621)
03ad5d52bf869d29d6f4fc9323ae3adb83da801a MGMT-2466 Make the override columns text and add migrations (#569)
3c42660941f4300d4fd7886b6ef6cc3b6abef4df NO-ISSUE Fix README issues, Add Go Report Card, remove github workflows (#620)
4ecbf7cb604310b23975379fd8755ba4b768ca7b NO-ISSUE Bugfix: regenerate ignition from fcc (#564)
4b637d6c62360e20c27a3aae6323376646cb11a1 MGMT-2695 Move logs upload command to separate cmd (#616)
40484491161f5575e638ae23a95136faf26061d7 MGMT-2444 - Update OCP release to OCP 4.6 RC.x (#619)
d825604dd26bcef0b8c2fa2378902fab2b49d8c0 MGMT-2692: Fixed waiting for server in authz test (#618)
c535c67af1a82aea1335a6a0e0b16be74f659310 MGMT-2227: Use running livecd when running on prem (#592)
0607d0d2935a929d7909076a7829c0cf8a942b39 OCPBUGSM-19651: sending event about cluster installation started (#608)
d6fa3b9e072489ec8a0e8d8389455b6ab0351152 MGMT-2674 VIPs DHCP leases are not renewed in OCP (#610)
428749c6e418d18f4c8d992e9ce634a98069f69d MGMT-2479 Cancellation stops only installer container (#595)
659f5ef5ea5a2855833b1f63b31a56e15205d2b5 MGMT-2598: Added finalizing to cancel/reset transitions (#606)
e1ada7020893532c2284cba27a0bf6b5ce5375c1 MGMT-2472 Format bootable disks on Install command (#593)
d6f364442297731f049c806f07c26097bf940e71 MGMT-2463 - implement OCP Register day2 cluster (#598)
48e397c3a5432b6acbc290fefe893dc7e4f03fbf OCPBUGSM-19585 Register disabled host (#607)
06ee8d4c1453d9b2e7a88274fe9003f7a5a3778c MGMT-2480: Wait until server is ready (#600)
f06fe06a75a022d8ce1449e737552547161145fb OCPBUGSM-18248 wrong validation message when host has 4G RAM (#537)
c368b96ba54c699d7b7b8aba1cb1e40008fb6c62 MGMT-2586 - fixing updating hostname for day2 host, when there is another hosts that was already installed (#605)
0f0ca673a206a8b8c0aef54130a53b2b154d7cf7 MGMT-2635 Bugfix: GenerateClusterISO failing in subsystem tests (#604)
e72cbef67a5ee55bbd50eacca3e5a9c669047fa5 MGMT-2625 Add HW info to assisted_installer_cluster_hosts metric (#603)
b1b91e27272e917f09bb1ecf38909dd097684ff0 MGMT-2431: Added parameters to get logs command on installation failure. (#576)
e43d20843bc1d5dfc3b34838cb157a75acb8ff62 MGMT-2295 Give the test cluster a unique name (#597)
2f2920a79bca475a77be1070f2e8311958c74f4f MGMT-2480: change authz test server port (#591)
3520dc3dc191187c704d9904cb4a3e522b085458 MGMT-2416 Fix wrong state info on timeout + test (#589)
1dd3d75832377b30dfa0a7594239dd9805effea5 MGMT-2389 - Missing cluster_id in some logs (#587)
8e9b1ccd3366bd2355189ef0e15670ff7f775023 Update assisted-service-on-local.md (#586)
23f8c2b84441cb3c240aab17192c3e57201d88b4 MGMT-2488 We are automigrating db twice - remove automigrate from main (#585)
889a9f77d660b57fc0e9b2a86dc20b8dd8f027e0 MGMT-2480: Fixed flaky authz test (#583)
75bcede4828d27c0c48ac97bcf1fad6527eaf4f7 MGMT-2036 - Agent APIs have User Identity filter (#447)
fd4fdf886425e8c1101796749a17677f5ec2a13e MGMT-2237 - PostStepReply API will return BadRequest in case the request exit code isn't 0 (#547)
8be5d33d867cd33883ddba7c0767221395df90f9 MGMT-2473 Enable command to return multiple steps (#577)
a89b8e8f3d576c71a2d8cdd38c6983ad8bf8e4cc MGMT-2364 Return post_step_action enum in next step API (#581)
1463352938a68995a8107526aa6d4e81895a8d51 NO-ISSUE increase CI timeout (#580)
bfa0d5fa8feb575604b6ae38634d00e83fa6f4ba MGMT-2444 Update OCP release to OCP 4.6 RC.4 (#573)
0617d1d3d2333244b8e4b0a947ac96402a951530 MGMT-2307 Publish release images (#563)
2fbec6e9aa263fcbd60b08c2c5b4b6244d842edc MGMT-2407 Run all jobs periodically at night (#572)
d6e0afd56a4294619048b9c6b2d4b8253e7eb4ef MGMT-2069: fix conflict code returned by host registration to be an infra-error type (#566)
a310366d189a25e0eb7e4fdd6e74282545721220  OCPBUGSM-19280 adding api int to noproxy param of assited-installer (#567)
34c9f05b35869e2eec03c57cbe8891d3cacad55f MGMT-2415 change id label name for HTTP metrics to clusterId (#579)
7236ffed2eecac1ef01135863da9b31fa8f5dfb4 NO-ISSUE makefile: added update-service rule (#554)
c631bd9262b1c32b61801f285d79822e0782f45b NO-ISSUE Use the centos image from app-sre (#555)
d35f8c02431b1f9e2f39fb7888a64f8b721cfa55 OCPBUGSM-18606 Improve log messages for failed step replies (#565)
016a1dfbe165968ca698d11493d86027f13bf281 MGMT-2069: make server return 409 code (conflict) when host tries to interrupt and register (#543)
7fc7d6ebd05863d1ecd765cbec1de1189f059728 MGMT-2401 (#529)
32e252fbcc36fd1b924bee76b2bf1a86a4eaf0a3 OCPBUGSM-18082 - Fix install command failed test (#558)
2099ea324997095feed271c38b9d6cafbf11ac2f NO-ISSUE Using centos postgres except for UT (#560)
b5cea760619c5c8d00b78fa55f1995c6b958a705 MGMT-1780 Allow user to provide manifests for customizing cluster installation (#215)
0b1ffdce7a399b4cd8e296cdda07b5b7498cdeb8 NO-ISSUE Fix installcfg logs with right format (#559)
c70f70aa2e7bfd38ad4495b4b65af317f5e543b0 MGMT-2313: Send an event when a host is chosen for bootstrap (#522)
84d6a0b15b55c69d438ddf78b5ed7bc390edf8aa Mgmt 2230 added authorization scopes (with read only admin) (#448)
949935cb478d25037e1da2c96602faca8e8c4853 MGMT-2448 Add installer image caching to host discovery (#550)
373a4f5671df445cd1d722e40c479c08e2bc9bcf OCPBUGSM-18082 - Increase defaultWaitForClusterStateTimeout (#553)
684a8a214bf686e423ccd6f1480ca1f4aa16c2e8 NO-ISSUE Use log.Errorf with format strings (#545)
10f76a0f3b1f2b234c72fb2e743b0229d520fe60 MGMT-2420 Collect additional bootable information on disks (#549)
c71e780ddd5fc4108279fc8bf32365903f809a2d MGMT-1176: Onprem: configure discovery ISO, agent and assisted-installer to talk to assisted-service (#540)
20be1190c194426f294f6ef9342cbcc1f674d539 MGMT-2037 Avoid dockerhub base images for centos, golang swagger-codegen-cli and postgres (#551)
fdd11d8b4ada79f7e0fa8e64a3d39e22603e0545 MGMT-1843 Publish onprem image (#519)
b052c7a458a560906998117cb5421115491c42c9 OCPBUGSM-18082 - Worker number should be 0 or >= 2 (#467)
78817a56d5dcdd4d5916e179feb4d010a8b9e49a Merge pull request #544 from openshift/revert-471-osher/image_publish
bf8a84269403f7b7864adc7de203985441479cea Revert "MGMT-2307 Publish images per versions (#471)"
e6a19e06268df0df7f0f25543f50f6ba6cd4a144 MGMT-2211 Move next step runner command to host package (#541)
a55041eda96e2b812d0987cc10df4e79981212a0 MGMT-2289 For image generation, only leader should upload base ISO (#539)
38aa88e8d8cb882377d3641f08305742368ffa57 MGMT-2301 expecting completion times on both success and error to be updated (#499)
72346b3879038af0300ada8a0dd63f776811db43 MGMT-2307 Publish images per versions (#471)
47056aada979ba7a45e6181effe0f92cf467f003 MGMT-2427 openshift template: added SUPPORT_L2 (#526)
1e698d5deee2aa46a4315ce900cbd4bb77005b11 OCPBUGSM-18826 wrong validation error return when using out of range prefix (#534)
ccb054109c0163342cc280d9a07ebc975c098125 NO-ISSUE Remove sleep from unit test (#531)
1cb72629a151cea535e66b813dd5e9c17f16a4dd MGMT-2326: Added controller_logs_collected_at to 'cluster' relation in DB. (#480)
6198396cdbd17f549741f321cacb55a067277b2a OCPBUGSM-17572 misleading suggestions when saving invalid CIDR (#535)
65fdea33370f549462809de5db251830db09d4ae NO-ISSUE Jenkins print kuberenetes snapshot (#538)
ad83f5eb2ec78790578b2d97554678b61efecca6 MGMT-2427 use SUPPORT_L2 env var. (#542)
62c1148ae4ed3f52f95c624955ed98c5ac0f601d MGMT-2385 move upload logs from install step to stopAll step, to upload them after agent print install step reply (#527)
cbdf12ce506331bb1e1986bad9d932ad48dff737 MGMT-2364 API to signal next step runner to exit (#536)
c26d9e7a9e5e002784f4e527f5a123ae14865f6f NO-ISSUE Set local ut run db to alpine (#532)
ed2b4f27fff99b4f57a3dcc4fa72cb38a78f17c1 OPCBUGSM-18587: updated stop installation cmd (#530)
a046038de064b6dba81980ca5c10b2fe82ed79f7 MGMT-2377 - Fixing Monitoring deployment (#276)
7f3ab64b4376249bdc5b05a8ce8b39568ce37d83 MGMT-2367 Fix multiple events unit test (#528)
d3a5af0f73132bd3db091cbbcc50a381779bce78 NO-ISSUE adding gitattributes declaring generated files (#520)
374090504cdd15613d02e7d9e5f5db2ce9e2d91a MGMT-2195 Add CONTRIBUTING file (#376)
8c6c7ce63a5e4fa12615e829fd0c30102356e361 MGMT-2211 Send agent command on registration (#509)
92036bc015309f953a9bc0dbc6acf76b16afc287 MGMT-2392 - allow updating api vip dnsname/ip in day2 cluster (#523)
37eb2c338d36a75947c4d94ac617177308449e18 MGMT-2296 Host and cluster monitor iterate in baches (#510)
f8bc63cfc5e8de32fc08f18956582bb8e12e27e7 MGMT-2318 pass verify CIDR flag to APIVIPConnectivityCheckCmd (#507)
1ff1f545ca51ed3893f2bcbf73c2e8ecf0e9a620 MGMT-2270 Refresh installation timeout in case there is a progress (#492)
af2abfde1a9a0407023faff8a452b6c1455ce8b2 MGMT-2189 Update onprem ignition config to v3.1.0 (#373)
a9d29269ecdc80aafd35cde3b2666ad2d3c53877 MGMT-1793 - Allow discovery ignition customization (#310)
d3c304de44fad43cf333e85332cced061c3f426e BZ-1886431 - Remove ignition-generator leftovers (#518)
3740b043863a573e6dfbb7da507a7967936b335b MGMT-2238: Deployment files: Store namespace within quotes (#424)
a5b904aa00bfb01b9640d42ca18b5cb415167a76 Merge pull request #516 from ronniel1/revert-owners
0cbff1e08d9a55f469575dbd51ea394f71ea17d6 Revert "Temporarily disable push to master"
a3df690a892980c1bf06982c73e2bcab36b5d271 MGMT-1990 Added MVP files to showcast them in oredr to continue or stop the work on this line. (#368)
e0ba26f1b69153f00528c020665accc30b40ce14 Revert "MGMT-2283 change unit-tests db into quay.io/ocpmetal/postgresql-12-centos7 (#444)" (#512)
4a93c17704d92972975f9e8bdf6fb362d510e380 Merge pull request #514 from filanov/ut-fixes-master
b6c990801da13f4c62395078d4d43597f9aed550 NO-ISSUE fix cluster unit tests
05dd42a37c673abd6e8f2c0ebdcde050c116b206 Temporarily disable push to master
6556d73f994a800701d60a5e64411832224fd10d PD-648: Wording tweaks (#351)
e61870e93e79779d843ae748b977c7325ac09f6c MGMT-2381 Missed image expiration events upon leader change (#511)
cc56fab1704f164613187e3746180045532eb150 MGMT-2341 Add host hw type to host metrics (#494)
d71789f5f1ffb13bd06c7f54bd1305f51b2398b0 BUG-1886087 adding HostStatusResettingPendingUserAction and HostStatusDiscovery to filtered state for ntp validation (#508)
00d0c314244985330dcdea880d58c9996595000d APPSRE-2377 Use a random ID instead of the commit hash (#506)
7b7cb11038c1a18a109d2ed5c35f23ffaa6ffa9b Raz/mgmt 1659 cluster cancel status (#501)
672ba610467878d6b8ade6299751486c3449306d MGMT-2077 - create subsystem test for day2 flow (#493)
81c6ebea00052f94482b02b88f2e7b21d51f9baa NO-ISSUE Increase CPU limits (#505)
ed23d310c4e3d72541d518c24e76dbc2b2757a4a NO-ISSUE add merge back to commit check regex (#504)
9d121b2df4c9b73d26d31cc13fdf7ce89dea60b8 MGMT-2363 Add clusterId label to host related metrics (#503)
e096751a5383c239e524b3938098486ec3071568 NO-ISSUE Remove prefix commit message checking to a substring check (#502)
6fbf08a436ff6fdcfe81f64dfc2b0d6f34d44269 BUG-1885920 failure in host logs download with presigned url (#500)
c17c5da682a0edfc54f1f1ee3145d14edd3fffd1 NO-ISSUE host: remove redundant debug log (#491)
b7f400d9ee810503ff6dbd58f95ea66f54b161b6 OCPBUGSM-17571 Block creating a cluster without a pull secret (#498)
19a7a52091365dbc9da31c80e82f6374f10ea4be NO-ISSUE Increase unitest timeout to 20 min (#477)
1ff6644f1d35351d012edf9fdfffc21492092d73 MGMT-1710: trimspace around provided pull secrets (#497)
06defa2cecffa66306fda01d29653ceb701405d8 MGMT-2372 on-prem subsystem tests broke after livecd.iso was renamed (#495)
d66b40982f800ff84d687b3fa3c38bd9c0572943 MGMT-2359: return forbidden error code when host in installing-pending-user-action tries to register after passing the reboot stage. (#490)
b413cedf127753ace7bc5870978ce6b911c20743 NO-ISSUE Add build-all Makefile target using ASSISTED_ORG and ASSISTED_TAG (#485)
db25814995741778ca1efef25f64bd2d43ac92b5 NO-ISSUE Use infra_error for all 401 and 403 responses (#335)
14541283deacde6c5b10f74957e6d66458d5704c MGMT-2357: Return an error when the cluster is not found for upload logs (#463)
46acba81198d57c7bf895505d763727f41543ed3 MGMT-2128: Change log filenames, including for presigned S3 urls (#410)
f23730c0375d8de0ace5330443be94562879304f MGMT-2288: For image generation, call copy parts concurrently (#468)
352fef154311db14d3b51f6841ea70677af58dda MGMT-2342 move ntp validation from host to cluster validator (#488)
8f900c19d08256fd8ec2261488a6da2e039cf3e7 MGMT-2329 - update OCP release image for 4.6 to fc.9 (#489)
b72737c95bf66cd7ee537c8afff754f879dcda4a MGMT-2314 Add cluster_id label to cluster related metrics (#473)
05096b6ffb5014526a57187697cf3f9fe39e3159 MGMT-2271 API VIP connectivity check (#450)
088207ef51b053ae6d6fc34729448259da3e5bc5 MGMT-2138 Added asisted-iso-create rhcos image download back (#486)
5e99ca8078256fd4e12b6270681e5cc6eafae262 MGMT-1755 Setup TLS trust on-prem (#255)
3edebbbdc705f0d97f44b6dd0c87a45d50e080b1 MGMT-2356: Update livecd name in S3 (#487)
bd26ab1859fcdfe34f36e4f660b5d8992c06436d NO-ISSUE Verify minikube before Makefile targets deploying to minikube (#484)
e485ccaccb010742bd13c395b1519b90de2d5f2e MGMT-2182 Add event on successful cluster registration (#483)
defa93e0a45e2ffeeefd0af8640348c90b6acf50 Igal/time skew validation (#482)
50b60a9713b7bcedc1dd085b31686438d5597b07 NO-ISSUE Use errors pkg instead of fmt.Errorf (#481)
e540e7b74e950a08aef0cd147ee6abda67e56998 NO-ISSUE Update Owners file (#479)
58477a1e17f5fe3d5e7e67ad70d290722e28e33a NO-ISSUE Use gotestsum tool for testing and publish junit on Jenkins (#456)
ab7a7aa25e81f75435886b891b02a10cb9b4639c MGMT-2328: Always require users to reboot hosts on reset.
eae4e47dcf9911928c5209df5dc906529c08aca3 Revert "MGMT-2230: Implemented authorization by scopes (#460)" due to wrong commit message
61dab3fa39189880f9369751916fc20d71c8fa0b MGMT-2297 Cluster monitor should filter our installed and clusters in error (#475)
3c89196958d865b4d829f388d20bdf1b346c4b32 MGMT-2279 Pull Secret validation -  Auth disabled (#470)
6a9e00d3408b093ebc6ee370fde0e0625cbbc1cc NO-ISSUE cleaning vm pre build (#455)
2f2f6960d06572bad9d8f2c21b996c20261f4e06 OCPBUGSM-17732 Add timeout trensition to host installing status (#446)
c12cf2880e561e0daa11dea3818ab054619e94bf BUG-1885001 Register Error event will show internal error (#474)
60c69c58e00cd109e411a8ff216beecd8d1d0e0f NO-ISSUE: grammar fix in log messages (#418)
e6c9d6e85290d8e34adfdf4d79c2ca27b75cdf3f MGMT-2230: Implemented authorization by scopes (#460)
ef78e6735113d12a08df298bb18e12f66f6a018b MGMT-2337 Remove create, delete and monitor from job API (#472)
d539663747c34d1cc61603074955d3f4ea338362 MGMT-2240 adding time calculation to auth, register and update cluster (#416)
b2387026ae90998bae36effc0a67025918bf6ca6 MGMT-2075 swagger: API connectivity check request and step (#425)
fa286d1bf46caf9ef6733f652224b6d3ecdfd85b MGMT-2072 register cluster - use adding hosts status (#459)
ab8ee02fbb5ab0c70b385fddd7c3b7c596126dec MGMT-2148 - InstallHosts imeplementation (#465)
5486a542ec0e92265d2e5cb2e65c05cde0adeba2 MGMT-2038: Make for-update transaction in enable/disable (#462)
bc38637567b26c3daa98dca10db278893c096582 MGMT-2252: Don't log secrets from the ignitionConfig (#464)
0cfb84ab9a5722cc8c86efe96f2580fc433b9318 MGMT-2052 - Patching OPENSHIFT_RELEASE_IMAGE variable to make that customizable on the Assisted Service (#443)
7790f3b19528a79fd63df5345b01cfb4860f937f OCPBUGSM-18341 added upload of install-config.yaml to s3 to ignition generation code. This file must be available for download on cluster installation. (#461)
0c3f9290530fd881e0a7b0c4944d5a287bb25956 MGMT-2292 cache payload in UserAuth flow (#445)
88fdbf500d08eea8c719aef38205c5704a1567d4 Refactor ignition generation (#454)
7cb480d897401c986e7d0ca3d7dbb5fb3bda6d8d Avishay/mgmt 2287: For image generation, cache info from base ISO (#453)
6d84a2ff83f859928edf594e1a16fdf5a74c7618 NO-ISSUE add kni-projects team to reviewers (#458)
c05110c76426df9ce4d1c876af1a86a781062c34 MGMT-2073 - implement host/cluster state machine for day2 flow (#440)
2ca06e5f827620ec720e91b7af76825a73e0edb9 Eran/bug 1883887 (#452)
a0cf150a6df83220d022ce670613d28772c73358 OCPBUGSM-13814-Extended-ssh-key-validation (#412)
f2d9619d6a32300e2560194229a3f6dd9b1608ac MGMT-2281 Configure OCM cache timeout to 10 minutes (#449)
bc77fd1ede9267cdad76c01f8f0afe9097709497 MGMT-2282 Create a random name for the initial iso job (#435)
f9066dc89ae2f609ada80ea6ccaa6357108f493a Igal/controller logs (#442)
d0132974c15c8970d7335f0959d0c75f3df753b4 MGMT-2283 change unit-tests db into quay.io/ocpmetal/postgresql-12-centos7 (#444)
63e9e8838db483d0cea2318a27a4c5f21d4f9265 MGMT-1944 - Add cluster Id and host_id to API logs (#375)
e19a247adc1a3c062d2b912630e55388223aea2c MGMT-2281 OCM Client connection reuse (#434)
2650ff71e8380d787155395e0bda24a46ce216dd NO-ISSUE Revert "NO-ISSUE Verify minikube before any Makefile targets (#431)" (#439)
eeae863733803cf8befdc0fb1bc797703640bf4c MGMT-2072 - implement day2 create register cluster (#427)
1d23951e9269e59684e2cd9d89a3fe5c9241d27d NO-ISSUE Verify minikube before any Makefile targets (#431)
617b2653fe82b78f5c9dea6655f8e555e29ce543 OCPBUGSM-17629 Revert "OCPBUGSM-17629 Revert "Move Agent Auth cache to AuthHandler (#401)" (#422)" (#433)
b18442a675a0e3cd64a705624bfb6733429fe07f MGMT-1743 - use smee to proxy requests to run the jenkins job (#371)
389017e9759883e438778bcd0046a268dfdc3239 OCPBUGSM-17615 Installation hang on Finalizing (#388)
26822a49b4cb6f5aa29efdb6120397490330e403 MGMT-1970 Set DHCP vip allocation mode as true by default (#429)
f9dc682fbe7d38b70b08554b18ffa9007a306ae7 MGMT-1987 In DHCP mode, auto assign machine cidr in case there is single host network (#381)
25f22343525fef7f532c08651a7eff9abf17e368 OCPBUGSM-16309 There is no BE DNS name validation - fix calling location (#400)
8e0c0516e6573c374475967e07cd43cacdc9e9b6 Fix onprem subsystem tests rebase (#428)
935614482558917eee7b50d966d5dbcaa143484d OCPBUGSM-17629 Update OCM SDK for SSO retries (#426)
0eddabf6141cb6612a40f6c75334bdb753fd3611 MGMT-2187: Optimize image upload by using UploadPartCopy (#392)
d7d4a53ee8edf3fb56c947e483738ce642ef3d2f MGMT-2239 Fix occasional failure when cluster is updated with "nothing have changed" message (#415)
ce04dbbf3b3b5cb3af2825718972c56204d483c6 OCPBUGSM-17629 Revert "Move Agent Auth cache to AuthHandler (#401)" (#422)
827e0de35acd7b7ee9a6bf40815c7a7de6e8eff0 MGMT-2249 Add the old default as the default for the parameter (#421)
011d2dcad0540d6bd72876148d94ce37a8dff643 MGMT-1802 ports ignition generation from python Job to local golang (#185)
27cfe0da424cc8837613517378256ce528d2ab2a MGMT-2249 - Add the AGENT_TIMEOUT_START env to the deployment template (#420)
7fd51db086763350e21512b794158c9b706fbf81 OCPBUGSM-18040 Cluster installation fails with error : the container … (#407)
cad2ecb15484684434307f3556ce6ef6597880c6 OCPBUGSM-18042 Agent unable to start container during discovery (#406)
691bbbfe74311c53fe5dcf92c453b3f5a36abed2 NO-ISSUE: logs the correct error when leader election fails (#408)
b58eeb97d6a87ed6a6d670928c99faf812acaac4 MGMT-1734 Add Jenkins stage to run assisted-test-infra (#268)
de3ea464ff50771e34a2e11928daefe8b353ce68 NO-ISSUE Removing pre commit ci lint & Add GH issue as as a valid commit message (#403)
8bd7f4bd01bba7d601620fe14a21e3a5ba7a1d75 OCPBUGSM-17629 Move Agent Auth cache to AuthHandler (#401)
95df2f9dbb60a325c9b1486e8f53958f5be93e68 MGMT-2070 Set OWNERS rules for Jenkinsfile and Dockerfile (#399)
05aa9ca28d042970cccc15df7b54f147b8c099a7 NO-JIRA improves commit message checking (#389)
e4f63c20f34c32d28092c4484dc75808fa2d75aa OCPBUGSM-17629 Handle failure OCM call for IsAdmin (#398)
9f3509e50cf54ff2a2f8c7391abcfe401c02e1b1 MGMT-2217 Send notification on abort (#385)
6712278c27933ed9e4a901820c17d7401df2c366 MGMT-2223 - Add request ID on Auth failure (#394)
97f808d90e9ea85fe5ff4da4dd250665214d79c1 OCPBUGSM-17903 In DHCP mode VIPs are not updated in database when cluster is in pending-for-input state (#391)
d2acc8dd28aa30fcc4f17e4e914516413807a710 MGMT-2192 Use refreshHostAndClusterStatuses as a generic function that refresh host and cluster statuses (#393)
b793c526a1687a3181d657d8feb0196a414ed48d OCPBUGSM-17301 Node fails to boot due to tailing enter in the SSH key (#386)
0d78be94ebfee5949bbbaef7d36df188258ad7e7 MGMT-1837 updates, Remove default progress state (#349)
cfaa3b131f6207781d4f9ea29198f15467510a85 MGMT-2016 Delete logs_uploaded_at on reset cluster (#384)
f4dc3e15b6551b3d892d90f8e7227e2bfa288533 OCPBUGSM-17295 Set HTTPS_PROXY to HTTP_PROXY if omitted (#383)
3a17e7a34e6f0da48504706a3de72ab1eb3e5275 MGMT-2181 Check status from ocm auth client and return api error (#377)
85291e49bd897e83c36ee07eafd33427f72130a0 OCPBUGSM-17700 No event is logged for installation completed (#382)
823bc1cdd5086e665152b3f2bf182eb8a8a6df54 MGMT-2019 change back default log format to text (#379)
553f6899e27f4e22895c9b3a277dabad9ee5f013 MGMT-2215 Increase starting timeout for assisted-service (#380)
55c0e659b0f9f7fda4153e635fceeb6f8211a757 OCPBUGSM-17536 adding lock for automigration by using leader election (#372)
e56d3e509353ece524d064c90f38632c2f1962d0 OCPBUGSM-17629 Filter cluster in "complete_installation" (#374)
7e8f6119d80479a3f72faa9ebd98db4027e09539 MGMT-2153 Add commit-msg hook (#370)
60a1338c7ee3854e7b6ae21f159018c7be8c5a9f MGMT-1776 Pass S3 secrets using a secret ref rather than plain text (#119)
031250031ea626cf535cda6e744d7b10e1b00c25 OPCBUGSM-17520: added noop transition for resetting-pending-user-action for a disabled host (#369)
12eb214183c9f7eb7f58debcbbd2273bc3da7198 MGMT-2170 - fix the mapping between machine and BMH (#366)
f7df479d879ceb25119b470a8fc281f5fa02f497 MGMT-1015 Fix date format in Swagger APIs (#350)
760bb681eb7eb31df50f66c16c21cb6d400357f3 MGMT-2153 Enforce Git commits formatting (#348)
13d8e23fc2226130e19b25d93bf79cad84925289 Add eran as approver (#367)
5dbf46840f6d1f1e04caeeb5055ff7a366c6826f OCPBUGSM-17431 Fix auth error reply format and return 503 in case we failed to access ocm on agent auth (#363)
70e5cc16534500822320caaae895ceb378d6b536 Update OWNERS file (#365)
43693034cfac1291d35a080fa64ecece8b50669f OCPBUGSM-4577 to be installed cluster need 3 master and at least 1 worker(if workers were given) (#355)
6b147e99138834f855fdc9af5f444472465b3270 ocm client: support OCM_LOG_LEVEL env var (#359)
e900640ead5869f27e6749214a26fd97f090ac07 MGMT-2051 - remove v4.6 workaround, UI is ready (#354)
9cf1b17a062ad3ed3dc5bd82f97cfec260e2d449 noProxy in ignition should be formatted as array (#364)
9b7f33317b3139e2b32855a2978286830e67c59f Pass proxy settings to install command (#362)
87de489697859806845691a128e6b7f7d2ca6ff3 OCPBUGSM-17486 Logs - adding date modified to tar files (#361)
b8ac4f419201c445ad5aace05bf0177097cbf88e Making app-sre-jenkins job fail if the scripts fails. (#357)
2f8244f5723b01355ef630d74c50349dcc355e2e MGMT-2037 Use quay.io images of wiremock,s3server,postgres and grafana (#353)
f6ae92ef03483f844619910684626ff3218cd639 Add FOCUS to unit-test target in Makefile (#313)
b2bb4401c6256c6f59557919074f3c2d6e8a0e9b OPCBUGSM-17442-fix-enable-host (#356)
a63552a1ba5c42b410e356282ac2f4bd21cac063 Make it possible to disable route53. (#352)
af1213d19636016f2400aee168ad182339aed3ce MGMT-2115 Fix case for failure to convert hosts to connectivity params and error message is generated in log (#347)
e9d1a4645363622e7904eb173d01b4ba50ec174c MGMT-2133 Add leader test to subsystem (#328)
6a3fdb3bb8c773c1b1425c9fc1bb07e7884f918b MGMT-2151 Fix formatting on Agent Auth error (#346)
45ba8f0a0c4122d5ebc40dd73a6698d25479646b MGMT-2152 Update Jenkinsfile avoid overriding pod logs (#345)
e9f86103fb322f238e95485f075758f9e2df5424 MGMT-2147 increase image expirer timeout to 4h (#344)
a47bd21c71071f6f6d2fefa18b2b963cd4db191a MGMT-2120 Avoid updating same installation progress (#331)
6b166304ed6a92dbd117c2a4d514d507011fcf5d Remove require true for REGISTRY_CREDS in Openshift (#343)
20dade9036b5b7af4489359ecaa64047f3e696f1 OPCBUGSM-17391: cancel/reset from installing-pending-user-action (#341)
a4b7be67bd3d7c7dbabc5af841e89c8125daae0f MGMT-2012 Handle DHCP lease allocation timeout (#318)
3338ff5be24e35445ff9d18b5d63ea4044eecded archive log artifacts (#342)
1bef497979eb8408a6d50b3c465ca39b85dc861b MGMT-2019 Json log format for assisted service (#329)
840bc0fa92bdc62406f48cec3d2baad069011b20 updates comments and errors to reflect use of tar instead of zip (#339)
dc344dbf7fe8689ef0800c35ef676c4806f7b480 fixes three bugs in pkg/s3wrapper/filesystem.go (#337)
2a80a634547f4a7cf1a78b815d5e904262dc65a4 MGMT-2030 Add QE Registry Cred to Pull Secret (#320)
6a9706a4ffdefd40163f52b91661893f9de3653b Igal/cluster logs fix (#338)
ebf48b3a763e468d875734b74362d5dcb360a263 Changed livecd-iso to pull from ocpmetal (#334)
990e3e0c8e81b492665d044c569e21f29869d928 Revert commits (#332)
3bc7ce4a2602ec476b722f92f4de775ecb20bc33 Add missing parameter to NewBareMetalInventory in test (#333)
662603f257481339b2e73c57dc2aa491f6dd1fb4 MGMT-2043 - Implement GET /clusters/{cluster_id}/install-config (#288)
3f196257e2b2b6ece79a09fbbbe19da79b937183 Adding missing parameters section (#321)
23880268114caef91f74a5506d11270c1bb0b8d7 Fix flaky unitest expecting event (#330)
5603417fded9baa3e01eab074a9051e8ff36be72 Set client name as other functions (#323)
1be0f8277ed5a9e3d1322db0a5cad833215999f8 MGMT-2027 Update onprem build dependencies and Dockerfile (#289)
d3fdfb9ad7e95e3ee32bb21981eafc525e3907a9 Use common error function (#327)
412f7411dc873c64f963bcda9b6f947f2746dc2f MGMT-1837 Reduce timeouts of hosts during installation, according to the step they are in (#304)
29b6df3b322a09b0a0cb0030850391a7b7b884dd Fix issue with iso creation due to missing build arg (#319)
39d28ccd4eeefa8bb0c9a4b1d185427b2e4001bf MGMT-2130 Delete permissions for leases (#325)
72a5e6f89a3f208cea1a9f9c656a9b1f5e0b662b Add pull secret validation on create cluster (#281)
a90b3c3555439a6d505af5262633c99499ec0171 OCPBUGSM-16309 There is no BE DNS name validation (#308)
9f1949be04c7c299c02bb2f10dfdec166e4c6cae Add SERVICE_REPLICAS_COUNT to skipper.yaml (#312)
d10d6ea4c78f699dc15e6781c57c8fb658c8a7f6 Format discovery ignition json (#322)
9672bc0ab4217f9ef14eff7ef8fa40d42cf06724 MGMT-2120 Add progress to an invalid status log in UpdateInstallProgress function (#316)
3d2454ba388c23bf59b9b6d65880c985c732cd8f MGMT-2111 Change configmap permissions to allow update only on specific resource name (#315)
7c4f7ed3a3ec4547df4498a7af7570c169c4d262 Added livecd iso creation files (#303)
a2a61f93f35c53d0275696379bb69900ce3babd4 Adding RELEASE_TAG to openshift/template.yaml. (#314)
7e8cd9564c3f0d445201ffddc800669b65a5660c MGMT-2099 Fixing skipped status on subsystem tests (#309)
74fa0df6cc3742ef23dbc93369fa9f46cc040a47 MGMT-2038: Refresh cluster/host status on enable/disable host (#311)
5d7f301f621f5ab3731a57830fd3916685fff769 MGMT-1727: subsystem tests for auth/authz using WireMock (#203)
932ba82be93f0e2fe511ac6ff8e74b5f95005fa1 Prettify Jenkinsfile (#306)
4f6a017793d43b41cf143d2a4caaaea22cbcf717 Adding post deploy Job to trigger external CI (#299)
32f6a0bbd4933a485120e2a4ab4f77593a8504bd MGMT-2030 - Add Red Hat IT Root CA to ignition (#291)
0c9519665d82ce424d7af6f7f8a3e3781e608017 Adding REPLICAS_COUNT parameters to openshift/template.yaml. (#223)
4d9ba788c7bba597ac01270514d5d7f0b2cd6b1c MGMT-2041 Presigned url for cluster logs (#302)
795c571633498cd1a1b90a88dfba406c860a8648 MGMT-2084 Connectivity check should not be invoked when host is in discovering status and disconnected status (#300)
594b96368e75c70414c4beac709953d3477b1b7f Igal/leader new (#294)
f0172a8c509c97bc4b9ab738b6ca1a3a657ef863 MGMT-1591 Substitute cluster status consts with swagger models (#298)
d372dfedddb352dd5267447fea860105c63055d4 Substitute host status consts with swagger models (#297)
739cc5e932ffaa1aec1cccdceb8c154236519fc5 Fix subsystem test as a result of free addresses removal (#296)
553ddd249cb3f0c2db929d6522960822c9bd1ac8 MGMT-1826 Clear host's free addresses field becuase it is not needed by API users (#282)
43d487ff2658e760276405d77f074bcc4b0a6bc5 MGMT-1707: fix installing-pending-user-action event log (#280)
8ac0e2d530fcb1313d76504b28790a8d6e184b76 use ocpmetal-stored 4.6 image (#292)
2e3fe7a0d87814bccf47bcc68e3761d00ccb160d Raz/mgmt 1685 installcmd installation timeout (#290)
01d9152b460a5e800b86c1e5fbc1bbf4ee43eda3 MGMT-1621 - update ignition config to 4.6: do not set provisioing int… (#191)
00d3ac3e82d60e4e7856323dcb780b654af76c8e MGMT=1918 Validate hostname validity on the backend (#260)
888b1a759030a0248b988055ff7b471745fe15a6 Use proxy for discovery image (#287)
b83fbd3f1c8ce03a99fa3a7967e4857100ae3a2f Kill insted of stop postgrace after unitest (#286)
cf7f46a027835b9d1d1d0f0c3440b239ddde3d9f Igal/stream logs with upload tar (#272)
a72eee6d314362406f63b8984f548b8e73309abf Igal/presigned (#261)
208ee051ebf7c45f92833d9220c0467af0d60af7 Fixing base DNS issue when trying to configure route53 to a cluster. (#270)
571d75adba73ee653b160ea5e9691ef7224d9077 MGMT-2033 Add agent image to the installer command line. Needed for log sender (#271)
f0301697793875c8ba0cc171da1e0b92d070de28 Merge pull request #275 from ronniel1/ronnie/jenkins-revert
5bd95dd6f1195d49aa5d93f8a6bac5ba36c3d36f Remove omprem subsystem from Jenkinsfile
6b39652ff43206e1e8957742ded7861367182f5b Wrap logrus logger to OCM SDK (#193)
ad5d32b3eff968fa4c6fd6cc48d8099538c4fa8c MGMT-880 Add LOG_LEVEL (#263)
44dff4e1c86b87e758d2cf2d072ea958c33b408b OCPBUGSM-16641 Add UserFilter in UpdateHostInstallProgress (#264)
1eadd7e513e2d21243b2f08c08f828780d86c2fa Restart minikube when starting build (#269)
9b7dd997c1433ad097ddf6570bd3731cfc925e84 Moving Jenkins pipline to run on parallel for k8s testing & onprem (#266)
2fd5cfb832e2804d31dbe9ce58f66b8060dedfe2 MGMT-2023: openrm flow fix (#265)
88adb4ba968e1199675afdf7425032c4144ba2ce MGMT-1883 - Add update cluster install config api (#230)
1eba27a85dd3c298f424e9d8cbe2598b8e200dd1 MGMT-2018 Advanced networking additional validations (#262)
cad2f91e5fc6c9c3997da959842c4c9dba12027c MGMT-1940 Fix token parsing error format (#258)
07cde14243e32ce1578cab7815ec7f27e2a8990e Consuming route53-creds secret as a volume in openshift/template.yaml. (#259)
1eece26dd56622fb8f50b393ab654574ce55aaf3 Raz/mgmt 1951 add reset cluster timeout (#244)
882a49e166721e44c4d13eaa73fce2c54afb20ea Fixing build_deploy.sh. (#257)
64ec6c533180eae922a89aa1e13531ecde5d3146 MGMT-1937 - Adapt validation messages to DHCP mode (#256)
681d571e9fa16e090eae704ffb4c999103b17fc8 [MGMT-1982] Proxy value must contain a scheme (#239)
82d0607c9515d40b9f4c8d2704d38705b8a998a9 Renamed image name on quay.io/app-sre/. (#238)
5f8695916e3991601d3ce6038cd96a69cc427fdf Raz/mgmt 1685 (#168) (#237)
3deb5465bb7a5aee0687f7e58a715641f5312ff0 MGMT-2007: Removed preparing-for-installation cancel/reset subsystem-test (#253)
ea8d280323e8a5401a47fecb94048ba84c0d0146 OCPBUGSM-16612: Handle MethodNotAllowed when updating tags (#252)
7e4578676064108e583e79ab55218b9c34c09bde MGMT-1955 Create event when vips leases are allocated (#246)
15faf93471230fad2a63cdab984484c0d63876fe OCPBUGSM-16649 - added missing target argument to deploy_sso_secret (#250)
f239a85fc64f2093c198a983b2c62098839d0ccc MGMT-1998: Revert "Raz/mgmt 1685 (#168)" (#249)
5a475fb3fb9e57d8626b1934777b57cca072da16 MGMT-1654 Remove debug API (#247)
35c7b2b6b304f04e3263953c9a37ab955868f44f [MGMT-1984] No Proxy does not support '*' as value (#245)
2d96a0af33b6525527af37113fdc4498fe62bd55 MGMT-1685: Fix installation timeout deployment in makefile (#243)
6f45701a30baa08c2bcb858f6a958ff00a20df52 MGMT-1961 When switching between 2 machine CIDRS in DHCP mode, VIPS have to be erased from the database (#241)
cd7ddb95cc25054afc19b5040962431b878a639d Raz/mgmt 1644 (#187)
b73df402143043afe9811fc02afe12aaba5388e0 Raz/mgmt 1685 (#168)
de324a38036abc28a2709b2543227e60cbf29c9c OCPBUGSM-15826: Rewrite status infos (#166)
2f0da134c290b592f409ae6f700bb0a5814287f5 MGMT-1844 Improve errors handling for Auth and Autz (#164)
75fbba18afb7706a1da324ca61986f1c876e3c74 Raz/ocpbugsm 16238 (#231)
058a96f242c32874d3465c908a17f0f1c116fedb MGMT-1950 Bugfix race-condition in waitFor subsystem functions (#226)
5a78ea291cfc2e977357577a6365e4da50d56ec1 OCPBUGSM-13814: Added SSH public key validation (#233)
709d6442a624dd525f78bbfb0bec4fff9c039ce9 OCPBUGSM-15827: Severity for host insufficient status event should be warning (#148)
0a97c027f287d78859bc06437db4e19308e9a418 MGMT-1506: Return minimum host requirements (#198)
70874e1a55e20edd5861b04144043c65871afc34 OCPBUGSM-16205: Remove empty parenthesis from event info (#232)
008a36b844f6c15bf28dae64df74b9073053afae Fixing build_deploy.sh and pr_check.sh. (#229)
324a9d8ff263908cf13b2b4e37cf93df2b0b0c76 OCPBUGSM-16477 [Advanced networking] Illegal CIDRS not verified (#224)
1ef0b1eb3a4784380eb4bd7512b3b22463421a5d Adding 'liveness' and readiness probs to the deployments. (#165)
5482f9792ea155906d526f232a7ad64bf9f4e7f8 Added image building to pr_check.sh. (#222)
dadeaadf602d99139487b59935d8d450781e232a MGMT-1792 add ready api to assisted-service (#218)
a90d8af52a6148d8422976b9ad01d7c3b180c36f Mgmt 1680 Add agent version header for agent API calls (#179)
65872e32a3298fbaddfbbfb93cda8cc242021032 MGMT-1849: Delete PVCs on clear-deplyment by flag (#161) (#220)
628817ba756e1449228895d9dfbeb9bdfc1d393b MGMT-1865: Add 'force' flag to job Deletion (#208)
011fc82debcf84cf1ad2b3f64e8d408bf4eb4c22 Changed the TAG of IMAGE_BUILDER in openshift/template.yaml. (#219)
20efdbb2f054c6236bba330c05e6bbb3d7fd4bd7 Updating the value of SELF_VERSION parameter in openshift/template.yaml. (#217)
88c0423ac7636a80be54c433340b516f1ba91a54 MGMT-1864 - Validate advanced networking fields (#194)
af4758a42cba7f905675c34d0384fedddbda238c OCPBUGSM-16347 delete ingress configuration on cleanup (#209)
ba1422ae556f2774f026b32711be1999246a1912 MGMT-1924 Remove severity of logging message when a host does not belong to machine cidr when checking free_addresses (#213)
8d758cfaf6981e06a5bd1698a5449e39566bc57a  MGMT-1923 Notify and fail job if minikube is not running (#211)
a8fc8bff50468396d354c9ad94bb546277b5e47f Igal/upload logs (#207)
e3743b2e40ddd381817cd579b2aba26eaab7bee5 Wrap JWKS and OCM URLs with quotation marks in configMap (#101)
de3a2888c8803dc288744f902be7ac9d1a0f85cf Adding missing parameters to openshift/template.yaml. (#212)
62dd595f950c329dc220234530439c7f3ffce78f Add -r option to xargs (#210)
d70c2b94413a784aef1d0a5c56eb71ad8dbaa03a MGMT-1450: Fix auth.json path in live ISO and FCC (#184)
6c2dd870665d972f4eb4057c0a1e0d0690b7a6c8 Revert "add link to notification" (#206)
5c8a396599f1903fb65b039666f9e928562cb51b Fix docker installation in build image (#205)
44ca24ae5a9769ceea060b7ba990eb8562d35702 Add debugging info to update tag failure (#204)
6424b58f25bb9c46608fd7a946cee7f327d90b7c Adding 'assisted-iso-generator' to app-interface. (#197)
32f9e0745048bec8f3b42322d081421c7176d875 Add slack notification
41667cb1e52f980ab980cd2d9d0f745bb40e0e09 Replace print with log in UI deployment (#200)
e26d1f0e2eac586eba97e33e2e64b19c6182e20b add link to notification
c881326c5f52f3e3298bae5bfebfd2cdde17280f MGMT-1723 Run UI yaml generation directly (#199)
396c9f8701e69f705349bc1327b091d0d241457f MGMT-1867: set user_name as 'admin' when auth is disabled (#159)
bf43908e4385589ee1ed99c556811f093b7d3a75 OCPBUGSM-15906 - Cluster has Ready status although DNS domain is not set (#178)
d6223a5cd0efbf57cc735d9bd60b3400bef1fc52 Mgmt-1768 Cleanup remaining s3-volume (#174)
55ef9784fba7a894907fb3ce0cbb0a18f04afaaf Revert "MGMT-1849: Delete PVCs on clear-deplyment by flag (#161)"
3f53620644be27b21deedde4c50e26b178f08bfc MGMT-1849: Delete PVCs on clear-deplyment by flag (#161)
fe691804453808f910373812d48e9d82454b6f5a OCPBUGSM-16154: Fix image expiration event (#188)
76c85fa5429debc5c9d764a198b9e673a6684a26 MGMT-1678 - move installing to cluster state machine (#192)
70daf8fbc52dab11a713924fe2ad0c0a210484db MGMT-1792 Move dummy iso generation to main (#190)
51ca9e2028d55530fce5f79d019ca216fc586a88 Add service name to notification (#177)
888a07a981b615b0c8998fcaf857f2773e311c94 MGMT-1903 Add bootkube to uploaded logs + code refactoring (#189)
02697a65db48dfc89b9a5763ef3ea73cad73cf8a MGMT-773 Auth Handler test enhancements (#70)
c60b3a5ce412ed22526e26266e21c5d98548f0a1 Use Token Auth via OCM SDK (#155)
39257efe5e72395c6ec4ac61898721e9c97a96cf Revert "Igal/upload logs (#128)" (#186)
f3c40c11cebba56520cbdf4fe142df130d9ed1c2 Igal/upload logs (#128)
c97cc22389180e45acf9e79902db03abb5229149 Improve on-prem documentation (#120)
0b406fb2d976b993b30214b59544177540423d35 fixes error when re-generating an ISO for the same cluster on-prem (#183)
8095be475c3c55deb95fd0943efc29e03e11e91f MGMT-1450: remove s3 from live ISO (#181)
02dab0583aa08becbff2c2dfd05c95282605a70f Hotfix remove mistakenly discovery image iso (#180)
e44e64bfbf07d016b72adb5919e3d4dcd391908c MGMT 1450: Create assisted installer artifact to run on-prem (#175)
2b2afab3356d241433c40ac0d5a8dd63da4c7e7a Raz/mgmt 1245 (#172)
efb51577c1b50b7d7c5da55f59222c20c405c1d5 Revert "Adding 'assisted-iso-generator' to app-interface. (#156)"
fdb29efcc1f2af5a9b5581311ee1c17e20726e50 OCPBUGSM-16010 Add UT coverage to cluster refresh (#176)
a39818f2ea3a3d219287c9699347bb33579c6694 MGMT 1768: Create and use local filesystem implementation  (#151)
f221dedbab3dacfe67aac927fc2b9568de4daf2a MGMT-1859: use CapabilityReview via SDK (#157)
85f2a590413e3f95d5362a6b27c5fdc269646e97 Validate Proxy settings (#171)
95325d0ac8aad408086fe7783cbee8cbab0985ea MGMT-1863 Get preassigned url to download logs (#167)
26be30904d6526cdbb9924bcf8e28281d025825e MGMT-1877 Wrong image for dhcp allocation containerized application (#169)
511e948419c6f691293dc09f8dca096b95b03687 deployment: change aws mountPath (#107)
ad4c7b1332fdd1185c2722ac6213ac42b86b014b Adding 'assisted-iso-generator' to app-interface. (#156)
676bb1934e73728bc64cdbb0351858fdd90e4460 MGMT-1838 - check assisted-iso create during subsystem from local image (#160)
a294fef29e2cb68932586f752c251270af420378 MGMT-882 Enable deploy with HTTPS without cert verification (#143)
8411fdededd6114069a52fdb7e3a33a50002bc6e Let the DB time to die before restarting for the unitest (#163)
273f0d793132af2df57e579f24820ab170511aae MGMT-1855 - Logs spammed from UpdateCluster (#162)
b74ae00e8bc8747fa1d5e3fc7977cbb7312f3979 MGMT-1577 auto assign host role  (#104)
07dfcb9f7055f29fd048af90f6cfb168d6e98636 [MGMT-1828] Generate new ISO after proxy was changed (#141)
a26ab6f8f19e5a7213162e2ce52b5436feba8df1 fix master branch notification
7214f27f44e2c8efe17c13a34c07e0d50e45b113 Igal/download logs (#150)
916203d5e7b1c3924b3b63ec4d867faeabca8eed MGMT-1834 Subsystem tests for DHCP, and some bug fixes (#158)
2ed1b5a67f91f9e611e279298dc184970f19f498 MGMT-1858 - subsystem should use dummy ignition image and not a real one (#154)
ab94f187ac43a24d31dd90349f01832e3c946bb3 MGMT-1667: added minikube profile flag (#137)
73b28affbc9c55eb83806b8dd8f621644bf076f0 OCPBUGSM-13634 fix clear-deployment to delete configmaps as well (#153)
e3c47705fb97ed67fc10c982ddb88fb0fd7d7b74 MGMT-1430 - Authorization support with AMS (#73)
56a4f040d500a3ccfadaad82c2442198cfc8fc3c OCPBUGSM-14226 fix subsystem-clean to remove correct pods (#152)
975ec36f5a7f5cf13f7c37dbdb8c76e65baa7e53 MGMT-1833 Change cluster and host state machines to adapt to DHCP mode (#144)
6b9d3c1d5a3902967318f2b4b7c5bdc2337c7f58 Avishay/ocpbugsm 13596 (#124)
23c70cc4dff007c33f98c8f4be977561204316a6 MGMT-1759 add notification when master test branch fails on jenkins (#149)
d05cf2468ba16fe371541d44c4102f8e53cbf047 Igal/upload logs intaller (#147)
257d160c68f326a61520432d9331ec8fbd9a6209 fix subsytem test install cluster requirement (#146)
52c5f3e97578df5127f77b83d8528295741ebef4 MGMT-1841 Increase wait for service timeout (#145)
e185e8c840a2106456f5c0824adc72acdc9113d6 MGMT-1677 move preparing for installation to cluster state machine (#139)
e70af7dcf59763ee6c697fb409887f00ab5540f5 MGMT-1839 fix adding query_option to db pointer (#142)
3b181ab2243695887dd8fa6ada0a0f6565358d2a MGMT-1720 Modify UpdateCluster to handle DHCP mode and machine network cidr change (#129)
5c7d206740a257ffbb6edfeb657d0f60bf8125a2 MGMT-1835 - change iso creation image name (#138)
c1f4618e10daf69cf4e0031a9ece5aaea9565f0c MGMT-1836 increase subsystem timeout to 30 minutes (#140)
931bb06eedc3afadeb1f6c11881bb23b8c0a9189 MGMT-1801: Store image with .iso prefix (#127)
8458233ac0391985e8a2c49ab6857a8091a1ee5d fix dump yaml (#136)
641506ebea5c5b51ac710b138b0027b3e2b83166 Update image assisted-ignition-generator name (#132)
b171f481526e539d7c60cb51b65f9b915ffb4135 The working directory needs group write permissions (#134)
680d75b7681111e1cdff30f4195d37a7162c72c4 Use the latest ignition generator image (#135)
b3634c3b334ba6935695cf67a1ca1de28cac01ad Fixed assisted-iso-create build pipeline (#133)
1736f656feb7b2c72bed84d08da6058a5819f550 fix subsystem tests - cancel installation with a disabled host and reset cluster with a disabled host (#130)
4c515d7efbfd61c6ba8917c7db8735ecaab711b9 Added assisted-iso-create to the build pipeline (#131)
e34001885643d9d4fadd984edf84cb7958c16428 Update local job to use assisted-iso-create (#121)
6b2b14c29dd7574bb841706cf9ebd90ce16e181f Adding ServiceMonitor template (#126)
6afedb3d0101e0d565062e2d4833aefced60a2d4 MGMT-1388 add validation data to cluster model (#78)
45260ed7dc2ced56bc419a46f209599d2c9f4194 MGMT-1772 Use an env var to set the s3 url scheme if not present (#95)
c205081f5c299ee41b1392056fe62311318ebf3f [MGMT-766][MGMT-1108] Provide HTTP/S Proxy for OCP cluster installation (#41)
dbee9bb72a44a796181150b622b6f9615ed1db65 Added masayag to OWNERS (#100)
8d6cb02f7d706e21383aba704ab8aa53c8cefcf6 MGMT-1721 Pass mode of operation by bm-inventory to cause creation of flag file to Openshift (#115)
b2c3b196a4bb28105eceaf3d22292650d221b8ed MGMT-1819 add --network=host to docker build to solve network issues (#125)
05c8bf17b2180adc5adfe27537bedb957d2697af Removed ConfigMap from openshift/template.yaml. (#122)
6a391907802c07251ac85d18eed667572f076c6d MGMT-1788 - change the iso creation image to ocpmetal (#123)
9373b652676889ae6c9a5360c4c8a908b7c3e3ed OCPBUGSM-15610 fix wait for service in oc-ingress target (#118)
b167c8b91acf50a3cd1ac0ab87dd907070146ab7 MGMT-1788 - move coreos_installation_iso to assisted-service repo and… (#109)
4a139c063ee227dce1bb9056bab88f62b34a0f99 OCPBUGSM-15610 fix makefile to set domain when waiting for service to be up (#117)
1cc938f6bebe6955ab9dd93bee94fe17db617cbf MGMT-1783 and MGMT-1784: presigned URL fixes for AWS S3 (#103)
720d785e40597a53bc76ee4b7b1b57d9db1bfe66 Setting assisted-installer-agent as default image in assisted-service-deployment script (#111)
e48975015cd294cb5f0ab1f79c89700404987d85 MGMT-1718 Add new command in the bm-inventory to invoke dhcp lease allocation (#71)
7824ffb617a6b11234083eb612facefcc28edf13 Set Jenkinsfile with timeout 1 hour and cron job triggers hourly (#108)
06df84c58baf3c49226c98fabb6ac2646e694692 MGMT-1797 fix get credentials (#110)
98258d5a1814890ed445069d5c642fb1ddc368f1 MGMT-1764 - move ignition generation to assisted-ignition-generator (#89)
c0784d9c7bd50cb39b4c9afceaf04dc43d227934 MGMT-1791 remove disable ssl from s3 client (#106)
6af4f3238b10a2cbc628f48e26af68b07e189b34 Removing `namespace` field from all resources in openshift/template.yaml (#99)
62dcbcd62c0b72921535bd2f6f57248117de4bf8 Make multistage production image to support Prow
72a35d28d168e8bba8931a7e760120c45e327666 Adding ConfigMap to openshift/template.yaml (#96)
e11b610b8f92a7013dbc0bbab00a9aaeb24b9715 Igal/upload logs (#84)
c47f761dfa9352955f17fa4437d7fa4cf3257f9e Revert "Fix yaml dump"
e7e79cdf1abe349c6d0eac44d8ba1b56a926c176 Fix yaml dump
9717529019a6fdd3c49ef82c9ce4f41b5758f9d7 MGMT-1738-Run assisted-service on-prem as non-root (#74)
dff95cfaa324739f7251d5f12377e54641a45a39 Hotfix catch requests timeout exception on deploy assisted-service
510250b9de85700018ecee8c63f8ac811ddb048c MGMT-1767 Move git repo ori-amizur/introspector to opnshift/assisted-installer-agent (#90)
f27aab1b8f40b767b7685df36c7c2f578a95c42d Fix requests timeout
aacccb838253ef31b1ec4856fa2e8f08ce64754f Set Auth disabled log to debug mode (#92)
6872676afe6f6ebf7cfc98b5fe3b29f75f0598ad MGMT-1770 Verify assisted-service is healthy in deploy (#91)
5113705b16859e5f748f72c23f1682dc5fac40ed Updated env variable name for route53-creds secret. (#87)
ad90218e38ed26a2cf36226be1469bf526fc13d3 MGMT-1762 Remove old images pre test (#88)
10127328b9603aba18163a447cbec4c3b7d41d8b MGMT-1669 / MGMT-1637: Add image presigned URL, size, and expire time (#52)
26da029482e6b0556f21e6f534d4c6a0e2f5329c Update state diagrams with missing states (#85)
840503e529611df7e8e609fe7f661411cf23876e MGMT-1178 Change image pull policy to Always (#83)
3241a420a5034e384210ca0eeb3c65842d891919 Add Agent Auth to Hosts list API (#61)
81d799158c199d4df56d003adb7cf22603a6e73e MGMT-1757 Fix upload ISO generation UpdateObjectTag error log (#79)
dccec49e794b4a406f43e54836a5f131d38a53fd MGMT-1661: Fix unit test according to new AWS output (#69)
0a39ad044ed17b4db0cf642840f0705ee2062e65 Raz/ocpbugsm 13597 (#50)
adb1d3e9d4b6b2b56d158a2e0f1a2e9cace25a16 Fix README formatting for onprem build commands (#76)
e76247f2e75e638088d9addc431470d2764ba16b Pass the current namespace as the NAMESPACE env var to assisted-service (#77)
e986184716421633ab159b0362f3f8a93d7e7632 Igal/enable cors (#65)
7360244b4beb5fa46f44b6321bef41ddebaba5f2 Changed swagger-ui link to use swagger.io generator instead of github pages (#72)
e9552a7de84621fdeb3926e3f13701d08c0aab9f MGMT-1717 Swagger changes for DHCP allocation (#43)
973b846f98963867c9eb509a309e3ed48eda2110 Fixed indentation and removed usage of 'scripts' inside the steps (#68)
c4f1aa9e8625eb5ff35022010895b70eff8289e0 Merge pull request #67 from filanov/michaelf/jenkins
e87c03a49a7f6c519f960b9ee24d9dd9037c1b64 Fix Jenkins push to master
b3a12689fe6aa1d4222288beb149df954a452b3a Revert only push master image
11375135380ab0f963c82e1f509619da430596ac Set only approvers on OWNERS (#63)
7ead1fda2c6369f42043eca4980bbb2043370c78 MGTM-1173 fixes for https://github.com/openshift/assisted-service/pull/46 (#62)
592ddb3a5e6718a4651c95e8f37f0f3289f6a181 Use official swagger codegen docker image for client generation (#44)
41167b6858bb81d2418a097ce8670a51f01a397d MGMT-1661: Ensure aws xvd disks are discovered (#58)
9d70f83e321a37a791fabaa9c02ae8b34864c1de Change Jenkinsfile to use env variable for the image name (#60)
5e741c8388d0ce2fe5a8d05acfcc34e8d2465e7c Refactor Jenkinsfile and fix OCPBUGSM-1866481 (#56)
feb32e82dc38daf8d838d47e73f8ffec480c04b2 MGMT-773 auth handler should not use populateKeyMap when auth disabled (#55)
d75955a06cff0ed1fc1fbfb47bd1a4639081876c MGMT-1649 Add host installation disk path property (#51)
1e23423a77c187e4fe98b0e477fd3031b23a4496 MGMT-1715Replace host and port with URL (#49)
bc195f66886a28590a1c4348c7327dbf389a531c MGMT-773 - Auth disabled by default (#53)
9ca9af7cddc07b0b101e37a5ad818dbec3f1fefe Auth handler - Support cloud.redhat.com authentication (#45)
2ed2e03d9f7fa76136c8d94f2022ceaaa1a2bff5 MGMT-1626 - allow openshift version 4.6 to be passed as parameter during cluster creation (#47)
1aab3396412a5405c6bbf901079fadf02fd03518 MGMT-1681: Use only official AWS SDK for S3 operations (#39)
11e90672a9079f6732689a6e6694bcc9d178fca8 Changing deploy-test SERVICE image to an unknown one (#31)
bb7a43f047b704539187c2e3e1617a4090074203 update latest docker image
2e639424af270c1cc375335c193eced590555335 deploy on same agent
f2d56e482c68491d6daa2b1c82731a7c14151402 tag pushed images
bf18182b2d66b5a6fcf520806d473dbdd478578c Removed s3-object-expirer from openshift/template.yaml. (#29)
34af1e6da8bc6d084799db329a4f94fc0a70cfaa Merge pull request #38 from openshift/osher/quay_login
b35818bf4252334b19db845a110ac083b03c2100 Remove OBJEXP from jenkins file (#32)
76195885286158d3f78d49af1cbd0a4d5a38fb45 Fixing DB password's env variable in openshift/template.yaml. (#37)
ebeefe24568d94b7c339bc14a00d0ab14fc0e705 fix quay login
25b42b9679ddc37c50a4cb6387390c0fb1a9fcbc update pushed image assisted-service (#30)
46d935b061aa6b6dda58371dd4bfe5010eba0099 Merge pull request #28 from openshift/osher/release_master
ee6476be2013ba4c926e768a76c5e8669d4b4cc5 Pushing image when master is updated
9a7ac159dd965cbc1db31b5a116c90b6855c96a0 Rename INVENTORY_URL, INVENTORY_PORT to SERVICE_URL, SERVICE_PORT
eb11d42d3af565973294204b6541483d1b73f8a4 Merge pull request #27 from filanov/mfilanov/prow
6e2bc12a9cde82544e2d72ecb38a01c2df87e984 Fix APP SRE changes
4246f222247464bdf9bce0e0ea1ffc3a1c343c66 Fix agent to available ones
df8373895f85912553981b1c52ca9bd6abafb7a7 Rename bm-inventory to assisted-service in tools
e82e512a883895a404da25a5fb17f1d4ad6204dd Rename bm-inventory to assisted-service in Makefile
0fe1fabb7b177335cf712d69be8cce8df60deec1 OCPBUGSM-13662 fix deploy scality-secret to get namespace option
88b3dc3ee7dca6a74e90363770f5587c6d09f22d OCPBUGSM-13662 Allow deploying postgres secret to costum namespace
953f4f0f5cc3c4505b3d5c31466cddd2ad6c67ae Removed unused code from openshfit/template.yaml.
7b86b9bdc22ec88ec5d628edc52bcb5f9ef55897 Connected `assisted-service` deployment to its ServiceAccount.
9746bab2cb4bd1bcdf9b99b1cbeb5cab41a99f62 Renamed the app's name 'bm-inventory' --> 'assisted-service'.
780e79a06297878a8eb9287eb2d522659859812d Added a Service for bm-inventory app.
909cba69dbf4838fc54cfe7ee541523043c7cba4 Updated the deployed app from demo to bm-inventory.
14d42c923f260936395ff5a322f70d608eb0d3e7 MGMT-1433 User-Auth pass Pull Secret Token as env param
3e4197f5cf1bddcd0b9f63fc0c7fd850d66bb246 Removed default values from S3Config.
2168719525670fa5459f66c6096aeb75ca43dbdc Updated use of S3 credentials from Secret.
2ff9b6c6676d8bbf9d1a8562d6ba7badc711f44d Removed default values from DBConfig.
e7f9dc69c37643713406b13513741b8dd30a6b01 Updated use of Postgres credentials from Secret.
bce5f1422d2216bf74a3d770b1d0ab6ef0cdba82 MGMT-1582 Inventory: delete cluster installation files generation job on reset
3ccc7ffaa01d91652829c099a9c1f4558bb80168 MGMT-1582 Cancel/Reset from preparing-for-installation
7a9be43d2b9ccdb765c4c02de8cf98912c743659 MGMT-1428 Simplify secret creation code
9ab601c57fa51ae585eac9efebe6c2731bdcc9c6 MGMT-1428 Add TLS option for OC deployment
4d43d9827984e821f52c2e22d20f5a1a501a110f MGMT-1670 Remove redundant log messages
7dee6b66d8ece213e592ba6cfd8efdbf03181aaf MGMT-1686 Add option to bm-inventory deploy option to reduce minimum HW requirement checks
af98c8b1f699cc064c658b9454a862013bd10aa1 OCPBUGSM-11342 Support SSD drives
9fa2ae67439a4b9843642d7178ba33c6684c8684 Created a pkg for DB.
43f4ac379b79ca4906abe1512593812e3cca992b Add OWNERS file
26000c94371097e96d16751d8fb45a3307884334 Rename BM_INVENTORY to ASSISTED_SERVICE in build_deploy.sh and openshift/template.yaml
edb9513b4765640c88db1db2ca82556be5eee1b8 Fix python client generation to work with assisted-service
6497b3543fa16fd2c61847b7d976c605a47d3231 Rename bm-inventory to assisted service in github actions, Jenkinsfile, build_deploy.sh, openshift/template.yaml, pr_check.sh
9bfff0637ece4029e3f22135ed88f0fdcca034ee move deploy/bm-inventory* to deploy/assisted-service*
2ed6222d07d8b6f8bb28eecb89d978bf16d84231 Rename bm-inventory to assited-service in Makefile, dockerfiles, tools and dpeloy
8398012d07d1988ed5f888661a673d01e242d91e Change dron to work with assisted-service
623bc3fff30b45e2bbf2ac8a7ae8e61e611148ce Change dockerfiles assisted-service and README changes
e6a1f1b48aa83bbd62bab6a6ee966cdb0bee5fd2 Rename filanov/bm-inventory to openshift/assisted-service
279d58703a39aab80b6a3fb79d68b5eea2463473 MGMT-1080 adding mount to journal docker to assisted-installer
0cb5745a1213842bc64846e07933bdab3edca140 Fix bootstrap stages enforcement
a23a0ef87cdb8daa6f71f6273a5fd2de2c33d0da Add /vendor to .gitignore
e1b3edd50df7c16fc5ccddb3d0d73a3f8637ac87 Fix tests which rely on execution under three minutes
d4c4b553f073c679000ed5767ac5e39441c69119 MGMT-1658 enable disabling host in pending-for-input state
c7950ec7bb3dd056d5c8366fe5d3c382c0f46048 Avoid pushing PR images from a fork
a1df761465ef84ce7a00a2fa47e7178fc7bc0abf Updated S3 bucket creation in cmd/main.
a383160bc07789a7036e799ba5fd91889816e34e fixing sub-system test, dding system vendor info to test hosts
e7f68ee930180df992504db3f338012cbee9defb OPCBUGSM-4299: Allow canceling installed hosts
141fdf2447b14ab3289e4ff507c2a8ac095876aa MGMT-1231 moved '--namespace' arg outside from the mutually_exclusive_group parser
5600f1cd4bb2ede00dc85ece0b77eef021f3ad7f MGMT-1646 clearer monitor log
3dbcf3532a3f8cd47d9500f2f8e3b04821c80aff OCPBUGSM-10683 Deploy UI: pull image
fde7c9d90ab68b871bda33832edcf1ea2c9fe4c1 MGMT-1647 Add test function getting cluster masters
9d0f4de5feb4752226f5b305f9a9c24e1a25c886 Revert "Publish image with PR_{hash} tag for any PR build"
279bfd0a83090e6b089331019a95c50e4679fa23 MGMT-1643 - trim whitespace on the result returned by minikube command when calculating inventory url and port
fae4019fe6b2b4b3295904fa1bf1da7264d3883c MGMT-1643 - trim whitespaces around inventory port and url in case ignition generation
60ddc8b676490e6fd32d976a6764542ad09668cf MGMT-1382 autogenerated
b5c33bb81eed693ef41b86f2d03527d4c369187f MGMT-1382 Add an option to download install-config that we generate
33421a7bcfd1d1c8ef1ad66acbee60071d4db985 MGMT-1231 Makefile: accept NAMESPACE argument from user/env
b092d355bc6306f9df4e843101154b6f1088edfb MGMT-1231 Deployment scripts: accept custom namespace
5f70bfeaebc73d885d17da043b910a9c2d1b61b5 MGMT-1231 Deployment files: custom namespace
07b245727e3fbdf92a3861ae19252eba5f299e96 MGMT-1110 Add message of the day to agent
203bbf7835e5eba094eaa0c799b8cd04a0056f33 OCPBUGSM-8565: Add cluster name to register event
1c902d742100940f6a287f29faa3cb58ae5b63c4 MGMT-1402: Add events for all host transitions
98b9918956cfed464e77b27366d231df79ddbf01 MGMT-1413 Added basic identity implementaion
b48b791ca8e87b1ae98c15f312e97a54d384b22a MGMT-738 Added fake auth so we will get default username in the request context
df593fc9a50a85cd783661eb9f79f23486ca764f Autogenerated
ce424a72253954db213760e774a024fa29770dc3 MGMT-1413 Added owner to cluster swagger definition
e4500b8bdcc272a95785d88b35fcabf984b9d8cd Rename inventory_test.go register host test db name
2695a1aa5be9fb5e2eb09b719db3f58b9aacae75 MGMT-1616 - move OCP release image configuration to configmap
1e9e18d53c5c444312b1a6852bad38ab9f65d466 MGMT-1129 Machine CIDR calculation and VIP verification should exclude disabled hosts
091444b8b4950574abd0f8fbc3f98b9bcd2e8a03 MGMT-1634 bugfix report progress subsystem test
30e856456cebb8fe605f7950844cdeda936ca365 MGMT-1632 Subsystem: fixed "cancel_failed_cluster" test
08508061ed837bbfa2f0319af0e6d85f2485fe28 Publish image with PR_{hash} tag for any PR build
2702eb6e355ce1461aae389170ec7f873ef8035e MGMT-1635 improve s3 wrapper bucket create error
2ddec11f26343cadacffabcfad75af0ceb9eb5aa MGMT-1583 Reset Installation: allow reset from various states
3f8f8adc1067042f3c7e53ee2715cea76e5de4b9 MGMT-1041 return forbidden error when host register to cluster that does not exists
93230f986f3212f98f255d0417c1417839f845c1 MGMT-1041 Swagger add 404 to host registration
745b7b79ed7b16a4405e5633c80a681528a3986f MGMT-1618 Validate pull secret is set prior to generating the cluster ISO Added UT and updated subsystem
796ca8e97e5cbb777be73e7b1469096a343b56d9 MGMT-1118 Update ignition for RHCOS
3e3f5b4b7e48ed45fa56403f60e51e8866d6e551 MGMT-1583 Subsystem: Added cluster test
18d2260ad3d654e841c740765bb8cfeccf684a65 MGMT-1583 Host Monitor: check for cluster errors
912bf73ffbf79ec9e4a1546c94fd87af06aedd9c MGMT-1318 - enhance BMH CRs with relevant inventory data
4e9577273c5cbaaceb4e7ebac7f6d6b5ec48dfb6 MGMT-1607 Upgrade bm-inventory to install 4.5.3 OCP
f68d87229d36bb201a20e7c9b1753ec245033d81 MGMT-1090 Remove the HWinfo host operation
a06383ac80fcf961ed07bb68a051f1bbf6677eaa Added "Waiting for control plane" to host stages
c6013ad5774cd78e3119cfd805a87db3b34e4e51 MGMT-1241: Disk according to GB not GiB, clearer validation messages
0fadccc27219143814f9f50315eaed6f7017e927 MGMT-1596 Update hostname should be allowed from pending-for-input state
a700912784c94389de6952f23a5c2387a4ab7f04 MGMT-1527 Getting an error in bm-inventory log when updating free-ips information
8f73237394fbcb15800702da7ac2ff93c77eab7c MGMT-1603 Prevent dummy iso generation uploading to s3
b455f7c70064a0a3178465a7dba5936da86846a4 MGMT-1595 duration value is incorrect when we report installation phase seconds for install command failure
723d32de312c0d41d425cbd0413e61721d223c07 delete debug.test file
643896352f4f16deeee583b20ef81ae23830ee25 unit-test target should wait until postgres is ready
79d8e0a3f303d0fcdffd2c9d108c44d540b4ed11 Fixes after rebase
afcdeb00456eade626ccecab3627c0a2d8b0eb83 MGMT-1537 - Use supported postgres image
51c1d16a266af82a26fc4ee46fa605d5057e4fea MGMT-1528 - Rebase fixes
23e9baf99831f97c3e4cff6ea25d8ba24d1ea829 MGMT-1528 PR related changes
113a2b46cf85791b6f632eb09b92216d9e589a22 removed maria related files
f2ba117547ff665155c48d0c7dd9d6ec5ec8e1aa MGMT-1528 Use dockertest to run UTs with postgress
6a17cea63c5114ad9a066ea7a8ee7d160dcb3244 MGMT-1528 update drone
3c066d66ec0bcab2702599d4993c100104ebb085 MGMT-1528 test fixes
72a201167ee4ee8e2fd877accf7c690507871ff9 MGMT-1528 add postrgres support to assisted installer
32a8d1388681386d90847a51a220fef3c0919a97 MGMT-1593 update inventory should be allowed from pending-for-input state
7da212794302e890946ac40294e7d967dc0d19de log collecting on post
1cb3f292f045bcb055bd7d2c34f4f6744c645845 MGMT-1594 remove unused ImageBuilderCmd overwrite hack it was used to run a dummy iso generation without pushing it to s3 for testing
7229b9711f49700e9a154afde747c90b4d957639 S3 Expirer unit tests
c30e997aee153980d4038aad7114e3538b9f7431 fix code review
142b9fa478f166d1a7fc88a0310c141f3b8d8e2a MGMT-1355 adding host metrics and cluster installation duration
b24b47f4debe9f684342161fcf49b0108d058504 MGMT-1564 move stage_started_at and stage_updated_at fields to host - adding a new model host-progress-info
9104ab355b40f6b97f452f2ae06c968e53fea798 Adding details to README.md
e30b53054f33a698bb0702cd25c2af3ee0763ecc Fixing PSE deployment and added some adjustments on Prom svc
808371289dc952cd68cddf75d8b37d3c7f2fe39a MGMT-1490 Enforce stages enum ordering
5707aeb9f74f0523ebbf1eb3ab3df8b8c9c9867d Bugfix UpdateHost and UpdateCluster err value
1e06a201c1b1db72010fc395d1eb9715757155fd MGMT-1566: Add missing API events
2f6151c9d1993bef3857da6b437ebd43587d735b add agent to pipline
8e03b40b1df6447203228ed5c960ea9ff05a91db Added Jenkinsfile
5648748e7bbe8871b9f3f4f1a2f5aa744f51c439 GMT-1380 Refresh status changes - Add refresh status support to stateswitch - Removed code to avoid logic duplication
d332d401bf13b28719eb026fb955fd102cedf0a9 MGMT-1380 Changes - Validations - validation-id support - validations preprocessing before refresh status
f548419013f349a9472c34a11e8a7989423f0dcb MGMT-1380 swagger changes  - Add pending-for-input-state  - Add validation-id and its values  - Add validation_info field to host
9748e8fd1e81bcb9aa663331a8d45faf33765ccf go.*
94601686b66e278132c5e503afc4109f35dd084b MGMT-1581 Bugfix unsafe status pointers
699d9d076e01d34cffdf3428d5b45aaf0d6f2aeb MGMT-1579: Expired images are not deleted
6a03f7e64dcb7a6112b7e19494d86bc6fa1b592a MGMT-1567 Change cluster API to use dependency injection to get host API and not create it inside the modele
13ababe499875231fcbc7316ec33e2d5325961e5 MGMT-1419 - always set hstname in ignition, so that the hostname reported by LiveCD will be the hostname after reboot
6b04aa64bedad6166ddffc752018f1a390b65a8a MGMT-1339 - BMH CRs should not be created for disabled hosts
c54f19a9b98dc1b3803e13583cafb1212341122b MGMT-1565 change cluster refresh status using get cluster from db once It will prevent races when we get cluster with state A and then because of a race we can get a cluster with a different state.
caf3dc405ec94ce4eb95ab0903495600f24b24c3 Add FOR UPDATE db option to install clsuter transaction
fa011bc02523d688838f61f3d8ee42246ca31713 OCPBUGSM-4255 Added reset and cancel to eventsHandler
7435e91193790347e5c80318ed01d48438b1842c MGMT-1518 add request id to host and cluster monitors context Add request id to creation of dummy image when service go up
4351cc41f38492b2e66bbc3721d65c4343b0e988 Remove UpdateReplay
30433d58624b9026f7af62d8e098878ef392af18 UpdateCluster receives parameters and returns a Cluster
09b0e77bbb44a14eee4a28b92096c8eb5c15b8e6 MGMT-1479 Add stage_started_at and stage_updated_at & MGMT-1493 fix status_updated_at
195481270cbe57dbf124495a1f80e3581a4d8b06 MGMT-1486: Image GC support for more than 1K objects
ca31019cdb5bd46979e5b4fe18b54d94c67380cb MGMT-1453 fix: Ui shows one host in error but actually all are in error state
173e37ae646212e5acc2b7a28f5282c02b3f9578 MGMT-1559 Upgrade to OCP 4.5.2
c037fc4551c196dc29c698d13f43cbb3a99b9778 MGMT-1540 tests
24b0fd05db85a15a5a5e6ebd981fe616170660c1 MGMT-1540 do not allow hostnames as localhost
70fadf9ce0bd98cb59cf939ee5dacf5ae8d0f13b Deployment script : Fixing failure when there is still no app but wait_for_pod already running
3709c79dca3d38df30a30e4fe4b7cdd142e4e6d8 Fix README.md indentation
d166cbbcc9aaa436ca1f0dab713b33de12dc84ae MGMT-1460: Add severity to events
9e071b59e2466e196e2a77ee7ce100fd9a99a407 Auto-generated from swagger
78e59e4910d1223767fada426f56a16ff00bf5ba MGMT-1460: Add severity to events (swagger)
5fe67f2f228a3c35ca806c4c0c30792814045307 MGMT-1355 fix code review remarks
010c095739c8a9b7d796d543750c0d26faa6a02f MGMT-1355 service metrics: cluster creation & installation started
cc3db2a67f0ffd73926ce9396942aaa7f5c01a1f Removed all traces of s3-object-expirer
19c65a7f322d1090fb08cd1ea6a98d620b5a0d4f MGMT-1526: Clear bootstrap on register
c6a204fe92e138b2c9b20b32ecd2fd25152bfb0c MGMT-1500 Add preparing-for-installation state to hosts
d64cafa9551f00077f2b7f0688be04f3dd34d2b7 MGMT-1502: remove dns records on cluster reset
10bae0aef25b0f02c6b305f1ebd0d1aca826c0e5 MGMT-1481 docs
3485081162e09bb0c4aca47d56c293affd47ff0a MGMT-1481 autogenerated
3cb8216cbb92f3b70423545d2f3c05abcb994b8a MGMT-1481 tests
21947df589ffb9e2f08f49d5094c30085b27f6a1 MGMT-1481 Adding complete installation api : 	1. Adding new api that sets cluster installed state 	2. Adding new state "finalizing" (previous installed)
62b4ee7fc197c1d7a444c8c9810f1aa36c8b908b MGMT-1481: Swagger for complete-installation API
d402ed1f355e97b80163cb5339d4cadfa74b38c5 MGMT-1367 Add to agent the pull-secret for authentication with cloud.redhat.com
1f56f4ac95a3992975c1752b6f147a464b951008 OCPBUGSM-4240 Skip disabled hosts on cancel/reset
6d243c5f43e93c46c797131664eabd269eb66bb4 MGMT-1520: add status_updated_at to updateClusterStateWithParams same fix for host update function
2a0525a054f53873340478cb8ed85fe4f5eed5b6 MGMT-1516: Fix "code" property in returned errors
a0010f42c9ebcb8de86c67c435639cacf6aee0fc MGMT-1505: Add clear message when trying to generate image to quickly
40b23b37354b8c52918784539162291f2507da6c Removed "Finish Waiting for control plane" from host stages in the swagger
582aa4ae8b1b6bf619146b58a9ed110159b5a6e8 MGMT-1510: garbage collect dummy ISO immediately
ff357461c8065c4994af07ddaa2b8e948d44f4f4 MGMT-1511 change cluster prepare-for-installation to use statemachine
4f0755e9f276609717534a0e6cf0ac9f7833b420 MGMT-1494 Cancel/Reset: Return host progress stages in response
5a2b6fdd86505c93939060ba2648f92b34a8a22c MGMT-1501 Added subsystem
4bb5afb18ea97fc31e0be38ecf191ddc7886f1ec MGMT-1501 Wrong boot order lead to cluster error state Updated the cluster installing getClusterInstallationState to consider "HostStatusInstallingPendingUserAction" as installing status
b55faec5cb09fac75bcc285c658dc9a77fcc8a72 MGMT-1349: set timeout to prepare-for-installation status Refresh status of this this state will check if cluster status haven't changed for a 10m, and will push the cluster into error. This can happen if the service was rebooted or somehow the async part crashed.
9a0b34c8b9a14b54c38b474b88257677f86a749d Updated bootstrap stages Removed HostStageFinishWaitingForControlPlane Moved HostStageStartWaitingForControlPlane, to be after HostStageWritingImageToDisk,
f597e49ffdff391c0994df627e26f378cc78125b Clear s3 expirere leftovers
ad986ca0bdf138497cf64ea8f5920d34e5db9862 MGMT-1424 Host: set bootstrap=false on disable host
a2434cb6b8905d823772c6bfaee6adf264a80d16 MGMT-1424 setBootstrapHost: check if already has bootstrap
b0626be169b846d35f6ac652a4430c8e2c30bdd5 MGMT-1417 Tests: Added cluster & subsystem tests
c7dccc6348e749a2eda21ca1c58f5e785ccc9c8d MGMT-1446 Transfer Controller image flag to the Assisted-Installer
0e1a97b9e9c9534360ae0d3fa4d1937ce87e92bd MGMT-1417 Tests: Added cluster & subsystem tests
097e5e60f380dd06884efea887b03876ed8321a0 MGMT-1417 Host: auto-generated mock code
05796fa552dae97bf0ada84842dc980dff2d0a64 MGMT-1417 Cluster Monitoring: Apply new state on cluster
ba469923fdd89f386d81a76d54e07da0f1d52ef0 MGMT-1417 Host statemachine: Allow register from new state
2ce1aaaa167bd528e07c4cbb4bc550d6503d958e MGMT-1417 Swagger: added resetting-pending-user-action state
64ea845712869fcdbdcd50a3582b175f53b388c5 Extended tools/wait_for_pod.py's timeout.
5b52bc6f37bd11fdd8ab1985a854ef556b965624 MGMT-1445: Port image expiration from Python CronJob to Go goroutine
9ade153d9ca69d5f00299b972346e3c13052e620 MGMT-1487 Agent might not restart in case of failure Updateed the restart policy: Set StartLimitIntervalSec to 0 to disable any kind of rate limiting Set RestartSec to 3 seconds delay between executions
fa8bcd4dd1916c3a31f55e2cbf182d74f5846b3e Remove mock generation from generate-from-swagger Delete generated mockery mocks
348a33aee5479e7e193d87df2fb5b3c85c4d55fc MGMT-1358: validate cluster name on register and update
1e419f0061353b5aa733d197e82cdbb75f9d86ed inventory: rename filesURL
6c0a514e3a784b6263655b5684dc88d5595ae27b MGMT-1444 Move ignition generation outside of install cluster async part db transaction Change install cluster asyn part to handle errors with defer Add request ID to install cluster async part context
539b6a4944a4edcec57a2deeabf16a30ac776143 inventory: remove unused variable
e1dd7daa2510112d6270087a7463f1331218b676 Revert "validate cluster name on creation and update" It breaks many subsystem tests
2d1b80fd51e0089a9141601205809af6be8ecca1 MGMT-1404 Instruction Manager: Added stop installation cmd
0b31f0927aba9217741635416aa434546f28ae7a configmap: set base_dns_domains from env var
e5bf82a2a87979a9e074e435f914daf3e1d30083 validate cluster name on creation and update
e77072fb0a85f8d4e809046b46d2ce45905ad5fe MGMT-1414 Updated resetInstallationCmd
e903c396b70761a7e6f074180ef594fee0eabf73 MGMT-1414 Swagger: Replace reset-agent to reset-installation
b284f571cdbac685b54d966aa5625c7ae7a3662d MGMT-1401 DownloadClusterFiles: verify file exists
5029ef66137d1d4e1b03e99fbe6e934139e75d09 MGMT-1401: Inventory: Delete all cluster files on reset
2bf067a6a7533851e935ef274865405a9d7c2e1b MGMT-1401 Inventory Test: Fixed typo
5dfb47db8831d2a8c65a2759645ee56f7db72e45 MGMT-1401: S3Client: added file deletion method
b2f6a5a991f1cadee261c488ae2084b37bad74fe MGMT-1454 Separate HostProgressReport field & Fix host stages
da2d7056f9e726309776cfe300bbe9a2da4088b8 Remove binary file
06fa0e00b4c586a5c9f8715c1cf120b5410bff7a Fix flaky subsystem test
9f499221affde0ea2ba1a8580c8a6b40983e84b8 MGMT-1374 validate that hosts can be installed in the sync part of install cluster API Reply example: Not all hosts are ready for installation: [2ccf4f6b-cc1c-4c3f-81fa-8aaab4c33073 b1ef1f7c-82a3-42d8-a544-60b8bd3422e5]
cba320f55d0dbfbc13b80a4a40bccb6e9c873aa7 MGMT-1211 Add installing-pending-for-action state & Handle wrong boot order
516b498f71b5fe28e34b7b2d29738e0b7c21300f Revert "MGMT-1401: S3Client: added file deletion method"
30ee36db92e73dc8caa4cb1c3afcd640200c6101 Revert "MGMT-1401 Inventory Test: Fixed typo"
55bab8a1523e886786a875310442a78c2ab77983 Revert "MGMT-1401: Inventory: Delete all cluster files on reset"
b4e077e425906d78687cbcd57ab1b71c344ac045 Revert "MGMT-1401 DownloadClusterFiles: verify file name"
3340c78f7c50513859d43936f088a3aabd12bcd5 MGMT-1401 DownloadClusterFiles: verify file name
8f0bf1f79c05a67fde73a79b3a4c6345d4ef012d MGMT-1401: Inventory: Delete all cluster files on reset
444ee5a7663a70c6546e9f36e3da33b8d5386757 MGMT-1401 Inventory Test: Fixed typo
2f91bccc5365d3854a77ca82c8d8eb4e3eefcb16 MGMT-1401: S3Client: added file deletion method
12d2574b933b1c955cc88c6e5ba6a98e142bd2a7 MGMT-1457 autogenerated
116eec80b93d85827a520f55666e8f23af089624 MGMT-1457 Add progress status "Wait for ignition" to host progress statuses in bm-inventory
1f16f242c0359d720abe51bb778a94d01d62c273 MGMT-1441 add empty implementation to cluster refresh on preparing-for-installation state
d511ad4e037c0e5c0a7c5533ad63d3bb39b1bc95 MGMT-1423 - requested name will always contain the current hostname when the host info is returnd by API
6336a3a6d279d66f91c42d505aac197593321563 Remove stages array from DB
74de2f47244462175c6084bf05e4451f4fe49612 Add getStagesByRole
9425c7fbbc42189276f2734c6e6b91932c73063d Add Configuring stage
8a7ad67b21467de43c64b0033c8ce39c1ce18c50 Reformat ProgressStatus to HostStage & Update DB
2322bc0cf7a4f3269f60477d4e2cbc280b146c47 MGMT-1284 Enhance InstallProgressParams with status enum and an info string
58535ea6bd57f23547bd82bf12bc3bb5de1d344b MGMT-1188 fix installation_error_reply broken test
43edfe3b9f92e59314a42eda752aa1841aa648d1 MGMT-1435: Add state_info when first register a host
27501e2f60b0fc7becd75fb78ff60d25ef05da25 MGMT-1401 status info shows parse error for HW info right after the host has started
b03a48bac339f656b1c951315f58283d79a8442d MGMT-717: Do not generate image if a valid one already exists
cd6245d781682160eea081a2519b76f32a918678 auto-generated mocks
139ec35593056d06dbc97ca940291fad25104053 MGMT-1429: check length of GetMasterNodesIds reply before trying to set bootstrap host
abbeb9eca46392f1fb861a19e703f6898c804669 MGMT-1313 PR fix
babfce47ccbb03d326f12b4a8427835217ece2f6 MGMT-1313 Update tests
ee491b5ef7e6a22cd3aca6d71ec7524c6f41a4db MGMT-1313 autogenerated
6da08c5c3a70387bc8f5cc1f03c803e2f0c56f74 MGMT-1313 Move host UpdateInventory out of state machine model
655cfac1cd5a763c959612b6b19dc43567d82157 Bugfix SetBootstrap field
e34f8681bd4e1be9e99be3563cc11591f3d5b965 Add logger to subsystem Use logger in install cluster flows
32196c2fc7e0ec347cad75a5cb14b0f648d7055b MGMT-1411 - adding subsystem test for seting hostnames
0d260279893beabdf211cfba915505bc6a97145f MGMT-1409 Added support for release-tag in versions API
9c9be2bd154a19ba74602315716638c6f0a14e56 MGMT-1409 result of generation from swagger
ffff4df04dd57d0794d6f2d3021ca26895bca30b MGMT-1409 - Changed swagger to add release-tag property to the component_versions endpoint
ca99c59db5930bc802092d05d10ac435a97d3e26 Added UT for request-id middleware
835ce062b7ad2e7914a75795e9d7a7f981dfee54 Alternetive waiting for mariaDB to response in drone testing
e1cedc2f35d008927f7d95d7d69a742fe40b01b9 MGMT-1126 Split cluster install to sync and async parts. the sync part will lock the cluster in prepareing-for-installation state and perform some validation After that async part will move the hosts and the cluster to installing state after generating ignition files If the async part fails the cluster will move to pre-installtion-error state and the user will be able to retry the installtion
c7b826e465beeb0a70d7ebbf169e6b90e73754c5 MGMT-1126 auto generated
456f16f800ee9b8c1a3f9fb23203ce8135fed1c8 MGMT-1126 Swaggger - add new state for cluster to support async intalltion, preparing-for-installation
16436ddceafb035120ffe84944e7d80715950244 MGMT-1312 move host update hw info from state machine model Update HW info don't affect the state so the only validation is the states that allow getting new hw info, including Disconnected, Discovering, Insufficent and Known
46c6cc6103d953a41b8fdf598e64665fbad2e5b3 Unite host roles from hardcoded to use swagger models
1e083b29e17f9feafbd4b0940b0ce960f51ca6c6 Fix make create-python-client Updated BUILD_FOLDER permission in the swagger-codegen-cli container
5cb192f1d284e6ddc1983c04a3528688d9adacc4 MGMT-1317 change disable host to new state machine model change Enable host to new state machine model Add GenerateErrorResponderWithDefault to error utils, if err is api error then return it else generated new error by the default code that passed
2ad4a78839569eafa1ef7944880bc96a0ddf9fa6 auto-generated mocks
83df05becc78e34c27c6461a8d557208779ba12e MGMT-1406: Return updated resources from APIs
a27df826ce100f49d5f2c11b5c1a426a2e801343 MGMT-1406: auto-generated from swagger
e12c626841259debe57cbf07c65c311f0a768c63 MGMT-1406: Swagger - return updated resources from APIs
234dd557e85e22d05749f5dbb8709bc45a5d0294 MGMT-1272: Fix statusInfo for host register during install
7924255a7a649c551d31aa0b9bdde80a38fb93dc Go swagger generate missing files from free-ips commit
c26ee7957186a5196a5b9b3198bf65d5807f0853 Fixed deploy tag option for empty DEPLOY_TAG_OPTION
a8417bdea2f70e93b1d37687087fe9dc4c6693e4 Support deploying UI with podman
961eecbd32eb0d4cc7ef381b6e791965645e7951 Updated the deploy-all options in the README
eb2a69b9bf3418983efe4e200c8332ea63716815 MGMT-1377 Added deploy options to makefile
c535ec3e5aab6a683a8d968fe0f9e8bf49290205 MGMT-1377 Support deploy manifest in bm-inventory deployment scripts This should allow specifying different image tag for each image
e266816e9228649647534762737a209172860aad MGMT-1214 - allow to change hostnames of nodes prior to install command. the change will take place after RCHOS reboot
4bad494ac71876bcc46b0fbb36d8f99bef8ae822 auto-generated mocks
fb357270a493475f3716f95e68474cff94cb06c6 MGMT-1316 move install host to use state-switch
53c74680153a098ec17b101c4fdbb74916eedb03 Fixing push github action, adding build of python client
c19c7d76a6b1e094b071ba4e3ffa17bb6fdacf64 Added link to the swagger ui in README
30cb5813e918c557c294cb96b4c5b8ad060dd22f Removing -it from docker run command in python client creation
ffb840f4fd0b0cb2077b8c77436efb7008c2e897 Adding create-python-client to update and update minikube
a1dbf936b82989091ee986b6eae70d7be73c374a Changing name of release github action from image-push to release
5ba809f4dfc4d18f21b5a6433d101f0a2a52c89a updating github release action to create python client before image build
ef194df879449ef872932f81e19f04364235f9f9 Adding python client
2bc90b42f0e2459db4409039d2e88567620f98c0 Revert "Adding python client"
96a262cedf2ff87a9e2ba53c707bdb979dc89a03 Revert "Adding BUILD_FOLDER environment"
781bea65ce7d218dbce553f1730567fe3539756f MGMT-1396 Unclear message when the host is insufficient due to insufficient number of disks with required size
a7c8c2cc2208ff202dd60a0b0d0c664e0f2f4da1 OpenShift Template fix
3b6a2d22e62f44c38f8bc496e41fd18fe7c387bf Onboarding to app-interface
d71e77435b4e1f3568f74d56948223bcf4827041 Adding BUILD_FOLDER environment
62a33ecc44cc2d0f9df269415f54fdb6c464781f Adding python client
2be8913344d35eb2f449762b464283d97e1a909b Prevent test crash in case inventory is defined in a host and the monitor starts working
a0cc79d1c9b999c5d3ea85181e90bbbb7dd4018a Fix github action due to change in skipper
c2cfa5a4e492bceb7e581d30568a699f94c397ab Revert "Revert "api: added managed domains listing""
67bc2cd7c80c264c7f71428990be50a9e73a3e6e Revert "Revert "Generated swagger code for managed_domains""
0bff1953705c2c6920e5056643e39d28fe04a9b2 Revert "api: added managed domains listing"
9ead1fe9e917f609a9b34975d72e5dcdd54b228e Revert "Generated swagger code for managed_domains"
cd9a64f671ee1304ec4e8e2fc2967fa6284806b5 api: added managed domains listing
6674f86b647d66a6df2b1d9a0e0bb0f2e18e681c Generated swagger code for managed_domains
41facfae07b54f39c65e3a5b540486b21d9c5552 API to list managed DNS domains
7f425b434f18e10afeb262e7b665185daa874790 MGMT-1236 changes:   - Add validation that vip is in free list in addition to free list query   - Support query of free ip addresses - code changes
bc619a6badfa06b36448ed8d7f180f610eb2b269 MGMT-1236 Swagger generate
66e112751727bb8c07d5e479bad8e4a821c2567e MGMT-1236 Support query of free ip addresses - Swagger changes
4fbe33126545852538a5c5dcc326a44ab37a8c9e Set default wait for cluster and host state timeouts to 30 and 20 seconds. the timeout should be grater then the interval of each monitor.
4051b53e8983f2ae47f39e34469e39d9595469a3 MGMT-1357: Add content-length to downloads
3bb0edaefd7bb4ef6474e6ed5944f555a9d7a83a Fixing #320, wrong NS deploying monitoring services
9e10ac7537b2c6dda19d1bee477776de3e5d8790 MGMT-1205 Subsystem: Added host and cluster tests
ef79ca79d1264fdc8c407d21a68d93859982f681 MGMT-1205 Subsystem: Moved getStepInList and getNextSteps to utils_test.go
44f52a1b80e2fd00be640466e12644844214e5fc MGMT-1205 Host: Added resetagentcmd
a1a51efb1632c661b0808323ece466d164d5c31d MGMT-1205 Swagger: added reset-agent cmd
ef412c889b277d7904d068b12b4ae11350b3ac5d deploy: handle route53 secret creation
7788ed229492ba9ce5eceb8347ebd35543d165bc MGMT-1230: Add event when an ISO is generated
930355098cd301df7576994c2ab73cdcf77cb7e1 MGMT-1286: Add events for host state changes
18781d32ae735d08d64643f908b8280b51b04239 MGMT-1071: Change UUID in the cluster events to hostname
e07a78268a21671400bb722fad47759f3d9ccf86 Add transaction package that enable to add FOR UPDATE query param to db or transaction
7fd0f632d5e7f3581ab5bbb14f27330c461b2cfe MGMT-1101: introduce Route 53 DNS service support
eefe9de29951b248114f40ed01f29d407fbbc05a MGMT-1099 Subsystem: Add reset cluster tests
8cb83391cd83381a39b9e49fc6f3b90037aa93ef MGMT-1099 Inventory: Added ResetCluster
0018ac0da6c5770600e091e7920316dcf8215f11 MGMT-1099 Autogenerated mock code (reset installation)
d76a32739dc748fcb9f6874f58af48167f5c9fe2 MGMT-1099 Host: Added Reset Host
b263f9f1fa48e39ad6a2ee8e1dd162851d6fa2d9 MGMT-1099 Autogenerated swagger code (resetting state)
90f8e77a7b0620ff584ae5432bfc84b91ae4d636 MGMT-1099 Host: Added Resetting state
c4bd8e073aede55100f01c1817b29b135f695025 MGMT-1099: Add api to reset cluster state (swagger+docs)
f67334baa092f57f36506f1bd7b722d6c0224206 MGMT-1099 Cluster: Added ResetCluster method
7feb46afcdce618130ca070bb3db0323a6d72182 MGMT-1099 Autogenerated Swagger Code (reset cluster state)
45e80ae61c4093197aa2c4680ab18ae573a006b6 Add reset to state machines
fa10ddf00033f6ea11278e80a0fa3b0b8a96070b Refresh host status on every cluster update operation Add FOR UPDATE query option to handle race between the update and host monitor in update cluster FOR UPDATE is not supported in sqlite3 (unit tests) so testMode flag is added to the inventory to disable this option if we are running in test mode.
44086f64db2151ae5fd431cddbdb8634ae55f031 Increase subsystem test timeout to 20m
5da401ea590593b6769a8bad8339fdf982c47f5d Subsystem: Added cancel installation tests
606426ff0a8e958de6a7fd14d4775f924c37ead3 Inventory: Added InstallationCancel logic
ed760b169e1705fff952ae1e33fe42c62bb98014 Autogenerated mock code (cancel installation)
d2015a7c5b9ae35c24d9ee9ef593f18b86e851d0 Cluster: Installation Cancel
0cf5eb6303eb20aed67e5f0ab7b88162ce68e702 Cluster: Added statemachine
c7e1fdaeab0caa4ada09728c5984e862d6de8b84 Host: Installation Cancel
89d1925c6e3479fd55a27c90688daee0dc86f1f1 Statemachine: Fix typo
f4199258fb689474c51e6d0d2341bbdcfa7dc7a5 Host: Add "reason" field for PostHostInstallationFailed
d18677114eb7c87960a5ae86165033332b96bf95 Autogenerated Swagger Code (cancel installation)
cb583f8642de3896eedc594ed7019208fc8789d5 MGMT-1131: Add api to cancel installation (swagger+docs)
9e8c222fdf299ec2e35747f949f3abfa7fa03952 MGMT-1329 Trying to download an ISO when cluster is starting the installation, can cause the installation to fail
18218412d29122640bde7cc713c6c6be509d0a14 Increase bm-inventory timeout for waiting for service to 5 min
88d0daa83810c0e1363a95b5f601f232345189c6 MGMT-1314 Move host UpdateRole out of state machine model update role will only update the role of the host, state will not be affected.
ac59f635b4c18e18d8361afb3aa03aefb65afb20 auto generated mocks
8672eef466febd2a7344da295799ff49f96148b2 Added Monitoring integration for Assisted Installer.
352f53285f084376da6df29da7fb94b2dff4a180 Revert "MGMT-1131: Add api to cancel installation (swagger+docs)"
fa8a3f0afbe6255f0dbb41adea1df8640584c27a Revert "Autogenerated Swagger Code (cancel installation)"
f785bd6ac0c01321f9d37bc3304b0e17b7f6fb1f Revert "Host: Add "reason" field for PostHostInstallationFailed"
0500b790142a9702b382620fdb7d5be1d2ac927c Revert "Statemachine: Fix typo"
d1f6b79218fcd91f298e759b6ad4800788154a87 Revert "Host: Installation Cancel"
02247f557795277d78756eb3683eefa7f47c41cd Revert "Cluster: Added statemachine"
eb5010fb69eadf61b4a3d9b8e33c543c90b102fc Revert "Cluster: Installation Cancel"
219d2f4f39f9c0f94379f297032ccad06c29814f Revert "Autogenerated mock code (cancel installation)"
8fcd71b7527809daed6062370a3f52221d572412 Revert "Inventory: Added InstallationCancel logic"
9c41d98bd9db9d8295b5bf6099494f1a604bbe25 Revert "Subsystem: Added cancel installation tests"
ad0e0ff52bc98afefbaba1891084576f439d42a0 Revert "MGMT-1311 Subsystem: Fixed state info"
9863948931cbfa4646726f0c1cd0d6e0763fb654 MGMG-1242: Add event when an ISO is downloaded
1d16004c457177c97edabe4369e37a2602b4c3ea MGMT-1311 Subsystem: Fixed state info
e171cd283f3a495292857192bb0e0aebf9785375 Subsystem: Added cancel installation tests
0d413e1a222f0353e46f2257c2d96dedf5443b49 Inventory: Added InstallationCancel logic
b49947d5226ae2c7880fc425c98754a626bdc1e9 Autogenerated mock code (cancel installation)
94f5fe7f3558b8a1d3f3453fe390c689bcd052de Cluster: Installation Cancel
972ddee35f51aae34827a8f4383e111971f97f33 Cluster: Added statemachine
15fd43315be3ec4ea7c47c01bfa9ba5ba6d45d92 Host: Installation Cancel
19dfd69133f9bd0e97358afffbd5af4d13454cb4 Statemachine: Fix typo
bc8e5195f17f5eca4566f78920137fbc2a450865 Host: Add "reason" field for PostHostInstallationFailed
d99c2696e379dd0ed0a1172a647d8cbc1f7a1636 Autogenerated Swagger Code (cancel installation)
690b773464d8c8c3ce23516c961e5d835dcee283 MGMT-1131: Add api to cancel installation (swagger+docs)
6a1998ad7f59c93c0255a0f300de49ac7c0b085b MGMT-1240: Cleanup old s3-expirer jobs
696cf7859c8ff83807d1b9af9e4b63540a4e0a01 Fixing depeloy-all issue with wating for inventory pod
dcaef737f52a57c7fafad10c5a97da1b39e99076 MGMT-953 - move insufficient host status handling to host monitor and add connectivity check
15101374bc4beeeb3c3ce22b7bd32aa7e1e7defb MGMT-656: Candidate disconnection monitoring
54d56712b59d306125ee68d2014c98cf1e995e75 deploy-test deploys bm-invetory image to minikube to ease testing
8bcb797b6ae46419aeb62343e955d6064b6136bc MGMT-1016  bm-inventory configuration specifically for subsystem
c852ae25e86b72cccb2ba8a141837f6c7edb50d0 MGMT-1143 - make generate
526c8c4e100ad08394de04bf91910be5b026b0d3 MGMT-1143 - Enlarge the column for event message
185b2d348c933b95167484c66398bc6f68e9ef6f Enlarging pull secret size to support Prow
6172dd5669951205717ebc1cd32cf4ee61c0de1c MGMT-1059 Post register host transition keeps host role in case host exists
69b2bfb6d5dfd919d9688331fa4457c4a10f2960 MGMT-1229 add resources limitation to image generation and kubeconfig generation
8be5812ed6f9dd67f1b2149d05bc6071054916b9 MGMT-1207 autogenerated
1fa012a902fcff872bd2c9f34c08598d2d364fc4 MGMT-1207 fixing tests
0061d4e0c59ff8d6473c9d4d779a84fda95e080d MGMT-1207 adding make next step in seconds to getnextstep reply
f2b7b88d126b4e03d9168f5343373923eb342a32 MGMT-1220 bm-inventory should invoke the free-ip tool and store information in database
c0c03e4f48ea8a80a2cb02cb1a2ff8f6c3061945 Swagger generate
3ab9599ae49a47c6143430e56453a680cb89e2dd MGMT-1220 Add free_addresses in hosts table
ac3137e52e04e038d0f80afadbbb99d318a9323f Swagger generate
094c4b5735489ed5d9b971dab7c8edfe0c02ece5 MGMT-1224 Swagger changes for free addresses scan
f3edecc14cee1ac6b69578a6fa2a2dd87f5bfb50 Update drone to run when: 	- new PR 	- push to master
4aec1989d459264cbe02dd214191d50bc226041e MGMT-1244 Change default mariadb volume to 10Gi By default the deployemnt will try to get the current size if exists will use the same size If not exists 10Gi volume size will be set.
1e9e4c43cfb06ac1deac72dac6746cb2e0751579 MGMT-948: UpdateCluster set in DB only if param not nil
4ec67927ec4dfca09119e5068a2c3849bddd5581 Fix s3 expirer deploy-tag option
a1a717b92a6189e6b35672dff7745376358fdde3 giving mariadb more time to load on drone
095c5fd9ff75278b04840d0b4a61dc5309f23644 Subsystem: check StatusUpdatedAt set upon cluster/host create
90bc6cc3e8f03e2fff2b3eaaad99cbdcc20b1990 Auto generated after go-swagger version
bc619802c1bbc9c695eee1f5460d0c287d4c0bf5 Adjust go modules go new go-swagger version
4a64cd7f88b87d139096b1fa95c9ad60af34875b Sepcify go-swagger version to v0.24.0
d917c5fd6dfcd124fd5052338cd9e2d357e22b95 MGMT-1043 Disallow update role when host is disabled
304c9563e75da8256e7bebbc64f088b4ba7c67fb MGMT-1103 add .drone file for drone cloud CI           add option to run bm-inventory in test mode 	  tag subsystem tests as drone disabled 	  disable dummy image for test mode
d93da8024a90f25b1ae9eeb2829183fafd0bf2df MGMT-900 Add resource limitations to bm-inventory, mariadb, s3 expirer
f3560c153e0acca6f5ef86d7c3780de554fb4c6c MGMT-1210 Update bm-inventory to use coreos_installation_iso and ignition latest tag
f905ada3401a4f685d0b29a5e8409069334009df MGMT-1115 Run Agent service with podman
a094b8ccf1681d932e36c794f12ade31c9707ab9 fix reporter spam log, from info to debug
1aa32202e38284054cdf99a6625c221bbbab704f MGMT-1144 Get version implemention and tests. API will get the versions from environemtn varialbes. Save installer version when asking to install host Add agnet version to host register api Update ignition to have agent-version param
161d391c3a2079cfe991cde569c80070369f9a26 add HARDWARE_INFO_IMAGE and SELF_VERSION to assisted-installer configmap deployment script
da005e93cbf8e2503619e08de0f58e70d737c06e auto-generate
31a60243dd111ffa6805d6b75586efd06ca2d860 MGMT-1144 Swagger - add versions api. this api will return the current verions that beeing used by the service, including self version, discovery-image, instalaltion version, iso genenration and ignition generations image. Add image generator version, cluster ignition generator version and installer-version (install command) Add agent version to api and DB
3ffec2a367fbedfd71dd1f718646ad858b14a946 MGMT-1203: Set StatusUpdatedAt upon cluster/host create
9c16418a728df8398da00c66ff19a6666037bda3 README improvements
f47d736f26b7a8a574401dc584c0ac6be3cd50ac Re-apply MGMT-1145 Move agent commands to execute only changes
ae86a3ad4f9cfcb31e04bcbdd9d83b3be9304522 Revert "MGMT-1145 Move agent commands to execute - Swagger changes"
36702d54c7e3bee877cfd89a669ed31aa18c8edd Revert "MGMT-1145 Swagger generate"
d1b66d25b435b802ee55b13d6d46768146eb06f0 Revert "MGMT-1145 Move agent commands to execute only - code changes"
7ce8afa00674b4ff7b2bd56c512c280785d0ecbf MGMT-1145 Move agent commands to execute only - code changes
98dc9da1e2acd4c3aa1867a48287ef32f6b00440 MGMT-1145 Swagger generate
c00143a445d40027412efeb661a9ecaa170c34a4 MGMT-1145 Move agent commands to execute - Swagger changes
b42d679f5f3e3732ff9090d0527b466fae2ddbc8 Get hardwareInfo image from env
f73f4fc39b4b11488779e07a8d3cb0f948ef631e MGMT-1181 Updated install and hardware info commands default image tag from stable to latest
7fd7e2ba3fe13698add3b1289d7785c88199cc8a Updated Makefile to use latest tag as default
ba60f7ee5a842d770e359082c41850816c9d9be8 Added release.yaml to github workflow This workflow will build the repository container images upon git tag creation and publish it to ocpmetal registry with the matching tag
7ced2d7187e0b070389ffc61f47a841c7447d78f master build publish image with latest tag instead of stable
be06098e94adaab9f7cd39297c30e0c60f18cd86 MGMT-1150 Add an option to deplpoy with specific tag All the targets will be taken from ocpmetal quay.io account. The usage is to add DEPLOY_TAG env to the makefile: skipper make deploy-all DEPLOY_TAG=stable
67c0caef9b86c36a1b3123623b162336456561b2 MGMT-1164 - Adapted prometheus endpoint metrics to contain the cluster-id where applicable
d625aadf20fe23974f0d5bc8bb42c6d0254fe56d Removed 'tests-passed' label handling of the github action
32d82234ed8721eb1cf5d05e5a41c7ee83cceaac MGMT-1128 Every execute command that will fail - will change the host status to error
9609d801b59f07992148eb3fb17fc30987b86405 MGMT-967 Result of generate from swagger
73892bd197c0bdb67447585c33b98a0eaed84584 MGMT-967 - moved from storing the models.Cluster struct, directly in DB to embedding it in another structure
683247b75c799b50a30f01a7341a42b450aa25d6 Reduce lint time by connfiguring go environment on the build container, to point to the host's cache
83836d1c17f18516ea6e3f8cb276a60c83ab284e MGMT-1123 - in ClusterUpdate, don't validate pull-secret if it is an empty string
c6e70a97ea882e477a9abb34e4b4dd3baf932801 Add timeout of 120 seconds to assisted-installer-ui ingress configurations, the default timeout is 30 seconds, without it long sync apis will be dropped, for example iso generation
cc76ac838ed02b476c07f78cc464290774d25907 CronJob to periodically list objects in S3
522410780047e589193b099c26f35af2fd560520 Add Apache 2 License
c213b0ec2f26a0d218055325f250829b87be7d4a MGMT-1078 Verify that API-VIP and Ingress-VIP are not equal
7460699979d9766b002abba87635c7ceee56182d MGMT-1107 adding subsystem test
c346bcc354dd656de37af9e4154fd6ccb932b35d MGMT-1107 Need to filter disabled hosts from unique hostname validation
6c646c4943d24fde17cca59eafffbdbc0780c923 MGMT-1068 - fix code review + adding subsystem test
bd727e288ac34605b4da59be41fae58983068ede MGMT-1068 node status stay installing although the install command failed
e6891315968ecc10ce437eec90533790822b8b19 MGMT-1080 Add /var/log volume mount to the install command
d901b82c9036980d9b443ae4c3d2dd3f8607c609 Autogenerated mocks
eb36eb1e3409cb19f7c4a78ba0349f5d2a16608d Rename VerifyRegisterHost to AcceptRegistration
9c22562d0a52eb02859ec29a2b3754d737b80e2e MGMT-1038 tests
52094b5e4c999f25f9d456f10623be3d48cd096d MGMT-1038 auto generated mocks
170fd9d3fa86a0a04c117f36c1c8dace6bb4b6ea MGMT-1038 prevent update while cluster is installing
6483ac1d933f5cfe933a2a3b63c3ccb0f7496134 Add timeout of 120 seconds to assisted-installer ingress configurations, the default timeout is 30 seconds, without it long sync apis will be dropped, for example iso generation
cd16ecf438ac24c225d3f3a95a6f7eab0b023147 MGMT-1074 Insallation hangs in case master node reboots (before the actual pivot) In case an existing host tries to register we should let the host state machine take care of it If the host was installing it will move to error
22a5b9a2f858d31c884a7e3000a1f50447df0f06 MGMT-1084 fix validation message
9cfd0b32bc3f615d211eca52f45f71263bc7a4cc MGMT-1017 autogenerated
763f2b3e6f6446a72117cf97ddb13f6341392d07 MGMT-1017 adding tests and test fixes
765e4653c4390ceaf7820fdb22ce382fe3bfeb36 MGMT-1017 bm-inventory should not allow hosts with identical names
f712531150dc26513e38f29a71baef37c4a462aa Change db transaction usage. Instead of doing rollback on every error return the rallback is done in a defer function
8ec26c4ba5b201f46569581e264f994907c0bef1 Makefile: deploy-all to deploy S3 expiration cronjob
0534138d5b50f2e3f56a0f2ac7a7060587c1210f MGMT-1086 - Changed all direct usage of global logrus, to use the log configured by main
fb6ed7d2fdce1be558cd8a0fb3266817b58df50f MGMT-1070 configure logger to report the caller
c87a154a0654f27bcf00292d80d4faeff6df5289 MGMT-1058 Download kubeconfig panics if it doesn't exists yet
43f0481079d05e39e7975a2dd17d67010aa502a2 MGMT-1013 - Change type of ingress vip and api vip from ipv4 to string and validate by regex pattern to allow empty string input
f8917e59de2ca6eaeceb94c355f2bc8bc1e7397c Swagger generate
c812617d6175fbc5580495a5ee22de7cc48c6606 Swagger changes fot MGMT-1013
e91ca5bba8e32a791570e4a1c992a5d81148236a Added subsystem test for host registration during installation
03bce96638e466759750f6aae26b981d1819bb64 Preparing the Role and service to be fully compatible with Prometheus monitoring
de2be4794aa3f22efef3b1238a9e9f98090f773e Updated cluster.go fmt.Errorf to errors.Errorf
08378c32f3277f427f5bee3fa07842c33809a845 Return Forbidden in case a host tries to register while cluster is already installing
5b47e20f0b65f46ea838696f5d8bc62fe3287d6d Autogenerated
d8dec7d0bdefd2bc2914a3b058e0def5aa4c533b Swagger chage: added 403 error to POST /clusters/{cluster_id}/hosts API
65ddc8ef70205f73f8dc56093ee136d813c331d1 MGMT-1042 - There are no logs in the service when we deregister a cluster/ host
c47dd8ac66c64c04051c0c7ab974c8fde3c4267f MGMT-1021 cluster install will collect multiple issues when trying to install cluster. Disabled host will not return error when trying to install and state in the same state. Add subsystem that test cluster installation with disabled host
373440a899e3b3e92f91e85119e26bc6dd3d6f3c Add env to skipper DEPLOY_NAMESPACE, DELETE_NAMESPACE, TARGET, INGRESS_DOMAIN
72f83dd040002b490c575cb2f8e4d07e6c3eda3f MGMT-832 Update README file for oc-ingress (Openshift with ingress configuration) deployment target. Option to deploy UI
52c302ad7d9b63e17f32f8a1cc114124a60f2a73 MGMT-832 Add deploy paramter to oc-deploy target. DEPLOY_NAMESPACE - true by default. DELETE_NAMESPACE - true by default, used in clear-deployment target. INGRESS_DOMAIN - In case of TARGET=oc-ingress the script will support specific domain or getting a default domain from ingresscontrollers.operator.openshift.io default openshift ingress operator.
1cbaa403dba6f709cf432c492555501818dcb5de MGMT-832 Define scality resources to 2000Mi - it will overwrite the defualt resources limitation if not set scality may fail to start
73c1e78d8b4c2ba9097cb929000e36d8bba357c0 MGMT-996 - Validate the format of the pull-secret
c4e3119b31f95424b279ab4019b8918815bb7d7b MGMT-1027 Discovery agent image should be taken from ocpmetal org in quay
3acd537eadf655fde18648cab93b2a603a99de1a Added a tool to use mysql cli on DB exposed as a service in minikube
ecf569391c8203689a93dc48a417a4e07e9b94d9 Added a tool to get the git-revision of a running pod
4e32622950b68bbe178e931efb6c5d940e712638 Added UT to cluster VerifyRegisterHost
5c0fdc9eaf707d44ce108b768ccb3bc93b6759e2 Autogenerated mock_cluster_api
7f64ffc92e42b12b9540373f43a2288283c799e9 MGMT-779 Prevent host registration after installation has started
be59d1e18367228eccdfb3eee739fa4767d03376 Fix flaky test, (download_config_files in error state) The test fail in case the node that fail to install is the worker. Updated the test to fail a master node
b33fc3375db54c38285ced1b91cc81e761c893f1 MGMT-998: Clean ISOs older than 1 hour
448a67d8e35aeeb0caeb40d2f2b8ac425ff7d0c8 Revert "Get the agent & hardware_info image from ocpmetal"
2da374458802ed20e4f950fceefc1a07c6890dde Get the agent & hardware_info image from ocpmetal
8302ebda7a253b43ab169d3999f16d8abe2771d3 Fixed UT
b75418905f077fb8685e36386cdcbbc4ac513ae5 Autogenerated mocks
3a9f6ac94ede7e64438932b74b67dac6e60767df Moved the logic that check the cluster status when trying to download a file or get credentials to clustrApi
b78b67363a409d9340a3d30449b944cc68a9afe8 change to image-builder that can run also in non-root environment
e3b5455fc3648c2c395376347ce7b7680607fbe5 MGMT-1001 Fix transaction rase. if a long transaction didn't commited yet then another transactin may get hosts old information and commit it after the first transaction. So it will overwrite all the new information with the old one
2b7aa5707259060527f4284fc24f523eb79c95b3 auto generated mocks
e06f748e647b987dde102eaa5089113a0bd5df7c Set DB parameters: db.DB().SetMaxIdleConns(0) db.DB().SetMaxOpenConns(0) db.DB().SetConnMaxLifetime(0) Change getClusterInstallationState to use DB from RefreshStatus Fix set bootsrap to work with transaction log fixes
c38b83a62d9ec9f96551da226668bbdf6887675d Return host state monitor
c54e0936963ae2b4adf5f8a6e3c5b2c5d767d017 Updated timeout waiting for cluster ot get to error
ecdb0e3e899b6332aa701c09aa9df31940302fa7 MGMT-960 Setting install start at and completed at timestamps
d7aa6b97d7e816113832ea60461a39f3644cd991 MGMT-1012 Return host network as part of the update cluster result
a379c08b96212e63a8bc5c8cc85d7c0b98cc294a Added subsystem test
e3f5ae1509201406b2e3df3f3c63132c31e831b2 MGMT-1005 Allow downloading files while the cluster is in error.
038011db445bba0b1c5ddaf3a0ffa965134dfd23 MGMT-976 - remove support for None platform and for openshift version 4.4
9facaf0b5f385619b1bc7b378bbfc4ad5601ff94 MGMT-832 Set new default role, service account and role binding that enable basic operations for non root user
42be52efd969ead6592561f3e15d8d1f838aa280 HW inventory steps should be sent to hosts in insuficient state. Made the insuficient status info a little more clear
a26c850e3e9e7c808d0cc0e93c4b376e709bec24 Fixed overriding default attributes during UpdateCluster
f8ccf641710707509d9d44cb33ab5aa6687f8496 Moved network params defaults from the cluster definition to the cluster_create_params
109f90501912f9f0004e44b7375621bd4e435f26 Disable upload ingress ca subsystem
91092f5dae486d5868caf171fd542e4a5a0b3da9 Revert "Use Eventually instead of for loop"
f656f0314494ff8fd8a0c15b40c9f008cdee4950 temporarily didsabling host monitor, currently there is a race issue between it and installing command
34d3f830c8f4c6147c4aa5e0d377fbb5c2fae568 MGMT-984 PR updaets
5a598f29f0d37df8ef1815c75f9f2160c6177162 MGMT-984 update tests
d17917326cfe8c72ed6d92067e78271c926bf23d MGMT-984 workaround for the first ISO download timeout, assisted-installer should create a dummy ISO
de5577cddf46b0b63e0c501c28de53b0c5e7861c Use Eventually instead of for loop
eed830418b2b05a2b8f3b5784156959a25718487 Autogenerated mocks
4e931682d019a04d8d2b2f0ac67da4840dbb9235 MGMT-924	Rename kubeconfig without ingress cert to kubeconfig-noingress
12f3a82285bb4e3aefa8ae1ee80d73326d33b2e3 Add subsystem test for installing a cluster without specifying the network params
e5b702e68c94fcea894a65add9bdd7b1add8868b MGMT-981 Added default values for the network params in the RegisterCluster API
55252ec5bec23e7afa59fc1292d1f62c6f3ccc10 Autogenerated
9fcbc6710435db686ea72a9b124f21529e7def4a MGMT-981 Allow creating a cluster without specifying any network options swagger changes: Added default values for service_network_cidr, cluster_network_cidr and cluster_network_host_prefix
ae7a9939f650d55e643078f499ed25cb265eaeef Result of generation
15b49b2c30418f34f4c95cc1b85e93538251eb48 Removed status_updated_at from required fields
466e780657aee7ba8efff671fbd303a9cad7da86 MGMT-985 - Update the pull_secret_set attribute to true if the pull_secret has been set
6e3573106ade57d2c014f2a631c5b89ecb08018a MGMT-985 - Generate from swagger
4bcba054053c16cfa5cd15420272860fdde9579d MGMT-985 - Added pull-secret-set to swagger
8cbdd5ba7f87372497c8b6b9efee8a9e88493fd4 Use gorm.DB.Transaction to manage install transaction
b2a39f3249201b60c0c66c773d1cbe942a04f3a4 Rebase changes
c9962cebacbbef88e17e18f3f7eb102126a27ac3 Fixed PR comments - Removed RefreshState - Add flag to VeifyVips that forces existance of vips when verifying - Moved host refresh during update to a function - Fixed generated error by update - United verifyApiVip and verifyIngressVip to a single function
4892ef4adbe3c348bede94e235f9da0df3c5d616 MGMT-911 Test modifications
2127654e36b43fa75090b98b31ee9c3a653f329e MGMT-911 Code changes   - Moved machine CIDR generation from installcfg to update cluster and store it in DB.   - Make machine network cidr creation rely either on api_vip or ingress_vip   - Remove API Vip and IngreeVip from cluster creation   - Add verification that all masters have an interface with IP address belonging to machine network cluster   - Allow host to be in known state only if it belongs to machine network cidr (chosen network).   - Allow cluster to be in ready state only if both api vip and ingress vip are defined.   - Remove dns vip   - Return host networks as part of the get cluster
6dd33bfb2520c2d9cb09b5093ac83dd0eec3bd43 Swagger generate
bb12e28f1432b8c0a78e1923fa6bc2d5c75e7e3e MGMT-911 Swagger changes  - Add machine_network_cidr field to cluster  - Remove dns_vip  - Make update fields to cluster update operation nullable  - Return host networks as part of the get cluster operation
69e6f032d381fdfe11ef7f4012a2053c3e420145 go.* files pkg/job/mock_job.go
8f60b4622f91a97a1cbf3bb6d7b532c63631e4a1 MGMT-656: Candidate disconnection monitoring
d4ec78ce9561157675771627433d8287cad73356 MGMT-656: Autogenerated from swagger
b514740ceab9078e5d798fa8f352f3cc338d435a MGMT-656: Swagger: add checked_in_at host property
661bc2c5aa3fd67c9fa2e3e1b11f22f3b3720469 Add UI deployment
4782e4cccb0eaac167ed6b2c76d8b29bc4944f6a Makefile delete s3 bucket creation ling ignore unsecured s3 operations - support scality Add s3 client wrapper package and use it to create s3 bucket when service starts
eb509dec07011baeb3e50ed9d3612b00385a0604 Skipper mount KUBECONFIG path and KUBECONFIG env
c9ce184c61c3f3bcd8e41d032e30c70df65e6700 MGMT-970 - update status_updated_at attributes for host and cluster
7293f2f8c5161b8da71611564f194c6f6c19ecfd MGMT-970 - After generate from swagger
33dbc2ab05ff3f4e019dfc7d62e7ce53d8bb1933 MGMT-970 - Added status_updated_at attributes to host and cluster
c516c156a40c4100f4cebf4de98780885ed283f6 Revert "MGMT-976 - remove support for None platform and for openshift version 4.4"
fa6d9f00b9568ffae366929bbb790a21bb755fbe Updated override release image back to 4.5.0-0.nightly-2020-05-21-015458
ce58ed82dc27d2eb7214353baf048a77e6fd7904 Added console_url to get credentials response
169ab34eef4ba01fc05d8eaab7c843786d15591d Autogenerated
378a2b9cf963009a8701e7dedb2d293e222b3314 Added console_url to get credentials response - swagger change
dc38d57232639c16d0ca2725d982c349067dcf47 Moved the health and metrics middleware to /pkg
12446ce648707263d2c8970125cf14b39ab0b1a6 Added health endpoint
c1b2eeae729b14e4c3b079bcbd887992976f7e9d Adding metrics endpoint
9ddb0f10e32f84c4c2f6c8af7298946bd04bc2d0 MGMT-976 - remove support for None platform and for openshift version 4.4
bc779acd13ce814d895c16424b2b1eae88961057 Results of make generate
4fca02428cd2ca454818760cf5a245e7cc55c6bd Fix versions of all that is installed in the build container
d9d82b4e892e1b53ff74d71a8569d3daf525e64e installation can occur only when exactly 3 known masters are present
5dd829bd690d95d70d9606542d9985b59ed7c46a vchanging 4.5 openshift release image
6258d9390e40007d0b63aa773ae1f6ec460d003a changing openshift release image
eee180e2896183abd745d8f6b4e6632f2a830f99 Adding subsystem test for kubeconfig and igressCa apis
72b73c6f64fad7e9eec534152e397f7454bce9b2 Autogenerated files
31e781ddb1faadc90aca3fd82a8f9c2faed546f8 Adding unitests for ingress-ca and download kubeconfig changes
cf38abed03965f498c90cbe46a24ada4fe10be3c MGMT-910  Add to bm-inventory functionality to upload ingress certificate and add it to kubeconfig MGMT-925  Add api to download kubeconfig file
56d8b4138679dda20ec35288c8a2f89c19a43b22 ~swagger autogenerated
26d93cd1b9f29c662ca8e256513cb552647e25fe Changing name of ingress-ca params in swagger and adding kubeconfig to download files(temporary)
ac884747b2186501cdf79a35e47da41bd586326a MGMT-908: Autogenerated from swagger
4c64e58d8c503ef9ea90546879f0ba2b6e4e413f MGMT-908: Swagger for kubeconfig APIs
7060ce632338d46ac628f2ec86aea3ea4af34829 added swagger ui
4b967de28b386f50a9632a1fd3cee8304d98f752 MGMT-796 Implement connectivity check getNextStep
7f45cfc3409310975380d0f63446b42a693d61de Changed GET kubeadmin-password to GET credentials
97f31536bdad5588a123f9246d4dc4d71b13e9eb Autogenerated
0d7fe83159a7ecd563d04d2ee806892d85885754 Changed GET kubeadmin-password API to GET credentials
3362ebb1ecb87851cd994ff98d70a370796be132 Added subsystem
455e383eafca56c7cd8e4fd853d5b1169e4d351c MGMT-914 Add API on bm-inventory to get the admin credentials
17244d57a5ebf38e19d8246a3dbd92754664f4c9 Autogenerated from swagger
35f84737c1e382aa14becc5852ac7b94d1f59a00 MGMT-914 Add API on bm-inventory to get the admin credentials swagger changes
25333580c7e8aa25e8abb1b9edadaa58938deca6 MGMT-950 - set DNS VIP to API VIP in order to pass igntion, when DNS VIP is not passed from UI
23c5cefc26f05f56db386726a1755f3d2879c1c3 Set image ssh_public_key length to 1024
f69eb70441392345a633cf6c419213c9a3db1106 MGMT-844 add to cluster state info
033d88fdd050c5ae207815db19b63fcc142ff7ef MGMT-797: Code changes for storing image properties
5dc85b28b2bb8345dc818d54d17b71a866dc7e57 MGMT-797: Autogenerated from swagger
95e1023621c4f53156747b4893f333b829ae49ec MGMT-797: Swagger changes for storing image properties
41ff0f209628608031ad48303631522841b9dd2e Update README service update with namespace
62cdcc1894081597b1100b5af24ec42bd58c7f8b Added request-id to the events
4515ca9913b6f970dfe59fa0d955e2702979a44a Update swagger
e7f115bc7871e5a30cd4c358752f58b825ec59a0 Fixed review comments
416dec2ad689b0ea1b6f9fb5c2b4cc071ff1ef3d Code changes to support events
d8762b40486fffa6644c53072eda09fc8d61f1b9 Added basic events API - swagger changes
dc18f98edc9ed37e7e2e336231d88b1b4eabfc83 format sources
46dbc2bd6b1ad9432cf0def72d708fe2f0d8abcb MGMT-931 auto-generated
3cf6e99845616da62b5069f7883c166831a7552f MGMT-931 Swagger - set status info length to 2048
1dbe323d5f03212085f322735e3b9ae13492522d Fix envconfig parsing for ClusterStateMonitorInterval
548dc238009b56b8aeea929cddb55ef8c4c44fae Fixed logging
f21da1d305a1eb7c66df71273d019a9cdc9d7b9a MGMT-809 Align iso ssh username to be core
8e54d69f5939975f40ff091e29ed7e25e81df5e1 PR #5435
3abc27e45c20b4e0039c52646490be34ccad16e2 PR
d093e06deb608f1322c09788a642ebe679274863 fix cluster install, timeout waiting for cluster state to change
1ff4c5f915491f4ec6e6f9cbca0095e9e8fc1a9b Revert "Disable flaky cluster state validation in subsystem cluster install test" fixed test This reverts commit 04067c19e5437a9b96952b4863d7bacf14afd6d0.
04067c19e5437a9b96952b4863d7bacf14afd6d0 Disable flaky cluster state validation in subsystem cluster install test
f6403fb153d45bcb3204b61e28c410a6ec029fe2 MGMT-799 discovery agent service should be restarted in case it exits
2f285324d59e08d47b6ad048749152750ac3a96d go generate
7e5676743e9ba22ce849b56778da04f5d932335e Re-add installing-in-progress status
767bdc6f3c3ade8ae166139da27133e38b4307da MGMT-761 move deploymnet to assisted-installer-namespace
84e01c9e19b9af1dcb5cb5f543a626c6b50cfea3 MGMT-915 - adjust hosts section of installconfig to reflect the correct number of hosts intances
042ade08f05ff9fb37d3bab6cf8efa89ff64a75e go generate
8ddc47654e52e8d45dc59d0e87c5f356ec813984 Change register host to new state machine model Fix registration API - Register will check the current state before activating state machine Cleanup existing code
37b74697a5e86f9fa32f6c2b72bf97c4740e1291 Add stateswitch to go moduels
1c7a5ebf0f47e208b5f9d78e1802665b12237711 MGMT-913 Added UT - Validate install command
2fb93850914b2b86512f2335f888625408f9455b MGMT-905 assisted install container should be named explicitly
5357219f1649be8c05c6ff993ec80e186309785d Tests modification for MGMT-868
3de0c7d579528ffcc6e46f5fea01b63ad2571b2e MGMT-868 Calculate machine CIDR and add it to cluster create params
3615ca2a0133881cac125279c1042e506532c104 updating the openshift-version release
261e029f94b85e6d1f5535669beec0b5858ada88 Updated generate-from-swagger volume mount to have write permissions
d57a89cc6daff96a9bf36771ff80fd7b4d92dd66 add support for 4.5 openshift version
36a6f4849ed113ecf230e4b57d5141ebbbc5b6fe MGMT-822 Test modifications
d5858c4429cbab45a0db772d0960843cd0cb73c6 MGMT-822 Changes for new inventory
fdcaa6f5ab88f7b3211895411eb95e495b5a750c MGMT-822 Swagger generate
f80d9f2049ce5f16eff5b75752775eb28439d30f Swagger changes fro MGMT-822
0de8d4a105501324cc9e506c0bc596151eb88734 MGMT-820  - add ignition manifest generation image based on openshift version
03f0ee529f3357ca256388ea586028c6ebc2aba9 tests for MGMT-747
62884db1a85309435c2513664d739445470110a3 auto generated MGMT-747
ed1a341bbfc9468fd409d5dec6ec7812f589017f MGMT-747 Cluster status should be updated periodically to to reflect changed in host states
90e4243d82aa7d810d5e8dad9356ba60a5b9111a doc fix
03d0733d5061eca922164b07b7c5dfa04d989300 MGMT-820  - support platform none nd platform baremetal for ignition generation based on the Openshift Version
c985da5ebcf2bc20d4fd618d81ea1eeb1f9ea6dc MGMT-848: Clean up ISOs that are older than a day
2c429a0e38169d2a7fbf995e722ae7522ba055d9 MGMT-873: Code changes: change install action return to 202
61401d2e5e315ad0d41678bf57d13023acc2c286 MGMT-873: Auto-generated from swagger
a85c701985ed92c4eae43d401de739f703a635e6 MGMT-873: Swagger: change install action return to 202
e2db5c4305638814adeccd933fb9b05c9a1210d9 Revert "MGMT-747 Cluster status should be updated periodically to to reflect changed in host states"
1e612bb4eee86a2f3cffe8a11f0b12663a6699a3 MGMT-747 Cluster status should be updated periodically to to reflect changed in host states
3ecc879f00619d2157e7d26830cf09b308745f21 Remove postgres deploy yamls (unused)
fd6bbc3f587ce8649e9679d526249ab0c26f2357 MGMT-853: Use PVs for mariadb and scality storage
a9f19858eb255a02ba72620a5998e8605ca86db3 Fixed error in image-push workflow
d1f7451030d3674be3e67b42afb4bb6f7ee3ca92 Add git revision to the container's label, instead of a file in the filesystem
a45c55aa8cd95789ec22acc82f18008d142e9cb9 remove __pycache__
c2eaaac8768ce941acd6fc4b5e4777e87b5e62a6 gitignore fixes
95b7ed2eb7e16e2f6a1d04cfab37dc1c8ce666be update go modules
80c1a6eb0f7e26e17f27607abc26ca1a9d75885f MGMT-808: add reason to all HTTP errors temporary adding the full error without filtering, later will filter out only the relevant error message for the user
b0fdc35b7deb786fdd0e86c86923add326bb0928 fix subsystem
71d9f0337d4c4a8ba03dd95955c9019acaf25156 Use predefined methods for setting hrefs
7ec1c17dcffa6b30b0173d37405dc7ea1984df68 Add support for having multiple different dockerfiles in the repo
86d0c6118d468116a6edd55ee5dba12504531ac1 Github action to push the stable image will now also push with the tag of the git revision
5e51be03f6a5debd63aa0bd12abb48061806e88b Added /etc/git_revision file to the container
662ab8b7353fb87091be3180a347dcc34e45c5ea Add __pycache__ to gitignore
2d39913c5b7ec0a0e086d258c978eab303d47032 MGMT-854 - Fixed commit after rollback in InstallCluster Also fixed the error handling in that function
f001a5605b03412df99df2335d09f630e0bcd18d Move deployment to python3 scripts Convert all scripts to python3
f3a0bbd95eed5afb24fbeeb7af638ace80031ef6 add pyc to gitignore
a7836211dcfc0e3cb473686e80b8e04575cc4235 Change build container version to go 1.14 Add boto3 and python-pip to build container
a3c4d59adad78e11d0f2e9e18788cea1dd8cf942 Revert "MGMT-848: Clean up ISOs that are older than a day"
91de37e4e4da54065bfaf2dd9329d85b4dcb4a6b autogenerated : Change vips to ipv4 format in response
708ec3bbecf495e5ae5502c4819bb9790ae03618 Changed vip format from hostname to ipv4
602e0a4fb99b1df2aeb3336e7562796cb34f64ec MGMT-849: Fix clusters href
2745f6700f46e43fb338096649f1a3ff8382c12a Add .*.swp to .gitignore
82d05890d5fe8d9e3b937dc481e71efdcabb3c0f Add a link to troublshooting document
733bec7bfee16d12ba889e66af8ad1243cbef03e MGMT-848: Clean up ISOs that are older than a day
ac443e57211d2235bfebc249913346accbd37812 MGMT-841 Assisted installer should use kubeconfig-loopback Map network to host so localhost will get to the kubeapi server running on the actual host
c48a7aa5ff15c6598cd191901eb12d1c2543a9d1 fix install command
2c9d9c82e876b2c601e50c16d84de9bf846f1202 Revert "Fixed isntall command"
78e91f761943781127fc434bd5f98cbb6f944538 Fixed isntall command
3dd8f1379ecee86a1ae533506ffd7950fe039281 Fix tests for MGMT-688
a08e9fac0d08f1e95914cd668af380d75753b986 NET-688 Swagger generate
eb7441687111228bb67abfdeca14a8cfd9059ca2 Swagger changes for MGMT-688 - Ironic output compatablity
e7c4f0afc20ea1ca62d7314bb582f60e5522e1de Code fixes according to swagger changes for SRE
0c10c86739352c814c5ec5181bd99a5abb874f5a go modules
8b03242ceb2f48d29a12a1e6737811a7d0b0d654 auto generated - swagger changes for sre
98c7ce4189f4ad5a1f1f769e185a7706d5fc048c Swagger: change according to app-sre guidelines
1b6ae9ae5b785f028692d93ada8aea4ab042c9c9  MGMT-703 - move install logic to getNextStep
26a507df4f53fc7b00d1db8dfac2a122f79f3346 Update readme instructions on configuring docker registry
505af64160ee99a4cec32638ea65557ed046ab6c MGMT-815 change host status to error if progress report failure
84b69058ec25edeb218b1631752e4f26785d43bb Remove deploy-for-test from makefile Update Readme
3b8c101ce9dad125ec6c9ea805d1c6d15b126c72 adding installation to cluster api
d902573a15fa3aa2fd293b5e15b6baebfc7f7b3a Adding openshift version validation to swagger. Currently only 4.4 is supported
b559b208497b31fec61719d7520508c72789cb82 MGMT-765 Passing openshift version to assisted-installer
bf71bf788b435ef562b90c022274425a40676c07 Revert "adding installation to cluster api"
fc6295a9b6461d122b5b659777f4a81ba430bd9b adding installation to cluster api
161ac9ebdeb778c4c43006592f7b9fd8aebb5c9c Create a build directory on deploy-all and deploy-for-test
b83342a05cb950ca22eef8208b3a7b3d679e933f Added a periodic thread package
53f78363730ae716d15174f4cbd0c0c33aeec8ef Changed github action to use python 3
007ad54eb595ffb1fb0329e70648f294229e1e53 Add output of the go coverage tool to gitignore
00bc5fcc7ffd61de638966332a67f55db6f9a4d9 Boot device ordering change: 	1. Adding name filter for nvme disks 	2. Changing sort from by Name to by smallest size
14f220e956258739ba5aefdfb0c44a498cf0b802 Fix proxy configuration, remove http from http_proxy
a815e5d1da76f6589dcd5bfd139171c0b5ad3269 Pass the host-id to the install command
86859f0354150ca618add97da343848b9e349e91 move deregsiter from step api to register api 	update tests 	update mock file
599655aa211b70cecdaa9750c2e62c8f8d73eb35 code review fixes
04cb8e5dc144280c0003a90e581d1749b2e559d8 Inventory use proxy url to define ignitsion proxy envs
c7a186fccfdd8d7ec6d9884a42510df53335495f auto generated - change proxy ip and port to proxy URL
ca050189ab870b3b9713e7906d77df85a23dc97c Swagger - change proxy ip and port to proxy URL
1b3483457026218d8c2b5db013ed8f1047345a2c add created at field to host definition
94b8e93b1bdc59ebe44f17487aa34e07c8551bd8 Swagger add created at field to host definition
03237e4be76277be89b8b3fa56239514ce82c593 MGMT-652 Implement cluster state machine      Implement a cluster api interface supporting 	 * register a new insufficient cluster 	 * update cluster state 	 * deregister a cluster.
3a4b84721362ee9cd4cb7eb78472f8b2aaafe062 Remove 'http' from host parameter in bm-inventory deployment
ef1903511e7cf73a32da26eb3a5fd7471953b594 Set HOST_NAME env to configmap deployment Add sleep after deploying services waiting for the service to get an address
b9e41db3ccb5c809738f1ee793e8be322d61c08d Add HOST_NAME environment variable to s3 configmap and use it s3 deployment
f3561c5430b09458ba1f3e1e95a44348241d1617 deploy maria db with LB
524cd1530bb15e5b08da74f5f014ae0ccfb69aef wip Makefile
c900b51f710087d93892e6df193e2012365638a2 Set all deploy login in makefile without external hack files
8c9e17c128aedd94ffcd2b155a4531cbd4b47ca0 MGMT-677: Add Progress update API to host API Add subsystem to test host progress report
383110aa73f123443c049f658c34aff6f76a4b46 auto generated - add progress api
a5613ad70744758468b475281694b2b04a1b5bc1 swagger progress
730c226994f4844c953f6a4fe78e474e4037d50f MGMT-705 Choose boot device for the installation, taking first one
4149e2c731cbf602a2551d2d8c69efa6f9574d3e Revert "MGMT-705 Choose boot device for the installation, taking first one"
ed2bfc6186b63e129b1a1c94108d57af7b248379 Revert "autogenerated mocks: Choose boot device for the installation"
f6cc49b2abc1f13c8dbc72223265e73c1e1401bc Changed name of image-push workflow
dd569e993fb803a7a0233f07c6fe8b0790e7e4ad autogenerated mocks: Choose boot device for the installation
67087a5a800b695b76fc476390946aac1c5946d9 Use the proxy params when formating the ignition for the iso
6ffbb00ec58232d87c918bbd97d82276ec81e9e3 MGMT-705 Choose boot device for the installation, taking first one
22e22c41d00ab50db9d7d81e556b29102d7dd2d3 auto generated - resapi mock
4023f7e356c151176c8f2e445d6d1cd64edaece2 Generate mock after generating from swagger
52c848f7c6075509801d5b8308db2c0f1c7b5ca4 getNextSteps logic and unit tests
78c1202f391660d839e237d8ec6902dfcb63f7e7 autogenerated: delete hostname format for proxyIp as it doesn't match ip format
c9a197462821e9696006115d54fcf6b831fc17c4 swagger: delete hostname format for proxyIp as it doesn't match ip format
35547a199ab14852b15e70ce2886de8d30d9611d Generate mock for the client
1f0552ea36c35b1027451100f7d130176c234ac9 Fix Code to handle openshift version on cluster create
d1589385fead5283d4822f4186023e5d033fa0e2 auto generated - require openshift version no cluster create
e98a08dd8136c06b3ac742f21d49a353698ea706 Update assisted-installer to latest image Latest image uses the bm-inventory client for fetching the files so there is no need to pass the s3 params Instead we need to pass the host and port of the bm-inventory service
7d33915487107236ebb4ce94e7f88f42f845ef36 swagger: openshiftVersion set only upon cluster create
6371bf139fab13196c77717c013df98c705ea9a2 replace error return with the correct one
bd2fb5bd88f05ba765daffd51cd872783100982d Use stable assisted-installer
82784795ad0c0661ee30051acdff002e7ba8c53d auto generated - added status info to cluster resource
fdd89cc077873167c7fbdf1bead15e91d0d68399 Cluster state machine: add ready->insufficient
9e7fb76e19f2b0729cf2616c4befd84a1a8d0ae5 swagger: Add statusInfo to cluster
d8c0eecc7a96547cc778cfc58817f46b66aea632 MGMT-694 Download image should use ssh key from parameters instead of cluster ssh
82d667d96eb65997e8e414fb3f6048f6c15ee3cf MGMT-697: Split download iso to generate iso that will return iso id and download iso that will return the file Update subsystem tests for image generation and download
35a82513fb84ee4b7c02bf4a2004d0c3a66e9005 auto generated
411076587e7940ea5079f18d42421c2ca5db5adb swagger: image id is required
27e78f3a89272352843879440f3ee1411beae826 swagger fixes
317ee4f6d88dfc13ccac68fac73a84e6f5f2c22f MGMT-697: Update swagger to split download action
e0a16be1d9150b6044d7de3d01e31e7414f91901 Change html template to text template in addInstallCommand fix panic in addInstallCommand, change the function to return an error
c58b8c5b786ec35cfa6dfc1c2c741d093e210630 Moved to common 'quay.io/ocpmetal'
6faab24b6f1ce43b42f77ca51c185a6814b1cad6 Remove cluster's createing status from inventory.go
49b4dd8b694969429caa0aeaaa0a374476100136 auto generated
4f4df5f3b1f560e71265b89c77bc2c814ca0e19f Swagger, update host and cluster states according to documentation
71b1ab94fb6f2ae00cfdb799b5c34ca95594872d Split host api to API and StateAPI all the different states will implement StateAPI and host manager will implemenet API this way we can other functions that don't involve host state into this interface
82b2c5ee35bd34da141f23e29c271d37c889ca1b Change statemachine.go to host.go and move tests to host_test.go
10dba00f5a3dcdcfa39e22861b9e485fd38b9a8c fix file name
dcb9e6b2124ee0fe3f62a14e5a09a71e82827d09 Change default service version to stable - the same as pushed from pull requests
a0544bd403ef4288166552b23bc09293b6171d20 Allow overriding the installer-image
fd7bd5d0487467a9d61e05883de52d159d85cced Change the install command to use podman instead of docker
6dbf54e797eae71e12b851dda8aae3fc5bc39680 change golingci to 10m
1bc15697aef095ea8822d9851bf8f3c75523843b Added action to push image to quay
dcb62c4ae23d72027327a78d5f7abc2c546a4ca3 Added workflow for unit-test and lint
b0fd0eb14c19a5967e640a4fc89553929f187e71 MGMT-659: auto generated
c99e0a78dadf0dbe1825809b8dbf06597bc6fe6d MGMT-659 Generating ignition files should be done only once
fb56c8e6beecd641ee438b5257899a77e01136c9 Make inventory to use job api
cd04d59484411bfa5b2448371cca5161436ce136 Add job interface. It is wrapping k8s jub execution and monitoring
68947cf1bfb3d03d51ded183bc42d6b2150993e5 go modules
c6a796061c4f99b144d4887787f2be6d42165f10 Set OPENSHIFT_INSTALL_RELEASE_IMAGE_OVERRIDE env for the generate kubeconfig job
5e198540a73f1e5810f646c5db4be2ae60a48de7 Added basic install command
84c20908ff9b50087c7c202523e5078654f88650 auto generated
f25e2f7610fdcb2adbf18ab6d8cd3b6c5c7bbb09 Swagger change hardware_info to hardwareInfo
b21d593d926e3287e23a94d7da10bd7fd4bf3a06 Fix Job monitoring not to sleep after the first iteration.
80a984896d8b19da6a2e10dc0054dde871831ec3 Hardware validator support getting configuration from environemnt variables HW_VALIDATOR_MIN_CPU_CORES default 2 HW_VALIDATOR_MIN_CPU_CORES_WORKER default 2 HW_VALIDATOR_MIN_CPU_CORES_MASTER default 4 HW_VALIDATOR_MIN_RAM_GIB" default 8 HW_VALIDATOR_MIN_RAM_GIB_WORKER default 8 HW_VALIDATOR_MIN_RAM_GIB_MASTER default 16
4d5fc659780fb9d5804328951cdb0b72da863c1e typo fixes
ff627116da57fde751ab9a2923fd7d5381a86b81 Run agent instead of introspector
d495f77f925f7b7b152b9ca601f12262bb3caa82 Fix hardware validation logs
d2938895770bce67064c4269cb2eabc018064970 Add retry to get job in job monitoring
45cff8589c78cf27981c3035a329cb6631009184 Increase golangci timeout
aec73b5e2c26d5fc2bb91b8c6128b54e59343e9b Inventory use host api Add subsystem test with state machine and insufficient master on cluster installation
89cde9821354590129e1def03a9bf6da95f3dd07 Add Host state machine - set of APIs to be activated on host. State api will look at hosts current state, activate specific function to the relevant state and update DB with relevant changes State machine install operation support external DB object for transactions Update role support custom db object
36ec38b26fd6f4c4532d560afda3615de56abd83 Update cluster state machine
81f42867c67a2543ca8ec338c6efd5d3f15c3e5a MGMT-644 Install Assistant should pass s3 credentials to all s3 related jobs
bd28f6977faf50066be59b640392dae3a7ff8c11 Add sleep in job monitoring
093d350483964f2967bd79d131ad29c77f64a5fa Fix rename hardware validation sumMemory function to getTotalMemory
937962465a0b19ba8a63a5205fa961ea4b2916d8 MGMT-651: Hardware validation without disk space master: 4 cores, 16GB RAM, 120GB disk worker: 2 cores, 8GB RAM, 120GB disk defaukt == worker
7695a3fa9307bdb9c05c2e1459e2024bbe260c40 go mod add units
f624f814917e1451e28c99db52778e121434501b MGMT-660 Fix job monitoring to wait for retry to finish
a84fd43cc57d34176114c066a17a157584237e8b Dummy hardware validator
2fc93bd805dd8f2f312ba41924e88b69c9632c0e Add gomock to build container
6db4b520fa37dd4052784a3cb707fd7ab85385f1 go mod add pkg/errors and mock
fbb92cb5e9ce32d162012a8d7f2e1b2a411890e6 Add unit-test target to make file, run all test excluding subsystem Add go generate to Makefile
a8969b81237753a6be408bfbcd3f878a056a7b69 Fix HTTP Get error check. validate status code as well as error
e5028fe93231bb756a0835c34ac3bfcb1d7bcf2e clear db before starting subsystem
453ce939c4dc1c94a71bef428976407f954191b6 Create a function to generate iso name
46ed361b766512f7a3a71683a4d5e3fab6672457 Makefile will clear generation-kubeconfig pods after subsystem tests
85b6f945be28075fc4bc5350d5ac8d589df3aeb7 Fix Image creation job. if a job is stuck no other user will be able to call the api, the fix to create a job with a uniqe suffix.
aa748d0fe05989283e8d98a08665364b362c325f Add content-disposition header to image download API using a middleware to the responce content-dispostion will set a default name to the target file to download
3bb45221d21d40a9262c59ce416210133bb60257 auto generated
d694ba3df13ed5ba907d65640706abf244b78eb6 swagger change download image file format to binary string format in order to support rt contnet-disposition
fdc3fa229a42439cc31a85fe3d5e86d262516179 fix go mod
179b704105337c5c55ae4b9868d2b9ba75c3315f Added error to log.fatal when cannot adding scheme
21933bab3477558b89e4f89c189dd6217281d19a Added request-ID logging to inventory
84e619a2aaeacace1a4da330db7eb4831e3dfd18 MGMT-643: Store hardware info reply Add HW info tests
a6a2aad586bd153e4e81fa6a434019a63bedf56c MGMT-643: auto generated
042836d7f0f0195894f67fae71312dfd74da7c12 MGMT-643: Update Swagger hardware-info type and change introsdpection in host model to string
ac8e077be5203b0510fc4ac7b16955ee59ed6c41 format fix
775062480cf09d322d672a343e54906c4de64133 Add readme info :  Linked repositories
ec099d830053bb485f9c167dbb8b57235d6b5d28 auto generated
2973cadee5d6c884c2a5998f43fd598994d53d37 MGMT-611 Add API for getting the cluster kubeconfig
e3286acdf48fb3c69f467e8594f7045642fde760 Add goimports to build container Added format make target - it will run goimport on cmd and internal folders and update the files
58b04d862d74bd94f75c389131c5abcfd4383a46 lint fixes
247b802ebaaf1a1a0b3f463b42306799f2035b33 Add linters
091687288e0fcb874fd20e515dffd644443bc14f Add linter config file
a44efaa827cb94b452d433d8be8654cc89fad3a3 Log debug step-id when setting the command
6eadc598616f79650d40a68043ebf7175a89400d Run introspector in the host
b5297df5873c76f0bbb33a6aca9a3202c96f88a5 Support agent replacement with AGENT_DOCKER_IMAGE
08a459a574097305dd4824eb3868f40c5654b1f9 fix lint issues
8b87dce8b38f9aadf69ede0672032ded2747671a Rename subsystem/utils.go to subsystem/utils_test.go - fix for a lint issue
9d67aef5974e7a578af2bc709d6b742cd96161cc Add lint to build process
a4f4cdefab895badfb404da538e80bc159575b26 auto generated
4a200617ce2c7f908f28f4442c8398d0ad6d7bba Swagger: rename next-steps to instructions
3998920523e617b3f13f2b70aadc8d699b38c302 Update node state machine
7ffd97a0bf25b369f3dffe4ed899e436143296af State machine updates
703f334c0adbb7a49c068b6b14b633eddd50423f MGMT-639 Remove statusInfo connectivity and hardwareInfo as required parameters in hostsaAPI
ae3e022905167b5d87cb2ef7f0e450c828db2fda Once install is activated an install-config will be generared with cluster parametesr. All nodes will be set to isntalltion mode - Without validation at this point. Set all cluster parametser when createing a cluster Fix update cluster to update all parameters
d3990166c5bd72b0968a8cbf79a257906a2adaa5 auto generated
06942e939f7fb2009ba3b05490c18faa14dc69cd Swagger - increse pull-secret filed in the db to 4K bytes
b65e16d38c57e63b38eca7cc85f0450d38fcdf8e go mod add yaml
6f2198f12353ba371e0c2e31dbdad802c4977051 download image test bad flow
b3f2cbb7bf8d92d2b57bfea99a33d42834e16979 Add download image system test
15ee055c52d1a8a0a6681aeb702d26a27b9c26f9 Support system-test More complex tests can be run only on full deploymnet system By default those test are not running and you need to add 'SYSTEM=1' to the exectution of the subsystem. If a test have 'system-test' in the description it will be executed only in this mode
61192ed29788b434c6fd5b9a12095288593ddacb systemUser to have sudo privilages
b39b698cadaa1b1ef981ffa32587768178f24006 Cleanup image status
8627f970a9f5b0642161161155a2b5ac4b712968 added empty implementaion of DownloadClusterKubeconfig after swagger changes
9cb117221c58e34193b65beec011e55c657e67a3 auto generated
e9f61db3b19dfb713176b2bc0e4d63f9fe2f6075 swagger: add network and pullsecret params
e782fa05ea52af190c9c29c7f63d66bb5fc8fa6f swagger: add kubeconfig download
6bfe20b13424426eb31897dcb1088eac69f0d1dd add logs to subsystem
6569282bab9bbe2315f24e0a3e71bffc5ce51496 fix host href
3505662cc7b18186318615fcf338ae65c48798fe auto generated
efac0675ace3feb7ee0f5ace3e9b6011f4a7b4cc swagger - add created_at to cluster model
b50092c867c71c1fbb43e5adf371e35865ef4de9 MGMT-619: Enable host to register several times. After expected or unexpected rebbot the host will be able to register again and go to discovering state
ecd67f63f1adb23bc019e8fd3dd2635a24cbc3cb add post step reply to subsystem
b62c1c8173330b2e9958bd52157c851b5e2aa2c4 auto generated
89d560bf202566dd271e7a8ea6b7b521e8bbf2d9 Add logging of agents requests and replies
ed9fc60773df292979ee75a2257b8ec320e03fb0 swagger: make properties camelCase
2603740bcf5683012f5c6b4be8a8da6e4a79353e fix download api
077d9b1050246e5f571923a777f83bf527d42226 Subsystem - test long ssh key
471015a259535e2db6a985c10dabecb3e81759c8 Fix broken subsystem
5349fbf9d16e67ad2c680eb3b52049a44be2785e auto generated
9e9aa2f4f8d8d3d4189dcd48b520734742f272ba Swagger - change ssh-key default size from 255 to 1024
f8eb6724f2ebaa66e2af1f97c0611743e39dec90 swagger: move host-related URLs after cluster-related
b06caa959c13361b944640965dba69fea59dd6a7 - First debug implementation - Implementation of execute (initial)
7f7bc8a990ddc29f10cc2614ad90913e73af4d64 swagger generate
3935eb039bdb70f33d997875f6f8e4f3cb42c303 1. Add support for execute step-type 2. Add command and arguments for execute 3. Add step-id Note that in the future, step-type will be removed, and the agent will only execute commands.
3f6589b78983e55ad304a11c570dcf9afd12a8c9 fix ignition cluster paramter to cluster-id
00e3a0b22ab4f9fb6dc2a7160cfeb821ae59a1c7 Add cluster id as a paramter to the ignition file.
021d55702e86dfba341572ef64e0de109dfcae0b MGMT-613: code and subsystem Move host api under cluster api. Changed host primary key to host + cluster, it enable the user to register host to a different cluster if he changed his mind host list get cluster id as paramter
baa06093d5ec7c09d36fcecae66edb8c0e83d99a MGMT-613: auto generated
e23e271d2bf35eb15cab94e8f75834c7cf3cacdc MGMT-613: Swagger - move hosts under cluster api
fd0a348a916b5d2f678eca140313232a051b2abf MGMT-589  Add SSH key to the ignition config in the liveCD
3a75a08d8968c779aecf427c029d27a20bda6f7b go mod
5d9b75fd679ca7ee4be1667dbea75ef08825c944 After swagger changes implement download image by the uploading to s3 and getting the object for the user implemenet cluster update + tests
3275f26b9ad93271eed002c5f1dd0bdd39eb414e auto generated
77e4f192a28f071044045e0b658132744d59697b swagger - remove namespace and add cluster_id to register host add x-go-custom-tag to all date-time propeties Swagger add 404 to new cluster operations Swagger change application/vnd.efi.iso to application/octet-stream, vnd.efi.iso is not supported
8f41238f37b5818087112ff2a42e899b05c613e3 replace postgres with mariadb
323c8ec1ed30e37aaca766a2bc115a71fc520431 swagger - fix cluster id duplication
806bb8b7429412e551dd5267603ad274a5cd0e25 swagger: remove image resource, change cluster flow
6109d10c7c57ebbd094c33ec73db45183059b35a MGMT-543 Nodes discovery framework
02d41f2cc057e420427f2374acd34a02edb71e22 partial implementaion of cluster create api
6f90e07ac76dee5c840fc405680e466224ab0674 auto generated
3a287dd8039a9cca18dac0b7d5b15e7e7ab162bb swagger - change cluster schema, it will contain full information on the nodes. it is doesn because gorm limitations, can't join two tables with only part of the fields
27f3260e4456d5e2439cf8ac2148479b259e6dbb add focus option to subsystem-run it is posible to run test by regex to run just use
e3818ad15ceeea74cbd52f731810431eca629503 Increasing waiting time for scality service
93cda513b6b356ba738162662715aeacfc1e8007 clear garbage create-image pods in clear-deployment
95d66aafee28d8095687080de2b09bf6d6536b42 makefile fixes
f1ff5966528ec4c0772a08dcb93a9da6a8f05c16 fix makefile export issue
423e0ed46749e8f452cb1758013483641d98699d subsystem fixes after renaming node to host
afd926c0d2243bd0f19f18e31a9629df0ae936f2 file rename subsystem/node_test.go -> subsystem/host_test.go
5109af34b1327be45cb63647be922be042f8a212 code changes after renaming node to host
7db0d466bed112da02e0a28e88a4160e41feecd2 auto generated
3807fc9307746270f37f247dbcbe075a9990e9ef swagger - rename node to host
de98c5149df88cf22fb8d53ae2c34c9c7757e1b8 Update readme with SERVICE environment variable support
aa64190dbfb48b1864af9b62258accbb560aa332 Increasing waiting time for scality service
9177d03c6143218c480e262afe5e7d60384a3b34 change bucket creation error message
a941f4d30b1983e291676a3cf5d1b036fea0fac1 Take SERVICE form environment variables, it support changing the image tag  with environment variable
6be6d92d46d8bb496be7bff7873cf2591c232fac Moving aws credentials to local folder
4cc4528f8aef52622411bac19b0d4fd0dd3b9ce7 change sync map to regular map and work with mutex. there may be a bug if sync map is used. get debug command and delete other command that was set if there is no lock on the map.
38f0111829f29b72bd3c69e76585fdcc11374ecb docs: Add state machines
d3be600e1cfa8c5057eaff3fd5b5a0cb045f83c6 Debug commands set for specific node added subsystem tests for debug commands
404c7543573dd6c32bdefe96d150d39eb685f1f7 change deploy-all to a full deployment for a sysmte enventoment, it will deploy s3, db, service and will work as a full operational system. deploy-for-test will replase deploy-all and will deploy everything for the subsystem evnironment
460195885e45ac2b0cf4ff99cf450a9a84a0f7dc Add aws cli to build container, it is used to create bucket in a full deployment
40baf80da918f764046b76abed5da8e14169d9ec support s3 deployment. deploy-all will only deploy dummy s3-config without actual s3 (it's out of scope for subsystem) but if needed there is a deploy/s3/scality-deployment.yaml that can be deployed and then need to exectue deploy/s3/deploy-configmap.yaml and it will init the right s3 url.
7df6d9317cdb17b83544d790a78b573948509054 update readme
c5b16c14a960e80bfad2e6273a8876829ecf62cd auto generated
b422fc42c9942af62dbb63fb58cfe1995f29d036 Swagger: move enabled property to a state
9e21664c07a4c1d5690aaa7c57a91457ea506431 update implementaion for new node  apis update subsystem tests
712b853cd44664d9d9d2158540fc889ae81038f3 auto generated
fbab6ea649ee8839ab397148ebfc7ebe8955f961 revert node deletion, we still need this api to start fresh in case of bugs
e034e3b4a391443c84995e2a7d3eaee5e326ab86 Update swagger
caacd05ce18a8315af79983401c84477261c8636 each next step request will return hw info step by default
1b9e9130d840f6615d4ed0c8e1e550e486fd2bdd makefile cleanup
4714afa05f54355ec3e17da4197614d959c448c0 makefile added subsystem cleanup after running subsystem, there is a bug in k8s that sometimes when job is deleted the pod still exists
5e2e4e4ef0302e7332b69baa865cb197ce5c7efb modify inventory implementation after swagger changes
e1f1c56571f9eeb60fdda5bd6985a1803612548f auto generated
8403f9b1ca58c30a044184d6ae0ae91601cca645 Pull request review changes
45842331b5a9f230ef5056365c2de6f2cd2a83b8 Add health-check and connectivity-check replies
a99a17ce063b2f72fd80de9a8e27c1f092cbd076 Multiple changes for connectivity check - Separate connectivity check request to named objects in swagger - Change StepsReply to StepReply - Make the StepReply send reply data - Change node-id to uuid in all places
7513115287e3480081836c097e2a5a81e1d1daf5 start working with skipper
2105410ecc9d409ec6e53223844e8512fd848251 add libvirt client and mounts to support minikube commands
d092aa450f8144737f1527333f73b268c66aa293 add kubectl
825ea5a3989a6d27a313680f394c458c101df31e add docker login paramters to build container
bff12183a852b99631d72afbed8ac92a6c16c6b6 Added minikube to build container
4192037e08d7e6727d9c85df7efecd62b0e7b6fc update README
777c55d6f16d8b6fd66d3184c54c48dd6b87bc53 change generate-swagger target to generate from swagger
b20b051505d598398a4bf9fab2987b37b025890a set default registered node status as discovering
bc1d245b95a0d3c92034c3b9662dc739ac26e704 auto generated
f0d1850926ac6aff15aa2bca687adb3b3515a46a update swaggwer with node states discovering, known, disconnected, installing, insufficient, installed
0fe51f26e31b531e5bcd351e2bc2dbfd46f954b9 go mod
f4fda0ef94601246436c5fb56eede3669fbbbc87 use environment variables to run subsystem, it will automaticali connect to local minikube and get the ip addresses
1443a133e1841b451224ae02a0121e50c319d081 fix debug commnad should be a single shot
ca0cc2b68722c3c14a658407e9ebdcdfeaff6ff8 fix debug commnad should be a single shot
9a514b5f14fc9b8d6539f118ab9920604a76574d implementation of debug command
71ef0095363b7a88562e7de178ea43b740865488 auto generated
75b90ff387d3e943c25577c4e9e0aa30d00521a3 swagger added debug command to set a single shot command to the next node that will request the next step
da4a3ce8d511d2d94a09390fe87dba285a17afc4 Default to building the build container in case it doesn't exists - Don't specify build-container-tag in the skipper.yaml Also no ned to specify container-context
f0caf4f6a4c7134fce39474045180ceb1c6d35ec Added apt-get cache cleanup
825cf507d74d5453b06fcc00a856408e496256cc ignition will have a default user 'core' with the password 'qwerty'
9e4c97df1b30197288a7ab0a1f65abf551ddd0f7 Minor ignition fixes
37889ce9c5661b5da71e99a5921ead9cadb5f03e Dummy implementation for next-step api
cc8c5e082ab4475fcad5016246a9ab0ee54981c9 auto generated swagger files
f619001a1700e7531e20943f4a2cb850783efb0f set enviroment variables for the image builder
83a8ba894ffab380b47fe78dded76eebb6353677 Swagger changes - change opcode to string and add network connectivity check parameters
4352801f898badfa66d1e769decba0ee2df4a8a4 swagger - next step operations from the agent
cece03ecde25bcc184a250e5b0bde11f1e877227 code fixes
ede8eb131dab7138d404da451737e612b2398547 use postgres dns name instead of ip
297800758a4209755ab38a9acc530ec16a945935 add serial parameter to node creation
e5d9c972262b29266b0f935451475d99b884e0db basic subsystem with connection to existing k8s cluster
180ab337edffbe5062c5c12f26f3ea10ae0f92ff mod
b7654f21e4c8695615426f688a59910467b76428 deploy roles to support images creation
814d64a424b35ff89c6265cbab415ed6be94ebf5 image create will run a job and main get configuration with environment variables
169b207a49a3ff08fce2dba6af0c1a674c774dca implement basuc crud
f32af6c4832d23be2132fcb7dbad49624117af48 swagger changes - added 500 reply to some apis
df700b557989ca8add5c8c5c1561e288dc508c9c postgress deployment for testing
1d6717c993aefa377626bfd977375e96b6d8d692 go mod
5b52cfd5a911ca25594a99fc83402041b29613fe image api implementaion
c73340d72956ff34b598c480afa7d441f5579a01 Makefile tmp for testing
fdf83bf1b587107936a3fde3bef1003067284ece swagger + auto generated
9eb12e68c73687b36d93c6edb76d71ab28a4999d add support for minimal docker image
a78c8c1505dde0323d6c0f0f26d0ccc7281fa870 gitignore kubvirtci
d508bbd754fcb05d77377ea4517c8ffea33d83af fix go mod cache
eac473ab7ded1d226fd3f730a63fb5ad0cab87d7 add listen port as flag to the service
5945af7e2ca5148c18bf49c8e04b66d6a72d07c8 dummy implementaion
530dbbdff103be3cbae4a4d826deda2a7452b479 add auto generated files
5834a6cb36b1a04dd1129c971bce37d7cb1212b8 add swagger file
add7b15295f2d4a40e63ad91c19fe44be713dbc0 Add swagger generation option
e896c103e87df209b545d6be820b98e179a9f9a0 Add skipper support
a0710eb914c1214b712e9440ef1fcaf6378c5c40 initial make
6f371d4d6c2c0473fd99e942bea6417496852571 Initial commit
```

Status: Syncing successful

### Branch release-ocm-2.5 -> backplane-2.0:

