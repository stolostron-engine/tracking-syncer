## Syncing stolostron/multicloud-operators-foundation with stolostron-engine/multicloud-operators-foundation

## Status Summary:

backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Synced commits but not tags.  

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits (first branch sync):

```
d81a766719fb42a74e44b5e13e536e6c918d85a8 run the health server before newManager (#489)
3519739cf85bac1afe091f8ae8251ff9fa7ca484 only cache logCertSecret namespace secret (#484)
8392b1f2f54c6836eae3305dc6c064b29e0e1947 Create oauth redirectURIs claim for openshift cluster (#472)
8306366507cb257171d80ea4bbae81fa865e81e0 Add env for registration operator branch (#478)
4d3bfb250a690599044d85eb6a347cf1406cd14b add test for cluster from clusterpool (#477)
bd577d0a14a0b3e7d1ddf528babb6d6160535146 allow claimed cluster move to default set (#471)
2151fcd1bed7daade190ce1fc9c4951e7d2fe26a Ignore vscode to trigger ci (#470)
f170329f057f2ccef2c29b35e23f3f846c8bd3dd upgrade addon-framework (#469)
ffc5b5e7d9bf3bcc23b5035506939bed10c4b117 fix no route in ocp 311 and errors in log (#468)
d03b83c6a5a9e5b621c4491fac80e13cca5727fc revert addon-imageregistry defaultclient to be compatible with old user (#467)
b4c020adb5f1fd08b58636aa1285b9ce7a36a121 fix empty imageregistries annotion (#465)
3d77d5cb35fd04faf4e5a627cc9eec75cb89cb66 enhance imageRegistry API to support multi-registries (#464)
633623536f299d8e0eafca02c7e11c90db18ab5a Add backup label (#463)
9dd125f16c272bb1cbe22b56785a6b870b34aff5 fix the addon is deployed on OCP311 (#462)
e3f678617264235ee216d07fd172c99d298b8f80 upgrade go libs (#460)
4d4b63e6388136ce9c4c1cf875a601aafb354960 fix addon image and nodeSelector override (#459)
2ea99b88c0fdc4188b1002bbc6b5c982495eb3d3 fix addon service type (#458)
8c48c4e7dbb83ed81785d83292c267a935877cfb support to detect RHV for OCP (#457)
128591ce9dbe0c8c6f5e777fadae8f4333c59a19 fix rbac about generate rolebinding for clusterset (#455)
a34aeee9fcb24dd286081df06fe35aba97a96725 upgrade hive (#453)
3733b519c3d7c93205c3d8acf1f24b2a70adb613 use new set api (#447)
0001f46a5115fe43c606a068e5e7ee00abec3b68 fix product cannot be updated in ocp upgrade failure case (#446)
970fb58ad8790f906053358a7bfc3d9caee042e7 ignore ai create clusterdeployment (#445)
4445a66a872a56a2bb629b59d764c4b45c3d0fe7 fix SNO no ocp console (#444)
09044c147e63408e697d96fc0324678b8b2c4cad refactor work-manager addon (#443)
b01ead83c195e3d43a8b34f2a1f0510c4698694d upgrade libs (#442)
633e594a70b8ba9adb3db8b9c22d304210743570 add exclude backup label for clusterclaims (#441)
cc30cffdf5706cbe8e47b4b17ee9b22fa98cdf7c fix CVE-2021-43565 (#435)
172fb944faa95d7968eda7e38067e7ea866e88b2 Rename GitHub org (#430)
1fcc350dd5f14b5ff0b1ce4b9866c15b9e72b808 add test for config checker (#429)
dc05ae5408a5e73e8e44d3be60d43b38f0cd250b update the guide on how to deploy and clean up (#424)
e58a38287948b283ada26a0c406d142d0285d446 fix the issue failed to get infra in ocp311 (#427)
b6aadd0ed647c06fce1cf6ee4a2d9fe0ee95ed6f remove the sleep wait in config checker e2e test (#412)
56270b1520ec5896981db689b3afe0cd893cad8e upgrade go to 1.17 (#422)
74667b711106d354f45f5de28408b3604dd77ce6 handle request error in webhook (#414)
abf7edda49a037ae41e65ae0d0025b87abad1bb4 fix the issue that failed to check the openshift when the mappering meets error (#415)
92233355d0ed2b62d7408d5a5205dd621c0e2961 fix the vendor is others for ROSA clusters (#411)
1db488072a852269a1499f48c1132a846c868797 add config checker in work manager (#407)
b7edddc313c9d346ec761b01b17ebd6f73eb1098 fix the incorrect image of foundation agent in e2e (#410)
b3497e4a37207b2bca4151d847a4c819507a003d detect product ARO (#409)
869c13ac1e4e59ae7aa25510697f06a454269b79 detect product ROSA (#408)
06ee625afd249de1310ef549a1f68a9f1e583fdc append proxy service CA (#406)
a4a6934a679049834e44eec88dd522e1e77220b6 upgrade hive api (#405)
45105bb390d6c1f654a7755e6920f0824d48966c Merge pull request #399 from ldpliu/sync-set-label
d5e1675f094317fd2b4bc32e9bddc4dbfbdf5213 sync clusterdeployment label by cluster
b296cd01e3f79f8685c023eca49cca414a36e42c Merge pull request #404 from elgnay/upgrade-clusterset
8cf24ce4b7b06df68baf40ad57740d54faa9812f upgrade clusterset
063d60d0b2eb0b7fc65fb073ccfe4d208d6ac17a Merge pull request #403 from qiujian16/auto-deploy-agent
ace03c94c1e6a79ea07c8a3a8fb34fb0760d5174 Audo deploy foundation agent
5373a6b17085a3d5868bf8add5a6ac6f908231ae Merge pull request #402 from ldpliu/upgrade-hive
c0eb5a4923cd4472ae9c0815ecf6039b0531602e upgrade hive to 1.1.16
dc43ec703e62594e3942c7f06d38d1897550ffea Merge pull request #401 from xuezhaojun/fix-voluerable-lib
86fd34c0ed57995a366028302368309aa500499a fix voluerable lib dependencies
c40c50b561d247d643d09d8a7e61881e5abf4f71 Merge pull request #398 from qiujian16/deploy-agent
ee505246f3f83135aec8eeea04ae0ef887f73ec4 Merge pull request #400 from zhiweiyin318/imageregistry
0813d4873405bc0d3a4764e1174931f4fa5315e7 add imageRegistry method
113ebd1b1e4aa931d87d60b6e67bd425d72a3161 Deploy addon agent
773be55fc097e1d5e29d64d37f3a8d2bfecf588b Merge pull request #397 from qiujian16/update-deps
6fda91a51d044f3a1322d36b82d1f13a1adfc195 Update lib to open-cluster-management.io
51557a572f1108fd13d1c8959a1e4500188aa45d Merge pull request #390 from zhiweiyin318/add-registry-crd
80f172188e983305529c2db5c863390dac8ce78a add image registry
8ca433dce8200b93dfecb0014a84d3d8c2961867 Merge pull request #391 from ldpliu/upgrade-hive
6c46a3253f0ddba0a021ca5ff76221a95f15d669 upgrade hive to 1.1.12
d7bf1af18c9459f119767ae8026c35fbc80121f9 Merge pull request #393 from zhiweiyin318/fix-provideid
566a033dadcc82dfbf94c93648d450608fe302e8 fix wrong platform
dda6b80090951ca7abcc9bc8aca86d13c9202b26 Merge pull request #388 from ldpliu/e2e-ca
e062da12fb347138f401fb94d27ed7e365f838c8 add e2e for managedcluster ca
7ba86824a77a70ba4e900a10be51b3d272ad4ac5 Merge pull request #389 from ldpliu/test-e2e
1089e25a6f0d90ca3499843371516d3d092327b0 [Do not merge]
af8653e19d731ff23c70e4ce05e0a65d91bc67db Merge pull request #387 from ldpliu/clusterca_info
864e16bf29fd7bd3cfcbf599cc65d283ed71964b add ca to managedcluster spec
e0f92ba7c4d07b6a44c366baee2e1fb364d4f3e2 Merge pull request #385 from zhiweiyin318/replace-baseimage
e76fb8f5c6edc512c0ac183aa74e5d88df5fe113 replace base image of docker.io
deae12e40bda3c38e7fb460d14999e19e57b15b4 Merge pull request #383 from zhiweiyin318/mem-leak
c595b13055c5b3411fd7d376ca1ff80849228c25 fix cert pool mem leak
e6f9cc0b529585a398675ecb0a9dc82f5917f78b Merge pull request #381 from zhiweiyin318/offlinenodes
54e56170f5ca582f08360f31735cfc2cf1c78cc9 empty cluster status when cluster is offline
2b456f6c88c5f44b1e722c5756e5ba94b9145632 Merge pull request #379 from zhiweiyin318/optimize-e2e
b5df50deb87618e8c6057637705e94a58b5a19da refactor e2e
eb657d8a82808eae57f26278406f3d205ab90357 Merge pull request #377 from ldpliu/clean-finalizer
30a1af9ef9fc37682f30c518728ccf0929f8ef11 handle upgrade from 2.2.X to 2.3 to remove finalizer in clusterrole
81c0f51fd1d310bc650c95287d834c257dd8f1e3 Merge pull request #378 from zhiweiyin318/makefile-prow
be540923611fe88bfaccb30a011bf65126c9f7a5 add makefile prow
9f6bb852a353f700268324f167bf19731066efa9 Merge pull request #374 from philipwu08/skip-ownerid-appsub2
a910a90dd35d093c5c2fbf570cb9511cf387f592 Skip updating user and group ID for appsubs
e2b133b3891879da6a86b4f74b27bdf5286ccd8e Merge pull request #376 from zhiweiyin318/cert-controller
6e5aa8f74a655b8fbeace53809e39fde05bfc22a add log cert controller
4db33f778b409bb2a069259c1a848d44f85565b4 Merge pull request #375 from ldpliu/bma-reason
ae99a70a989286dbbc8b73112a64d08f98c37149 create const to contain BMA status reason
54a287418178c6e28ae6dc76b05a574039312130 Merge pull request #373 from elgnay/update-addon-framework
1f073a0089a951f0ba5fd9aaa2589cc73b7578f1 lease compatible
50e98437fcaee8d90814c946f1d5e85ce230661f Merge pull request #369 from zhiweiyin318/fix-clusterclaim
fa523248943a02b5390bdc89bab5436e49ddbfa6 fix delete customized clusterClaim
2ab9cad59f0fe2e9b59ded9ad2331b7392dc5b84 Merge pull request #367 from zhiweiyin318/fix-webhook
77cb0070fcc459fc303df60e189a8ded65d634d8 fix webhook cert rotation
2d91a71e365c8b0c2d435ad9b0a593bf0730be26 Merge pull request #361 from ldpliu/fix-qps
681e510aa6258a548e106cd4b6d98b39edd56b3b add qps and burst for agent
0c5034a24e4b2259f758aaee464117818362a2a3 Merge pull request #366 from zhiweiyin318/update-clusterinfo
06c3eb1b0bf6995bf672c379141d4417e836185f reduce clusterinfo update
73833b381b9925910efb2bde9708df1843e6e0e9 Merge pull request #364 from ldpliu/claimedcluster-delete
b7d9d828c8491a31c4b7d0c67ea77bfe2259210d fix claimed cluster can not delete from clusterset
aa4711bbfbc7d65c9bdb3f659aad5faba5d8eda1 Merge pull request #365 from ldpliu/set-rbac
87304f000db94f197009845c138156012285a3e4 fix clusterset rbac
558b4154dff0ef15e0829a9804a650c629612b63 Merge pull request #360 from ldpliu/enhance-clusterset-e2e
63c26eb7653908710893619b6793db443a47af62 add more case for clusterset rbac e2e
22356b9e09b2dba81e70c098bdb1885a29e3a96b Merge pull request #363 from zhiweiyin318/e2e-inventory
850131f638c5127c0dda68429f110c1b351bb3f8 fix inventory e2e case failure
34d33c2dac2e0a3c458c06c29a0ca34f3ddb7216 Merge pull request #359 from zhiweiyin318/upgrade-pkg
8720637cf902b7dbb91a7c230514fd548099610d upgrade ulikunitz/xz to v0.5.8
9a48d3528e1887f6ee2f5e88865be3054884d71e Merge pull request #358 from hchenxa/hchenxa
a1859b947ee1eca47cfdc090af65473270621754 add check before accept the managed cluster
7083f717bdff139b72603d15a5f05e56b9e97bbc enable the junit report
432e03ea07b1ee59ad548f78a584b2bb9ed96b7f Merge pull request #357 from zhiweiyin318/sync-labels-claims
557500acad64a1ccb2a7250d68b7c4c6d579feeb sync labels to claims
b94b9054ce27cc46aa0f01fe4edeb75e3a596cfc Merge pull request #355 from zhiweiyin318/sno-claim
5d70a82b96f49ea78d534158c7ff7a9b4566aefc add clusterClaim ControlPlaneTopology
6a0b857036c6d27c048bc95cd9b371ab89676ec2 Merge pull request #356 from ldpliu/add-ocp-label
99fb063773d29c42da8db025204dfa04b916afd9 add ocp version to managedcluster label
9a2433a70bb6d582c97c0de8ab22742acbce57a2 Merge pull request #353 from ldpliu/webhook-performance
51d90d2f60951de0037ceb57a6ad322e65f94fc5 Merge pull request #354 from zhiweiyin318/desiredchannel
11718dcaf9abebd1bad9d76e8f5f29119e0d9e66 update webhook qps and burst
d20db13e980370e6fcbbbaa1b7312d941fb749a7 add desired of ocp into clusterinfo.status
a71bc9c5898985acae1c795b153a1db1e3f85755 Merge pull request #352 from zhiweiyin318/printer
6e03050abf3eae1a985b51ca1ca3d35b1210e2c5 add printer for managedcluster.clusterview
392278bc8fb80c2f45aeb27c2a6670a4552c1b92 Merge pull request #351 from zhiweiyin318/shortname
550001aa7c1377fef04a013578a0337024e0d98d add short name mcv for managedCluster.clusterview
16f69b95ab03e1f770b79b854edc0337bbebc079 Merge pull request #349 from ldpliu/upgrade-hive
90770540733a58fa9f0e28a77b69172eb8b488d9 Merge pull request #350 from zhiweiyin318/dockerfile
8283b4e6d74b8c4c4fbc1ff1a05794e7ce1bd774 upgrade dockerfile with golang-1.16
a45cd66000f2bdb933321ac878ec8cea8db02234 upgrade hvie to 1.1.3
a9a7ad66550c78d13bb990b49b77055931108a16 Merge pull request #347 from zhiweiyin318/refactor-dynamicclient
5055f4719bedff2f5a9b62269de922365b6d8b56 refactor getting clusterversion with api
f8deb294e1e142ba2ca63695d27f5ab3c138eeb3 Merge pull request #346 from zhiweiyin318/add-channel
d00a575ac84336c4fe4ad42710e780754860df26 add channel to OCPdistributionInfo
d9812cd45609c3a3d2d79bd675d1242680fa7a13 Merge pull request #344 from zhiweiyin318/fix-view
975effd689b729b94b33f470cb165d4a2419a604 update the installation
0e326b84f113fe90ea17dd8fdf8bf772abc4112a Merge pull request #343 from qiujian16/fix-info-bug
a5d6beb76815405aa5a0adabe3b46d626f3cbe0d Fix nodelist bug
361481436bf9483da3c33a193db1c097d384fc8d Merge pull request #342 from qiujian16/remove-cpu-worker
508669c900e68a2004d054b6dc300212b1fb99e6 Remove cpu_worker/socket etc
fc8b57a7d4611f1ed4dc0721f42ba0e62a44d3d5 Merge pull request #341 from qiujian16/refactor-collector
a44c525aade22f7761caa855c6e3bdc0af513022 Refactor resource collector
1e738fdabb65a78ce4e311ea80b89429bcf044b4 Merge pull request #337 from qiujian16/update-rest-mapper
a9341d53bcf8479936490c94a7bcd94634b81328 Change rest mapper
289660415248694c4d7009673d8af9fd9ef77bc2 Add cpu_worker into capacity
085083b74a50e970b84a8a426d6ab1a7ce0e750d Merge pull request #336 from qiujian16/add_cpu_worker
685b92d88a1db242229ec0193f7804f2df00390c Add cpu_worker into capacity
b852c6001862038284f080113fb0c7479726f0c1 Merge pull request #339 from ldpliu/hive
0ca9ba78a7c6d72256bc4e51dc166e82333dcb01 upgrade hive
1a7abd6aa4f851ce450e66fea45498fc6630d6b4 Merge pull request #338 from ldpliu/enable-clusterset
5199e3066b5c2e6d6bf7ac3ece471af14c843210 disable managedclusterset validating
2539d82c14cdd0900f81a61321da78f29b4b0546 Merge pull request #335 from ldpliu/fix-muti-replica
db313afd69dddf71648b5a6a0e0980be1cc609b4 fix bug when replica is bigger than one
0ca21fbe6a3e9055fc5c1b7b945999b2eb98bc76 Merge pull request #334 from qiujian16/add-socket
6f9d2ff7e20042c8c167427ebd8725898e9e3bc9 Query prom to get socket/core
62b671f10aba0dfb2ccf26866256a6e4009ec7c5 Merge pull request #329 from ldpliu/sync-rolebinding
23a5acdfa157a6e33629ea18dd48839358fae169 clusterset rbac
8c407116c2e2e0150cc2a426912ecdd564126446 Merge pull request #330 from zhiweiyin318/clusterverion
aa7c7f92cc1b3500dfef4795c49703ff50987095 Merge pull request #331 from zhiweiyin318/owners
f21b9bde3e6d8c3f942b87883c5cd74ae0a5a3ce format owners file
591dc2d7103b14b57401eddb5c8e943bcdf9fe30 update OCPDistributionInfo
3d48742b06b83f33d1d18cb571535f464ad61242 Merge pull request #328 from SherinV/debugSearchProxyIssue
c5c0f55c034c4606cb47116750955db9e9395525 update doc, tests
f162cae53b91a0c343a062f37dc84ca93e2c2b36 update error message
631364c068a67b45a0b495aec4a6f9d9e42f320a get ca.crt from caConfigMap
1608b12f395f6d28981d7179a9ffb0a7b563dbd8 Merge pull request #327 from ldpliu/abstract-cache
a3f2166438618c72461e4621a56cb4850a5b4705 acstract cache
4ff82124f94597e043e2a0c5bc8184284b1211d2 comment out secret.Data["ca.crt"]
434684dc0274fd773e5b5b268b9f189feaf2229b Merge pull request #320 from ldpliu/clusterrole
40d756bc0af9ab804c37c1f5b66c16e40838ad73 update clusterrole func
8b0c93aa802cb46c308242e04172d8b7de7986cb Merge pull request #325 from zhiweiyin318/add-sonar
21cf42e315aaa3a485e0667833afa840358e17d3 Merge pull request #324 from zhiweiyin318/fix-clusterpool
612904a828b8875bf8392857c6660b14415faa57 add sonar properties
55e3a3a2b3b3455d9ed28f9af5aa5ea2a8ee61ac fix allow to create clusterdeployment with clusterpool ref
c4d7b3462d1873590388082cc317daf12455d192 Merge pull request #326 from zhiweiyin318/fix-lease-e2e
3bb318aa4fe731b978323962b0615f0b9727f1c2 update addon api
d6fcf203540bb25a70ed68dc0ce52335b7ed940f Merge pull request #323 from zhiweiyin318/refactor-claim
77a2a6153bd6c2dbbe0c738fb2bf0640a69dc997 refactor clusterInfo and clusterClaim
e94b719de6d5f3541e948dd70ad8f1ff748aa452 Merge pull request #322 from qiujian16/change-lease
215bd590a465b2fa641b414de875aa4257be8bfd Update lease implementation
2b45970d2f925e78e2d371d968dfceff8b6a3582 Merge pull request #316 from ldpliu/clusterser-role
f2716625e6e89820bf6e981d1cc96c4c4c6f3c8f add clusterset admin/view clusterrole
914568981eeedfcfcd8544ae6b69a3854d36e07c Merge pull request #318 from zhiweiyin318/validating-webhook
f5f0619c925c2ccf7927d01a05dd807ceb0a61ee add validating webhook
0cab703dd631fadccb17eb0069b0a23a77031a75 Merge pull request #317 from zhiweiyin318/webhook
1603ade6dafdfb46735c93db6143a04e958c7677 fix webhook issues
9cad4f278060ed76a75dcd7907a9f6f2b2353e79 Merge pull request #314 from zhiweiyin318/upgrade-v1
d4024ec016b0a0b246b9997bf456f4517bd249fd upgrade crd to v1
618396ddabcff3349865c7730a4fcea0c4a12915 Merge pull request #313 from zhiweiyin318/fix-verbissue
92624a5ad4caa9a781c448f6deb5b7c6c5c81032 Merge pull request #312 from zhiweiyin318/detect-zp
5bf541785fc11cb7a86be6de3c4cba8711cb7918 fix issue that cannot get clusterview using verb *
d80191fe63c40c043eee631d0dd3beac30455df2 detect IBM power and z arch
1fdfd89d111a4d06b13521a0b20c8720421b1d55 Merge pull request #310 from ldpliu/upgrade-hive
4c4b0d524c937d36fb99000fd5b59c4465314ffe upgrade hive
e6b185641c716c6247868d0411d870ea0d031d3f Merge pull request #311 from zhiweiyin318/add-rbac
e3c3619f25bc25fac299e74344d30b3987f49c94 add clusterview rules to cluster admin and view roles
1c4d77f6936a77f603f2b3a3d2975536c3f5a611 Merge pull request #308 from zhiweiyin318/fix-9463
af3513eca243ab1f6b98227ee17b9db32e2696a9 fix issue that only updates status timestamps
6259cf80126fd7ab4d63506d1ba99b0598ea592d Merge pull request #307 from zhiweiyin318/fix-e2e
82d2d91c310aeb563d02c83e17e0fec59347ad6d fix e2e bugs
f1bd3e4d3cfdf79909aaf5e63086f70daffae6a1 Merge pull request #306 from zhiweiyin318/add-doc
0628afbae4349cd76783ebb32e6335e8fe1b1b3e add doc for clusterview apis
a5bbafa474f6238cc8663992f06dc441edcd1a65 Merge pull request #304 from zhiweiyin318/clustersetview
ce6f799f9c50c5a2d1805abc39113115b3af24e2 add clusterview api to list managedclusterset
e9119744df158cba4f9449effb8f33738a2404ee Merge pull request #303 from zhiweiyin318/clusterview
cf92ad481ef186e21d74e3f1b2caffe8f772abcf add clusterview api to list managedcluster
62694f0cebcce638ca2ca2cc97d07c92106df56a Merge pull request #300 from qiujian16/fix-bma-ref
b08ab62ce26f3945a59ea118d9e1a83dd0028cd4 Fix bma ref
e6f18f686a55fcec9bada9ba047a5dbbf89fd21e Merge pull request #299 from qiujian16/upgrade-hive
e1b8f62bd641a5e9741001942383ec5d7cc7fbd1 Upgrade hive
dade98ef6f2d4ed6493eccf56e40769dd585fcad Merge pull request #297 from qiujian16/update-readme
f827c61a5720722389bfeb8de74b0b56ea3f2b9d Rename acm to ocm
55c8431ca7027b1a0236be9677221de09cfa1bcb Merge pull request #295 from qiujian16/fix-osd-labels
3914334c646d553c6c81ed9cbf03ce57bd457507 Fix osd labels
d4c03de4495e4276af7366f5f34d50bab69c33d5 Merge pull request #294 from zhiweiyin318/promote-go
cae08ebefc4e92f9b1a370bc563725fad1b75979 promote go to 1.15
38cf8723914e531a98c3a45964642949d7baff7c Merge pull request #292 from zhiweiyin318/retrigger
c31bb444672ffe0a87dde1795465411f4fcc0df6 retrigger the prow
3cc8ded84cf2fb867b41d1e002acd69ee2081510 Merge pull request #291 from zhiweiyin318/rebuild-again
b5d1661660aaed4fbf8e9990a03a5ba49cb424c5 retrigger prow to publish
fe8778cc0c53d3fa6293efecedc1851307d36f45 Merge pull request #290 from zhiweiyin318/rebuild-again
631dd0d99dc1e870b277c448a64a7529c8512d0c retrigger prow to publish
4da8bee8b9c70f0bc1e0f2e671686fb090d437d1 Merge pull request #289 from zhiweiyin318/rebuild
7f9b28059d3327ad7df6d5d8d174704c24f62883 fix typo
124c7c74cae2c75e0bae5dc13ff49de1d559378d Merge pull request #286 from zhiweiyin318/osdcluster
4b57f6986b2a9e7e5e09bdd380ee3ea4b21a8bae detect OSD cluster
f499efebc513ddd739c9a6904b0e4d5db516554b Merge pull request #285 from qiujian16/claim-vendor
415d46e0b9196bc5c7812e8838964195dac1514a Merge pull request #284 from qiujian16/rm-secret-watch
6a83177cb9e79ee6ffc463994a2e209d664883c1 Add openstack/vsphere to claim
f01a09c7e078fc8392f26e7b6a8fe583acad2936 Remove secret watch in inventory
5b8e91d607bf11c38c7ea4aad308a8aeb855caf2 Merge pull request #283 from qiujian16/inventory-fix
ab118314630242a25f054018dcbfe36f7949344b Fix inventory
f063a354ea2a3f93222ae7ec5b1af3185900ddd7 Merge pull request #281 from qiujian16/fix-proto
0cdd1ed7cfc4dba96996cd0613da4ef32b9637cc Upgrade gogo protobuf
455f6e1ca25fba2d132b11f059c7b8896a547190 Merge pull request #280 from zhiweiyin318/detect-openstack
41bf440602e2a16261ca0b99eb2059c627c7e740 add openstack cloud vendor detection
f9452615edda03e30b158381ba0d4f16ea2729f6 Merge pull request #279 from zhiweiyin318/detect-vmware
e3fca1335b236f82da2fbb0f7da4bf7a38ed4986 add vsphere cloud vendor detection
73a2649c6b2acedf2490280e3dc25172d7e56654 Merge pull request #277 from ldpliu/upgrade-go-slug
e0f42b36eb52f2bdf4ab4883f49be3b8a5e7fce9 upgrade go-slug
f61b5d2b963eedb38e18d9a6dcf8fdfaa3f9267c Merge pull request #276 from zhiweiyin318/update-upgradefail
078ff051b72ccb1772f28da778f00d599a075875 update the UpgradeFail defination
915c7aa6d37365e1e3f45488927440308c83816b Merge pull request #274 from zhiweiyin318/fix-ocp3.x
798d2ca1c7c0b6b0d1d651e72a5e37b9df2ad931 Merge pull request #272 from sdminonne/contributing
5d9e25d42b11f5a76a3a5084e949509bef24f84d show OpenShift 3
1574337b1b1830e87fef057d9aa8279a67656628 Merge pull request #273 from zhiweiyin318/add-claims
b9591354c8f5463f4555f194bf5fe79b6e02cb12 add claims for submariner
25244438b5a0ffef0adbbf034d1ca7f1c12054f7 To improve dev experience: gopath bin in path
a1a58a65585d457e0b14c69731c7968db41822b7 Merge pull request #271 from zhiweiyin318/check-ocp3x
e2507050ddff3139989533613fc8c2589bea891e check ocp311 version
ecc11bb3281cf091794723a08982bf87cd9f23f6 Merge pull request #270 from zhiweiyin318/retrigger-prow
4f4f58cb39fbb20c35ed4720051d3033346aa5e4 trigger the prow to build images
0cea23d757de163e77d5201f0dfe11bdbc697317 Merge pull request #269 from zhiweiyin318/revert-PR266
722967e30632b14d7f1de6b4caf93693053a8d72 Revert "remove cluster conditions in clusterinfo"
2b45a8a2c1443d2bf68317e81c37af09c9101aef Merge pull request #268 from elgnay/clusterclaim
6ce99c8fd72a60f73ccff5bf738ac7170f706599 Add controller to create & reconcile cluster claims
5f63a132e0b9f393425d1f42865522bcb57423a2 Merge pull request #267 from ldpliu/add-lease
8a49b877f08ac50437dd61d89230f34672601d33 add e2e
d5e9c13c832cf172f9e24ccad6592c4f8ab630f9 add lease controller
60ef45157161b6d4ec2af817fb95d8e689a480e7 Merge pull request #266 from zhiweiyin318/remove-cluster-conditions
1acfdce60e571c1fa4532a568b05f25fe0c60279 Merge pull request #264 from zhiweiyin318/ocp311-version
57839edaaa506d5f4f0cb3b9b12cf7237dceb9b3 remove cluster conditions in clusterinfo
401d93a0981a8261ae4d68e98c6784fa0f85632f ignoreNotFound error when get version in OCP3.x
fb645a9bfdaeb3d1d14c66ec78bef88e28323e20 Merge pull request #263 from skeeey/contributing
586c4f8af62f8ff542414994241dac1e4815aa3f update contributing guide
779455d2110858bda73e3b931a2337af2350df54 Merge pull request #258 from zhiweiyin318/log-mem-leak
8a3735ac172d3203fe4304c9ad756a4971fd4edf Merge pull request #259 from qiujian16/fix-patch-cond
be652f46bc111f36ac5b6bde93c94434592b38cb Fix bma status when using patch in syncset
e6a771a59b74880fb9649eff67e963e865175b9c Use null logger to require less memory
b927183080d96ee89c699f4dcabf5f5d05fe01a6 Merge pull request #254 from qiujian16/inventory-e2e
ade32b2074da67b171cdb42530e02c0e9938d581 Merge pull request #257 from zhiweiyin318/fix-autodetect-labels
8c75e80f7a0ecaa0bcfd8930f453e54dee376b30 fix that update clusterinfo labels constantly
2bdad984170dda44191cc62d5170f7e9e4306ce3 Add inventory e2e test
714a41fd8f3e2032fbc3ce617b6968253138f7ab Merge pull request #256 from zhiweiyin318/update-registration-operator
bb3123933f77f6f693306c6e35a588b89167feb5 use olm to deploy registration-operator
937718d6390dd0b33d56402b88e0a0965dc6c09e Merge pull request #253 from elgnay/issue_5554
d3f22aa12a9c2804e1cbe687cb1baf58184612de Trigger rebuild
36578a3b7408ce452af7823200486d90f27ade9f Merge pull request #252 from zhiweiyin318/trigger-image
44e7d2d6f78e2432d30a11117f51a0fc55644401 fix typo
8e32473c7f03d397507b279ed362a85468e18e74 Merge pull request #250 from qiujian16/disallow-secret-view
41bc2d2d12c744533a59f3bd78ff383059e42b85 Do not allow secret to be viewed
9f2a8cfdbbc0026960d7f1a05504e40e97c0c63e Merge pull request #249 from qiujian16/owner-role
a487eac8734ee6ccc6121384805748f8eb377793 Allow setting ownerref to secret from bma
a9f4396aa9fad2449ede4870f7d037129e89e4ba Merge pull request #248 from zhiweiyin318/fix-gosec-scan-findings
4b5337e457eab0cf60e91600154b8fc221a9cb79 Merge pull request #247 from ldpliu/clusterset-cluster
c39eb89831cc6a47a1db99d5bff0d8269cd14bb0 fix e2e for clusterset
39e9ae0def48060a9ca9f493b9dac3270b11fb73 add watch clusterset
6aa1520b87330d560ef11167c56c8cfb9e1fb1c4 fix gosec scan findings
84a03696f498a17daca4863dd1fa4eb7a2295e73 update hive to hanlde verify-deps error
2b2caf5bdd8bc9fb80df8d7bf31d33012dd1af0c update api
64dbe54e2214a482d37fab2417ce301e98709522 change clusterset to cluster
15e5ba405ca76e5e5c789cfd535babfe4f61677b Merge pull request #246 from qiujian16/conversion
07bf05d3938d9f0dbe864486e02c9a65715b99cd Merge pull request #245 from ldpliu/adde2e
0d8f546fa4b7b6cfd5dc4ad832e94fef2482cbe0 Add conversion func
37ef0a8d303d92469ce3f9fb5794b72a269e862b follow review
c7b05d55ae3d9edf6db587089cd00181043b1d93 add e2e for clusterset
49fe471a71442d6f00b364017d74524a7e171dcc Merge pull request #244 from zhiweiyin318/randomviewname
0ec44b1b39b1367390ad3dc57e29925e25e5f91d generate resource name in e2e
c0cd1df2c0f19f47021d4bf17ad801267771b128 Merge pull request #243 from qiujian16/inventory
15a746a968c2827bf3deb49c4a249b199721d290 Merge pull request #242 from ldpliu/fix-permission
6c19b3fc4a5836d56dda3ccc1dab3b3238221bdb update to hive v1.0.9 and adopt clusterSync API
c723e99754ace5931511faf0769bc45a5896bc98 fix clusterset clusterrolebinding permission
f328606535228cc9f3c100ba703047160eac2379 Merge pull request #241 from zhiweiyin318/fixroldbindingwarning
0f7cf11997166f454c2506680264f526210e744f fix the failure to update rolebinding
d8f38c9b2723a38a84480000cfcb06e488fb0fc6 Merge pull request #230 from qiujian16/adoptmetav1
0ae1908c1c7f60eb9321729a26a31dfffe976a23 adopt metav1 condition
e63f54ed99f05d4d2691d8cdb952bc3ecc8815d9 Merge pull request #239 from TheRealHaoLiu/add-TheRealHaoLiu-in-owner
88c021c9f4e5df8eed22f015ca73fbf582b31b54 Merge pull request #236 from ldpliu/sync-clusterbinding
fa29c9ea617080d7bd50ddd4d4aeecc0827d93aa add TheRealHaoLiu in the OWNER file
bce0ad5f6112d259ad15f1bbe4788f6844d33a1a change binding clusterrole
72c2cec9a292ab6378fa37adfc0f2745cda40c5a add errlist
1eb1ab84563dd53ec0d05a00c9ea1f315eb9c789 add clusterrolebinding controller
ed244849f21c29c6f970fe19d0c6a39a9676db6c Merge pull request #232 from ldpliu/add-clusterset-subject
7d5ef039955b594f480b139c5939fac9f9cb70e7 add clusterset subjects controller
2299d656be05c25cdf97b095b353eb667ca2e04c Merge pull request #237 from zhiweiyin318/fix-codescan
95a36c53c2657b69f5e9e20b1e71b48d490a4b04 fix Remediate Static Scan Findings
db21ea3e63e5a58c24084a2bda354944c370b612 Merge pull request #228 from zhiweiyin318/clusterID
04d51ad4beec080c333511db4368f78fbf31dfae Merge pull request #233 from zhiweiyin318/clustersettable
2576acd3c7d0550e5cde2312c8e899399a311146 Merge pull request #231 from zhiweiyin318/tls-minversion
43c84740bc81ecb1c9a69c82282c837adb138f9c add clusterset-cluster mapper
ce00948dc5c6188d635a76c4afea3dccc1b4ce5b speicify the minversion of tls
59da25f53a2a8d95a225de6968cfef785ac3f02b add clusterID label for managedCluster
fe741169d6b63e27a04fa063d876901fb79beef2 Merge pull request #235 from zhiweiyin318/deploy-registration
10fd681f1303af643be93d022a7fcabf230eafaf deploy registration-operator using manifests
49613eb91583068c44798a969fd57ac995ceee5b Merge pull request #229 from skeeey/fastforward-test
6608bdbc41185884320c53215b3dcf03c8a434ff fast-forward test
03b3729134ba8bc8b2a19602a5732382655d5fbe Merge pull request #226 from zhiweiyin318/remove-managedclusterclaims
a9da001071700197e191bcbfb53d4025aa97d7dc remove managedclusterclaims api
aeff56063567c3fca2bedde330065dc076f8f9dd Merge pull request #225 from zhiweiyin318/azure-vendor
7c06a2c915b3654f071bf4674399a126414ab40e fix wrong kubeVendor on Azure
f70295614b0f994e997bfa132f09027ff6614b36 Merge pull request #208 from skeeey/e2e-refactor
bb4c35138a4a133e04151072ddbf7ef2ca12c7b8 Merge pull request #222 from zhiweiyin318/remove-acm
7ca0382a735b589e21e76a18fe342d2d36f6cc58 remove the acm references in binary names
bf1c0b4d602ab3c19c6923c2b6cb531e91a10d74 Merge pull request #224 from zhiweiyin318/fix-proxyserver-deployfail
efa3f7a7b88a0ffd0f26a746fcb416f478339c72 fix proxyserver has no permission to create dir
57fd11dcb7aa7431c86a05e0451cd9fdb0854081 Merge pull request #220 from ldpliu/fix-run-as-user
78c585c49032d38548cf4821ed7d41e8692c92c6 foundation need run as user instead of root
447677c5e0ed533e51a091dbef3604a126b55aff Merge pull request #219 from elgnay/claim-webhook
d1aef73e2d247215d3c1aadf17e64d7deabf2c6b Add validating webhook for managedclusterclaim
e2adc1efc65fbf1f2efa2703b59263d313883fee Merge pull request #217 from ldpliu/add-hack-dir
3d3cb09c41ccad0f0fb6a28781cfee0eb3381a2f test prow e2e
cfe4f25a134130cd3cfd9439215cdd273232b1c2 delete useless code
bb9c0e81390bd7954c67279083939018feb9e438 Merge pull request #218 from ldpliu/fix-label-test
fab61d0b5df28d89ca83d238870ad88f34c8a771 Merge pull request #216 from skeeey/fix-managedcluster-deploy
1ef856c538fe62a2715b482a4d535b57ba917587 deploy foundation agent with manifestwork
43f65c09635345ca9a9ed4c31ab98bc7eac71190 Merge pull request #214 from zhiweiyin318/remove-acm
b5cc847b1cc35bed9b877f6ab6b9948f2517bc63 rename acm-controller dir to controller
85ef612b72ec3baf19b26f165c1572f2dc527771 Merge pull request #210 from elgnay/claim
dd336d54ffd2e3513239f99c78ebc2ee19af873b fix label test
bd5659c8ff64d4ae4d71d895db38171953b2ee76 add hack dir
2dcdcf87e21eba791797e509c11233e658110bde Add API ManagedClusterClaim & MirroredManagedCluster
17a7db9d43ca7421cf1413080436dd03e4d5b37d Merge pull request #212 from zhiweiyin318/rename-internal
6ce3c10b3e9d68dab3d81fd50bc353cff9e92f96 Merge pull request #213 from skeeey/fix-managedcluster-deploy
d97730f813a6b681dffb4a6c1b3a7e215beb96bd fix managedcluster deploy
bfc21f321eab0e27938a0973077e62ab7e93c3ed rename internal api dir to internal
53979dda9683bec4d35e9dab680de121e637f48a Merge pull request #211 from skeeey/fix-managedcluster-deploy
eaf042de0a935f6a9a8471e6dd9a0e8d3a00e1dc fix managedcluster deploy
ef7625c86c1422d6cfa15701219a390a360b479c Merge pull request #209 from skeeey/fix-managedcluster-deploy
4ac8ddf3fcb5aaeacf4cf80a851a0f63daf7ce9f fix managedcluster deploy
e148950c5a7dd9e0bef7d1c1b28ac8f34ce2a3e9 Merge pull request #207 from skeeey/e2e-refactor
4a9091616cadef79d37b745a9230cd49a4fa1fea e2e refactor
e224c1537af3c923f721eba3e98f402697f2362e Merge pull request #206 from ldpliu/fix-dockerfile
1dac3034e3b2fb901069f26ac04e0539dada5eef delete user-serup
f6e9f4bd0b3ee0b1a9ce0b6b8233e7f957899027 Merge pull request #205 from ldpliu/fix-dockerfile
06bbbb650c2568a065b2fd0c188cf404f0d2ef4c fix docker file to build image
d27c22b0fe6464651c543f297d5666244fdb8dd8 clean build-harness code (#201)
b8ba7012a73f305208d936356e2cbbafb9c92f24 adding apache license (#203)
773d9477c6f3b046bc5d10da4e78b97b5f733058 fix e2e when managed cluster do not on hub (#188)
f8dfb42d08b8374464f0b255dcb7cfe308103e30 remove certs and protobuf (#202)
58f7c26f86153692c5453cccd76fa0dc75d83654 add clusterinfo condition (#200)
d7a5077aeecd0c3b857744f7a3e94c0fafc5065e add vendor directory (#198)
1e37896ef108550323214c7232b253df7fa5b578 update kube version (#199)
0685abffc5c0570cf4f260371862a57a5c78ed63 Create SECURITY.md (#196)
8c1c575db23a7f2a616b9ed018f64c97596441ee remove old apis (#197)
6cef9c45ec686af5b95775e22c4bdf3cb8151bf9 add ut (#194)
38dd173f586134d2c791ec369568db13363c45fe sync inventory to acm-controller (#193)
e7fd4de9a44bd65ea05fc4b94c010a8765b21f28 add reload apiserver (#189)
2968ab5b2b810bf015ea9da520d147d08f75ec0c do not return when meet error (#187)
23a20605fb8e70d2e371fda691ea5aea1485de33 fix e2e when managed cluster do not on hub
d7120842f7a6b86c46349e3f15746c0d88972d35 remove ns access from dynamic role (#185)
3e1c65d6d3cb1788a75c818fa98210498fa7b7fe add 2 nodes for kind cluster (#183)
4cd6f2798bc0ec5dcacd1e69c193101c9d5b0366 fix clusterinfo ocp distribution (#181)
47ccc9f5fb776bd0245392240437ba4cf63780e2 fix no log service (#177)
e611aa268dbb725438fa61ad2d0fd323f96430a8 update labels of managedclusterinfo (#178)
8120f61bf0149426fcfe93a73f52ba9cba71c38d fix vulnerability issue G601 (#175)
15ca13d50bf2999e0b86c06a5e68985089cfe5d7 update cluster role (#171)
f5a932a72435676dca03468ccde518d1ccdad239 fix namespacedName (#170)
f7d06a37d9be6e8ab3561d90b750b1acf4895c7e add clusterrole and label (#168)
ba06ad52422eb643818bb693f34ebffd28814b0e add auto detect vendors (#167)
3965fdd47134fd1bb6292b828755d97a351bc43f update e2e readme (#164)
eafd6586a34652df589efc7211a02340f46a8dcb add deny ns webhook (#165)
65dac50ac459a8c8a91ac2ccae8299c5fd623739 add check deployment created successfully (#160)
bb468f299408f96f88821fd8b2bce71ef3d63137 add acm-webhook (#161)
76e2cdcf6e88695c681708c3a7469a548b5d9503 add clusterinfo and delete cluster in e2e (#156)
336aa7402fb659a0e1e3c6dc71f6b3bb86071445 upgrade jsonparser (#158)
7cd7e75f11173df2e637a9e72dc018402662b569 add changes for bmh-online (#140)
c8a49ce5551fded0a63c92c6f1a4ce87780eb81e add rbac flag (#155)
413616bdb738db0997b53a839b66a759d02bc87f change e2e action (#154)
9f81f1239bc6074a0ad521d453d0f5520796148b update role for agent (#153)
aa21260ae3d936d4bd7106368bc6606a18b48042 fix typo (#152)
fc921398bbcea3685c323277084cd67606663889 add property for clusterinfo (#149)
3c8d0d42c07b69e4179cdfc4e89b04d472dec73b update version of docker-credential-helpers (#151)
84ac09fa211d488d612d6d5460c2a42888c4d9fd change to managedcluster (#150)
5a77d73067cd620fff80c776b237a61a3cb162b2 change cluster admin role (#148)
162256731fdda0085261c694d72603d31a52714c rename spokecluster and klusterlet (#141)
70350a5485a535f3b5221f945d6e954597586793 add check if clusterstatus is null (#142)
31089a401a316b784dfc45f6ee439a2dfe8a242c add ut for klusterlet (#139)
c4322c8cbc2749344376e8a7ca31dd24ca62f198 add ut for acm controllers (#136)
7025e4b71db22ff3ffd349251a0f71f5b3641a72 fix get ocp version error (#135)
6b65884f7785012e19115ac887e9361b076e8d1b add gc controller (#131)
08a06646adaef47afc5828f24632981543f9c026 change conditions in ut (#134)
9af31fcdb2cd436dc57c39c1a7b52af65f995453 refactor conditions (#133)
d31da6291a5296480c7b26bd5b93b329d7118b13 add ut for controllers (#132)
105b880c302038dde60aa372ba704ed3930c593a add clusteraction e2e (#128)
673883ae72e2082d7f9f5dfe5382b7b09d9770e2 add spokeview e2e (#130)
5b7cd78e0b9c3ecc75d01eed64128c1fcf50d2a5 refactor clusterinfo (#122)
c3969e5e2ea19504e6b9a842c419ab46329a89a5 add health check for controllers (#127)
3e6ac6383b31cc8b34e6c82b2c00668634360c20 inventory fix (#120)
89fe3a7b7cd8f5a6befe88c0769c46a4b7eff09b add docs and upgrade version (#118)
1aaaaddbed1d480f952c3f58b8c34272c3a59e94 add acm controller (#117)
d5cb5069f3c4d230f9f97a666b13733b31c8f53c Add dep on api repo (#116)
7d07078032edf6fe7a764e3dbb92483702e7365b add spokeview (#111)
f483ebad9048b0c25c978574ecd395cc09f85993 add log (#110)
17f174630f866b85e3e5e25f8f464da9d444799a add ut for cluster action (#115)
5054a6bb17dc2b618cd0a47716f852881fb8fc9f fix vulnerability issue (#112)
f8105fcaf90401ba9faa9dc78f4ca61454555aaa Add basic cluster info (#109)
a23a48cd44681ed77dc907a0455ec0465dbaf4e2 add clusteraction (#108)
b5f8795fdfa19e2c3707016fb78eeb3316205f86 run agent (#104)
0090098e02452c408601e39b3476df24ccf4d324 add acm-controller (#99)
3e184790ee23517796b183970fb6a4c80ff0a1de change version v1 to v1beta1 (#102)
dbdc2b0aa35cfcdae56253527e8a82d3099169e1 acm-proxyserver (#98)
cf86058f51b88b6d1493a86aa8145bdd3d8bc9f2 remove vendor from master (#101)
fbb1f50ace845dfe4ac729ac832a7808dd2379a0 Change to crd mode (#96)
e1c801b92453bd00f86278a37b77f072d47811ea Testcases for inventory controller (#92)
9b19a0a6c901c54bfb4087b750b9da69cc57a724 Vendorize build harness (#94)
cb8100e5a3ed0b83fa32be428dfa211ab50eef5c fix gosec issue (#89)
10e690a4c0b5fb8592427e509ac8ba46f609a4d8 add ut for klusterlet (#86)
b1e8f3d3750baaf6a3d849207b3214c9eab6a685 add ut for registry (#88)
e86830acb40063a852098303e80821ce73edee1c add copyright check (#84)
93c5686cff167cb40cec19fbab2c83fe8f7d3c3b add ut for storage (#85)
8de3164b3ff84f9121dd5192455846cf79f5d67f add ut for printer (#83)
04065a9131b3dae5fea4440a4fcf7b6f6c85e78c Update README.md (#82)
7cc30eecade8f45504f4a72a04012d1f32a4cbee using seconds not nanoseconds (#78)
ab01e775761d014dad3a1ad463ffc9039f6af25a Add ut strategy (#77)
f50c9fc4cd9565aeb9a8029a1c4d5c166ca90e5c Handle updates to clusterDeployment name and namespace (#72)
5a468f74f67be0d02831c98b4d6814bf6ac4457a add sonar exclusions (#76)
b80b3f572122aebb644c48341b8c7e2bd7f5e627 bugfix: missing return after syncset creation (#73)
e3e099cd3ef275e28f1cc33022512fda2d9097f0 Change group name to inventory.open-cluster-management.io (#74)
12b111eeaed9bd698c376aeb3d639bca9338ab56 add unit test (#69)
f16fa5857c376417757b8837e898684cfa105e32 add e2e case when threr is no managed clusters (#63)
f95264eba7ace9530afba0e55449f50c791f215a retry if connection manager is failed to connect the hub (#70)
2353cccd2cece6360b49501183ecc4af4149d6b3 build-image support (#68)
c386e72305d3381038582da577e2088aea88e06b Renaming the inventory package name (#66)
9e047d716b4d664f539047bbdbf09b8aef0c2132 Adding docs for using inventory (#65)
f104124fcb929d8bb6aaf48aae1bfdbd45c36f56 remove KLUSTERLETVERSION and ENDPOINTOPERATORVERSION from printer (#62)
8dd2efb45c6c8afa49f9797f2ba566dc4bba5b0b Add clusterregistry protobuf (#59)
7c8310c530f09106dfaa8f3873438cb7882e7a87 add cert rotation e2e test (#57)
ac8ab150c2e24da209e44b3d36c906a6700db924 Update deployables API group (#54)
696e5abd4c3bb4558251c952356b6ed4c4d5e1b1 using label to select pods (#52)
23ddca15837ec362ea4c5d7828c0412d40bdbb5b add protobuf for mcm apis (#50)
3168c0b6f0f528ae7f5b92eb4f05b77061f6efa7 fix security issue (#46)
d2c4f51b3f44f29dfb8f5117156278712d011c87 sonar onboarding (#45)
99bb173e5e30ef116afa84c4ee842227b543dae0 Merge pull request #43 from open-cluster-management/fix_mongo_env
87086385de4252b5b598247ded73e97587dd992a fix mongo env name error and default options
16e92f7fe944a7b526de840fd30b8e6d8418ea9b multicluster inventory integaration (#27)
d6b67755fdab705595890ddc3f7a28adc054eca7 Merge pull request #28 from open-cluster-management/add-e2e-testcase
53be7b736673fe3243b2cc3459c52ae375502f24 rebase master
51069957f1e8d3a6cf8fdd6c6f903dd9f4ebd271 fix delete work error (#39)
299aa28a0d8c9933560c0e376abb96111b0e48d1 security enablements (#35)
24e4e2e19263b86b23dc17da3a93a67bbd482531 fix nil pointer panic and empty namespace to get resouces (#30)
e2508d20926c94f40a5f538f680010c8207cd300 Upgrade dependencies, pinned to k8s 1.16.2 (#29)
f25c281078a35af51232ed28c59ee6f809ddc638 enable security scan (#26)
de714a7a788986b2b97c3afe5e0114dc27137a14 Update svcdiscovery readme (#24)
39f4e19d2e602445344440e1b0992b7568e026e1 enable e2e test (#20)
0b442005ec4f0664fd1e18d271a97814ab2fc2c6 Fix conversion bug (#19)
2dd783acd6aa17972b54294099a9fe9d04c4a8a7 using quay.io/open-cluster-management repo (#17)
0068f5a35a70e6d7ae865d7f229f2592bd1e4316 Add image scan in build (#13)
dd072810725884de177841abb2fbe65216f105e6 remove endpoint version (#18)
bb66ad094793d22bf0e3fc185ab9f00bb60faeed Remove helm (#15)
a50b4f7493fc3f26e716eb842522eb3335b87855 add role for subresource (#16)
b19384df091f20779bdcdbd23d5cbf0ee6bd16be enable lint (#12)
a1cac8f162b877806a45090f7136f580812da651 updated ubi (#8)
66818683ff9a5456fbf2e8c8d4527dafd3732940 Remove default tag extension (#10)
2649bb00f1d0fdb0fed71c5f527bf35d7480919e Only build on master and release branch (#9)
f2d4f294d12560dca5944436016f4ada4d5eee73 Add build-harness (#4)
0e6bbaf8542f30171885ecdb4aa92232cb6a6945 Merge pull request #7 from open-cluster-management/e2e-test
6e0500da0406ca77ced103076e89715de264f093 add e2e test
d2468084f1aeae4a210e9a2b13ccf444c675edef Merge pull request #5 from open-cluster-management/sync-code-kustomize
54a5526be72198ecbb2c9d0ca7e6a5a5ce293020 use kustomzie to depoy (#60)
cb598d84884a963962c402b5a711fd83b3167769 Merge pull request #3 from open-cluster-management/sync-with-synerge
4a93473729bdb9f51e544041c0cf03cf2d24d44d sync with synerge
2411b612471fb91321614eef7c1f2a5facac176c Merge pull request #2 from open-cluster-management/sync-code
b19ffc2b9cae3f0894ca0716d7b05db2b47f4203 refactor v1alpha1 apis (#69)
277b18c6a513dfe0eedc8a162d7003a6b1073b36 change api version (#68)
67cf79c3876893b030c238de9ef2020fbbb0ae42 move request proxy api to v1beta1 (#67)
035f20ffaaa06b3a754f5577f581939b1733c0b4 Add sonarcloud
e764a2687fbdc742385e3ca34b1800b61cd6d59a Add sonarcloud
9fb9ea30fbd1d6f241f04463a129c4d5a7f85bc8 Add sonarcloud
e02b96abb3c8cf2c944e844016de47a1b0588604 Add sonarcloud
f5321a030be1b0fd2a2f7ffb9ea0c58aab942630 Add sonarcloud
c034799575eb8f50b29dd2065c7e10eaa76be351 Add sonarcloud
ea1d4c834d56ba47b941f4e7f502f5e492c97e6b Add sonarcloud
a8ca3e3ec36f1c780dbd89ce50ef49575742bfac Add sonarcloud
de72cfee22578e2cddacbdf8346fecc2595f6d96 Add sonarcloud
db5d6abc4cf2eeebb7b7c9fdf6bfdd1d3148f9ef Add sonarcloud
4c0756bd63d6941126daf11c2c353eaaed055cfa Add sonarcloud
8a74658d9d4ca313cd37142f8ebef0a3bb9d74ab replace import path (#66)
380032322780839f2fcfb5cd1a7c4107fd3ac4fa Update API version to v1beta1 (#65)
0b9650bdaf3020224f840f06f6e7510ef6f7472d move repo to open-cluster-management org
fec237add0265a26db647c0385a0d15352257341 Add create options to schema for cluster controller updates (#63)
8c7730081bb3537d730249dbc2d1b04317d23f06 Fixed typo (#64)
c74548122d86565a8e6d5810f6f8a61f51442834 Fixes concatenation of a log message with the value of an Error (#62)
4ca256f2893c6e5d1fba856e2631cc6cc87165f6 2020 copyright updates (#61)
c7aac3b0a77f377fa6af571aa42bc2b71132d469 Refactor cert renewal logic (#58)
2f738fbcfcd06a7391d5ccbdcac35c7b3468ccc8 using an uniform binary name with build (#57)
dc4495e85d0674dd3aed2d116bcab629bae18981 parent 9bd9803120cfb05bc8aaf2fb65e6a71b55e88bb6 (#8)
9107bbbe0f624d04ec5d5d11a494a1c4a6337560 label fix and update to readme for spoke clusters (#49)
9bd9803120cfb05bc8aaf2fb65e6a71b55e88bb6 add proxy request (#47)
e7ad575fb4802fe8725e2b8dd6402672743491a0 fix klusterlet version is not right (#54)
ed44c09b5709b2ec4b40551fa7ee727086807840 Add endpoint version and impersonation (#28)
96743d92a59d6849801375025ff0852e7b0bc934 Using refresh ca instead of restart klusterlet server (#51)
5d7a76acd75527fdad01ac53b68d5a31c9513038 Chmod of config docker script (#52)
1d793098c19fbb2bc055cdd50986b2ceb34736c5 add service-registry and klusterlet-endpoint doc (#46)
5478746183e65c4c841573020db64cb3dd0e0a62 Change registry repo (#50)
4b811c295ddcf946aee1fc31d67f6fbc6b5ea9f1 Refactor klusterlet bootstrap logic (#40)
2a00f13bacd7ad064e189985b8fdca010fde0445 Remove controller cli flag: enable-bootstrap (#41)
8af5c24a2c2074deff0a7dfdcf5f9834e09518cb ocp-scc (#45)
5272a9a00d2aa73a52475b5d7e6eefb5a69fb785 enhance cluster join process doc (#39)
ae8b5894dcdf5868cc73568caf322e2c31e74082 add resourceview work doc (#31)
f7cbcad28930dfafe076a623003a8ef24e6444de fix markdown ordered rule (#34)
07c98a681b0f124b4ebcdbdbdb9691b029e912eb Remove godox (#35)
7a74eb228bccdb460a8e16ad7b4214e609da370f fix lint checks (#33)
3efe67eb14ea480549ee33c512f02da9355860b8 Change mongo to use appv1 statefulset (#32)
b49b38a10b4df5c6d4f6b37d3851508b2a7267a9 delete retried in workstatus (#30)
9b744a2003c60759d2178ea1c461bb52e3055e59 add doc for overview, clusterjoin (#26)
2b911cf30d641396b80183eeec2240a1d522c524 fix golangci-lint checks (#27)
e07b140167d5c9a2e9940c8ebd39b7aba032f5d6 Add persistent storage requirement to README (#19)
47ec5551c803d3565f612c84694c9ea06a418d35 reduces controller replicas from 3 to 1 (#17)
df12969f561d4c50a9ca9fef57e2dffcb16b7a1f adds multi-stage build to Dockerfile (#25)
3135a0cc28ab58d8cd63720882a98ab12ff1f12b logs actual error loading bootstrap server (#14)
eeff084eb048bcabb2088a74d77ab20fc36fd1a4 Fix bug when updating resource work without labels (#18)
9c2f45046e0706f76db5e4d1015afb2b720d719a Add more details about bootstrap kubeconfig file (#12)
be6eda89a61cc33e37d377389d202e61abea78b7 adds instructions for populating vendor directory (#15)
7efe9f34ba15fa66bcb51a462579e18ce7d2384d Add policy and binding back (#9)
7dccdfcc7878cf197fa5b6074cbb615529fe7ec6 add owner file (#10)
1520a9f29769bc46ed4eb60e6b6e6b21d3849596 Update readme to run on ocp (#6)
e7a8a66edf6b85e1a0f1c0dd6ebc4a12a23302a3 update badge (#5)
dae2c3180b612ca01e69bf38f47d3f74f3f47544 Merge pull request #3 from rh-ibm-synergy/test-prow
49bd8f9db945ed801a9b39e20909789d3792cd49 Test prow
341f0d6a1929bbde96911cebb381eee3476f5686 Update README.md
ff2075755891eb2430f59a9ae5d6cd87186dc4ac Initial commit to rh-synergy
```

Status: Synced commits but not tags
