## Syncing stolostron/managedcluster-import-controller with stolostron-engine/managedcluster-import-controller

## Status Summary:

backplane-2.1 -> backplane-2.1: Synced commits but not tags.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Synced commits but not tags.  

### Branch backplane-2.1 -> backplane-2.1:

New commits (first branch sync):

```
bd9079866b1854c410e7660c853a1a8200e48543 trigger a new build to fix cve problems (#162)
d46cce69e110bc63d04848334aa57d285c5a6656 Delete addons while detaching clusters (#161)
cc6cab558ff07ea844bb0c106f53350f900b352e fix error logs caused by empty annotation (#160)
a600d1882b091d83950864f08f8bde29861b8190 fix nil cluster and add more ut (#159)
3e07cdbe540adfc91563b2799deea0a4aa4e5134 upgrade hive (#158)
dadc2f0b919a8e236b5f1f8d6c559354a65caa51 update imageRegistry api to fix issue 21706 (#157)
7ad888d822942a832ffadd8b267983a97521af22 fix the addon is not foce deleted (#156)
40446777be20156e790be1cbc771b66b093ffce2 fix the lenth of sa name is over 63 (#154)
e2771248ee1b126ec89e415ac8e1afb9a5f31d0d fix no indication when automatic cluster import has failed (#153)
8faaf89aa9308b2d4f3682809946eaa466d69fd7 force delete all works in hosted mode (#152)
da808d535155d2c3872eb2f4b9c04b5f683477ba Rename management cluster to hosting cluster (#151)
785fc3321ce94d3b68f5953e0b9b3ec5e821b846 add auto-import-secret annotation to keep the secret (#149)
7da8dc8b79d0ed8373399d2a1f2135c16ebd781b add disable-leader-election flag to klusterlet operator (#148)
516d1b0dfa34b3551f974d5d6e37a38b963066c8 Replace metal3-io baremetal-operator (#147)
3a3bd02377a8609747d0df70ab672575e0b9b6f5 Update Detached mode to Hosted (#140)
ef5fb4f8557de9b6ce1a421a4b0d654ce4dfb20e Add doc for klusterlet detached mode (#136)
6453bdbf103114c00b2b27097c3c9161f58a5922 Add lease permission for klusterlet operator (#144)
08c3d8d5870dd7d7f74c4f58a6bd43c392b82bf2 force delete addon with finalizer (#139)
e3cb866bf029a9e4ea7d02658ac5b78f684854c8 avoid to add finalizer to manifestworks if the cluster is deleteing (#141)
280f254fb3755b138d9d02b861ff49a24b2e0185 wait addon manifestworks to be deleted (#137)
f525df8ef1f78e0cbe3ca436215ae191226b2f5b upgrade hive (#134)
9a258bfe55dc9648b1cd9e8d77d5cf4677c7b55c Make klusterlet detached mode decouple with hypershift (#133)
69e9935169da73e3edea4f628dd4b61bc04c36d1 correct the type of secrets (#131)
552d4490b31ceed61bf0535bb3a6a0ae5826b143 update klusterlet CRD (#130)
d77f24523fd6d356b3772c2cee196462cd1ee423 maintain the cluster name label (#127)
5b379fd119f5f0666660e728618186c798abb26f fix: create agent namespace first (#125)
de744393736edd463b47ba64f925e567f5cc1599 Import cluster in hypershift detached mode (#124)
5ba29c770be3e69083075f3b8ee0a708dd939aa1 Upgrade klusterlet api for detached mode (#120)
0c5ad0e12e0bd43a4984fd31de36d62ac56ef6bd Fix flaky e2e test (#123)
8bb4e99bbab3f6fdaa963167c8b3dd852a64f6d6 delete the cluster namespace, even the provision failed (#116)
6610737811b8f2b57661a3789ee74e3d21ebc078 using claim as the cluster name label (#117)
6922f767d2c1836111d0e26029c9f22e78fe04b8 update crypto (#113)
836b15c4d8c72826a489444ba50677bc2637a0c0 rename repo org (#108)
884905557ba9e956ec7f975c01c72a7e6d577307 change imagePullPolicy to IfNotPresent (#102)
c8d23df41475a2786565bcb2eeefbdce7b904d93 update go to 1.17 (#100)
2fb6f7e429c8fb7a316f767236ed47fdbf52c883 customizing secret event sources (#88)
d1d7bb50894afea7d1212cfa23c96627d3553821 fix hive create-via annotation (#97)
db83a60d68cfc0e6e2bc22ed93db62c9edd9c8dc postpone deleting manifestwork (#95)
2f67172b940f8f1f56f9b350c84a733393f382ad fix cannot delete ns if no infraenv CRD (#94)
188eb1c9502a068f0b65611776d4dfd889d0495a add infraenv rbac and crd (#93)
bb3fcebb22963f928b800198230931b5a779b4b0 fix InfraEnv is deleted when the cluster is detached (#92)
04c70d452e8ab693f964ae1d8519db149ca13be2 upgrade hive api (#91)
f1db62bdae67cd26d14c7ae6ec621ec3b6b9a0b0 using patch instead of update clusterdeployment (#90)
1d46075f5039d4a023b432ce63a53086758bace0 set the cluster name lable if it is empty (#87)
a1b8b5e4ff9aee92db2d1e10970b11062d3619fa enable refactor code (#85)
1c77a08dfb0d096d7c2811b98c7669669b565d1e add nodeSelector to the pods of klusterlet (#84)
be5a2a41f884caf588d5c28d5fd4d83a361ddd90 upgrade hive to 1.1.16 (#83)
cca3ac9eed5186f1fcdea28718c4a3228b04a265 add clusterdeployment-controller (#82)
baf1453bc1c87775f1d175a1c98f174e3a75eaec add autoimport-controller (#81)
35f5fe30a97c227a45f0dc032a5b5969316d0e26 add e2e-test (#74)
7de5b621cbcf0c2962d5097addaf08a4dfe48932 add manifestwork-controller (#79)
d1c125957104a51908b4b979dd3a5ef9c8ddb7f4 add selfmanagedcluster-controller (#78)
c07e545953969206d67a69712994365b4d6bb5ca add importconfig-controller (#76)
a87a9c8167530476cacb768d7df274cf1ad4685c add managedcluster-controller (#75)
b7f61076e4e96c11861213e0312528369a383f38 add importconfig-controller (#77)
f6651a95de03c688599afdba82a765e742cef089 update helpers methods (#73)
f643b5c20db4f16418346f8f7b3d5b639b385b81 ignore temp dirs and files (#72)
5f53d3e83e358f18dbfabbfec74e869f05ebe338 add scaffold methods (#71)
2a016c67ad5393b106cb909c6931e14778ce073d image override by imageRegistry (#66)
b5e2e7453065fd92bb9f9b184be673734b8ca1d1 upgrade certificate to v1 (#69)
1d0033e45d6fcdae496065041260e9dfbfc1f7b2 upgrade hive to 1.1.12 (#67)
75d85b3b92926632e831328c781719108da27b59 upgrade release version to 2.4 (#64)
33cf2014906d2c1d3087ccbee6d1dd0b3101098e Check if pod not ansible (#63)
4d5abcd08f622566775dffca5142a8c059518dce add owners (#62)
f25cd42944797ef7c1e2f7044aef3b3397da097f Add both crd on mw (#61)
f3303373a6de4bdeef7248b21e48582abd92e1b0 Add business logic for created_via annotation (#60)
4139ab23219e442642524d8d22c83a5bb60e83d1 Fix prefix check length (#59)
cb39f921673aaedc1b633ccf9b7f60be0e34b0ee Update operator name (#58)
6ea6de1ef891eddfca0cc8ea54923356211c026f Use Patch to add finalizer (#57)
04ce97102981f63f3a58ee0675a1e3b54cbe6cb4 reduce reconcile time (#56)
cd0568009f32a7a8bd1d19c83fc707524cd92620 Remove imagePullSecret from klusterlet (#55)
fa0a3fc815cf17f8d10434314184b4c599a4684f update hive api (#54)
803564b2fed4031656a4bc2a0532655d8f4d67a9 Add CSR delete/generic predicate (#53)
dac8750c3a8e9a716dd349b0d424e81cb644d43b Merge pull request #52 from itdove/curator_pod
e007a2cf5d2cf1046eec5b899f22f6ff179d0aae Do not delete ns with non curator pod
86692a1118dbe62ab337af512d68fb12fdc093a6 Add MAX_CONCURRENT_RECONCILES (#48)
3f21ba2179a88c1953679f7413466fc69dc402b4 Rollback v1 (#51)
6d9ab6562748f26fccff6e2fe30392547558ff0c put v1 in the crds.yaml (#50)
29f2162aea0ffee1dbd7854087cf8cd13930f755 Add node permission in for klusterlet role (#49)
aac576a3a875457051e6c5971021842add3e6ae4 Upgrade to go1.16 (#47)
25f9330e8a7665f2eb806792d6f6b55d81acf07d Add management workload annotations (#46)
47526c7bd83900d4b7e48f62b612ead77896c1df Use latest applier (#44)
0190b8711cc18a9aff5a2f0a7ef10fc14cb26ce3 Upgrade the hive api (#43)
db26ab1550cc739e2816ac8fc0020c95718bbed6 Fix unit-test self-import and add extra unit-tests (#42)
1ad4efee7053ae3ae54f65767c20cd2545b00d26 Add commit-msg hook (#41)
0d82f933f4568f73f03d4c467ae5ad809d5d21f3 Fix kubectl versioning (#40)
e063bc24b1f3b970f016bb4afa2648167b282b36 Port from apiext v1beta1 to v1 (#34)
bad0540a58707413393c21af39d8444f005cd168 add community deploy (#39)
fafcf26839c71e0249fb8567e8030f018d32b80f update base docker image (#38)
9d4217aadcd12910ccf808c999c835fa3866a49a Optimize processing if cd not yet installed (#37)
c38a86cc8954e0f7b39c225a29a1bfebc6219120 fix list mw with namespace (#36)
f9bd2defd1523343d665239904b44712882a6c8a Fix func tests rbac/err if failed to set mc cond (#35)
4bad4bc70b3859d9c678b9ad5e3f16b6cf3e2120 Add check if pods in ns before delete (#33)
02e053e52c9ec0e3f678da367caa090abdd65a12 Add comment on contributing + conduct (#32)
f919dcff37be79b37d0c2e69b48dfc23b194b585 Quotes for name and namespace (#31)
fd8092850988aedfe110d76a1ba3b36768498148 Delete syncset (#30)
ede34838c7b4d109c9b4365365fe6f58cd9170f0 Add finlizer on clusterDeployment to fix BM (#29)
24efb96f7b1831ab600fa09d00addcc6a2cf28cf Remove SyncSet in favor of Applier (#28)
278f396ed33aff9781e7eacaa7bc010fe40498d9 remove dockerfile.prow (#27)
6ca3b6c63bd1825bee3f75c031617ca1d23d9182 Add check-copyright (#26)
d1639a1900951afd26953fd2766d67d8e3fdff21 Create functional-tests.yml (#24)
1427744cfcdc8893b9b783ee9596029c1036f344 Update README.md (#23)
09e2ece339650791fa04e6898733a7c7693c8ece Fix auto-import-secret deletion (#22)
e323ba0210a4f7d32010d52212b8849a781cebe8 fix lint with new base image (#21)
f4ad3bcf80d8d8930519c22a43fa4b69eb4c54b6 fix lint issues (#19)
25b426368cbc860d6250a09a13fd08f2937a4c1c Update managedcluster_auto_import.md (#18)
046981aa32afc67204eea3d02c9d97701422a781 fix copyright order in some scripts (#17)
9e6265540f91ba89f38a92df6de5b3b5eac022b0 cleanup readme & makefile (#16)
b6b2e7f53d4e9fd692f2390039777fb077d819f3 restore dockerfiles (#15)
821bcfdbd7281b8cf37327f86016659709b30de9 update copyright (#14)
943e085668daaaefc2fc5ef80ec13f1f4a74811a Auto import pr (#13)
d706db929afc736abbdc7104385a698511ee3587 Add coverage (#12)
6d576f454e73b75cad427cdc0676c2b9a963b3db Fix lint (#11)
6b3284f132adae3f4abbd0d1c69d4ee933abd333 remove vendor build harness (#10)
9b7d79ba9bb2a2f769c6f4c0cbe1dd0a21f78b94 Update copyright (#8)
96679ebf1795f29024f42c01ff588bc5d8ca4b54 merge prow updates (#6)
af6b86d895d2b36953e59bf87944326e0028da22 Merge pull request #3 from open-cluster-management/fix-owner-file
f358e15589b3db654d0965e8d8d718c725710601 Update OWNERS
8f2e8d468114ded0c8c2330cf099bea3761b9806 Merge pull request #2 from open-cluster-management/fix-makefile
7a6ab67d6d59553f62b5c1f30061357faf665076 remove copyright and update dependencies
049ad3844593ccd30b6e774fc789fdc680ecc152 Merge pull request #1 from open-cluster-management/update-files
440e497c3d8f2356d575d6fafd175d3ba4f74135 add contributing, security and license files
f0b405c45473c77d8272f251c05427e5b251edd6 add roks support (#187)
55e59b543fb76b349df1ec7fbb240bb97167e006 Fix copyright-check.sh (#186)
ffe9b3335bdb08acb4d920047a2419fd5d14dc9c Remove e2e tests, check copyright (#185)
1d4b52da6357b4c7e90bf6333702cc93871d8a29 Merge pull request #184 from open-cluster-management/klusterlet-degredation-fix
acfe62f9504d78ceae850ae840e8b5c2f9666d2b Merge branch 'master' into klusterlet-degredation-fix
c18981fb9f0904613aba3e01256b05b6ad95c230 removing resource specification from bootstrap
e4da77ab2b803aa285f39374ccb7c5fcbd23a9c3 Add new rbac rules for klusterlet (#179)
cedf50639198d628b8e05b91c96f49a301431223 Merge branch 'master' into klusterlet-degredation-fix
7e8820b458d38610b50418ff9ed3c564f33df658 fix
4983c72f0e69e5fd2295a024dbb4cc84c581eb1f remove manager from test (#183)
836e0a8c14b8885d10ec969108f09616e1337094 Improve test coverage (#181)
24966c80dd0ddc449324a1bb0c3ba736c1f7718b Add unit-tests/remove packages (#180)
05fda426c0ebc0d4e39a3b5068dc8704e95e78e9 update readme to trigger build (#177)
c13d97b430b05494d4c6e3f6cccacf563bbbc3b7 add secret non cache get (#171)
50226723641ad5e6fcc80b852c4fae62855a06a1 update to 2.2.0 (#168)
a839a69dbb1e22d148dd09be3edf71525eaf5e8c Add label "name" if needed (#167)
b5502338f43d99a7185e36b82565fc6a2afac023 Move AWS secret to coverage ns (#165)
3e18a2cda3bffdc4ff94ad90b073b8fe4258e8b1 fix operator-sdk missing error in travis (#160)
eeda3eeffbedc1b93e04928663d6213dbc6c1e22 Use REST API in cover for k8s and aws (#164)
60775554c35d7525989be82d0d1cb78b58586040 Optimize coverage image size (#163)
8f358f7589c17ed6ca8616d858b4f4aa7f93a540 Add label in NS (#162)
90e5c68959d6b98a4543bae9bc41a8d4d3f4e29e devendorize (#161)
062874e6339cfcd383a72bdcf676c34d62271dbb fix vbh when in travis (#159)
df115a8a2c4d8859de676df757ddaa882230fe1d Enable code coverage (#157)
f2a9a61c56312f8820ea7984daddd704321d005e Never update the SA (#156)
5178a49ab8b2075dab5b1b72577737631e86047f Add servemetric back (#154)
4441272a8e09850da9014855a3b2485aed0da574 Upgrade library go and add predicate (#153)
86a7584861834b59eafbc6553b927a6885852747 Self managed (#151)
e9232339132e14afba1f28f4b2e55592901d8094 Fix vulnaribility issue #4416 (#150)
472ff823d73c97d1dc6571afe8dfec1a33434c5d Disable leader when not running on cluster (#149)
ad81bf4f13a5731e6b2bbb21b6616d9ec4a636ba Upgrade to k8s 1.18 (#148)
2d2ab31480e4a70c297047ce028b1f3c1c3736c5 apiserver custom CA cert support (#147)
a759bdeb5368e686c94e99a66e7723c47b117290 Remove type meta (#145)
5a65d53c78d66119844da07c0a25bc66186015c3 New create e2e tests (#142)
527bebfab5c79761d918d0191a0a18bf2a17b8fd Update cluster_role.yaml (#143)
59435867865a6df10df8b83ad253982d3ec58490 Complete exclude imagepullsecret (#138)
1176b61ccb93fd5d7ae097570495b561bf409396 update to 2.1 (#136)
0bad06e510c1219a9dd0cf86d30ae5bc1e4a8902 Fix pull secret name in klusterlet and add to sa (#134)
c9202eae405f38b54d99a04368d5fd1b55b0c5c7 Revert "fix image pull secret (#130)" (#133)
199e6bed3d00e8d2b1da60afe31fbd4965d96363 fix image pull secret (#130)
3efe6c3b5a13f20de6e528b88126736dfd610707 update docs (#129)
1be907687bb8c7a9b32511ad22f3fe78bfe1e97c Update detatch_managed_cluster.md (#128)
cf38ee61f2bc3ad8d4b2ce4e83a860d3061d64d8 fix typo in klusterlet clusterrole (#126)
253ba85f36e4688aa464c4b8e5f3cd4bd8c2ca79 add doc for manual import of managedcluster (#116)
59366d93faefbdeda2f689eb23b1adbdbea90b3b add aggregate clusterrole to let work-agent modify klusterlet (#124)
614c53519de0e4a4dbe035b17e01e97aa7d0fdf3 Merge pull request #123 from open-cluster-management/ff-2.1
291f40ae498e003d516ae18389d3a98cf3506977 Update for release 2.1
111247389cc782cee121157c77220e3faa93de27 fix functional test and code smell (#122)
01a9720e8c2ab5eb22bb161680ba4dfb028aca92 fix image build script (#121)
699669c692783b5e7c01570f7d0881b3d03978ae Implement Delete/Detach (#120)
83764a169e3ac1777e36ed251ee3091c012f332f Add Auto-csr-Approve (#117)
2fe59f34b7f92980b7745d5ae0f142fd1f04eb5d ManagedCluster + e2e (#111)
46a2b85657ab9fc032c62ed668c2af45f33a7cf9 Add microdnf update (#106)
3a67a08b0c3c1ce63056eb49d5e799e1a1c71d86 chage back image name to endpoint-operator (#108)
01a5db23bf87ba2fade4fd1cd555ec7bf2f35a9b Rename EndpointConfig->KlusterletConfig, Endpoint->Klusterlet and component APIs (#99)
a87e57dd3e1c0d9210ac5d3544b93aa0a4524720 remove service registry (#100)
dfd1f7c3c7175ab53b13e5d9aa6f19e7fe01377f Merge pull request #101 from open-cluster-management/create-2.0-release
15db92d8b06d237d82ddd67a74df239db1f1355b Merge branch 'master' into create-2.0-release
12ff0641605c5b80c5ead7d97295deb5bc6917f2 Add coverage (#102)
1ca6494b9e23992b56d6d890082958e43b216c7f Merge branch 'master' into create-2.0-release
ba2a21c57f4d91d06fdbb4de23bfbcdfc9a04eaa update version.go to 2.0.0
aa8c3befc19f8ed0b80c5697b75a2abd17324a01 Fast-forward to release-2.0 (#98)
a8d9ad2dcb071f46dd2d7d96b21299c55fde02c6 update COMPONENT_VERSION to 2.0.0
8bbd51ee838c6f0bb1410ed3fdd52e8697513f63 Fast-forward to release-2.0
25accd4ecf2962629241a4095ab979651aec1c6b Vendorize (#49)
4896ffa1e1acc7f1ca180cfadebba1b7f0a11da1 Upstream build (#96)
bc1914e6d6895ad18ef1fff286954ec16fc06ca3 update endpoint operator (#93)
ca8bfa37b061f89848e8c87f6b5a28e1dcaf4b1d fix edge case where default image repository is empty (#94)
a5266496c5964ada117d3514f986b63b1b065df5 support ENDPOINT_OPERATOR_IMAGE (#91)
511e285e03d8a096a037d735dec577cebafb72e7 Update test_endpoint_config.yaml (#90)
afa173cb40c04478786341a580b3565420b0aa40 add tag & sha tests (#89)
1cc3bb9bdd81e3f4f301cdf5595d63b3951d4b01 add sha for endpoint-operator deployment (#87)
f081df6f4d15f233a70562820233d4e480f55fcf add unit tests for clusterregistry-controller, clusterregistry delete and endpoint update(#86)
fc41c9c254d2158d5315c07c1d36233608fe07e8 Merge pull request #83 from open-cluster-management/smeduri-copyright-checks
7502092b81d076b8b0bc720f66c53527f13f9f0e Merge branch 'master' into smeduri-copyright-checks
de17c6c633ec9fde3c04424ea0b2a653a92ebcdc Merge pull request #85 from open-cluster-management/itdove_remove_kubectl_new_endpoint_operator
d9f58698514914e4de7f20a749dd3403413be950 move copyright-check to check stage
2ed7809f5d9ad25a21d9e6775a4e95e41d827b3d Update go mod with last endpoint-op
2209096e956037fbf465d63d6397f7f4b5f028eb move copyright-check to build target
4917efae96a9fa374305c7a43b2c4ea61fef3dde add copyright-check to unit tests
050d559f5d3a9e37c6988d6ce7cbba714a2ac0f8 Add copyright checks, update copyrights
5dad7b56f01ff0ec10f671af41292ef0287adcbb improve functional tests (#82)
511ffbcc70751a36cb05afa6419d853e3edd39b1 Add functional tests (#78)
c8ad39fbeeb4521e1f1b821e7b5236fd0564ea5d update endpoint-operator in go.mod (#81)
06133521b573daccc8e868c31aac72fb39cea07d add endpoint-crd in import secret (#79)
f1d8cebe8a5f4313c122fa503e8b6a15668b205a Update endpoint on managed cluster (#75)
6e6f51e2651598a5364038b00eb5add483008c68 Fix selector syncset (#76)
574a83057568366106f79dcef623beb33234a610 update endpoint-operator (#77)
373b43eecc9a16d1a93a085f07e7fba27ae7ced6 add ownerReference to syncset, importsecret, and endpointconfig (#72)
ed186c21274b3d0adc7169292fd71934b73833bf update endpoint-operator module (#74)
dfe40064e431abd3d116a41df3434fd19869697b Merge pull request #73 from open-cluster-management/rj_g304
359dadad9823f9e68c81f8295095e18050539336 #982
21c97bb8438c0b7ffcd807635fb42be821eee69d fix adding finalizer to cluster resource (#71)
6331ff34d79bb60137cdbd9972dc6889d069f9de Update test_cluster.yaml (#67)
f8986f345f84eb39a1539051a8789364adced43c requeue on fail syncset creation (#69)
00a65eebd7b13790d0ba87375e0fc6d709f0c141 fix make run (#70)
5424cb527315720537a75be9b974fdebfe9f34cf add default values for delete (#68)
6751ba83443484b3725a49a8647c2072806a9047 Update syncset when endpointconfig got modified (#62)
d0d477e3c51eebc88cf053f396639208136ad237 clusterdeployment controller should not create clusterregistry resource (#66)
76b129e53ce721bf9630b001139be35cc249252d Merge pull request #65 from open-cluster-management/move_sec_scan
0da457f49c29f183b1cbbbf3961048e109344bdc Run make security/scans only in .travis.yml
78ba9ffdd186287c94ba17101c001108e16f9029 Merge pull request #63 from open-cluster-management/rj_enable_scan
1e8f2e50b988b37865343b196f6898dfd8b1961a Update .travis.yml
e680697a3ce9862fdfd6ff0dddac9b94a15fe0ea adopt build-harness release-ff (#57)
098c38720a5ed443c2bcee77248574ea13749cce restore makefile
c0c65fc450855184c6b167292a503c08891beaa5 update order
5fdf925031ab13cf78981b11a3e0c515c393006b update comment
6b50e6112c2b0f61a6db9a3a05e5aaca2a0b0d3e add default imagePullSecret & defalut imageRegistry
7499ecb799bf99fe24b76624a83ce9c789331ade Merge pull request #58 from open-cluster-management/rj_run_sonar_scan
cb8779e233321a288168f7b277ed82b7f4e7c7fe Update .travis.yml
a7f145615cd9cca16e5ced6be1be9e1b808168ac Merge pull request #54 from open-cluster-management/default-pull-secret-and-registry
889a548738e3f6ea028aa698f536755de8a50134 add default DEFAULT_IMAGE_PULL_SECRET and DEFAULT_IMAGE_REGISTRY env variable support
f2d0ec88b751b0b1daf0bac3256766295d3e7c09 Fix import object (#47)
de05fdeb08af3d914ca6c177e18559d027b7ad3f Update Readme (#45)
223192e5144862b5735ec33e4834b98fd97085b3 Use latest endpoint-operator
2c7be032c7761f01657ce8d269d4cd0445941bdf add howtos toc
73e4153cd1b225cd78b124f923af9737822ef13c Merge pull request #33 from open-cluster-management/rj_sonarcloud
9a101b3541535da40a0b039f82014da625c13ae1 Update .travis.yml
76ca28fee3c8e11e7c9125e5bedffc927091dd70 Update .travis.yml
89eae73884d45dfb1d5f649ce7540fb327daca0d Unit test without sonar
505cc73b781cb025e8869010667614a656f7ff54 Merge branch 'master' into rj_sonarcloud
7c9dde0dace54e072d16029b94323fed47af07a2 fix unit tests (#41)
6102869961eb37f83c795d1e218e5a6d1d39bc77 Merge branch 'master' into rj_sonarcloud
f6d55519811234d4c8b65a5a6c28b8f9baba3e03 Replace openshift/api with real semversion (#16) (#39)
75e14745fac36c6b39657c3c28dc44da16d86707 Update .travis.yml
436a57e20dc33912529c9c42b58a3786701d27e1 sonar: removing debugging
62567785385c7711631dd8bf1348a77beb9d62e1 sonar: debugging sonar scanner
e02828a41bbaa5938cc2e2de1b6053c3ed8c52d1 Merge branch 'master' into rj_sonarcloud
ce5520cd9bbe8556b7e502c126974ce1096b3949 Update cluster_manual_import.md (#32)
e06d800bc12aba4904942ebcd0a04294908882e0 Onboard sonarcloud
9231801787111a04889e03efd7c3a7b28ab54ce8 remove .EXPORT_ALL_VARIABLES and use export (#31)
55ee9403c7ab59be4357982cb4a2489f07c03aa1 assume postfix always come with a - (#30)
ff32b4669d2315a8f7de6b2758a217cf788bc7fa Update test endpoint config yaml (#24)
9d7d2377f23495d448c2cce8c6ee6b1fdd9bbc1c Revert "Merge branch 'release-1.0.0' into master"
1620be8acf03746e865589ab367aeb0038490b96 Merge branch 'release-1.0.0' into master
ab821b3c65a87422f29b784749f1f5bd382b27f6 Revert "merge from master (#23)"
cf602c680e426c28785fac929830babc33064bc4 merge from master (#23)
2d3b24e9901c091c272030ed56a94d8dd19def7a Add links to manual import doc (#20)
efb318696120671212b7c4c6b5999cba96b980bf merge from master to release (#22)
92af9d01e1fa27c2c03a0255073dbf1b57ca0df4 update image name and operator name (#21)
90f229fb3da202cf04e776df9e2c41366aa8adf2 Add tag postfix (#19)
e2e69c06410d24d5d9ed954fae72e3c41a96256a Add security scans during travis build stage
7feddc127c8a71243202756627e43c10b90619c9 Bump ubi image to newer ubi8
80d99592b174a5b32aa7dde4982bd72fdeeef81a Make common travis before script
15ebbd11353307c227fe268bc1c7b7e4dce59f53 Make common travis before script
22b773a344c6130508c03268ced51d689a0b8852 Switch to new repo and pipeline
bbcd51ab8cf2315be3d5b6b96f9bfa4bc7909f7a update operator version to 0.15.1 and delete endpoint api
84d75909935d06d18d27deb4bc0e629371d0b9d2 remove cm cluster-info and read config from infrastructure
c0b5f1d8ee239749a5651adda638dcb92e38e2a9 Had to fix the tests because not correct
a6fe6a2255ad9e7910ab2e8759a4c9e455a065b9 Manage reconcile error and add License in zz file
13480d5d7908a461bd7de9c13b3991ac2af7e835 update controll version to 0.3.0 and update endpoint on managed cluster * use apireader to read resourceview and changed import for log as it is deprecated * added unit test for getresourceview * add unit test for createresourceView * change multicloud-operators-foundation version to use latest * change controller logic * if cluster is being deleted, don't update endpoint
392202f0061ef3c0a4789587c202976b502b45e4 delete endpointconfig when cluster is deleted (#41)
897af92992521581338a60f0af32b3b07eb265a1 bootstrap clusterregistry unittest (#42)
d6b9817163a376d37f7483d5f011ace850d8e09c clusterregistry cluster deletion (#27)
54a2d807e8e5db2df2f384c995d7309b8e4d45da Check if CRD are installed for launching the ctl (#35)
43b4f1ed9dcbf82e17e43a3c74609bca9d9eb705 adding design documentation for the controllers (#33)
95b7bdd339d198863ca5da69540c1e570e46f266 add cluster registry unit test (#29)
bb752c626d0c586dd9a3047b09b1b430b23c87ea add endpointconfig controller to generate import manifest secret (#20)
7c4b1a95ae3fcffdbce61f1ba2134112a6743c0b fix PROW build issues (#23)
77896079963d81a870be1a64b9e829fd15995f1f .gitignore, check dir, install hooks, add user_setup (#8)
f22a08cb80e6b252cfd27d3fe116ee7cbf3157d9 Refactor clusterdeployment controller (#7)
41721c42f11c4e39e70c3cc5c8777f29efd782df create clusterregistry.cluster even if EndpoinfConfig doesn't exist (#6)
3e6089f27b974957ff4a73b387807c91df6a0d10 add selector syncset creation (#5)
db942c5121f12103edf7bb66926d5a8a3cbdaba1 Deployment automation (#4)
3564716dcd116f66fd5e6977b18912d26ae02429 switch cluster-controller module to this repo (#3)
e664e377deae5cb7edbdcf6e4831091470ada963 initial commit, moving from ibm GitHub (#2)
7eaa8c4c7eef3a29166957d4929832afab148bed Create OWNERS
239f9ea85e644c8cfea1e5c7e2508e43b5235d65 Initial commit
```

Status: Synced commits but not tags

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits (first branch sync):

```
bd9079866b1854c410e7660c853a1a8200e48543 trigger a new build to fix cve problems (#162)
d46cce69e110bc63d04848334aa57d285c5a6656 Delete addons while detaching clusters (#161)
cc6cab558ff07ea844bb0c106f53350f900b352e fix error logs caused by empty annotation (#160)
a600d1882b091d83950864f08f8bde29861b8190 fix nil cluster and add more ut (#159)
3e07cdbe540adfc91563b2799deea0a4aa4e5134 upgrade hive (#158)
dadc2f0b919a8e236b5f1f8d6c559354a65caa51 update imageRegistry api to fix issue 21706 (#157)
7ad888d822942a832ffadd8b267983a97521af22 fix the addon is not foce deleted (#156)
40446777be20156e790be1cbc771b66b093ffce2 fix the lenth of sa name is over 63 (#154)
e2771248ee1b126ec89e415ac8e1afb9a5f31d0d fix no indication when automatic cluster import has failed (#153)
8faaf89aa9308b2d4f3682809946eaa466d69fd7 force delete all works in hosted mode (#152)
da808d535155d2c3872eb2f4b9c04b5f683477ba Rename management cluster to hosting cluster (#151)
785fc3321ce94d3b68f5953e0b9b3ec5e821b846 add auto-import-secret annotation to keep the secret (#149)
7da8dc8b79d0ed8373399d2a1f2135c16ebd781b add disable-leader-election flag to klusterlet operator (#148)
516d1b0dfa34b3551f974d5d6e37a38b963066c8 Replace metal3-io baremetal-operator (#147)
3a3bd02377a8609747d0df70ab672575e0b9b6f5 Update Detached mode to Hosted (#140)
ef5fb4f8557de9b6ce1a421a4b0d654ce4dfb20e Add doc for klusterlet detached mode (#136)
6453bdbf103114c00b2b27097c3c9161f58a5922 Add lease permission for klusterlet operator (#144)
08c3d8d5870dd7d7f74c4f58a6bd43c392b82bf2 force delete addon with finalizer (#139)
e3cb866bf029a9e4ea7d02658ac5b78f684854c8 avoid to add finalizer to manifestworks if the cluster is deleteing (#141)
280f254fb3755b138d9d02b861ff49a24b2e0185 wait addon manifestworks to be deleted (#137)
f525df8ef1f78e0cbe3ca436215ae191226b2f5b upgrade hive (#134)
9a258bfe55dc9648b1cd9e8d77d5cf4677c7b55c Make klusterlet detached mode decouple with hypershift (#133)
69e9935169da73e3edea4f628dd4b61bc04c36d1 correct the type of secrets (#131)
552d4490b31ceed61bf0535bb3a6a0ae5826b143 update klusterlet CRD (#130)
d77f24523fd6d356b3772c2cee196462cd1ee423 maintain the cluster name label (#127)
5b379fd119f5f0666660e728618186c798abb26f fix: create agent namespace first (#125)
de744393736edd463b47ba64f925e567f5cc1599 Import cluster in hypershift detached mode (#124)
5ba29c770be3e69083075f3b8ee0a708dd939aa1 Upgrade klusterlet api for detached mode (#120)
0c5ad0e12e0bd43a4984fd31de36d62ac56ef6bd Fix flaky e2e test (#123)
8bb4e99bbab3f6fdaa963167c8b3dd852a64f6d6 delete the cluster namespace, even the provision failed (#116)
6610737811b8f2b57661a3789ee74e3d21ebc078 using claim as the cluster name label (#117)
6922f767d2c1836111d0e26029c9f22e78fe04b8 update crypto (#113)
836b15c4d8c72826a489444ba50677bc2637a0c0 rename repo org (#108)
884905557ba9e956ec7f975c01c72a7e6d577307 change imagePullPolicy to IfNotPresent (#102)
c8d23df41475a2786565bcb2eeefbdce7b904d93 update go to 1.17 (#100)
2fb6f7e429c8fb7a316f767236ed47fdbf52c883 customizing secret event sources (#88)
d1d7bb50894afea7d1212cfa23c96627d3553821 fix hive create-via annotation (#97)
db83a60d68cfc0e6e2bc22ed93db62c9edd9c8dc postpone deleting manifestwork (#95)
2f67172b940f8f1f56f9b350c84a733393f382ad fix cannot delete ns if no infraenv CRD (#94)
188eb1c9502a068f0b65611776d4dfd889d0495a add infraenv rbac and crd (#93)
bb3fcebb22963f928b800198230931b5a779b4b0 fix InfraEnv is deleted when the cluster is detached (#92)
04c70d452e8ab693f964ae1d8519db149ca13be2 upgrade hive api (#91)
f1db62bdae67cd26d14c7ae6ec621ec3b6b9a0b0 using patch instead of update clusterdeployment (#90)
1d46075f5039d4a023b432ce63a53086758bace0 set the cluster name lable if it is empty (#87)
a1b8b5e4ff9aee92db2d1e10970b11062d3619fa enable refactor code (#85)
1c77a08dfb0d096d7c2811b98c7669669b565d1e add nodeSelector to the pods of klusterlet (#84)
be5a2a41f884caf588d5c28d5fd4d83a361ddd90 upgrade hive to 1.1.16 (#83)
cca3ac9eed5186f1fcdea28718c4a3228b04a265 add clusterdeployment-controller (#82)
baf1453bc1c87775f1d175a1c98f174e3a75eaec add autoimport-controller (#81)
35f5fe30a97c227a45f0dc032a5b5969316d0e26 add e2e-test (#74)
7de5b621cbcf0c2962d5097addaf08a4dfe48932 add manifestwork-controller (#79)
d1c125957104a51908b4b979dd3a5ef9c8ddb7f4 add selfmanagedcluster-controller (#78)
c07e545953969206d67a69712994365b4d6bb5ca add importconfig-controller (#76)
a87a9c8167530476cacb768d7df274cf1ad4685c add managedcluster-controller (#75)
b7f61076e4e96c11861213e0312528369a383f38 add importconfig-controller (#77)
f6651a95de03c688599afdba82a765e742cef089 update helpers methods (#73)
f643b5c20db4f16418346f8f7b3d5b639b385b81 ignore temp dirs and files (#72)
5f53d3e83e358f18dbfabbfec74e869f05ebe338 add scaffold methods (#71)
2a016c67ad5393b106cb909c6931e14778ce073d image override by imageRegistry (#66)
b5e2e7453065fd92bb9f9b184be673734b8ca1d1 upgrade certificate to v1 (#69)
1d0033e45d6fcdae496065041260e9dfbfc1f7b2 upgrade hive to 1.1.12 (#67)
75d85b3b92926632e831328c781719108da27b59 upgrade release version to 2.4 (#64)
33cf2014906d2c1d3087ccbee6d1dd0b3101098e Check if pod not ansible (#63)
4d5abcd08f622566775dffca5142a8c059518dce add owners (#62)
f25cd42944797ef7c1e2f7044aef3b3397da097f Add both crd on mw (#61)
f3303373a6de4bdeef7248b21e48582abd92e1b0 Add business logic for created_via annotation (#60)
4139ab23219e442642524d8d22c83a5bb60e83d1 Fix prefix check length (#59)
cb39f921673aaedc1b633ccf9b7f60be0e34b0ee Update operator name (#58)
6ea6de1ef891eddfca0cc8ea54923356211c026f Use Patch to add finalizer (#57)
04ce97102981f63f3a58ee0675a1e3b54cbe6cb4 reduce reconcile time (#56)
cd0568009f32a7a8bd1d19c83fc707524cd92620 Remove imagePullSecret from klusterlet (#55)
fa0a3fc815cf17f8d10434314184b4c599a4684f update hive api (#54)
803564b2fed4031656a4bc2a0532655d8f4d67a9 Add CSR delete/generic predicate (#53)
dac8750c3a8e9a716dd349b0d424e81cb644d43b Merge pull request #52 from itdove/curator_pod
e007a2cf5d2cf1046eec5b899f22f6ff179d0aae Do not delete ns with non curator pod
86692a1118dbe62ab337af512d68fb12fdc093a6 Add MAX_CONCURRENT_RECONCILES (#48)
3f21ba2179a88c1953679f7413466fc69dc402b4 Rollback v1 (#51)
6d9ab6562748f26fccff6e2fe30392547558ff0c put v1 in the crds.yaml (#50)
29f2162aea0ffee1dbd7854087cf8cd13930f755 Add node permission in for klusterlet role (#49)
aac576a3a875457051e6c5971021842add3e6ae4 Upgrade to go1.16 (#47)
25f9330e8a7665f2eb806792d6f6b55d81acf07d Add management workload annotations (#46)
47526c7bd83900d4b7e48f62b612ead77896c1df Use latest applier (#44)
0190b8711cc18a9aff5a2f0a7ef10fc14cb26ce3 Upgrade the hive api (#43)
db26ab1550cc739e2816ac8fc0020c95718bbed6 Fix unit-test self-import and add extra unit-tests (#42)
1ad4efee7053ae3ae54f65767c20cd2545b00d26 Add commit-msg hook (#41)
0d82f933f4568f73f03d4c467ae5ad809d5d21f3 Fix kubectl versioning (#40)
e063bc24b1f3b970f016bb4afa2648167b282b36 Port from apiext v1beta1 to v1 (#34)
bad0540a58707413393c21af39d8444f005cd168 add community deploy (#39)
fafcf26839c71e0249fb8567e8030f018d32b80f update base docker image (#38)
9d4217aadcd12910ccf808c999c835fa3866a49a Optimize processing if cd not yet installed (#37)
c38a86cc8954e0f7b39c225a29a1bfebc6219120 fix list mw with namespace (#36)
f9bd2defd1523343d665239904b44712882a6c8a Fix func tests rbac/err if failed to set mc cond (#35)
4bad4bc70b3859d9c678b9ad5e3f16b6cf3e2120 Add check if pods in ns before delete (#33)
02e053e52c9ec0e3f678da367caa090abdd65a12 Add comment on contributing + conduct (#32)
f919dcff37be79b37d0c2e69b48dfc23b194b585 Quotes for name and namespace (#31)
fd8092850988aedfe110d76a1ba3b36768498148 Delete syncset (#30)
ede34838c7b4d109c9b4365365fe6f58cd9170f0 Add finlizer on clusterDeployment to fix BM (#29)
24efb96f7b1831ab600fa09d00addcc6a2cf28cf Remove SyncSet in favor of Applier (#28)
278f396ed33aff9781e7eacaa7bc010fe40498d9 remove dockerfile.prow (#27)
6ca3b6c63bd1825bee3f75c031617ca1d23d9182 Add check-copyright (#26)
d1639a1900951afd26953fd2766d67d8e3fdff21 Create functional-tests.yml (#24)
1427744cfcdc8893b9b783ee9596029c1036f344 Update README.md (#23)
09e2ece339650791fa04e6898733a7c7693c8ece Fix auto-import-secret deletion (#22)
e323ba0210a4f7d32010d52212b8849a781cebe8 fix lint with new base image (#21)
f4ad3bcf80d8d8930519c22a43fa4b69eb4c54b6 fix lint issues (#19)
25b426368cbc860d6250a09a13fd08f2937a4c1c Update managedcluster_auto_import.md (#18)
046981aa32afc67204eea3d02c9d97701422a781 fix copyright order in some scripts (#17)
9e6265540f91ba89f38a92df6de5b3b5eac022b0 cleanup readme & makefile (#16)
b6b2e7f53d4e9fd692f2390039777fb077d819f3 restore dockerfiles (#15)
821bcfdbd7281b8cf37327f86016659709b30de9 update copyright (#14)
943e085668daaaefc2fc5ef80ec13f1f4a74811a Auto import pr (#13)
d706db929afc736abbdc7104385a698511ee3587 Add coverage (#12)
6d576f454e73b75cad427cdc0676c2b9a963b3db Fix lint (#11)
6b3284f132adae3f4abbd0d1c69d4ee933abd333 remove vendor build harness (#10)
9b7d79ba9bb2a2f769c6f4c0cbe1dd0a21f78b94 Update copyright (#8)
96679ebf1795f29024f42c01ff588bc5d8ca4b54 merge prow updates (#6)
af6b86d895d2b36953e59bf87944326e0028da22 Merge pull request #3 from open-cluster-management/fix-owner-file
f358e15589b3db654d0965e8d8d718c725710601 Update OWNERS
8f2e8d468114ded0c8c2330cf099bea3761b9806 Merge pull request #2 from open-cluster-management/fix-makefile
7a6ab67d6d59553f62b5c1f30061357faf665076 remove copyright and update dependencies
049ad3844593ccd30b6e774fc789fdc680ecc152 Merge pull request #1 from open-cluster-management/update-files
440e497c3d8f2356d575d6fafd175d3ba4f74135 add contributing, security and license files
f0b405c45473c77d8272f251c05427e5b251edd6 add roks support (#187)
55e59b543fb76b349df1ec7fbb240bb97167e006 Fix copyright-check.sh (#186)
ffe9b3335bdb08acb4d920047a2419fd5d14dc9c Remove e2e tests, check copyright (#185)
1d4b52da6357b4c7e90bf6333702cc93871d8a29 Merge pull request #184 from open-cluster-management/klusterlet-degredation-fix
acfe62f9504d78ceae850ae840e8b5c2f9666d2b Merge branch 'master' into klusterlet-degredation-fix
c18981fb9f0904613aba3e01256b05b6ad95c230 removing resource specification from bootstrap
e4da77ab2b803aa285f39374ccb7c5fcbd23a9c3 Add new rbac rules for klusterlet (#179)
cedf50639198d628b8e05b91c96f49a301431223 Merge branch 'master' into klusterlet-degredation-fix
7e8820b458d38610b50418ff9ed3c564f33df658 fix
4983c72f0e69e5fd2295a024dbb4cc84c581eb1f remove manager from test (#183)
836e0a8c14b8885d10ec969108f09616e1337094 Improve test coverage (#181)
24966c80dd0ddc449324a1bb0c3ba736c1f7718b Add unit-tests/remove packages (#180)
05fda426c0ebc0d4e39a3b5068dc8704e95e78e9 update readme to trigger build (#177)
c13d97b430b05494d4c6e3f6cccacf563bbbc3b7 add secret non cache get (#171)
50226723641ad5e6fcc80b852c4fae62855a06a1 update to 2.2.0 (#168)
a839a69dbb1e22d148dd09be3edf71525eaf5e8c Add label "name" if needed (#167)
b5502338f43d99a7185e36b82565fc6a2afac023 Move AWS secret to coverage ns (#165)
3e18a2cda3bffdc4ff94ad90b073b8fe4258e8b1 fix operator-sdk missing error in travis (#160)
eeda3eeffbedc1b93e04928663d6213dbc6c1e22 Use REST API in cover for k8s and aws (#164)
60775554c35d7525989be82d0d1cb78b58586040 Optimize coverage image size (#163)
8f358f7589c17ed6ca8616d858b4f4aa7f93a540 Add label in NS (#162)
90e5c68959d6b98a4543bae9bc41a8d4d3f4e29e devendorize (#161)
062874e6339cfcd383a72bdcf676c34d62271dbb fix vbh when in travis (#159)
df115a8a2c4d8859de676df757ddaa882230fe1d Enable code coverage (#157)
f2a9a61c56312f8820ea7984daddd704321d005e Never update the SA (#156)
5178a49ab8b2075dab5b1b72577737631e86047f Add servemetric back (#154)
4441272a8e09850da9014855a3b2485aed0da574 Upgrade library go and add predicate (#153)
86a7584861834b59eafbc6553b927a6885852747 Self managed (#151)
e9232339132e14afba1f28f4b2e55592901d8094 Fix vulnaribility issue #4416 (#150)
472ff823d73c97d1dc6571afe8dfec1a33434c5d Disable leader when not running on cluster (#149)
ad81bf4f13a5731e6b2bbb21b6616d9ec4a636ba Upgrade to k8s 1.18 (#148)
2d2ab31480e4a70c297047ce028b1f3c1c3736c5 apiserver custom CA cert support (#147)
a759bdeb5368e686c94e99a66e7723c47b117290 Remove type meta (#145)
5a65d53c78d66119844da07c0a25bc66186015c3 New create e2e tests (#142)
527bebfab5c79761d918d0191a0a18bf2a17b8fd Update cluster_role.yaml (#143)
59435867865a6df10df8b83ad253982d3ec58490 Complete exclude imagepullsecret (#138)
1176b61ccb93fd5d7ae097570495b561bf409396 update to 2.1 (#136)
0bad06e510c1219a9dd0cf86d30ae5bc1e4a8902 Fix pull secret name in klusterlet and add to sa (#134)
c9202eae405f38b54d99a04368d5fd1b55b0c5c7 Revert "fix image pull secret (#130)" (#133)
199e6bed3d00e8d2b1da60afe31fbd4965d96363 fix image pull secret (#130)
3efe6c3b5a13f20de6e528b88126736dfd610707 update docs (#129)
1be907687bb8c7a9b32511ad22f3fe78bfe1e97c Update detatch_managed_cluster.md (#128)
cf38ee61f2bc3ad8d4b2ce4e83a860d3061d64d8 fix typo in klusterlet clusterrole (#126)
253ba85f36e4688aa464c4b8e5f3cd4bd8c2ca79 add doc for manual import of managedcluster (#116)
59366d93faefbdeda2f689eb23b1adbdbea90b3b add aggregate clusterrole to let work-agent modify klusterlet (#124)
614c53519de0e4a4dbe035b17e01e97aa7d0fdf3 Merge pull request #123 from open-cluster-management/ff-2.1
291f40ae498e003d516ae18389d3a98cf3506977 Update for release 2.1
111247389cc782cee121157c77220e3faa93de27 fix functional test and code smell (#122)
01a9720e8c2ab5eb22bb161680ba4dfb028aca92 fix image build script (#121)
699669c692783b5e7c01570f7d0881b3d03978ae Implement Delete/Detach (#120)
83764a169e3ac1777e36ed251ee3091c012f332f Add Auto-csr-Approve (#117)
2fe59f34b7f92980b7745d5ae0f142fd1f04eb5d ManagedCluster + e2e (#111)
46a2b85657ab9fc032c62ed668c2af45f33a7cf9 Add microdnf update (#106)
3a67a08b0c3c1ce63056eb49d5e799e1a1c71d86 chage back image name to endpoint-operator (#108)
01a5db23bf87ba2fade4fd1cd555ec7bf2f35a9b Rename EndpointConfig->KlusterletConfig, Endpoint->Klusterlet and component APIs (#99)
a87e57dd3e1c0d9210ac5d3544b93aa0a4524720 remove service registry (#100)
dfd1f7c3c7175ab53b13e5d9aa6f19e7fe01377f Merge pull request #101 from open-cluster-management/create-2.0-release
15db92d8b06d237d82ddd67a74df239db1f1355b Merge branch 'master' into create-2.0-release
12ff0641605c5b80c5ead7d97295deb5bc6917f2 Add coverage (#102)
1ca6494b9e23992b56d6d890082958e43b216c7f Merge branch 'master' into create-2.0-release
ba2a21c57f4d91d06fdbb4de23bfbcdfc9a04eaa update version.go to 2.0.0
aa8c3befc19f8ed0b80c5697b75a2abd17324a01 Fast-forward to release-2.0 (#98)
a8d9ad2dcb071f46dd2d7d96b21299c55fde02c6 update COMPONENT_VERSION to 2.0.0
8bbd51ee838c6f0bb1410ed3fdd52e8697513f63 Fast-forward to release-2.0
25accd4ecf2962629241a4095ab979651aec1c6b Vendorize (#49)
4896ffa1e1acc7f1ca180cfadebba1b7f0a11da1 Upstream build (#96)
bc1914e6d6895ad18ef1fff286954ec16fc06ca3 update endpoint operator (#93)
ca8bfa37b061f89848e8c87f6b5a28e1dcaf4b1d fix edge case where default image repository is empty (#94)
a5266496c5964ada117d3514f986b63b1b065df5 support ENDPOINT_OPERATOR_IMAGE (#91)
511e285e03d8a096a037d735dec577cebafb72e7 Update test_endpoint_config.yaml (#90)
afa173cb40c04478786341a580b3565420b0aa40 add tag & sha tests (#89)
1cc3bb9bdd81e3f4f301cdf5595d63b3951d4b01 add sha for endpoint-operator deployment (#87)
f081df6f4d15f233a70562820233d4e480f55fcf add unit tests for clusterregistry-controller, clusterregistry delete and endpoint update(#86)
fc41c9c254d2158d5315c07c1d36233608fe07e8 Merge pull request #83 from open-cluster-management/smeduri-copyright-checks
7502092b81d076b8b0bc720f66c53527f13f9f0e Merge branch 'master' into smeduri-copyright-checks
de17c6c633ec9fde3c04424ea0b2a653a92ebcdc Merge pull request #85 from open-cluster-management/itdove_remove_kubectl_new_endpoint_operator
d9f58698514914e4de7f20a749dd3403413be950 move copyright-check to check stage
2ed7809f5d9ad25a21d9e6775a4e95e41d827b3d Update go mod with last endpoint-op
2209096e956037fbf465d63d6397f7f4b5f028eb move copyright-check to build target
4917efae96a9fa374305c7a43b2c4ea61fef3dde add copyright-check to unit tests
050d559f5d3a9e37c6988d6ce7cbba714a2ac0f8 Add copyright checks, update copyrights
5dad7b56f01ff0ec10f671af41292ef0287adcbb improve functional tests (#82)
511ffbcc70751a36cb05afa6419d853e3edd39b1 Add functional tests (#78)
c8ad39fbeeb4521e1f1b821e7b5236fd0564ea5d update endpoint-operator in go.mod (#81)
06133521b573daccc8e868c31aac72fb39cea07d add endpoint-crd in import secret (#79)
f1d8cebe8a5f4313c122fa503e8b6a15668b205a Update endpoint on managed cluster (#75)
6e6f51e2651598a5364038b00eb5add483008c68 Fix selector syncset (#76)
574a83057568366106f79dcef623beb33234a610 update endpoint-operator (#77)
373b43eecc9a16d1a93a085f07e7fba27ae7ced6 add ownerReference to syncset, importsecret, and endpointconfig (#72)
ed186c21274b3d0adc7169292fd71934b73833bf update endpoint-operator module (#74)
dfe40064e431abd3d116a41df3434fd19869697b Merge pull request #73 from open-cluster-management/rj_g304
359dadad9823f9e68c81f8295095e18050539336 #982
21c97bb8438c0b7ffcd807635fb42be821eee69d fix adding finalizer to cluster resource (#71)
6331ff34d79bb60137cdbd9972dc6889d069f9de Update test_cluster.yaml (#67)
f8986f345f84eb39a1539051a8789364adced43c requeue on fail syncset creation (#69)
00a65eebd7b13790d0ba87375e0fc6d709f0c141 fix make run (#70)
5424cb527315720537a75be9b974fdebfe9f34cf add default values for delete (#68)
6751ba83443484b3725a49a8647c2072806a9047 Update syncset when endpointconfig got modified (#62)
d0d477e3c51eebc88cf053f396639208136ad237 clusterdeployment controller should not create clusterregistry resource (#66)
76b129e53ce721bf9630b001139be35cc249252d Merge pull request #65 from open-cluster-management/move_sec_scan
0da457f49c29f183b1cbbbf3961048e109344bdc Run make security/scans only in .travis.yml
78ba9ffdd186287c94ba17101c001108e16f9029 Merge pull request #63 from open-cluster-management/rj_enable_scan
1e8f2e50b988b37865343b196f6898dfd8b1961a Update .travis.yml
e680697a3ce9862fdfd6ff0dddac9b94a15fe0ea adopt build-harness release-ff (#57)
098c38720a5ed443c2bcee77248574ea13749cce restore makefile
c0c65fc450855184c6b167292a503c08891beaa5 update order
5fdf925031ab13cf78981b11a3e0c515c393006b update comment
6b50e6112c2b0f61a6db9a3a05e5aaca2a0b0d3e add default imagePullSecret & defalut imageRegistry
7499ecb799bf99fe24b76624a83ce9c789331ade Merge pull request #58 from open-cluster-management/rj_run_sonar_scan
cb8779e233321a288168f7b277ed82b7f4e7c7fe Update .travis.yml
a7f145615cd9cca16e5ced6be1be9e1b808168ac Merge pull request #54 from open-cluster-management/default-pull-secret-and-registry
889a548738e3f6ea028aa698f536755de8a50134 add default DEFAULT_IMAGE_PULL_SECRET and DEFAULT_IMAGE_REGISTRY env variable support
f2d0ec88b751b0b1daf0bac3256766295d3e7c09 Fix import object (#47)
de05fdeb08af3d914ca6c177e18559d027b7ad3f Update Readme (#45)
223192e5144862b5735ec33e4834b98fd97085b3 Use latest endpoint-operator
2c7be032c7761f01657ce8d269d4cd0445941bdf add howtos toc
73e4153cd1b225cd78b124f923af9737822ef13c Merge pull request #33 from open-cluster-management/rj_sonarcloud
9a101b3541535da40a0b039f82014da625c13ae1 Update .travis.yml
76ca28fee3c8e11e7c9125e5bedffc927091dd70 Update .travis.yml
89eae73884d45dfb1d5f649ce7540fb327daca0d Unit test without sonar
505cc73b781cb025e8869010667614a656f7ff54 Merge branch 'master' into rj_sonarcloud
7c9dde0dace54e072d16029b94323fed47af07a2 fix unit tests (#41)
6102869961eb37f83c795d1e218e5a6d1d39bc77 Merge branch 'master' into rj_sonarcloud
f6d55519811234d4c8b65a5a6c28b8f9baba3e03 Replace openshift/api with real semversion (#16) (#39)
75e14745fac36c6b39657c3c28dc44da16d86707 Update .travis.yml
436a57e20dc33912529c9c42b58a3786701d27e1 sonar: removing debugging
62567785385c7711631dd8bf1348a77beb9d62e1 sonar: debugging sonar scanner
e02828a41bbaa5938cc2e2de1b6053c3ed8c52d1 Merge branch 'master' into rj_sonarcloud
ce5520cd9bbe8556b7e502c126974ce1096b3949 Update cluster_manual_import.md (#32)
e06d800bc12aba4904942ebcd0a04294908882e0 Onboard sonarcloud
9231801787111a04889e03efd7c3a7b28ab54ce8 remove .EXPORT_ALL_VARIABLES and use export (#31)
55ee9403c7ab59be4357982cb4a2489f07c03aa1 assume postfix always come with a - (#30)
ff32b4669d2315a8f7de6b2758a217cf788bc7fa Update test endpoint config yaml (#24)
9d7d2377f23495d448c2cce8c6ee6b1fdd9bbc1c Revert "Merge branch 'release-1.0.0' into master"
1620be8acf03746e865589ab367aeb0038490b96 Merge branch 'release-1.0.0' into master
ab821b3c65a87422f29b784749f1f5bd382b27f6 Revert "merge from master (#23)"
cf602c680e426c28785fac929830babc33064bc4 merge from master (#23)
2d3b24e9901c091c272030ed56a94d8dd19def7a Add links to manual import doc (#20)
efb318696120671212b7c4c6b5999cba96b980bf merge from master to release (#22)
92af9d01e1fa27c2c03a0255073dbf1b57ca0df4 update image name and operator name (#21)
90f229fb3da202cf04e776df9e2c41366aa8adf2 Add tag postfix (#19)
e2e69c06410d24d5d9ed954fae72e3c41a96256a Add security scans during travis build stage
7feddc127c8a71243202756627e43c10b90619c9 Bump ubi image to newer ubi8
80d99592b174a5b32aa7dde4982bd72fdeeef81a Make common travis before script
15ebbd11353307c227fe268bc1c7b7e4dce59f53 Make common travis before script
22b773a344c6130508c03268ced51d689a0b8852 Switch to new repo and pipeline
bbcd51ab8cf2315be3d5b6b96f9bfa4bc7909f7a update operator version to 0.15.1 and delete endpoint api
84d75909935d06d18d27deb4bc0e629371d0b9d2 remove cm cluster-info and read config from infrastructure
c0b5f1d8ee239749a5651adda638dcb92e38e2a9 Had to fix the tests because not correct
a6fe6a2255ad9e7910ab2e8759a4c9e455a065b9 Manage reconcile error and add License in zz file
13480d5d7908a461bd7de9c13b3991ac2af7e835 update controll version to 0.3.0 and update endpoint on managed cluster * use apireader to read resourceview and changed import for log as it is deprecated * added unit test for getresourceview * add unit test for createresourceView * change multicloud-operators-foundation version to use latest * change controller logic * if cluster is being deleted, don't update endpoint
392202f0061ef3c0a4789587c202976b502b45e4 delete endpointconfig when cluster is deleted (#41)
897af92992521581338a60f0af32b3b07eb265a1 bootstrap clusterregistry unittest (#42)
d6b9817163a376d37f7483d5f011ace850d8e09c clusterregistry cluster deletion (#27)
54a2d807e8e5db2df2f384c995d7309b8e4d45da Check if CRD are installed for launching the ctl (#35)
43b4f1ed9dcbf82e17e43a3c74609bca9d9eb705 adding design documentation for the controllers (#33)
95b7bdd339d198863ca5da69540c1e570e46f266 add cluster registry unit test (#29)
bb752c626d0c586dd9a3047b09b1b430b23c87ea add endpointconfig controller to generate import manifest secret (#20)
7c4b1a95ae3fcffdbce61f1ba2134112a6743c0b fix PROW build issues (#23)
77896079963d81a870be1a64b9e829fd15995f1f .gitignore, check dir, install hooks, add user_setup (#8)
f22a08cb80e6b252cfd27d3fe116ee7cbf3157d9 Refactor clusterdeployment controller (#7)
41721c42f11c4e39e70c3cc5c8777f29efd782df create clusterregistry.cluster even if EndpoinfConfig doesn't exist (#6)
3e6089f27b974957ff4a73b387807c91df6a0d10 add selector syncset creation (#5)
db942c5121f12103edf7bb66926d5a8a3cbdaba1 Deployment automation (#4)
3564716dcd116f66fd5e6977b18912d26ae02429 switch cluster-controller module to this repo (#3)
e664e377deae5cb7edbdcf6e4831091470ada963 initial commit, moving from ibm GitHub (#2)
7eaa8c4c7eef3a29166957d4929832afab148bed Create OWNERS
239f9ea85e644c8cfea1e5c7e2508e43b5235d65 Initial commit
```

Status: Synced commits but not tags
