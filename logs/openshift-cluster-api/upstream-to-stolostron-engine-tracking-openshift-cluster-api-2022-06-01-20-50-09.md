## Fast foarding of openshift/cluster-api into stolostron-engine/tracking-openshift-cluster-api.

## Status Summary:

release-1.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-1.0 -> backplane-2.0:

New commits (first branch sync):

```
e09ed61cc9ba8bd37b0760291c833b4da744a985 Merge pull request #5402 from vincepri/update-deps100
ad95a968c951da1b5aa81000ee62736714376308 Merge pull request #5401 from sbueringer/pr-fix-book-make-serve
4305dcccd3092665e8a4074b64ef82d3c3b20183 Update dependencies for v1.0.0 release
aee6dc9217f0ba29a3eefad2886e3596abeb953d book: fix make serve on MacOS
be7f24682c2361d951cebd07849eed7cca8fd132 Merge pull request #5388 from enxebre/leader-election-resource-lock
00d00505d9fa3e47243bd97789ea31e415442c9f Default LeaderElectionResourceLock to leases
ffb41d53a6e7c25bfe8f08acd6104a7501451ae4 Merge pull request #5395 from randomvariable/e2e-upgrade-doc
18ecf48ff1ca739b54d0eafeb47263f5a1a24e43 Merge pull request #5364 from ykakarap/version-compare-utils
ae6aef37dc5afecad649f74be00bbdf1ae75d974 Clusterctl Upgrade Spec: Add details on how to use it
33e9f42e6daa0638efa6ceafab321c5a46802aed Merge pull request #5391 from sbueringer/pr-clustertoobjectsmapper-use-objectlist
62cebab94dffbb07e45180e4ca89ecdd5041e0df ClusterToObjectsMapper: replace runtime.Object parameter with client.ObjectList
0cec4402f19dc7afe0ab1111347b0bb92867e8fa Merge pull request #5381 from fabriziopandini/KCP-reset-ownerremediated
e9f50000b88991803012f44c9a260f477d66d09c Merge pull request #5387 from ykakarap/certificate-empty-issuer
e08fca1ac775492c43d1ccbbc62045a018114d7a add organizations to certificates
59968dba18bfc9cf349b3a6fc82d010ae182267e Merge pull request #5374 from killianmuldoon/pr-clusterclass-quickstart-guide
f4380fc82fa2eef5119967d9bfea9d428e103e76 add version.Compare with CompareOptions
0a1f790464ca2cf1f2029656774df387c1456644 Merge pull request #5377 from randomvariable/moar-capi-upgrade-variables
233f0703eafb065257922e3aeda4ddf4242c8ed8 Add clusterclass quickstart guide
613bf911c7da950a6ba2cc8c9acf7bb86981de3a Merge pull request #5384 from sbueringer/pr-fix-developer-doc
e1de82d4c9de0fd3758bd204964ae592be21d745 Fix make commands in clusterctl for developers doc
73e8d96db3b7d573d8e5f1fc368689770a6603db KCP should cleanup OwnerRemediated condition if the machine goes back to healthy
7ce48aed2626ebb59fc48e117d7076439f5f44a2 Merge pull request #5386 from sbueringer/pr-clusterctl-upgrade-flag-validation
dab6d5d305fe2f718f90dd6477de65d8666d9ab5 clusterctl upgrade: enforce that --contract or provider flags have to be set
d939d439a169f2d0a7293583fb491b19fc3e55f9 Allow passing in provider contract and clusterctl binary in the clusterctl upgrade spec
e25f0e3ec8c45af3ec2fe84cf83efa03c7d5c579 Merge pull request #5382 from sbueringer/pr-upgrade-cr-to-0.10.2
66ef1bbc5a8c94f056f85b721ee5565c3c768c4a Upgrade to controller-runtime v0.10.2
6ab9c28c36dc6fa52b97f6f2cd645acf48ec2906 Merge pull request #5372 from sbueringer/pr-fix-certificate-target-namespace
1bf3a101cf9ad77be29e5c002a20b9e6693a2650 clusterctl: fix Certificate target namespace
cab465d98a13f8fc813880dbc87668b80097a7bd Merge pull request #5358 from fiunchinho/filter-watchers
bd674685d15e94d97565c42aa89887d88202c5ab Merge pull request #5376 from knabben/main
c02bd6e9a18605d872e26ee3736158c7fed8665d Redirect on curl k8s stable version and kustomize install
286a22fbbefb8c8cfc4a9a260c747fafa65d40c1 Merge pull request #5366 from killianmuldoon/pr-update-conversion-docs
bbc8384de05e417e90e2e970e3aec2bef4b7f11b Add clusterclass contract changes to v1alpha3-v1alpha4 conversion guide
101b405b3a69d197fe05bd2e76389c0376167ae2 :bug: Use the watch filter label when watching resources
119feab01c0ce84ba232a8982ccf2fa1956b9c71 Merge pull request #5365 from sbueringer/pr-propagate-annotations-to-bootstrap
21e7983a7735f33fae8b064abd030513d7b2e4f9 Propagate MS.spec.template.annotations annotations to bootstrap config
13faadfd59b2b744f45b51df7fcd5492894916e8 Merge pull request #5362 from enxebre/api-conventions
0be85a7542840390bc6406ca01bccc9c26e0eb82 Add required/default case to API conventions
6d1f69218935b43b4783758c579e96c7072a6803 Merge pull request #5360 from sbueringer/pr-fix-capd-conversion
0b49076dea24d0274fc9b6a69c2e6dc56043f134 Fix CAPD v1alpha3=>v1beta1 conversion
8bbfff6a809f7ea0d3fbdfd4586ab0e82e080d8a Merge pull request #5354 from sbueringer/pr-fix-clusterctl-v1alpha3-ugprade
b533485f33085ed5fd71f099a6b3fef9e7646da4 clusterctl upgrade: ensure old controllers are gone before installing the new ones
573f005559b452813e4dd8175a791dc2d1b143ed Merge pull request #5334 from budhirajamadhav/addClusterName
3d6d31413de9143d0277dc588918ab13c3b70f53 Add cluster name on printer column on non core types
fc480622663ae4117ad94a912c51e31df78591db Merge pull request #5353 from vincepri/kcp-updated-machines-total
1f8fb792be33358ec12199d30c0cfcfbfe12a759 KubeadmControlPlane status.updated should be calculated appropriately
45ad7d1074d8497e47106b2eb927290eee7f23a2 Merge pull request #5344 from fabriziopandini/rename-EtcdClusterHealthyCondition
c5c07f5b907e56d423b23bed47068abbb9b225d0 Rename EtcdClusterHealthyCondition
70d1bda9d2ea0b7d4e5ce7af9ce159d0f531b461 Merge pull request #5343 from fabriziopandini/fix-topology-controller-rbac
1ee02012a43cd34d90a408af2e91f447d8bcbcf8 Add permission for changing ClusterClass to topology controller
304f013f58800aa939ac7b2102de08dd6c3e0416 Merge pull request #5304 from sbueringer/pr-api-conventions
c8321904a29dcb3983f720fa1ab83b049351532b Merge pull request #5335 from CecileRobertMichon/main-book-link
a0e7738b7cedd8d35991bde7f49ddc7b1f7e803c Update main branch book link
41caccd8e700320d76e35cd1a37bc573c113f5b7 Merge pull request #5331 from CecileRobertMichon/netlify-main
f70fd502a6848d84eaaad29792adbfc8bd0956d7 Update netlify config after default branch rename
e514ef76ab07ddeb39b4dace747626fad6f9c65b Merge pull request #5299 from ggpaue/update-cert-manager-1.5.1
14f62b9cc0a84a02053f74683954ccf55d3d2579 Merge pull request #5328 from sbueringer/pr-improve-e2e-clusterctl-logging
075983907e7b76dbe6967617c5ac1feaa310a108 e2e-test: improve error logging for clusterctl init/upgrade with binary
dded2c0480e2e6a7153cc3ba5632b55c9746e072 Merge pull request #5305 from sbueringer/pr-fix-optional-omitempty-fields
ce2bfe271e60add8b5865b37411481a636514681 Merge pull request #5326 from Iceber/fix-link
b75062c95d283880964c0a13482bd82b7523814d docs: fix the broken link in introduction
2d07978ac3540df3093208814dc1fcc8b4d0a3ab Merge pull request #5321 from fabriziopandini/clusterctl-enforce-provider-order
1e170f60fbc94b05d1ed07fe1006c437c7f44c2c Clusterctl enforce provider order during init and upgrade
37026449b8a5c78d14152b886d47a1dddb744c6b Merge pull request #5315 from fabriziopandini/remove-machine.status.version
07c0a4809361927b15cde2747b34142b7c7ead15 Add omitempty to +optional fields, drop omitempty for some status fields
f2cc2113db1e53e6a719cee76ab85a6ae58028c7 Merge pull request #5317 from killianmuldoon/docs/update-errors-doc
235cfbc54e80a3969c0a4dfd2fd4d3ef7db57e14 Merge pull request #5312 from sbueringer/pr-more-renames
abd6f017b65e19a77c0ae34b93aacec652176dd2 Merge pull request #5301 from anusha94/add-missing-optional-tag
aed5ec9b736b01351cb3eaec3ff25891a3970b4e Merge pull request #5278 from fabriziopandini/update-jobs-documentation
612a583d820a4e09601cc7a6fc7cfe4e54159fc1 Merge pull request #5310 from killianmuldoon/docs/update-tilt-kind-setup
351a79317ed8260e86f94525ef44d98bee8f15d8 Merge pull request #5313 from sbueringer/pr-fix-1-22-latest-e2e-test
3b7701beac49025c7beffa62f0b87680ba00a011 Remove machine.status.version
061e6001344afcb0a464191beb6aeb51267abb1d Update errors doc to reflect intended usage
5a1389e4eb45ab94a02c20b3d04a627ebb43b320 Update book to use Kind script for Tilt setup
40c9b78fa322be1950b5c1fd57cafb341d5b326f Fix 1.22=>latest upgrade e2e test
ec30875d5932d7cc9dd0f3284370f3d3bc6ddde1 Change a few more references from master branch to main branch
f596cbde45a7615cb596e6412380e980a099436e Merge pull request #5293 from vincepri/conversion-linter
43fb0190e4f3046accfe7a90f11ee79a149b6a86 review findings
3da7a18b40810cd8a33975e81c89978c6c8beedc Merge pull request #5288 from killianmuldoon/pr-delete-deprecated
5efb7d70477c9d010e420a5bca7a62405ab088b3 Merge pull request #5232 from killianmuldoon/test/add-kind-setup
9b21c4fc22debc5aae27de298b5e826b8b6614bf :seedling: Add conversion-verifier to always verify conversion code
c3351784ff9095fd1448d7491b7372b5098bf4f7 Upgrade cert-manager to 1.5.3
5c7d80d26b2da9bacf30537164d94c3098b55539 Merge pull request #5259 from killianmuldoon/pr-object-matcher
6ce891341e27cfa0c09bbc57452eebde4196b9bf Add composable matchers to internal/testtypes
f4410f13ac3499fb0cbc0b029ae79adde0dd7ded Merge pull request #5267 from sbueringer/pr-add-machinepool-conversion
617a8acc2a12dface40619b921ea14869244a221 review findings
4a68ee70aeb9fc4f5bdfa3bdc60ba2b36a54646a review findings
3f54f62a6c6544705b8e765712fead7ab4831643 Add docs on removed items
934bc9e625ad05a8c321398166e9a5ab1587385e review findings
e00217f47c8854f8a87ebd5b259cc625669eba8a Merge pull request #5292 from sbueringer/pr-consistent-crd-columns
e6062a894b725826ec6f59e5532e575288dc4cf8 Merge pull request #5303 from fabriziopandini/make-condition.lastTransitionTime-required
8f28814c8614fcd565b48495508933024e818704 update deprecated types in line with PR comments
8cd0d3bcea6f305ee9a978a5e6ad4ec343807923 un-delete deprecations in api core types
9fdf087e91f6b4ffb5daf5366b0b1927a884d7a9 Remove deprecated items from the codebase for v1beta1
edbbe876ea72afbcbc2dae85c8f5e109bc9cd738 Merge pull request #5297 from enxebre/md-internal-main
9377ba2a19ea69f716f88689f6a550698d4da4b2 make condition.lastTransitionTime required
1e5ca192758f28987c7d6b761fc29b2cdfd9e628 Merge pull request #5302 from fabriziopandini/remove-required-marker
3b96e1931d70f1547d30fae333eb81d0dd2aea58 Add API conventions
348a94b49cde246d2c612c60717eb1989530ea2c remove required marker
769f0f9108c4289c4e99ac1c2e2e0987fa55faf9 Add missing optional tag to omitempty fields
7f8c8aa1a58221a070f74bdac84c2044d9f1dfb7 Move mdutil into an internal package
4860222a821b02011a3a2c0051e62332837764cb Merge pull request #5276 from CecileRobertMichon/main-branch-docs
c317301ba539df555514093f103940cf1c9579c5 Merge pull request #5275 from CecileRobertMichon/branch-rename-prep
b2765128816d3a38df6f85c03407e08b92b5c7c6 Add MachinePool conversion
58905fb5140a7844c3e24aa70d255fb8f9d0c491 Merge pull request #5296 from killianmuldoon/fix/duplicate-imports
0e2f09d1c4f3caba5d45e8b02295c6c4d672935d Remove duplicated import statements
84b9cfdb4f4a9f3ac7d05a433a1f4f0d9e173bdf Merge pull request #5280 from sbueringer/pr-add-dockermachinepool-conversion
c2cca8155a82766d891a74a842a6c98f8f6bc34b Merge pull request #5286 from killianmuldoon/pr-add-clusterresourceset-conversion
5330150b73cf5059bcd3f7303667af7662c77390 Merge pull request #5271 from fabriziopandini/clusterctl-support-v1alpha3-v1beta1-upgrades
3a975a3d839b5b224061a72ac2c6a10a5d75d30b Merge pull request #5217 from fabriziopandini/group-resources-in-tilt
e8591e4f8691093bbde49bcc75576123de581253 Ensure CRD columns and their order are consistent
7f2304d1d2ab740de559a739ed2192b2f8872116 Add script to install Kind for testing with CAPD
761ce3ff86c7d5270125f491e753205ccb13f4a2 Add DockerMachinePool conversion
712b195313f048ce2a668d31eda184a72a976ca2 Merge pull request #5285 from sbueringer/pr-add-list-conversions
df6d02e89afa177aeecac63a1f72782bcda9db58 update jobs documentation
a22f51483483ca6fd3871f4985b35dce2de44fb7 group resources in tilt
91cc8654d149c81c82dc53926a81ee5fbcb384ba Merge pull request #5044 from killianmuldoon/fix/clusterctl-upgrade-delete-inventory
445cdc3387f80c02baf271277b8bd90e312b2942 Merge pull request #5274 from ykakarap/clusterclass_liveclient_list_machinedeployments
23c412ddb03e0ba6d3f9aad7aff994bb13dde934 clusterclass: user live client to list machine deployments
c6ea715ecab281642af87e2573d93fadf3415c1d Merge pull request #5249 from sbueringer/pr-upgrade-controller-runtime
3849048e5b74096e41528f11a94b5427ec11ee90 Add conversion webhook for ClusterResourceSet and ClusterResourceSetBinding
81c140df55612bfa97705322222b639ad377b725 Merge pull request #5270 from ykakarap/git-version-lookup-fix
6b88941d401d5542c0212ff6518d68bdf1802630 Add CAPD and KCP list conversions
106e2d6ff68ab6b797816b476176e4149624f665 Merge pull request #5273 from ykakarap/capd_conversion_tests
d54d7ead7afa9278f686d951bd87c3783f875d7d Merge pull request #5264 from sbueringer/pr-add-upgrade-doc
b9a8de8dc008facf147372c63daa5296e268c7b7 Add v1alpha4 to v1beta1 upgrade doc
89df9472d1678ed8ff59f4e124d48ad51ffd85c6 address comments and fix e2e tests
b95cebb891283b32f0052de00b8c6351163a3dd6 Change all references to master branch in docs to main branch
de3b93b97609e1321c43991d50699dc9ac0abce2 Rename default branch to main in scripts
821da3d7a5c806b13e0ae00ef282011fe6f43376 CAPD: add conversion tests for v1alpha3 and v1alpha4
2ebdffbc0f41df69d02bb4be19be61c030c7564f Merge pull request #5270 from ykakarap/git-version-lookup-fix
7e93b600f25aa517766f71e535a4070800d4c157 clusterctl support v1alpha3 to v1beta1 upgrades
e2317311a763e3777a2fb482980b932803c7c602 use only annotated tags to calculate git version
b8ad4e45cb36815a0b009b709ef3a4b29061c1bd Merge pull request #5248 from vincepri/v1beta1
fc52fe3d5cfe05d436a7d2f0ba3cf8a1399aad59 ✨ Prepare the codebase for v1beta1 types
7cd30261112bcbeacb073a89e0c7b7eefaa12812 Update Kubebuilder PROJECT files
c114880eb20caff471f6778ef22bd3dbbcef709f Update the metadata.yaml for v1.0 / v1beta1 contract :
e904a59a56be98cbaae1799492254c4200e9b99c Rev golangci-lint to v1.42.1
c55b5013fcb84841cc3705dfb250cdfd8b140447 Update test framework and e2e to support v1beta1
e482405b91f7a28bf9d18b10f9d26c2c4486ded1 Update clusterctl for v1beta1 support
65906413f83431f5a651115ca9691a998fb1c8bd Move kubeadm upstream types to upstream<suffix>
527799079d3a79883e65bc90507fcdb629c445dc Add v1beta1 to docker provider types
d2b69b17168cd9e49de11617d8c39ce719d167a5 Add v1beta1 bootstrap kubeadm types
6ed6476d5efecb8eb8b21b64f2a0496bcf7cc9af Add v1beta1 APIs to experimental types
4369793a5872d1d721d302a5d1fea78b6be113af Add v1beta1 APIs to controlplane types
61243ed8461652be80e3134afb89b5aa0c7c851f Add v1beta1 APIs to core types
53d99d849d63e2bcfdacea4869b288952e0f50a6 Update generated files
7d8e1d7d9698495d06c113eb0fe7a15ec6c52dde Update module dependencies
a3e4b37c40ef8bc8ca1748fecb9b98c88b868e1f Merge pull request #5056 from Nordix/ms-avail-condition
6a81b84eeddc9acfd88126cfdd88fc375685fada Merge pull request #5261 from killianmuldoon/docs/update-calico
b4be01a1d42aed1c02730d46fac27ad82965c49f Merge pull request #5251 from superbrothers/complete-cluster-resource
b1eb9092a9ba6d0ad3619e558b7afb03927c022e clusterctl: Add completion support for cluster resource
6d88e7564935c948912eb0502f1ca49671c5cdec Merge pull request #4980 from asalkeld/memoryReader
f40eb7abd128b1ac162107433c33762de4f9f783 Update calico version in quickstart guide
7475a6479c37da9000bdfb70b80365ec80d37fdb Add a MemoryReader for the operator to place config from a secret
5883e99d1ad9f7d6aa60a62240ff77172ed81d53 Add Conditions to MachineSet.  * MachinesCreatedCondition  * MachinesReadyCondition  * ReadyCondition  * ResizedCondition
0065d5c80a1be27e81250eae170915b88a8d53a7 Merge pull request #5247 from superbrothers/fix-dynamic-completions
cb43fc8e54f23a8e83d9e56c652b7fbca835af28 Fix a bug that completion suggestions for --namespace are not updated
59ccc97514d1ff576198e1925b8d062da6920ef3 Merge pull request #5243 from vincepri/go1168
6c9b8983814c640147cff2469e05386254a5b301 Merge pull request #5225 from fabriziopandini/clusterclass-test-cleanups
b80194fc95e47ce965abcd5798db5cabc012aa41 Merge pull request #5237 from sbueringer/pr-fix-kcp-conversion
bae26800ade39ac5d79650ba5b9e23ec2b80be8f ⚠️ Fix group issue and add age column to DockerMachinePools (#5206)
7dffa69fd454215106bcc569aab3746410fd7bd3 Merge pull request #5094 from superbrothers/dynamic-completions
861813179cb8d3a3850ef1a67193898738b03edd :seedling: Update Go to 1.16.8
4e87b5fc63ae211e6ab58d94dcb8c5858ecb9b75 Merge pull request #5242 from sbueringer/pr-improve-capd-docker-build-caching
7084de351638b42fddd0633a4669f435e9c9ec68 Add backported rolloutStrategy to KCP v1alpha3
926921f83a78f67a91bad5eab6073c7072f5d1e1 CAPD: improve image build caching
8de099515bd13045512690ceb83f6b23bf5549e0 Merge pull request #5228 from killianmuldoon/fix/clusterctl-panic
42d2371080798c33481709a80f008f62598c2bc5 Merge pull request #5241 from enxebre/remove-constants
ca7e71b1279decf20cc37715b9dace4a02f4a790 Deprecate unused MachineDeployment constants
8bb9afa38a99c75d377ede43689d504025526165 Merge pull request #5238 from sbueringer/pr-sync-v1alpha3-const
d1c7c0e43617f64d4e7bdb406d6638d902ca29b3 Add dynamic completion support for context in kubeconfig and namespace
99c64f50bc92ae754512662044b575aa78b5813b Merge pull request #5235 from ykakarap/upgrade-managed-topology-cleanup
04e1ddff7e0fbf88de47d68e58aae868bcd3008c Merge pull request #5221 from enxebre/watches-infra-cp
b0e96add95a8a9d7d4d4b83ef7e5d730bba4050e Add watches for infras and control plane in topology controller
cc9c5bcc7039c8e2b2b75ad71779df807a793a10 add missing constants of v1alpha3 package from release-0.3
c2c4da812ab51c25494409b2c19cbaee87c4b514 isScaling error handling in control plane contract
f8c3205b11c2403841c84b6f10c40e9b42d50032 Merge pull request #5178 from ykakarap/upgrade-managed-topology
9672f4a9b7f48ebbaa5a1e350dbb211db6ec3150 Small cleanups to ClusterClass tests
2b81f62ad668ddb010cb37d734ca0677c752a13c Merge pull request #5231 from anusha94/use-index-func
a24cbf2a7873883a9768cffbbba8f6179eb19142 Merge pull request #5191 from sbueringer/pr-improve-template-deletion
7f5451f27a1da1f6e1d531a53048b0f562adb80c Fix panic in clusterctl describe from nil reference
1f03aca667747a350ce1ba445bb2aac5c6306eea Use .Index func when building field.Paths
ae31c7c8fca559ff2a76d951e2d324872ab5cfdf Implement template deletion for topology-owned MD and MS
a7fa32b01dedb33a52a2def16d82118f570d5f51 Merge pull request #5223 from sbueringer/pr-fix-workload-test
b35306ccc9e9c8cb1467eaf62ba39c1f4469b22c upgrade support for managed topologies
6baf3eb05cdc8a1a2746c73c4aa7bd815ec7d72d Fix flaky TestGetWorkloadCluster test
846b09beb54ef7fb1a5e0fc1df4406354afa9691 Merge pull request #5153 from sbueringer/pr-cleanup-error-templatenamer
b7e990488511e6be73d54e6c2d32f980bb65e576 controllers/topology: cleanup error handling and templateNamer
c50aa1f673e9b3ac255416eacbe69eaaee06d3ae Merge pull request #5213 from fabriziopandini/allow-clusterclass-compatible-changes
718b43733a203fa94baece5b25d9ad50a29aec92 allow cluster class compatible changes
d56c775209fa980d4ee5799035e996c273f12de1 Merge pull request #5215 from sbueringer/pr-fix-flakey-patch-test
494b8ccf9e5da293301156968a4e655f8fff664d Merge pull request #4390 from mig4/contributing-docs-note
68e828fc2378a3e5dc61b612c0c8bc2eb7431a1c Merge pull request #5186 from detiber/e2eFlavors
18dc6507fc0fef065214aee73671a1611530d75a fix flaky TestPatchHelper tests
074c2cb334ab54e4f8ef5ddcf40a15a3aa1044a3 Merge pull request #5214 from enxebre/fix-comment
541f8665cc6ed93ade3f39ad08647d8a28253786 Fix mistaken comment
279873014151650d49da05eb5a5fa36182ae63a9 Merge pull request #5209 from anusha94/add-cluster-topology-md-label
69755eb6f0752f980a3731f497f2bbb42953a79a Merge pull request #5165 from sbueringer/pr-make-topology-controlplane-optional
e2a0b0c115220c53ac4c43c17e317d586c71e073 Merge pull request #5211 from sbueringer/pr-propagate-labels
4db49525226e1c9ab518abe9147ae68c69936f3b Propagate topology labels to MachineSets and Machines
00e665040fc306e419529309fb753a0f326b5733 Merge pull request #5210 from SataQiu/fix-20210906
ea5ac6bbd346e221be7d709c16f02dd9f7584bf9 Add ClusterTopologyMachineDeploymentLabelName to MD templates
d1c9c410a364921c912e4e2163ae92754347e5f5 cleanup: using Complete() instead of Build() when there is no need to return a controller
84d7a3c3fe202ce090bf247a11f54ac3a902041f Merge pull request #5202 from vincepri/machines-cluster-name
30cdde428ab0527584acd2c4a48cc111fe54611a Merge pull request #5201 from vincepri/tilt-reload-gomod
4309b1f216c08a0ba416b475e3395b842f7968ba Merge pull request #5200 from sbueringer/pr-upgrade-controller-runtime
fa55e8260e131e71c0ee97e51ab03223e9192d0d Add Cluster name as printer column on core types
b62c3bc7f855eaf9cc1cc180149defc84547012d :seedling: Tilt should reload CABPK and KCP on go.mod changes
4e0a8e6fe4e32551625dba45c5238eac976689ab ugrade to controller-runtime v0.9.7 and Kubernetes 1.21.4
b99ff451026f6bd6a16176a885276c562a9c8e62 Merge pull request #5188 from CecileRobertMichon/release-action
f882252094f1d800d73b3dad71ad6fb15610eb4d :seedling: Add GitHub Action to automate creating a release
947147213c525b03c146f46c2eb41590abc1bf71 [e2e framework] allow for overriding flavor for all e2e tests
56167df1ed057f76812e220a4fdeb313775030b5 Merge pull request #5181 from spectrocloud/clusterctl-maas
0c1b1fc9ac5828f95eca89c1094dd3dd0a98a73d Merge pull request #5185 from alejandroEsc/ae/move/fix
313b1fa9c6b205d06d979e73543cd47d477cf00d fix: make move idempotent by handling machine objs correctly
ec87b0044a83b3ac52ea691739b1d0cb48e26052 Merge pull request #5180 from Jont828/age-column
02e6cd26cf49948b74bf94b6de4be9e67e24862f Merge pull request #5179 from stmcginnis/add-stmcginnis-reviewers
778feb8bdf8aae4c35e9abde7c37f8d44d4f5890 Add 'age' column to our CRDs
7a75113b5d24528a36e1646354cd54f294b9320f Merge pull request #5187 from sbueringer/pr-fix-kcp-meta-reconciliation
51cae47a1d2539be7a18ff282423bac3cd4d39ee KCP: stop reconciling ObjectMeta into the KCP machine template
fde4fcba28f433a70da0c3122cf125cfb3a8557f Merge pull request #5182 from detiber/kcpUpgradeNPE
95cb70477902c9fe09d56334f799614ce302820b Merge pull request #5137 from killianmuldoon/pr-update-tests-with-builders
7601ebddedd5aee436172ab3faa30467b75573ac [e2e framework] Avoid NPE when KCP does not specify ClusterConfiguration
a4f56ddc3539fb522db11f6ca4b35f7d7ca2a755 Merge pull request #5134 from fabriziopandini/cluster-class-cleanup-logging
d75a696f9af51792abb7b039784f0dd4253cc7c2 Update tests to use new ObjectBuilders
79234da378dd31bdd2501d2be7150dfcb4851f2b cleanup topology reconcile logs
7f32001840d34deb1beb33bff2d78075fb876af1 add maas provider to clusterctl
867f41918d3c278f3e9d771cf81b61fe7717563a Add stmcginnis as a reviewer
8e43e3a1cfd3d6baee609817a6f8850a798b49f0 Merge pull request #5173 from sbueringer/pr-propagate-metadata
85953a9d63d2c1219b563791dcf36018df5fda5b ClusterClass: propagate metadata to machines
a274abe7374037014a1cf3bc02b6399b5b73f27f Merge pull request #5177 from alejandroEsc/ae/restore/fix
d25bbc2ea9c71bf482746c358195c0678f638042 fix: log in restore cmd causing crashes
b3a86a726cd896338bab402d93d8d3e0ee8235c7 Merge pull request #5172 from sbueringer/pr-fix-get-gvk-metadata
0b8a04ae18be60886010a0495e9eacff60dbbd1d util/GetGVKMetadata: fix get PartialObjectMetadata
764d1bd793a031e1c5f702a9c80dc248bf34832d Merge pull request #5170 from sbueringer/pr-fix-reconciler-log-name-kv
2282884d4e9e84448554e98c72a23382331ff59b fix reconciler kv in our reconciler loggers
c7793f615764f8250c6d215ef4f0fb4f55a13ca0 Merge pull request #5166 from vincepri/golangci142
cdc93477b35848a89f78332d0ea1e754f7164ae3 Merge pull request #5164 from sbueringer/pr-misc-clusterclass-fixes
b77f972a4b37785feef89b76343433a948ad0300 Merge pull request #5143 from sbueringer/pr-kcp-convert-machine-ref
684d7536cca615377e2810f25c66e5a935f58542 Update golangci-lint to 1.42.0, enable more linters
ad2d9724f6514012846d5dd6e3362b7996f0b26c Merge pull request #5161 from vincepri/proxy-conn-pointer
4213fda446d23d978e5a6c53ae6f414abe37a19b Merge pull request #5167 from sbueringer/pr-fix-capd-panic
fcf96a55c7f0a944218403f8bab8c861ea13c0e1 CAPD: fix panic in DockerMachinePool reconcilation
31b6d2c8c14cdd899c4669c1346203f854568575 Merge pull request #5149 from sbueringer/pr-doc-test-exec
13c4d9e26da7d13bd3fe1c867362a6b0397db1f7 book: add tips on how to speed up test execution
408f30bada3e2994f93ea1dddd468682f8e63bcb kcp: convert infrastructure machine ref API contract
c8e51e38095909eeaeafc7dc5b6daecc7c0858b4 Make topology controlPlane optional
cf6797b9c94370df577665d3bd5fce511ca7cdfb ClusterClass: use namePrefix func consistently, fix MachineDeployment template rotation, fix unit test panic
dbc0120b1120e54141d97d37bd4a81285c1df859 Merge pull request #5160 from vincepri/update-contract-ref
6c138584ed462aeca11dec53ef5caffe22376d00 :seedling: Conversion of references should use a CR client
b0e4c8bd0156674bcae8e3bf662dda2278fd444b Merge pull request #5151 from killianmuldoon/add-reconciler-to-logs
811442460c25ba7d5e9467773f7a031232c582b0 :seedling: KubeadmControlPlane internal/proxy should use pointer structs
9c92a8d436f1b12ccec9f218d27387ec6dced5dc Merge pull request #5158 from sbueringer/pr-fix-clusterclass-controlplane-template-rotation
98f6771e0cf1da7af86574291a0f21132ba39508 fix ClusterClass control plane infrastructure machine template rotation
fb4569aa93be02e77a78c9c06270111db3b50aaa Add reconciler name to loggers for context
af60d1df6a6200d1d6ae38b8f3b1eb9eb2a7c7f6 Merge pull request #5110 from enxebre/mhc-log
a6bda00cdf2dcb908bb1dd24af45de22bbd3b7d5 Merge pull request #5155 from sbueringer/pr-add-killian-to-topology-reviewers
ab40dc79d20f1b546318892edda99fd7ba777308 Add killianmuldoon to cluster-api-topology-reviewers
7b97ceaa3184019ddd7ea816327bb5709895114b Merge pull request #5154 from killianmuldoon/fix/caep-cluster-class-formatting
f48bd7391eb3916ece09dd0c69415b8a11abc9c3 Merge pull request #5055 from killianmuldoon/refactor/move-test-mock-objects
bd404efaa3a52f7e8dde3f48ed1a5c623c4ddb8a Fix formatting error in ClusterClass proposal
dd0a73fcc68879b29f77b73951aaba1cc9853d07 Add internal builders for testing
1ce945674c122310cb0c040fb587be23e05fd6db Merge pull request #5150 from nagygergo/patch-1
9b4a51a01341f483b22ba1dab21bee00be6c067c Fix typo
103997de6485c00f58dd1d8db9e34a98adae6e3c Merge pull request #5148 from fabriziopandini/move-predicates-pass-logs-to-v6
cf769543a93ea7f1605be10c186a5ac2997aaa3b Move Predicates pass logs to V6
dd8048ce988bd7d7ab6dce760c2ce12e06c2482b Merge pull request #4985 from killianmuldoon/caep/update-clusterclass-with-rebase
3e54e8c939090c97a718a553ee6dce5b4c054731 Merge pull request #5102 from sbueringer/pr-envtest-with-kind
8f9f1ba4ba2d019824746d0e74443e0a5cb51dac Merge pull request #5131 from vincepri/allow-machinetemplate-mutable-apiversion
ddd267ee9a6e9b130d57b7310bb82dea0828af97 Merge pull request #5140 from fabriziopandini/cluster-class-create-contract-package
812be2c7321c420f64b1d420dc1a74dd203ee458 create internal/controlplane package for ClusterClass
6fd74faa34395eb25486848b146033968a407359 create internal/contract package for ClusterClass
36d4d2eede00c84774296ea8cec0b1db9c196cc2 Merge pull request #5144 from sbueringer/pr-bump-clusterctl-upgrade-to-v0.3.23
61d94c6c1a04375275111230272d9230dadf41bc Merge pull request #5109 from alexander-demichev/docs
c6f8e21f5a2b81ad3682595d175747a52f1ea0c6 bump clusterctl upgrade test to CAPI v0.3.23
766dfe08d37aa0bc9548407c84b2441bea5121da Merge pull request #5135 from fabriziopandini/cluster-class-create-check-package
79cea8534e327f246d103b6888b97777771678e5 create internal/check package for ClusterClass
495158fdb31e99a0dd8ceedfb5320cda42ebd3d8 Merge pull request #5138 from vincepri/default-kcp-rollingupdate
331195d06026ad39d93d7ad9164164e76ff0cd5a :bug: KubeadmControlPlane rolloutstrategy should be defaulted in openapi
63bc71411d792c98502a18e2f1de79b74fd7c3d4 Update testing docs
75104dc8460eddd17659f41c06a10e93966d7764 :bug: KubeadmControlPlane should allow to change the machine infra apiVersion
cdf2905db3c60cbc3fa6bd3b8d92877f64b3b164 Merge pull request #5128 from fabriziopandini/fix-blueprint.HasMachineDeployments
126c71d2635b32e41ec280ebc2d2012818b25b32 Merge pull request #5126 from sbueringer/pr-add-clusterclass-webhook-to-envtest
2432dd3c3404bcdd259c48de1ad19434756af91e Merge pull request #5105 from spectrocloud/document-vscode-debugger
a2bd4c4758a7d7796454af8b6a6f4c0acafa8c48 Merge pull request #5118 from Nordix/uplift/cert-manager-kashif
3c8d891336c9e250c5ef12559ee7e1056c2d0c46 Merge pull request #5127 from sbueringer/pr-fix-clusterclass-webhook-nil-pointer
70b8b5befb2c295baa3fe782202bf421a4b4bc27 Merge pull request #5129 from fabriziopandini/add-mergehelper-ignorepath-option
32fd1578a78a19cad225e6154a52987ae0e9d634 add mergehelper IgnorePath option
e7c69bb78b7b82d84b086bb24c0439ba312b5fb0 fix blueprint.HasMachineDeployments
cc06f9bd3cf428e36e385218773e478839243e8e Merge pull request #5119 from fabriziopandini/introduce-topology/scope
f950b4c4ae0f3be530a7dd4a29a5d38bec404b1f fix nil pointer in ClusterClass webhook ref validation
984fb38a8d6d125726bfc893e2c635f8fe38ed89 envtest: enable ClusterClass webhook
5ce6413994429eca72d845f2d4116173fa3562bf Rename clusterTopologyClass into BluePrint and small cleanups Co-authored-by: Vince Prignano vincepri@vmware.com
71d1a3447d1d4d84566f0a64871f0eb4b907aa09 Merge pull request #5104 from shivam-51/docUpdate
1fb53c85d7ffd25f9e2fe0004be006a31ff51d58 Merge pull request #5117 from fabriziopandini/move-mergepatches-to-internal
bdea4892ef203c074d7f7b4fc4338c225b0dc931 Set unhealthyLimitKey for logging always
5ee07ee2e4f77ccdd969cbf170a4aab25ae3df25 Upgrade cert-manager to 1.5.0
a116c8d3f5f8080b22f92e008be0337c08fe60b3 Updated Quick Start doc to include GCP env variables
b36169346f8fcbe5978256d374fbba16d9d8c124 Move topology/mergepatch helper to an internal package
70917d9b2c4c8a5219e427d788e92072e53ef0e5 Merge pull request #5100 from sbueringer/pr-fix-clusterctl-upgrade
2ae1490480540438a4d62cbbf202baeef50a7667 Merge pull request #5116 from fabriziopandini/make-mergepatchhelper-skipfields
c31a00c1bcf4694aed92b1f8c18f72792e6ec4b5 make the MergePatchHelper skip metadata fields computed by the system and status
ec6a3258e905f3d8db92be7555e38dee9395356d Merge pull request #5090 from sbueringer/pr-default-clusterclass-machineinfra
f9bed2aa77879218d8af62de42c578c36263265b Merge pull request #5114 from vincepri/topology-review1
d484f5ed651242613973907a52ab4890d15111c0 :seedling: Cleanup controllers/topology code, add more comments
482f6684f4245dd29f8341c6dc435ca28857d693 Merge pull request #5113 from mboersma/apple-silicon
1f0c8eaa342f5e9d815d607b8dfc125cca8d1dfc 📖 doc: mention clusterctl download for darwin-arm64
39e6ed14261f65dae2ba817f21b0c21eec789158 Merge pull request #5101 from killianmuldoon/pr-reconcile-controlplane
7d33496c199ff0a7e999c8ca999e89053e3b44b0 Add reconcileControlPlane for topology controller
b35fc64f79baaffd96b56cbebcd8463554b60ad6 Merge pull request #5111 from fabriziopandini/fix-cluster-class-reconcile
09f6ebf095f418f5ce66f8b9c12a5bed1a76c824 Remove info automatically assigned by the API server when cloning templates
4c958ef0d5dba69e52e68a757ef73b4adb96c70b Avoid panic if there are no workers in a topology
c26190e8821ffcb5b379ed9bfee244e9694658d8 Change delete behaviour to respect inventory
20ad71d5c658c5545d5aa0db4d90a230aeee1cd7 Merge pull request #5107 from mboersma/update-for-azure-rename
a48fed4e8d19f9c51c62b98a966131cee0134ec1 Merge pull request #5072 from sbueringer/pr-reconcile-md-topologies
1d8088f3c5e9d9e79015cac41fb9769c58143edf Merge pull request #5106 from sbueringer/pr-move-defer-of-to-be-fixed-list
362f129583b16bb71cabea75f35b684eaa20d7dc Reconcile MachineDeployments for managed topologies
76ceb966abb8593bf7b69bca09861c79efccdd2c 📖 doc: update Azure provider links to reference main branch
003873ad62402a05977b922352dedae30ffd9028 Merge pull request #5070 from srm09/cc/compute-machine-deployments
e736105774a602c61045f5d6b3c6e03eeb9c9f8d Intentionally ignore Deferring unsafe method Close on type *os.File
b043a33ce6f954c1dc166d25a1e8984c296b3916 Adds logic to generate machine deployments
f17648e01f02c8593e80e3a6e2198b1c12380d24 Add validation for ClusterClass compatibility
fae587ac7189218bd87407e74822cdcbf425d5f2 Merge pull request #5096 from sbueringer/pr-handle-v1beta1-crd-whc
25dcb0009c51364b70ae3e182a0ab66b88603014 added documentation for setting up vs code debugger
f23f2635cc8f4cbc931c67d62b176518649e4918 Merge pull request #5093 from detiber/clusterctlUpgrade
fe7850a8d5b5d71440070bbdae348df4fe086ccd Merge pull request #5103 from sbueringer/pr-update-jobs-in-book
ccfb9fc4d3a75dbcd3897c1958b40083675026b3 Update job overview in CAPO book
27d64dce9fcbddbffb3be925d34777487cf9372d add shell script
1868b9a3300925f30c48ce423ffd001792dc8dd9 Merge pull request #5081 from sbueringer/pr-e2e-test-configurable-mgmt-cluster
ae000025b726284b7ea1ff98d50391b12ee5a0f4 update
7ceaf3102b84590504383e195c380d17b927ea82 Add env var for envtest with kind
68ef481b5e626a1f0fe08d2c100bfc8004ab1c49 clusterctl: fix target namespace in v1beta CRDs and WebhookConfigurations
f8cc6f57acac58763bfc84d8589ea1a05118baa2 [e2e framework] Add ability to run pre and post actions during clusterctl upgrade spec
896e927f4deb24a89a2b48865994e1657acbd87b add some more doc about Kubernetes versions
dffe1ce5d0fd4e66d4b2ae62a475321417387f6d Merge pull request #5092 from detiber/optionalMachinePool
f91f5027536a032de6c7065f65b7c2faaabff16c Fix clusterctl upgrade e2e test
7331b2f3bbd2684b04d811f302ad4071e21ed434 [e2e framework] Allow cluster upgrade spec to work without MachinePools
498348e23773107c157ee01f729f63a91b00fd15 Add namespace defaulting for ClusterClass ControlPlane machineInfrastructure
f6fd5ed7dc0fa75788f76f17c64ae82976fcc70b Merge pull request #5031 from ykakarap/kcp_status_version
0188b290115404ca862a22f1e69b3f4c53c87ab6 Merge pull request #4934 from ykakarap/init-wait-ready
fa91d8a608bf8ed3cda7d8bf7e36d385225e04d5 add version to KubeadmControlPlaneStatus
79686f616a1455e2bc3226230b28218066f8918f Merge pull request #5084 from sbueringer/pr-add-topology-owners
0b665589f72252f14d4a0b40a88eec7932f2ba58 Merge pull request #5079 from vincepri/add-node-info-machine
bff7e6b8f02e2af83f83526847034f67c12b5d58 clusterctl init: wait for deployments to be ready
e804a164e10974270b71e3f846249c9fa3976bf4 fix review findings
e5d5c26db0dea5183351ffea9f620c4a68b83109 Merge pull request #5082 from ykakarap/clusterclass_cluster_events
4697cb029de8226043e1ccc4d2954584fa6438c9 :seedling: Add Status.NodeInfo to Machine objects
8654bf5ebee7ad77894aa363a5cfdb5a0994662d Merge pull request #5088 from fabriziopandini/pass-clustertopology-featureflag-to-capd-and-kcp
5d601fcdc6961d3b5eb1bbb86591b3bece39047f Pass the ClusterTopology feature flag to CAPD and KCP
99def25e0627f44c966dfa111fe920439b9334cc Merge pull request #5045 from killianmuldoon/pr-read-clusterclass
383b9d0dc1412caffa0f6efa27cf08e2b7d890ee Add getClusterState for Topology Controller
7c76c15905b3c0a4da503792a9a1c1583c4ec844 Add ykakarap to cluster-api-topology-reviewers
b88eb50035b39af815282d63431199ff1c584c9e e2e tests: make the management cluster image configurable
683c0ad44d2dc4c28612131162070003190406b7 implement ClusterReconciler.clusterClassToCluster function
8ff6ec836aa4f72e6722d10e0f81ccba4cb8be4c Merge pull request #5080 from sbueringer/pr-upgrade-quickstart-and-tests-to-1.22
5bcc68d1c22cc30b5aa29ed2964393d1b693ff37 Merge pull request #5075 from spectrocloud/add-capmass-provider
33399c7dbc4fd3c6226594d5f5da4ce2b7a1ab04 Merge pull request #5052 from fabriziopandini/clusterct-class-reconcile-infrastructure-cluster
d5cb23d96589e505c37d675b1cdcb94ec21ac24b Upgrade quickstart and e2e tests to Kubernetes v1.22.0
3b9c1b71b8bdc3049ea92970991e34afd9bbda7a Merge pull request #5077 from vincepri/increase-time-poll
505b45c15a1f1e8bfe284b49dc232ec6d3072f94 :bug: Increase polling interval and timeout in ClusterCacheHealthCheck
01a5f2ffaefe118ffa83d2031600e179477a585f Reconcile infrastructure cluster for managed topologies
b33fefba227a353b5f3f95918d8a679378c544e0 Merge pull request #4981 from asalkeld/memoryRepository
9d44379e879ffdf3cabc70c66261497bd783a1a1 add maas to infra provider list
cbaa42db166c3696ab22a018d2a9418fd3425410 Merge pull request #4967 from ykakarap/clusterclass_cluster_topology_index
baa78973f98216e05bdbc03874722aacd23fbdd3 Add a MemoryRepository for the operator to populate from a configMap
239e4d1811ffdfdd54dbe87f239e898a6ec29ff6 Seperate out LatestContractRelease() and LatestRelease()
f873fd03dada63356e78e06ac41bfe77d618ba50 create index for cluster.spec.topology.class
1ff006a73a4e03863c72c00e5f1cd87edc4ded5a Merge pull request #5074 from vincepri/cr096
2b3275b5bdff3b33931adb212016d1c549923192 Merge pull request #5061 from superbrothers/local-etcd-extra-args
46a708dd360565baefe7beae67a7c5eed1de09a7 Merge pull request #5030 from sbueringer/pr-add-disable-test-env
af53b4b0f59f328bce428f7d63bfee6cc04acf33 Update Controller Runtime v0.9.6 / envtest Kubernetes 1.22.0
9044184bf1c68f1af9c9d239377611550786d864 Merge pull request #5068 from ykakarap/kcptemplate_clustertopology_flag
7c9a33270c8c490eef8bd6f9a2ed58db6ee8ae76 Migrate envtest setup to envtest.Run, add CAPI_DISABLE_TEST_ENV env var
ee0f31dc58f035ebb7f38de014bdbb515901a8bd Merge pull request #5071 from fabriziopandini/move-clustertopologyreconciler-to-separated-package
15d4d4fbc1e7bc17b0a592c007d6d77daf273108 Merge pull request #5004 from ykakarap/add_index_package
00556a3d2ea04a268be9a004214077a56fcadb01 Move the ClusterTopologyReconciler to a separated package
7e7fba17bd683b74a00a3baf5073f7d0bc05d4a1 gate KubeadmControlPlaneTemplate usage with ClusterTopology feature gate
12184b209cd30c9bd2845b05eafc41f17ea52360 Merge pull request #5069 from ykakarap/dockerclustertemplate_clustertopology_flag
8e61e2688f9ec6a4a2bfb99a4b2fb9f3012ddceb Merge pull request #5002 from fabriziopandini/cluster-class-compute-part1
e70846d9bf833b909d80667e078ac194f3e9968e gate DockerClusterTemplate usage with ClusterTopology feature gate
4e61173a190cd234600e2b87923712ed7d89f43b Merge pull request #5063 from sbueringer/pr-fix-e2e-disable-metrics
ccaebbf2e99c1b15483223b29bc96a0bec60f855 test/framework: fix disable metrics collection should not disable watching deployment logs
2e27118e45116fb52dd60d8874176830c31c74de Make local etcd's extra args in KCP mutable
92e386733059aaf87f63c19aa729ba166d68c6f5 Merge pull request #4992 from ykakarap/clusterclass_validations
558ea0f1c19477f9097e88e8422d530266b5d223 add additional validaitons for clusterclass type
1741d44d45414b9f26201ec7dc8c10b6b021bbea add api/v1alpha4/index package
24b57cfa44041e1a4aba883f9043b31774644469 Merge pull request #5051 from sbueringer/pr-fix-cert-manager-version-detection
80cdb6385208d8e53b727c79d0b0c4a85b520c6e Document that mdBook+plugins are downloaded automatically
cb9fca6449a0bde5c640ec6de8675f057f123635 Merge branch 'master' into contributing-docs-note
83f2f48e53663e49164f0ef8ad23a04f9dad8f53 Mention that `serve-book` auto-updates on changes
de92839ecc9f399daed3ec82166810cb9c812f17 Fix wording
5f9e7e069242591d59d4e2502805785cdf1349d7 Fix wording
f95d638aa5e657f55816ba1d1ce3fc2511f3bbb5 Merge pull request #5027 from sbueringer/pr-add-bootstrap-template-update-doc
e3e90e3eb465f092f203e0656d1936eb4fb21e0b fix cert-manager version detection with EndpointSlices
aafd9fe430358d36c946be695865d1a4caf57d10 Merge pull request #5050 from sbueringer/pr-fix-clusterctl-backup-panic
f88a7615e22d897d3fb86dc87113baeb95d12c93 fix panic in clusterctl backup
2c5e6890151cac9126034f7df2dd60baf1ca1832 Merge pull request #5042 from CecileRobertMichon/upgrade-tests
0a5c9607cc55b2269ca5c083181feb092f17dc26 Merge pull request #5048 from killianmuldoon/fix/update-test-address
a9bee8837738910086628cbbcd50dfe560fd4030 Update envtest listen address to localhost
3f220870c44108f1f63c50d3bf1afdabcfe14202 Generate desired Cluster and its referenced objects for a managed topology
ca0b6a9fff774e90b869b5b25991251a1d31a4af Add flag for skipping conformance tests in ClusterUpgradeConformanceSpec
1c39866774726af917ec2c1cac44dbaa876097a0 Deprecate partial upgrade tests
914e79ca83be56acfcdadb187b2edc2d3fd49433 support NodeRegistrationOptions.IgnorePreflightErrors (#4905)
a79fafbe703ff3be3c50953e6ffa147f8aa09b71 Merge pull request #5034 from fabriziopandini/cluster-class-patchhelper
9657769c58479be47aa5b7186514230df22a8a94 Implement twoWaysPatchHelper for ClusterClass reconciliation
872703141ec138af63209ba60382e508f0048d93 Merge pull request #5022 from fabriziopandini/cluster-class-templates-and-reconciliation
c24337a5b2e893bfb5e30abfc153c400732ce581 Merge pull request #5007 from sbueringer/pr-read-clusterclass
35ff95d1973044ed03b4895d887788ccbaca480f Merge pull request #4945 from spectrocloud/wait-volume-detach
39f47041a7897b378956a8f7b69fe5ed4d8ab017 Merge pull request #5040 from sbueringer/pr-introduce-new-test-crds
504e2a3e86377a003119f2618e9e2010c5563c71 wait for volumes detach after node draining
614857370ac5af609d89f50e444d4f19b3301958 cluster topology controller: implement read ClusterClass
a01ab183939eecf08c3151a13e5145729c7a8ecd fix review finding
af4b98df6214c5e130d61ee5ff715e643547ed18 fix review findings
1744df95b741a45ea546d33305e155309229f599 use new CRDs in unit tests and adjust them accordingly
90c1f2c5dee0d61b290650887d614e136cda7f77 use new CRDs in envtest
132703da6e189e962664a0a769f36256ac1197d9 deprecate test CRDs in ./controllers/external
8265b0f8337ffca971973376518ecf675c9a69e1 introduce new test CRDs
5aac303b28b66c40d4cacf628a2fba941558c469 Merge pull request #5039 from sourabh3b/update-generate-cluster-link
8f25f608a2ea355d0bd0fdb55cfefae50492e853 fix: update generate cluster link
c582038943cc216d4b779760f189f044afa1655f Merge pull request #5014 from asalkeld/fix-webhook-namespace
b6d4adcdaf22a775ae5c61ea82b36ffc886a2496 Clarify template conventions and template reconciliation rules in the ClusterClass proposal
c4232d82785b112a94e799f2b82a95a3395c8326 Merge pull request #4959 from GrigoriyMikhalkin/capi-4629-controllers-pkg
2f5bee4f126a94ce3b9a4f9d124ae914ea776498 Merge pull request #5033 from sbueringer/pr-kcp-untrack-objects
4a01fee71aff0bf764b8dccab334bfea5b0d1748 Merge pull request #5012 from sbueringer/pr-update-book-kubernetes-versions
488d1b4511a9c63b803372266722af0560d46e12 kcp: stop caching ConfigMap, Secret, Pod, Deployment and DaemonSet
a33e91e31f264549f558fbc5f4128a6561d530d5 book: update supported Kubernetes versions
00faddd5e71aea934f2eebc961becdcd2f55b945 doc: add update bootstrap template doc
99049e7853bf3ee72e8112da6487a6e14f6db5ca Merge pull request #4963 from GrigoriyMikhalkin/capi-4629-util-pkg
53168dc14650d141488678551f056b946b0b74c6 Merge pull request #4962 from GrigoriyMikhalkin/capi-4629-exp-pkg
ded9d6c0c2c6a37be6a7814fc667b52f5cc60117 Merge pull request #4960 from GrigoriyMikhalkin/capi-4629-bootstrap-pkg
0b12730732dce92b4b4b73a0c2ab303ca7321d62 Merge pull request #4961 from GrigoriyMikhalkin/capi-4629-controlplane-pkg
ea421c2aac34fbb6c3807a3b2f0a4630d5732a7d Fix webhook service references when the namespace is changed
63c535c7a0b3a574a33c5477174440598af95420 Merge pull request #5028 from vincepri/cr095
3332afc981ed55e6b3f4cfb7b132ad4a04ac4abb :seedling: Update Controller Runtime to v0.9.5
6deec3b77668e47b51ae4c9dbd41a441c44fceef Merge pull request #5017 from sbueringer/pr-ignore-command-injection-in-tests
52b976061c448f2ae410afa0ed6667a2a5e17437 Merge pull request #5021 from stmcginnis/capd-restart
2f3a76c5670c1ce035f7f382db5ae1f79a44d0be Merge pull request #5023 from vincepri/mdbook0411
b71c02fc58a11e4cc006e5b17e68b7abfde49492 Upgrade mdbook to v0.4.11
c90f3763617d8bd33c697bebd1be5cfe37a2102a Merge pull request #4993 from ykakarap/controlplane_topology_optional_replicas
04647ea9d08d0a8e9e5f75791899b4bec20e85bb CAPD: set container restartPolicy to unless-stopped
459e8e6eebf4d213299b7192124092d509a4cdb4 Merge pull request #4949 from fabriziopandini/clusterclass-controlplane-contract
e12ed2c9b62bf4c6a71311a11dabc70f7ac34152 Extend control plane contract according to ClusterClass and managed topologies proposals
23e0a239852f5857d149984287876cfe0060b27c explicitly ignore command injection (in our tests)
deea51d67b7a7de00a30efa4e139f7455bcd790c Merge pull request #4904 from ykakarap/kcptemplate
a7048697ea499331bd83c9978007cf255a763903 KCP: add KubeadmControlPlaneTemplate type
19d190e3e35e0ae2683747f332419e4889530368 Merge pull request #4986 from fabriziopandini/cluster-class-testutil
fb171294eb371a18bed08f9a9c9e9c14ccd86a85 Add test utils for cluster class
ff3c2bd907489853aaf5781a4c6fb17509012525 Merge pull request #4989 from sbueringer/pr-add-webhook-healthcheck
6e3aa4a085c9f8527c8e412116f84da2dcab7e70 Make Cluster.spec.topology.controlPlane.replicas optional
c1f399c9791f3867b6acb891f86161642f6a4a06 Merge pull request #5000 from vincepri/clusterclass-controlplane-alignment
8131b65f00606a3dd625caa1d87a330c6d7bc188 Merge pull request #4997 from timoreimann/surface-etcd-node-check-error
125eeced6a4a4ab8e8d8e309496849a24b68be13 Surface etcd node check error
bc720b46ecac781eed350753e254eab90a637b85 add webhook readiness and health check
f85f37a0b607829ede5356d4a4fc4be2f03b523a Merge pull request #4903 from ykakarap/dockerclustertemplate
fce43edf16b581b0d04abe5ae174607f10b21555 CAPD: add DockerClusterTemplate type
509daead3284bd67017795bf4c5fb9d059ca91fc Align ClusterClass ControlPlane with the rest of the fields
039c1d8324697a3dfbe35ec294f7a0a7096e83bd Merge pull request #4947 from enxebre/fix-noderef
0f1bcfbf3cefaafdaabe895d3a9f0f9af25dabb6 Merge pull request #4965 from fabriziopandini/cluster-class-controller-scaffholding
ede33e3e1aa66239cfc14b9e6ccee2b8671d32e8 Merge pull request #4975 from vincepri/update-release-notes-doc
672b80655eec73ea70ff804c4803f87850ef4d63 Drop aggressive requeue=true and find machines to nodes by providerID
78cf4e9ba8e2387e175b44f501b321d635b5554e Merge pull request #4951 from stmcginnis/capd-lbconfig
daf871f272bea18d6186af79efdf2750c13eba36 Merge pull request #4995 from sbueringer/pr-upgrade-clusterctl-upgrade-test
018ca0a6bf160249cb57f18939086614163fe858 upgrade clusterctl used for e2e test upgrade tests to v0.3.22
e3b758d07c9b5e16255f56ec6244fb9f7d09d164 Merge pull request #4990 from sbueringer/pr-upgrade-certmanager
b7aa6138aeeb8fd3094c3fe481f5af44576942e0 upgrade cert-manager to v1.4.0
9478711d8783980caffb0527f5e4707367cc6d26 Merge pull request #4987 from vincepri/cr093
b6821fbc3d6a02df5c23a996ea1e789c8f3c6637 :seedling: Update Controller Runtime v0.9.3
35ddf0c38d7afec337a02c8ad388bc3488769d28 Add ClusterTopologyController scaffolding
2b5910793fa4f03c0391f7b4a02189db9aac74cb Merge pull request #4977 from stmcginnis/kustomize
c83de075f822a9a5bc48bab660248cec49ab7747 Merge pull request #4976 from srm09/cc-impl/cluster-controller-for-topology
415770fa5898278f68b2136fbd6d41479593fcde Update links for kustomize installation
3d09aa1c94ff42f72aac6f9b2c891b88602e59b9 Adds topology check to cluster controller
7264f91a4ee9f3dcf0091af08007fd349a232be0 Add ability to set DockerClusterSpec load balancer
c5bfbec448added37bc2bb861b93ce03bf431063 :book: Update how we generate release notes
5296d7fafefe5014400f140dfe9cc73a82be9d76 📖 Add info about contributing documentation changes
60b0cfa4c474adc38ecca97335c96d98e1f71c9e util tests namespace creation refactoring
c42f35f8c41e1d8bf3c8c19cacbdebe1ed2275c2 exp tests namespace creation refactoring
ddb0cd0e897e90284987d3d006bec5aa7bdb9fac controlplane tests namespace creation refactoring
5bf69ce94104f312a3cd2ab0b8248f3f64d36486 bootstrap tests namespace creation refactoring
036955255cb0c0ff755991661849a3148f10f2ef controllers tests namespace creation refactoring
d9a16c99ead2077a239b79b8adec5ae0f88c12f5 Merge pull request #4928 from fabriziopandini/clusterclass-api-types
9719e4f9ca2a59f7cd41d3518066202c9971b9ad Merge pull request #4521 from enxebre/get-node-index
fb67f57c2c33aa9b16864cead48f8ec42966567a Add ClusterClass types
604a4650df233d3318f3e37874928c40f5debeb7 Merge pull request #4929 from fiunchinho/missing-watch-filter
9fbe82703aeb53b1258e40c2af9cf366f696effc Add watch-filter support to ClusterCacheReconciler
4d087c0f5d151a7e35b35b023a3601b7211a372f Merge pull request #4964 from dims/switch-to-non-alpine-kindest/haproxy-image
925ed4bf60047377130708654461b6f5fb6f5e9e Merge pull request #4958 from spiffxp/use-dl-k8s-io
df5a943514ba8d4f179bd553550368f79e74edfa Switch to non-alpine kindest/haproxy version
be8ce08326956fb539c128342710aaf267e2dfed Use dl.k8s.io instead of hardcoded GCS URIs
831ed7db702b1479daae06d2d3f7cfebb2ce879f Merge pull request #4955 from srm09/cluster-class-proposal/fix-diagram-links
1952ed6d4e88066e27368d51416a25b6d6e8f9db Fixes incorrect diagram links for CC proposal
2b9bcaf24d5c1232c32d6b541715629aacab6f93 Merge pull request #4952 from sbueringer/pr-fix-kcp-aggregated-role
75d12c71133cae29334a79af2dedb2ac5cf3d802 Merge pull request #4937 from sbueringer/pr-fix-upgrade-to-coredns-1.8.4
3c9e61af9572e3b5eaa70d46ae2b62a66c804d21 Add Indexes to NewClusterCacheTracker with providerID index for nodes.
ea7d15c82d167bbdba700f42bb8d99599730f386 fix KCP ClusterRole aggregation
109abc52c02e0a00089ecd69a7ec17ff21fb187b Merge pull request #4625 from Nordix/md-avail-condition
c0caa60879805ad49be306470ba3bc24b75f1787 Adds Conditions to MachineDeployment. In particular, it adds `AvailableCondition` and `ReadyCondition`.
2d8357b1b5ca3507bee849326ab6e988bc276125 update CoreDNS ClusterRole (Kubernetes>=1.22,CoreDNS >= 1.8.1), fix image pull
c5bbf36420b14d6465b107df689701b4b3ffdb25 Merge pull request #4895 from sbueringer/pr-fix-unhandled-errors
ed520a9381e7f28d11fcdc152538c28917d98e12 Merge pull request #4893 from zhangdb-git/master
3b0e046a80088947c9bb857107e7ff36e0fb7dc8 Merge pull request #4944 from schrej/fix/4943
a97cd3c00c8adad174ac78ac117f38a690b44922 Merge pull request #4899 from sbueringer/pr-document-jobs
8c48f7a07a704a2746701a6573d831d0654a9d44 Merge pull request #4942 from vincepri/accept-v1-v1beta1-admissions
7e5424a151c29b9e90cbc68112211cbd97b7a5c8 validate namespace of MHC remediation template
a374bf23bd12130012ae248cd63a4472a0dcf727 :bug: Webhook registration should accept both v1 and v1beta1 admissions
f627bf97cba889c5a5b84ff52ff756b060adb1e4 Merge pull request #4918 from sbueringer/pr-fix-cluster-class-proposal-nits
f68c82ab408508b4feb808ca06e78c73d26763ca document jobs
0b82ddf9023494d246388e9b37e1d2cc4d416972 Merge pull request #4808 from vmware-tanzu/save-restore-feature
0dc394ab37af1455a4465ee0e0fe55a485ee4cf8 Implements Backup and Restore.
bc94459d95c6809875ea78bb748e766165a09c2a Merge pull request #4907 from sbueringer/pr-upgrade-quickstart-to-1.21.2
44aeb1798bc1103a1f4d6e3237bde6e65f2c2b88 Upgrade quickstart and e2e tests to Kubernetes v1.21.2
e3febc783fc5bdb6f7d194f65e9a9e78aa2fc890 Merge pull request #4413 from stmcginnis/no-docker
38fababcfc3c7e4f7bdbe28ec7b930add9685d1d Merge pull request #4420 from sbueringer/pr-improve-inject-debian-script
23e90c870b18a2fc81fdc64fcec31952526523eb Use docker API instead of exec'ing docker cmds
add2c14d01e5ba54ff2d432ba59a4abfacaa0ca0 Merge pull request #4932 from randomvariable/bump-go-1-16-6
f1a4299f875f23186343283343b47917d2bae836 Bump golang to 1.16.6
b2d9539802d5e325a383f611272b4abd150956e3 test/framework: improves the way we inject the debian script
0452e8b6c83df098085b08798b35e81c373f21df Merge pull request #4924 from fabriziopandini/fix-DefaultValidateTest
d40b90ac8af1f7d08bb8c4da2a7d7846b9cf3d6d Merge pull request #4925 from CecileRobertMichon/fix-quickstart
6153b98892a9bfd3db9b57822ca00937018146a3 Add back base64 encoded CAPZ quickstart variables for creds
2da4b01a83cd10b8da93ea0bd96601ac84f4f723 fix DefaultValidateTest ensuring old object gets validated too
fc9c68264371e47d7c0c0c8ee8f166d14ebd658f Merge pull request #4912 from ykakarap/latest-releaseseries
0257793b32a133cbbd897256427ea1a108959a2d Merge pull request #4921 from nader-ziada/azure-quickstart-update
54da989e358be7122ed1a3f64df1de37f99c3c65 clusterctl: use newest release series of same contract
1570cf85dcf3571143cc49a94a66bdcb839442e1 add capz identity instructions to quick start
c4578216b88abf999062f34bc9915a357887fbe4 Add detail about ClusterClass reconciliation in ClusterClass proposal
87270011c60fdd336949ad22dd1b3c59498b8480 Merge pull request #4898 from sbueringer/pr-improve-quickstart-doc
4284fea6b423c3d6679c1a97e93712b99494f307 Merge pull request #4911 from sbueringer/pr-fix-mac-fix-kubeconfig
7d193daaa9e52ac655a1ee79215cf0c814527848 e2e tests: fix fix-kubeconfig for mac
4456b51b37a9d2a02982d06296c8c2acc90d5c35 fix unhandled errors
37c862b5c9256d7ae65cd8ee8ddd7a103d51fe90 Merge pull request #4894 from sbueringer/pr-fix-nolint
d1a613229edaa01582b6ea43f8a6f4205889e82c improve quickstart documentation
52d9cb44b87b1d2a8c2016d5804b5a8c7747b4fa Merge pull request #4892 from CecileRobertMichon/quickstart-0.4
16e3698546084d142cd0714621ee20702bd043bc Merge pull request #4890 from sbueringer/pr-fix-e2e-test-metric-collection
43cb458506087e7f59de3f943816ed352bf50a6c fix golangci-lint nolint:ifshort
51b5e474731314e60f75c91024b84e9029d135c0 Fix incorrect indents
ad4b4e8f6126e374ed2953f8160e47bf6f117e25 Update quickstart clusterctl install instructions to v0.4
7768a6db2ee986da2458e9c73d4c3c988095a4a7 fix metric collection in e2e test
18dbaecab79a79ac1d4808d75caaa00c68991c3b Merge pull request #4678 from srm09/proposal/cluster-class
a63c286f10cd206dca3490a8ee4a98d6667ae3c5 Adds ClusterClass & managed topologies proposal
a5e1b5fe003a29ec09a433cc5f6118e76993caa2 Merge pull request #4883 from randomvariable/ensure-finalizer-rbac
b495c58906e19f765da243df265b44e5329f1ee4 Adds /finalizer permissions for all controllers for Kubernetes clusters where OwnerReferencesPermissionEnforcement admission controller is enabled.
87142407f122f08ea7d363b9349d37e8d069e404 Merge pull request #4882 from randomvariable/july-2021-dependency-updates
b3c0e6f2aeae7fbd7dc556dad0f0bde1481db890 Update dependencies for July 2021
ddf72df1b67fff472420bec231c407471c6e0257 Merge pull request #4881 from randomvariable/byebye-dependabot
9515818c27164ec8a1960a0b034ae654eb37ba44 Remove dependabot.yml
65a66179b95f2e6f5ba94dd9fff92c9c90330891 Merge pull request #4866 from CecileRobertMichon/clusterctl-older-api-main
355bb9e2bda312b5d619bbd7270a855e6601d494 Merge pull request #4861 from vincepri/build-arm64-linux-darwin
d2c2ddb90a8abf8298540aacda903bc5b0354fac Merge pull request #4854 from chymy/fix-judge-err
ab6342efe471be74379a910673ba057c3fd5f887 Merge pull request #4865 from CecileRobertMichon/v1alpha3-book-link
cb6380bfc52442cb267f9eaa2862060cf09ad7c9 Use metadata.yaml in github repo to fetch latest release for older contracts
5d14ef0c7e25539388b532882821c8b750195ac3 Update v1alpha3 API book link in introduction
e7d72f7f8fc4156784272d1816f322e6cd1a4e5f Merge pull request #4855 from chymy/fix-nullpoint
8bdb6ef15d681afbdd9423a60dcb0f6d531a9581 :seedling: Build clusterctl arm64 for linux and darwin
b7c01e503f4dc58900d924d4d5eb31af3b4faaad Optimizing potential null pointer issue
81bc3d38bb4d61089da27aa251240e8976076466 Fix conditional judgment issue in upgradeControlPlane
686aef6a95613cfe87631e92a11cb55349da4725 Merge pull request #4850 from vincepri/improve-release-notes
c920241a8cf1eeb27d17263d0d19064af6bcb144 Merge pull request #4852 from vincepri/k8s1212
8c0a601b9e64af519735c84c47ceb340b077a6d3 Start testing with Kubernetes 1.21.2
604f5983899c6099f2adc4c622dccc25824566ef Merge pull request #4851 from vincepri/cr092
f6ea0d0ebc9e16557bdd4a0608327c2ac2b5c7a0 :seedling: Update Controller Runtime v0.9.2
ef5b247f5d18db8f43a847c082c9021e48d479fd Release notes gen categorize proposals and summarize doc changes
87daa8aa41dd271352288de79e34aabf82644a92 Merge pull request #4849 from CecileRobertMichon/upgrade-docs
9d2df21209711953cf640e78912392b2f5b1c5cd :book: Update upgrade docs for v1alpha4
7f879be68d15737e335b6cb39d380d1d163e06e6 Merge pull request #4791 from anusha94/gt_one_infra_provider
d6b31bb877d37a629695af530d0c180348b0d2d6 Allow e2e tests to install more than one infra provider
e57f23aab48fe60bb1304bcf614bc6ea4211a0d5 Merge pull request #4845 from randomvariable/tame-dependabot
048eebc4a861d17d64d62fbea1b7d46387cd9193 Merge pull request #4844 from vincepri/envtest-setup
a149fcfaa028bdf13be16724db84078bcea63a0d Dependabot: Change to weekly, enable auto commit of generated code
77f62724adb45ed039c6a759b65d09734ad3e4d8 Use new setup-envtest binary to setup envtest
6b5d9ab3f0d59083f3f7329a31741ef60db04a06 Merge pull request #4843 from vincepri/cr091
da54aae53848e483514f2c005edfb55e52526f7c Update Controller Runtime to v0.9.1 / Kubernetes v1.21.2
51a2795bf0f03c4e0ff124ae39366c9c4b939b7e Merge pull request #4831 from stmcginnis/dir-permissions
6c688c4bd745300720b2373ae8b48dd715824c2f Merge pull request #4823 from randomvariable/etcd-bump-v3-5-attempt-2
0967466df058b5bee51f785aeb53d7f9f505e75f Merge pull request #4830 from CecileRobertMichon/drain-timeout-interval
29d910b3eeaad0b9d376ca993c946adebba657a5 Remove lint exclude for file and directory permissions
6973ec12fb9f77b36cb4b22eaf9318193b221529 :seedling: Make node drain delete timeout configurable in e2e framework
8ad555dc1e819cfbf73264e46b41472a5fdfefe9 Bump etcd to v3.5.0
59c620c36aead9e76157210a063c05d33c3bd276 Merge pull request #4822 from randomvariable/revert-etcd-bump
7b2defb20ae64bfa85def210d7de9ed79b810798 Revert "Bump etcd to v3.5.0"
86466a11f43a0679d561bd1e18e050050b22fbcb Merge pull request #4769 from randomvariable/etcd-bump-v3-5
f1da11eeb574aa61e565c52edee3ab2de5d2069a Bump etcd to v3.5.0
3bdca52bdc28ef7213b9da02067642dda309326e Merge pull request #4785 from aayushrangwala/rename-listVariableOnly
f628be0930168701c75683165b1b97c47aad0a05 Merge pull request #4818 from vincepri/log-clusterctl-move-improve
4e05fb7bdc31d6b7b6cac560e2b0684d147a81e6 :seedling: Provide more information in clusterctl move logs
5177a4756317e48ce06117a1586f5a14cc950809 Merge pull request #4809 from shivi28/capi_4676_final
028ac54c0ea3f848c5b4d7682b954999a342d531  :sparkles: Refactor multiline yaml const
20756a838f1ece80c7bca913d7a591d17a7c0037 Merge pull request #4499 from stmcginnis/no-docker-testing
9154e6e5865ca6062739cc849616484b2ac1b5a7 Merge pull request #4815 from vincepri/kcp-node-drain-move-mt
9633b3039978edbc7eabdeba165a9d8a8786ae57 Merge pull request #4813 from fabiand/patch-1
8e63984b9fcf8b01ec0229a5d011b66f8a8372b9 :warning: Move NodeDrainTimeout under MachineTemplate spec
642108699f7f6c0c6795451243b0bfdcf7b62061 providers.md: Make API Adopters more explicitly
bb194afc75aafe2464163928080c0a7b25ea046b Add context to docker operation errors
e0ced24598da02d8d64d93da71acbf86fd6a7e32 Use docker API instead of CLI in test framework
19b900defb84434e3a23d786c311c5daf9d94d6d Merge pull request #4798 from Ankitasw/add-ntp-mutation
4957345745c9947d0cabda4053ae671aff0fff05 Merge pull request #4787 from vincepri/correct-machine-provisioned-phase
5dc521db2e461086810348cb65df7a594af630c5 Merge pull request #4806 from vincepri/improve-book-readability
854fe4adb761fdc6dc7f24a27809ee2397ca135a Machine status.phase should be provisioned when there is a ProviderID
899870387d35ec83efe30ce957379fec6f048dd2 :seedling: Improve book readability, fix bug with tabs in quick start
b8aa173c367460e7b108366bf3d7fcc03e4933a9 Merge pull request #4800 from vincepri/update-book-css
525d63cee220db6ac5191f942979679ab4665bea Merge pull request #4801 from vincepri/update-owners
fbcbcc7273e7d9b7a2c35d5064bd81a670dc171e Merge pull request #4804 from sbueringer/pr-cleanup-golangci-yml
1d07d6a93abf31000ba6d80cb301c4d54a37c76f deduplicate linters, move exclude to exclude-rules
0987bf12b61d40e0ff2b5e9541a75f2d8be115e2 Merge pull request #4792 from christopherhein/clusterctl/capn-setup
7027a1b55bbd2c8cf968c3c37aee2808b2ec6e7a ✨ adding CAPN clusterctl
bcdff653408cdea3f470de7805c3fb7730409017 Merge pull request #4796 from fenglixa/fix-make-release-notes
6290fbddfe7840362b1f5e7ce807433e8e629a5c Merge pull request #4797 from sbueringer/pr-improve-migration-doc-part-3
b70fff868ba97e3ebcb72347c7c979cf27c75b54 :seedling: Update OWNER files to be more up-to-date
e47f590dcee2263dd3db15ac2e65447b05e1183b :seedling: Update book css to latest
aa4268129c1af227031326a8dc949bfd57f80000 add ntp settings as mutable in kubeadm webhook validation
ebaeee3f396bf5d2aed9c16eabb5dcae536ce5d3 update v1alpha4 migration documentation
9bca9e4205c6287b29c3697623952994a438d0eb Merge pull request #4781 from vincepri/update-release-guidelines
878d751e8f18bfd74daa24d5b80ddbb4193ed33e Merge pull request #4793 from christopherhein/feature/add-capn-to-glossary
81cb1078effd776a5aa4a3d11f793129e01e7297 Merge pull request #4789 from sbueringer/pr-improve-migration-doc-part-2
572a944008af2beede1f9cf95fbf6fa4372e9ace Fix the issue of make release-notes
a4c18c0b92f06d0d2339b0922bfb731f81fa9fe6 ¨✨ Add CAPN to glossary & clusterctl provider
5bd7903c5af1db352e34d67dbe628871c566a9cb update v1alpha4 migration documentation
565391725a60f739dffd27b211910cdaa970e595 Merge pull request #4783 from vincepri/update-mdbook-0410
252ab79973542e4f8487898b118177dca035a2eb Merge pull request #4782 from sbueringer/pr-improve-migration-doc
756256fb06f4b28ccca8057293f9b5518f04b6c8 Merge pull request #4788 from vincepri/update-readme-2
db6e21ea3b2b6b2bcd35eac6215bf56802b40163 :book: Update README for a more up-to-date view
5daa7eec4fd93a3b361ee872f1244954c714c378 Rename ListVariableOnly flag in TemplateInput
85e890d3969b19964c28e85ef6782f77c6d91b18 :seedling: Update mdbook to v0.4.10
709542f42c348160a1b4b22564e899fab857a4a9 update v1alpha4 migration documentation
45a0abb58cf1bcd65c9b35b0f7e189ac2cae6f0a Merge pull request #4652 from enxebre/hasMatchingLabels
e113d8b6e11acdd8cad97b87457629426fe0a925 :book: Add note that test/ tag must never be annotated
798007a1046b9ff55d1b3d7990cd12d6a4c8d35b Merge pull request #4780 from vincepri/enable-lint-test
01fb233f9aa19f22891594913c81774856b602f6 :seedling: Enable golanci-lint for test/ submodule
9ad4ea8a21b8d663e2786590445c13759ea842c1 Reuse hasMatchingLabels
1a539da6e12c842c2f73e6a23a52d5a0588e4ab9 Merge pull request #4778 from fabriziopandini/update-book-for-clusterctl-generate-cluster
15e72d4a3443ab47699022f6c6f908f0669ede7e update book for using clusterctl generate cluster
e970639fd4cb56003039878e82ffbc0b2e950a9e Merge pull request #4775 from vincepri/bug-makefile-go-version
c6c82ef0a3464dee3161ad8d81d762767f087b75 :bug: Makefile should reference the correct Go version var
f13f7bcdda5157fcc8fef2566d258624bd136a34 Merge pull request #4774 from chewong/unmarshal-to-pointer
c6a6c2c7b97dbe247778490858b96c19ec246330 🐛 unmarshal data to a pointer when parsing kubetest config
027f39e362cc775a6b6506e03427e426c77479ee Merge pull request #4771 from ykakarap/builder_args
0792a6068376ba10b0cf7d0bb685c96859f57d7c Merge pull request #4772 from vincepri/fix-readme
21ce645b1cba44c985f439b877aabb7c6c010d0c Merge pull request #4768 from fabriziopandini/add-raw-flag-to-generate-provider
a31425b3c576d410d461695eff2e27d563b96ef9 add build arg to override builder image
33934b449ddcba032f1e54f2d70e19bffec321c1 Merge pull request #4773 from fabriziopandini/update-instructions-for-rbac-proxy-removal
af87a1f16a24964d5902eedd5a2bc55f9419e6c6 update instructions for rbac-proxy removal
25006fca1daa5c670ace6cde3b3a0a2d48bf03ce Merge pull request #4748 from fabriziopandini/remove-embedded-cert-manager
a6de0a3a02aae09d181a82b97c0bff0a66ee17c8 :book: Update our README for more friendliness 🤗
de99c22bf37e38508253cd0a5b03f7dafbb0d198 Merge pull request #4640 from micahhausler/remove-kube-rbac-proxy
29d739ca499661215a16df485e6435fd9f942820 Merge pull request #4751 from fabriziopandini/align-v1beta3-types
477fd77ea81b727d82cf25889ff4564676cb4f87 Make clusterctl support for cert-manager more flexible
ab68ffa48820fe6c2ed9102aa603cd7973ca2f8c Merge pull request #4722 from ykakarap/index-machine
7857dd2bae01d2311dbf862c8e171079c3bd1f09 Merge pull request #4770 from randomvariable/smol-bean-etcd-note
6a1b5a552e2b6783967d33189ee08d8633af5409 Move registering field indexes to the noderefutil package
9e0c489a39389d9d71a018998b69c0cea5abd51f Merge pull request #4758 from enxebre/unify-ClientUncachedObjects-name
c39f3569e1e8d4da0b821973f1f2c11ed7231b77 go.mod: Add comment about etcd versioning
b82cdab0ecc3b8a538dd5960e14e66de1233d1e6 Use ClientUncachedObjects name consistently
786375f4c1f8e60ef08e7d01460b22acbca0f46e Merge pull request #4757 from sedefsavas/crs-timeout
29cc0560be76112e0f98c6b5db47d086033aca2d Merge pull request #4750 from ykakarap/set-useragent
e1387aa51d625144fe485b971723d99a7145b3a0 Merge pull request #4746 from randomvariable/2021-06-07-dependency-update
ff43603648aeba6c8a139a4d59b1f1bcde58aa5b Add --raw flag for clusterctl generate provider subcommand
882339b37c66af75543b8a646b0b283066c245f1 Update dependencies
773eac1063665becfc4e4341406d095cfae35826 🌱 Update controller-tools to v0.6.0 (#4764)
8d81b09f188cac86f0aba78068281699ee58fb17 prefix user agent with "cluster-api-"
154cbfa81de1567c8002c36918e2fcb39b721101 Merge pull request #4765 from CecileRobertMichon/provider-go-mod-test
67b6251052a743a584463d4fe0236ff581385d47 Make envtest to accept list of objects to be read from live client
10f1e486491396790bb6275c914cf35e5763682d :book: Add replace instructions to v1alpha4 provider doc
19d791f38b2977f39b3ebd84b6bbac8812660c65 Merge pull request #4761 from randomvariable/remove-kubetest-viper
2c7a4f3ef5cfae89342858eacf23dfb1d9450e21 Merge pull request #4752 from vincepri/cr090
8445e16aa41e6dc5183ba5dcca208828dd175bab kubetest: Remove usage of Viper, converting config files to kubetest arguments
2da7fe0fdec47b9119f017ccf6cb7e30710e0021 :warning: Update Controller Runtime to v0.9.0
aedeb168a793cb3a0a1acaf3b6ee46026e492646 Align v1beta3 types to latest changes in Kubernetes
bf66e6ccc015ee383dc42286f9920c9905f5b208 Set the UserAgent in controllers
55f064d1b9fcf3f0a7b1a32e43559bdff4d3c2cb Merge pull request #4038 from tcordeu/bootstrap_cluster_logs
386a8522cf3df6ab28eaf499009c37fce988fd4b Merge pull request #4719 from shysank/control_plane_decouple_wait
7f15ab946385c85376c6f978695763f12d91b8b1 decouple control plane status check logic for customization
369c3cac12936aad211477a20acb40b0bcbbdc36 Merge pull request #4726 from fabriziopandini/introduce-ClusterctlCoreLabelInventoryValue-const
a8904d7cd277c0ec110c2f1fde930f7c7c1dea0d Merge pull request #4744 from randomvariable/dependabot-no-gomod-prs
503cc5560a15cc45d78ff20eb03032c0782f278c Merge pull request #4733 from kubernetes-sigs/dependabot/docker/test/infrastructure/docker/golang-1.16.5
64524eede39d4b65e1c5fd9179698a3d4dab06b4 Merge pull request #4725 from fabriziopandini/introduce-CertManagerImageComponent-const
61474ff4f8d7271d043962acad3212a8430b1287 Merge pull request #4724 from enxebre/use-secret-defaultmode
3f6326f966431259ec0af28e7bb5070418370dbe Merge pull request #4723 from sedefsavas/secret-predicates
f45787fd261dd2b2ea6b55835590fbd724faa084 dependabot: Disable automatic PRs for gomod
24643c7c185024e400aaae57e1838153457b9640 Merge pull request #4735 from vincepri/add-dependabot-prefix
d6316ddf1bc95fc71b2b559ebc708e7ca2b912cf Bump golang from 1.16.4 to 1.16.5 in /test/infrastructure/docker
246c3e26b6dca05ed41268abbe1644f011969500 Merge pull request #4732 from kubernetes-sigs/dependabot/docker/golang-1.16.5
6687e835fc0f7c208faa0bc8ac1af585637f1ed6 :seedling: Add dependabot prefix to commits and PRs
17a4d536554f111af093c533f117ebd112eb3e0b Bump golang from 1.16.4 to 1.16.5
0f7548541107649774421caa87b7a1c2b13f0f6c Merge pull request #4730 from randomvariable/dependabot-config
f2da39d0bacdf2396c07bf34938d8d0a1e5829b4 Introduce const for ClusterctlCoreLabel inventory value
303483aeea393e066d69e8c3757326c37c7a3ff3 Remove kube-rbac-proxy from cluster-api
40bc05baa24a6e6e6f85a650b6947143129468e3 Add dependabot configuration
a298eb1b48503c94f7cfeca6c14f09d93d282663 Merge pull request #4717 from randomvariable/linux-kernel-kube-proxy
5b6d89600915e9bc6c283eeaa406f36fb50a7e1a Collect bootstrap cluster logs in E2E test
26c9d4175cd9f787668764836d6ade454ea5787f Introduce const for CertManagerImageComponent
e29ffc2576cb9940c36e4bf75cb6d7da6e19598b Merge pull request #4693 from ykakarap/expose_uncache_option_tracker
1fe22fce31556dc59f851a10bdac5f87cbe02edc accept options in remote.NewClusterCacheTracker
578429eb1f0097ba17282716ea9ade6a6a1da6b7 Fix for Linux security update https://github.com/torvalds/linux/commit/671c54ea8c7ff47bd88444f3fffb65bf9799ce43
e965ade2269b4884dc5498788e9ff165f249dc98 ClusterResourceSet: use generic predicates for secrets and check secret type in controller
b64c41c4ad655f03883e290ef5d7e443db39d152 Merge pull request #4682 from rumshenoy/docs
95e9d0d22b884e27de151f64f144cf967736e772 Drop 420 dec default for secrets
02e88ac4244b19af33f806a397aa4efbd55da10f Merge pull request #4721 from vincepri/cr090b6-2
1f79d487a980eb3e36e6564aec1bc82a8022dce4 Minor improvements to Cluster Api book
0591d309c493a0d34f8ae73c4781ee59297787cb :seedling: Update controller-runtime and ginkgo dependencies
61e63e0dbbe50a276174826aaf1bcc9847ebc3a5 Merge pull request #4297 from fabriziopandini/adapt-clusterctl-to-new-manifests
9fe5c4900e173abec09e89cfed63c09cf8052f13 Adapt clusterctl to webhook deployed with managers
ded3b90e3a2f4bb9b816708eb79fac40432dfb37 Merge pull request #4628 from fabriziopandini/clusterctl-move-multi-tenancy
0a261ed58e7cadc37d8f21df010df76c95736f23 Merge pull request #4718 from vincepri/go-mod-test-tilt-enable
4f56d8fafccd971b0a2d608350f21f562a80b785 Merge pull request #4706 from fabriziopandini/fix-e2e-context
70e959802aa7722efefe69158e868d7ff3eec4be Merge pull request #4649 from stmcginnis/exportloopref
7a5fe58fe8bd91b4a447c7165fffec5766fd31fd Merge pull request #4716 from fabriziopandini/fix-TestUpdateCoreDNS-flakes
546d5f869f4f48c88ea5e2e5f2f3d7574248152f :seedling: Fix Tilt live reload for CAPD provider
2415db440b0fae4f66d5104c6ad72c8aa8ac2d52 Merge pull request #4713 from vincepri/go-module-test
c6e62d259f1b841326850996230ca9057923c5bc :warning: Introduce the sigs.k8s.io/cluster-api/test Go Module
593f1c993982e0d2732ebfc52cb7d5d48b43cea1 fix e2e tests using a single context object
dfeb2c5bb1d6fc1615ac979b2c7c469a4c1b6e9b fix TestUpdateCoreDNS flakes
40841d9837b825a3d080bcf6683ac3a58277c286 Merge pull request #4715 from vincepri/cr090b6
d0ce23a99ad5e19d82db00b242d054c8bdbde8c0 Update Controller Runtime to v0.9.0-beta.6
cd3a694deac89d5ebeb888307deaa61487207aa0 Merge pull request #4704 from Madhur97/capi
53b581e7de87484b38b313c9d048da62f23bcbab Merge pull request #4710 from ykakarap/unit-test-coverage-cloudinit
f7218358759a5c926e4e28595348928b24513e77 add unit tests to NewJoinControlPlane
ea0bd3c91ad3f122220dcc3a721ae208a9c46c84 Tune ifshort linter max-decl-chars
5afb4832c45b747701db39e746b21b3965f7c029 Merge pull request #4708 from fabriziopandini/improve-clusterctl-list-variables
5310648cc15c5170c207eaf4a245e1634aad674c Enable nilerr lint checker
f9d608c8dc22dab4e97f58bf8abdbcc0ea6907b1 Enable exportloopref and ifshort linters
356dee9b4a1ac7dbb0ce22274a7ab6205b31cd79 :book: CRS API does not allow empty selectors
4042f3779aaf6fa5db4808d75dcbefc1225aa53d improve clusterctl generate cluster --list-variables
88b3ee3e1ac58440bc450126922a723cbc86f7ac clusterctl move should consider Secrets from provider's namespace
df2ab2f54e863124dde1fddca19694d3ab8190b1 Merge pull request #4598 from fabriziopandini/clusterctl-move-infrastructure-secrets
c4bf2e7b5f5f59a9f0cf61fe4c3b70d90e9112a4 clusterctl move should consider Secrets from provider's namespace
a74b6a6428cb89c1ba0866e86c292734f85eb350 Merge pull request #4698 from vincepri/move-envtest-internal
aa049f15e75d3ac715c2a1a1e58d34fa77280eef :warning: Move envtest setup under internal/envtest
c9f1dace00aef9b220ca38685e5be6c4be3334f7 Merge pull request #4691 from shysank/kubeadm_v1beta3
8e7d77421c39785ee771fd53595774fe41b83973 Merge pull request #4700 from vincepri/golangci-lint-download
9f4a6083cdf86bab7b8f0e3ac63523d4967a7269 Merge pull request #4694 from fabriziopandini/deprecate-Provider.WatchedNamespace
4860e700931dd0197658d8273071abe20ceedcc5 Merge pull request #4701 from CecileRobertMichon/e2e-pointers
e322150d9ffc72c72b011a776fff91bb40856b9c :seedling: Download golangci-lint instead of building it
8a62f7e67cece84090893132b2007b1e734be703 Merge pull request #4647 from jackfrancis/e2e-machinedeployment-scale
002735ae5a37b07a87731f401dd6c3c00a5edd5b :seedling: Fix E2E log statements printing pointers
f555207f263a7b085dfad659104b9a0ace293e28 Merge pull request #4699 from vincepri/go1164
376dca06eb95ff03f4b156772588761b45c2f80d :seedling: Update Go to 1.16.4
58cdbedccfabf3804eabb64037c138467400e7d4 Merge pull request #4697 from vincepri/golint-update
c9e08a610208a93559d5f46cf7bb6b70ffa42cdf Merge pull request #4696 from fabriziopandini/rename-inventory.GetDefault-methods
12c7339bab9481dd5792740fdf29accf7173fe95 Merge pull request #4686 from ykakarap/add_readme_bootstrap_kubeadm
70ee1bec1daa74554415e810b3f91ca64c82974c Merge pull request #4695 from fabriziopandini/more-watchingnamespace-cleanups
0fb33bc44d66a095ef5bffbc8aca7d056bc818e2 :seedling: Update golangci-lint to v1.40.1, enable importas and revive
fd9a33cbc14da9cd79def602f73f47f99b55c7b0 Rename inventory.GetDefault methods
40ec4b11e1c4a415ee173abfc77a35ff195c013f More watchingnamespace cleanups
429e26c839b33632c093117f8cb2ef9bd7ad1b98 Deprecate Provider.WatchedNamespace
2bed3c331abc681ba4d058d96bca51004f2fe3eb Merge pull request #4690 from vincepri/deprecate-newfakeclient
b091ad362da01a863ca38f67564c1ad0cb0fdfa3 :warning: Remove test/helpers.NewFakeClientWithScheme
2e4deb4e6c202ce4c9ca85df6996b0545f4fccce Merge pull request #4689 from vincepri/fix-scheme
f84d114b9b392d583059f2da9f8fd3c1127c439a Merge pull request #4683 from tcordeu/e2e_separate_kcp_scale_in
72ee11af1bec2e9dcd3fb22cba3f718839658d89 Merge pull request #4645 from mboersma/clusterctl-required-vars
bc07b939f9a1917223f184db702aa97e12094be7 update kubernetes to kubeadm version parsing to include v1beta3
75a97124baa00d849e3bb1ecfddb917bd79b31d4 Divide KCPUpgrade E2E test suite
24ea203fa4ba03496d977bbbd3a60f97bbe5b3d2 Merge pull request #4668 from fabriziopandini/remove-clusterctl-management-groups
3659f228e889da9a3f4d6867614b7476655da6f9 Merge pull request #4692 from vincepri/eventually-condition-assert
f88947bbc6a32996c18ca717970a128ddf290579 update types to satisfy cluster api linter
efe4efd1f5129e7632b75b741ee702a2acd7244e add kubeadm v1beta3 types
f10c947c570a959724ef3a693a239292d6a2893c Merge pull request #4688 from vincepri/fix-conversion-tests
93a6e9a6f9e05113b7a9a993fee6801f9c325de3 :bug: Assertion of Machine condition should be in an Eventually
3f6f5434deff9006901289dbc15cf8407e3179be :bug: Use unstructured for conversion utils tests, and fix how we set annotations
29333cd0802cf7bec32b57455c19262ab3d7b5b0 :seedling: Use client-go global scheme as much as possible
dac8d41df9ee1b3f105b9e226f57259f8d8c29a4 test: add MachineDeployment scale test
364de39e643a8b7625f24fd64c7f794dbfa06980 update kubeadm-bootstrap doc and add to book index
0e1629b751119108de2f20cdd49da43bc4fa1e93 Merge pull request #4653 from enxebre/add-enxebre-reviewers
5b7cf36173d1eef96eb090821485344646260ee4 Merge pull request #4680 from mboersma/update-cert-man-ext
60b7ea43e9d6caba6705064b6b02519df2b7385a Update cert_manager tilt extension to fix startup bug
0ec3c310f62060ccdcf154180eb893bda6af695d Merge pull request #4677 from fabriziopandini/fix-TestReconcileEtcdMembers-flakes
adc8ff1ebb0900f83c50ad02465d16ed4ec6d0c0 fix TestReconcileEtcdMembers flakes
afe3533bd0ffe6d5250b61e96af585344aacadb1 Merge pull request #4674 from fabriziopandini/remove-clusterctl-delete-namespaces
0599f3fc2f61822a69c56c24617fee9c681c5305 remove clusterctl delete --namespace flag
3dd54cf749b62a6737fc87573eb0ea208bb7689a Merge pull request #4664 from sbueringer/pr-migration-doc-linter-fix
f1834fafae216719c5a541098f7e475487e01d79 Merge pull request #4643 from fabriziopandini/stop-updating-ClusterStatus-for-KubernetesVersionGTE-v1.22.0-v1alpha4
cdd8b2900f3b09d4a31bb340b001365d25bee4c7 Show required and defaults in "clusterctl config cluster <name> --list-variables"
6c7878e7b4a9c402e63f6d3317f595b559625a0e Merge pull request #4670 from jackfrancis/machinedeployment-version
502e4ba5d92d1016cb6eba00e9d3fd95fb1450ea normalize MachineDeployment version validation
40e737bd26565977e28f8b0fe548e0fea7d9ac57 Stop updating ClusterStatus for KubernetesVersion >= v1.22.0
c6803793164abe26b61dae2f1b9b375d4acbecf9 Merge pull request #4669 from vincepri/enfoce-golint-comments
7fa478e42df87b3d603ed932207fd0b1b6cb7b57 Merge pull request #4663 from sbueringer/pr-upgrade-kindest-images
2d0a5f063e2fadba106cc91f1a21eaec1d8c0101 Merge pull request #4648 from schrej/fix/capd-btrfs
511afc8cd6bcb44fdcfa682da2cef588abe047d9 Merge pull request #4626 from sbueringer/caas/sbuerin/doc-local-e2e-test-execution
6db0dc843fc1f94776b4c0f9f235b0a87a524d14 :warning: Enforce comments on most of the codebase
3c673999e2b7b6bfecc8a14e47315bb9b524fe3a Merge pull request #4666 from fabriziopandini/remove-clusterctl-watching-namespace
aba35d72b2adf31764c1d13d1c5e67e943878226 Remove clusterctl management groups
0d4903ff4dc62a4edf1c11ab14454b47d86bc569 Remove clusterctl --watching-namespace
fa1cee57595ace32cbd7900ad73cfb74737b2bfa Merge pull request #4661 from chymy/fix-book-link
ff6a70df124571f030e68d89fc6f0c0a152bb1bf doc: add local e2e test execution documentation
d2813d0a22140a7f49e93f2ba00406f790f2249e Merge pull request #4662 from wilsonehusin/conformance-entrypoint
76af959cc00e43e820ba542184d17121a8213031 doc: add linter fix hint to migration doc
79e54d54964223ba174d402d304d0b9f1943bb06 upgrade 1.18/1.19 kindest/node images to latest patch version
3aa8d27415faaf743d1988fdcc376b87c12f5581 Invoke ginkgo in kubetest through entrypoint
620355864d0212388c5dad9f42e323d4c9753273 Fix quick-start link err
fca52981fe0afcca91a0e014a444f703d83c64fc Merge pull request #4657 from vincepri/golangci-refactor
af33e43d891e3af3787e86bceabce6b8e052c984 ⚠️ Refactor golangci-lint config to remove false negatives
d6b962ca6817dc261904c5b9a2b0e76211c62973 Merge pull request #4469 from sbueringer/pr-upgrade-kind
6bb92efb8046ea4a5a9d0670339ecf65558b37df upgrade to kind v0.11.0
2b60ccdb716815ef1a44ed33308c8f777f2df105 Merge pull request #4575 from CecileRobertMichon/machinepool-logs
9d1b97f2e8862cb2803a60c0f9469868c2f72235 Add enxebre as reviewer
04c2635950ac02dabe08b9b656411e461fb97d1e Merge pull request #4644 from vincepri/kcp-metadata
9acee8cd174a77f8a3f2406d7f6caa7ffc4713e9 Merge pull request #4646 from CecileRobertMichon/kcp-delete-mp
fa24ccdee83d4ce1fa3b1848748e9c42a500b683 capd: add support for btrfs and zfs
634a2d7ab3562bc91ee48d1462576471f00e6011 Merge pull request #4584 from shysank/clusterctl_generate_part1
aee107b158d0bbf33a0fdead31576d6fa56129de Merge pull request #4630 from Daimler/bootstrap/cloudinit-duplicate-files
3e9c84e9eaf49d9fe2e80acb918d07ec9352ddc0 bootstrap: prevent duplicated files in cloudinit on cloudinit.NewNode
180fd36c33c392ab8462e5c6157dedacb30e9e79 :bug: Wait for MachinePools to be deleted before deleting KCP Machines
5f500693a98f1d1b2559cf2781830f5bc647dc35 Fix MachinePool upgrade e2e test
322608e3fdaf5b1241badb4efc6b4e305705ea58 Add MachinePool to e2e framework log collector
b535ff15fd1de2675d7095bf7007f71a66c093fd deprecate config cluster and provider subcommands
95f428eedf96aec466caede9ade343a95e03149f KubeadmControlPlane: Support metadata for machines and propagate to all templates
bcab8bc3004dc75450cd0283d4eb6a2c3fb14c66 Update generated files
b654ac7ab462a62a048ac680485a70fcc209b73b Update module dependencies
58583914ed0034203ee398f864b5e023b2ed65e2 Merge pull request #4631 from stmcginnis/enable-golinters
36dd674c5b0c288454738e9579aad67b7563859c Enforce package docstring format linting
6e85f962dec310d64af67be78c4c0f6771fc06fa Enable package and exported function comment linting
f5dec18def709194f81a6106943ad80a88e8b4e5 Merge pull request #4638 from vincepri/cr090b4
493fb803994db8264de8d813d1c9df5db663e6ef :seedling: Update controller runtime to v0.9.0-beta.5
a10e659865c4a893619966e9f3e4dc5aedcd5367 Merge pull request #4574 from CecileRobertMichon/new-mp-group
72d1a4ca16fd3bdeaec31bc61a16937c15b28572 add generate cluster and provider subcommands
8780d1da76da31e9047fafba66661cf8b019d7ec Merge pull request #4637 from vincepri/remove-kcp-hash-unused
7db4e3af9bfa87f99da18a75a994381f29ebf357 :seedling: Remove KCP internal/hash unused package
06f58a66353d5a22a2849f2f516ee71e4664c323 Merge pull request #4471 from JoelSpeed/disable-node-startup-timeout
2be6be2ade895dce4d48fb4f2cca48b686149293 Allow users to disable MHC NodeStartupTimeout
e7fb8eee37c7fcf3f0dec51331c7ca16095f5313 Merge pull request #4606 from chymy/cleanup-unused-var
9d8bcf141feb8a5e6f426ea90505d6cdd37701dc :warning: Change MachinePool experiment API group to cluster.x-k8s.io
e46cde9001d95e7145d89e0b24bff8e18ee55430 Fix CAPD machine-pool.yaml example
18b2741ac70ac5f2da29dbf3eeba545d0431f454 Merge pull request #4607 from chymy/fix-comment-0513
9a69d3b2861e8de41fda227d01a852f868365b33 Merge pull request #4627 from sbueringer/pr-add-troubleshooting-doc
36bae1a67d6464aa7a7475e43c7c457188576cae doc: add node bootstrap troubleshooting doc
b398cb884a5b60055f4c56c9a3a2323bb2ae7995 Merge pull request #4615 from mboersma/go-test-controllers
a78914c9357a85e4bb26259e82cf9825f7f0f683 Merge pull request #4624 from stmcginnis/enablelinting
97f658d189958cc468f5dcdc0fb5ca1ec495e0b7 Merge pull request #4579 from mshitrit/tidy
02f7225a240d1e7952bf6316c0dc091a8422d31b Merge pull request #4513 from enxebre/node-to-machine
82fdab42d0ae0a8e4efa293d6800f2e369c419f2 Merge pull request #4558 from mcwumbly/capd-ipv6
54c0d307a5f0a4edf3c3f93b31a5907281c194cb Add ipv6 support to capd
6a24e15c523d083739e2d605249457c212f92a33 Enable excluded lint checks
34a649353afa630dec379d69497909cd07257fc1 🌱 Refactor tests to plain go in controllers
4026985b65c02c078219b729e3c0e9e6c88f96bd Merge pull request #4616 from mboersma/go-test-controlplane-kubeadm-controllers
e040daee068b87e000068bb01a04beff73aad15f Merge pull request #4612 from mboersma/go-test-controllers-remote
799da053dfc87e4cb82a0133d5390f2b0c3f1619 Merge pull request #4614 from sbueringer/pr-capd-pin-cgroupfs
972c45c60328e55a16bdddf6887415c7df1cf61f test/e2e: pin cgroupDriver to cgroupfs
def0fa807ebcfdd285ed63a95cee090509a7ed24 Merge pull request #4568 from schrej/feature/4543
b5ffb8bbb87dadbf5dd4ad2795c51426dbb98dc4 Fix comment issue in controlplane/kubeadm/internal/etcd/etcd.go
59fa9490cc9a780694b9ca3f99ba000bc8de4d3d Merge pull request #4602 from mboersma/go-test-exp-addons-controllers
647a956332cbcf10eced029ec8ee3fd1007c6c53 🌱 Refactor tests to plain go in controlplane/kubeadm/controllers
05d78d141779e3a43e7c917ab801154c2d6844e8 Merge pull request #4604 from chymy/fix-redundant-judge
011dd9fd6cc6e65c9d08b5e57d81b64852b162f5 🌱 Refactor tests to plain go in exp/addons/controllers
8bd4c500e56bb6d52edd0390cdc8c55e1d55d624 Merge pull request #4613 from vincepri/backoff-kubeadmconfigmap
f8971c97b232ed1bcd2de0ae23551a59648a9d21 :seedling: KCP should use some backoff when updating kubeadm configmap
e39f6f374c693766e4161e39e85fa08c31afb225 Merge pull request #4603 from mboersma/go-test-bootstrap-kubeadm-controllers
c849885aebd5f7c48403abb51a25ed7a2c15ecf6 Cleanup unused variable
13ff486a894d0a82f9cd650c24caa3bcc35f6815 Remove redundant judgment condition in controlplane/kubeadm/internal/workload_cluster_coredns_test.go
5252e7ae7321b7aebe6097834e7df5a12b6076cb 🌱 Refactor tests to plain go in controllers/remote
ef06802c35179bb21206555d76222509ccce7848 Merge pull request #4599 from mboersma/go-test-util-patch
93ee29cd8a54e452f04d15c7a82e9fb07afb6006 Merge pull request #3708 from fabriziopandini/clusterctl-upgrade-e2e-test
87803d514c45f4f0d0977ae7a530357368b7fee7 🌱 Refactor tests to plain go in bootstrap/kubeadm/controllers
7720994f80793c543064cc17a48c0103ce7f0d51 Merge pull request #4601 from mboersma/go-test-exp-controllers
cdae7ac6ef1e2ae71657e0f08a245e5c04dc136e Extend MachineSet controller tests
f24d2e5665bc1b4fe380e06f1d1f15a57c184680 🌱 Refactor tests to plain go in exp/controllers
d2faf482116114c4075da1390d905742e524ff89 Initialize gomega locally to each t.Run()
3a2f7c7c38ce289fe50b1bd12a8b32fd646834c5 Merge pull request #4600 from chymy/fix-anchor
a2b976d8e11504f2751bbe5874fbd950831e6b5b Merge pull request #4597 from mboersma/go-test-util-collections
4f5ea4c1934dedfd2482a00c543c89905e255433 fix anchor err in 20190610-machine-states-preboot-bootstrapping.md
ae8da03a74b3e1365ba679e779ac6efe3f5d60cd Tidy: fixed typo, unexported methods and removed unused func variable
529c457241eee8b15f413e714df564ff7549d845 Silence linter by removing blank line
0ff3320d4d55b9f60616659e018dffef7e241cfb 🌱 Refactor tests to plain go in util/patch
959494d40b4b9e8221b22b2747b9a0b02b6d1c07 Nest t.Run statements to show context
6043ec18780b0f62669ac3e0477e42d2e8ea683d Updated based on review feedback
96dfa93681976738952f2beae96d6d5e662f0525 🌱 Refactor tests to plain go in util/collections
321ec3976b18200742b4ddb5b706e28b5d5657a7 Merge pull request #4443 from fabriziopandini/use-cluster-API-owned-kubeadm-types-in-KCP
5c19ea1f6099e68539146aa40a7631bda618c6c1 Make KCP using embedded kubeadm types while manipulating the kubeadm-config ConfigMap
61d8ca86e0f2d4c61c8b23db1f576f231807f5bb Add ability for nodeToMachines to filter by clusterName and namespace
6c8b2dc2534bd37fbfc7d0889cf8d7e4faf33c19 Merge pull request #4594 from fabriziopandini/KCP-remediation-2CP
61ecf3d93fab880833213a17aa8c5454026be356 KCP remediation for 2CP
2c9a6f341d8dfb6b8a87c1c42d425835cfc8e929 Merge pull request #4592 from vincepri/add-link-doc
02600257261a976422af5ce05bb0491e506e32a0 :book: Add v1alpha3 to v1alpha4 migration guide to the book summary
81daee59acd6e9fad4dc14f9844ca83e7023aa92 Merge pull request #4561 from fabriziopandini/KCP-remediation-fix
a925feb87650af4ea17b50d83815ff4010dafb95 Merge pull request #4219 from randomvariable/node-attestation-caep
c07e9b3dd6425ef32a9981645e80cee72b76231f Merge pull request #4564 from fabriziopandini/Improve-KCP-conditions
d79e38054e94faa3c6504e007f63eedbc79403ec Improve KCP conditions when node status in unknown
ce15591b737ec5cae8384c6267e250d0fc2f13a7 Merge pull request #4506 from enxebre/refactor-scaleMachineSet
2a6e55dddc7c9fc16515b4544f511abfa6327413 address comments
d65730c04fda8aee594e3a80084b4f8c998d9c94 Adds node attestation proposal
6dda08f83614ae589da3802b40cdce2b6f09a1f5 Merge pull request #4576 from chymy/fix-typo-0506
47269217ef5c7c8695f241ee5f2dd05321a4edcb Fix typo in docs/proposals
56f4f9a6df5d383265485b4442d80b9cd0c7fbaf Merge pull request #4570 from fabriziopandini/fix-clusterctl-config-cluster-regression
bb2fbfe31f6c733901927dcf50cadaadb8f6fe79 add clusterctl upgrades E2E tests
b0c00ff593db4dc2f545b26b542de1e93063bb60 fix clusterctl config cluster regression
ff489c82c229bb2a616fe3dab61999861ed52904 Merge pull request #4498 from enxebre/unit-test-md-rolling-reconcileOldMachineSets
1d15a5b7cadf5c5ddb3964be3482ee57c52e1832 Merge pull request #4517 from sbueringer/pr-ease-local-e2e-test-execution
b876bd214393dad6830d6680fdab1dbee0d7f133 Merge pull request #4573 from vincepri/cr090b1
36cff637b6774397a73a604575920589b0651c5f Update Controller Runtime to v0.9.0-beta.1
3065a926259f682f65cb8331b5f2543b270882a8 Merge pull request #4303 from JoelSpeed/external-cluster-infra
6424396845d0c40193931f74d5fc75917f0fbe3c Merge pull request #4417 from prksu/fix-webhook-conversion
44a4d428f2551092bcfd73660e1f1d4b5e557ca6 Add externally managed annotation and predicate
8129ca55d5a4dd9022e04c8435a792dbeacca301 Merge pull request #4567 from davidewatson/macOS_doc
f9db369d742747ea9791b44450b7b4be94662a09 Add annotation support to util.CloneTemplate
d1d2524ffce2aed3b2552640c738c27bbe475cc6 Make a concrete recommedation and don't hide under a tab.
b13ce3e3819fbef2855e252ae2ae7356835b4fa3 :book: :seedling: Note macOS may need more memory.
b4369266a3ba78888e48f486f2a2dc8dbe372531 Merge pull request #4500 from sftim/20210420_book_introduction_tweak
7766ac50d4d3ca81fffa61957bbf014ee75a8f63 address comments
befae8ed558e24bfbd9cc20d671ff8befd161098 Allow KCP remediation when the etcd member being remediated is missing
402a4524f00671eabe6441c71d749dfe258bc43f Merge pull request #4532 from enxebre/use-GetScaledValueFromIntOrPercent
45b6080c276453c2f30fae3e093679a15c7ccdfd Merge pull request #4553 from fabriziopandini/allow-clusterctl-config-on-empty-clusters
54adb43f9c6524993364839c73ba533ab6c9dd6f Ease local CAPD e2e test execution
fd78c9023be18a3291a53af164f0d308612d0626 Allow clusterctl config --from on empty clusters
4afa5400293f0c2548f2ffa5994843d4871d5058 Merge pull request #4550 from chymy/fix-html-tag
7ce39a03b5754cc160927dd6e2fadf10e2dca36d Merge pull request #4551 from chymy/fix-misspelling
cef11ded1f802e3f28912a80ab383c55e3b5c98b Fix spelling errors in some docs files
521f9e4af72c0e196998ed398528901f061d1940 Fix html tag issue in developer/architecture/controllers/control-plane.md
4a73373f293ff798a635f8f07566632fde418c5f Merge pull request #4549 from sbueringer/pr-rename-upgrade-rollout-after-fixup
3c791ddb1b2af4ee34dc60742bb8a16e87d00442 Fix  KubeadmControlPlane conversion upgradeAfter <=> rolloutAfter
355cc78742d47e6fdab2e67136124385088c7516 Merge pull request #4547 from ludusrusso/issues/4546
f8816f8d60ff4a93fea356d317d8d43de225cf87 Merge pull request #4545 from ludusrusso/issue/4542
0eb7406f97d21afadbf8e57685d699813b69cefb Remove unused DNSAddOnType constants from kubeadm/v1alpha4
c32d640404f5048fef376f2d09cbcff2c73996d2 Merge pull request #4535 from vincepri/rename-upgrade-rollout-after
db4736853644a6440a1b2eea990d7af99a29d992 remove ClusterConfiguration.UseHyperKubeImage from v1alpha4
9d825629d89c9394ddbdf1484fc9e389cf544146 Merge pull request #4544 from vincepri/fuzzer-metav1-time
a31cb9bad91b4c375c0c047ce7cdd84cf6e10a18 Add unit test coverage for machineDeployments. reconcileOldMachineSets
450a28370cb3aa01f168ff870c490a6189d76e20 Drop usage of GetValueFromIntOrPercent in favour of GetScaledValueFromIntOrPercent
5eccee7ee4e270c47e791154c709109c322429b1 🐛 Fix v1alpha4 conversion webhook failure
0beb260bd3b29d7ea96dc1aeab2449b94146d4a8 Merge pull request #4516 from ludusrusso/issue/4177
b53bae0474af0c3e59e5a0664048af886d76ac35 Merge pull request #4529 from fabriziopandini/use-golangci-lint-v1.38.0
68e40f182bb04c4f01f2c6d7fbeec8f7da2befd3 :seedling: Add a fuzzer function for *metav1.Time
924d3642089aee8d6358fc9eda76b6fab8d0e223 use golangci lint v1.38.0
d0e35ee9c408de9bfa284a7cf58d20ff19ca629c :warning: Rename KubeadmControlPlane spec.upgradeAfter to rolloutAfter
261d231912b16496ec8a97b45cadee198ec9eb42 Merge pull request #4540 from chymy/fix-func-comment
30aed6a7a346149c280bde70afc21b1622b78bfe Fix comment issue in method
4ea7d2c88eea7bd7f95d5e205ecd1c7c5a01aba8 Merge pull request #4538 from vincepri/update-cr0090b1
03d551f4b257afe5a5bee36a56f0d7f86518439c Update Controller Runtime v0.9.0-beta.0 and Tools to v0.6.0-beta.0
a0186d222e01a85000701bf83b9869bff4f47a12 remove DNS type from api v1alpha4
a0313ebfbbee0960956ea7577432bb9ff4ce500c Merge pull request #4528 from n1r1/ext-remediation-proposal-modifications
da0c45cd115de5c011f34ffb966f147562fbfcea Merge pull request #4530 from chymy/fix-anchor
c8a11304116ecaf75e199c851d1b6e7b96bb6af4 Fix anchor and spelling issues in docs/scope-and-objectives.md
962cab3f255359342b718f3e9bb66e58985b7b0e Replace ExternalRemediationTemplate with RemediationTemplate since the latter is the one that was actually implemented
cc1298536490f67b8a48dc8876dea22dbb0eb736 Merge pull request #4515 from sbueringer/pr-fix-upgrade-e2e-test
4702dd407b473fa331374fae4aee082265518572 Merge pull request #4511 from enxebre/fix-4509
2ed4f785e69352f01d8ca6dd59aa3cf6c90a8201 Merge pull request #4524 from chymy/fix-typo-20210425
4445a51dff6e2b6405a5d2ef535a79144a2386ad Merge pull request #4523 from chymy/fix-comment-20210425
bdcd38553ec0acd0370e0588003e254600af8aaf Fix typo
a2d44fdd8cb1e194dc9a4e707e471732606b4c4b Fix comment for UpdateImageRepositoryInKubeadmConfigMap
7a67d6a079d1c472b66360db8dce90bf5c918d95 Check Strategy is not nil in MachineDeployments to avoid panic
932893fcb7ae1eeb11783f44112ea218eb52e6ad review fixes
9f0127f763f9b825a67b601378de81fdca5bbf62 review fixes
70e11cda64df7e8f6b6114ba088c27b10477d290 Fix upgrade e2e test
a4ac38b17f7fdbf09ba0cb7de02309262c004158 Refactor scaleMachineSet
6750716532efce1e6cbd6e1123a063fed29af4ef Merge pull request #4510 from wuli-jessica/master
ea99b73aee5127e0e1cf2022bc926862d8cd0bf9 correct two filenames
46dc43a725c9acc168fb7171e5710d3e12db8633 Merge pull request #4505 from enxebre/rename-unit-calculatestatus
dcfd306016534f363ea1d03a6178eaaa88b7214a Rename unit test to TestCalculateStatus
102c753ec14c3f6ebfbce7084e1176eb62e6d80d Merge pull request #4504 from CecileRobertMichon/capz-getting-started-link
a0c20feea0ac70a88e13f7ee662c715d03f1251c Merge pull request #4495 from enxebre/unit-test-md-rolling
50f89f372d3e451806f4e00c4aeb12952ceff9e8 Merge pull request #4135 from enxebre/unmanaged-infrastructure
a641e30d169805ce31a60263d8ca6937f9034073 Add unit test coverage for machineDeployments. reconcileNewMachineSet
9f094b25defc5473dfdc9fa3550deeb9db05c253 Update Azure Provider Prerequisites link in quick start
8bac033459c451a56c2fad2f32e5cc2ae42eaa79 Merge pull request #4501 from sftim/20210420_improve_links_to_main_k8s_docs
6103b95bb040c7ad4ccd9bf98374de45543289d4 Merge pull request #4496 from randomvariable/capa-book-link
294e7a3e69b9f6e291acf737db564b5d4b0d7170 Improve links to main Kubernetes docs
8864dc08e5dd8fa80a1d5f9938ab7b21aa80e90e Revise CAPI book introduction
dd52dc01b6eef110ee555bd5ca2628002495f437 Merge pull request #4492 from detiber/emeritus
87526c65dc64bde3dcbf4bc3ebb1eee73e954eda Merge pull request #4494 from chymy/reterr-redundant-judgment
2f35ed662741ffd9ab88c03a0a1ad6b51b924262 Docs improvement for AWS
2ef661e3713e789d686d0ae12500a20eb1d4d530 Fix redundant judgment for reterr==nil
903cebfc5c935c95e68d67d4e6f21cb0baa34dd3 Move detiber to emeritus status, update security contacts
0983562c7b22e8386434f5bf4a907660ad16308b Merge pull request #4479 from CecileRobertMichon/owners-stefan
506078bb31bab8d82982f770644c6ede9d09f181 Merge pull request #4487 from srm09/fix-typo
cbda02f7868b452452b91179b39e378288be3aeb :seedling: Add sbueringer to cluster-api-reviewers
ea1b70eb691749f5b7b8065960ed949789f3308f Remove CecileRobertMichon and vincepri from cluster-api-reviewers
9bfe6a1ed0c312e4397ff66fa6303e9943695b2b Fixes typo in machine types
1b4faf5d6282bfdd0fac543c798238fe2c9a6046 Merge pull request #4478 from CecileRobertMichon/owners-fabrizio
404215420c883e8003fb9422cd81a46eb2b678a2 Merge pull request #4480 from yojay11717/master
2965181e0074621dfed778066ef07a6578bce690 correct a word
7a3b56d40681120830e40797f6b233a890d85775 Merge pull request #4476 from fabriziopandini/fix-CoreDNS-1.20-1.21upgrade
3bc596eea96cb27e23c8f2d6c758f6bd56db67b1 Merge pull request #4346 from relyt0925/ondelete-rollout-strategy
b61143ceac7ca2c29f5aa134ad15d01a55b2d8d1 :seedling:  Add fabriziopandini to cluster-api-maintainers
c886a45528aea35836a8376570c41fdc7fa661d0 Alphabetize OWNERS_ALIASES
405345853e445066a77f12a9127aaf32ff2626c4 Fix CoreDNS upgrade from v1.20 to v1.21
d270d95be0a9df978d1a518744c8b9ada83239b6 Merge pull request #4327 from chymy/fix-figure-notfound
2469f743633bb98e656b99f79bbf4b58bbe7c931 implement onDelete MachineDeploymentStrategyType
768695b2f6ca44d9fa6a4661176e39caaab71dfe Merge pull request #4427 from mrajashree/docs
2deb9de8c6426536fd2939c5f7bcdc32facd3142 Merge pull request #4333 from scottslowe/issue-3373
70cbb84ce279d97ab1670b36140a85bc352f943b Merge pull request #4455 from ludusrusso/issues/4382
026be8b8a8fa4525e8a3a6050c251f8b309c1d53 Merge pull request #4460 from chymy/add-healthprobe
8481b9fda3298d6eddb15e504ae9383ddc86ebd6 handle deamonSet in InspectImages and FixImages
aaea64e524bfcc8d0cd429b2baa4e6956dd8d0bc Merge pull request #4470 from sbueringer/pr-fix-upgrade-test-fix-coredns
e2313d5dc7889538d667598fae9b05b3c94eddf4 e2e-upgrade-test: fix verification of CoreDNS
dc27cdcb7226f90e6fe7a66ce773fa63245f4a5a Merge pull request #4466 from fabriziopandini/fix-test-observed-generation
71c3b21578ddba65483433b697da8acc47ac59ac Temporary disable the TestReconcileUpdateObservedGeneration
cdefccd51803bec8a1ccf3e753002cdcf53ba511 Add healthprobe for bootstrap and controlplane
d1dc87d5df3ab12a15ae5b63e50541a191b7fec4 Merge pull request #4465 from chymy/import-path-err
d8ea1b488be711d7a14ec2b01561903f8da8317a Fix Canonical import paths err
e4ae2abb15c26e7e1d59dd90cbd050e6be007552 Merge pull request #4459 from darkowlzz/patch-1
b1475dd62782ab608a32c2f5ddd5b645a379a9ea Improve project news docs statement
2cbeb175b243da6953c4edf9e7ec99eac4e2a4a2 Merge pull request #4453 from sbueringer/pr-fix-capd-cluster-paused
ec3492800174af48377566ef100feb9cef12aec8 capd: do not reconcile machine if cluster or machine is paused
bfc6f80add5c21b8dc2b704951f42bc14708ebc4 Merge pull request #4451 from davideimola/remove-ginkgo-from-kubeadm
377532855522dc84a2872f9404157af24f2b4260 Merge pull request #4448 from randomvariable/ensure-defaulting-validates
46b7feeb0489f691d95a33b6a46027f56f59c2d2 clusterresourceset: Allow strategy to be changed from "" to ApplyOnce.
8c9bca7d8524ebaf94d1704f2f9ce5c4bc0540cd Adds a test helper to all mutating webhooks to ensure defaulting passes validation both on create and update.
a4dc7ad7d90f9afacd60decc41072d5096f6f702 🌱 Removing ginkgo from Kubeadm Controller tests
27850a4f980a8d440dc0221f9b9e0a7db8fa87b5 Link architecture and code walkthrough videos in docs
866e1136fff28695aae4a529a1b830853ebec82c Merge pull request #4439 from Nordix/fix-max-surge-mutability-issue-master
768407972739108a69371ce4a8f1d681f34adadd Merge pull request #4432 from sbueringer/pr-capd-debug-infos--on-container-creation-error
5ad599e4122a074792b1d01a915a049d627e3189 Backporting rolloutStrategy caused an issue 4437 in release v0.3.15. This PR changes all KCP fields under spec.rolloutStrategy mutable in master branch.
c7c586faee8a713464175bc967eeff224b170733 Merge pull request #4393 from davideimola/issue/4341
133868933341a80280b3258800eaca028f03e442 Merge pull request #4442 from stmcginnis/conversion-gen-4441
2d47627d586831f3de50679fc0032a118eeddd30 Fix the observedGeneration update
4fcb19456e5d72c09f8230409c42550b193b029d Make conversion-gen output dir explicit
5f08b4ad3e87dcc4da6d1f923274d7e3ccd48c2a Merge pull request #4255 from fabriziopandini/add-CAPI-owned-kubeadm-types
e8cb88e428d75389bf2a4737639fbf787ee64178 Add CAPI owned kubeadm types
e66809aa0ed6b31ebe5fd72cd7c76d12b9691d82 Merge pull request #4431 from sbueringer/pr-update-gcb-docker-gcloud
e0a8a183b7f11e007dbd0e5b5de5ac1345454537 upgrade cloudbuild to use gcb-docker-gcloud with go 1.16
c5b434a19c4d7a7733112f220c990b6833604df5 Merge pull request #4230 from shysank/feature/4194
c7b22a6823cf03a2a5a67ef60f0dc0777082fde5 Merge pull request #4378 from fabriziopandini/remove-gobindata
5afd3ac0578694a694fa42bf9d1904023a012ea6 extra validations for v1alpha3 -> valpha4 upgrade
3d3dd08e6b303bef9d6245509f2afd4d9ae6b23c remove go-bindata
cf5190b085f91fc5f6fd5a2ee9f36eb936cc2567 cluster/mover: improve messages when patching the cluster
a01dd6f3031669e19e4aca3478470c21ac1f263c capd: print debug infos when container bootstrap fails
77093e2350cdfad5db64c88978e313c08e12a20c Merge pull request #4421 from sbueringer/pr-kcp-include-node-list-err
5a555af52ec65b387f854847eeab9c4c7e5db816 Merge pull request #4425 from Evalle/ISSUE-4422
f189c0e83f209d933136dc7b2cadc81d7525b892 Remove duplicate upgrade word
8a54688e2c5da087712d0c4c8663cc952708f997 Merge pull request #4328 from Nordix/clusterctl-alpha-rollout-book
25fc8a312a2c6c2423f7bb84f6d5d1771e63328b Merge pull request #4414 from sbueringer/pr-e2e-test-increase-docker-observability
5b03941ec8c0f9d2b5df956fdf5bf8d73ae5d809 Merge pull request #4317 from Nordix/clusterctl-alpha-rollout-cleanup
00b2032b1f7e5384491ec82154966d3e46d315b0 Merge pull request #4398 from ashish-amarnath/lb-status-filter
88c5e4b2a1f6570a433570e8317eff7d97db0e1f Merge pull request #4424 from chymy/fix-typo-cy
21649b93e9480fb52a6f95bda8beed825f9076dc Fix typo
2ea6cfba1b1c599fae71cb5af90cd7e2a4c4be27 Merge pull request #4402 from sgirem463/myfeature
35f5617bd4ad027f2b31e3d03c01291f4544b9af kcp: include node list error in KCP and control plane machine conditions
5a2c17c47fd131d05ef3f77bbb89e5a28be3a4a8 gather more Docker and containerd logs in ci-e2e.sh
4cad56f8049379b9bd31789dc62603653c511abd add a warning message that KubeadmControlPlane is solely supporting CoreDNS as a DNS server
7f879862f3745c44c3a4c69606ab0c842db96cd6 Merge pull request #4399 from stmcginnis/ioutil
c77042297d5b7b649f818140411f35f42d678252 Merge pull request #4418 from sedefsavas/4407-2
60bea39d4e0cdf0e0d7bcd586e997d0d1f5f0619 Minor Makefile cleanup
1e53587dc351ad8f9320ae7a424cef41f34ff795 Cleanup recent work with `clusterctl alpha rollout` command.  * Switched from use of tuple to object refs  * Now using global context  * Moved MD specific code to a separate file.
a224c4dcf6419eb06c6c9b9d52eb69ff5f20e34c Merge pull request #4397 from fabriziopandini/fallback-onbuild-if-kindest-images-are-missing
1968af7c480a0489122e28e11fce8db55b11a016 Merge pull request #4357 from ludusrusso/issue/4356
65d2e42b33953fd72587569f66f7661e82de7e9d Merge pull request #4415 from fabriziopandini/fix-E2E-remediation-flakes
3551887b9dee9c0b43237db6d7721d4d3e733d84 Merge pull request #4345 from ludusrusso/master
5281c32c24779fb4014c80ae260b1ee1c5654cdb Merge pull request #4410 from sbueringer/pr-add-junit-report-for-ci-test
b323861991c7f0092c357eb1de6a985a9159d3dd Add CAPI book section on `clusterctl alpha rollout`
5c068db93307abba0b19cb2d949cd75831d87934 🌱 [capd] Ensure Loadbalancer IP is not empty
d5ade7dac7adc09ed9319eaa07c35f85792fa4d9 generate junit report in ci-test.sh
020857b608eb3318af94d889a9bfdf961287cf4a Wait for all the machine to exist again after remediation
fec46e4f7a4039574a32318b1c562f004d563c46 Merge pull request #4412 from sedefsavas/4407
d90492cb491150ef0916e32dd5f3cbfb4074c538 Run ensure-kustomize in CAPD
431fc398cb4d0b9a4ee57fe7f70545388aae958b fix shellcheck errors
44a3667718c8d58052cdde2335945c68a23512bd Remove CAPD hack/tools directory
885daea54159a20e3d3a730e4b8366446dcca25f Merge pull request #4404 from sbueringer/pr-fix-mhc-reconcile-md
ad1091121a880c5113c9bb76f61111e714c91aec Merge pull request #4347 from Nordix/kcp-rollout-strategy-e2e-test
5291e100a8d94076f186c1fdcff4f49d2a5fd1b8 Remove deprecated ioutil usage
01f71d28be6aeb3f7587e5a15c8bc923447311b0 MachineHealthCheck remediation e2e test fix
ef47e2a91b56c2015722e13aeb437025a11aa4d0 fallback on build if kindest images are missing
b5f22feb5a44b5663a35b57a09dc86378d4aa042 Merge pull request #4385 from stmcginnis/tilt-dev
96ab9172b7c173ae366bc281b4daaf0c82392226 Merge pull request #4391 from vincepri/golangci-action-edited
1f808400fbf5ff53980c02980b95faf62feb394a :seedling: Include 'edited' to the list of PR types for golangci action
8d5fb93a172affa1d84a0f08647212d26f16f609 Update tilt development instructions
8f1013eebb45e7017fe0067f21df99ede34ec395 Add E2E for scale in rollout
aee65de4a18b891dba7bc7956867f436376cd028 Merge pull request #4375 from sedefsavas/crs-test
3de1188f06026d59e733ec1a1bce946732986c75 Merge pull request #4376 from Nordix/fix-kcp-scale-in-resource-status-check
c437b3b115ac82acf10c101319052c1b2973ccdb Fix issue comment 4293
7124a659accd32639c8d021fb7ea9570a4fcc860 Merge pull request #4367 from nader-ziada/e2e-mhc
1449f9b2720b482ca8e0b3efec8ad848b20a7858 Merge pull request #4374 from vincepri/golangcilint-action
7f4f14f742037568d5b1d7c9eacf7436d17240cf :seedling: Add github action to run golangci-lint
e97ac8dbb6c62b188a2d739c3fc721ccb10af751 Add externally managed cluster infrastructure proposal
919ea770296d0b3393c2b354b50ef3287c8aa4f6 CLusterResourceSet test fix
26ff3dff0d8e0b8c5635619d879e875699dfffae Merge pull request #4362 from vincepri/makefile-gen-core
f2888dd9931a354912663ff0618b44590a0570d8 Merge pull request #4360 from vincepri/refactor-golangcilint
7478817225e0a75acb6e14fc7b438231578073d2 🌱 Run golanci-lint in parallel and enable more linters
1671cbf562ead1e95b2b861eb503dcbc1e4340ec Merge pull request #4130 from srm09/e2e-test-for-upgrades
2dfa493166ba27da95d8b7ad79a34d2f7221ec2c Merge pull request #4373 from sbueringer/pr-fix-annotations-util
d934d49ab368543059d6b7e4da8cc910b25d5865 pass the cluster in to the get targets
a07ba3560c528804fbbecd8e8ae9dc1243573fe7 Merge pull request #4371 from shysank/fix_4354_regression
6e281f9fa5bb54539e02465c4a53b70a11f6d77d Fix annotations.AddAnnotations (if annotations has been nil before)
69fcde4078efd24f0a9193e7778c9ba140e7d61f Merge pull request #4372 from vincepri/cr09alpha1
d2a9e7c9fb2e5b9a070c91ddf8d25417c79840d8 :seedling: Update controller-runtime to v0.9.0-alpha.1
3f7430d7cf84cb40fa2168149d222417add76a31 E2E test to upgrade workload cluster
27fb6edc149bc3f19c01cea632261f1a5c55a231 :seedling: Reorganize Make generate targets to run some in parallel
33ee55935acb8aed735d53456903b4bd253ae0f9 fix clusterproxy interface
c3ec6cc75565c4ce59fd1c0e803f7886e5c68c4b Merge pull request #4363 from vincepri/object-meta-simplified
fcc3879aca65f2f62981d96980c5bf83ee44bae2 Merge pull request #4368 from vincepri/crs-test-bug
432272a8c4a46bf6c607bb7820eced0dd49be1cf Merge pull request #4366 from yastij/scale-sub
cbe5fb9d362d0672ecbf0c1955855886f2f55d3f register kcp's scale subresource to validate scaling
4eb5b05f2145cc2ac716c501a738eccd07b740b2 Merge pull request #4369 from vincepri/go1162
ced3420bee1ff0057498a98a610a288bbc6c7f1a :seedling Update Go to 1.16.2
81493624dd8859f47af2a4ba32e6e189a6950f5f :bug: Avoid masking possible errors in flaky CRS test
9f6b80065f02f71b89f73e4d991aebfa2746bf63 Add github action to update homebrew formula of clusterctl
f9699fb3f7572b66ca710cb48dd23c839d2cce76 Merge pull request #4354 from shysank/apply_with_args
f4645609f1286a55334cfb353619069c23ed2b04 allow extra args to be passed during kubectl apply
440a0035c0ddf463147652976878cc2015dbc235 clusterv1.ObjectMeta should only expose labels and annotations
5cd1132aa75f6358d66cf977164ace68ec87efe0 Merge pull request #4349 from stmcginnis/controller-gen
47a5bc54d923ba5bd96ad12ac46f5d595283bfc7 Make conversion-gen output location explicit
34e62089fa3378fc3391d4f2e7276b581c790d2e Merge pull request #4307 from GrigoriyMikhalkin/CAPI-4275
aeeccb333f5025a046892452db301253a766c4f9 Merge pull request #4353 from vincepri/update-deps090alpha0
f39a263d435c6da6104538f7676b9bbed92e977a Merge pull request #4199 from fabriziopandini/clustectl-v1alpha4-should-block-on-v1alpha3-clusters
36c2180bfbbfaac61b049548f83e4482be7eb368 docs: Add install with homebrew on macOS and linux
28f70b46bce7c1406660e52770ec8bf7c7487af0 Add information on using kustomize with CAPI
e4aa0c6ad281c14e4cb1205234579e9689e6c7c9 Merge pull request #4285 from mig4/3401-document-upgradeafter
2f76aeebdf767a06d6497cded306f7702b283108 Update CR v0.9.0-alpha.0 and golint 1.32 dependencies
a55ff9bec8120b3e8245d1025cb7cb24c32864cf Merge pull request #4340 from stmcginnis/book-cleanup
5ff8484059d27952978be421303a859efd425f92 Merge pull request #4350 from vincepri/cleanup-bindata-go116
840ce46c60c5d4d5292f6b43d85cb7cdf6f127e0 Remove most of bindata targets in favor of Go 1.16 embed
f310fe99c5817eb0c38f8ccdb71345c815b63065 Merge pull request #4207 from CecileRobertMichon/util-filter-cleanup
3d00481a50a8626aaabda75dab36608d598a1aa0 Merge pull request #4348 from MaxRink/mhc_docs
20481e63121be8070164a28565b97d12acceefe3 update MHC docs to comply with current impl.
c7046ccf7525391172900512d0fed9623cfb1ade E2E framework: support relative paths in URL component source
01bce1b080f434043cf85d8a5c87735364b4d2dd Merge pull request #4335 from srm09/check-for-external-ref
5b93524b68a037eaa8d18fd6616360aa4d66b873 General docs cleanup
7a9cc5faafd4d78cc1c5abd9a3eab406a7b777c7 Merge pull request #4332 from davideimola/change/normalizeFlags
69aa31e39e924e0a133c20a0eb488f148a8b2581 Merge pull request #4339 from kinvolk/invidian/fix-ci
302bc2b5736dec6d393915a854c480db8d327606 scripts/ci-verify.sh: set executable bit
f14aefe7e6849e8e03a01babaaf76828a4ed05fa Adds condition when external ref is incorrect
10cde50056f63212f1c6a1831a37aef70dcb12c4 E2E framework: support 'file' scheme in component source
21740cbcd0a2a8185d96fbfb3cd05a2b09fcce6b 🌱 Normalizing flags from _ to -
c0804467112134886b6be66df7874218f82aea1a Merge pull request #4314 from alexander-demichev/ci-verify
939c26f4475fbd9347f02ab95dd40b4744da67e4 Fix figure 1 not found
12cf0b56d0459dc0049dc191ef25f2c7bc90966e Merge pull request #4323 from MarcelMue/use-variables-makefile
b1c8248b39561f50aaefa6511dc1500a3e2c6258 🌱 Standardize machine filter functions and improve testing
41d5087af359f0c8b86bf0be6bdecd96a0cff261 Use variables in Makefile consistently
abdaee558d015938726f1aeefca0e2cb8014b67b 📖 Document `UpgradeAfter`
0bc5750fcffcb47f88b46e821a8a7785bb04a6a0 Merge pull request #4308 from vincepri/cr09latest
bfd1c2cdecc9ce53fdf53bb61635d16fb79e3617 Merge pull request #4298 from fabriziopandini/use-distroless-for-CAPD
c81ea718a0c81b16d69e7dc164ad4c927aca3ec7 Add CI script for running make verify
8d2174d831cad0b3a1df99eb93af88f5ac9b78e0 :bug: Fix finalizer behavior with fake clients
49ccbb87a37c8855ed18b1c3039bd6605d2e79f8 :seedling: All tests suites should wait for webhooks before running
1f21fe1ce4a7a88285182a4efb28559649a3af82 :seedling: Update CR dependencies and Kubernetes 0.21.0-beta.1
752c727cf58bf4af94d3337c4f8e21980ee4c06a Merge pull request #4302 from prksu/general-crs
b677a376f4a7b3769efa5536bec3c778fab08bc8 Merge pull request #4306 from chymy/fix-link-404
3cb347273c7de8972e30ea334d89cfe72ba50afc Fix link 404 in 20190610-machine-states-preboot-bootstrapping.md
c9b7ecbff469dd8ff9d7e0fd58af263f225224da ⚠️ 🐛 Update envsubst to 2.0 to fix escaping of namedpipes (#4305)
345d392ffc2f1b7f22849d3fa59cde85e38da76f ⚠️ Update klog dependency to v2 (#4284)
c9e9b2717ba12e2284f9e633e14b2adba3da0d88 Merge pull request #4078 from Evalle/ISSUE-4005
abba4c99f8d3cc0a44fffbfa0001c16ea67294d2 Merge pull request #4098 from Nordix/clusterctl-alpha-rollout-rollback
38584db52c1cac52c03560e812b16ff207d50069 Merge pull request #4301 from fabriziopandini/fix-version-support-doc
b936885009a815415413fcd50b21e60cd916be03 🌱 Make RegisterClusterResourceSetConfigMapTransformation to be general (not only for CNI)
d42f93b9d2d628c7cacc2031aa644cc3a016eaf7 fix version support doc
1155588065f4807da9fb10a99c0e027d66c24058 clusterctl v1alpha4 should block on v1alpha3 clusters
fb763c1f961027160e66292ea73f86159601afc4 Merge pull request #4300 from binchenX/minorFix
826de807fc7310df834e6df86cb7909d0bcf6a55 :seedling: fix the typo in error message
18029d5add127cf4d91ed36de70cc1c14e4e9b4c Merge pull request #4295 from jimmidyson/machine-pool-descendants
78ecdeda530235a374b21591498addf36fee9cc8 fix: Include machinepools in descendant count
9ca491c79fb2decc77ff4e5e8183ef07f43967ae Use distroless for CAPD
1f07103fdea881dd8dcbf28883aea2b7dc95a63f Merge pull request #3752 from ncdc/mhc-use-conditions-for-node-startup-timeout
ff383eca185911abf5078eface4dc74bf71f6e8b Add mutations to conversion tests
ca9dd7e1da84e8133f9379a5b8dd3bfa8c0443ad MHC: control plane init / cluster infra ready
d1032c65d858c2bd2b7cf5e6235ec0b8eb163a43 remove cluster.status.controlPlaneInitialized
2e64a16506df7ad95349916997bd464af733b295 Add ControlPlaneInitializedCondition
d0c3bf865f05acbe7dc23bd854bd4c19390ed845 Merge pull request #4161 from wangzewang/master
a9144a861bf49e06c210035fbba5667fffdb609f Merge pull request #4227 from fabriziopandini/kubeadm-types-stop-gap
e9e3503af7d2da7d6d9cf5c06d70676c05c80070 Clean up "deprecated" variables/functions in v1alpha4
6147c8cb0832c8049178e7dd9c298abee7ad1fa9 Merge pull request #4170 from fabriziopandini/kubeadm-types-KEP
cc47feb9141e2741bd644f48c7c48f8208d1672d Merge pull request #4236 from fabriziopandini/default-cgroupDriver-to-systemd-for-1.21
949a9aa614d140e35607d17feadc84431e52bddd Merge pull request #4213 from vincepri/enable-crs-default
2db2e49f7fa2f0febc5a8f2cd4605fc861aa5c96 :seedling: Enable ClusterResourceSet by default
d0ffbc088c92b7c379adc008620b005d2324061b Merge pull request #4274 from davideimola/fix/updateCertManagerModuleVersion
d18ddcd6e861ba374394936c87fbbf7d54d9a790 Merge pull request #4128 from shysank/feature/4020
7d53242eadffeae4c6172c05bf5fe2d89c7f3d4b support range of values for unhealthy machines in machine health check spec
f37d8116982b92cd972c7ec0f4d72e79ae079ae8 Update Cert Manager Tilt module to v1.1.0 as default
febfe5bca95629617a3f3749b592c7991f8d5234 Merge pull request #4277 from dlipovetsky/cert-manager-tolerations-regression
51d1fb6936b0664be3529e3094bbe6e858572466 :bug: Add back tolerations to cert-manager Deployments
4fc3399fdcbac1006ea4a71a47dcb8405c78667b Add kubeadm types KEP
ef7a51b6d7250b891de323832a351fe6f76787fe Merge pull request #4073 from Nordix/kcp-rollout-strategy
74a70a68fd8ed848db44d3639486cc865242f31c Add rollout strategy support for KCP
cf0b6d77851651840600b940ae8dee4c4c165bf0 Merge pull request #4216 from goushicui/master
b00bd08d02311919645a4868861d0f9ca0df35ea Merge pull request #4202 from fabriziopandini/clusterctl-v1alpha4-should-not-upgrade-to-v1alpha3
de2941e7bb03996fd320d5a21a90dbc9345818e5 clusterctl v1alpha4 should not upgrade to v1alpha3 contract
df91a0e8db5ae2e8cc7b84e440850d614abe26e0 Merge pull request #4267 from JosephSalisbury/improve-contract-error-message
845acb242e084962d247dabb85f98af97c9464b7 Updates conversion error message with reasoning
3cd6fa17719ec58d981623b738e5fd8722b953cc Adds command and client for the `clusterctl alpha rollout undo` for MachineDeployment.
43efbfdd44b6f68194fcdb27b0a4cfe055227361 Merge pull request #4237 from fabriziopandini/document-policy-for-workloads-on-KCP-machines
046ab290ba3ceb633ed971b1dbc9b84983e9c731 Merge pull request #4220 from binchenX/doc
13b8097f20d30b3104c399ee838c66e1b72d1911 Merge pull request #4245 from MarcelMue/individual-service-accounts
a05b4ab42c050c6cf7a45a2829df1cec244828e2 Merge pull request #4250 from sedefsavas/removebazel-master
b476c4bde6387838d53ec65f1e44468e20858f7a Change CI bucket for conformance tests to the non-bazel build
780f05066b35c231d4e619815d6210d1e6db0eb5 Use individual service accounts
0cd93656725effbae1824e901a75f2c1ca7a803c Merge pull request #4249 from ShrillShrestha/updateLint
b4903f9268f30259cbce1f7ab869c4f05753f620 document policy for workloads on KCP controlled machines
ca07fe0b9916d75713df828a557466b71964897e update golangci-lint config to use disable-all/enable
086cdbc6f3c351e2a4f22d4544452a70d3222bdf :book: improve developer doc
ff200d64c75fa9a2270486e036270e014f1583b7 Merge pull request #4240 from fabriziopandini/fix-kcp-remediation-when-nodeName!=machineName
b836d51fe6fa9d5fc8469d2a5dab68bc5125f5ba Merge pull request #4238 from vincepri/cr09-go116
342d261b140ff6183f93d5e58e0798d7d3e99225 fix kcp remediation when node Name & etcd member Name != machine Name
e9cacc0931eff0118442a5e596b64eccf380c731 :warning: Update controller runtime v0.9 (main) and Go 1.16
f7351b1659926a009608dd6b63c8b53c93ddc280 Merge pull request #4171 from alexander-demichev/nilcheck
8d25ab047ab89121b165f4d29988e9de560871b7 Merge pull request #4200 from fabriziopandini/clusterctl-v1alpha4-should-not-install-v1alpha3-providers
3715ef43365d7c64ca420f784c14e0210021af65 stop gap for kubeadm types removal in v1alpha3
9f236d1810675aa0b93871ae13c270ed80e6788f Merge pull request #4217 from kinvolk/dongsu/fix-ensure-kind
69afa1f68dc38f13d8acbcd90e4b125387cb07bd Add check for empty maps in machineset controller
b5c93151a0a14f04b97d1e8ac0436e68ac8865bd more comments
6bd7e31f94ed5d2507a9946571d92dfee1a6abfa address comments
7014345654d695a9c741017c7e7f54b1439c0226 default Kubelet cgroupDriver to systemd for Kubernetes >= 1.21
69baec5bae6df1e3b6f353e259abbb0bb3df8f39 fix panic bug when getExternalRemediationRequest return nil
fc5ee145ea542994eb612d0de699283201b043b1 Merge pull request #4228 from scottslowe/issue-4138
23e0b2db07cfd24435be05c17d885b0eede1bbb8 Update MHC documentation
3e572ed75817aa30354310430912558d20fb3a8e clusterctl v1alpha4 should not install v1alpha3 providers
8d1396821ca9bdb46b4dc3b63344f72f934bf443 Merge pull request #4215 from sbueringer/pr-improve-v1alpha4-migration-doc
0dab2d9751974071f46ea2f2b82919792a1c5c5a hack: fix semver comparison in ensure-kind
013aa99fa1407b987c943d47ef2fac6e44b48e30 Merge pull request #4187 from MarcelMue/remove-verbose-flag
56d2fa1d18209b9163c457f374405a066750d38a Remove verbose flag from make test
8ef13da0e704209408b81ca6c5f6fa6e306fc2dd Merge pull request #4212 from vincepri/patch-helper-validate
0274cfbec07570a2cc0a8dcd87eb2ecbd3490d8f Merge pull request #4208 from sedefsavas/dockermachinepool
a877397f256d4b35d95cd1beb3fd3267914e0b20 Merge pull request #4214 from vincepri/switch-k8s-gcr
355542c66ffd10f3af0860721046c1cbf72eb1ac some minor fixes for the v1alpha4 migration doc
b0a8b2280c3fdfbf0294e7995049f934232d99bb Switch published artifacts to k8s.gcr.io
3b108acd4d76c544c276a45b5926972108c5b74c :seedling: Add GVK object validation to patch helper
bc756c4e7ed08313413c1300859bd4dceeccb25a Merge pull request #4211 from fabriziopandini/restore-fuzzer-tests
b2e1038236d030c2b71e599211b30f514630ccfe restore Fuzzer tests
1e8af4dfa9f25e97c58d16b24323ec42858584c9 Fix docker machine pool status update
be43e851ec49ba272716c50704b523c1a3dd761d Merge pull request #4204 from fabriziopandini/align-kubeadm-types
f615d7c76d481aefbbc359097dc4ce6257a48f84 Merge pull request #4186 from vishnukarthikl/watch-fix
0fcb59bc32d046b18ed85215e22955a15c431977 align kubeadm types
95f492b5638168157d6df0023c54c3726b1cb384 Merge pull request #4148 from lobziik/webhook-cert
f905b7f0e120ca2ed1faae42340072ee57d4851c Merge pull request #4168 from shysank/fix/4032
65e5385bffd71bf4aad3cf34a537f11b217c7fab Merge pull request #4188 from CecileRobertMichon/quickstart-update
e62f4d18e390c75dfb7718aee4a6ca742cb2b1f8 fixing test failures
5c85a0a01ee44ecf7c8a3c3fdc867a88af87d73c Merge pull request #4189 from ajayk/docs-fix
17d20ecb01a574526c1c12226be15e400b01526f docs: change to clusterctl instead of kubectl
98b7eef0726e169b78c06a277653574aab013543 :book: update quickstart doc
522b569b12318ca189e898137f55f32f2d593173 Merge pull request #4160 from CecileRobertMichon/refactor-cp-utils
0ca16e1dca4c3940866957f07f27376b366314c2 Fix ObjectTracker to allow retry on error
cb9a06b8b5835814c80fb11ecd3069bd1acf1db1 Merge pull request #4164 from alexander-demichev/validation
9a4c630262f3147c5b218b5ff369c9e28761f5dd Merge pull request #4175 from gottwald/fix-nil-pointer
338375a908423a3843512ced6b9207ffcfcbf882 Merge pull request #4167 from wfernandes/core-provider-metadata
4e6fe8bfefc01044f6f28e16f776b27d1d38432d Merge pull request #4169 from superbrothers/fix-completion
fdb2f40d4582944e89a724d11afc78e262c97d42 Fix nil pointer dereference
29d57a7b09c85e515da1f27e16071a8f972bc5c0 Add possibility to specify webhookDir for CAPI/KCP/CAPD/CAPBK managers
bfc1498d363b90f8c695aca2ba4f19d57d60ceca Merge pull request #4173 from vincepri/cr082
b40f31f0294dd1c1a98ab0d14ee7c425a2200cdc Include metadata for the CAPI releases
13242693476e845db6f8c2ba47816e1dec9c084c :seedling: refactor failure domains logic out of controlplane internal package
dc658141b153908e853b77489107aff889df4fd4 :seedling: Update controller runtime to v0.8.2
dbf553b158b4f299dca9a2c47f62e32f4ece14b8 skip remediation for paused machines and those marked for skipping
8388953c964016539b00fedf292589254436f801 Add resource schema tests
7a9b6a18c952ea78f366315e1a314aabaab3e71e Use openAPI scheme for defaulting machinedeployment replicas
0729917266db1f06a1b5bb39f41a91b48d966a5a Use openAPI scheme for defaulting machineset replicas
5e4319811ff084c6758dc917fb43735e5cc7fe7a Add test for listDescendents fetch MachinePools
72a8bfc55979c56eb15810d954399a790d67e71e Make clusterctl completion zsh work with sourcing
51a6d64d171c42fe18dd6983eaed7556a8e94184 Merge pull request #4163 from CecileRobertMichon/version-util
67618d859c58c7f568415da7bb91cd5bba099d83 :seedling: Clean up kube version parsing
4a6cccd2ddb1acba09d49d691acb33d52a16075e Merge pull request #4119 from MarcelMue/add-watch-label
fc41bf68a4eed611977fb981474dfb347f615f15 Add watch-filter label
6db673fb8a880e28cbfc344b1a29530e0bafe65b Merge pull request #4153 from elmiko/autoscaler-task-doc
5b19957707b1e0ea1c500b1f0b0284bd418a0d3b add a cluster autoscaler page to the book
d753a209210c2616caf2a2188f67318a7680e477 Merge pull request #4157 from vincepri/fixup-book-deps
d9755b6a0e4fa1974deb1c565b3b3796cb473725 :bug: Book pre-requisites should all use realpath
207400d28e930ff917f27add3bbfaa49f2021449 Merge pull request #4113 from superbrothers/completion-zsh-native
886a16731f90a7662ec1ce40d9b17cef06b28003 Merge pull request #4013 from fabriziopandini/upgrade-cert-manager-to-v1.1.0
24926f65a835ba0c3b70cb44e92651d752efcf94 Upgrade cert-manager to v1.1.0
08149972c0be98c3a791f071ce16c45134dad8d5 Merge pull request #4149 from vincepri/increase-verbosity-crs
023f829e4849fabcf4dc9313e3b69a8be27c8107 :seedling: Remove verbose log line from CRS controller
df86f35fbc58da9fc4f7e36a2b45dfa93fb95ad9 Merge pull request #4101 from sedefsavas/daily-build
fd37deef67330b7e3a5da112154a85dfbc182a3e Merge pull request #3929 from fabriziopandini/Remove-RequeueAfterError
bc5e2075e57a090b721688ad8d44796c08e7edca Remove RequeueAfterError
8d75200741d239f79c1cf4c407eb612657540b40 Update the capi book
94591f4da237d3f34ba6d4cec595853077654ffb clusterctl completion zsh: Use native zsh completion
da2fab98df3ecb4d94b323f9ab15b50ca931de1f Merge pull request #4107 from Nordix/capi-issue-4103/feruz
4798d19635f4d8474423301bf3771c44e6e75fee Merge pull request #4140 from vincepri/capd-golang-based
e4757e3ea66f8ef1f791490b492786f62ed167d5 :seedling: Use debian-based container for CAPD
7508fc1a008ee7a1c8a8d2d016239b05c06e858a CAPD nightly build
168bdc72e0d9580cfd1f2acf4482f94db2532788 Merge pull request #4104 from Nordix/cleanup/switch-to-CacheTracker-furkat
f26ecef39af1e112c447da447ddb56e71f514402 Fix check for nil condition before assignment, error message and better comment
77ff4a620376871bf28845ca27dc318b2ef5e738 Add new Tracker through the controller initialisation
7b7b1c8bc3430a89927380b5833b77587d91a43b Switch KCP to use ClusterCacheTracker.GetClient for the workload cluster client
1acb1b0680b5a7ee32016dfdb26955b0b8c273c3 Merge pull request #4054 from Nordix/clusterctl-alpha-rollout-pause
53d4091e6d63e10c349f893d9bf89bc55799507a Merge pull request #3985 from fabriziopandini/run-webhooks-with-managers
374e626d2f3c7e0fe3bbe1e6e33037fdc2fc73ee Merge pull request #4141 from vincepri/go1157
88d38fe7391cfc4541a921bed16838508c927b68 Merge pull request #4129 from sedefsavas/crs-live-client
b64bc641d7249eac534d29de03ec7c7d16e0a56e Update Go to v1.15.7
280db9a796d5e1c2b3b75aa3036fcfe44f669909 Run webhooks with managers
0d4e430a4ce37bf10fb7c6255ca9fc197a0a95f1 Merge pull request #4109 from srm09/update-controller-runtime-version
f1cdf7b516d2612aab41d1035aa7912c4cd13602 Fix cluster resource set not getting Secret/Configmap TypeMeta with live client
89deebcf2af0e74bb728f2fed80ebcf96d7eb50c Merge pull request #4125 from devigned/apply-res-param
5815384407bd3cc7f641bf1a3156b7cbc37f06aa Merge pull request #4060 from nader-ziada/remote-user-agent
7d14e9b1d1ce5eee4a6a8ba2e092da1fa1d9fd8d Merge pull request #4121 from Nordix/fix-4110/feruz
3bcf832257a7e939bf1cc20ae9c0c5f4150ba711 set user agent and timeout for remote cluster client
cff67603c580418187619858d01f5e15a3fbe7b9 Merge pull request #4059 from Nordix/bump-kustomize/feruz
60e17cfb555772fa600fedc318151f7213319f39 Merge pull request #4127 from cjcullen/patch-1
16b8ac4bbf597bb57fb46aeab2a172202abc80a4 Update mdbook to 0.4.5 to fix CVE-2020-26297
e823021c166511fa01e0b43d93e3636778b5857c add result parameter to ApplyClusterTemplateAndWait
8079024a377afc659306f3bb64b4935ba83a7877 Fix https://github.com/kubernetes-sigs/cluster-api/issues/4110
1356c4a7db13ddbe8a1fbaa80b606c65e107117d Updates controller-runtime version to v0.8.1
a597f9ec9faa0ab840557a5e17b0f5ee760bb5b4 Merge pull request #4092 from fabriziopandini/document-clusterctl-describe
c34e2d14c4ecd81d5ecd23038774d96c23d42df8 Migrate gcr.io/kubernetes-ci-images to gcr.io/k8s-ci-images
5da747ff79d760c7665b4f0a7dd9b6259c694d74 Merge pull request #4070 from nader-ziada/move-version
75104a2b93c051a62debb4044e7edf376fa3c161 Document clusterctl describe
b08ed532156e011a0e100a79c11a1726577524b7 Merge pull request #4108 from vincepri/release-notes-remove-image
2f9d0599052e24caba3be73a95d0b81e4b32d319 :seedling: Remove the image placeholder in release notes
37941fe876ec60dfdad514ccb0b8daae2b37964e Merge pull request #4084 from CecileRobertMichon/sentinel-file
fc42ce2c721ffc7e47af9fc4e17b89d7d13167d2 Merge pull request #4079 from CecileRobertMichon/kubeadm-script-code
e85197220edcd6a0142444628be9a9eb858b63b2 Merge pull request #4081 from fabriziopandini/investigate-clusterresultset-flakes
b769eab5ab39fce0e2a21ada40dc67f32d63e902 Adds command and client for the `clusterctl alpha rollout pause/resume` for MachineDeployments.
9575c376d85234726306f156b913775169d3a613 move version package from cmd to util
23ab5630cef14e40ab4f5b6d770d85ba9ec15915 Merge pull request #4093 from fabriziopandini/update-kcp-proposal-disambiguating-healthcheck
abf8035027472af2a1dd412a72423fead706d3ad Merge pull request #4100 from prankul88/testing_doc
76c8c35f1bcae887024586d5f68091dfff2345ed :sparkles: Add sentinel file to signal successful bootstrapping
f92d4ba974278fb6b9f44d75b8838a8735e63a2a Merge pull request #4094 from fabriziopandini/KCP-remediation-E2E-test
f7e36290b0d79b54736c3950d690101d213aaca0 Merge pull request #4064 from shysank/fix/4046
d42cc809ab2eec737e6841d58a43e759ac2f592f Merge pull request #3833 from wfernandes/mgmt-cluster-operator-caep
c182b31131951faf9c4bc9f56a36dddcbf164504 Update testing.md
2955368e058e0f24a2999460933dd43971116661 Add CAPI Provider Operator CAEP
c61521971aa027a63a4f1bf8b3d0e6ed7acae18c Merge pull request #4074 from fabriziopandini/document-multi-tenancy-contract
e22d361bb921a011043903e07f37ff10697509f7 Add E2E test for KCP remediation
da6e467069058835776700f8b91a847b75b4c3d2 Update kcp proposal disambiguating healthcheck
bb54134ba062fa8e338e0b0e106f790dcef99bcb Document multi-tenancy contract
97436cc02fdb5cf68c1c313a2b300899bb2a0fed Merge pull request #4086 from vincepri/wait-for-manager
18473b7ba9e21e82bbd1af16b55b217989dbeb5d Merge pull request #4069 from jsturtevant/add-kubetestrepolist
aa86bbbca22a29f7850ab6841c4736e5c3d76df9 Merge pull request #3904 from srm09/refactor/machineset-controller
aa51850504544661eead1685479341bccf9dd39e upgrade kube-rbac-proxy to v0.8.0
d9d0c55e909988531c3c8bc2bddfb83e67ab6738 Remove async behavior of BeforeSuite
96c16641beae6861491acd4544401ab9da3e7625 :bug: Test environments should wait for manager before running tests
90dfe193d044d31cdfaa5edc6df4baefd96061ec use different CRS for each test
cd9b964814ffc4b3accf95688cf3e03694180b21 Bump kustomize version to 3.9.1
dca31d79113862909c590cf896032d5bc4f1acac Merge pull request #4071 from shysank/fix/3973
61dc332270dc63fc5927ef4eef18ff58cb54d9bc Merge pull request #3916 from fabriziopandini/test-k8s-main
6978084bedf8e5f2253691facd73383a15f4931e Merge pull request #4083 from Nordix/skip-test-labeled-serial/furkat
55944799ea68ff1b8c134d2b9b94e94cece394c3 Skip E2E Conformance tests labeled as Serial
b3edcfef30eb9029f3fb57ec09b39746d2c77419 :bug: Set error_exit code arg in kubeadm bootstrap script
a5dee81b2b969732f8e2825d31a743ac8bfdfbe0 Merge pull request #4072 from superbrothers/fix-typo-cluster
03d92d163603993c543f743d0162cbafd8622d9c Add optional parameter for using repolist
3b9bdcef2343e03f900b3253195e0fdf7728e12d Merge pull request #4076 from Nordix/fix-ClusterResourceSet-test-flakes
96e26aac93eeaa399f9d277c4aa4f9262b1b9fc8 Merge pull request #4067 from fabriziopandini/investigate-test-flakes
d1e4645cb43a0886d760e22355b7f6c64bcfe482 Increase timeout in clusterresourceset controller unit tests
e746d54d96349854568c97b6828bb8587b3f4df7 Fix typo for "cluster"
8cd36d1f8c2741d1cd18a6a5115b7452f6c51066 return error when trying to patch a stopped container
97ff5f61c1e2e7bd68ebe92314b608ad13479cfb Avoid reporting health check error when the cache is stopped
daba8fea8d536b896c2ac28d97d97385cb3f3e71 Merge pull request #3942 from fabriziopandini/clusterctl-tree
52794b5c085cf41e75d352754797ac3e004abbb8 Merge pull request #3980 from vincepri/increase-default-leader-election-values-kcp
e7a6ee03509651ba891df4bca0ae8625d9e16271 Merge pull request #4033 from Nordix/remove-embedded-md-furkat
019559deb28536ad40b8c44be83a3502bb54f2cb use non root user with id
e4b5725c2b2a0175b2a6c8ed317877aeec3b7e7e Remove embedded metadata from clusterctl
6be9dbaaee24246c076ecfc234b2d4d68a077ec9 Add clusterctl describe command
953ad253ee2bc169ddda765efe5851c30ffb1def Merge pull request #4048 from CecileRobertMichon/node-annotations
0c7d0a29c2ac6d1166441555873dad1d29b7f77f Merge pull request #3857 from Nordix/kcp-scale-in-proposal
f92a777cecc7354addd1d74a033ce816b6ef23ea Annotate nodes with cluster and owner info
57c6d549ec1ffabf93b460e51efdeca856d97c1f Add e2e tests for workload cluster with Kubernetes from ci/latest
25631455b71c9143d7fe8b3004f696fb8945e1d9 Update KCP proposal with scale in
b6c1b5b3db3d062cf89e7c66ab233fe503767362 Merge pull request #4052 from davidewatson/OWNERS
1ccc83fee8c40295bd6ffc1f53c7a3f17545de3c Merge pull request #4051 from davidewatson/README_2021
5d795d968fe8ea7a5e752439d7e39a79f0401e92 Merge pull request #3994 from shysank/feature/2083
faeab3df99c47516f0a2f3fa755ff7e709940051 Move davidewatson to emeritus since he has not contributed for too long.
66fafbd991ee75eaf9c3daf592518d52eb4f05b1 Update README to point to new agenda document.
b40466802be9844e34450e60cf8354867df42b67 Merge pull request #4045 from rustycl0ck/fix-ipv6
9baf52a46a8d8844ad98aad45d2ac5991a2c0bfa Fix APIEndpoint for IPv6
0731252f230ac797720ea65dcf5683f0dd0bbc66 make kcp spec mutable
aef70fe2d1ae967abcad5a5297ef43c2abb56597 Merge pull request #3921 from fabriziopandini/fix-dockermachinepool
995597dc195324c5cd3ab95750f9eb9e8beda6c2 Merge pull request #3773 from shysank/feature/2585
a06fe963de3c93d189ffa725e218260ebedeccc6 Merge pull request #4034 from fabriziopandini/kcp-adopts-kubeconfig-secrets
506a2987d78e7815e646f1d3188cc0d475c709d3 Merge pull request #4023 from vincepri/uncached-configmaps-secrets
011d92c31d4b1d2b06ba06a10b99573c497151a9 Merge pull request #4042 from fabriziopandini/fix-e2e-conformance
2031398156105a0cef3263ab469fd2dfd3ecaec7 fix e2e conformance test
65295ffdc8c55b4d9ee06b997e43045d515bde12 Merge pull request #3951 from fabriziopandini/allow-test-templates-per-release
1ac789696f38282d236e0318221fb95753cbddbb Use uncached client and partial metadata for secret and configmaps
13e8b81b4e5f6345f01ba00e531feb54e47ecd50 kcp should adopt kubeconfig secrets
c4066e77e9f3357d3327e36660e1c94730f46a52 E2E test support definition of test files for each version
dadd7bd6233edb1e422e7af282e923abff52f830 Merge pull request #4017 from tcordeu/e2e_pod_logs
380ef5da5aea171d9cf299df1644220f964f6652 Collect pods logs from workload clusters in E2E tests
7d01abe6c9e491cf317907932f92c0ca390b1857 Merge pull request #3818 from Nordix/node-drain-e2e-nam
a613952e56e49d807894513365b72e91fb29187a Add e2e test for node drain timeout feature
539f651812cf9cd6dfb8a3f47a3732941ba232ca Merge pull request #3995 from arghya88/remove-fakeclient
e6c20f7d08d852647c4c63f2cb733745ea12ec5c Merge pull request #3838 from Nordix/clusterctl-alpha-rollout
1979640f4934824780dbb20076b9be33ff07b8f1 Merge pull request #3811 from fabriziopandini/add-K8s-conformance-e2e-test
eb4ca99d9d8a508f0d180482e11d357b1053da8b Merge pull request #3799 from shysank/fix/3540
9b261b2458e47a0f48b1d85613fe68189a749f33 Merge pull request #3434 from spectrocloud/ms-rep-count
183c9570fd566672aae6e85e8eaf4fdfb9d6d338 add support for delete policy in machine deployment
f5939fd5246e7f1682399e8004e5fd43fa565240 Merge pull request #4003 from CecileRobertMichon/mp-arch-docs
9139d011f4328f888f2bb7917c93f904b8309b19 Merge pull request #4002 from tcordeu/kind_network
b69666515f2affeb969372d914f895ba77edf9f0 Merge pull request #4018 from Nordix/doc/update-book-bote
35b21845ecb8a513292b3540d5745992221c15d4 :book: Add MachinePool controller architecture docs
ffff2a34c3c3a954b6878640f18e49e65ba726d4 Merge pull request #4021 from randomvariable/update-gdrive
97d1ad0eff227912eb51d37de9b198f347300a28 Update notes link due to VMware GSuite migration :(
7b1db267f8ee464e04860dc3c7826995fb0fedee Add envsubst as prerequisite in developer guide
2925bd9c42ba3a147c96846d3eaa7462f42e5414 remove deprecated fake.NewFakeClient and fake.NewFakeClientWithScheme from tests
6a7adda9ab47588c182c117aada1b084837ef03a Merge pull request #4009 from ncdc/ncdc/emeritus
c08b8e09a0e06d79f3b07086e0cc37ed82d2773c Move ncdc to emeritus
bec5e1260c5074c6a4b47ee2a62be942ee45b5f7 include machines in deleting status when calculate machineset replicas
0219d3ba7309cca936910430ea0e1580249a6350 Merge pull request #3992 from sheetalsingala/exampleprovider
20e5a1aabcfb60674a1dd6837732708d8662510c Merge pull request #3999 from spectrocloud/mhc-status-target-fix-cherry-pick
7e94adb30a87960673502e0ab8ab9826d502b694 Merge pull request #4000 from CecileRobertMichon/rm-bootstrap-data
725a1fb9541056efc4af61b07b33ee7c7c8fd2e2 Merge pull request #4001 from cpanato/add-gcp
313762a67f4c0f654a083a56df00f25014c0d85e sort mhc status targets to avoid status keep changing
ed9029bf32c3d2650703030f1783a21e7664653e :warning: Remove deprecated Bootstrap Data
0f5d069fa7ad7f74a63451698d3cbb99855fdfcd gcp: add capg to clusterctl providers list
970212f09e7c818f64ef57dcb81b70886c70a669 Add command and client for `clusterctl alpha rollout`.
3dfcfc05349df44cf2862b3b550fcde83d151fb0 Use Kind's default network in CAPD
53bf9665f99493744534019d5d24d0920ec3e2fa Merge pull request #3979 from srm09/capi-secret-type
1b4962c9cf72c414628769bce9bdbb691f8f5897 Merge pull request #3946 from shysank/fix/3839
2cd98235f7ed416f34f8310ea5d96e112880a2d2 Moves machineset patching to defer call
96d5083811e9506c1ff13049bf906d2dfb636bde Remove the example provider
8437691189ad8de58168f6de1312e8ee56813a5b Merge pull request #3990 from CecileRobertMichon/remove-mp-strategy
9cd808ebbe8ec9bd8af38939508c44d0834ff6a6 Merge pull request #3948 from Nordix/kcp-scaledown-withAnnotation-furkat
207aadd050d3be3585898fb1ca0fa6394aacfb6f :bug: Remove unused MachinePool deployment strategy
ca2cf1adeab8bec995c90513fc822661f973fe2b Merge pull request #3981 from vincepri/cr070
b21d303ef162ed521faef55775799f5af810df68 :seedling: Update Controller Runtime to v0.7.0-alpha.8
8441b284d19ad4818572e872c6b5b966b277ffc2 Merge pull request #3976 from vincepri/migration-guide-v1alpha4
0baeb9e0481282becb945978ca41c3850343f5ea Merge pull request #3977 from vincepri/exclude-scale-down
cc6c50830d64b5525ad5cde66bf49db82d485abd :book: Start documenting v1alpha3 to v1alpha4 changes
d531afcfa3087cce511f1e7f4bb622994c9df4c2 :seedling: Increase leader election lease values
308e35262eb632788dfb1fbe77dfcaea73504af7 Adds a possibility to mark a specific control plane Machine to be deleted by a KCP when one or multiple machines are annotated by  `delete-machine` annotation. This PR:    - makes sure the oldest machine is deleted first when there is one or more machine is marked for deletion. It implements     the prioritization logic in descending order with respect to rollout policies, while selecting machine for scale down:        - select outdatedMachines with the delete annotation        - select machines with the delete annotation        - select outdated machines        - select all machines     - adds a unit test     - updates the KCP proposal with a note describing the behavior for scale down with annotation
90c54656329c2c00a5b17f8103254f85ab66ca3c Merge pull request #3960 from vincepri/contributing-guide-backports
4f02d5f1e9f732bcde37bb0d14db1736f5552865 Update secret generation util functions
45aaa161a1ef725f0345d230deda0e899f954a23 :book: Relax our backporting guidelines and policies
a284134baba582cd8d7263b325e8e00e0594394a :bug: Scale down checks excludes machine about to be deleted
23df184323d33ce4c5f3f6054f5818b1c878ad3b Add MachinesCreatedCondition to indicate template cloning failures
f91546ac71bb3a629dcfae0e50df81ee0382be2f fix forNodes to only fail when all etcd members are down, rename forNodes to forFirstAvailableNode
f0536bd6787cd410864617d89e6c4f986a28a018 Merge pull request #3972 from CecileRobertMichon/docker-buildx
e6426a6392110fae676a12ffdc683eefdbb57c39 :seedling: Use 1.1 experimental dockerfile image and cache go/pkg/mod
f574c65cfd0a2f7c556a473ced919aa93a7c3bb3 Merge pull request #3959 from benmoss/patch-1
fa3e5b3b89f68b1c1c0103dc635e16a8672eba65 refactor client instantiotion to be able to  write test, add unit tests
09d34e8540d418bfb9c989cb991ac220fd6a3d09 Merge pull request #3964 from vincepri/reconciler-etcd-members-safe
343666665690149c3eda0ca28eb51d1b901e6435 Changes required after review
eef7bb9227377c31df1d20a60c4d8d778346fa68 Add Kubernetes conformance E2E test
e85c952daea0bfe42adf63d54c959614698991fd Merge pull request #3941 from fabriziopandini/clusterctl-use-v1alpha4-api
c04d34e48d87da12490d647cce47832f70f19a95 Merge pull request #3668 from alexander-demichev/labels
d85b6bf0bb396b7dad28036432d4fa9593dbe1e6 Merge pull request #3966 from vincepri/delete-node-cause
0d4ed0c093693df7b1d7c2470a1c367f22284a1e :bug: Node deletion should check the cause of the error
0adc4b327dd12aef7b1094712e93f532a749f394 Merge pull request #3963 from shysank/fix/3923
979197c35281c21bb34a7bc0b70f5c66af6c48cb :bug: KCP reconcileEtcdMembers should use its own NodeRefs
74730d114c69f7d63d981ae9af698fd451bd378b skip spoke-hub-spoke conversion fuzz tests
5803be36e13addccf7cda31e7fd0b75dc6287d29 Merge pull request #3962 from vincepri/forwardport3919
ae7725d5e9ec0a3f582a559d4cba5221c96dda44 Prevent reconcileEtcdMember to remove etcd members when etcd starts slowly
2cb4e72d0583a1751869d850446c1ca9bf160a6c Merge pull request #3940 from CecileRobertMichon/mp-token
0fd4a3b155186f15049d98fa3c3b93f93577b91f Fixed failing tests
22cd6fcdb2788de233d8c67faa05f7c9786b76d4 Mark KCP machines with delete annotation for scaling down
98f950158da03be49c7f1b9fc9577d97898a686f :bug: Rotate MachinePool bootstrap token
cbf6188f32b5bf038d4f9c245f45a254de234b21 Merge pull request #3950 from fabriziopandini/add-v1alpha3-test-templates
adde66e27580d02f31ff7b38f253a23aa2360b96 Merge pull request #3956 from fabriziopandini/kcp-remediation
b0fd6c886824a68d6013801de804cae8eb0df818 Merge pull request #3955 from arghya88/remove-DeleteNodeAnnotation
76be5b636a8b97bbffbde12c323e397206b5d50d Remove myself from reviewers
39be724c02ae074282ac8dfe885f5a775d529abd Address comments
b9c39f6859cee7b6e10c13bf6f6c118cf197ed44 Stop passing the logger around. Instead use logger from ctx
5e82988a79b3ed986c767276fea3a4eee32bc2dc kcp remediation
60b78dcfe3382e3ab760b790a1a1eb6f2aa1edaa Merge pull request #3925 from fabriziopandini/upgrade-RBAC-proxy
f87f292d9c0394c0efa536cf49f11d023c533d0c remove deprecated DeleteNodeAnnotation annotation
ecc2dcc3d78b38fe581f9bd46c978d228ad8752c Merge pull request #3953 from DolceTriade/DolceTriade-healthcheck-typo
fc8e780a1d4c473570c0c62f32751b56c1a18b32 Merge pull request #3947 from MaXinjian/test
97c495b66014b37ceabb89fa7b86f9616fa3fc7c Merge pull request #3949 from fabriziopandini/clusterct-add-v1alpha4-metadata
4172a3e5b1a6832b70cb070eaf1fee4e5a1c583a Merge pull request #3922 from fabriziopandini/kcp-conditions
510754074a358e4139aa970fdb67445bc2e8463a Fix a typo in the Healthcheck book.
eb7a1a74a6e1ff7a0dfb8c86e9b3aacfb8b35417 add v1alpha3 test templates along side v1alpha4 ones
448082b2bb78d0bd72fb9380e9e6f9e892c97a2e Add embedded metadata for v1alpha4 in clusterctl
e5b02bdbce6c32b4dc062e9e1f14f8ccd16e8952 Merge pull request #3945 from hasheddan/clusterctl-fix
64eaf5780413843563f22d37cf35e2c277dc8f23 Merge pull request #3943 from hidekazuna/capo_v033
a7f9eacfc344c5315e6f825eca4d7c1c6da3b34e Cleanup downloaded file   $ make test   $ ls -l /tmp/ | grep kubebuilder-tools -rw-r--r--  1 root root 52352311 Nov 26 10:33 kubebuilder-tools-1.19.2-linux-amd64.tar.gz
ed19b5843bacb2dc93c1b88ef34a6a559c434d6a Fix small typo in clusterctl command docs
dfa4255e02c79f22c0cf85d259b81bf8070fd8b2 Update CAPO variables in quick start
6c468075924bbca1bde8b83681148bd323518c03 make clusterctl use v1alpha4 api
515a30a6e481d2f93a7bdd333f78d6f305e70033 Add interruptible label to machine node
3de9d53bd581d1e1b3ca0d27956069058bb24d2a Merge pull request #3934 from srm09/align-flag-names
ee5cb1248464d62d9035aa18ac8c44cfc689f89f Align flag names with k8s components
15f0944fad8c1c4ffcdb16e7da3e916609bddfb0 Merge pull request #3901 from arghya88/mhc-err-fix
c9a0f6c3602bfb85437c97130cbe67fa6e01ecfa Merge pull request #3932 from wfernandes/add-capd-k8s-version-note
ace4e245d02d6c4a73ba91534858e9c9a684a169 Merge pull request #3937 from arghya88/un-deprecate
0b10f5c879156f024a48273022aec0ac68414475 un-deprecate WithOwnedConditions and OwnedConditions
52f208f014a10bad98fd956bc6e724032c3ff2e9 Add KCP conditions, split reconcileHealth into preflight and reconcileEtcdMembers, make both use conditions
1e7df1d3c4d609fd1148935cda1c0850d387d519 Add note about k8s version when using CAPD
69980887ff7d1f73f2ce7c6525b6afd824bab3dc Merge pull request #3931 from wfernandes/fix-docker-cluster-template
695068143bd4ab6a10f0ff56d3cfa61e8f959f27 Update the docker cluster template to reference v1alpha4 resources
107f832fca47f67e0efcbf6d94b005d6a3826ddd Merge pull request #3928 from yastij/relax-validation-kcp-main
59911458f8c2c24eeecb6878a2daf035e277f975 relax update validation to allow rotating ssh keys for KCP
e88a34f1f6d731c433586cef9866417a86924f3d Avoid MachineHealtchCheck to return early on patch errors
410024443176ba8b787c24eeb51c9597be2cd8f9 Merge pull request #3884 from JoelSpeed/allowed-remediations-v1alpha4
d7e509c027b014487f9fa7532dcb5cda68f90778 Upgrade to kube-rbac-proxy:v0.5.0
46ad27b69a6abaaf30af309cc51c414c5c8da818 Nodepool should not use Status.instances from previous reconciliation
e6b0039b4aa1021b0a9afec8a527d969c20acabb Merge pull request #3918 from jichenjc/bug/3505-1
28e2067cd6664adc01f9b48bd47687f36eb1f8f9 Add remediationsAllowed field to the MHC status
e4fc3afcc79da313ff529775272a357766163d77 Add conditions matchers for use in testing
5190aefc5ac27e6a4a9b254cbd27cb1716a200aa Remove hard code version and hash in manifest
91b70900dbaffc257b604601c85a166279738573 Merge pull request #3912 from prankul88/k8s-drain-update
ff014c218353f42d06f9dc00aa8ef4f84de84994 Backport of high cpu usage during kubectl drain
defb99c408b54dd8b58fc586eb424425b4198484 Merge pull request #3896 from arghya88/resolve-cni-resources
08260e71b18e977ae47e17101bedc1ec855ccefa Merge pull request #3888 from windayski/typo
e9dd33dfad106de9aca14793604f5afb545aff40 Merge pull request #3899 from vincepri/live-client-tracker
e5551b9d6fac85b10731b8ab5810890be534fd1d Merge pull request #3905 from avestuk/select-infrastructure-provider
d3e8dae7d074912b7161b88827a8d535421d148f Remove leading colon between --infrastructure flag and provider
65ad6b37299e1348e68623d17adf78a6a2a16678 E2E framework resolves CNI_RESOURCES without using env vars
12e5e6b7b7fdb25b796b002eae92bde874e8ba1d :sparkles: Add GetLiveClient() to ClusterCacheTracker
d87a39c85f87f60858c578feaf5192d5679a140e Merge pull request #3893 from vincepri/controllerruntime07a4
a10530fb0193498944baa06e7e08c06087fbae99 Merge pull request #3883 from arghya88/refactor-kcp-healthcheck
ddaedbed1330e44c5569683b34e35dc2e3574c99 Merge pull request #3882 from arghya88/forward-port-mhc
f7f7b9ea81a089b8dee8d304b84551c79320dbf1 Merge pull request #3890 from sedefsavas/machine_condition_forwardport
76242c4e8361b4ca6e0ec8c8f60ca6ff3490e90e Add Makefile target for docker build pre-requisites
84dff24a2dea929ca808688ca02d045c7c552fe2 Update controller-runtime to v0.7.0-alpha.5
463c545165b5414c5d4e9f4a9b5e7a17285ed18c Add Node related condition to Machine conditions
3aac2fc87589f8d5e1e3a1e89c7808889ccd226b Merge pull request #3871 from benmoss/clusterctl-debug-provider
a1b6969693e0bca8c06741c99d632230984e2280 Merge pull request #3870 from srm09/debug/wc_dns_test_flake
4bad4adb5e04cb9aef163ea98379675ecb5abfb2 fix typo
7bd35f2fbce7adef40c89561ba6da746f07be0d1 Reworks test to add cleanup for each subtest
71ba9246f9cd2d718e81866cdc869c10fb90a9e4 Merge pull request #3864 from maplain/check-kcp-to-avoid-draining
dc5149cf2c823eaa22a226a1c85d447124437995 refactor kcp healthcheck
79de3f463a184b341359eafb28c40afb7b35b8bd forward-port MHC external remediation
7424a1a6cdca5c5973ea90d04cabae339622261f Merge pull request #3877 from sedefsavas/fuzztest
1232dca3a8b519f737f2845110fc64a4179935cd :seedling: Avoid draining when KCP object is being deleted
a0d10c19c481143ec8ba71cadb66ae41fbe6b2f5 Add reverse fuzz test
88d751cf2a7f2aaf918c6e294ed9532cf8988009 Merge pull request #3869 from Evalle/ISSUE-3859
17c482f124bcad09e1b41c43e31fa5e62c75d9f4 Merge pull request #3817 from alexander-demichev/labelproposal
6b3eeb3240a637194b5f95ced42818389fdd4b20 Print provider type and name to match config file naming
d737e273e731784dd672a9fffd5c14870ec57e93 Forward-port modifies DockerMachine condition status to report for control plane to be ready
5ac19dc6a5f78f98282f13d5159dcb2d91e4d89f Merge pull request #3853 from arghya88/update-corefile
205e25fc2d2a04ed6eb91a35b2917d386cd1d095 upgrade corefile migration to v1.0.11
d270d985a0b93c14337db5cbf480d69ada252a5d Merge pull request #3852 from eratnch/update_go_version
6e1757a77bf0070a361f4d805ed4b57cbab8a55a Update Go to 1.15.3
8ceb23c29144669fd57a75672b70c9de39ad80db Merge pull request #3844 from arghya88/refactor-testfile
0b1108ec4722450ffdba89e4ff36e646bb1aae2e renamed machinehealthcheck_status_matcher to test
2dd66d6e1559f47302c263cd75bd20265ce6403a Merge pull request #3749 from srm09/v1alpha4-types
36611d1c4b8050fbd615f49c9c3b80f598554679 Merge pull request #3815 from tcordeu/kind_v0.9.0
e73e3d9021e5df61ea2861be6f73698a031a63c3 Replaces imports with v1alpha4 types
46d59bddc9e193c5d91e49d7d457d62ad8ded921 Generates exp v1alpha4 types
0bb5410deb63c3f52f561af7d76d80141e4eb3df Generates CAPD v1alpha4 types
6b5d2f022339262378aef80619372d7a62266ac6 Generates controlplane kubeadm v1alpha4 types
b54e3ed50115f4b02c8a8be499330ae45709d07d Generates bootstrap kubeadm v1alpha4 types
0ba375c75ad2e778f3afa50b6c593c079df4f303 Generates core v1alpha4 types
28c941aeb7912411bcb195af47c99bc936f8fe0a Merge pull request #3767 from vincepri/caep-releases
b84b8630d707877ade92311e097dad4df71df8b1 Merge pull request #3754 from vincepri/roadmapv1alpha4
8d42ca098b8901dfae571e154790194d10ef3f24 Merge pull request #3841 from christopherhein/bug/proposal-link-update
69c6c2eba70e98b01a88111e7dc40e69c5b8418a fixes link to proposal root to /docs/proposals/
169440de58bb676909af1e400f8cede84d0120fb Merge pull request #3823 from benmoss/docker-list-output
a6cd352af6087dbee423d1208037912105163b1e Update Kind to v0.9.0
be5ff75585e4762ae8ef2a9166dcfd16a9f2b8a1 Merge pull request #3827 from prksu/add-capdo-in-capi-book
1319d61c6efe09dbe5e72a199317d90342cd90cf Merge pull request #3826 from sedefsavas/forward_port_nodewatcher
a58b8e5043a219b9bc0a0c1542ebf454de988bf6 Update spot instances proposal with interruptible label setting
2ceef1db4e1ddc490403f8ebfc6ba4ff80eb3c6e Merge pull request #3814 from Nordix/update-capi-book
7d96ce2541be2245f0d4e1101c2ac1ba9d387abf 📖 Add CAPDO quickstart in CAPI book
9e99cbf51cdd602f5300ee808bbf0d389c5eb3cb Add node watch to machine
c60114284e73f1f0cff96a3387ab92dc7344a04c Merge pull request #3820 from rawkode/fix/make-cluster-config-copyable
c1647481f73cbdc96dafb1acc62f993c60b2e34d Merge pull request #3616 from jsturtevant/capi-windows-proposal
96812c1631252c9903e98b6208c6f1dde35190a2 Log docker error output when we receive a non-zero exit code
5e742a6a02fbf68a0fec2925ad718317047ca4ed 📖 remove single quote allows copy / paste to work with zsh
f1d05fa61091f8989c1d7811a3975eeec63cd1e4 Merge pull request #3719 from Emc1992/readme-docker-1
918d0de588d6c5407d9c698704a85e6a8310d75d Update required configurations for Metal³ provider
0008b5ba109e839067b96f4c5b52eab9fb657eca Merge pull request #3775 from eratnch/tilt_cert_manager_ext
c1a858cba480263ffb39d084d52672bd1d636359 Merge pull request #3809 from prksu/cctl-fix-do-provider
c7c0fd749e447ae178960cb4b378b00bbef9994a 🌱 fix digitalocean infrastructure provider name
07f14819c150ee33d93b724ac752f9d53950e138 Merge pull request #3790 from fabriziopandini/rework-skipped-test
eec97b12a229e6bf2ed5635ef874bf4d3716e2f6 :book: Update the roadmap for v1alpha4
c60ae8bc54168eb53fbedfe5c788f88cf4af8d39 Merge pull request #3776 from arghya88/remove-tmp
eb011e6a0dec8446a991c96be9bfe15399bd495b rework skipped test
405040671f05be96502b1d2f8d0e6b3b1b640b2d Windows proposal
6404141e933ce31fae6d48841e10475c843a2ba0 Merge pull request #3794 from fabriziopandini/use-controller-runtime-v0.7.0-alpha.3
5151aea6563ab14ccb3314e29e0999a9b00f0fb9 Merge pull request #3788 from prankul88/update-init-help
7ca692a4cec04ed8e44bc920b979cc00b84a2a32 Use controller-runtime v0.7.0-alpha.3
38d797175464a6f0b4d2e7546eaa04ef85d5796f Update `clusterctl init --help`
aec55906f6f4d254831e712513498662b247cc0f :book: Define proposal guidelines and policies
ec91428c7c415c65e8467ed6e45b24623db7d1f5 Use tilt cert_manager extension
51b6068cce12b455bc5d8ff70f0c3b7e319f2b70 Merge pull request #3730 from randomvariable/kubetest-machine-pool-support
b4cb2fca47edfd2e16d0175f035bfd8a5dd0fda1 Merge pull request #3705 from srm09/feature/add-conditions-to-summary
6a39a222f726ba2efdcebd7662af69d0879d4cb5 nit correction
ed580e2b92e3ebfbece20d31407c24c443432da4 Merge pull request #3768 from vincepri/gh-action-verify
08a9593c2ccaf755a25b05357e26b0db781cf9d5 Merge pull request #3777 from muench-b1/patch-1
8357d5572bbd594c59857836e8ff650397814e39 remove usage of /tmp in capbk
22f7d4ac5469710556ff5fc391a92e150fc7a2c4 Update quick-start.md
5e04d903be382112d18a31f206cc153ec75e24f5 Merge pull request #3774 from dswij/tok-log
fa9939dd2ac925e94eda6210912943e6bfd9e391 remove token from log
3dd38537ad8eb507d7a8797cd50b4328176abb20 Merge pull request #3735 from vincepri/controller-runtime-07x
8cec72bfafecb058d4bedd6ec73f024a52b8934d Merge pull request #3592 from Boutheina-Dab/capd-machine-deletion
15a2e4bee7e1e1b2543a9511b2c4ac50f1c7a5b4 util/patch: Make sure that objects are created before acting on them
1469b1ff9f489d7ee2057614864825dab8f2cb04 Cluster controller delete flow can now use client.Object directly
67a95dc9d8eba77f031917d686b9da369d91f95f Use context.Context throughout the codebase
1bcdf22c460fb016b0a70505c45b86b3559d5e46 Rework kubeadm control plane tests to be more consistent with the rest
9eaa3f543b34f6b2d024d2dc749dd2acf39a2137 Mapping functions now panic if the type doesn't match expectations
2a2d0e49ccc31cf1002e7259e2d66244c203e5c2 :seedling: Add github action to check PR contents
ae6e932ab0ee0bf0b545135bea7964dac4ee7561 remote/cluster: Use context for cancellation instead of stop channel
13b2351494cec41baed94fc92fdb97722ab4decd Use NewDelegatingClient function, the struct has been removed
2fb95900850630b6594172cd8afcda1aebd37eca Exclude tests that should be reworked
737f435a4a269ad7bc18debb17f209842d2bbadd Clusterctl cert-manager test should handle both webhooks v1 and v1beta1
f462eb14ee3346e14a57fd40abeef666b7e92397 Update kubernetes-drain to use contexts
c553023952d4e2e766d538d676044d4b74120060 Remove log and scheme from reconciler's structs wherever possible
f918f452bef11cdf0a9c0f83672a87c348a3a38d Use handler.EnqueueRequestsFromMapFunc when registering map functions
c58bb2e08e7b595e1b3589f4e45e336e4c16514a Controllers SetupWithManager now accept a context as first parameter
5b6a2abf320ae9722fbe84068bf4c089c0ab838e :warning: Use client.Object instead of runtime.Object
ab6faac1080af960430ab7437ceaa36c651324e1 Rework envtest start/stop to use a context instead of channel
34bdfc7fccafb7e1d81eb7b6c0307dab330002fc Pass context based on signal handlers to all managers
5b81666213a7fdd428b41ca3b0e3357d0704f796 Update generated CRDs
4d1816db343958fc3d248f93009a892c2d3ebdff Update go modules to controller-runtime v0.7.0-alpha.2 / k8s 1.19.2
9cbf8be8d643203d99aca6714825abdabcbca0b1 Merge pull request #3724 from vincepri/releases
edc1b8f472cfa43a0a4141dd97df36594903858e Merge pull request #3736 from elmiko/move-autoscaler-roadmap
74303e90437a349eba7253814819422198f48fc3 Merge pull request #3723 from sedefsavas/machine_requeue_after
c7d29f15291ddda710d96f983867aee8ed313ab9 Add RequeueAfter to the ones previously had RequeueAfter.
a82cfd9346b1d1f45668dae35c3dd5e8ff413c89 Merge pull request #3759 from vincepri/use-live-client-kcp
a7690b77626c5a520ed1bbb18e56f3eea7c69792 Merge pull request #3757 from vincepri/patchtestnamespace
bdb88e1d42bf8747f6a3df2a003051977598a526 :book: Add release guidelines and policies to contributing guide
fb5b8e991c13c78e86b8c072b32b150d33936f37 Merge pull request #3758 from vincepri/use-9443-port-capd
c285f2d753465d2adedcbea04320d230ef8f8443 Merge pull request #3756 from vincepri/leasesrbac
58768307a894c9f5c61475a6d4c6c2eca45afb4b :bug: KubeadmControlPlane should use a live client when listing machines
4181b72cfa17f39af7972df2c1f1f19c4aa4c9c8 Merge pull request #3755 from vincepri/newclientmanager
56b5822b8e228810cf20a46d43412bb0f3a97b39 :seedling: CAPD webhooks should use 9443 as port
b39f29e372802d271b9feea9c289feb6568b9ccc :bug: util/patch tests shouldn't use a non-existent namespace
2c24281026929effac8af568f45ae0fda80fa1de :warning: Add required coordination/leases RBAC for v0.7 leader election
5774dc083476b73e277650ca4b3119609684e299 :seedling: Use util.ManagerDelegatingClientFunc in all managers
1e90432b58ef08af7056202e21df6b281a13cd25 Merge pull request #3753 from vincepri/controllertools04x
3b1ccc4c08168ea06bc70de1147d848948b83ec7 :seedling: Update controller-tools to main tip, use webhooks/v1
bc3c0e82071db440a792bc855429e57450727d7c Adds healthcheck conditions to machine summary
7fdecfe013260f6ca4dd5afa1ae72a37766f7506 Merge pull request #3746 from vincepri/min119
233e30a4d53e8d6e288f6440c8052a07c379cbae ⚠️ Update management cluster minimum Kubernetes version to v1.19.1
a4625808f1de59af0f1318d87fa231a11e010cc9 Merge pull request #3750 from fabriziopandini/e2e-configurable-nodeimages-for-bootstrap-cluster
8ae4779c6ba031b4aed18ce58f89ab758724ddff e2e framework allows choosing the node image for the bootstrap cluster
9962a01ca981385318f2d57e49377b9ef5c9f965 Merge pull request #3744 from vincepri/kustomize-build-fix
fdc0632f0c262a5f26c9152ffad138d5c2f8e08f Merge pull request #3742 from fabriziopandini/cleanup-e2e-framework-and-helpers
042ab21c5e761139ab6ba43f2bf54edfd25ad552 Merge pull request #3741 from fabriziopandini/remove-deprecate-func-e2e-framework
d9fcaa1cd6eac068a2fc9b1cfc65892d7791f8bb Update generated files
f9f6293ebf6c3c6aaa42d1e6db21e4feee79be53 :seedling: Retrieve kustomize release binary instead of building it
7474f66deb78b6b906c736a921f4dce50da010ff Merge pull request #3745 from vincepri/kubectl-client-update
34a036b7391cfbcb46dccb9893127b42559c8c80 :seedling: Update kubectl version to 1.19
f728084ae97006def107dfe0f000b07893745f14 Merge pull request #3691 from cpanato/GH-3322
1bf7a640150189d3efa1ceeca92d4a520f994dda Merge pull request #3737 from tcordeu/fix_create_local_repository_doc
d2ff718f9af60c6f9079e6c5bcd9ad63579b69b6 cleanup old function from e2e test framework and helpers
d83cb0e4b25766f302f063606c9dfd8ec6b29a89 remove deprecated functions from e2e test framework
1c541d922f20b343ff68be459ca489d8d28745b3 Merge pull request #3740 from fabriziopandini/fix-condition-counter
d589bcfc2affb927bcd1e47a2c116d2dbc227024 fix conditions counter
b9a16e24e6e0ff42b4a13fdedaba51e47fbc10e9 Fix create-local-repository.py documentation
48077988ec713a98451cfd9793be9b46b768f768 move autoscaler scale from zero to 0.4.0 roadmap
e94d4504382dadb16501468699569ad0f8a2e524 kubernetesversions: Add option to inject CI artifacts into a KubeadmConfig for a MachinePool
af6630920560ca0e12179897b96d6ea8bd830b63 Merge pull request #3685 from richardcase/eks-controlplane
688d6d72bcee03e2aaef14faa0d1e8de17ee5977 feat: add EKS controlplane provider
9e2a7c7a886a9e3a06e7b67d9a2e4661991eaf5c Merge pull request #3688 from srm09/feature/priority-of-conditions
50f5f6ad92ee4c0e5d3894d7b83e7da4fc774133 Merge pull request #3725 from vincepri/fix-makefile
4f267e0e161cc58933e70a23752203e3771eaa86 :bug: Fix Makefile target to clean-release-git
c997c1e5cc64b1f70a6922b9984b914bb49fed30 Merge pull request #3721 from arghya88/avoid-linking-master
87ca420d1ff2fe1bacfef74443acae288366930f Remove RequeueAfterError from machine controller
bcd80d18ba56e0586abc6fd271018eb417af579c Avoid linking to the master branch of repositories
eface850bba38fc52765c5d48efd8cb29d73a994 Reword docker readme
7523f71dfd58a8c4e358b057da611546dc72fdec Merge pull request #3662 from Nordix/node-drain-nam
d4fe42f8f6751c186fb7273ff87731a223d9ff6f Add the ability to specify a drain timeout for machines
5754973fbf6c4a35f3af2e2d01bf64b85b935972 Merge pull request #3673 from newrelic-forks/issue-3631
a0a8a75b1f02db5041f6a865f0c1946cb5f22e64 Merge pull request #3703 from benmoss/dead-link
cc86dbaf0dfd4863962c50aba1effb3a193a527b Update broken link to CAPA prerequisites
cddd57babe2a1cfb29973d9339f6389dd5130cf4 🐛 Fix node deletion under managed control planes
626a8ce3be9ef7116de032341304e77999867cad Merge pull request #3709 from randomvariable/update-netlify-output-dir
f598caf8bb28dd78b2607c19df75e7932f605e28 book: disable link checker in Netlify pending access token
cc0126006ae6a212084878960636961b8d23083e book.toml: Update bearer token
fc43e7de3fd7aec99ff1ed3e98293bb57e7df9cc book: Ensure make targets for book building
0b605cb9bb9baa5f449dc6eaade1f7e0139bd7d3 Merge pull request #3479 from benmoss/e2e-cleanup-kind
d54bfb157d915eee1438f7e330b051afbed34e62 remove capd's machine deletion
26c6cc5a4103750fe988dc66e294078b2b14fd83 Cleanup kind cluster if it fails during setup
863a791a82d7c8f426b5e13540d39c03cee3218e Merge pull request #3627 from srm09/feature/add-conditions-to-machinepool
9b75eae0ce4dce8110dfadedb65605c798eb3f89 Changes priority of machine summary condition
aeae5c380fc6ac6a5481f3024b31b182f4503887 Adds conditions to machinepool
7bbd5cc18d0bc9c298789a1cdd50749599abbcf0 Merge pull request #3704 from vincepri/fix-manifests-build
8addaf0b31991501aac71da210f4b8ea8b2ce244 Merge pull request #3643 from vincepri/conditions-force-overwrite
7d0deb18b44305a993783b50d7e2ee458615ff3e Merge pull request #3687 from fabriziopandini/fix-e2e-log-collector-errors
05da807ddcfa00f285d642d985e9f1a1abca9df6 Merge pull request #3530 from randomvariable/upgrade-statement
bb05b6dd1fd680c304ca72566b81ce33ffcaae2a Merge pull request #3637 from jichenjc/remove_todo_1
6612afe3584a8341e849b99dc20042da376c930a :bug: Makefile release target should properly clean the git tree
b0d942e280592e890233fe59afb4927ee23469ab Merge pull request #3701 from srm09/feature/remove-step-counter
6c0f1992bb841d6bd21a417e12969917985c987f Merge pull request #3699 from CecileRobertMichon/cabpk-docs-2
b0e6ca3e04a02376544c1f43e94a838964a44dcd docs: Update upgrade documentation
9bb9c95f846a0f2cf85f7a1b61ba63cd80c5cce2 Add virtual node checker
e20e01aca078fbaaa3569dd21d5844a9d9e9ab0a Removes step counter for kubeadmconfig conditions
d66eed92a1ca9041908055096ca8f7625c5f9df0 Merge pull request #3633 from wfernandes/fix-flaky-mhc-tests
7fd7788556f191adec0aca49581ba147efb8ba26 Refactor MachineHealthCheck tests
712090d93cdc928aacfcfa13f63b30395f007384 :book: Move CABPK docs to book and add examples
59faa7b1c63ba301cb780836891e7b10098fce34 Merge pull request #3652 from randomvariable/test-framework-extensions
b0236f2b3c1d0ee9e6a8dffd1baaa22fd8aee17d Merge pull request #3676 from fabriziopandini/kcp-remediation-proposal
ccb4ad5362f5ca57dcc3214cd2c69c87f916c287 Merge pull request #3506 from devigned/e2e-mp
07515f6ba2c0370515335e247919c85dbefddb25 go: update to use go 1.15
56479832c7f7fee2f3af85bef9fabf18e0db0ba1 fix log collector error
0d915622095b879313aa72917f112618b5ede5c7 kcp remediation proposal
f631989d3f7430b5825644a5461e116f48ed2e28 ✨ add docker machine pool and e2e tests for capi machine pool
f06e2109dc9cc497e917f34d226413542aba5b51 Merge pull request #3675 from fabriziopandini/increase-sync-frequency-to-fix-e2e-flakes
e59acfae1cbef54d3cc55efc20666df7e785a2d0 add docker mount to control-plane nodes
bf34fd0de176ab12202bd41992ac4a888cf1d767 Merge pull request #3657 from fabriziopandini/remove-e2e-templates
47ffedfe62b3af67a7a3f9da5669022c089594c7 remove e2e templates
995578c4e53a392806adf0a81c29098d7612a559 test framework: Add kubetest, kubernetesversions, ginkgo extensions and additional suite_helpers
3158562c6ceca6015fe18974fb8fe9ff577ab31d Merge pull request #3682 from jichenjc/fix_e2e_link
8137d2d6a3449c1d73cb9ec605c8f359fd85c95a Merge pull request #3681 from jichenjc/add_CAPO
6d5d45211a37bd98d1ced354e81e8e0c969c8537 Fix e2e link test failure
57e3c05232ae202e2fa87968ad11811fd084b22a Add CAPO into contract list
9809625ca3b3776822b0a413005cb357779b522c Merge pull request #3474 from benmoss/verify-links
c00d3f2550057ae6ec8a54523a75384e62379441 Merge pull request #3671 from detiber/proxyIsh
756cc28ad115a328d7d46c259af304c986cac32a default GOPROXY if not set when building mdbook preprocessors
456152e445e4832688c2bd1f7d77b897abe6edd6 Merge pull request #3672 from sedefsavas/etcdbackoff
456283674fd02aa3a38eaf69586c5b90099d19e9 Merge pull request #3648 from Nordix/fix-write-local-repo
a17523e11627a09cd35a300b9ef234299f78b2e9 Fix yaml file write issue
34f63a1941dbacc7827aa62e1f715c2cbb7af0a2 Merge pull request #3598 from jichenjc/mover-dry-run
00a9f3e7342d13fbfc4b7e41dc8bd475d4d7031a Support mover dry run
c90be1158bf7ce7b09b21fdf602e552d5fdcc8bd [KCP] Remove backoff adaptor for etcd
469a7cc1f19f40b6f085fae60daabd53a0042e83 Switch link checker to mdbook-linkcheck
2ea9aebd94c329c5322d8ffe8927104607478361 :seedling: Support patch ForceOverwriteConditions option
1930c00e67b3b0c8556346169dcb87639650a08d Merge pull request #3667 from fabriziopandini/increasing-e2e-timeouts
8305b7c49c695172f4a2235db5b261f09dd9be22 Increase timeout to fix self-hosting flakes
630e25128c52edc3008e6cd839c3d647fc831d70 Merge pull request #3665 from wfernandes/cleanup-suite-test
44440fc03555260676676eb7ca84bc4473da31a9 Remove unused ginkgo suite test setup
92f416c66a5067c26dbbb97abdb96e9fe7cba55f Merge pull request #3630 from vincepri/save-deepcopy-calculatepatch
3ce0d8e45855f97fc0f9125ff141e1ddd0fd620c :seedling: Save a DeepCopy when calculating patches in Patch helper
cde112b20c2e9b126d74e9804ad353e1765ecdc1 Merge pull request #3654 from ncdc/cluster-cache-tracker-single-lock
f881755d4897695b28b4759ec4253c423ba67e56 Eliminate possible deadlocks in ClusterCacheTracker
b545ca1215fb5a294f3b150c1b7a5296a2c59c77 Merge pull request #3619 from jichenjc/bug/3603
bbc7e01a283c2a5407f63f151ac5a719ae639d3e Merge pull request #3644 from iamemilio/clusterctl-get-kubeconfig-docs
afd30481dbf487c1e6a926c9f6c5564eb9011556 Merge pull request #3659 from vincepri/mdbook043
658b999688e49be04b74cd00f6a6cf83660e7acb :seedling: Update mdbook to v0.4.3
a206cefe84e70257a2932363954e87fe034e0c90 Merge pull request #3655 from daschott/daschott-azstackhci-provider
7e04a454d9623e75175e02a070db562f86b7c559 clusterctl get kubeconfig docs added
0e886b905a67c68b5bce3f249aaff13079affeeb Add force move support for object
3de6ddab22f00df739fd897b2cfb9bfcfcd927b5 added AzureStackHCI infrastructure provider to list of providers in the CAPI book
0cf9f80b63047b0694b668bee6eff6dfd046e16b Merge pull request #3639 from fabriziopandini/fix-self-hosted-flakes
b79d3ecb07e57e2e772740ccc46c8e8663ffd9dd Merge pull request #3651 from fabriziopandini/use-kustomize-for-e2e-templates
a1c55534a922a3ea71ea2700c9419624cd2da25a Merge pull request #3622 from superbrothers/clusterctl-completion
f96d5f0fcf8bec2cbaf40f17799591eda4eacbb0 Merge pull request #3650 from fabriziopandini/fix-kcp-adoption-flakes
7d4dde83613cf4fe643907f3668a7f1b945448e1 Add 0-9 to `make help` to allow *-e2e to show up
90f6e46b599ad1410a0563d03aa29a2871ebdf59 Merge pull request #3649 from fabriziopandini/fix-e2e-logs
40011b92ef08b4a28f530ed5086c5a1b84c488b0 use kustomize for e2e templates
e2a5f899ea805b1558178f817ee817d6111bf59c Fix self-hosted flakes in E2E tests
c6695254332d9ae3fe6d0427ee10b99fa7cc3128 fix-kcp-adoption-flakes
d2db1dbfa8af368d66d792421d08894104deab97 Fix e2e logs
624ddb00abdd7e6972b5cf37a16ea8977c3f7fb1 Merge pull request #3618 from newrelic-forks/new-eks-bootstrap
2c4ce19571b420455080d536a30d816cc4c64452 Merge pull request #3646 from vincepri/updatecr0511
b89060987b34d319211679330abbb9a01a00d8fe :seedling: Update Controller Runtime to v0.5.11
0db3effb8ab0655d781090f9afba441bf66e6cf1 Merge pull request #3642 from fabriziopandini/fix-machine-conditions-ownership
9293bd61dc021bc5745e73ef4df4db8d0cc42a1f Fix machine conditions ownership
e734f29cb19b6e1f63ab46799c9ffd2495237055 Merge pull request #3605 from fabriziopandini/update-KCP-proposal
b068d9498b9ff060a686515758444c29f1722363 new eks bootstrap provider in clusterctl
20a302a01bfa74389254059edea09694298dcbcc Merge pull request #3636 from vincepri/fix-bug-hasowner
3b06cb1d24634ad74df4963356957c031312dd5e update KCP proposal with latest changes
178fbbfd5d5176b7475ef3a9a4e7735b2cc07718 :bug: util.HasOwner should not compare with the API version
cd8ac0570e854e88839b69818490e54ee22b8ccd Merge pull request #3617 from gab-satchi/3558-clusterctl-delete
dd5a68dd19272aeddb70b9ae568d2e40828bc11f Merge pull request #3634 from kkeshavamurthy/capi-cleanup-doc
8c3e0fecbd195c6ce5d9822c197f38de54f92b08 Merge pull request #3628 from vincepri/save-deep-copy-patch
e54af12cedb2f9d446dbd28f51418237b7efafd0 Add a documentation for the clusterctl completion
5002af40fdbb57f5b39a9b6615347cc2d351b9d8 Implement "clusterctl completion" command
69f292ed0a9c019ca6eaa8a49f5729b418320169 Add CAPI Clean Up section to Quick Start
c8b8d0f98f4b2ec45864cebd611c4073b7c8caae Merge pull request #3632 from vincepri/delegating-client-tracker-cache
211334dfc190b9f5ef7e598cb3826e10ac598efe :seedling: Reuse the same RESTMapper for cache and client
feaff31a93174f79929f1264f47f8ad057577454 Merge pull request #3629 from vincepri/update-go-11315
19e40cd536d5ea0296599e2678e7cc70e385b452 :seedling: Update Go 1.13.15
45de611901c6e18c07c5831be2936a4e57e816eb :seedling: Save a DeepCopy when patching typed objects
7f8fa2d1799039de04ac32a046e95400bc9f060d Merge pull request #3625 from vincepri/metadata-only-crd
b315908a3acef50cc8a44f173ddc7af33cbee4dd Allows delelting multiple providers at once - allows for deleting all providers in a specific namespace
a407dad675fc793c38168aa5cefddeb74afd6258 Merge pull request #3614 from bboreham/python-nonbinary-scripts
6dbac9defd3593a22bd9ee33a5bace351b50a466 :seedling: Use metadata-only client when retrieving CRDs
159064c9c213d60a594cf41b9b378462a8bf94b6 Merge pull request #3626 from fabriziopandini/fix-tilt-file
7bb327184cf3969d4336e6660f0eed1aafca6630 Fix Tiltfile
7d142cbc0d770bc210625547769f1f506efa6fb0 Merge pull request #3553 from cpanato/GH-3099
a76329aa7af2b65f6cf80ed3d582116086824754 Merge pull request #3623 from ncdc/predicates-logging
2e1d3770c320869fd96f9c82337dd3a328f8ff1a Merge pull request #3621 from cpanato/add-capdo
d6cfa9b3942df1ac25104cc3fcd6a580d94c1724 Merge pull request #3615 from ncdc/fix-cluster-cache-tracker-healthcheck
8f42e8a5d991a9974502983bc581e1008028277d Merge pull request #3624 from ncdc/remove-crd-deepcopy
2d50424bed42111c18083e2d68782f7ea1b17592 Eliminate extra DeepCopy for CRDs
3f9f021b4e15f6e3a183a07ea9cd456177066f47 Move log delcarations inside closures
51d643c4e6c6d3e667489faf61892ef8153ae1bd Fix remote cluster client healthcheck
783000678b05616733d271168db8b34c0f83fae8 add digitalocean (do) to infrastructure providers
f49a68055226be1ee62af4e047933484faadc387 clusterctl: add option to use configuration file in remote locations
51ebe7e8082f861611259df671b01f19bbfbfe11 Merge pull request #3613 from bboreham/improve-conn-error-log
74fe8f5945f19ba1f3e9ae66a90a17e78e27fc29 Merge pull request #3612 from bboreham/fix-crd-error
eb54308618c15350699e4df98bf9044ff2df6f6b expand CRD error message
73624ed082e948e693a14484549b3db53c1b7ae1 Merge pull request #3604 from Nordix/tilt-mael
ced376ef9b542b73dad679e0af954446d9688d94 Write yaml files in native text format
c266a6572514d6b0b61721d085a930c4cdcb9239 Improve logging for workload connection error
4324e956c07dc5f338b2784f79d634bd38834e8a Fix message for clusterctl EnsureCustomResourceDefinitions failure
e5f9ecd9925b643ee2c63f951edc3e72bed825e0 Merge pull request #3602 from jichenjc/log_ignore_secret
6451884dc8fbc2a0c5fae8677beeb4599e801841 Merge pull request #3600 from fabriziopandini/fix-e2e-mhc-remediation
47409bc9a9174285683063421f0cf5048f928853 Merge pull request #3596 from superbrothers/e2e-kubeconfig
ba17094d8da57a9bd030111636a10f81c471b40f Add log to indicate the secret is ignored
938d36f85324c285455c74dcd91e5e96ade8e2b3 Merge pull request #3586 from teoyaomiqui/master
c633616dd8b945d2ee41ca999013597f6d0cf52c Allow custom providers in clusterctl client
ca6113262fc8e9af4b30d4c0cdb5f05e865eda4e Merge pull request #3608 from randomvariable/clusterctl-api-restore
953304d1cb59b650d227a069ba301df515e645ca Merge pull request #3597 from superbrothers/fix-typo
f19f4a7bb783cc015dd272fd60e15c979082944f clusterctl: Restore CNIManifestPath to struct for API compat
cb929794b9481b598bbaeb8158ef9828d1245643 Tiltfile: add option to change provider go main file
0f5b6d54967714925a75e1e768a39b4849fdeede Tiltfile: Parameterize running kustomize on provider config
e476b4cd23421077225656f719fcf43cc1bfd9a9 fixes E2E MHC remediation
5164a1f0e2a9f4bb6c1c3ebe304877ee470ac9c5 Merge pull request #3585 from wfernandes/e2e-fail-fast
da74db43626718a8c0515402d32ba15ceb79e74a Fix typo for "controlplane"
07f9783c2e66a86845a69c0ab58ccddf31467baf e2e: Display path of the kubeconfig file for the bootstrap cluster
a260cb4c3b2cf2f32379f6ae5d8c6312780e9ca5 Merge pull request #3580 from fabriziopandini/e2e-get-machine-logs
2acfb0ca77657abd41b58116f1e0584cb0d2b266 Stop entire test suite when a capi e2e test fails
7c24f10b05ecd70eb3f56e6d2925f0c3243bd9e8 Merge pull request #3578 from Evalle/ISSUE-3561
aa62f9ba71154aae851d05b7e2466bdb4c63701e Merge pull request #3590 from fabriziopandini/add-how-to-triage-e2e-failures-docs
5037a94b606f2016f129bf677ee97c7e9b5a7139 Add LogCollector to E2E framework
53ac7069c46d0b2ed11adfa0c569868c88086f6c Documents how to triage E2E test failure
e0e4f964ec2a4ddf85e08c6cda927c8c8cbeab5b Merge pull request #3588 from CecileRobertMichon/m-ssh-quickstart
cf467a0fefea032290e3261ee89d98e3d7623ca5 Add version print column for MachinePool
edbf6310f93c71f73e4e41cca0e36dac9db8e3f1 Merge pull request #3587 from sedefsavas/e2e_ginkgo
ec03e95f65c4382371fd746dfaa1dc8aa43fe12d :book: Simplify Azure quickstart and remove optional variables
6abab65da8c136b53d023fe3ee4a53b4d6a16f7a [e2e] add quotes to GINKGO_FOCUS
5a1dc25fd0ff30572b6b4e49d5bb24c81213d480 Merge pull request #3557 from wfernandes/cert-manager-upgrade-plan
4a9cbb8451ab5bfeba35d40be594e5f2ea7d331d Merge pull request #3552 from fabriziopandini/improve-capd-error-logging
5d131b533cfd02f2d426eb341e6de205d7c443b5 Merge pull request #3583 from sedefsavas/delete_ginkgo_focus
2ddb799f706366a4bd175889570bd4df0267b29b Merge pull request #3582 from sedefsavas/pr_blocking_e2e
6701463acd1d997dc39dfcae38991698876fd03b [e2e] Delete GINKGO_FOCUS from ci-e2e.sh
d5819a018486338922ae39b069e78b5822f17234 [e2e] Add Quick-Start test PR-Blocking label
9a1948ee0bc7226f26276d778b140630de88a04f :book: Document our compatibility notices for sub-folders (#3579)
0750183f8efe59eade230f01ac2492958ba00fe5 Merge pull request #3514 from fabriziopandini/simpify-CAPD-quick-start
82e7f83d63a98a4bb77ec1da52d29ca07c723c08 Merge pull request #3575 from superbrothers/fix-write-state-file
a9c75fb2374d5cdd5e9e7294a5f404bd2d92f0ee Fix a bug that fails to write the version state file
c07b9db619118ca88206744ca41731b7c355bfe4 Merge pull request #3551 from vincepri/fixup-kustomize-tilt
3462a5c366df18a7ca33d6b3a2463f198fe0a6a4 Merge pull request #3548 from danniel1205/update-providers-documentation
0154e3dba372ed49324b8664e52828334f15044d Print upgrade notice for cert-manager
6a23c275737c81514e8d6130e7d9fed8aaa1f032 Merge pull request #3567 from fabriziopandini/e2e-pre-pulls-kind-images2
e62357a5cf782b74f809fe2e093c4cfaa4717dfe Merge pull request #3559 from vincepri/enable-spec-verbosity-kcp
8f0485227dff19064f6625cd912b53878a464130 Merge pull request #3549 from fabriziopandini/add-deleting-failure-reason
09ac0492ba639a8518e15a23bc2b477eec93f286 pull e2e images on CI
c4ff8e19556a29b4ef5746fb3afdccdda1333b40 improve CAPD error logging
e1f67d8ceb1d5b30ef967035f7a0d1b1ee088b37 Merge pull request #3562 from vincepri/disallow1190upgrades
df133826284cc9f93ee599158377e05e3dcbb8fa Merge pull request #3556 from fabriziopandini/e2e-pre-pulls-kind-images
4104be96ac6585462709ff82fda4ecb238e22acc Merge pull request #3560 from vincepri/add-version
1fbeb75b2e78caca0e19d8f2af504f974a9ee30c Merge pull request #3563 from sedefsavas/revert_e2e_kubernetes_version
3ea51900a4d7941faeac4da06bd75ec44c91c1c3 :warning: Disallow KubeadmControlPlane upgrades to v1.19.0
61406bc891cb6fc46ba738e2d5d474712ac05cb6 Merge pull request #3529 from sedefsavas/expfeatures
c734ca1af3068b4b6d539536cf83092d8d2618e8 Revert e2e test Kubernetes version to 1.18.2
d8c5c1def622e31cdbc0d89cdeb9d230dd2e7658 :seedling: Add Version print column to Machine and KCP
7904d5b638679ae8ce024e12bb7e8585e1327cb6 :seedling: Enable KCP kubeadmConfigSpec.verbosity modifications
4e263c41e8662bdbae0977e31c64747085dcf8e3 Add experimental features section
14d2705398eeaf9b1c5cf922c67aec0c5264358a pre-pull kind images on CI
0411ca37e3034cd4fcbc3b9915099e0ece9906fc Merge pull request #3554 from fabriziopandini/bump-cert-manager-on-e2e
be789035a8db9935ff8f1cf4c04e0e45cebf7de1 bump cert-manager on CI
753725cd4f5b35ab880bc85654eaadb3ebe9e15d Merge pull request #3550 from a-mccarthy/update-owners-file
aac511372855e423028422b156ff0aa22f5b736d :bug: Tilt should use a supported kustomize version
fdaf422b4b30381ddf42eaea88577355888bc621 point users to owners_aliases file
d67b831fe3b3b3c7bc9afec6e0700b5d7fcf9044 add deleting failure reason
9315b344e9972d7984e76983daaeb64ca6aec163 Merge pull request #3546 from vincepri/update-cr
897db52649325ef498385b35e3e7e2820dcd8754 Merge pull request #3545 from sedefsavas/update_e2e_to_1.19
10d5be07878bf4212e0875689a474bd464d3c7de update the misleading sentences in providers documentation.
0a5f9889b758450394535568786f4f74dba02c5b Merge pull request #3336 from Nordix/kcp-log-etcd-errors
6ee07b3ff2c4162a3959969a6e9c20d813ebc4d2 Merge pull request #3541 from spectrocloud/fix-endpoint-zero-check
b20f7efd5398c4f86e780774deebc4ee48c9b4bd :seedling: Update to Controller Runtime v0.5.10
2355edfad97f3a4c9ad93c550250a1c448b1c75f Merge pull request #3544 from vincepri/expose-error
bafc9f356aac5072519a57f0a48706d7e6a50da7 Update e2e Kubernetes versions
491b34ffb1ea4a5ab2ec6afdaf364a058f5833e7 Merge pull request #3543 from vincepri/update-corefile1010
3ad74fbcd9e7ed5129437a0d8ad1216588351302 Ensure that etcd health check errors are logged.
5d7576529a34fffa6979aaade4458e47a48db0c4 :seedling: Expose CoreDNS errors to users when validation fails
c974e7a8179777ea51120fed96d3286f728c0cda :seedling: Update coredns-migration library to v1.0.10
506f16be8618f0dc9958ebcf977367b075d15851 Merge pull request #3527 from fabriziopandini/reconcile-delete-conditions
061583b680d1293caf25aa0578abf5ebc68c377f conditions for reconcile delete
3444475883138448383fb1279013e5a04683a4d1 Merge pull request #3408 from wfernandes/add-test-reconcile-etcd-members
fffcfedb09dab668b45b71c748f6609a53baa518 add APIEndpoint IsValid check when both host and port are non-zero, change controllers to use IsValid
b7546f7dd05b3860e4b1430f68570d444f09ed53 Merge pull request #3484 from wfernandes/clusterctl-version-check
ef3d1573714dfce2820b8d7ca184dfee01d3099c Add clusterctl version check
42fd8c21149f233460ed235e2c2c902a70206a2a Simplify CAPD quick start
7e445a129abb28b20ede1040cc64f8766059eab2 Merge pull request #3273 from mgugino-upstream-stage/machine-deletion-hooks-impl
fddb669ec40153aed3daf3f1c184730b5b958878 Add test to ReconcileEtcdMembers
6fd476aff997b0c40cedbfad58101bdafb5b562d Merge pull request #3532 from benmoss/fix-links
9b29fa5646940e252968dd8eae685788b0d771eb Merge pull request #3209 from Boutheina-Dab/capi-webhooks-envtest
00359e329f3dbbc4b9970d29ec0deabdf84fa366 Fix link to docker-provider
9637747a9b42bf78834ab070e0d36ef8b4f11ec5 enable webhooks in envtest
dfdca6335fbae089c4fa103c0697887cb7b3d6cb Add selector to CRS test
f8a924a1fef76b50605f810eb17466492e3fc8bb Merge pull request #3531 from Boutheina-Dab/mhc-test
1d7b639ddea89c838ff55b1549fdfd664b1395a3 Ensure correct log output to MHC
d4101d79f33001db88e2ca48dc485ed6ccaa8727 Merge pull request #3350 from wfernandes/add-get-workload-cluster-test
c946b8a0162476ee05d6a21febdf610d591e6d86 Merge pull request #3508 from srm09/bug/control-plane-version-check
0e52218b62e34349835b7b2cd3db5a914d3f519b Merge pull request #3298 from fabriziopandini/kcp-external-etcd
bf3f5710963f6d20a606a1fa1e81e95ad06780d4 Merge pull request #3522 from joshrosso/docs-concepts-v1alpha3
3da81fa4261847394ad6619e1a3cb27d3f0b4811 Merge pull request #3521 from joshrosso/align-print-columns
494b8b146055390d0fa49910f5ebdf02e83199d5 make kcp work with external etcd
53cbd917db13c795f5c8ac76163f9e98be125030 Performs KCP version check on update
2b71eebdec7e361e9baeb8f1454f8a6e0268c169 Align print columns between machinedeployment and kubeadmcontrolplanes.
62cf509da2696049c98e60d33cb8f641ffdb1bad Merge pull request #3190 from n1r1/ext-remediation-proposal
918d58ac8e0ff7f34598558c04fb92de67a0da9f docs: update concepts doc to inlcude v1alpha 3 schema
3db2d63b567d69af01c4f6b4a3212adf0a8c6dfc Merge pull request #3467 from sedefsavas/CRSCAEP
332946c44c8a3cbb7527d0251757355992063c12 Add GetWorkloadCluster test
b36e3bf09e24e0bc8444e1770706ac1b3ddd1089 Merge pull request #3455 from sedefsavas/binding_cleanup_crs_deletion
11485f4f817766c444840d8ea7e4e7d1a6b94cc9 Add external remediation proposal which enables opt in external remediation for unhealthy nodes backed by machines.
269a4823ac08ce566bc182e0b5206626204a9416 Merge pull request #3513 from vincepri/close-etcd-client-after-use
bb203e4b2e2dc031ec38c8d72e3402608a273dd3 Merge pull request #3480 from fabriziopandini/allow-single-image-override
469e7e6123f16f525003bf4105caa36cd446aa0c allow single image override
e38df08235e2fadea502df775232424033b4ca43 :bug: Close etcd clients after use
eb07294ddebe8099c359c35a1e42f79244e7d33f Merge pull request #3502 from rsmitty/allow-all-versions
becf876764277382539fa5c9c95483cf2ac4d565 Merge pull request #3507 from wfernandes/retry-list-resources
df05f530db81d44ec1d331e584a685aeaff03792 Merge pull request #3511 from fabriziopandini/use-cert-manager-v0.16.1
3dc410f8ced609187f8d32ddb9680ff7cb4e2461 Merge pull request #3510 from fabriziopandini/document-get-kubeconfig
4037cd7a73969a6fbd345cc467ebdd572291b0af :bug: accept prereleases when no releases published
b4217be15dc292cdc447a37082cc2d02a5db0e4e Merge pull request #3500 from danniel1205/update-capd-examples
3d3bcaa1a70aa63b79cb56f27f7324fbcef528a4 use-cert-manager-v0.16.1
c10e4a730d0a263c65637e24aaee7a51ab48b857  document get kubeconfig
1927d3dec81a83e930ad5ff297849dde4fc500e8 Retry getting list resources via discovery API
f8ef3fea9c46b4fa55e9735860b5c7bb67cb9a76 Merge pull request #3364 from fabriziopandini/clusterctl-upgrade-cert-manager
7c44e1eacf72f5e9f4042cc06c1e3832bfd720d7 Merge pull request #3332 from sedefsavas/e2eCNICRS
101d2bf006d4a5ab06212cbe06a35e48fd6f73e3 Merge pull request #3501 from genehynson/fork/fix-windows-path-encoding
f52763ad7c7ef70221d6866e69a1ae3372ec07ab remove redundant label of cluster.x-k8s.io/cluster-name from MachineDeployment spec in capd examples
481ad57f33091f8a1c89850c9a1a5705abbf18a0 Remove ClusterResourceSet from bindings on deletion.
ca50ea9fc7a4265be07c908a09dd11ccc212b82f fixes issue with Windows, paths can't be escaped
ab4dfc991676dd1cc206bd4a57c792c546b1c77c Merge pull request #3503 from rsmitty/master
6e0e62dd2f7771fb851a5c2d333d4e738b9e8015 clusterctl upgrade cert-manager before providers
3af94bb0b08f5cd06758edd1ec866e3dec6e4715 Merge pull request #3477 from CecileRobertMichon/mp-requeueafter
55db459546c74ecf24f3ed107f8e9a8668486ddd 🌱 add sidero to infrastructure providers
a7b468352b36951815a651c727a2ab686f9c9cfe Merge pull request #3499 from rsmitty/test-fixes
e9da75a3758d6492ac2f0ae2fd1671e602280c55 :seedling: Remove RequeueAfterError from machine pool controller
c562528154bad3e75ed7b2a940fc511a995c374a 🐛 fix github repository testing
57a1c7e4e6a2b8093da02454d8a244c0cf667751 Merge pull request #3473 from alexeldeib/ace/capbk
f39fe63f594cbf468be256472c929ef88e151042 bump the k8s version from v1.14.2 to v1.18.6 in capd examples
c229c88ea70962dc3732b9fcdaaef492cfb8022f update current capd examples to use MachineDeployment
44f3aeae8690864b9205b9e592698a31c64b30bb :bug: avoid in-place mutation, duplicate files
e0324d62e39701625dafeba2d465611d86a9b78e Merge pull request #3445 from vincepri/requeue-after-remove-cluster-controller
e30eb1429c96f8873c1d5edfebfc38463b83dd7b Merge pull request #3489 from detiber/capiIcons
5c3e993a82bd570495cf5de3e14ba9fa86673af8 Merge pull request #3449 from fabriziopandini/improve-version-support-doc
df4712475a06bd5e6fd124f5f405fedab0960ce8 Merge pull request #3476 from CecileRobertMichon/mp-scale-phase
70234b542adc48b6d02e2c12c20d274ab8d555e8 Add Cluster API icons to repo
f55cb6a07003100b0cfcbe725f1fbf921175b2d2 Merge pull request #3481 from fabriziopandini/small-improvement-controlplane-provider-doc
9d0d1ccf6010dcc47d723df91e410f1973ed43af :seedling: Remove RequeueAfterError from cluster controller
7eb6c4ef4adf331029c18d8dbdfd644496524028 Merge pull request #3462 from fabriziopandini/upgrade-cert-manager-in-tiltfile
3ae0afb766ca74dd3c4d057c349416db2569f328 Merge pull request #3495 from fabriziopandini/fix-mhc-condition-const
70eafa2e89e6162944a29b4ab34e5cb2dfaed701 fix MHC conditions const
38810211da3f71dd3ce61d9f1fa85a690dd98790 Merge pull request #3490 from detiber/FixPacketPodCIDR
4579de87755544c0f062d1a0bd81e38ad8f8fc48 Update Packet quickstart to better work with Calico CNI
43dd623ce667a1ff33e0d2d649b9a3dea2977f02 Merge pull request #3464 from wfernandes/remove-metrics
70a499ff02857f179ed0f8f695e6ef46093400a9 small improvement to control-plane provider doc
b49b6a32d889142b7b037b3e072c42e626efbc50 Merge pull request #3475 from CecileRobertMichon/defaults-mp
c1aeccb679cd562c2cb1742e20ef319cc4805f28 Merge pull request #3472 from CecileRobertMichon/fix-mp-kubeadmconfig
06b8868f04640b2ac9fde32228f14034edbd39b1 Merge pull request #3478 from devigned/typo
2e150d32b8ca9f309fb590b3bba9a2ac2b4fd7a6 🐛 fix cluster create not paused when paused log entry
a53412e20cbaffe79f3f7f34c5c775c6576f3b68 Implement deletion lifecycle hooks
515be2a282cd589f177a9238c19cf6133f33babc :sparkles: Set MachinePool phase to scaling when infra is scaling
0088326add8157d738ced644ee1bca1bb1e39340 :bug: Default MachinePool replicas and MinReadySeconds
8017330ec9a80cb7446d61757e29e5285ea7bc30 :bug: Fix ClusterToKubeadmConfigs to include MachinePools
32899ad267dbb89208aec074c412d8f2055bd159 Merge pull request #3454 from wfernandes/clusterctl-init-ignore-pre-releases
f8dd8a3bdba86bae3e72abdf2c8d7cbac9573cf7 Merge pull request #3470 from ykakarap/kubectl_column_mismatch
4e90523fa94618a4cbddbd9fec98ab052873bc89 Exclude pre-releases when getting latest releases
c3839506634fa1e651382d58d5f0289c7ccf5561 Correct Type and Provider column information
ef5a9e7bd4aa232bcc2f2fa87caf2c7354430c91 Merge pull request #3337 from rsmitty/move
55fe8908b794a64bd072269bd3de74e8f3a37e9f Address comments
cad5ffe3f6835bc06337e38259166b4d4b5b2c20 Merge pull request #3468 from mboersma/e2e-failure-help
840fbb3e3963432d1800a6fa9180c04564140b27 Merge pull request #3460 from wfernandes/wff-add-kubeconfig-command
9455243709fb9af85ba3b7ce120c80aca5a473de 🌱 [e2e] add debug output for deployment failures
6b6c8e06a35cdeb4ef709569dbb4754c5d694370 Merge pull request #3448 from fabriziopandini/improve-clusterctl-upgrade-docs
21e49a05f1f700475d0e63eca80eeb70da954c66 Merge pull request #3446 from wfernandes/upgrade-watching-namespace
4df8035be0348cb1e1ccdd3bb802bdf70d015974 Merge pull request #3349 from fabriziopandini/standardize-test
c5e33019c5467ad26ceaa11c75a263e2d061d8c1 Install CNI with ClusterResourceSet
a43be552880482dc5e7dce043a901d420b435229 Updated ClusterResourceSet CAEP.
97bb13c7bded352faa99be36d0a4a179e181f340 Add command `clusterctl get kubeconfig`
4ecd3ebec6e5a49f9e5ce540e92b9352291cb075 Remove old metrics from v1a3
a9b98a8d912fdd669b371bca766f2abc87208b55 :sparkles: support ability to move custom objects in clusterctl
76a9f1a2ce37cda2db6f1d137552d2b4c33a10dd Merge pull request #3463 from fabriziopandini/fix-move-clusterresourceset-flakes
ea18a053e1224922ff5077b6b7809ecea317e8a4 fix CRS move test flakes
3c347aeea97f690dbe22ec30f49f047379be808c upgrade cert-manager in Tiltfile
ad631d74502a91995b3e65b421f71991ff799e4c Merge pull request #3313 from munnerz/upgrade-cert-manager
19a37e676cb714d212fe8222ce5f65d5a6c410a3 Upgrade cert-manager to v0.16.0
789abac0171ec701c35fcfdab5654cab6049e9aa Standardize tests
60ce90a7bf173d008b39492be45e1a1fef02bcdd Merge pull request #3132 from mgugino-upstream-stage/machine-deletion-hooks
b8fdef664b7648df7fdb4ebb23c7efa7aae0a8a6 Merge pull request #3456 from sedefsavas/remove-rbac
7c8bb5e75f65d1f2376e20df8a965a166183bff7 Merge pull request #3444 from benmoss/mhc-paused-machines
9ca08a793f85ad7a2af4e3b514e8348850ed5ad3 add tip on using multiple config files
5b453c09476a5f859290e1e034d0bde1295f08f8 Remove unnecessarry rbac rules.
8da4c8b6a1564dc83535c21aeeb51a9822457238 Include watching ns for custom provider upgrades
7896219e75ed0ba928bad494f3c736f5d947b930 Merge pull request #3433 from CecileRobertMichon/azure-json-rm
9e0806f8082773a78e004cfaef1af28781b89004 Merge pull request #3452 from benmoss/envsubsbtbsts
cec436cccfbce958190a691ef8a983a1fa2f1220 Fix broken link
69347982dc6983615cd439e975cccb397083859e Merge pull request #3443 from vincepri/remove-requeueafter-reconcilediscovery
3faed2ba35d80505dcc53d7e88e952b6bd3415e1 improve version support doc
d9f12116675f8f974ed74a9ae4cfb638fd20f1c4 improve clusterctl upgrade docs
3900bb1cb2cb77c6ceebeb747647b22db2817dba Merge pull request #3442 from vincepri/remove-jsonpatch-replace
568105aee32092ac86682ae56ac315dc95b56662 :book: Remove azure.json variable from quick start
ec880946d41879dbf21c4bdee08dbc698c8fb7bd MHC should not remediate paused machines
231f6ce2b40bc24e28a72c9cb4aebac8d3cd0cdf Remove RequeueAfterError from CABPK reconcile discovery
e4d7f80c6d6a72ba432fb1ee37a98e404d364d38 :seedling: Remove json-patch library replace
459a61cd8789d28e7dcba55988d7b07db327bdd0 Merge pull request #3389 from a-mccarthy/update-readme
3ae90857a5ab1b21bf35bcdab2daf3e259454b96 Merge pull request #3436 from wfernandes/metadata-docs
9e4e82aabd2dfe7a52ebd0b7d6b802a9be4ff93d Merge pull request #3410 from sedefsavas/resource_watch
6311dc2c1f966edde41c842fb812596fc3ca0b25 Merge pull request #3405 from benmoss/kcp-rollout-bug
4de2d9bea11acc364a88158e03fc8ec6c00ca74c Merge pull request #3406 from wfernandes/clusterctl-generate-yaml
b23099f44725aaf8c9415321595f009351825211 KCP rollout maintains even distribution of failure domains
8ca7578a17efcf0355d1ddf1ff6705a28d2ed76a include providers info
8d3fb61bfc93b018b8723f0918f87975117a10c4 Add watch for ClusterResourceSet resources
d635164121a5ab75bd0f7b6d2423ce802c80dada Add ux note for using embedded metadata in cluserctl
78c886c844db142aefc2e5768f6cb67abd8bd68d Add generate yaml subcommand to clusterctl
e955160f6f30f61eabce65231899a1fe9d513046 Merge pull request #3310 from fabriziopandini/generate-coverage-report
b2f800271287333cd763470f7bfd3476bf23573f Merge pull request #3423 from nader-ziada/azure-cluster-name
a2a78ce4dff4d8672186d5fcfd791f6d54ef3258 Merge pull request #3431 from vincepri/go11314
fae9f8b5646fa346dbcb7470378967cb0c91f89e :seedling: Update to Go 1.13.14
147a874cd20e514c18f429d47659b2450609717b include not about appropriate way to ask questions and consume project news
41f522424a8cfca8347222ba6f91a7cbc84ee88b add note about clustername validation for azure
5cacc9f47d4f94671a56bfd014a74f23725d8505 CAEP: machine deletion phase hooks
95fe9e2c2c48cb7c765e40fe97861f22765441ff Merge pull request #3414 from CecileRobertMichon/escape-quotes
d14ec63c3b2938c4a101058e72483bc4438026a5 :book: Escape quotes in AZURE_JSON_B64
c1165cc7889c7e188e5cd4fc2db1b6477004d90a Merge pull request #3412 from yastij/bump-vsphee-provider
13dd1ef5987382d4eeae5e41a2bb9a51900a1a80 add v0.7 to the embedded metadata
abb1468ed54acd5097da39f0658ce028239bff49 Merge pull request #3411 from wfernandes/wrap-repo-local-error
b94ab42377557d391476ee35003916f6e7f24572 Wrap error so as to not lose context
bed3fb7ee4eb3b9e2ed567f85d95f5b88faa3dcd Merge pull request #3402 from vincepri/requeue-on-errors
ca6439ed742050f9229d0ae34efcf4e27a177ff2 Merge pull request #3409 from benmoss/update-shellcheck-url
63e0e4ad1ef8fed225e032de05dc90a62f7c297f Fix shellcheck install script
a43a8fd55ce0d93366fd2d7016c25cd4fbd947bb Merge pull request #3394 from detiber/testFix
ec92edab33be88da06137335f929cc0bdbcdf274 [e2e framework] Fix race condition when testing ClusterResourceSetBinding
803458af87913be102942b0a5b511ee2233be4a7 :seedling: Requeue CRS on errors
38d49ae7e8c328790ad74e935b5af207d75b7064 Merge pull request #3387 from vincepri/deprecation-notice-requeueafter
21bead8f535fe6567b6fbd3bf80592a669428a57 :seedling: Add deprecation notice for RequeueAfterError
60147823dc2131b822125598a73b2ad34e55b050 Merge pull request #3366 from sedefsavas/binding_cleanup
352c21ba2271641aa03842a386ef8fc7355db278 Add ClusterResourceSetBinding controller for deletion
e332eb5f77d43b57e25c1aa3dbd8e94fb76b8e66 Merge pull request #3392 from newrelic-forks/rudoi/capz-machinepool-helpers
b39196ce2a9f2c4fd25bad886701920b55a45aa5 chore: add MachinePool helpers to util pkg
2d74380cd641a85e04b7450c6bd166c340933de3 Merge pull request #3388 from vincepri/reconcile-health-no-requeueafter
b3300c701e63a790a899c1bad19dd37be0307f6c Update community section of readme
c9e496b4e2c8edca521471955e69de1d0304160d :seedling: Remove RequeueAfterError usage from reconcileHealth
60a6daf4b9ecb74a9111b3269e7016988a8afc00 Merge pull request #3386 from vincepri/kcp-delete-bug-requeue-after
7e81980715deaba5f41fa82b7b21976da0c68d64 :bug: KCP reconcileDelete should not use RequeueAfterError
23aad1f1e498f564d7b745def25930ecd62c615f Merge pull request #3385 from benmoss/mhc-logging
c510161e2c2639a4c5e8a1683c34a016a1d236ac Log when and why a machine is marked for remediation
823941bbd7ada775cd25bf16645d7120f81e88ef Merge pull request #3382 from vincepri/fix-cmp-log
c4a7420ba643e141e57694181816b4aa01e4681a 📖  Update site home page (#3376)
7d92339fffd475d39a3ffc168b00f90ad7ad1aba Merge pull request #3381 from vincepri/cr059
f8cac939e45dfe9f41458d3a74b4dd6dba75b31f Merge pull request #3378 from ncdc/fix-tilt-kustomize-substitutions
d0401038567b6ca4bd29f7c4dd5a3182c1c86b16 Fix kustomize_substitutions
e458d627c4b56e978ac6c460bb862166cec341c8 :seedling: Fix logging comparison between conditions patch
36131f9a1898834a7b6604e9e2b482fc4059ea47 :seedling: Update controller-runtime to v0.5.9
24b7f4219c77590b64bfdbae566a3cdc782ab894 Merge pull request #3377 from vincepri/add-diff-patch-condition
c5b31fefe2b21a16ec2f1dff6053876d41c02037 :seedling: Add cmp.Diff to condition patch conflicts
682ecea739ef4843c1190432c7deb46da9afdb32 Merge pull request #3374 from ncdc/no-gvk
4f09531d68fc5bcc9441d18ae973d80caac4656d Only look at Group and Kind for GetOwnerCluster
337b406652a2bc7e4c042f5e986b416077eca30c Merge pull request #3369 from benmoss/docker-version-flags
17e686ca6b3e741f9a34b32ea101fcd3da55c087 Add version ldflags to docker-build make targets
b9bcc8c55bea0cad1b22cd872162d06c8687befe Merge pull request #3267 from superbrothers/crd-relationship-diagrams
2408cb0c21de302ede880a8e6b9a1cd025ac9f60 Merge pull request #3295 from randomvariable/caep-security
545f589547611f9e2ae94d02748263c9c86dccc5 Merge pull request #3356 from fabriziopandini/fix-matchClusterConfiguration
9a5ef88844649bc7f4e8fefb118cdceb7ee1f133 Merge pull request #3355 from fabriziopandini/improve-clusterctl-doc
bb05bd2e3d5c2a6bc9431e3e163e46a8c44b37eb KCP: fix problem in rollout detection logic when ClusterConfiguration is nil
5a9c62e1fc6b2ff1680a54a39cca47238e3e9320 Add CRD relationships diagrams
9aaae9f9b5152ed4dc8ce8f2fe6e51f8c6395a37 Merge pull request #3361 from alexeldeib/ace/tiltenv
73b18d51186bca59321de558b5c7fbb8d486aec4 :seedling: fix tilt with envsubst
17c315835bbdbbaec917c615f2846100ab085a55 Merge pull request #3362 from CecileRobertMichon/cabpk-feature-gates
3e93eca244dbd140a0d15f23842de35ec97e9dfe :seedling: Add MachinePool feature gate defaults to CABPK
30062aa9aa9d30e9ff3b7f7f61cfac9a25c1c9a5 Merge pull request #3303 from CecileRobertMichon/azure-json-secret
31d55003ceaa5af7adefae8d0fc074683284c512 Update CAEP template with requirements and security model
19afe6cc4abec48f16211617d7f8a6571f6a2997 Merge pull request #3346 from newrelic-forks/tilt-settings-list-of-dics
6fc829a56c2e98d1d4de3d21c64d7d3730fd3d2b improve clusterctl move doc
58ae30d062de5fe95a91fc1fa2a7c4cc30e6c23b Support a list of dics in tilt-settings
49f88d511f9584cb37bd38522a869ceaea9f2242 Merge pull request #3347 from shreyasbapat/doc-fix
34ac896995b49a11e3302ff242b27d8cfdced3e1 Merge pull request #3320 from benmoss/capd-tolerations
0f7ade43f5d34667c031917812d6be1d5f9f5159 Merge pull request #3305 from fabriziopandini/improve-healthcheck-docs
bb3a4e5d1f9a845b57ebcc3e25d459d7318d388b Merge pull request #3334 from wfernandes/add-machinefilters-tests
98773836297726db9112bfc6253e0b83a5632a9e Merge pull request #3333 from wfernandes/add-update-coredns-test
20207d1a4603d53f70f1332bd195cd78c04890c2 Add details about lifecycle/active in the documentation
0c5dc63dc32643ae36a53fded34d1a1a3d7522ae Merge pull request #3314 from vincepri/add-cecile-maintainer
dfe7022e94b8f61eb27a9606e270e09c84d29767 Merge pull request #3341 from benmoss/resource-typo
12fae10aaead3b117018fface848dbeb95bd9be7 Fix typo in ClusterResourceSet flag
7312ffd4b3ac34a5c3b86b8ae33a85891bb2077a Add tests for MatchesTemplateClonedFrom filter
ba6e3d7fa4f17e14589b128ef02e50242969562a Add test for UpdateCoreDNS
846ca08db5939e5bf88104b2f34427e7316ee7b9 Merge pull request #3324 from tvs/allow-config-changes
d6733bda6dbc2b2e4d873ed27421e6cbe5a9e165 Add tests for MatchesKubernetesVersion filter
434a076e8b52d9fae208d29c2b3213ee9b7a8a92 Allow KCP users to mutate node registration options
4e07b0c23f6782fa5ca3729c3f9ed005a6f9a203 Merge pull request #3328 from vincepri/update-cr-058
7fa6c2b53189d226d62ccf0e4ecf940512dd1763 Merge pull request #3325 from fabriziopandini/add-featuregates-variables
4caba1e62d74c6ed01a6587cff1c14eae4336670 Update controller runtime to v0.5.8
3edb8d5e42c63f985591662219c1a6ae06e4db37 fix e2e
50318492b886bbd7f6c28b51a29d7dc7dc2e2949 add variables for featuregates
e020060957ca4cd1e0b8bf2ae02b1c26ed85ffa1 Merge pull request #3270 from wfernandes/template-defaults-with-envsubst
d4907ef7aeed6711cff4fb41ba7f0da7a0b5542d Use drone/envsubst to provide defaults
8281181573cb54c33d35b17939c00f0fb39692b3 Merge pull request #3319 from tvs/opt-out-kubeproxy
2b4020d91dffde0bb1b37104b119bf372f3b72d3 Merge pull request #3317 from sedefsavas/CRSmaptolist
10e85e386f55dca0b229aa6ecaff44529ee9719d Change ClusterResourceSetBinding maps to lists
bed682cf9aafe86752ebbc9272fc890405274167 Add node-role: control-plane toleration to capd
4c5249c55b2b65b8d7d7c510e0133805983d1113 Merge pull request #3196 from prankul88/listDescendents-update
23430a3c05401dbf2ac281ef9a927227aa71ae4b Fix typo in listDescendents MachinePool
b828d4c9c685a47c9a60482eb48b97dcfab94c90 Merge pull request #3307 from fabriziopandini/improve-implementers-guide
5c826db271422d72722859b74c7615714a44071f Provide a way to disable kube-proxy management in KCP via annotations
5e5bcf06b056250f5570294bcd69bc2abe03eca7 listDescendents fetch MachinePools
af94a13fccd5410b359cb301414d4c72e9a78284 Merge pull request #3243 from fabriziopandini/move-ClusterResourceSet
8db40f286d0b63c896ec988ba1c5566e81934baa Merge pull request #3312 from sedefsavas/removesemantic
fcb38887d008d0a89040a8de9a02380b7ee39ab0 Promote CecileRobertMichon as maintainer
652bc7ae651b3359f589202d8a280edb765ca374 Remove semantic merge from bootstrap controller
baf4a03d8df2d668e05f3776c1843d0a9bd8e12d add a make target to generate test coverage report
35efd43ee54b11df5d16b803002f88cc12cb9a97 improve healthcheck docs
1de9e41f276c1ae243f5f21fe97b84667180f908  improve implementers guide
fbd8d9af61a1c6ab2af9ddc7c0ae93b0056b4483 move ClusterResourceSets
20385958a82f05c57866e5db775f4c9656b80f87 :book: Update CAPZ quickstart variables to include new AZURE_JSON_B64 secret
e68354f948db4855dade9ce7ec450328f20a3504 Merge pull request #3302 from vincepri/remove-hash-cp
c6e771175d68ab4080fbc23d5aaee56b59d7188e Merge pull request #3107 from sedefsavas/clusterresourceset_
add44ad0c422351a54b0b38138cd210bc8a2955a ClusterResourceSet feature
9a2aa086280f145b97afcebc13d0221b87cbaf9d Merge pull request #3290 from fabriziopandini/fix-clusterctl-logswitch
3c73ab1b8f793e9ca17d84283ed8adc6a502ad26 :seedling: Remove hash label from KCP machines
0b1bc5103cd6535a51e5412fa8396df845f53ede Merge pull request #3286 from fabriziopandini/cleanup-MatchesKubeadmBootstrapConfig
32002624de8de8c7beacee8190010f50e0b3e31d cleanup MatchesKubeadmBootstrapConfig and add unit tests
67d8712b893da09fa21fd87b4245b33531959f0a fix clusterctl log switch
5f0a49e0fcf2a1cb90b54553e7836600e571aae6 Merge pull request #3288 from fabriziopandini/remove-offensive-word
efc818f04b5e7b342a9e8f87235c167a390ca8b0 Merge pull request #3277 from fabriziopandini/cleanup-machinesNeedingRollout
e81b7d4285ba846f9a194733dcbfb906cd0af031 Merge pull request #3285 from SataQiu/clean-master-20200703
ac0f3d82dd008f78f1f564e46c2f592fd288afaa remove offensive words from the codebase
bafbf6e275ba2ed1e1fb6b47c8c74ed6f45e129e remove use of master word from our codebase
4cc7ebf9bea4212812965b51db5898499df77961 Merge pull request #3284 from superbrothers/fix-cluster-infra-provider-diagram
56aa90ab24ea6a32f3f35e8020dde87e0f9943df Fix the field name in cluster-infra-provider diagram
40e8a9abe7616468193025fcc7a32bfc1bd43bee cleanup machinesNeedingRollout
2ac3728d26593f7c54520999477aad45934e1c59 Merge pull request #3275 from kubealex/patch-1
fdbeab87fc8c24e2fcc3d7601d4c52dc620ab964 Bumped calico version to 3.15
cc45432cd30ddc33d19c6467f485715fae72ed68 Merge pull request #3234 from sedefsavas/3170
38d8699bb7c42f10b20a36a553161ba85f739fc7 Modify MachineNeedsRollout logic
34f04431a63311e90e46e908b13d11d2a4fcf773 Merge pull request #3265 from saimanoj01/saib/fix_spec
faa6e091f5d549a3757785e392b1e2942f2f1e23 Merge pull request #3271 from rsmitty/master
1daed584544a33939ebe0942179e1fc9823c866d Merge pull request #3268 from fabriziopandini/cluster-supports-webhooks-rolebindings
3ac7114ad538718cc28c02b2d9b6dcd7081486ee Merge pull request #3266 from spagno/add-observedgeneration-to-machinepool
2ec862a7ebc018dd87580e5a9e2dd681ca7ad8f7 Fix references to spec.kubernetesVersion for the Machine object to spec.Version
d20d38c629fd3676f9e19fe0021ec19abff9566e Merge pull request #3226 from spagno/issue-3078
f4d15f66edcd8067d4066f97c8f5a02fc93d3c99 :seedling: add talos providers to defaults in clusterctl
f08a696b60392e08782792f0edc2435de25ae375 Add ObservedGeneration to MachinePool Controller
4c84bb47a560321983cfd1e80183838e482b473d Added observedGeneration object in the status
ef2b61f7d4914352c1782436015ae94ef1b7e683 Merge pull request #3164 from srm09/bug/remove-machine-set-owner-ref
e57b36654aa10991753b55af68f7dac143833721 Merge pull request #3261 from fabriziopandini/allow-incremental-condition-patch
645b2c74f0137bfa01f394e2df1dd17898e02b12 Cluster supports webhooks ClusterRole/RoleBindings
2fb80bf9a0ba0f1477661b2ca3e33d480c82d8e3 Allow incremental condition patch
3804d97cc952771ba321837f97fa2149196bae01 Removes MachineSet Controller owner for existing Machines
76f2b16d872a291548cdcc3fc0b41865d98ec492 update to spec.version reference for the Machine object
e7f10ea4654bcda41cc6f029c1b8009497ff0bf3 Fix references to spec.kubernetesVersion for the Machine object to spec.Version
94de3608da2aad973e2d19b82b20c79bf02f51e1 Merge pull request #3249 from jayunit100/tiltfile-kustomizations
8f0d03b0ca625933745845633f3e91d74803e08d Merge pull request #3233 from joaopapereira/issue/2871
8e3598b5f13c1dd70d2a14d5fe3f7f7afa011db0 Merge pull request #3262 from randomvariable/capture-metrics
42c3212c032cba0f5713d8c2c0da6760aaa986de Adds tests for InitImages
492970b1c9d14551f04e819a49e4216c9927fddd Add an error message if missing substitutions for kustomization w
f429fb51c6a583a05bb5d465bd5fc753e484b279 test framework: Enable metrics collection
cc327c8dcb389d288c72a07aed85f3a4581bbae4 Merge pull request #3263 from gianarb/chore/packethost-migration
fc9ddbd4f750008889a0a66c04c2b11df7dbf851 chore: provider packet is now part of kubernetes-sigs
bf704ba57cc86874b4f4e39202baae0b68788e4e Merge pull request #3258 from vincepri/add-opts-patch
75b02ce3d75606133d8f778a907cbda1b215f6d9 :seedling: Allow Patch to specify options as well
fd73b181efeb3f2027c26841e1c08f5cab0322e9 Merge pull request #3250 from andrewsykim/capd-machine-address
2fc37ea047ef5adf302b06322bc8e7046d5ce921 Merge pull request #3246 from wfernandes/doc-namespace-prefix-bug
91bbf41564963a2fce87394621f4fe734b4540b5 Merge pull request #3214 from SataQiu/fix-finalizer-20200619
e874a89c47d4cdf9e14fda545a5765db77cf24f2 Merge pull request #3115 from wfernandes/clusterctl-templating-default-yaml-processor
7d0a5601fed3993a4007cf500603f03f80684ed9 Merge pull request #3253 from gab-satchi/test-fix
ff769704b83541916ffe912a3a988bdb0b0fc5a8 Adds custom matcher for MHC status
bebff1b83d6f9e10e55415c3624865339dc1e878 capd: set machine addresses
a9b58bfe2470e375c3d96ee95160f29ea6c04d43 Merge pull request #3186 from gab-satchi/2863-mhc-targets
5264b3623d06b8ac6338639f136c275bcb63fee6 Adds targets to MHC
c8527be29adb86b18daaf0ecdbcb259aacc60cc9 Merge pull request #3240 from vincepri/improve-mhc-tests
e87da61eaec4eeb5d0cd702099e2b8380b2ba719 Add YamlProcessor interface for cluster templating
d39c6ebd2c19aab7472136ca568de16082ece0b1 Add known bug warning for clusterctl delete
1b92bfe57fc597badd497f70bc7eadfa1dfa4a4e Merge pull request #3245 from bboreham/kuberentes
c6f62666e6fe17e21eda5cc8f0d0aced0f11733b Fix typo: kuberentes->kubernetes
a42d5075ee96bce0afcabec5870454da7329f63a 🐛 MHC tests should create proper machines
303f4923517c42a0fad9d40935eafcc151e0f288 Merge pull request #3241 from vincepri/capd-image-fix
e7eb0a6fd85eabb6859bec420d8ddcd0ca790324 :seedling: Pull images when building capd as well
49fdf548037df53f08d2af5893848b269e318941 Merge pull request #3239 from vincepri/remove-build-pull
2e3aed42dde543a392596390ef7415c84c3f6199 Merge pull request #3236 from sethp-nr/patch-3
c9a2bce54e48c42f7f921ea028f94a8d1b8df7fc :seedling: Remove build --pull argument
aad6ede8b5cd098e8a5f4f557a80441655bd8611 Merge pull request #3238 from vincepri/fix-path
f8928e3ec67322cdb49b8305d3ff4d1a4ab6f568 :seedling: Use full path for golang images
3be45e1570ebd6b861b4d79eaca9f079ab2cf0f5 Merge pull request #3237 from vincepri/prepull-images
2a9c5c32964b704bd9ba05711cbdf5197576a9d1 :seedling: Make release-staging should pre-pull required images
b197abb0a22ee55390559497d192e4c3881bedfb :bug: Properly adopt cluster secrets on upgrade
241d24738094c617f1c686cea121f17d01df3c48 Merge pull request #3235 from fabriziopandini/fix-image-build
52f7bc7346184a350788813c2a4498205f96c560 fix image build
d044be3ef0508a9852ba9854f8cd5ef7dd6fc272 Merge pull request #3116 from randomvariable/clusterawsadmv2-docs
f0193ae49c5aea9a0fd0dd3857e4fc2072052447 docs: Update quickstart for clusterawsadm v2
50b8c78b4e1754cc61ef2981b03180358a8db74d Merge pull request #3232 from benmoss/mhc-scoped-cluster
2c3e881ee509885b239b309d78804067be203944 Merge pull request #3181 from sedefsavas/kcp_annotation
024d170f3327af80613c52a116c31c22a718b57a Merge pull request #3231 from vincepri/use-patch
ca7807529d21838fd680f38d5a9c88401f907147 Add infraref annotation to KCP machines
5e17099e6269cc79727cfa06344d3102c7534cb6 change controllers to add finalizers at the first reconciliation
7cc45ccde8d0bcaa8fd375fa1de530467e59a01b Scope MHC machines to the cluster matching their clusterName
3c8814e056a112a0963dd72f928404df0660cba4 :seedling: Use patch in tests instead of update
4a5d66b71a3b97648ae5eef103cf7bec284f5c35 Merge pull request #3222 from wfernandes/delete-machine-no-node-ref
02c36a65c044d06acc81aad441f42d440c9cbe4d Prioritize deleting machines without NodeRef
c550760574c19419037df1edafe45e22ee46c0d5 Merge pull request #3212 from nader-ziada/azure-quick-start
8d137e60e14f04b0f83bb2ec024baefa5bbc3f87 Merge pull request #3175 from Nordix/pkcs8-mael
77c424e1815f2c5cff65fe9e219e5774884dc183 Add support for PKCS8 private keys in CA certs
e5a920ac1336e982830839769e42acd9429e12e5 Merge pull request #3229 from vincepri/test-timeout
b9579984fe898666983b8fce3e99678ec7a6dde6 Increase test timeout
05de560dc711baf2b58b209bc570207a3eea0d13 Merge pull request #3228 from vincepri/update-deps-jsonpatch
50dd4fe5eb11fc70478feaa3b94b193cecff4859 :seedling: Update dependencies: controller-runtime v0.5.7 and json-patch
0e9f5a8b1142443dc59d7c77db349068b00d287f Merge pull request #3224 from hazbo/test-ensureNamespaces-works
132537e610babade8d5a13cc2a66020f334b1edd Adds a test for ensureNamespaces
3a4b104ab952ec546ac3746592b04bcdb2af87ca Merge pull request #3223 from vincepri/update-cloudbuild
40ec227223fd3c14fb034ef376f9d184527b44a0 :seedling: Update gcloud image for cloudbuild
70b8b69323d0ac1dd5ac4273be68a8d1f3c40d35 Merge pull request #3221 from fabriziopandini/fix-docker-experimental-annotation
e9a98a4e0ef6bfd28b380063e6c4ce412322f83f fix-docker-experimental-annotation
c6dedc546f226ad47fce62a75d22af166aa01d6a Merge pull request #3220 from fabriziopandini/update-gcloud-buildimage
d96d3e36edc973df21ceaa9521746abdf4376c61 update gcloud build image
11714ac3e1dafd5ff2a0285faf4d2980fd566ad2 Merge pull request #3219 from vincepri/refactor-mhc-tests
f245e8ac13677b8ad2e7079924d0552cc944b5a7 Merge pull request #3207 from fabriziopandini/add-conditions-to-cluster
e0a0fd8bdf5fce98df764934fabc0636af247b81 Merge pull request #3192 from vincepri/update-roadmap
31d84b1243edaa3e852d4f3a113c7704367288c2 Merge pull request #3194 from fabriziopandini/reviewing-tips
1fbeabf021f22d40ba167508fde001592c36f3c2 add conditions to cluster
e6161ff64ec3e9bdf67b133272879f61a8079ac4 :seedling: Rewrite MHC tests to be consistent with rest of codebase
2dd6943f2b792fcc1ec724223a7f7dddd5b7b748 Merge pull request #3217 from hazbo/add-test-for-ensureNamespace
f2d71a3b27a9c8d95e90f17ae9d723237bae0e57 Merge pull request #3201 from JoelSpeed/fix-watchinfo-equality
15f0ae5933b7f23f1a4182e5d8ce00f7c152ebe7 add reviewing tips
fd43486ef3198040ec575fd14c1bf6519c95df45 This PR was initially to write a test for the `ensureNamespaces` function, not to be confused with the `ensureNamespace` test I have in this commit.
257525f7e7675a2429883ac85f64fc6580765658 Merge pull request #3191 from vincepri/update-contributing-review
b1c525c7dfcfa0b4cedd232c3dc9746bf3787de3 Merge pull request #3218 from fabriziopandini/document-docker-version-requirements
58f919c5e2de3f3b7a2026ab96a0e06c5b3526ff Fix for watch info matching in cluster cache tracker
23e36adb1770081f091fd7bd638c4828345bc34b document docker version requirements
3fe965cd63a32d18fcd71a2a4e4906025c3202e3 Merge pull request #3215 from lsytj0413/fix-object-cons-for
b42f2dbcdd178d3655742d024aa8236084a3da52 feat(bootstrap): initialize variable out of for range
3649e78c790aa453b9ebeb5462d7ef70a65d8ee6 Merge pull request #3213 from vincepri/envtest-klog
0225dbfdb3fd16538336a2cc6f6857119bf72aec Merge pull request #3139 from fabriziopandini/add-conditions-to-kcp
359108d0aa9fcaa5dca77733f59406d3546452e4 :bug: Envtest should initialize controller runtime logger
80653d174c6f5bb5ea76fbafbe2f0c50cc1185dd Merge pull request #3210 from fabriziopandini/use-docker-buildkit
46bf40c32f8b598018fb87fb6c9c0cf4a8a75b58 Merge pull request #3206 from wfernandes/cert-manager-sideEffects
9b6fc5aab860b712b585988d96e4b54386821eed Add AZURE_ENVIRONMENT env var to azure instructions
b74df8d2edcd45440726ff851b2097ea7f9e7912 Set sideEffects:None for cert-manager MutatingWebhookConfiguration
9e56210e602343e4438a8376bf3d464b8a872ce8 Merge pull request #3211 from kinvolk/dongsu/fix-typos-cabpk
04c2ec937aef93e40ac7dda9f1ffb9f8facebb81 Merge pull request #3208 from fabriziopandini/remove-errorAndWarningSummary-from-conditions
8b13136c1cb6da39c666f75a0a9cd58f6e2d77ee Fix typos for CABPK
20eb90a25c4d411846e829fff3a0d7fa16c97d0d use docker build kit
17d55348cfc43c4a6e18f2f7f2da269fdb65d944 remove error and warning summary from conditions
74f2b4fa491a2a3aedc6b113a16c5b51d895ef24 add conditions to kcp
53e98d22ccc1510a18b2caead34f4a8014a29983 Merge pull request #3157 from fiunchinho/machinepool-failuredomain
6e6ba84ca0a29367503bff69b4a5f36e7e1d2a3b Add MachinePool support for FailureDomains
3de5009b156e5cf42e2303de79e6bf2da83feffe Merge pull request #3199 from spectrocloud/add-kcp-finalizer-first
e84a8f60a856c620f83b4a711e1b422d83dcf218 add finalizer to kcp in first reconcile to avoid race condition with delete
247fcacd515c5c8c18bdd8a0ebf57ef0525aa96b Merge pull request #3180 from spagno/master
1b41ca4cca657f61f095bca34b939a6e64442a81 Added variable for kind 0.8.0+ due the issue https://github.com/kubernetes-sigs/cluster-api/issues/3013
03ce5fba0ffb91e6cc75455cce57f5a6ed0f3a38 :book: Add more structure and details to roadmap document
1fb525058301933f65773d5add669e9e79b1e3d0 :seedling: Update CONTRIBUTING.md with high-level review guidelines
2bb56ed2eb2a91cb59b740cb286992952da3dfed Merge pull request #3154 from vincepri/use-tracker-client
71a6fd702bf0b3ebce0920539f39ec4d21f96588 Merge pull request #3188 from fabriziopandini/remove-conditions-counts
716b093c5414d0611f9a302b3a744f9a9819cb45 remove conditions counts
24e5b8818269c2b7384e441602256bb421c51bd3 :seedling: Use cache tracker to get a client for remote clusters
c97bdd7317cb40d263526773c47a097c863118c8 Merge pull request #3179 from fabriziopandini/apply-conditions-patch-should-preserve-lasttransitiontime
2b501499337f575540d1f6846b60f345a26f468f apply conditions patch should preserve LastTransitionTime
0580e915892e2b454aa14ec5d4fd3a32f61134ea Merge pull request #3172 from benmoss/kubeadm-dual-stack
cfc7c5b813d395f3318355e58c80fa4b59e315a2 Merge pull request #3183 from fabriziopandini/fix-push-images
ebbc072f0d05bc5b07a92e2f9989f9e168ad6bf7 fix-push-images
714b0a97484465a05a67d8ccd1b64aa388b9fac2 Merge pull request #3140 from benmoss/kcp-regenerate-kubeconfig
650a357de4b126d76d3c44fc10670bebb867208e Merge pull request #3108 from benmoss/machineset-remediations
a9fc88e0c67b45d3de907d8e4053fff8abf118bb Merge pull request #2888 from gab-satchi/2844-kcp-etcd
cc492868061d1a98d2ec895bc5e7bca258a4eba6 Merge pull request #3177 from maelvls/mv/push-capd-image-staging
2c77beb565e8150bfa8ab5b078fe6ebfa1b23514 MHC marks machines for remediation with conditions
76382636e03dcf997c59c4e425c19e666ec2cebd Fix support for dual-stack network ranges
cc7d30b2e5d01d2a2aa353fee2c983900353efdb capd: build & push images to staging registry
ecbc288adc911424187b4d293151017c48e3ca34 Merge pull request #3171 from fabriziopandini/fix-test-NewFakeClientWithScheme
b5962688a4b44c008cd04c138a14a76ae1f2d40c Merge pull request #3152 from fabriziopandini/improve-condition-summary
bfc6e20f4118e9451a989484177936987639e404 fix test/helpers.NewFakeClientWithScheme
685d100f6702e70abc1e5cc6cc7f378cecf82a92 Apply new conditions summary func
85a1d2d35112ec8a5dc87ac65192600d97cad0c9 Improve conditions summary
5d508484d4c876953d9dc8aca5d9fc355cfff66d Merge pull request #3169 from vincepri/improve-conditions-patch
deb7e2c83095c255cdcfb037a9c74e52dd7df5d5 :seedling: Improve patch helper condition logic
61debe3c6ee8a7dadb297c8a8b6d8a25f09d2a93 Merge pull request #3159 from vincepri/reuse-testenv
2aeb53299285a86cc9ccaa13365ca58d0b61c8ac Merge pull request #3165 from CecileRobertMichon/mp-scale
d3b3393643ba03430ac032f0f87eda925acf7d97 Merge pull request #3167 from superbrothers/fix-typo
aacf5e37239914a37fa3195741ab8052cca69ae9 Merge pull request #3166 from srm09/bump-golang-version
f173272c55ace9d84b70c46fa9879a750f05d15c Fix typo for "timeout"
808a752beaca3c9be33ca05b82f3f49ed93c5b64 bump golang version to 1.13.12
07db32997cc693f7b7d8811a3a34b3455fbcd238 :seedling: Refactor testenv and remove unused ones
8412e12d573e30f0fa4b6a54131a9919035564c8 :sparkles: Enable kubectl scale on MachinePool
03cff233cf16a1c8cb36f5ec9314ec030a8cf1dd Merge pull request #3136 from fabriziopandini/add-conditions-to-machine
5113f801f130f2d8f0a1b90403b7d868c696c1b8 Add conditions to the Machine object
6494b2d0479131cbc2013f0a0f6193ad27bebb1c Refactor condition helpers for Mirror, Summary and Aggregate
88d43aa5c3755b27927cce21a38cb7a1b0d1da33 Fix to allow multiple test environments
0801817cfd0814764264dd3d2ad03d5df817ac06 Merge pull request #3162 from vincepri/remove-integration-test
129f9c33671b7b72b082546e298d0a45240a2d3d Remove pr-integation presubmit files
eb1f61b831845b19394a3c96986a5456480b5818 Merge pull request #3147 from CecileRobertMichon/mp-version-validation
d70a45b711c63eb7d3c5bf9aa8bdc8e655fb79cd Update docs/book/src/developer/architecture/controllers/control-plane.md
f4fafc58b1d488d071e0c6509f52cf617dfa66b6 Add some docs
990dea9f830e7c1b1636fc6febe64a5d818730dc Merge pull request #3156 from vincepri/mhc-test-fix
691f2688ec648f5940bf443fd64939fd53b1aa57 Merge pull request #3125 from fabriziopandini/add-conditions-to-kubeadmconfig
a2ccee9a7b9037bac8ca07f5b148f23a67607886 :seedling: MHC mapper tests shouldn't create new test environments
28b1087a10015beb421b51cbd4eade9653744710 Add conditions to the KubeadmConfig object
53ca4a0a2e1f20bec1378e904ce1d06305d9b990 add fake client wrapper for setting resource version
0840409bbcc5c18c2e1a58d615f181093c99df84 Merge pull request #3155 from hidekazuna/update_quick_start_openstack
518efd9b793087242f1f1e401788ec4f44fc1c22 UpdateSecret -> RegenerateSecret
2708f8e44cb0e7b013379a120401fc23dbfe59ef Adds forNodes that will use all available etcd endpoints - exclude node being removed from nodelist for etcd client
f541e1d98ea1155f56e618249eef92c30163b74f :book: Update quick start about OpenStack
8a03ae7d608f6dfd3befa7b08ee076253d8b804e 🐛 Make MachineSpec Version validation consistent with KCP
bfb2a3bd04b0fb663f7ccece29fe6e2e4879ea84 Merge pull request #3129 from JoelSpeed/mhc-integrate-remote-cache
35fdce2414501ebaa1462dceaa0eee8949efca7a Merge pull request #3142 from fabriziopandini/add-conditions-to-dockercluster
f31f0cea32d03b158b381ffb330c5b61b87cd82d Integrate shared remote cluster watching into MHC
b8e2384e94c774a82e28c6014d6296b1f8fbf33d address comments
c437644da00406b515201a48b5b93f29b09d3878 Merge pull request #3148 from ykakarap/getOwnerMachine_fix
6d12f849dfee9944b3ed76692475aa468263e4d8 Merge pull request #2685 from dippynark/add-kubeadm-control-plane-manager-role-aggregation
420be29ff38d9ce6762304c185d788d67dde72bb OwnerMachine lookup fix while upgrade
d54acb51d11a3e14a88b4f9f64f8611d58044f7c Merge pull request #3118 from vincepri/wip-patch-observed
984c5aaa83a15df6470ccf18f797168e666d07e1 Add conditions to the DockerCluster object
d09777b1a19f7635d75c978fd844db6e3003a927 Refactor patch helper to handle observedGeneration and Conditions
c6458f3c45393b3ee4e3266703d31844f5cd138a HasOwnerRef -> IsControlledBy
5e1cdf8af620b0a4dcca9a24c0f669ebf86ca75c Simplify nil check logic
1bb583d47ede0e9a3d5fee4a7edb3137059b6684 Fix err wrapping
e72c3ae2c3d845e01154a2a374b239c015d28ad2 Merge pull request #3122 from fabriziopandini/add-conditions-to-dockermachine
48f201066e1b5559cc9949a2c78536bb73fca516 Add conditions to the DockerMachine object
abd2eaeff7712e336fb476da62a8c917ae25212e Merge pull request #3123 from gianarb/add-packet-provider
617783e7e8016a41fc2a6f4ac77abf487ebfd0c8 docs: added packet where needed across the cluster-api doc
f9488acf12d41522ce6f3fcc3455626450ffb9e3 KCP regenerates kubeconfigs before client certs expire
037eced5a9e20c0ca91849cf03ac53885e9c7e81 Merge pull request #3133 from sedefsavas/unstructured
574f13b0cfdff28fea1a1f33c9984187a4e980ac Move ToUnstructured function from clusterctl to util
0e88a403eb18d26301e2693abfc6611e51712502 Merge pull request #3135 from prankul88/remove-log-from-Eventually_loop-e2e
b9f238938280b4c8248c22e50f72d44ea59b9238 Merge pull request #3120 from benmoss/bump-linters
88e65e07754db06b906853e9a4c7386afd0cd497 Update golangci-lint
58455c922f415db8fd693b9d51bd546879898844 Merge pull request #3114 from alexeldeib/ace/webBug
61c949c199afdc5a0596bec0173456eb709237d9 Upgrade test should not report false-negatives while waiting for conditions
ffe99b16ee515cd27b1ac2886001f58148cc0924 :bug: fix CAPBK conversion bug
7b9762100a1d4852a037a9ace0ea96af0b22c20e Merge pull request #3130 from vincepri/envtest-improve
e9d8536b4ecf00e492b6f5c06ccbefbd7fdd90ca Merge pull request #3131 from vincepri/inclusive-other
20dcfe8b3a50ca189dd96044b714243cc4f38dde :seedling: Opt for a more inclusive other category for our emoji
eb8982acfdecd2395e6047521be7ae25e66a98e1 Remove 1s full cache resync from envtest, use delegating client everywhere
3ac3514fed2ea4f0e42b69234994c21af929ac92 Merge pull request #3124 from benmoss/clusterctl-stderr
2afc70d32567682f93468033433e72fd428fc8f9 Merge pull request #3066 from CecileRobertMichon/etcd-mount
d91041321910001b45bb5a8e36b6437db661bac4 :sparkles: CABPK: Support disk_setup and mounts in cloud-init
521cfd8ca1d6b65b8f481fbc0fe28590db11fbcc Switch clusterctl logging to stderr
cadd99c790bb1809a1ef6c14af583e771dca0494 Merge pull request #3121 from deitch/packet-provider
0e6c10b325d11518bdfceffa39239bf474b7de6d Add packet to list of default providers
78850eabaad9ff04708ac30f9f725086b0631ab6 Merge pull request #3094 from joshrosso/capbk-repo-update
256bfc03ae58495e5ac6d48ab5a20b6af2369cb4 Merge pull request #3104 from benmoss/observed-generation
6f8a777d9f1585681422f42a612ed34192f26ed3 Add ObservedGeneration to all relevant objects
87c0343549fe6dc8017eeb94d66f7c826e75cc4e Merge pull request #3105 from scottslowe/issue-2557
e5f05ce90a67df9ac3eac4ff5c9fab6ccd3540df Document the immutability of machine templates
3622e715454ad7f4a33ccba07db12f911ce2c0e1 Merge pull request #3103 from fabriziopandini/conditions-merge-utils
71de75bf3aec4df7f1cc263bc07cdcd177e8f4e5 Address comments
84203f5da55476b30de19c32040854e03936fde4 Merge pull request #3109 from vincepri/condition-patch-utils-followup
1c2ba2ad7b337a65566d07ac24d17a8065cf7bed :running: Follow-up to condition patch utils
70a6230d0eccd22d42d9e51e02dcf4fb5b4e94ca Merge pull request #3102 from fabriziopandini/conditions-patch-utils
06f6f808610b9b6d9cb57d128bc020b3425fc5f0 Add conditions patch utils
e8dea679af417b68f76d2787069dc58169c99fe0 Merge pull request #3052 from wfernandes/caep-clusterctl-templates
2ca9efdc0472faa1f2834879317225650dc33043 Add CAEP Extensible Template Processing for clusterctl
b37f94b2bb2c670e6f2c92ccfe3e712e006c1d52 Merge pull request #3100 from alexeldeib/ace/convert
7d12a45e59bf6b1b43d0ad47bdf464830aa5cb47 Merge pull request #3056 from benmoss/mhc-annotations
4842702321d6534c431aa5d379ea285c7ef51e88 add condition merge utils
01ede5fb1dd8f0a76aa98877d8e7f769a15cf4b4 Merge pull request #3050 from sedefsavas/caep-clusterresourceset
93bfa02db23e6285fdf7b1139b6d5a45369f0908 Address comments
b00dfdefa51a1c6cb64ff2b36a2f6696e8fa3cba Merge pull request #2489 from newrelic-forks/feat/kcp-machine-adoption
de469cacd216d9aa2aa49f2d853efceafcde9af1 :hammer_and_pick: adjust conversion based on review
be4c8a974462a9f6c4f0a41900890b5750f5d329 :hammer_and_pick: fix conversion, add validating webhook
33af0a8207e6398db587ed5ed8a723bb0e03d8e8 Merge pull request #3098 from fabriziopandini/add-condtion-utils
6c98f6dfcaf23757362b54a4e152e70d6a9af048 Add ClusterResourceSetStatus
d5b0274610f6b806f1a4c1c46b1172ce231efc6a add condition utils
f0a02304fb817853bb1fe5056deb9640eba3c710 Merge pull request #3083 from alexeldeib/ace/from
f792d74fc8fe8fc26546c08f018722a23006e855 :sparkles: KCP adopts existing machines
235e730c470fedeb0e9edcd84e447ac8f5bf74b5 Merge pull request #3063 from JoelSpeed/update-spot-doc
d60e9eef1cef09fd68d8622bf42c4e211bcabdd0 Update to propose using conditions instead of annotations
ba2c5399d39f52aa6ca8c2257b2bd577363eb216 Merge pull request #3088 from sedefsavas/capd-webhook
dcfd137e818a01a5f1a7b4d5e412fb1099cef6db Update Azure types to use string instead of float
fa96673db3b399a00029b84e5190f363b2412dcb Merge pull request #3089 from vincepri/machineset-cleanup
f610abd70f6fe3d26e3e87cb7c7d8c832c83ec98 Add CAPD webhooks
99cb87a621c53d60661678021f107031fb998308 Merge pull request #3031 from dlipovetsky/version-skew
1c4d847614e93e683beb84792937dce3d608fc0f :running: Cleanup some internal MachineSet bits
a32a783c8ed15ccf05809e85878ae70f3affa28c Merge pull request #3092 from akhil-rane/remove_wait_group_machineset_controller_deletes
ea5b234bf127b36fcdc7c27aab12eba45e919a1a Merge pull request #3086 from Nordix/enable-mutate-kubeadmcommands-furkat
0e71c56e3c3314db24b801c1c8e576f5509008c0 Merge pull request #3093 from joshrosso/fix-aws-quickstart
d5e9c3a3142aa05e7ca357277520dd0b82f9a230 Update doc references to CAPBK repo.
5ab9ac17b38f4943a477f0a20d8512a142274fd9 Remove extra mention of clusterawsadm in context where it is not necessary.
9b7df762cc14ea8b164f223648aa48aac212a7d7 :hammer_and_pick: simplify file resolution, style
fffe3f0b889e8e84f24ce1f4c6a618b274046ef7 Remove WaitGroup for MachineSet controller deletion requests
ec46f28e01bc6e3ddde903b9fdb212bf6bdeb84d docs: Kubernetes support matrix
f50487481eee941224ec79064d5be1560d82cfe2 Merge pull request #3087 from fabriziopandini/add-condition-types
6da53f08349e1cfea8ae0071102543cbdff6a838 add condition types
fb60c19b1ada535d58022b6fa817ae9fb38de1e3 Merge pull request #3082 from benmoss/kcp-fail-to-update-status
6b1b90badb59ecec0966c5968e0e4c208635e426 Merge pull request #3079 from vincepri/add-annotation-test-clone
d51a3600f3a62513cb2f15bdf7533a3f9650deb2 Merge pull request #3023 from newrelic-forks/fix/too-much-coredns
3cfc8d62903923bbbaf90b1caa03a0d7df475727 fix: allow skipping of DNS reconcilication
e634c34092207b7a090429e9330e2c47a9b1c3cf Enable to mutate  preKubeadm, postKubeadm and files in kubeadmConfigSpec
baedbb83b160ee134a065d3d9d16094e23d4e1a3 Merge pull request #3065 from cpanato/GH-2514
574fd86663665bb19e0cc7f9d475f9f69ab7fd16 :hammer_and_pick: update generated CRDs
3d1345d9d8be278f3aaf4736d9535ac47f6a02ef :hammer_and_pick: add Go tests
4f353d3a8b542dcaf7a0ecca056c52a69543ffb1 :sparkles: implement api, controllers, and webhook
d1d9871ebf3dc774781ab257e5f23ae08ba32507 Treat failing to connect to the workload cluster as a transient error
08e90608fcb2f5e7b41bbfc1eb3bde074ad01a00 Merge pull request #3017 from fabriziopandini/conditions-caep
9dd1ea54380aac57f728b01cf03e0c2365caf76f Merge pull request #3080 from vincepri/controllerruntime053
2e1f7b9ca59e66c46be3755f4943786061a13c13 e2e: replace fmt.Println with writes to ginko's writer
91638c4de6d5c361a6a48e415d5ba41a37c8bcc3 Merge pull request #3070 from mboersma/concepts-doc-cleanup
07c1bfb11bf045f82b3aa618c60302121c5f2358 :running: Update controller-runtime to v0.5.3
e0e567fcc0fb59dde53c26d5b94e374a4f8208fe :running: Test external.Clone annotations in template
cd81068d016ad34ba1fb3b12103d18274a859065 conditions proposal
4f0d46d11602d4a0f14ca003a9609f691cd5e44d Merge pull request #3068 from sedefsavas/e2e-makefile
b4e07c2da04774050dd3a976eabfaaa9a8a8f1f4 Merge pull request #3076 from fabriziopandini/fix-cluster-name-validation
65af999d5e06ef3d9d7e1556dd808885c7192acf [e2e] add e2e target to Makefile
97d5ed89a71431984a7794ce5f3db22b0bd142fa Merge pull request #3041 from prankul88/add-support-for-printing-yaml-clusterctl
34119bb96e08f5246903a0d2c96bf11b99edc974 Add test and addressed comments
4a49189efcf992adb5b23c4ca81d0188ce728777 📖 Update concepts doc
63f56ce97e2af278fbeeaceb0b8f1234aa054b66 fix-cluster-name-validation
da8e88b101e9f8fcd5f6dd4567496d8dbcea32d3 Merge pull request #3048 from CecileRobertMichon/disk-setup-proposal
19985402e53bd2fa6cf069344d8301d0d25e2b95 Merge pull request #3071 from gab-satchi/e2e-machine-helper
8f583196c6d4c4a45a6a2bbef84f3111763c483a :book: Etcd on data disk CAEP
ef440c4f80994f6b0f2b475076ae9c546c5deeaa Merge pull request #3059 from wfernandes/init-images-skip-variables
da0c29c9b080a6cd3041c07cb56fb8cf25286c76 Skip variable parsing for listing provider component images
2c3152c5bfbfa8e776beed2db61e19e839b9e5cc Fixes WaitForMachineStatusCheck to poll for updates
703111b822505e836236541ac51795bb38928a60 Merge pull request #3069 from sedefsavas/tilt-exp
8c8fda995919b7a7a4e2520e35c619925b5bbd7b Renamed "Sync" mode "Reconcile"
beff1e1df8e80d3a4fdb996c86409793ee491d47 Merge pull request #2839 from fabriziopandini/book-developing-e2e-test
efd073b3cd5a3959eeb2e3f4366ef66a2f815247 Add exp and feature directories to tiltfile
b15c8700efcf4407a072fd7da85ea216e2870a48 Address comments
15300a4b6924dcca85c94efdfc06fb80dccaf47a Merge pull request #3028 from sedefsavas/e2e-machine-status-check
69ebae660642368755c58671cac7f34b9cc48fb1 Merge pull request #3060 from wfernandes/cleanup-template-options
53c76fd8b4412202e2ffb0d2379059479f12bc0e Merge pull request #3061 from SataQiu/fix-goproxy-20200514
518360138ccea44981bbe75a61255c7af19917dc Merge pull request #3024 from fabriziopandini/drop-capd-e2e
d60e2bfb62a21d0a2aa45a6e2d81ad44f15a481a drop capd-e2e
2c1b4291f7b3b5519c323abd4e27502c7491c03e Use GOPROXY environment variable if set when building the docker images
663880861ba4ef7be09dee6673ded2208efab6b0 Remove unused TemplateOptions struct
2ef48927c9b9efb313e66ec093641b3b6cb99f13 Merge pull request #3037 from alexeldeib/ace/spec
45cce93f1690cd8b6761b40862b709377623fee1 Merge pull request #3004 from fabriziopandini/fix-test-flakes
898a8d9eada7e52687c53c9a6d62929abba8d750 :book: clarify providerID docs
5a53d567862d10e379a4b67ae4dc6aac8906919d Merge pull request #3032 from vincepri/no-empty-selectors
679a6c1e4081698163b89af83197e93222da0983 Merge pull request #3047 from wfernandes/clusterctl-kubeconfig-env-var
7ad907d4b5b9986f921f0c3bca8071a57ae94446 ⚠️ MachineHealthCheck Spec.Selector field cannot be empty
b180436a0d7946ddc081612b166e05ab82afb50f Add support for -o yaml in `clusterctl config repositories` command
e3518f4ac116663f2147a8d926b9159e7d0db006 Merge pull request #3053 from randomvariable/ignore-static-manifests
e0797c47257c6e9bf01fec992e43bb39e4eb519f Merge pull request #3034 from voor/add-tolerations-cert-manager
fb30ffb11d17f791620ff260bb5c1a77a1f3a458 bootstrap: Ignore custom static manifests on join
c5a21bee56acec6816b1123f617d74d2b084e63d Merge pull request #3051 from gab-satchi/e2e-provider
d7b44b49e3274f98bf2059c43bc4af28c324107a Removes abs path for url providers
d157cdc4a76cf001c6b9e8255e4c7de5e7f17544 CAEP: Cluster Resource Set
694b485ff573cf2eed22d1eee3aa0637275033f2 Add tolerations for cert-manager.
6821939410c37743b45c36ec91d94c37dba1998e Merge pull request #3029 from sedefsavas/e2e-mhc-test
761b9803b1fffc918bb5767257352c9cbc4bce54 Merge pull request #3027 from sedefsavas/e2e-md-scale
5bcbffe27c7cdf45bda3ff56fc68d0f68fefcb23 Support KUBECONFIG env var file paths
d4a3f1e650879f48eff0af0c99e6e30ab5d7ad83 Merge pull request #2979 from sedefsavas/deprecated
962b0eaa9d99c1966d65719ab1256a1cd0e2c711 [e2e] add mhc test
50350d8f6c243132093e98cea7910a8863ba3cc3 [e2e] Add machine deployment scaling helper function
bfa499083ba3c316b647d9c211baf4453a2cc1db Merge pull request #3040 from cpanato/remove-todo1
59ceb80f9851861328578469f0788230785cecf5 [e2e] add machine helper for status check.
e217d2dc7facb56078d9c2cd3dc4b6857b93db7f clusterctl: print stack trace if verbosity is >= 5
df9fcf9442ee353d2b388f8d79361a75d21ec487 Merge pull request #3035 from fabriziopandini/increase-e2e-timeout
515ec1ef3e763860129cb731fa33af3384ae83ea increase timeout for HA upgrade test
98d461988fec43f6471ff13417bfe079fcbc5b5c Merge pull request #2996 from cpanato/GH-2957
0ca8bdf88814b69274e3370ffd414820eb153714 clusterctl: add CLUSTERCTL_LOG_LEVEL environment variable
aa6acaac25ef923be874d31f4834d293625abb57 Merge pull request #2974 from detiber/CAEPProcessUpdates
9970a175c258395de4a601f96efb315c50db0656 Merge pull request #3025 from fabriziopandini/e2e-increase-parallelism
d40fcd73e6c1bdf2bd6e90f91c0a8ecaaeb184ac e2e-increase-parallelism
3cb12b019cc2c9d4ca83470fffdce5d5deeb1fec Merge pull request #2971 from spectrocloud/fix-duplicate-bootstrap-secret
5bb84f7968ac4c95a3e09130488123ea201173fe fix error from duplicate bootstrap data secret
0136b06420ce3a661ff090204b64133a0d8b37d7 Merge pull request #2945 from sedefsavas/e2e-md
c3ef9222bb61524f5d3705ca1bf1202f3afeb720 Merge pull request #3008 from dlipovetsky/kind-0.7.0-ci
d599e57b1715343ae9f63828eb840ec349608206 Update kind to v0.7.0 in integration tests
43ddd327a4963a4f0351c1e7aea47ef944b69446 Merge pull request #3018 from vincepri/forward-port3010
6106e39d2732e6ba088c24d82343891d3a536853 :bug: Exclude conversion-data annotation when MD reconciles
a799265e225b8f0e47b4642c8211a9213d0aea9a Merge pull request #3011 from vincepri/convert-ms
d118566b933f8af3c62e2d94e6ba75446cfac08f :bug: Convert MachineSet annotations from v1alpha2
730f6a48c10b4771cde89eb2216972d6a4177a4d Merge pull request #2995 from benmoss/envtest-wrapper
c0c4c3bff3de34e22379e18cee2fe741c0dafc36 Merge pull request #3003 from dlipovetsky/clusterctl-capd
58995caf8804dec79912fa89fc4490893deceeff :book: Misc. fixes to "clusterctl for developers" doc
5d7c1459b44a94b93dddc9b88b45c1e27cf53797 Merge pull request #2880 from JoelSpeed/workload-cluster-cache
090ebe6fff5ada1d4468ff46fdd8ddf42efc1b6c Add Remote Cluster Cache Tracker and Reconciler
6f47913e048fddcb36ec0ba3d2d93dab90f39949 [e2e] Add MachineDeployment upgrade tests
f7e4453e2e0f446fc69c0b59d594f19d3597eabc Convert controllers package to use envtest wrapper
6fdbc5ed794ff0224b698d0ae0d7e4ed09e2133e Add envtest helper
94418a9b6ec353c05a22c3e1718a5050065c2f1b fix-flaky-test
23a9ec341de33c399c542558c22046cb413082d5 Merge pull request #3002 from vincepri/uncached-check
26f5c70e0af0fb7c0cfe8a2a9a25062cb494dac3 :bug: KCP should bypass the controller cache when initializing
60eae740ada88164e4b395d176bf6a90bc5e591f Merge pull request #2877 from detiber/improvePausedHandling
30c377c0964efc789ab2f3f7361eb323003a7759 Update and unify cluster/resource paused handling
0bb5cbfc9e846ade5e327a5810cbb0c1b120824a Merge pull request #2987 from SataQiu/clean-20200430
ae33d8193e00f8c16a428c6b8ca8e48b3f9adb7c remove use of metav1.FinalizerDeleteDependents from tests
6dc38f9b64691822ccbefc8c08ae4a49b474f602 Merge pull request #2962 from scottslowe/2941-ext-etcd-docs
59a696e07b5e4620ba66ce17cd35d2d0b0ae73d0 Merge pull request #2988 from fabriziopandini/fix-clusterctl-soft-ownership
184c6f00dfa6efacc791dc41ed564c74467bbef3 Merge pull request #2968 from randomvariable/k118
10dc497e95ea1d2eeb9810d50930118631813635 Merge pull request #2981 from fabriziopandini/fix-dev-guide
a84d2b7394c97fa4b44a8059f48fd7842b0f3cb5 fix-clusterctl-soft-ownership
07c909bc8496a12e8ca35f6cb25bbed8c0499b03 Merge pull request #2980 from fabriziopandini/fix-issue-template
d5dd2997d37c0daba1708c915095d1ef8d2879de Merge pull request #2985 from neolit123/1.18-add-fabrizio-to-leads
e9a3e3707cb8ae78271092113771c3408f1800ef Merge pull request #2983 from fabriziopandini/fix-clusterctl-read-config
8c4adbd73449a1196125b99d9f94c74bc63f8ee5 Support Kubernetes 1.18 Adds and modifies e2e tests to test scenario Makefile updated for local testing
5480a4744973c5472254a7a5d8d88ae883fd35a2 OWNERS_ALIASES: add fabriziopandini to leads
96746dc911ebe5db867eca4d0e6617dd8cbe4fda add area label to the issue template
05d72fe4e007ca97d54e258cdef58eadd1da57ad fix developer guide
751be4ed3a26b5d1072fe10acfc4b96488bed239 fix clusterctl read config
0c36d10aa28383f48b5d2d8747cd7ecd045121ad Refine experiment deprecation policy and graduation criteria
e50ffef50bfd8908f4b793d8f22a305eca01d7d7 Refine experiment deprecation policy and graduation criteria
87ffed8b76d6dbdbf2089ac0c3cddece7cc0a364 address comments, fix headings
bf845fa2d035dd38cbfb04355ed0550137d6f7f2 Add deprecated comment for e2e framework.config
7cda00b20b09cdccf2ce4e5e952ecfdc0f87ccd5 Merge pull request #2958 from sedefsavas/kcp_upgrade_fix
8bbdd95a72db2affef94130bc51cf6c33e5a4780 Fix for 1 node KCP upgrade
ef72ed653063b5b2aceb8b35c288a7014ce7e3df Merge pull request #2972 from prankul88/developer-guide
49d1597d44d6cb05f2911846ccf7414131f26d22 Add additional context around experiment lifecycle
1c2d89c70ea6365f1920ed887e546dc9fa1663b3 Merge pull request #2966 from fabriziopandini/e2e-cluster-cleanup
5a2b54eb9bec6b2395e8a99c04120c831a9fe456 Merge pull request #2920 from benmoss/mhc-annotations
693da53ff8edb54a1e2cc3b775329e85a470e9dc Update Developer Guide
847621301fa3a651576cd743f9baeae5baca9d1c developing e2e tests
106c74960d8aec87be4274da5172a54995860feb add workaround for panic in high level helpers
fff092e8e6fd90fb4f5b86b13ee736b81f7c8129 Merge pull request #2940 from vincepri/ref-issues
c9796ac87f16be6161e38940208b7634e536cd53 Merge pull request #2959 from devigned/exp-infra
56290fba2256b6af66c04c04877556b73001c3db Merge pull request #2951 from wfernandes/fix-config-error
9e890d7cf9bd395ad3d9661fe804dbc8075317b6 Update MHC proposal with new annotation strategy
1876bc044b76efb1fabad9dae6ddf95303cdd075 Update etcd certificate discussion
6c31c0e9a2719724d524230e6aad769ef6f01a7e Update external etcd documentation
b4067020e6a4fb4c21e59a94323899e8f3ed356a feat: grant access to experimental infrastructure api group
13272a80e9c22cee6ae76949b0430fb97a0c77e9 Don't return error if cannot find default config
18ce96a31a4a7102848effecd05c3753003e092c Merge pull request #2948 from wfernandes/fix-config-provider-output
29dd8f3aa9b5a6b367df35b7e460f693f9e582d4 Merge pull request #2946 from benmoss/fix-external-etcd-panic
92e71e151dc66331a68676ab1c97a350e26a8f66 Merge pull request #2932 from alexeldeib/ace/tiltExtra
476434e1741288ebdda685aa6e25f1c199521641 :bug: fix typo in tiltfile
bbd0b8ba77457e9b25765eb1d3e889d69626f136 Merge branch 'ace/tiltExtra' of github.com:alexeldeib/cluster-api into ace/tiltExtra
83d342e4de81ab44b278907c32e4d8465914aca8 :bug: fix missing quote
5bc847de1a89e4dbfea3b212dd8cdf52bf4938f0 :bug: fix spelling typo
5beec587b49dd36ad7c9d5c5a43c6e648182f6fa :hammer_and_pick: don't remove helpful comments
8d45780a664708cc1ffae009138106275e7b045b :hammer_and_pick: remove extra files
07a65a49543c06c0f20cb065c28f56c06a7d8211 :hammer_and_pick: add machinepool feature gate for all providers
db6840c6853f57c10e7e43350476518ea6f27b93 :hammer_and_pick: fix extra args type
43eede24a8095c6097f5182170d001af664e6a5b Fix output of clusterctl config provider
99a95aaa59492924b04e6dddbea17992fecca24d Merge pull request #2942 from fabriziopandini/fix-e2e-timeouts
8c4e53bf7a005a767393f90de7436b6d73b2c7c1 fix: review feedback
3a4c1fbc72aa038a7adb52c630c56258bf07dfc5 Merge pull request #2931 from wfernandes/remove-cert-manager-clusterrolebinding
ffb8aed6acf6bfcabdddb385293cc473eec9a170 Merge pull request #2933 from prankul88/remove-e2e-clusterctl-folder
548482efbe0757c9dff9e9e5f6982ffbaf6c37d3 Merge pull request #2929 from wfernandes/fix-delete-annotation
515b651ed826328b884c432d75bc4e0d262146fe Fix NPE on external etcd with undefined secrets
e8966135e0659fa37fe0997b9cb39203008fc8df Add text in CONTRIBUTING and CAEP template document
a227df77f71f1bc82db1df93a6cf7efa9e4d2887 fix e2e test timeout
ac8927b588938f77ea8e637d7703c3c46226c651 Remove e2e tests from cmd/clusterctl/test folder
65b5a88055b6de3a8249e5282d5085611ee8b3fb Remove invalid ClusterRoleBinding from CertManager
60fed98ef4aced840fd2bbc95bd92fa3a22bb729 :running: Remove issue-proposals in favor of CAEP process
ba3bd5c095e0c7af6d39ff62a6bd77b8609722fe Merge pull request #2868 from newrelic-forks/fix/dry-run-side-effects
1fbef48e1d3174b3942e2da2793687184feaa196 Merge pull request #2935 from fabriziopandini/clusterctl-config-env-var
70921f2f0fd6cd2db218207848e4c36af0787495 Merge pull request #2938 from vincepri/legacy-docs-link
9f69b99dfb4607727f55d8fcf5c91953e445a9a6 :book: Point legacy docs to release-0.2 branch
ce1baa298f9830f7074d8725282f13eb6bf1c0ec Merge pull request #2936 from fabriziopandini/increase-test-e2e-timeout
30d58b802f528b5b4a8c5615fa7205c87028da85 increase test e2e timeout
cfc7abbaa437bee0effe746fd0d3853dfbfd6553 make replace variable to consider variables if defined
41867434092445b33a861c9c364b30fc1d5d9584 allow clients to set SkipVariable option
d83881e6bfeba5eaf5f982ac21e0e3e59ddeabd7 :running: allow extra args with tilt
62b7a1d777fd19a5af1884960eb59378844f90d6 Merge pull request #2905 from nader-ziada/config-provider
2481422f7099f010669a14d573d17587f721e503 Merge pull request #2884 from fabriziopandini/e2e-quickstart
8103e296bb062550ec8dbdc24fc3846bdfbbfc5f use skipvariables flag for config provider cmd
5596ab2a8d3f7dc14ca63e7f425df7c8f76fab3d add test e2e folder
32a48623f2c245d641ca7c963af818273a62c070 Add DeleteMachineAnnotation for MachineSet Delete Policy
3579b12838f9e28dc2b21543ddc044d97811725e 🐛 report lack of webhook side effects
04d9db7ec54dee1da47d1d182fbef5bd1f5a9599 Merge pull request #2887 from benmoss/remove-annotations
acdcd7ba3f56b410d331fba75929a5eb7c2ebd78 Merge pull request #2898 from wfernandes/fix-config-repo-output
64c1dbd0298b068d0701eb365bb61676cd86fce6 Merge pull request #2925 from rbitia/numberingDoc
3999986b2681fb46f669bf46e3221cfed157f32f adding docker/kind prereq
8284f6bb776019b4629589fc9d0970cf9b6abd2d Merge pull request #2922 from fabriziopandini/e2e-reorg-helpers
af82f1da387f35729006e81c2e31b5dca3d0ee4c Modify the output of config repositories
cd51c260340bb820663d621e3b90de691774ee24 Merge pull request #2924 from vincepri/chmodapidiff
cf10671566fbf78908408eb0d78757a9f204d28d :running: Make ci-apidiff.sh executable
d809bb5557ad3cddaea7b0d4ffff2bef47e7f9b2 Merge pull request #2923 from vincepri/go-apidiff
57126de7a0dfe47c3de4138ed4b27b7ead816120 :running: Add ci-apidiff job
87009ce5ee2624074007c637981f9b48e3368193 e2e reorg helpers
c96fd59faeac7d75d80335048bd681fa4c5f0073 Merge pull request #2856 from wfernandes/clusterctl-kubeconfig-context
02d07a2a7adceb7eae81ff57dd50f25633f7308f Add kubeconfig context support to clusterctl cmds
f38fd7d37aace69704b68adea3ee9ad2ef19c6d5 Merge pull request #2911 from fabriziopandini/e2e-add-clusterprovider-and-clusterproxy
01f5f2cbed3aed6980e638927b62fb41cfd5f2c7 Merge pull request #2917 from benmoss/capd-cleanup
20e2800770b16677e79d2ea0241994b6869e96af e2e add ClusterProvider and ClusterProxy
731b4d0ace4751d13395765086db4d518e83beba Ensure that capd tests always clean up the kind cluster
5fdcb9e8dcf0ce93d9eaf984a1de1b1377290f8c Merge pull request #2875 from JoelSpeed/mhc-warning
d2f01e77a10961f7051ab039630327a34587fce6 Merge pull request #2909 from fabriziopandini/e2e-improve-e2e-clusterctl
d5784c9a2961dd5e3f089413eeda548c9c0b56e6 Merge pull request #2817 from JoelSpeed/spot-instances-proposal
9082129bbd38a9388f52c9300e58e2da3293f517 Merge pull request #2882 from vincepri/update-roadamp
e3a4ed7977b6789e03cb9e4d6e5ca201e43a726e Merge pull request #2913 from benmoss/machineset-replicas-default
0d46af2b1e93caf39bc9936b1621f3ed8e2b8d46 Remove MachineSet controller Update fallback
dd029668e3d1e35404cabe35c3a85604d2661278 Remove machine annotations from KCP
eeb69f8eefa44b3de67a6460ac3da776cb496306 improve and cleanup e2e clusterctl
0b964b734167081a2a994f28983877140c58c50c Merge pull request #2904 from fabriziopandini/capd-selfhosted
65ea933e9f23a72a5450871b4d172c93b7750083 Merge pull request #2841 from sedefsavas/kcpmachinedeletion
c59b99591029e4a7426c861f75be7bd5464c1c2f Merge pull request #2907 from fabriziopandini/kcp-requeue-until-ready
c63a45f8d2b3e526b80079d0ae227c3f15f79082 make capd ready for self-hosted tests
a6879acb866c6269dcf1d531380807eaeda875bf make KCP to set Ready without waiting for re-sync
a19b557e078b7efb9b8d3784374559b25cd33e7d Merge pull request #2865 from benmoss/patch-1
4a06bfc4a187c9ed354336aa91fb66079b444f2c Merge pull request #2899 from wfernandes/fix-config-error
00c9d5763ac61340af40f76ea74b426e17ed4bad Return error if clusterctl config doesn't exist
538edf673303ad1361777a6a0da03589c16a61aa [e2e] increase timeouts.
3acda5218ff34b119be4e246bca8cc68614344ee [KCP] Recover from a manual machine deletion
f952f38bb3d2b2d8aa4085c2db0c56d3d2d8c586 Merge pull request #2901 from rbitia/quickstart-update
87487169485708dbe1562f57a279d1d35e860170 Merge pull request #2900 from mboersma/quickstart-fixes
7be2a0e02e5188349dfc2bf6a58ad9a3c707a511 cluster version req
2db9400891b0f8be31293e9457017092c24c5213 :book: fix some grammar in the quickstart
4d3edf9cd75a37b96ab8872eb44d6342b6209ea5 Merge pull request #2893 from fabriziopandini/e2e-improve-management-cluster
8869c2f18ce0289f62a51124b02939c7b20c8847 :book: Update Roadmap with focus on v1alpha3+ (v0.3.x)
ea22b7f68ccd13e04a90a27baff5af5b19723f8d Merge pull request #2892 from fabriziopandini/e2e-clusterctl-improvements
19121e7ad16a50f876cc7bbbf35753b41dd70c6d Merge pull request #2891 from fabriziopandini/e2e-add-namespace-utils
a9c8bf9ae7c1f53e28b77292832f762d5eab17da Merge pull request #2894 from fabriziopandini/e2e-dump-all-resources
beea8d889ee723e01e1b59a6251cb09ca8238b21 e2e dump all resources
5a0a11cc953907966d1dacd91fff459a8cc869fc add-namespace-utils
4b62b07a0a4d5e421dad13b8a3b8f315145583f8 e2e improve management cluster interface
163bf79ff81f5c05efdcff9dc0c81419d19aa651 e2e clusterctl improvements
efe6b709f680f26c1ebe474492ebbd98d4328c0c Merge pull request #2869 from nader-ziada/util-lib
262e9b354a1ccdfd2e7ea56124c491e640e0f781 Merge pull request #2883 from CecileRobertMichon/calico-quickstart
a739c7e06a8f455fb71f5fe807902fcd9e332af9 :book: Add Azure tab for deploy Calico CNI step in quickstart
7bb418c5b8125b02423596bf318aeaa166a63933 Merge pull request #2879 from sedefsavas/e2elogs
f1f88af7bf8fa39b04529f1e5ebfd5ac28e162da Add log streaming to clusterctl e2e
b1b35203e680c02a7a707e30927224812aeb122f Merge pull request #2878 from prankul88/update-machinedeployment-doc
662e2ec458fbf0e19b638ea62449a36a0f6fbbc8 Update MachineDeployment controller image in docs
65dc85f404ecf940d2beaa76d7a1038cb011d9db simplify code by switching from docker lib to util pkg
8aac9551b5b711d1796c6e807944d3e457ea32d3 Add a util library to parse container image name and data
cb8f8e40d3a013a9cf8328f7a3df5553501f7baf Merge pull request #2870 from fabriziopandini/add-clusterctl-e2e
743cc26809410f1b51b794e3753bee8551b08e22 Add note to top of MHC docs
af07f85ddf27ecdb57b2a98b5398159d3a0f7427 Merge pull request #2874 from sedefsavas/doc
772a5d15f8eb60f74e7d4b4516ef78ceb189cb62 address comments
e747136ef3ad1983914e10ad127d3f95f347311b Fix incomplete sentence in docs
abd4d8f3001e5ab71b9c6915e76a846fc3a12cd5 add clusterctl e2e
51138ad376d42552524527c10d7d02d530e93291 Merge pull request #2866 from wfernandes/fix-godoc
b8c3d93c5c36a2ea683eb2f17bfa61a5de344737 Fix client.UpgradePlan godoc comment
e34f9ac79c89e38e1b079cf0ef0528ddff671eea Merge pull request #2833 from sedefsavas/selectmostlogic
0c7d6e0d881242a432a05d615c49e84fe68e17bc Merge pull request #2819 from fabriziopandini/add-clusterctl-e2e-config
47a9925aa88e168e76b436fc341c42a31f0ebd61 [KCP] Fix for selecting failure domain logic for ugrade
e174682dc081ad9206c1efedd51bb8796f30e88a Add benmoss to cluster-api-reviewers
7a0dc68d103dd368ae3956f0f18bdae400223770 Merge pull request #2864 from fabriziopandini/fix-WaitForDeploymentsAvailable
a6f389e9e47b3b896e9be706987890f12bd50464 address comments
19ef0f5a271975536cb0574ce05b9e515040ea8f fix WaitForDeploymentsAvailable
0435cd9569a4104ead3311d21a25aebfc147df8d Merge pull request #2862 from wfernandes/kcp-unit-tests
bf4fcead5c439b9c42dcdaf1fd8ec543ddf76b6c Merge pull request #2597 from gab-satchi/2560-replica-count
9b909cfa2c72037246ded8ac0ae82c1e07e70581 Improve unit test coverage for KCP
02ec8e483f83e6f35c231d06bb7dea3519c1cbcf Fixes default control, worker machine counts overriding user specified values - machine count values assigned in the order: defaults, env vars, flags
22db99318aa8636f01fa3f71534a277e8b60ef72 Merge pull request #2820 from fabriziopandini/add-clusterctl-e2e-discovery
9fe8ad47e130758564d976dde7757d3edbba8c88 Merge pull request #2853 from rmweir/aks-docs
bbf11a9c2620eed1027c0ce56ed8bc27efc68cab clusterctl e2e discovery
ab058898e5ae8949459ebbc57664be8475ea05f9 Merge pull request #2858 from fabriziopandini/clusterctl-fix-replace-variables
9257a50abee60ae60589f29a4a0c46367904e1b7 clusterctl fix replace variables
9491481f3d059f1102acb75edbe07142bc8d1055 Add subscription id to azure quickstart
edb585e03ee23fb4d34aba7e69058c5e6b30abd4 Merge pull request #2848 from fabriziopandini/clusterctl-cache-github-calls
96f0bed8ad151a0bb29584d426fbee893ac59880 Merge pull request #2821 from benmoss/etcd-leader
a9c54ec7aba6cff939dde21d36a333b2621d1e96 Merge pull request #2832 from gab-satchi/2810-imageRepo-subpath
22e254d37416be6ac81982dc2db3af00b2bbe3f5 Merge pull request #2842 from prksu/clusterctl-k8s-server-validation
fa18c568a015036a60130ffeaabd5ab6d3cc062d Use 'coredns' constant to identify container image name
19c54a8d95a83fb3bd5a588158dc9b32b4ebde5e clusterctl cache GitHub API calls
d823fc7ba56ae98980f148932838be6ee1a8432e Return an error if the leader candidate is nil
a5b31e9b6682d6d7808ca108c5c7f94f423fe272 ForwardEtcdLeadership uses leader node
1c4935e4658093ee5ebc02a3713bfe99e237fb8c Merge pull request #2845 from chuckha/owners
86d4dccb8f8b11e777ffa5664e4df22afa2f2bda Update OWNERS
319076d6dc5339a069d8a50610d5ef18c7ce850a Merge pull request #2843 from sethp-nr/patch-3
2bb9546c0815abc75378edaef7a26f9c9f6b0605 :running: Work around DNS interception
21fce550d692243665cc5261a3f8036cf8e83952 🐛 Add kubernetes server validation on clusterctl
b5b5f508badeceaa4b5d97925f2ceb8204a8a660 Merge pull request #2834 from nader-ziada/cert-manager-timeout
cd655cd98e15d321afe4a978cfcf527dce23a57b Make clusterctl cert-manager timeout configurable
05a8f91b0c6001ced15a69d18afa7963153a124c RemoveEtcdMemberForMachine uses leader node
8553a3755a1e70fc72f7804dee5a65b31ecb8ae0 Add forLeader to etcdClientGenerator
3ec58ba0b216506b153e073fc7604da7c37ec55d Reword some test descriptions
48ca777fa0f3083ae4f45bdb9ea1a78cf5bfaa39 Merge removeMemberForNode into RemoveEtcdMemberForMachine
09f87a2aadcd590952e17684f5c05259337e4da9 Merge pull request #2829 from vincepri/remove-misleading-log-line
20771c7d149bfde3c1e00021bc3d024f930384f9 :running: Remove misleading log line in CABPK:
52330e92f0a6627804c1af52553e4d92f58b9815 Merge pull request #2802 from sedefsavas/unittests
ae3f83c3544fa5ae88892621e7d90f9b082dc84b [KCP] Add integration and unit tests
3f0710b1e25dffb2e0b93e8c3a3589763f97e8d8 Merge pull request #2806 from wfernandes/workload-cluster-unit-tests
d821cd5b6eced78eaf35fecc78b44f59a3e05a9f Add unit tests to workload_cluster methods.
3288e3e5ecee56ae7bf6007f55a4e1138fe1f3cc Merge pull request #2814 from tahsinrahman/add-controller-version
5a4df3dd0ddc40b800338d30bc80e0716d28d960 Add controller version in logs
f73b4fc13ecb5c695db5558f62b52c8ab63a9cd4 Merge pull request #2809 from wfernandes/kubeadm-config-map-unit-tests
6d54ec4bde9b49a5ed1991c22bf3219cf2aca36d clusterctl e2e config
2775242fb1fceab350ee0d3838de6a935cfe19e4 Add intial spot instances proposal
ecff70af1b839c4086335234d88b1b8c00c3383c Merge pull request #2807 from benmoss/update-image-repo
815ad8d92ff689cb8bc111358896ce5ac9e13364 Add test for UpdateKubernetesVersion
1be9d30282071a91adcd28f2c6bd911d8255be46 Merge pull request #2808 from nader-ziada/kcp-unit-tests
43c11e4e0cd8696b760de482457fce9d0c787ed9 Add more unit tests to the kubeadmControlPlane area to improve coverage
bedda68c8c1750b8b5fd9b339e1eb1351a9622fa Add tests, nil checks
6d80fc0e70f30dfd5938206ec782a82ac2ffbd19 Merge pull request #2804 from gab-satchi/2609-coredns-upgrade-e2e
1eac03509a921c8ce5971c7e9b6248d360fa5f30 Update kubeadm configmap imageRepository
ea4bc4be505456535acb6b2fa4145b6fbd29e707 Merge pull request #2791 from cpanato/github_repo_tests
ac2cce716cd53220adc254ec0da7cfb0de9f6b64 Adds coredns upgrade validations to upgrade e2e tests
2cc85702ab31f9ba2baf22adefc9b4a4a6e942b6 Merge pull request #2785 from wfernandes/etcd-e2e-tests
1717c75ab68acd919a705e36973d9a89ab175672 Merge pull request #2799 from cpanato/GH-2798
6b830c4f8e6d72da8202b2a8b79e88039fb4e39c tests: move NewWithT(t) to inside the t.Run where applicable
bf69bf0b586f3d8e3cedf9264614f8dbfd88c5ab Merge pull request #2792 from cpanato/GH-2787
127776bc46e84584734e4823ded4e2b8fd9a69b7 tests: add missing tests in repository github
718c19d8d096c4d3bdab43508c05fc504f2bc513 dependencies: update controller-runtime to v0.5.2 and controller-tools to v0.2.8
1c86f1c4b14619b138d1e2b45986a85f9df6ad02 Merge pull request #2797 from rbitia/quickstart-updates
61baa5b640f20b946aabc642adf980d869e0e361 adding export sp commands
0634eb8fa679ddeb9d20367f9863104095d643a8 Merge pull request #2794 from benmoss/imagerepository
e3e8630c00c5a95cc208ea964d79ede7c10b803e Support modifying spec.kubeadmConfigSpec.clusterConfiguration.imageRepository
68ba2582ba212bf7071d208351bcc84c2d046886 Merge pull request #2786 from Nordix/fix-issue-2775-match-jan
d205b684c57b6aa228c07c859746d9168433022e Refactor upgrade tests
e977a76b98e8b775e7f13059e5f3952bc6e6514b Move etcd upgrade test into separate file
314a00b9fdc266685d1440442cd30d2372fe0420 Delete workload cluster in AfterEach
25dd126c4e4605a3f7a1aaa603ac66e4d9fef13e Isolate upgrade etcd tests
56766360cd2c265dc1f0c3d1014eb614c46f9e67 Remove outdated comments
21146ecd25a526cdbd5576d3d10e7d553b90d03d Add test for etcd upgrade
d29357eab5e43c4afa293e55130a794820252d6f Merge pull request #2773 from sedefsavas/kproxyupgrade
61c12daec73cb41d00043dad2bb979918d11381a Merge pull request #2782 from ncdc/rand-seed
8494a2f45865ff8eaa5dd849044f31f885a9b084 Merge pull request #2780 from Nordix/fix-issue-2775-jan
b84e05771b5ae227c55e84a6c3a16db9b45220a2 Merge pull request #2744 from wfernandes/fix-yaml-err-msg
a076fb4d033a5cc3f38a99037ed268591799126e This patch will fix separator problem issued in https://github.com/kubernetes-sigs/cluster-api/issues/2775
2f4e31eaf88d0007cb01fa649a8a021eb2cb8302 Bugfix for match issue in 2775
c9e23102da2531e3d723fcb44401327654db869a Improve error message for yaml unmarshal
7012b9cbb37a2fa638a72ba5af8f324155073dba Merge pull request #2758 from sedefsavas/e2etestenable
917d7df2a0ae2e234ab62b8c5c58bca4a710c7bf [e2e] add kube-proxy version check
e65fb5c6cd271ab9dd80f28d1fc7f0ac79ddae4a Merge pull request #2783 from randomvariable/retry-for-all-nodes
5028770b5654066c3fddf339128d3e1bba954855 bootstrap: Retry node joins as well
864e95120f35dcfab9f21968faab76d1a7641a03 [e2e] enable all docker e2e tests for CI
2f296a3cab96ea071b6dbe0d91318cac479a5083 Seed the random number generator
2b2bfb90e952248bd264b1548f3d37147effef6e Merge pull request #2776 from fabriziopandini/clusterctl-add-retries
4672438fa4e67ba915a4698a11c9928040bcd505 Merge pull request #2763 from randomvariable/boootstrappy
b8026b35a857fb15407290507cb3ae202fa581b6 clusterctl add retries
f003f6edacba5c5d6a6cd812039150b43e2e39bf Merge pull request #2781 from bboreham/add-to-glossary
dcd3d51881552722234c3443d9d597f5e5c3db98 :run: cabpk: Add retries to control plane join
a406781c0f44f8252424bb9a32a27dbd5c9c52eb Merge pull request #2772 from sedefsavas/reorganizeunits
fe4f500fdc41f2b65d11c8e959bf9c2696e21c28 Add CAEP to glossary
3235dd07898593ef4bb7f6badfea0fb4c01052f2 [KCP] reorganize unit tests
12a5cc729167ed4ec1d92b8c69ad4df2515e2313 Merge pull request #2768 from sedefsavas/scaledownfix
3950a9c5614ebb0e08e35ec6e1100ac3c40e89a3 [KCP] fix for machine selection logic for scale down
30b339337efdaa476cde37a553b8a451ced853b4 Merge pull request #2767 from vincepri/split-files
e93b4c540b487e2e04c18ed4a87e3fec96811fde :running: Move KCP code from 1 file into multiple logical ones
3ac1e8c1db862f968e0a606491cdf5b4229df006 Merge pull request #2766 from vincepri/move-file
8a562611ec668224de005b77b8bfb342936fe734 :running: Simplify KCP controller file name
637b9c9363db12787dbcb0d5a342b07425ee5d8f Merge pull request #2761 from sbueringer/patch-1
f598bb25117952b4bedc6434bed1603de28c0550 Merge pull request #2762 from fabriziopandini/address-2472-comments
9a7f15d2bb66c1219e2f381839f891513478d7a4 address 2472 comments
5f1d2406a6e81b2107488bb9c5d1c9fc1bbb17be Update CAPO image-builder link
04ca7d1cb7f561eb90ea292d592a7b5e02138069 Merge pull request #2742 from chuckha/control-plane-tests
ba222591ce909f4400bf8512f9496d8f7cb9166c Merge pull request #2683 from sbueringer/pr-update-openstack-book-doc
80242decf6875ed1cca14348bad7095556e083cd Merge pull request #2757 from sedefsavas/2754
4a174e5def79f9d7a58284792d7b0b9a4d4ce214 KCP: fix for #2754
cf8be838f602701e2e0c7e86f7ea800606701d04 Merge pull request #2655 from sedefsavas/e2efix
36c2d6f947ac2f6eb280c918b6a4708bd99a6f1f update OpenStack prerequisites in the ClusterAPI book
35f28e985a909b9ce10f7a3a0aae79dd69a4f7c5 Merge pull request #2752 from fabriziopandini/clusterctl-retry-create-inventory
23ac30268aa08ecc3440184abc1422cf54781963 clusterctl retry create inventory
ec24629a36b52936d6aa125521b0ad803e94b3bb Merge pull request #2736 from cpanato/GH-2433-14
d1c2d701dcb8f0ec1bfd27dc479f9c28ad060934 Merge pull request #2684 from dippynark/add-gcp-auth-provider-support
077ef0cef51e16de7a25e5ab6f45b74c6f4faa6b Merge pull request #2750 from SataQiu/fix-book-20200322
a3b948404d0c4cb542a9e3460d7e5afb7a9bad74 small fix for quick-start
01226c2a53d1251fc6e94e7798dd1945871571d4 Merge pull request #2747 from chipzoller/master
7058fa6f49073a7dd27f815664300731e02d7c37 Added auth provider support to clusterctl
5e70dafa8c54db05912573c9ce4cf6addb7ffb0a Update quick-start.md
9c03e0a94c44060452c39658d23417c508f1f4d9 tests: standardize gomega imports
d66ced6695b6ae71b3226ddf943f5712bd88464d Merge pull request #2746 from vincepri/drain-nodes-cluster
88fb43a4c0fe659027d7330dde965b107523cf0f :bug: Avoid draining nodes when deleting a Cluster
8206c9252cb1a8fdcd44ad405ae08a81c72c6cfb Merge pull request #2745 from vincepri/refactor-cp-logs
2dcf93dbee77bc0ff8f3db9b39a2beacc21ad970 :running: rewrite kubeadm control plane logs for consistency
3483baf04000bbf0e44c4bc5d2ba4ce6ab9679e8 Merge pull request #2739 from vincepri/rewrite-watch
42bcaf1e7b42192408da99d9cfbaf0dfbdb547d4 Merge pull request #2734 from chuckha/partial-impl
d24f1495f977ff0f6c06148ae8dec6fea863ff0d :running: Improve Cluster.Spec.Paused watchers and provide utils
ef2873d33851f3dcb40495084d56135107e30790 Finish the pending tests and clean up a few other tests
632b296b115d311605c72aaa2741ba110b5e5cb7 Merge pull request #2741 from wfernandes/docs-aws-iam-policies
df9d6511179c25c5b3c76db9f85bbd499e033fe7 Add IAM pre-requisite notes to AWS quickstart
e0c232bef6af8b84d9051541afb8627d0df4555d Merge pull request #2740 from vincepri/actually-return
83bf04eea8e508011a2a13e69ad4588df027cd74 :bug: MachineDeployment controller should actually return errors
3d781deb897ce4efaa095c45fc94db733642e4bb partially implement control plane
a97903fa1e7e12f86ea1a2e2d1e4dda0b7c52a0c Merge pull request #2733 from vincepri/binaries-first
f34d70dbe07faacff3b982e569298c881ae537b5 Merge pull request #2729 from chuckha/modified-utils
594de67fca8cccf8cbbecdbb61b2ff79ff44d878 :running: Build binaries first during release
c085d0bcd3a0ed8b9759f3c24aa1c21efc3d0313 Add a modified util function
867b2afed0e6a4509a74bb123b7c6f2ab0f7ffd7 Merge pull request #2728 from chuckha/control-plane
67bae898fc9804d6c3b247f6a4d0c549ffdded4a Merge pull request #2730 from CecileRobertMichon/quickstart-order
aca0fb0bcaa0689f4420d2aca9a95e65227db760 :book: clarify order of steps in quickstart to deploy workload cluster
038c619307355a9122084dcf6f40599ce8e3de80 Merge pull request #2727 from chuckha/capd-timeout
f9078e190e7c0897786abd184ea29ec3a552d959 Merge pull request #2712 from CecileRobertMichon/quickstart-docs
17fe147e4dd8a82d2c58347bcf19d5c3d7703faf Merge pull request #2675 from cpanato/GH-2433-11
1bfdc02209ce78bd376b48dad1333485499c1a32 Adds a control plane struct to clean up the reconciler
337800f9f3403660ce399e8bc12f2ac720f4af2e Merge pull request #2726 from vincepri/use-leader-client
ab3ba06d870860bf6e0a909f0998c69507bbb904 Increase a constantly failing timeout in capd
b1a99d342e88ac2425f8e8bd8e62cad69ba3530f controlplane-kubeadm/test: standardize gomega imports
50b8d492df3b007dcbb0274060d0cf05d275b8cc Merge pull request #2725 from gab-satchi/2723-unset-dns
5c7ff07108404b1f7dcc65b3d420520d6d6f623b :bug: Etcd should talk to leader when moving leadership
697dee0e7a67239391464e1aea2c3e5fb7df58d6 Allows dns image tag to be unset
8b29a9adeeba4677da4221b887cce61155f925a3 Merge pull request #2679 from wfernandes/clusterctl-local-overrides
46879caecf541e7aad117432ba5b04bd9ce9e26e Merge pull request #2714 from elmiko/fixup-capd-cluster-template
84663c6c5de34e5a47b9a9f69c83c10c60ac2f69 Merge pull request #2720 from chuckha/improve-tests
e4a7b3d124c8c5fdb64465ddef918f57aef8c57e clean up tests
39d03a81309154be96a13c6eb45c04494236c26e Merge pull request #2715 from CecileRobertMichon/provider-docs
8d53a1197de363d716a29e6e2c8d01ab18e7eb95 Merge pull request #2719 from sbueringer/pr-add-capo-to-clusterctl-meta
62bf449c6a5f06b5c06697d8cc00e803c78ac50f Add CAPO to clusterctl embedded metadata
9502e8f582b0c33bb936b46017a2aaa24d6412a7 :book: Update providers list to supported v1alpha3 providers
a559a178e95aaf35b9c20b8b24d738b8361fcd70 Merge pull request #2707 from gab-satchi/2620-kcp-coredns-validation
f5b1315bbc09c5aaea51d9b57dbc6f8fb09bfd61 Uses released v1.0.7 coredns-migration
73315ff74e48058ca518e57a6f626821caab40b6 Merge pull request #2704 from chuckha/fix-links
fb6b135ec100fba449c1bc597ef976c09f29a0fc update worker kubernetes version in capd test template
ba6d842a98de2b9abd30c1d372f00907af9aff62 :book: update quickstart Azure variables
91215b8e5c8d634ab11aeb3112701ff2ed23458e Merge pull request #2708 from frapposelli/fix-restclient-timeout
e499ec592d954fee273194a9d5949d91a06cc548 Utilizes new semver utility that will parse out custom build tags
a21b1fb23f57b3ebeab4cf7c20393fbaf6c1efc5 :bug: KCP should set a timeout when trying to connect to remote cluster
5d70dff03dfc93e5c45875d70ac86373c705454a Merge pull request #2664 from newrelic-forks/rtorrents/2653
8329d0164e7ac89490dfab7d571273426932db01 chore: expose leader election parameters as flags
2e981412124777783da15726e2b729212a59496c Merge pull request #2711 from chuckha/remove-etcd-removal-annotation
877800f2f2a321a2a877ec669c931bdc1db41264 Remove a troublesome annotation
ceb528ce93dd82f833585664f0407fc8b82031d8 Validates CoreDNS version update - Skips validation if ClusterConfiguration undefined - Skips validation if previous version undefined
5f14f88152342e2bec7b43c904ecb911f8301e4f Merge pull request #2700 from sethp-nr/patch-3
ea82875cb04abbed482378fad421cde3dc993776 Merge pull request #2706 from chuckha/only-local-links
bd01f87a98eac285eac36913bfa96ddb15e841e8 Disable link checker in book
d71344431f5a774b9178ffea6cf2add06720751f Fix the links in the quickstart
5822d7b7c6d07c03790b3a789f6baf1f7b1b9c23 Merge pull request #2701 from vincepri/add-log
276416a5fc6346de112ce9aa3b44342f2507063e :running: Add log line when reconciling KubeadmControlPlane
7157b85b20c6fd77a128753e28e5261d3fa417f7 Merge pull request #2696 from chuckha/etcd-health-check
4472a5dddba6bc5da44bf7f037bf9864a69dd947 :bug: leadership forwarding for removed members
55dc3f5cf3a5eaee0ffbd0a0a1e5d7e631251255 Merge pull request #2698 from sethp-nr/patch-3
cd2c55e3ad2802a9b42b1f3c96558d41730b51fc Merge pull request #2699 from vincepri/fix-repository
be67001290effdfae90d40331cd12d89ec8f97c1 :bug: forward leadership by talking to new leader
8692ec9ef912b2ba10647b571576d01d7e62d5fd :bug: KCP spec.clusterConfiguration.imageRepository should not have coredns/
52269c5227ee9266476ed4496cc90ba33efb2d55 Merge pull request #2697 from vincepri/mmp-proper
32e6e61a254c170095c85816fb0ea0f6d575bb89 :bug: CoreDNS validation should only look at major.minor.patch
85efa5c3437584a4e5c78d2167cd7581f84d5350 Change the number of expected etcd members
b3201248243be638e921c4f7ecf346cd3e44c8ac Merge pull request #2695 from vincepri/move-leader-newest
0e354614364cdb30c46c339873c82c3811028715 :sparkles: Move etcd leadership to newest Machine
d5b9a37cc4efdf4872d266e3221d495e338a483b Use overridesFolder config to configure overrides
4d87796f86d57bbe54f2936140d5e49436fe0284 Merge pull request #2525 from alexander-demichev/etcd
afe5f9a38465c22c31cfa410967e123db8ebc067 Merge pull request #2676 from christianh814/patch-1
d06be1c58073953bc21e3d91762bd98dd28290c9 Merge pull request #2634 from JoelSpeed/joelspeed-reviewer
21c07c94c5473e0124a83ce8a412014d59cdabc2 Merge pull request #2674 from sedefsavas/machinesemver
84f0b3b2cbcf2a6ca8a8c8461a15cf878e455e9c Add semver version validation rules to Machine type
3af8e0a2e11c971bf0f0626a8364e9a7d1fae141 Merge pull request #2691 from randomvariable/proxy-validation
f4038928da6658cfb1341766135f66781d7929e0 kcp: Add additional validation of versioning
f5347ced6a5898df41e83bca69972a2cef142b6d controlplane: Normalise image name for kube-proxy
8e8c880b309a1b1dc4e6a085fcd2df07f296fabf Merge pull request #2570 from enxebre/fix-2565
94bd603999a11e0e95c9786b1b9db54ca5c542d7 Merge pull request #2678 from newrelic-forks/other/kubeadm-config-defaulting-and-empties
a963cbc71e028fa1228aef76059cc06667c34bac 🏃 mark defaulted fields as optional
29bd3d0d800b68461edd4729771ca2765152bddd Merge pull request #2692 from CecileRobertMichon/tilt-azure
47eeca02eacd339eb538dc2420b5b0c8cf76002b Merge pull request #2667 from cpanato/GH-2433-9
55aeccfe86bf31c53a33a61a7df4e65fa1b8d07e Merge pull request #2687 from SataQiu/fix-log-20200316
7f0354a9a87b2f8bdfb993b012114fb861bd7976 :book: show Azure tab in Tilt docs
0b27ad5d897136602072c885836102a8044b2279 Merge pull request #2680 from cpanato/GH-2433-12
1d5ae9d7e7853e0bb3ba50772905931649d7042d Merge pull request #2681 from cpanato/GH-2433-13
411cfbd23d309db0f96de0d7a2f8f1fb801bc029 Merge pull request #2645 from cpanato/GH-2433-8
95e7d7d9cfbb7d995f7c03e561c4ba2aacb013c2 clusterctl: log which value clusterctl mover is setting when pausing (add key)
3dd2de5a896cc33bf85ed3f8061b36fb5d3a8008 Merge pull request #2686 from cpanato/fix_typos
cb9b2dcfdebc29c54e89dc8557f43808153485ad util/tests: standardize gomega imports
b1bfdfb27d75189a12119a9ac608bbbe9e7d46c7 test/tests: standardize gomega imports
703b4af94a118d0829479105b1b00087cf7ddd69 typos: fix some typos
832c75eb9ba7682432f9957cdf1264c8a2bdbd90 clusterctl: log which value clusterctl mover is setting when pausing
2e507f4c52dfc9d2ea6ae95694e96f384d86a9ac Add kubeadm control plane manager role aggregation label
f11383ea28f46e10c7738e160aa4ec25b4b97dca Merge pull request #2660 from newrelic-forks/feat/speedier-e2e-image-builds
a433c40b4a4db24a1dc6284be66accbad302bc05 Merge pull request #2670 from chuckha/testing-doc
7c95b1f167a8ce0cd815a7c6dfb1d01f2002b28a Update docs/book/src/user/troubleshooting.md
156359de0ca290d5d21f1c3bcb1da1ff7c767125 [e2e] Move cluster cleanups from AfterEach() to AfterSuite()
9d39c3acc2228c52364ec6d0d7f742e8954f16da Update troubleshooting.md
bf6a34a8f91a73c99d46031c7b4dc499244230bb controllers-noderefutil/tests: standardize gomega imports
4422e8102d11bfd9b5674822f27334970b5e7910 controllers-mdutil/tests: standardize gomega imports
ba1aa04ce2805aede74ab2e83365f750d8acbb2a Merge pull request #2666 from fabriziopandini/clusterctl-use-exponential-backoff
54331c6e4fc5f27e4323d8b476f72a52b01e9d78 Merge pull request #2673 from cpanato/GH-2433-10
6d409315b42ffaea7a143ff8a49f8848d58aad2c Merge pull request #2668 from cpanato/followup-2643
ccbd5cf6292406783245df61f3be34cee6078a34 Merge pull request #2672 from randomvariable/fix-tabs
1ba44f5716d1136196aea9be2b9efb8fda3f8712 controllers/test: standardize gomega imports
601f4158232364f712857e2bfca528e55832b731 Separate tabs in quick start
3af93dc229cc85b46248ea5beaad1783820ab4c6 cmd-clusterctl-client/tests: standardize gomega imports
92ea5920a212b54f2be7f5fa2c5c11ee6f149e34 Update testing document
64d5067c333e6c106e54eb322b507816a113fc44 Forward etcd leadship from machine that is being deleted
6ec9a6b5e676fbdc3ecf8ffce32e127f52109ece cmd-clusterctl-client/tests: update gomega expect
ce5d51793e4c1da35f1e70d31fca5a13dccbfbc2 Merge pull request #2643 from cpanato/GH-2433-7
51a0c61aef2cbf9bd03394d937f19ca217bf12f9 cmd-clusterctl-client-repository/test: standardize gomega imports
a0110f6928749e40c81d93ccc5ed35887457c6ab address comments
574cd077509636d0da461a12961f9c991032a057 cluster use exponential backoff
5252a7a0cbccace0708efeae13a7771c1ed4dd40 Merge pull request #2656 from sedefsavas/pflagkcp
9e71df1105555418ca8350bb1451bccbd23bec6d Merge pull request #2663 from voor/patch-1
c0704517e1f34dfe6388d7153e34e7da324469a1 Merge pull request #2390 from chuckha/kcp-caep
1459279bb0e10304f0b87163d3eeedeb24771dae KCP: Migrate from flags to pflags
fbbd67fec266b7b3905671a10dbf7ea800b5fee5 Update overview.md
e408ee4cb433a126cf0ad65a22e36395d7b70368 Merge pull request #2661 from fabriziopandini/cluster-repository-local-windows
737e36921121d12504bd78a66f8d86c72c5daba5 cluster repository-local supports windows
bc07391625f97c3e20902b21adbb76f9d2dc552d Merge pull request #2662 from vincepri/fixup-404
9b93f426edf8448296d745f2833ee1d3b0aa9fc1 Remove links to installation.md/html
866bece82bce4a7fd5ef713a7e152fe667a3ee50 🏃 speed up e2e image builds
5bb2219e9c587f55c9ca309c8d02962350001b34 Merge pull request #2628 from randomvariable/capa-capv-doc-updates
c79ef7e02621104100d27182656a87032890ddbb Merge pull request #2647 from sedefsavas/semvervalidation
7d724eed63ecf4956f6a9eb3d985e2792bfbab78 Merge pull request #2650 from vincepri/move-filters-out
7ae984d6a7f01dac36007be37b3327e01153d18b :running: Move KCP/internal machine filters in a package
dbe88957481e238dbd46fe8056b8a6d1a44883e8 Update quick start parameters for AWS and vSphere
d02e8218793f296563867554ed01bad2131d8a50 Merge pull request #2644 from wfernandes/kcp-coredns-tests
77262915be35bbf3566522daaf10a1508d0c47f6 Merge pull request #2649 from CecileRobertMichon/tilt-doc
af95ee5ab0b86c832141fc3f541848aa3336f52d Add tests for coredns upgrade
b43f852872f24e50589ecb50e62c442e8d439f26 :book: Update minimum tilt version
e3a77b0220d62bfc969727dd9f5e9d43550e918b Add version to all KubeadmControlPlane objects in tests since there is a validation now
846731f8a0995ea0ac3e94fb453f563d5344e865 Merge pull request #2648 from JoelSpeed/improve-mhc-validation
8e7ee69aa81f81892e8508f1170b64dbdfa2a6ba Update CAEP to reflect implementation changes
69c0f012310ebc4cb154e3e5f8f66402f002ac62 Add KCP spec.version semver check
2389e86f3f8b348d1266f6ab226a9b2004635ea8 Validate MHC MaxUnhealthy strings are percentages
e3d592f858df0c7cb1baaf40ea4c50006bf2cd79 Merge pull request #2496 from JoelSpeed/remote-cache-watch
5c279e11f6c3c30d31fa7562bdf88dcf71c992a4 Merge pull request #2641 from ncdc/fix-kcp-upgrade-npe
54260061ddcef07160c11aabac80702edf2851a0 Merge pull request #2614 from cpanato/GH-2433-3
bfcc6f37fe122a9fd9f4c53a96c9410f916c2054 Merge pull request #2632 from cpanato/GH-2433-5
c5b7cd846d51789d952f637645b6d3ec9b82ace2 cmd-clusterctl-client-cluster/tests: standardize gomega imports
9c500eed6ea1dd9344c4483dddd1ad5a045ad4b3 Merge pull request #2638 from cpanato/GH-2433-6
b07cfa867ee55dc039c268878cb2e8c226759875 KCP: fix NPE if ClusterConfiguration is nil
b0feea045900d94b21cc4cafb84b4dfbd968a9c7 Merge pull request #2631 from SataQiu/bump-controller-version
fddcff2f94e3c9649d3d53b0ebf7fb858122e492 Merge pull request #2640 from alexbrand/fix-typo
be48a143415cefce07e6bc86a065c889e0d32dd0 quick-start.md: fix typo related to clusterctl
d0014155fed881510a8c21174e4e62be048a166a cmd-clusterctl-client-config/tests: standardize gomega imports
092ee97cd45e9f072115c2b19f117e4ba3fd10e2 Bump controller-runtime to v0.5.1
bb43b1e9465975a2ebc13a294955881573494576 Use cache for watching remote nodes over informers
6f9e7fd64884af0a68da532b224a6c29269369e4 bump controller-tools to v0.2.6
40e4724fdc99620efd98aa0752f22f028d180b72 Merge pull request #2625 from vincepri/increase-kcp
c6a420a8710bcaf1e0e389bae56079a778f41561 Merge pull request #2622 from chuckha/remove-kubeadm-reset
816f9f874d0ee58ee3c9f895e4622aad7cb45d6e Do not kubeadm reset in capd any more
b6aad253dfcdafc263e8b399d3a97732006b3069 Merge pull request #2624 from chuckha/version
84e99317f547f8d5ef0ab7e7e3337037f9d5844f :running: Increase default KCP concurrency to 10
2369761a2138e443c051062f1a08fc9c4657419f Merge pull request #2623 from detiber/updateFailureDomainDocs
639ae471ad2a2b2573d12e417b34898e3355806e Be consistent about version use
762cb28fed89afefa27c2b74dc653fdf88fe2c39 Merge pull request #2595 from fabriziopandini/clusterctl-doc-airgapped-config
b8ca3623eefb9f801533235f03733699869aebe1 Update provider documentation for failureDomains
508791327182c7bc4220e619a8ae5068fca59310 Merge pull request #2607 from chuckha/kcp-docs
8979daa20d1d1b2bb9492696844ddd7bb6842aa8 bootstrap/tests: standardize gomega imports
b0638fad646357e05349892810a121d383798dd6 Merge pull request #2574 from wfernandes/kcp-coredns-upgrades
8f8e2be7f6ac085fe53f957c7cf423e47d39efae Add documentation around KubeadmControlPlanes
af66cea7147ca07e6e52f505e4b8bc2b6b62bd76 Upgrade CoreDNS when ImageTag is specified in KCP
8214cfa0a614d2e99557afe3e02b72169b0ddf1f Merge pull request #2621 from fabriziopandini/small-fix-to-quick-start
5536e5e1ff6c73fe1a1c844d7a9c4f1054e8f046 small-fix-to-quick-start
e75e56b435c4fe5edf72dfd12d1ca3905928dae8 Add JoelSpeed as reviewer
c1acb351db0f78a8fbf42fca0b90c1aee22dd565 Merge pull request #2615 from cpanato/GH-2433-4
a9e0495aaee3ca52049a5aca87c200dd0cb727ec Merge pull request #2617 from chuckha/capd-artifact-output
37706a17daf81b7f3c0c64ec27f6b3a2a89487a3 Merge pull request #2616 from ncdc/fix-kcp-validation-etcd-npe
5348476f2b80dbae699c8308bc121599b85dda76 Improve capd e2e artifact output
f2555be359055c7eac86b5a85f22ad25e2dfe834 Fix NPE when validating KCP etcd settings
46d4250eecc5c50788f45eb3aee08e8082d1c857 cmd-clusterctl-api/tests: standardize gomega imports
f2a71f4043dc8408a9f35bdfae9df9774c655ca9 Merge pull request #2590 from fabriziopandini/reorg-quick-start
652eee135f5de576d0acc83ca02987c390240796 clusterctl based quick start
5f503ba9e4545712f5f87bf4c47a2524d72b295f Merge pull request #2605 from vincepri/cleanup-kubeadm-private-api
cd602ce6cc65cab1cc6a449aef7a93b43b033b08 :running: Remove private APIs from Kubeadm v1beta1 types
96ccd375dd2e3828195f7689d817cd0542c70abf Merge pull request #2598 from nader-ziada/etcd
d765b947670019f205d65cdeb062d3a166ca4850 validation for not having both local and external etcd in kcp
417ecad8b564a4308e84ee7bd18930c0595dc23e Merge pull request #2559 from sedefsavas/kubeproxy
37fec7759f8d2bbfb99c96e5e947fa6cc85578e2 Merge pull request #2604 from chuckha/upgrade-after-field
359b22a4c42aa82f356aa89207194573faaa8fbb Update kube-proxy daemonset image tag during KCP upgrade
6a08677ca498aafc035ad170ffe36bff6e13b741 Enable upgradeAfter field to be modifiable
5154da4caf18b291b1e1e1aba0c635e1d76d3093 Merge pull request #2586 from fabriziopandini/clusterctl-all-image-overrides
915d42e551bc9eb442014196f9cad1e1940f821e address comment
48be8c5d09f3309a5b7c636d410eb3d51b1aef9f Merge pull request #2581 from vincepri/add-tests-etcd-kcp
69b6fcadee48b9ce7f76f4de0112bb4cf517c748 clusterctl doc config for air-gapped environments
44bfb43bb60c51e7b13a01ff438311933d088d10 KCP etcd upgrade: handle conditional update & add tests
93bfcf7dea9c2acfb3988af58c098d8d7f1c2f8e Merge pull request #2592 from fabriziopandini/fix-cert-manager-timeout
fe88878c01ec7dd993d3ee16e5e804a8b2c47e3d Merge pull request #2589 from cpanato/GH-2433-2
d053396cd521241ece27417dd5202dd53c3084ea tests: standardize gomega imports
1f7b4c17c59b5d7e468652b024f1e5c599504008 allow kcp spec version changes
c22157891deef6a832a4c190c994b7750b440172 Merge pull request #2548 from JoelSpeed/mhc-tests
47e8d16582b41661c9ed29617e36c6b30f67f0d7 Ensure infrastructure is destroyed before deleting the node
b939d70c3a7de75bbf1b70b58e816dc260f35632 Merge pull request #2588 from nader-ziada/move-docs
1004ead0877282f2f8d952a98aca0b5aac5c317e fix cert-manager timeout
1fd69308fe9a83e3f63d95da65e8321f6d7ede86 Add message about possible problem when doing clusterctl move
9db9537a9da3d7682a90bc4435271533e7217080 Merge pull request #2582 from vincepri/allow-version-change
2ad0fb192973b9133e27059e6ac5892aa31ef0df Merge pull request #2583 from vincepri/flake-test
992f4109649d72ef3449174a169b0e3ecc25ecf0 :bug: Allow KCP spec.version to be mutable
5f5e57f8d02cfd9f9496d288269a8343eef9544d Merge pull request #2571 from cpanato/GH-2433
30f1be09dad69f78b4dbe23c2a58f5a64d730e31 :running: Fix flake test in KCP webhook TestPaths
078d188934e26b071e4db622246c5f138476c77f clusterctl support image overrides for provider components
810240aa628cd8b2dfa655abfbe1596d0b3533f2 clusterctl refactor NewComponents signature
e2917bf06435c7911bb000a9a83efe1f9aef112c tests: standardize gomega/ginkgo imports
4d0192c37fd0d0fa5d334ef8b90dd90d24526253 Merge pull request #2579 from chuckha/etcd-version
ba7decae795a4d6d5ad669941c284f34eb14ccb9 KubeadmControlPlane now respects etcd repo and tag
a447c9feb7c0fcd5e7d21d5333edae6e633cb66f Merge pull request #2553 from chuckha/control-plane-webhook
81719e3416809d993ed62d981ed6fe50c0c5b5c4 Loosen webhook validation on control plane
b51a61ec6b1007347524fb65766a8b351e4de0bb Merge pull request #2558 from fabriziopandini/clusterctl-cert-manager-image-overrides
158e99887e8b73148b0fc7db101bf5966d274f41 Merge pull request #2576 from vincepri/avoid-printing
f07371de19756a95a4a1f09c236ace004261be22 clusterctl allow cert-manager image overrides
cf1b3e35e96eb2cf2728e167fd884967d6a91358 Merge pull request #2575 from chuckha/ready-optional
16df55119f1bc3470927dcdbbbc9443816d02746 Merge pull request #2573 from gab-satchi/2572-logs-update
7132d61594d474484fe8890d0de2cd9a3bfee68a :running: Pass a stripped down object to controller.Watch
a298ab4b3481a25a81f7ab7da2626df5050e5ad9 Merge pull request #2552 from randomvariable/ctl-e2e-gomod
438708b7125ac0f5ab05998df04f5b869e9884e3 capd: Make ready an optional field
be2d5957276d416020784e64c41430c709ed89c6 Clean up go modules
b67cdd8eaa2f53967d548612ef47c6ba1d5e5275 Merge pull request #2569 from randomvariable/capd-bootstrap-reentrancy
d753066708abfec080e3be31a13c5a4bddd95afe update misleading logs
0b9dbbaaf30520e3ef369a0ebd76b69ceb13c69b capd: make setting provider ID re-entrant
1e035aacf6df838654e1e6bf5da8435929eb238e Merge pull request #2567 from JoelSpeed/mhc-docs
31a2cb2d90a3c3e52716267496fb86453727cc66 Merge pull request #2568 from fabriziopandini/clusterctl-allow-empty-vars
2fcd33ebc9e292df0c6fd490cc4ad31371897e8c Merge pull request #2464 from prankul88/update-defaulting
fe1aa8668ceb75177d4f83d5f38e9bc8879b55ee Defaulting webhooks should always set label from Spec.ClusterName
619071a988e13d6762d0865fccd9b52ab16cdf91 Merge pull request #2549 from JoelSpeed/register-mhc-controller
541aed9c8022cde54e747b93a9dbd54306240198 clusterctl allow empty variables
011ed380b5a1d491e3d6ed2dbeac935b108ec884 Add documentation for MachineHealthChecks
5b9dbfa519cf3b3d058047e7200da0f6b211462a Merge pull request #2564 from JoelSpeed/fix-capd-calico
f23cdfb563350bd724d87ec08a5bb9db3c334ff3 Add e2e style tests for Machine HealthChecking
ea7a9f4936ac2965de31303da9b18149d1445558 Merge pull request #2563 from fabriziopandini/clusterctl-fix-wait-cert-manager
4fe087da56264e93572127a1caf9ccc78547e1e9 Fix CAPD Calico manifest URL
e78f85302bf89003880b2a46c0c130b0c6f056f9 clusterctl fix wait cert-manager
017233e749edb8ae676575b5f83a997e23794765 Register MachineHealthCheck controller and webhook
7b3ecdf462950eaacf76dd8cb4c1061fffe27618 Merge pull request #2550 from sedefsavas/2469
1e50e937f09b80e0fff9ad473f3003f124e41f6b Merge pull request #2551 from nader-ziada/2546
ba73af84acc984a0b0cd38fc510d99b57c1afbb7 Add NoExecute taint check for KubeadmControlPlane nodes
ddbe5161e43522e1f615a1bc522c67d66378760d Merge pull request #2556 from vincepri/no-more-clientgo-incompatible
73262d7d295d74665eb8faedcc1d86dc423644ad :running: Add a validation check in place against client-go@incompatible
ac1dee8cf441dda7f1a36fd4e149e195ef16db20 Merge pull request #2547 from chuckha/refactor-workload-cluster
828f12ea7e2f315d72145da88b12532f80a26fad Add instructions for providers to upgrade to CRD v1
7e53ac0849efada148ad4acc0e26938ce1f4e53c Merge pull request #2534 from chuckha/capd-flakes
4ad7383b23af0b232cc73cce4ae9015e0ee3c97e CAPD flake fix
bd1285773d37edf404f1b62316bac9e7711ebc45 Merge pull request #2494 from JoelSpeed/mhc-remediation
835db803c126a143a8829c08ac6febf8b8efd3bc continue improving management/workload abstraction
8d6e9fb68b05fc955b625dd48cdd6929668ed9e4 Add remediation logic for Machine HealthChecking
7711f9528dc2d1655b12425f889c0aaede951e7e Merge pull request #2539 from timmycarr/master
45f9cbd6d588180b49f440677b6b08557fadfcf1 Merge pull request #2540 from Nordix/capbm-mael
a4aacce9416a118015d02b2967bca4123e6ed6bf Modify Metal3 provider repository
5bbea60660bcdf1f17b4a5798f10c4201642b5eb Merge pull request #2537 from chuckha/command-context
48f11e050e019ad3e2e3f3b020e2b3fd84a1e107 Update move.go
802230ae15c78875bb0add0f389ba2a4696e52fc Merge pull request #2538 from sedefsavas/2536
b12e701d2a402593a3f06cc0195b95f34bb23165 [docs] Add a section about matchPolicy to "v1alpha2 to v1apha3" doc
4e60875bfcf0f7df004a8284a3710dc154e078c0 Merge pull request #2531 from chuckha/links
5dafcdca7586d7d5b890a2e1f8993c7cb7c5664b Adds context to CAPD with timeouts
7d1358c4ea879386e4741563b6e61a1b9f244fa0 Merge pull request #2533 from sedefsavas/2442
56bb9c3e6249f705582b917190292cc017850efe Merge pull request #2524 from fabriziopandini/clusterctl-add-retry
fe3c8ed00d3b70b30ce6f03cb5ba83199bf638d7 Set matchPolicy to Equivalent for validation and mutation webhooks
edc797c90ec4b3d11393d915bc78687528aa8e0b Merge pull request #2532 from enxebre/roadmap-spot
db914e2447f557450dff64cabc6f882e67d8f09b Propose spot instances support for roadmap
5f1b9ab7c5fd7c7c52a9c1f9bc18e79c690ef0ba Merge pull request #2517 from chuckha/cloud-init
72ebca70dd7f5073649c7e2252f065108d0eba85 Adds a link check verification for the book
88506f80bf515f082aee73b1c6b0161a810330d2 Merge pull request #2488 from chuckha/kcp-read
e9038a58adf693d7b54228f145fee85416a94a83 Merge pull request #2529 from chuckha/book
3ccb9b91efab740a91dc807e5d0939dcca3435a8 Merge pull request #2519 from vincepri/requeue-cp
42ef987b9805009079f6373e793660ba493bdde7 Merge pull request #2526 from fabriziopandini/clusterctl-improve-error-msg
313a2eb9f967caacbf02dac6b156803b3c12886f Merge pull request #2520 from noamran/1550
4c6e9d9338d035291bbf08ed51f53bc54239c3d4 Merge pull request #2512 from vincepri/exp
d27e4a35ba16a921d577bc0d53068f78e8949ed6 :bug: Requeue while cluster's control plane object is being deleted
747d3347a98aeecffaa952263af33f6a4f027ec9 Update controller images in book
12e96256318cf933b7e0afbc608997c565322edd ⚠️ Add exp/ package with MachinePool
97097699f713161d5e9b4afa2620926f6c41bdf9 Merge pull request #2462 from Nordix/capbm-mael
eb75628796376f095c1e196301e1c402290b82a6 clusterctl improve connection error messages
40ea63e0b1a7f920965b021223b3b8c463ffac67 Wire up kubeadm control plane Ready status
fd19f2cf37c2791602472c7137846ffbee49f7ab Merge pull request #2493 from cpanato/add-health-docker
af518e9dcbdf78ed1747344fc919474c91f21cf3 cloud init package has reduced responsibilities
952a1d92fb7ab963a821579582af2c1b611f51c5 Merge pull request #2522 from fabriziopandini/clusterctl-fix-upgrade
158cf05fd368f2dce7bfb6404926f8f8c6b18124 clusterctl add retries on create objects
b06b0cd0432e22eaacc606c0a6c72e76a4255127 clusterctl fix upgrade
a643401d11cb35c6f7a42917ab125519729aba0b Rename Metal3.io provider from Baremetal to Metal3
3dc93ab4f278cc358a43f423354e4e60c4fd3a79 upgrade v1alpha2 to v1alpha3 doc
25a933a307b1495edc13f6bf7186c9d3328415e8 Merge pull request #2502 from sedefsavas/2459
18b03b91e96d3f3b70106de607516c03506a7e5e Use controller-runtime's client ObjectKey instead of types.NamespacedName
aa289e08abc3545909e05f11789ca253da7b0920 Merge pull request #2508 from fabriziopandini/clusterctl-remove-pkg
92c59da27ef67b014395c81f00793b721960c0c1 clusterctl remove pkg folder
cb079834fa40d09dbfdaf35de16679ccd8e4f9c6 Merge pull request #2487 from wfernandes/exclude-metadata
4c4fba50a908f56b0fa451c4e0aaee83ff81a7db Merge pull request #2509 from fabriziopandini/clusterctl-developer-workflow-with-docker
2642acbdf59b63b174e1d755f88b27b721ceeb3b clusterctl developer workflow with docker
f65d4aea4d2fe02d604dcc873cd736a29eacdbfb Merge pull request #2511 from JoelSpeed/disable-interfacer
cbdf897b015bbfed94de5d44abcabe4b64c9802e Disable Interfacer Linter
9bcf8ce5e1a05c79bf310ce456442e39061f44bd Merge pull request #2491 from SataQiu/fix-clusterctl-version
1029b64ac87d8dc2cee6423858c5ae207eee18ff fix the bug that clusterctl version command does not show correct output
5e03ae53c91683c1ade05c5635acf95364352abe Merge pull request #2504 from fabriziopandini/clusterctl-upgrade-plan-apply2
441d1de9e867ef2cc7ee91c3a028a0396808a131 Merge pull request #2503 from noamran/adopt
0990af6ce09125cbe589cfb7caaa3bd847082fbd Merge pull request #2506 from chuckha/capd-networking
265d6deb745217d88acf962f36f9b20caf83e4f4 Merge pull request #2392 from detiber/webhookTweaks
aa165a29ef253c7e989b0b82c7a08da1645ea5af Merge pull request #2490 from dlipovetsky/remove-etcd-member-cleanup
40225fa65386059c2a448dd99f9fd5ef798713a6 Adds kubernetes networking to capd e2es
4efe0fd564ec4c205830df77dde17bd967f44b91 Merge pull request #2498 from vincepri/refactor-owners
1c284d74141bc6a2be7642963bef6dba1156dcb9 clusterctl-upgrade-plan-apply2
1928ed769a539025776d829fd6a78442ddcfbf94 Update hash to include KubeadmConfigSpec, since we plan on making at least part of it mutable
b02e71839d357a7a9c37f47d81e1a350f6f6c89b Excluded metadata in annotation during conversion
d1e6475569fbe97f0b7af05beb3a4a3db5bc4ad0 removing clusterctl adopt from the docs
20715b149b3cafcef83c1e683bcb2b6c3b9b2a60 :running: Refactor OWNERS files throughout the repo
664e48131926f656f9dd0ba5cf0a393e6c0a2542 Address feedback for unit test
3011d8c2580c69c3be3e24133e69e27eb1dfac07 Merge pull request #2443 from wfernandes/bootstrap-secret-type
9ce4b9927216710e05530e9cf7d5e2d7d8106c08 Merge pull request #2500 from ncdc/fix-kcp-diagram
2611d564b76ed5c06e2fb28bc58815c3d8c0e8c2 Fix KCP diagram link
c60882f255a34c6d097c1022b9406b5ea60b37f8 Merge pull request #2492 from cpanato/update-go
81cf0aaea6a3221c3a303bfbacb3e8aca0b0ca0c Merge pull request #2482 from chuckha/reconcile-rbac
71a4eb5abf6505f6e9740038ab8230b5137f388c manager/docker: add liveness/readiness probes
f6d8b9966cac5ed4cda5437c913076382db5f6e0 go: bump go to 1.13.8
6ea40e0aab36f3576cab1c3d28c51730d29ef654 :running: kubeadmcontrolplane: clean up removeMemberForNode
308f931d5f0c457d6253efedffe7e860126c0744 Merge pull request #2485 from ncdc/kcp-fixes
b16a118bc9a934fc9a96980c71e563db9536f760 KCP: set managementCluster in SetupWithManager
2d2c9c86d49edfaeaec70001d66d3feb1211e4e9 Merge pull request #2481 from vincepri/improve-script-cache-ext-bins
d9456dfb5c26fdb23477326d6c18ddab38fe877d Refactors config reconciliation to the workload cluster and tests it
c340b226b59591b41e731321206c3b28bcfd2884 Merge pull request #2250 from JoelSpeed/mhc-targets
90bf080764e3f525c6759f1eb76067cca6942ac3 :running: fetch_ext_bins now checks existing version before downloading
349f46008797b67030f1eea30c832f44bf015f76 Merge pull request #2314 from fabriziopandini/clusterctl-drop-incomplete-plans
3d6efa3490cd2c4d8c5705b3052a0b56c8effb0a Merge pull request #2477 from chuckha/refactor-workload-cluster
b8e881eb76b8d30184e1688a5b290f651a037bc8 Define type for secret created by kubeadm bootstrap controller
4c4f45ca9409794f563e2f3a763645c8bc6f78a6 Refactor workload cluster out of cluster
56a063b01ce99aeb28b9971739e14af5ad7ee526 clusterctl-drop-incomplete-plans
d2953f9b445ceaa5409fb3456d8cd06dd02621c1 Merge pull request #2472 from chuckha/health-check-unit-tests
39fced8f2f455d0414a33e714a4988c2e266697c Merge pull request #2473 from vincepri/fix-kubeadmconfig-log
23ef7d7fe65359330d7f7b0085deeab45ae8de4f Merge pull request #2471 from vincepri/gobindata-update
502824eea85e3586eaa02d6cceea2994bd9be805 Add unit tests for health check function
1a81e8c46a63d4102a74f42d8144577afac1487a Merge pull request #2435 from prksu/remove-etcd-member
cb0376ef73f0ce306f3245a6fcb16fd619dfa5ea Try all nodes except one being removed when removing etcd member
9d80f0c8391fb0234fd2aec18bf913273961ed12 :bug: Fix misleading log when creating bootstrap data secret
b160b9a0b2d7822da540de04be8fa306eab5b693 Merge pull request #2470 from chuckha/cluster-etcd-client
b7752c931786243c6cfc5e0b8f369647af1f5863 refactor the etcd client in the cluster object
aad739589cdadddae9b393a57c690d13779e54f7 :running: Use go-bindata/go-bindata like in k/k
d8d126b6b0f7a8e829890161873cd64298f7060e Merge pull request #2465 from JoelSpeed/last-updated
d5a066b70e446374411e9732104b45eac8e697b6 Merge pull request #2468 from chuckha/fix-etcd-healthcheck
4785a84465348cecb5e84d396893a79d0af34162 Set LastUpdated on Machine status when Phase changes
5e92711df62cb07d9380a77e2a77802c0211ca55 Allow kcp etcd health check to pass
b1886d352b2ec4f82d86039876417fdbbd46ba78 Merge pull request #2463 from sedefsavas/2439
067f1e0f4e6a1ac0d108f150665ddff4a33bfc08 Add nodeMissing field to HealthCheckTarget
973f20563773ba32507b540cb460590ef96d50de Don't use pointer for mutex
81f6c32ac93105bd242b1136cec5cdbbfa761820 Go back to map for informers
451c720f40a744fb638d1110b2000853f9422804 Feedback #3
3b7e8f08dc8d4ba335f017c9b91f165592036bcb Add validation webhook check to make Spec.ClusterName immutable
f0bc1035b469ae8e74d7154b05e6e59bbc0462d5 Merge pull request #2451 from sethp-nr/patch-2
ce51864a472159270fc4d430c9e259f905df6802 Merge pull request #2456 from chuckha/upgrade-1.17
a72f0e08bad8cba009bc061662a8c9606667f278 Merge pull request #2458 from nader-ziada/move2
4cfa74a33caefaa5510f51ed64b6306e61f1b8f7 Report all healthcheck errors
a39618d45eda45400759223a8a73c99e591e2101 Merge pull request #2376 from vincepri/add-reviewer-cecile
0a0c8129dab73996c5cd4b8347ddad33e0146654 cleanup for machine_controller watcher of a cluster
85f5ea3883c977debc5c3875524629fe88cad7a9 Update kubelet and kubeadm config on upgrade
cfd09ef1231b6deb7b8a5347b908b8c3f7516af8 Merge pull request #2432 from nader-ziada/move
d92eee7e668c5f9868f70a6657f8a8be923c1a46 add a cluster watcher in the machine controller to reconcile
25b281e30f4304353c42ac7ebcddf37648847866 Merge pull request #2422 from vincepri/add-tests-configowner
7d2646b83ad3db428a586184b977bf8349b7ab8e 🏃Cleanup and add tests for bootstrap util.GetConfigOwner
f4409bf5a18ba849742f2289e1a647c972ed8670 Make hasMatchingLabels generic
6e569b23dd21397f692c78f88ff8254c78c715c8 Merge pull request #2421 from vincepri/clusterctl-config-twekas
2ccd5c27eaeecfedf8eec5cb72e6efdf0bbbc80b Allow empty status fields
fbab1a2ea90088aca40509bd272241c4656f45cf Use sync.Map for clusterNodeInformers
ea2cd28434b430af4b3d2981f5909a8a9f9bb28c More feedback
5ac9cc8c2c63595b2a6f39a535f16ed1e2252ccb Address feedback
843e020e178c9c1ee0f9507ae5baae86e2093f62 Use runtime objects for tests
e8a4b0f0a24447e5f56594b5de5dd502088cdcb4 Add context to remote clients
bcc257005bfd20c99144b475cc328ad62bd648b3 Drop namespacedName
cfd167c3358a8eb42bc14833073b2d872bfb9157 Use IsZero for Machine deletion timestamp
7a3919c6af6d3bfd2fb863d60050f8e15172ac79 Use FailureReason to determine whether a Machine has failed
0cafd055c59fb288471679aaee3358e0f31dd0c2 Use NodeStartupTimeout instead of constant
bf817c7ac0f445f4c65746a58e8776640e179099 Add NodeStartupTimeout to MachineHealthCheck
0b588951998b76f6f0cf484d72d9088f708fea00 Remove redundant namespaced name logging
5f22b428d01158e1a3827ae4cdb5e644ba69a3aa Return errors for requeueing
5f1300d06063da572304bef2a947fac8ac7182ba Add tests for watching of Machines and Nodes
5960a82cf19acc9eb051b93b136a936b8ca693d1 Add watch for nodes in remote clusters
2f8fba0e75b5a013aca261d1ea4efaea217033c3 Add test for MHC hasMatchingLabels
618eea12a4abce94e99eb149908c08307dd84e44 Watch Machine objects in the MHC controller
2d276e1e7c53eea4850c56cce6386e1f4dc58f49 Add tests for health checking of nodes
352001b0b759cf0369635979199405daca062f0c Check targets and determine which need remediation
eb80ce13ff5ea359e82c3919461cb9d264e8c9a1 Add test for health checking targets from cluster
3f130f0382d8f019776b605f8ad7176542a3aa20 Fetch health checking targets from cluster
2384b53345d96b222746463f417d56c1d436cfd7 Merge pull request #2436 from chuckha/ha-proxy-lb
746841eeabb63379b505c53e01684ed8c8b5a491 Use a better loadbalancer for capd
eea0aa1c4197d92ab4de3c4c631229ae6877b3bd Merge pull request #2334 from detiber/kcpUpgrade
97e8ebd665f5f44e9c60b6647517d8bbcbfec762 Merge pull request #2371 from alexander-demichev/dumpresources
1d8066c914165c6b0c5da09690bc3842030ce908 :running: Minor cleanups to clusterctl config cluster
c5161f51b9a2ed0c637126577d7d224ba9a7ec15 Merge pull request #2431 from chuckha/makefix
de27f2fe75f477cef227d90e08760a0a42b620fa Fix makefile escaping for capd-e2e focus
6db00d420938518b92273d20705de45ab36fae15 Merge pull request #2428 from vincepri/remove-bazel-2
cdec3cadfbabc0e3c9406fa12171be8bb37c12ae :running: Remove hack/update-bazel.sh
b814473efb54448a9eff22051f3b4e3416c83834 Merge pull request #2426 from alexander-demichev/fields
0faf084be64e6e365b1e4f6e81e607aa61f9b97e Add printer colums to machinesets
215b16b002fd843397f89200cd79d44891b20252 Merge pull request #2419 from CecileRobertMichon/clusterctl-azure
cab06ca684a08430219d71b954d78c4364d66489 Merge pull request #2406 from juan-lee/machinepool-configowner
c447c53c0f88398652195e1c9cf440ec99e74df8 fix: allow non-cascading KCP deletes
dc22488bd47f3112524af15672aec66ca49bf174 fix: Import sig.k8s.io/yaml instead of go-yaml
699484405e27a8b3bc75688158084fae00c5f550 KubeadmControlPlane implementation
3a3d888c774ef4af9ed4742c72ee3095b7fe6cd5 Merge pull request #2418 from chuckha/upgrade-test
9acc7a0a0bab3ed0f45bf6c06014310734f06360 🏃Add azure provider in clusterctl pre-defined providers list
83c5dc586610c2f630b335ea07d13bd057c8b311 Merge pull request #2417 from vincepri/cleanup-utils
e608999344c4f6e83ce368c9899f54071f6c1a21 Adds an upgrade test
d881dc607e05cd32084ccd468ac5b97e1b5f347f :warning: Remove unused util functions
f14c261bc1be4dd46bf7b701149ec5f2abd9849e Merge pull request #2409 from Nordix/capbm-mael
c6f673d18f8d58a37b1c358a9185eb4a71716d09 KCP: expect timeout from target cluster load-balancer
64940c05bdf57d5339abc99d44b3873b7a05af99 Merge pull request #2411 from vincepri/fix-util-ownerref
86ccb668de1a5cbc2a13df3cea00d75edbc3eb45 :bug: util.EnsureOwnerRef should ignore version when comparing objects
1b6acaf0da74c5dfd0cb085160fccac2a101a6a6 Merge pull request #2413 from sethp-nr/patch-2
b5495561f0bb2bdc515ab18afa8d048eb705f84a 🏃tilt: watch internal KCP package
d1d95d20e215b435fa01d8950e5ba5e97e80b0f1 Recongnize MachinePool as a bootstrap config owner
f4abc033a7c3036921f2108ea2b638448b454e17 Merge pull request #2399 from detiber/UpdateCommunity
103cd5b52afd811201462d77fa8afeb4389cf031 Dump resources YAML to artifact output
f3547962cdb48cb1330b97f16d9f5543c291d1e3 Update our community blurb
1435eed4f1f4f68458be3bb22e03345c19e6fa01 Merge pull request #2308 from hpandeycodeit/md_label
dab38c8abebda5e6041115bee13a607e6e6fe916 Moved MachineDeployment Cluster Label Name to webhook
19bb15479ef3fc8ef4db69aa71c775e93fa4c751 Merge pull request #2397 from randomvariable/set-kindest-image
78baff28a42a7fa7e94c66ccfacbb0a55fa008f6 test: Set kindest image to 1.16 for CRDv1 compat
098a91174c025560ed01c68f3579ecb8be750255 Merge pull request #2383 from detiber/kcpRemoveConfigMapEntry
3418ba72b15092faf6a1638a592409ac99d059ec Remove configmap entry when doing a KubeadmControlPlane scale down
47420b56da2d84da9c90e8ab3baa1ddc10128b5a Merge pull request #2394 from chuckha/kcp-immutable
3d0cebaa2c06559e46bec6601e6b97a02e9cd39d Disallow modification of KCP kubeadm config spec
075c43954bb2fc36cb83be6f1c8fc978f0e537fd Merge pull request #2382 from detiber/kcpRemoveEtcdScaleDown
8c455bc353946ea29792645717238c28824f1edf Remove etcd membership when doing a KubeadmControlPlane scale down
4d247d5ebca86081e2cd518938e8c61bcfe56c52 Merge pull request #2381 from detiber/kcpScaleDownImprovements
678e2ccc05413942f89f7d7b7163d2c61dd05101 Improve re-entrancy of KubeadmControlPlane scale down
9547a1c4bd6bbe02f019d772ecbe18fa4f0d4c8e Merge pull request #2380 from detiber/kcpPushLoggerDown
4852f4d30c8c1c7ab371968f113e862d77f84e99 Leverage reconciler's logger to improve log handling
6fcfc257d3604c23282c572468cbc3773a236c1f Merge pull request #2368 from SataQiu/fix-pre-releases
952da0f0d49be0ed18b124a756acd44ed9c56840 Merge pull request #2388 from detiber/webhookTweaks
3f4b4ca52a2aa971af788a8689b8a6c2d4067ec1 Centralize common validations for kubeadmcontrolplane webhooks, also add support for mutating the KubeadmConfigSpec minus InitConfiguration/JoinConfiguration
94aa714e9c9c35ece5569a90d1bac4b257393007 Merge pull request #2384 from dlipovetsky/forbid-scale-zero-replicas
5e23a40627b8601f7b9c68d30da403b107795ac6 Merge pull request #2386 from fabriziopandini/fix-provider-field
87dee8ebf8652232d4143c0abebb03e7643b7692 Merge pull request #2379 from detiber/kcpFailureDomainImprovements
c8594c425cc0f0b3d6fdc67c063157a092510360 fix provider-field
c6949a0aa795e8cd023d501b8ab6f9105fb18022 :running: kubeadm control plane validating webhook: forbid scaling to zero
76fd607773696b648676a42e5531c15b90948cbe Cleanup FailureDomain support for KubeadmControlPlane
13d26a587559a6743cc44afdb49c1d6e2160009f Merge pull request #2378 from detiber/kcpFilterCleanup
ac8b360b73d00281c4d2ca48da5304daa9824ab1 Cleanup KubeadmControlPlane machine filters
873422dfc23308d6c29534e4836ff8c83bb1950d Merge pull request #2359 from sedefsavas/featuregate
ddb58eb947c1d3ed9c31df9f25299c6069969175 Merge pull request #2355 from fabriziopandini/clusterctl-map-uxname-to-manifestlabels
a81c0402bb464495154426eb732263eb68ee6f88 Merge pull request #2329 from detiber/RemoveCruft
c8bb7505ae918557fb7357441b70a9a3f4c6799a Migrate clusterapi flags from go flags to pflags
0b40cc149204c8dfebcb5f764e76d706af673ab5 Merge pull request #2377 from vincepri/cleanup-ifs
894a05478c8049e40b7dc197a864c65f891a32b0 Remove use of apiutil.NewDynamicRESTMapper
201c5b8ec3ab6948cc6dcc6276102c04d04eef87 allows usage providers with the same name but different type
cb6b9f68dbc04eae6e99b8787aa6361565f4ceaa :running: cleanup deletion timestamp handling on external objects
5b0cbbd1250fd4ac06523e3634692d58301c2721 Merge pull request #2373 from vincepri/fix-data-secret
a5f502ab4703ad3b6ae3825adbe5b53406087686 :running: Add Cecile to reviewer list
4d26184b1c64fec047541ee04cea36c9eab8b698 Merge pull request #2374 from chuckha/filters
4360d372e3cbed6d7f8dbbe8543f578917af61ab Make sure to check deletion timestamp, fix nil issue with bootstrap config
47dfc1e048e689491ba20aba5e5db00461a82431 Merge pull request #2375 from Nordix/capbm-mael
c2bb7c77e373d9c17b07b5ba13fa68c6c8a77c90 Update clusterctl test/e2e modules
420a9ad4b07303136736d7a7810df00ccf8e4a3d Adds machine filters and machine set-collection
bc65e0d16df69b9e5717ca17b32f4b008b9782c8 Merge pull request #2285 from chuckha/failure-domain-expectations
3ba50aa912f287a20c476754a15ee0ce41fd548e Fix book CSS for 7th column on provider tab
838e617d32f606e8434c08e91f0f5898475ac4ac Machine controller should expect bootstrap data only in secret
49b14bbada1e72b7bea16786049d461b428700aa Merge pull request #2333 from endurancetest20380119/master
cfca2566cd88c575893615f99923730c2ca1c277 Merge pull request #2357 from Nordix/capbm-mael
1e3cde849ee2f9dd09761ccc05d678f2e48e5386 Merge pull request #2358 from Danil-Grigorev/new-cluster-client-refactor
1384c0f457c51973f91963d786401e37a9f98ec1 Refactor remote.NewClusterClient and remote.RESTConfig
ffcb1f6b99650725d47c57950d08c81429f28b56 Add baremetal provider in clusterctl pre-defined providers list
b2f7cde4fb52370588b17c00678e9fa039c6012c :bug: Fix handling pre-releases in mdbook
a781517f0d4b49be06bcd6d944f078bb07d8afc3 Make  instructions consistent with other contents.
8e2625815a2cdb1895821dd289fc63bbfb29d0be Fix the typo of tenant
c3a40b9bcbda64cd1951772e399bcae95e75d012 Merge pull request #2367 from spectrocloud/fix-failure-domain-doc
8e638c46fbd7448a6bc1f692d0cd094621e1ab59 fix FailureDomains doc
4ff9ae5b552195a6ec469dd11f6640c62b678f08 Merge pull request #1952 from juan-lee/machinepool-controller
27a6031a1d6aa1a310c905b7d1afa331ab1cfd2d Merge pull request #2361 from nader-ziada/omitempty
939231b9c4a66fb49d1f1ee93feafdc0c5f1695b Merge pull request #2360 from newrelic-forks/rudoi/kct-ca-inject
0830159343c5f50e30dd85115cd2f1f9113c0887 fix: add ca injection for kubeadmconfigtemplate
cadf7200abcc8231142275fa2aae29f22cdc2391 kubeadmbootstrapconfig passwd field is omitempty since its optional
5a4c0b8f0894482e0c23bbbc5734c186e21ed972 Merge pull request #2354 from fabriziopandini/clusterctl-reset-commandline-flags
16590d2c6ff825930ea6788e35e9f630895b9d25 Merge pull request #2351 from elmiko/issues/1774
bf7f303cdefde4732d968170bcb65aee250bf5ee Merge pull request #2353 from fabriziopandini/clusterctl-get-template-without-cluster
e486c08539109255f88703b4b5595ee3556fd7fc Merge pull request #2344 from jichenjc/add_ns
18da4ef61f027325fba7119b0b82b32f4586cc24 Merge pull request #2352 from SataQiu/fix-AssertAllClusterAPIResourcesAreGone
722be19117c0fc386a24aa41333e887ee91ddc94 Merge pull request #2296 from SataQiu/test-skip-20200209
7baeed7cfbcddaed5b0898580ec6b4c0ff827080 Extract failure domain expectataions into framework
4dd92312ae181ce0ee22c08aaa5d4d589464a976 clusterctl reset commandline flags
0d48bb12a23c1f2c7b796fd28be4b24c32e47c19 clusterctl allows to get templates from repository without cluster
0597f9b5af30d250d4a50cf57e01b8e7b1cb6d69 [e2e framework] ensure MachinePools are deleted
ebced8033bf2972c3e7528b26e4c3171fd11549f Merge pull request #2236 from Nordix/clusterctl-e2e
8c6fa72fb8b2a79de25c9816df298184aa9d21aa change some tab displays in the cluster-api book
0d7f739d3bec4b4ca95da10a27d8f189ada2d860 Merge pull request #2348 from newrelic-forks/make-all
7ee77ca3e5cbc411a100755bc4ede7e396f187c4 e2e: add skip-resource-cleanup flag to allow skipping any clean up
3904640ce1dedcf4cddf2377dc78a1e10ab26083 Fixes the 'make all' target
1bb7162c09279c5527e86d78467a5c8df4f02138 [Doc] Fix machine not found
7eead355bcbc36aa1625ecfde617dfc1f8133c31 Merge pull request #2342 from dpandhi-git/broken_link_clusterctl_cmd
1108cdd6a5be6ddce53591bf0c3a9d4cd0626e10 Merge pull request #2347 from Nordix/fix-register-mael
d3dcb27b8a552b512c4f5be9bf31618e20a0ed37 MachinePool API Controller Implementation
1f2fb6e196cce92cfd8bf8ef27f337e064f9bce6 Add scheme registration for CustomResourceDefinition and List
4fd4c7f2c7cd67c9cbd1609e2fa52b2a0cc98dcc Merge pull request #2267 from vincepri/update-refs-nicely
12b2539736a18fd3d07edb89a42a64288f433123 Merge pull request #2313 from fabriziopandini/clusterctl-move-preflight-providers
9ad583ba61e042c3d481ba7bde612b4fd5f83e96 :warning: Add support to auto-update external references
d09f59ec5460680d48d5979be341ef1dc4d9b564 Merge pull request #2335 from dlipovetsky/controlplane-scale
386d3bfae83bc10144fbcc8687e7ea0c891c7a9e :sparkles: Adds kubeadm control plane scale up/down
497be3756e48c18cf4f411ad209fed172ea707ac Merge pull request #2337 from vincepri/add-docs-tenancy
31a8b8732551d70283f7dfe01660f95f1fb2cd39 Merge pull request #2343 from newrelic-forks/ms-default-labels-followup
bfd4873159ae77fe84a2baca7fca06ea13053ef9 :book: Add documentation on how to support multi-tenancy with webhooks
26c05f1208213fde080c40fc971810af3c214549 chore: use defaults in machineset webhook
03c2bb6f4f7518f020cecf9506f4ae6f30620d46 Merge pull request #2324 from alexander-demichev/annotations
996227208edcebc6765cc7a28847001d3fcd487d Merge pull request #2330 from newrelic-forks/ms-default-labels
3fbeb1d9710f02e169df280a2318263c16dff46f chore: set default for machineset labels
ccd6f55933f9097ece9ba8df9c2903675f1481c3 Merge pull request #2338 from fabriziopandini/clusterctl-fix-webhooks-docs
f08f19723cd6a8af01c2b17c3893a33c2f16a66f Updated clusterctl configuration link at the bottom of https://master.cluster-api.sigs.k8s.io/clusterctl/commands/config-cluster.html#variables to use clusterctl/configuration.html instead of clusterctl/commands/configuration.html(broken link) #2340
4088c24b3649006d01eacb0aea11854ca7dfc4d8 Updated clusterctl configuration link at the bottom of https://master.cluster-api.sigs.k8s.io/clusterctl/commands/config-cluster.html#variables to use clusterctl/configuration.html instead of clusterctl/commands/configuration.html(broken link) #2340
5aea6d2b61ed0384d2289e248af08293f74e079e Merge pull request #2298 from fabriziopandini/clusterctl-fix-webhooks
ad249bc4a9951c9ea7c4a4c3660df4812d3a107d more comments
010e7227b8bd33ac3451680200d04d1f26e8c900 clusterctl-fix-webhooks-docs
98c34989547339cdb3c28dd31d8ebb8a600c1e20 address comments
7633c9d416af6d9ff377c20eaed20f66bac724d2 Merge pull request #2336 from detiber/pointers
13f9cbb857ee49ccac3358977845ace43977d7f2 Use pointers for Machine manipulation in KubeadmControlPlane
40e80c67aef65f587e6b1b1d19b022bce0ae6942 clusterctl-fix-webhooks
6cef3d1843e35b3e98e177accb789e78e9f6030c Merge pull request #2279 from vincepri/webhook-refactor
4ae3db42ad275aa176b50a3f79b52e77407bc73e Move MachineDeployment annotations under x-k8s.io
3b89a3d1e588f3c4ab9f7e40dcff766103169c74 Merge pull request #2326 from newrelic-forks/ignore-empty-objects
415eee7b9afb77e5282ad08a65e95f51fc1995b5 Test for multiple empty objects in a row
597b21f9f746f1653b81ae87de328b1b6c2fcb3c Test two --- in a row (before and after)
103de1ab4fd06a5d80cd4d24e7c74115501c2b41 Merge pull request #2319 from chuckha/cp-hcs
ad28a70ab0c3ee804cebc8084fdbb92e10cc24b6 CAPI webhooks in a separate namespace / deployment
0b5c77c7c4aab909dcd4f3f6f41eaf30c5772ee4 Add Azure kustomize_substitutions Tab
75560afe03eb6df7e4cfea9b9448e756f9ff665f Adds control plane healthcheck for workload clusters
af0542477f2bc874a091f70cf542258d399d15fc Merge pull request #2238 from detiber/kcpUpgrade
d6202478f1766ebba9e501818174a14d8559034c Initial skeleton for KubeadmControlPlane upgrades
02f3c38cfcb91d213ad6f8b4028a6527e8bfaa5a Merge pull request #2132 from vincepri/crd-v1
c3925143757aef02eb3ef6d9afc5b5a5de843fcb ✨ Update and require CRDv1
e0d1223d6630a76ee93b04805ee1372d4e6672a0 Merge pull request #2327 from nader-ziada/kubebuilderdoc
a14158b03ecdf203f61ba33987e12df42a91a7fc Add kubebuilder install link to developer's prerequisites
a0cdb3b05cda25ffad818f8d6453859dce9e0f92 Merge pull request #2322 from Nordix/fuzzing-mael
f946b6579ee4880fbba90c13b667e73cd402160b Merge pull request #2325 from fabriziopandini/clusterctl-code-cleanup
516e294551efe413bc47f0f1a6f1414e2e23b90f Ignore empty objects again (revert)
57ae35dcefec2e417c2dd546610204844cef2fd5 clusterctl e2e test suite:  * Makes use of the capi e2e framework  * Added a script to run clusterctl e2e tests. The script will issue a `make docker-build` and setup env var to load image into kind. Setup various cluserctl files and env vars.  * Added a test that creates a workload cluster.  * Added a clusterctl move test -- it moves a Cluster API objects associated with a single node capd cluster from one mgmt cluster to another mgmt cluster.  * Added a delete test.  * Use a local respository instead of local overrides for docker  * run-e2e.sh script updated to setup local repo in _artifacts dir and also create a custom clusterctl.yaml.  * Created util funcs to init a mgmt cluster and create a workload cluster.  * Added clusterctl delete tests.  * Added a README.md with instructions to run tests.
8bfa4578823656d363f8ba9d6cb802a4a7b73647 clusterctl code cleanup
771aa435f9484d819e7229ca46108aa23f3c123b Expand fuzzing framework to allow custom functions
78c565b11999368bce33efef38bd71d33cb2a7d0 Merge pull request #2284 from fabriziopandini/clusterctl-list-images
70565f5e0a610f04898dfa3d7feba516bdfa9b36 Rename comment form Init to InitImages
13d44c484542ee67e89a93c3fda84fdfaa8e9e3a Merge pull request #2315 from fabriziopandini/clusterctl-fix-to-unstructured
2305724b573572e9f75e1d668772feae04f9c863 clusterctl list images
4899fd33d696bfaf40e22293af4fdc85f83c7f8e Merge pull request #2293 from fabriziopandini/clusterctl-validate-install
187c48ea421d0939a4bc507f17187b2b442b6dda clusterctl validate install
73d7dfd096c3aea83e8d172aa700f47874edc7ff clusterctl-fix-to-unstructured
1f1db9c77e74534a6857f648b83dbc5ec7fcc3d9 Merge pull request #2266 from fabriziopandini/clusterctl-more-docs
31b18578049722a85a28a2034226d76e24c32b6a Merge pull request #2294 from chuckha/e2e-refactor
515541f3b5d140d0a993d058fc330dc2bffd2d11 Refactor the e2e framework
4a10541b9d8c39e7995944c7d8f78bc5f122a14f clusterctl-move-preflight-providers
f043204fae642f0133e0be3761233a7245c9e487 Merge pull request #2303 from chuckha/kcp-cleanup
f0e200e6acbd0cba3d12a090b487dc0555f7c414 Clean up the control plane controller
e939e07cb82f066eb0b85d58a0f75588378af5a4 Merge pull request #2265 from fabriziopandini/clusterctl-config-from
2d60f27e9670d5096b7d81d46bfeb4a6621c79ae clusterctl read templates from different sources
8b7ffa5dee4aa48f9e746c89a80a04b0871fb731 Merge pull request #2281 from fabriziopandini/clusterctl-upgrade-plan-apply
884c809b7644266a3ad24ae8ddf7f644b6bb1875 Merge pull request #2307 from prankul88/remove-duplicate-code
4d89d565e5bc410a81e2712425950e400c0a89ce Merge pull request #2295 from chuckha/hcs
b7dbe52af4abda58e1bd34d60667426aefbc695a Remove variables from ci that are already declared in Makefile
8acdffa8f194b430b2274556d5e6bb339a07da8b Merge pull request #2297 from prankul88/remove_lint-full
ff6e609f4efb8eed230cf958f7ce0e16260b923d Remove lint-full dependency
c6d3f310388c8b897972ae974ac0f95a36a87764 Adds healthcheck for workload clusters
81695dc55c44771fb3db91ebde8ec4d086041036 clusterctl upgrade plan apply
e3641e3b49384939cceeea1e9077ce833ccd74d5 Merge pull request #2299 from fabriziopandini/clusterctl-add-control-plane-metadata
a99918807965b2b168a8f15b9e890589094b5b70 Merge pull request #2289 from newrelic-forks/rudoi/md-default-labels
ad8a8a8f5c10a39f84e26b8b37658933aa7ddf0e chore: only add machinedeployment name selector when selector is empty
ad659a92645b4fa39fbb758aa1d523e223df6c1f Merge pull request #2301 from SataQiu/fix-book-20200210
f63843e9407243cf5edac0c90320075636b8e0f4 more comments
dd743b7f439fe1f5a7cedbf83e3428f66331c498 add developer/providers/v1alpha2-to-v1alpha3.md to SUMMARY.md
301f3f4957c2d29ac923f140f5e47ce2ac04c92f clusterctl add control-plane metadata
ea119714b764ea1713cf66b7bf45081aab8428dd Merge pull request #2290 from colinlodter/cluster-api_2181
2155f8eb411895d22b95c8c3dbdc2bd91da78f73 Remove protobuf tags
67c5b255cfa4c8a3099a67be0a4b98c814fa1641 Merge pull request #2042 from outofmem0ry/docs/quickstart-fix
d604c007e548e91d59891be833c5ca7a187a9204 Merge pull request #2282 from SataQiu/fix-Makefile
0f2bb3163e0c0eb379af33c52893d91a7bc71eab Fix broken target cluster link under quick start
52b208c8d63077454df33a884171ac3c68484ad4 address comments
0394f95f49578dc729bcf8095eb8769b7f087a97 fix regular expression in Makefile
5d3d0d1cbfda7a6aa101834509e1ac402ecd0ce1 Merge pull request #2280 from chuckha/context-whoa
0922624febec1a90003e1927072e8f5a1286b5e1 Pass context through remote get client
c976d8e0c99877c21495b451cb6e8e29ba735642 Merge pull request #2277 from fabriziopandini/clusterctl-cleanup-inventory
dcb625e592e814a3afb829c9ff1ddfd6b7609d23 clusterctl more docs
8aa5b6a29f1b4cf4b0a060d68d708ead6e4d821a clusterctl cleanup inventory
a552b9dedaf7b0966cd31f42576722609842e917 Merge pull request #2278 from aaroniscode/clusterctl_doc
6cee4a0b5df4383e5dc46fe4ecce0eb05b034bb1 Merge pull request #2270 from alexbrand/improve-tilt
d8639bf97e980c32be8e1461cec25f6025c9b534 add kubeadm-control-plane to the example providers in clusterctl dev docs
c9c7dd96ce125bf6aad92859ac420daf71666f2f Remove kind_cluster_name from the example
c7c590f67403fdb839cfc06e831a66946e18ff63 Add tilt version requirement
1345fe7043923390a0db14d826f487d42cb01637 Merge pull request #2271 from elmiko/issue/1951
4b7ca5aa580cabf3173ead93e6aeafbd34413901 Merge pull request #2274 from fabriziopandini/capd-reconcile-status-ready-after-move
5237d1cf1af0668598bf49106c792392192d26a2 capd reconcile status ready after move
5ac3f42002eb292972fa173042e9bacb8fb2ca88 Merge pull request #2273 from alexbrand/fix-quickstart
1ee2706b4be0f7228b6f92c5c9654330bc168813 Fix sample Machine and MachineDeployment objects in Quick Start doc
08bef7120b7d61ce2fe820ff2b964182c585f3d4 Merge pull request #2191 from fabriziopandini/clusterctl-use-global-logger
13e26902da99f7cee71b5805fea333150451854b add a Personas section to the cluster api book
f787617176c9ea7c8a60076326b420186decfba5 Add an option to specify the kind cluster name when using Tilt
55a9fe3cd2216c50ff2ecd90dab4816728323416 add global logger and make clusterctl use it
8e041b8ba4de420c09d132422e4fa673c9d9aa3f Merge pull request #2178 from fabriziopandini/clusterctl-upgrade-plan-cmd
12ddd37159bb556b97c1b92519ba18a0182502ff Merge pull request #2254 from fabriziopandini/clusterctl-make-template-generic
5ce39e9b643eb41118c18dc433784eb32b9d8bd8 Merge pull request #2246 from fabriziopandini/clusterctl-move-check-provisioning-complete
caf057646efde0660157437279bc43de01dc6336 Merge pull request #2235 from chuckha/failure-domain-doc
7ebcaa17574513c80df05579d7b9ffef22372ae9 Merge pull request #2239 from prankul88/update_constant_machinetypes
82a7ac0a01e36df514d855f3b348f375c0533970 Merge pull request #2165 from hypnoglow/drain-unready-nodes
a161c6517a88f2abb63a7dea0356b20669337dbc Add provider implementation docs around failure domain
e32306511e3b95a09041744d38d9642578735080 Merge pull request #2263 from vincepri/add-other-types
43e6ca6ab28163cd8b1e9f83bcbe6a2f76aacc01 clusterctl add the upgrade plan cmd
3fac37f7bf83daad26bf61b421c23242374c8358 move preflight check provisioning complete
7eac8e6a439bc68d8c22cd488224fd116b06d812 Update ExcludeNodeDrainingAnnotation
3468d816f1279b7ac69b88554d8b980d29469734 Merge pull request #2253 from jichenjc/add_openstack
d8093543e36735488b4e840365068362f76fcceb :running: Add other types to FuzzyConversion
e93944da08f68399b0869cde697774ca6e98319d Add openstack as infrastructure provider
b2ab4c203c74b078cf551044cc42ee881412baf2 Merge pull request #2259 from vincepri/add-fuzzer-conversion
836677b7d3ec59a77726919e26b00f3b00b29155 :running: Update linter version to 1.23.3, timeout to 6m
47788eacfe2ba68489ed18fcff55e0703506e517 :running: Test Cluster conversions with object fuzzer
ec648ecafb767ce75636463e57ef5b01a45c0de3 Support draining unreachable nodes
1ac59f3a9cf967bc744ea04741e4fb5745ab411c Merge pull request #2262 from detiber/shortcutReconcileControlPlaneInitialized
c37399c109dcac60cd81548f848f4162a589da46 Clean up ControlPlaneInitialized handling
2dab84b99f3ba13113fb7fd91ea79b607ece519d clusterctl-make-template-generic
f52ec705fec0d2c03678ba3c24247dad889e859e Merge pull request #2261 from dlipovetsky/etcd-clusterid
583f77931619d4273a984a09675877a46ff51e2e etcd client: Add 'ClusterID' field to etcd Member struct
f8572f882bd7f1518730073d2a59a6b3cfbf7095 etcd client: Remove the 'Member' receiver
987ef40a18357a70dfef1a66241fb31b9622f2a8 Merge pull request #2255 from fabriziopandini/clusterctl-cleanups
307d1aeb44f8ec4720827c83238f22d649924200 Merge pull request #2258 from JoelSpeed/mhc-test-flakes
f46111abde20b1bea4d70136fe275e2f2d8ce90d more cleanups
1180470dcfb48c310673807e52be1596e5fc8bd3 Fix flaking tests in MachineHealthCheck suite
5a616e29e9597f6d5c7be398a2168c9b1855d654 Merge pull request #2237 from chuckha/etcd-client
bbe403d321a33e3b1c12cd1faa1499b033040960 Merge pull request #2192 from Nordix/clusterctlv2-select-repo-local
1b3ec463d28c6949836299ceb127b5d132303691 Refactor etcd client
98d51d3a496522e6a22fadaa5e0425eed41e13f7 In clusterctl, adds ability to automatically select local filesystem  backend when URL of the repo begins with "file://"
f208101f26f92e87a5a122231b1dbaf77871788a Merge pull request #2247 from detiber/FixConversionGen
e84d175fcdc35b9be52027272aaf6b1bbdc0d8d1 Update version of conversion-gen
f5b4666e56d9b98b43951a48b644e47ba31a3845 Merge pull request #2221 from fabriziopandini/clusterctl-simplify-template-naming
d6e8d57a26f3a4497cf26a890cec139578a73bcc clusterctl simplify template naming
5cfd0f18f5266b2612489a712a428a2d70f1ea57 Merge pull request #2245 from fabriziopandini/clusterctl-move-ensure-ns
45ca8b1f565f2014ae8c95c8671e357b541e7f61 Merge pull request #2150 from fabriziopandini/clusterctl-logger
14b0558e69a8a068f51d909e09f98c4e99cdf89b clusterctl add logger
8fb847f21f7923202a9d04556cf049e89675b6e8 Merge pull request #2101 from JoelSpeed/machinehealthcheck-reconcile
ae41c8fec9c7e0cba406ebfddf56f54151980a11 address comment
23d4c45666aaa1feb8dea9b476f260e8f9bf7ea0 etcd: Etcd client with dialer passthrough.
6ad9dfa4c90aeec275c6bb563f172a3a3a621d17 Add MachineHealthCheck Reconciler Skeleton
ecb51bc0f701cbfc5c0509fc7e292baf0a6eff4d move ensure all the namespaces exists
385973f235c5c5682ae20c8807727f568efb0cd1 Merge pull request #2248 from fabriziopandini/clusterctl-code-cleanups
108f3963d6a5d3f81b22b13218c595807c7e45dd code cleanups
4a68ed22a1ecac1c4ff6b5489a35bbecb673f21d Merge pull request #2206 from fabriziopandini/clustectl-wait-inventory-crd
455123033d428be5b9bb09b086a95da16a70a089 clusterctl wait inventory crd
0a9b0fdd9e3eb26403838ad8a2d6912aa0f0bf14 Merge pull request #2134 from fabriziopandini/clusterctl-upgrade-plan
da6a2ba9c185dfcf9be69da82ce1aa947c32f0d8 add upgrader with the upgrade plan logic
6f00305afb2c5db2a01e86505da578ff575ca244 Merge pull request #2220 from fabriziopandini/clusterctl-fix-public-library
57da6a8ff84e96d8b16a0822b08dd82ef81a660b clusterctl fix public library
f068437d603eedc3e097887c74536339e0d6bbf2 Merge pull request #2161 from fabriziopandini/clusterctl-move-shared-objects
ca66c55c5901f7b856b25a56dd872aa2b1479ea7 clusterctl move shared objects
1680c04e2b4cfee433aab19f3dd89bc4b1102f36 Merge pull request #2148 from ncdc/add-roadmap
3591c7a1326abc6df2cf9784f5c2c99c0783f272 Merge pull request #2147 from wfernandes/doc-control-plane-up
788fe7bd946f44b2ac9606bb8e0c675cbc0f83cd Merge pull request #2229 from chuckha/failure-domain
0cd6e6cae03170b950802cf648e2599f47182838 Implement failureDomain on machine objects
4ec4ec416a91317f4e43cb2d885f592b776072c0 Merge pull request #2213 from detiber/kcpFixes
ebb673b82df2f2025d66b24322b2e133beb3ac10 Fixup Machine/Cluster controller handling of ownerRefs
aefc90f6df73601f116d419587f6a573ee47dc21 Add support for pausing KubeadmControlPlane
0f7caab2a2990f3a6d6a69bfe6d6978f66e18c9a comments1
ea93471ad47a70020d662ad6816e902ca153f12f Merge pull request #2211 from fabriziopandini/clusterct-fix-config-provider
4394b0cf48fa29f866e4b591f5bbd125e9e5a03a Merge pull request #2228 from vincepri/fix-enqueue
0360af973fb8abcba1d675ffc4707020036dd3a6 :bug: Enqueue request for the right owner in machine controller
7cdea780c77075abec93deb26ab7d2e1f96961ea Merge pull request #2212 from vincepri/refactor-external-objects
a2753675bc07ce85dd25857e671d811a49696bde Merge pull request #2154 from johnharris85/conversion-fixes
72e293f86fb0ba61732ba1a28ddc0fe46d43853c Merge pull request #2216 from wfernandes/clusterctl-allow-buildrelease
8dc29da144954514d0527dc7577b2b7389487d3f Merge pull request #2224 from chuckha/capd-flake
be8cd791b32eceaa295b05701aae4e6548db2e79 Fix cluster name conversions a2 > a3
e4e361241aaccc408fb7eff4de7284f9673e32eb :sparkles: Refactor external objects & reduce code duplication
8ecdf022fb041aedc0da81c5b742d090d1e1ae8c Update module dependencies
065eb539766dede097e206a7b549b5902d15f14a Merge pull request #2222 from ncdc/docs/fix-provider-diagrams
a81032949b53f08a8447a471e7d718df647e220a Fix flake in capd
b21b5cb26e7bb60af94e60900f2b42f4b340bef7 Fix provider activity diagram URLs
51da1c888d96a7cbdec5d931c4a72d5d50ab9c9c clusterct fix config provider
d63f047ed084faa39117cb5da4c6698638a9f4bf Merge pull request #2215 from chuckha/kcp-cluster-infra-ready
3bf237c4f95f72ee8f924e096ed0d3b8a410ca2d Merge pull request #2210 from ncdc/lint-all
b5c6659beb6ad6c06ce21468729ce17a406fd313 Merge pull request #2173 from hpandeycodeit/printextracols
534945b2db00df77137433dc4d40a9a0f37aa0fd clusterctl: Allow pre-release and metadata versions for local repos
215b0bb2e1bc6d8e2537285875190cbaf2c62029 Wait for the cluster infra to be ready
8920aaaf6e6387cea191da8d407a28fde321fb26 Added extra columns to print in kubectl get with (-o wide)
2ee11a5d2f5f53aff79761f62246538364c14c1e Merge pull request #2207 from chuckha/makefile-fix
f11e0a730cbbb089dc853d507129810770382d32 Fix linting issues
21558eb7aa8d4f7ed49abe84905414e56759caa1 Enable linting of all our go modules
a90ae92a50030d97976454351d72a56dc94a94f5 Merge pull request #2205 from daxmc99/finalizer_cleanup
0cbceec8d6ce47710c27859cd243090ed04a3742 Document how to verify control-plane is running
5a0b52ed91788a32cba6386211a31d2d55246a46 Fix e2e Makefile targets
1ca177a06ae6a29eac2b9699b795362924847a6a cleanup: use controller-runtime utils for finalizers
9275fc4a987d2aaf3e724b37e84f99b79e24d110 Merge pull request #2197 from chuckha/remove-capi-e2es
335ec70352661c532c47f13bd90b35538d0773a1 Remove capi-e2e tests
eb78ae1b9dfca9092608ca4f3fcb28179a9416c0 Merge pull request #2204 from vincepri/add-ports-ref
e22d76568db413e3c87e774f3967fea9341a0ed6 :book: Add reference/ports link to the summary
99319fa3220a38ab8bbf3bd3a0d4d6145872da24 Merge pull request #2199 from chuckha/fd-test
e32ba028a925cd3a817dc818549c6524cb38e867 Make the failure domain test easier to debug
c7682877b67947749d469f96884da2112f65e9b6 Merge pull request #2175 from fabriziopandini/clusterctl-add-godoc
d87a9825442ff0340fa8161895475f6cc640d23a Merge pull request #2089 from tahsinrahman/use-kind-lib
3b15689a0e22337c5d3313e9771400ef5fbf45f8 clusterctl add godoc and doc
0e809b81135d658436283236129ca8358461b50f Merge pull request #2196 from JoelSpeed/metav1-rename
3c53acf9c982867d7c5ce8dfb8914b0534fc4798 Rename v1 to metav1 in imports
76ea21f93aaea325f5e44e815e364fc02b3008b0 Merge pull request #2194 from jichenjc/fix_comments
34388cfb0c9853874a785aac037775ea12c4a2e2 nit: fix an incorrect comments
56c43310041d498bc2af39372550352a260c57a5 Merge pull request #2190 from vincepri/ms-hash-fix
503a0e834debcf4f9e20a1513f128c9bd1334964 Merge pull request #2189 from chuckha/capi-e2e-deps
f6b61d6ef7c9d1dd4ea8e792f03879f03afd1c1e :bug: Remove Version from references when comparing MachineTemplateSpec
eaa816bacdbac73b4c5005fbc9bd76f0d37edc49 Add dependencies for capi-e2e tests
54420c41251541fdc14ed2ebd59891d540085afd Merge pull request #2156 from cpanato/GH-1855
52117a9badf6a9d27c8053f460bfddae02fb5100 Merge pull request #1963 from Nordix/clusterctlv2-repository-local
3fa97a13f304896a86ee2fe8fc58b26d133cc7a2 Merge pull request #2104 from fabriziopandini/clusterctl-inspect-images
1e4af0d188efeb5d99f975c824633aa48fa8fc02 Merge pull request #2169 from chuckha/failure-domain
403fbd8e8ff85e3c9001e59ccc79cc6b095e521c Merge pull request #2163 from CecileRobertMichon/kubeadm-verbose
8ad19cf15bd53e72489f3c5a3ce8aa37ac3d7e4a Merge pull request #2177 from fabriziopandini/clusterctl-allow-buildrelease
205dd64e886b71d49f0c140410610b6e956d4960 implement failure domain picking
6f1e36cc961430f23ef6a8c949907ed2f637cbec Merge pull request #2099 from fabriziopandini/clusterctl-controlplane-provider
3c4dff9e48320437fa7a205ee23c143f27cf52eb Merge pull request #2180 from wfernandes/fix-flag-help
d1f5d6925a710906e29e8a36e49b745897e5b5fe Fix clusterctl --config flag help
959c0486e3b0037f0168e7c48179ea0653dee341 clusterctl allow build releases
0b35eea112b57571545e46a4b78851f011ed0614 Merge pull request #2172 from wfernandes/clusterctl-docs
0beaef47f72e0135d9bd3ae013f4f0a22a238d68 Merge pull request #2159 from cpanato/add_port_book
3322580153d668816903bed89e1bf36ef7b7893b clusterctl add support for the controlplane provider
333c719d2dd0f98f4a97dbea424a7b5e9d03a033 add health endpoints
35a5b6b437bee94bb78ce4fd4582166e0443d6a6 add documentation regarding port allocation
1fec6b1927bf3652441ce46c05189881971d8fe9 remove blank spaces
7f1c28c93fcf370a6ceadef6e57e25b2f3ecca89 clusterctl inspect images
506cb9af40aaf829d8c6fd905f02d67ba1a01622 Merge pull request #2130 from fabriziopandini/clusterctl-move-cmd
6907d45d20e15cef166beb8be362f62376fdf838 ✨ Add verbosity to kubeadm config
ab3ce8e7210a68ca6ec41df155f57c7dde82bd5f Fix clusterctl developers doc
4f21ea6757e90994bbf3f1b84244e39a7fec2d90 Merge pull request #2167 from vincepri/noderef-list-fix
5a74a75da0925c882d2a2d22bdcfbfbf56ccf1ee :bug: MachineReconciler.getNodeReference use continue token
eafd8873a4d0089929ba7b545127fd462bd632b3 Merge pull request #2160 from wfernandes/clusterctl-labels
7816c0c01a97824103a2ee8fa8078625f0d56d36 Merge pull request #2158 from chuckha/capd-e2e-config
91b1d18a140137660804436c51cab1a34b4af4b7 Use e2e config for capd e2es
cf28eb7f9f34f25066db0f72de967bbbbfd67c54 address comments
b3a8674227db7c3be145cab331e766292c175431 Fix provider label for docker
bf51a2502f9007b531f6a9a2c1a4eae1586fb8ca Merge pull request #2152 from fabriziopandini/clusterctl-fix-labels
605888bf68ea7b652ee303581d07b61f5607426d Merge pull request #2146 from vincepri/book-reorg
79f87e538d0b49c1a646acbfa1175413efd1e891 Merge pull request #2070 from wfernandes/clusterctl-labels
dd6a6d581296f412d7cfd99bb834fd90e9d6ca74 Merge pull request #2135 from prankul88/add-printer-columns-to-machinedeployments
b5b9f79af96db9f186a2a0132044b91cd0f11473 File system backend implementation for provider's repository.
b3413408e7de5c5e38cc54ccc941b5a38b16c74c Add Ready Field
9407fb4ea82320201cc495167304363f16547b17 Use kind as library for create and delete
566a0a6c0c3946765300cb2a23f03662720ba997 clusterctl fix labels
bb8a58c9dfe49b2062b9e035168e2b247411bebb clusterctl add move cmd
54f26d7fd2b5d1c3a96e14bff717040d72fe8b9e Merge pull request #2149 from CecileRobertMichon/fix-azure-quickstart
1855849bff7c3eae53579480b60dc8e6d3d0250e Merge pull request #2102 from fabriziopandini/clusterctl-mover
b2523fb59d952117ea37fe7a148cddb82af8421b :runner: Update Azure quickstart docs for new k8s version
84f2ccfbab80b1f7be84b8ce9bb71009d0bf3626 clusterctl add the object mover
9f337b4a1d733b945e22c141701209d73395b3d4 Add cluster provider label to CAPI/CAPD components
b221bfc3a2279a33122fc2a0f90d68492ec5ce04 Merge pull request #2078 from fabriziopandini/clusterctl-delete
9866186caff0b13cc62bf5e3ac2a1337a500e7f1 Add initial roadmap draft
efd6fb57114c36db5f50bd7ab55163c18442e161 Merge pull request #2144 from akutz/feature/e2e-config
b01d7e3cc653f12887691ac5306d0ab4cb2398ef clusterctl add delete command
6d17a7f01f346820e5d8f5b9731f21a8de21d247 Merge pull request #2100 from johnharris85/tilt-manual-mode
ed05ff29a3aaa2fd0509c69449d6513784ad0155 e2e config, management cluster helper
87948d4e27199a3d8bff77d578fcdd80762a9f36 Fix two go-lint errors
e785d8760ee4d14f06e3d650353058857be873ad :book: Reorganize book folder structure
6c520d60915eb99a3abacb7b4de0e7c054a66b32 Merge pull request #2142 from chuckha/capi-e2e-fix
3117d1830b2a1e5f721fa784323ef36c352e360a Merge pull request #2145 from rmb938/patch-1
4ec62f4818f44c623884d1eea5b330485b005804 fix spelling mistake in readme
5087d29091bb2ca91c0338fab2de3e98e6b9888c fix the e2e tests
dc71f01d7feeff5036b9abaafc6db0ec31ba959a Merge pull request #2136 from chuckha/log-descendants
da24557bffd5705fb43d6011c578d462cbfbcbe6 Add ability to configure Tilt mode
177f8bfb47227bb6bbbdcf16c2df33b4c5a0a3e1 Merge pull request #2125 from nader-ziada/paused-external
e3b00f06f04db1e48a18283bdbb11d21b0b6acfc Improve delete logging
2633a37403e3b146981b66c677cf39efa7a23124 Stop the reconciliation when the external ref object is pause
ee0b0eb29a571aa72894abb79729dccc1f75caca Merge pull request #2127 from aaroniscode/duplicate_errors
a820834bf43ca2cfcbd69e617282c875b2f9c6ed remove duplicate errors, and silence usage on error
57ae572d41b0d23fae859b8d0538bcc8ecb8f6da Merge pull request #2124 from ncdc/docs/fix-bootstrap-diagram
2c9a217b5c7f7c7f55066c170b9dadaa595511f7 docs: fix bootstrap provider activity diagram url
a7b1a089bb39a06e42ed487b1f7d88431adffa18 Merge pull request #2123 from vincepri/link-image-builder
904e6e82a553866897f3ae7d92f4216bf2cb5ae5 :book: Add image builder section
6a7b65ae476c26361a9649d5db443f8fc8eeae0e Merge pull request #2122 from davidewatson/readme
7b9ba2cda965b2e2787990c0ca0caa710f931349 Update README to point to 2020 meeting notes.
100c2d816597f2815567324b336413b7f1b96afd Merge pull request #2119 from aaroniscode/clusterctl_useragent
648f6f4636b354c34d30522096cf5d36b4378f5e set clusterctl user-agent
92b45b19963c7b9c8dc60d33141eaee6b5b49eec Merge pull request #2106 from MarcelMue/remove-outdated-bootstrap
6462c8226b4284a16b32bb082abd9ca8b6a2f189 Merge pull request #2113 from aaroniscode/clusterctl_init_doc
30fbf6bbf8bb3279561e60bd5fb65cad36b12890 preserve old text and modify to be accurate
4806d8d53a88c1e768a4307d487431ff8e920fd7 Merge pull request #2114 from noamran/1561
6605e0ac72c349997f1fe1128b54e3f149541e9e Merge pull request #2116 from noamran/doc-kind-typo
2ef0cd01f92eaea1fe74eef9cce372e340c7aa7f remove $ in tilt doc
31b641c78ef2a33df9e55b1ac5cb959dc4ef64a1 adding cert-manager prerequisite
2a02734efc0b26f07144eeed8c8edd0388e7b650 fix doc typo in clusterctl init for --core flag
db823b790de0e73614205895dbfbf2b4402bb833 Merge pull request #2109 from vincepri/kubeadmconversiontest
43d0c03d57f4c736fa5c558eda75e7a89100590d Merge pull request #2111 from vincepri/readable-gomega
1183a159892023f4039a593a194b6491942e4079 Merge pull request #2060 from fabriziopandini/clusterctl-move-object-graph
11eec41abb938c4752279922cbf4629a66cc6e3e :running: Make gomega tests more readable
f4bf01e486530475cad6d2a4e63dfdd74cd06b91 Merge pull request #2110 from vincepri/update-onsi
e348aebdb92eaf6b06e0252bd93b273bfddcdb0d :running: Update ginkgo/gomega to latest releases
00d4ec3676850d642c450e8f5983b257584c15e8 :running: Add test for KubeadmConfig conversion
62f09764850ca6313bd8c5562451237275ede3c3 Merge pull request #2107 from vincepri/labels-cloned-kcp
40a9f37c67e5eb047ba2b2bbd4303a78c3aa99ef :running: Propagate KCP labels to cloned objects
bf9707ed30235e8afe1f15446a0353b7c2884968 Merge pull request #2103 from johnharris85/fix-webhook-port
abbd257d68fe9fe2bd0ed4941c754df1e8becf52 create the object graph for move
e2eff2e595f3be4aa147e32cfe7e4adeb75216ae Fix service port selector
412f6b3f13399fdb0f815f12534feee6ed5fa4d8 Merge pull request #2098 from fabriziopandini/clusterctl-fix-docker-provider
30b28a5f7596695a0ecd012a0d23c547b2bbf55c clusterctl-fix-docker-provider
36ee6b04217695649e632c706cf93bfc52368a79 Merge pull request #2093 from clayvan/tinytypo
a07bd6ac55ef7bf887f282adfbc76bcdde4d6096 Merge pull request #2096 from wfernandes/fix-dev-guide
67f0c7f1512db38d4c3dfa52c24299e5df9e0264 Merge pull request #2095 from chuckha/kcp-e2e
421afb35294d275c0d1a71ae391d707939f1bb19 Fixing a small documentation typo
bf714a737810bd1b5db8e997050158998bde7d51 Remove link to broken REGISTRY env var doc
b409a4308a89f1d4319d8c27a1d4fdc68b1f8c40 Use KubeadmControlPlane in the e2e test
08f492c524ecdc0840d436a7353e1c51084e3858 Merge pull request #2094 from chuckha/delete-control-plane
fe4c5e434293a83fec41ed5ad4e4eb1072f2f7e4 Merge pull request #2087 from vincepri/remotefake
9d59b43104004af6f344c488b18f9a21377185c1 Handle the control plane ref delete in cluster controller
9df2ec74c82d83ec3de922665f34dca3631e3f0c Merge pull request #1994 from fabriziopandini/clusterctl-update-book
eea1679f9b674afd4a10247f9ed11bdc4f631a4a first iteration on clusterctl docs
1bab28806ad9a85e371d27811cf7d13695702955 Merge pull request #2091 from vincepri/cloner-ref
520299ea1bea7760cc82c30e7dbbb8539cff1a21 Refactor CloneTemplate / propagate clone labels in MS
457717940255bc5799a781be86efa8c47be1eabc :running: Add remote fake client
09baf60b7cf0b8805bd49914c436d7d5aed665ed Merge pull request #2088 from vincepri/refactor-kubeadm-reconcile
0348db5f25ae56c952134a5a04fb587a56be42d7 :running: Refactor kubeadm control plane reconcile funcs
d273a9a8e6ea6449589cb5d72f8e2291c0ec3d87 Merge pull request #2076 from chuckha/update-capd
9c2fc9e3ba8e7a3cb5cfbf4bebf6acc688e0a89b Remove dependency on kind v0.5.1
401bd4e02ec34876752df08994717392a69dbb8f Merge pull request #2037 from dlipovetsky/controlplane-delete
961aa48ba85fe017f83be0c976d61b7452016798 Merge pull request #2085 from lsytj0413/fix-typo
d1819a806df04a09076a8acd7b018d5a6bcff70b docs(*): typo regulat -> regular
827d3e4b339272d249cd3f9432ed4fef604440ea Merge pull request #2079 from chuckha/failure-domain
5fd8113089e6711364cf6077c8a7faa7d1a51ce7 Adds failure domain to machine spec
07ec969730c39e1875522282a84264c9bd30b11c Merge pull request #2059 from fabriziopandini/clusterctl-improve-move-test-framework
9d17c423b6483cc3da601a881c764a3df4acb84f improve move test framework
73c08cd8f71abd16cbcb57a5c69d8d3d112ea9f2 Merge pull request #2077 from SataQiu/fix-makefile-20200116
4791e00e88cabb0227d83f5df48883e7aa202e0e Merge pull request #2071 from fabriziopandini/clusterctl-remove-force-flag
830be174afb0a2e2fbd59af676cfdc31eb074f41 clusterctl remove force flag from init
b95cc085179ed30c13a7769619bba27db092ec4b code clean and bug fix for Makefile
fb39702963450c0a70075b49dd2e5064d09d14b8 Merge pull request #2035 from noamran/1960
9081f61d3e08243d3a6a4865a91059523599190e Merge pull request #2047 from fabriziopandini/clusterctl-config-cluster
31ebcaa5e83e33bc2d7857cd8a128b2da388ced8 Merge pull request #2061 from fabriziopandini/add-version-package
2f74797667dd86e2712b67bf7892e9d13453c5b3 Merge pull request #2075 from fabriziopandini/fix-clusterctl-hack
8b6ea75d7e48ec38d900f92a5742700a0eeb5e9f Merge pull request #2069 from wfernandes/fix-release-manifests
d3ecfbf569cd97d3b9db5597062af5312392e81a fix clusterctl hack for python 3.0
94376dd6959fc7d1d8666f45d9515352d05ba7de add clusterctl version
b7bef935a1b1132fbaafccccc68806469108e920 Fix concatenation of cluster-api-components.yaml
7884484b621f13f604e74f60053f4214a2f19702 Merge pull request #2066 from dlipovetsky/fix-apierrors-bug
015d9fbbc837e7b326043db223234933a6a716b9 add the clusterctl config provider command
a7412c7d967c2af5d0bfbeb9b1895487311daed1 :bug: Kubeadm-based Control Plane: Fix error handling during cleanup
5e03d6d1053cd141970c63ca4365d3a84709d455 :sparkles: Implement delete for KubeadmControlPlane
769f14e6852d493df34f1e6243693c4c646498b4 :runner: Add util function to list all machines for a cluster
897998569fb4f8ec70dffed92dff8789e1c46c92 :running: Use MachineList instead of Machine slice in KubeadmControlPlane
c9924f22046c84e5614abda0ae7d6f0bf1ff4024 Merge pull request #2048 from fabriziopandini/clusterctl-config-providers
718527da6acf3a7b7fa5e4634e91ab173fe230c1 add the clusterctl config provider command
80103ebe02019a561647f9d2bd2ed23572e657c0 Merge pull request #2030 from randomvariable/proxy
728fd4d9013b3439830a649c16211f33d6a6190e proxy: add proxy package for connecting to pods with http/transport and net/dialer compliant interfaces
0f62f835a81f173dffba4b5fc24f54a0e8d7c5cd Merge pull request #2053 from vincepri/release-notes
4e471a68206cec222ced2f29292777c48efaf889 :bug: Fix Makefile release-notes target to build binary
75f4b0da89ffbbd53246d95b9f2bd2a0a50e8822 :running: Improve release notes utility / add -from flag
7b2ad211f455008497059918da18085539f74115 Merge pull request #1903 from ashish-amarnath/update-ci
64d1f6aa1bf7e4d21dfc5de9f367682b1d43bb02 Merge pull request #2033 from chuckha/capd-update
3b341a962c74aef8bea13f5911890d59524bb680 Merge pull request #2044 from tedyu/machine-del-err-ch
2115595ad907bca07c219cfe9279f619fc92b898 Merge pull request #2043 from tedyu/ctx-todo
11590750c3ba8829fae1cb124579c3453cb0dc1c Aggregate the errors from machine deletion
8e9ff9c82b1f80dbe31cc1e844a0ccc03d219d1c Merge pull request #1996 from fabriziopandini/clusterctl-template-low-level-lib
db64a482f0da4bae0ec4ef00d91ac3be100cfe09 Pass Context parameter instead of calling context.TODO()
52cac4b7b25e68d686a3cb8bc1ee5e213b86865a clusterctl-template-low-level-lib
0d68bf91b89a1b691333da55e07c694482ea21f2 Merge pull request #2022 from vincepri/fix-more-conversions
78bfb4bc0f1a13488488df5760b5db6cb6bb0a55 :running: Fix more conversions / add tests
fd6a5d82d10aa5a3f40f9f1ad3d25c2d8d53a1a3 adding an auth-proxy sidecar container to CAPI core
de08a6fb521647424368cc652db753de11e4c503 Improve kubeadm bootstrap controller
039705a2822823e7651dd4e7572b3add3abb0109 Merge pull request #2040 from fabriziopandini/clusterctl-rename-config
d8d392ecc46cceb2cd36a0e3d35896462faf5206 improve capd-e2e to build off actual changes
dea45c9f917d2de3b85db12ccb32ba2ac6b68d70 Merge pull request #1974 from fabriziopandini/clusterctl-add-metadata
7e9b86c76e9a647d43eed527d1f48604cd9456bf clusterctl rename config
07286a7096ffa8b4e87f3bd3294febf876e699ed clusterctl add metadata
b9759d322d1a0aec461aee51ca66edfa2037075b Merge pull request #2039 from aaroniscode/doc_fix_tilt
1b8498d48452c9977dcd33f636abf57cb03c1bbc Merge pull request #2027 from fabriziopandini/clusterctl-hack
bef0d74bffa87f266e0bbb0ea27154af0ec7c1ad enable cabpk and kacp providers in example tilt-settings.json
0781bb1f31fafaf60c5070f65e8483c844c9ff43 clusterctl-hack
ef75be8bda4050d600c96e8909f1a074f31a4db1 Merge pull request #2032 from chuckha/cloudbuild
fdce104be7946684ed2048ea65a16ca9f5693cb6 Minor cloudbuild clean up
01f228d69c320e2be9b2fe03bc8402290651e166 Merge pull request #2017 from fabriziopandini/clusterctl-cert-manager
ff76de1a51ed21d4cab10fa7425117daae885b55 clusterctl-cert-manager
afdb440dc7dab3d25f57ca906567016c819e33ce Merge pull request #2025 from dlipovetsky/tilt-union-enable-providers
37b4013b1a75f8e799702f4ecec2f535b6c75480 Merge pull request #2018 from vincepri/clusterctl-minors
8bc65c3aa70c416b871b02bfe9cd31e17fd10737 Run CAPD verify scripts in CI
19f67639c99874ac2a651ed780894bebc0e812d9 Merge pull request #2024 from dlipovetsky/docs-tilt-kustomize-standalone
4d0d62dbb0045da499a3cd9cc15792f98e92c5de Tiltfile: union providers enabled in tilt-settings.json with those always enabled
429cbfc0b63e7cf41ebf1096c2a7ba98e3a38c79 :book: Add kustomize standalone prereq to tilt doc
e385d3d8dafcb71a2150c0262713416174b1cc35 :running: Minor improvements to clusterctl codebase
9f4dd9d110b424e0cd8f25dd26e5f9b9fff08bd0 Merge pull request #2014 from chuckha/kcp-perm
35a1b56f26671219160933e6bf4c65880a0b62d6 Merge pull request #2023 from chuckha/gocyclo
159a2ae31514616e31d7aaf13b83e6f922cb2c37 Add another permission to the kubeadm control plane controller
9284a03b1e43953a42a1355938da29a00ee426c2 remove nolint:gocyclo
71dc1dfc3b6941f911954a1d23e8e9d78cdd069c Merge pull request #1995 from akutz/feature/e2e-framework-enhancements
d7ccf9c2c2714f2c3fae308c7253dc3b1b431209 Merge pull request #1985 from vincepri/pause-reconciliation
d554066984fd5bce53a2b1dc412f81746393add0 Merge pull request #2020 from vincepri/controllertools116
6a27aa8c057cbe7f2639353da2a27ec84b09525b Merge pull request #2019 from jayunit100/patch-1
5b83d2ab9a1a9b007c4e483f9db4978a954b232d :running: Update kubebuilder tools to 1.16.4
9f23a0069756c8dd7e7196d977d20fab76be91b1 Add Workload Cluster definition
e4c46dd9c3372ed26f5bc252316caf888a3b47e7 Merge pull request #2013 from vincepri/conversion-improvements
f26760de82d9b4c52eff8acd2a8945076c5372dc Merge pull request #2012 from vincepri/err-aggregate
d2eb510e1fe9146feee83be38d4b8a25f698f652 Improve conversion webhook: add tests, fix preserve logic, remove nolint
3057acabbffea3e057f59a5872d3c2bd697930e0 Merge pull request #2011 from chuckha/fix-todo
726dd84fad061925bbc0c6b74a7c9630031f75af :running: Aggregate return errors instead of overwriting/ignoringg
3117944142e9a038294c73465c6b65673ba154a7 Improve logs and fix an outstanding TODO
d275273f6df3ccdd75b0f5a242349598ad742b27 Merge pull request #1997 from chuckha/kcp-e2e-2
ea48d0cbce4443165cf035e062d2f95d9d6e918a Fix framework and capd e2es after manager split
056b4b8161996d77323e757d1d6474cf6bad91bd Merge pull request #2010 from chuckha/bootstrap-cluster-label
d3a0e9a4d544972de5cbbf470c5985675122ec64 Merge pull request #2007 from vincepri/kcp-set-owner-template
a750e91a3599488c9a461e5f23dc6e418f147f6f Merge pull request #2008 from fabriziopandini/clusterctl-fix-init
672ab3c6e0b97a45896b8c432d6c543e546a4c9b address comments
07761fc1a6be3f5e3be4f47289b87c46071bb128 add a cluster-api label to the init lock configmap
ef4a6f8a797b3390583eee1b20a4cb6e38babeed clusterctl-fix-init
e50de4ee4756e43459bd30d1489d8175c2fd8774 :sparkles: Make sure KCP template resources have a Cluster owner
660e6b945a2777b4e61f70d9bdd0b50abf42dcd8 Merge pull request #2005 from chuckha/makefile-typo
5d71035e481a74f349c1047c2a5735e3b2813168 Merge pull request #1932 from fabriziopandini/clusterctl-init
db5e4181d964cd97c67c9351d9c401222c500006 Merge pull request #2004 from vincepri/up-machine-cloudbuild
1b7f51e6d4f4e28f95b60db4c1aa0992c8c101db Merge pull request #1977 from fabriziopandini/clusterctl-move-test-framework
21f1b2c24b8aaabb2700a4dd3e6b61b324483183 :sparkles: Add support for pause-reconciler annotation
2f58960f3a91cf899455737e375fbaf13b9c6347 Fix typo in Makefile
e4a35a527010d0810780b136866100c995c49351 Merge pull request #2003 from chuckha/docker-cache-again
ff3e5ae2c4ca6b6ca1e948e94649ce1ff0a4fb08 :running: Use 8-core machines for cloud builds instead of 1
34f1b8034fbda9e398980869602f3490236dabcb further improve using docker cache for release
437ebf961424ab3e316b10e33aec3fb0c8f525d9 Merge pull request #1992 from vincepri/preserve-downconversion
8afcecf32054d21909c855d352c010ced2492c3c Merge pull request #2001 from chuckha/cloudbuild-timeout
148085d1d248f31cf6506187adec11bfbc8cbc73 Support multi-node CP & MachineDeployments in e2e
f97c42ce00a9a2b119a8a9015132ddb842c963b8 address comments
9def4bbb5d09cb04b81af80ad76a64e701234155 Bump cloud init build to 45m
b05134783494598c0017a592356fb0391f380319 Merge pull request #2000 from chuckha/cloud-build-timeout
f830c557cdb68b07d6442d479618e72fb3b19546 Bump cloud build timeout
383574e925ac71296389556f6eec8696d32637d6 Merge pull request #1999 from chuckha/docker-cache
c3ea7502815fa87bab4ab5993fe9c3fc1d58f61d Better use of docker cache
6a6debc277a09713a106698dd7c5613f1c35238d Merge pull request #1980 from dippynark/add-manager-role-aggregation
14cc4d45569d7aeea1f012527a6444f12abce23a :bug: Preserve data when performing down-conversions
b6ae50b9611b3f352e89f8cefe39fe1fd0494fa3 Merge pull request #1972 from chuckha/kubeadm-extract
3fa8a4ca5164d1274d0ecfd235c504ab1628d096 Split up the managers
5a884eec423e46d73a5c0fddbcadab4d88ff6df6 add the clusterctl init command
8a34a6295405330764a849ba0dbc68068f678116 Merge pull request #1909 from jiatongw/clusterctl-github_repo
63ff715889dab572469c4bb5699c65027ab2b522 Add role aggregation to CI
94ff016d5be1f2d4b15d976b3f6d549be0b96585 Rename aggregate-manager-role to aggregated-manager-role
6ee5eef8df9a96101821eeb7dc04d3f0cff692d2 Improve aggregation comment for clarity
029477edc7973e2a3e45c03d08d6882dc9ddb659 Fix manager role aggregation
97e44e39684a8ee5a9d24da48274547d0bfee599 Wrap at 100 characters
c367ce643173691ff79f7d8b6d1f3421b597c80d Clarify how permissions are granted
6027ff421dd5f53ee206ae314fdc6720cb759e71 Specify YAML language, use foo instead of example and restructure
b152c699d4ddaffb6807d8c78fcb2248e68d19ce Added usage documentation for aggregation label
8698f3471698bd5cd1cb038331025b80cde1c9e9 Added manager role aggregation label
09949bd397eecbfeac4e011b0d2c29fdbf2ac1ef clusterctl v2 first backend implementation for repository using Github
dbe789259bdf6e94e8a51aa49daeccafaa2f0ffa Merge pull request #1981 from fabriziopandini/clusterctl-local-overrides
2febc3a3f58ed057e013d784a5a290d267600fb1 clusterctl add local override
02cac5c472aa408c5826587040aa4a77d6b2c5a1 Merge pull request #1968 from detiber/kcpScaleUp
965de3f18476f9e1cc66178373834424dbf7997c Implement scale up for KubeadmControlPlane
126a5c329b9a6c8ea79130b1965e60c205c137b4 Merge pull request #1973 from detiber/kcpStatus
f39e25f91565aae883876d4ffb8a7aa8b14d093c Start populating KubeadmControlPlane Status
72a7b2f1d9df0170ad5a43580ca2991b384f6e8b Merge pull request #1991 from detiber/removeInterfaces
c269be3086e9c191cfe3f53b12a390971d4c4014 Merge pull request #1986 from fabriziopandini/clusterctl-fix-RBAC
02d71a1ea11617ff441683851f767420676a632a Remove TemplateCloner struct/interfaces
84cd362e493f5edb7b16219d8134a008efb01dac Merge pull request #1975 from fabriziopandini/clusterctl-allow-config-override
3a0e009587e82a02369ca8ef2f96b9dac73e3291 [kubeadmcontrolplane] Remove KubeadmConfig Generator
88b9a6e3ccb96b6bde3bf5e8a19212874c9d1948 [kubeadmcontrolplane] Remove MachineGenerator
b20cd91ce92ec4ad2be0ea73a55d8a50ecf74475 address comments
e433e2d803ad4d869ee2d90e474e97893df26953 clusterctl fix RBAC
102981496ed83c2ccd8627c7832102344864669e Merge pull request #1982 from yukirii/fix_tab_usage_machinedeployment
30ee014a215a0492732cb0a9ddd511c9ee3b9b69 :book: Fix broken tab in the Quick Start
a26471f9f279ea37863cecf3148433367dd46a47 Merge pull request #1976 from fabriziopandini/clusterctl-refactor-fix-namespace
5ed3f5ec8018586348405f569e5071a0368d8224 Merge pull request #1978 from fabriziopandini/clusterctl-add-getversions
05d6f17b9b73173348d3ebba7777884b9777f7b5 clusterctl-move-test-framework
2109d0dfa7740f7eb3cb1f00ec1c1afe3aa6f9ab clusterctl-add-getversions
578f8d30846e155465d9cff4d0ab7a03db345f28 clusterctl small refactor of fixNamespace
8cb23da6238e470c0998bf78c14e953661b76d73 clusterctl allows config variable override
c246f9bca97a971ade2a9694c0c939c7faa3444e Merge pull request #1944 from vincepri/ms-controller-patch
a6db0cc4c9482a2a08f9b14455c165d395a6699e :sparkles: Refactor MS controller status patching
b3526e16762f3f5b40692887c42e2c4d0000904d Merge pull request #1925 from detiber/kcpCreateTests
366530a184ce9e38196ff984ade51f97fb0abbb4 Add initial tests for kubeadmcontrolplane controller reconcile method
83c7edf23e727d89880f3adc697a9db41488e98c Merge pull request #1965 from detiber/updateUsageOfFakeClient
f34dc39809b7362345d8dc531129b1e4c28e479b Merge pull request #1957 from chuckha/capd-prow-logs
e93c6ac8db4719df50cb466be7182c80f9c38ba5 Update use of deprecated helpers
6489960b74abbd3a8e57f3bde776cca7a140715c Adds infrastructure to get pod logs from a test run
e58d2a99e78223174cfd1b2b1bc38815427cdf43 Adds a way to get a clientset for the management cluster
d1feb5c5a2ff2c2ffaca3fe996dc218b485ada88 Merge pull request #1962 from jdef/patch-4
e6216c20941fb48b9bdd0f8fc34e6efafa84174c fix NPEs when the user doesn't assign labels to MD
053db10e21865e67f3169ac95890eb23d9047bae Merge pull request #1959 from detiber/utilInjection
e4961fcbb86c64f1a3a88b4d3e7f36736467dd86 Merge pull request #1961 from detiber/addLabelToKubeconfigSecret
161e5f3592cca193090c85419f79c7fa4bf04251 Add cluster label when creating kubeconfig secret
1815a456e8dca3809e9117054113a31a312445f3 Refactor template cloning for use with kubeadmcontrolplane
98e2b5a809452077d279858dca478f575747f831 Merge pull request #1915 from wfernandes/e2e-delete-resources
7b4493527e587b61842d6578dc260d3c6c96807b Merge pull request #1958 from wfernandes/fix-validation-e2e-test
65df9d96a13be67fbcf9b38a4b73b57f5b2bc613 Refactor for minor changes based on feedback.
2b7fce56e78842eaeef90e5509061263f62fae7e Fix validation e2e test
fd807a3d843b722a3b4feb3c9e3bcd752896daed Merge pull request #1814 from prankul88/external-etcd-improvement
48b7f34405c1d48190d87f49464ece5386287356 Merge pull request #1955 from ncdc/verify-starlark-fixes
3ecee600cbb1f79dedc21713286aa2d0285bacbe Merge pull request #1947 from vincepri/template-ownerRef
98daa586e0f6b3d373dffe5da04119e86d0ea8c5 hack/verify-starlack: better dir handling
302b4e446ee6cb612646899826ffe7128e94203b Merge pull request #1956 from jdef/patch-3
4c5edd4a9298b2897173bfa1b3904b4cc11f051e passwd is omitempty because it's optional
c4857b4f7a5407cda85d3cf38cf7f07c820faa18 :sparkles: Add cluster owner references to external MS/MD objects
f38f44a2bed68abb68d59d8ae13794b8ee51aaf3 Merge pull request #1885 from juan-lee/cbpk-contract
42a5f42fe74130004f527549313bd5e9a16fae04 Assert provider artifacts deleted in provider e2e tests
9d72db77c6a068ac12665ea737d5e590eeba13d1 Use pointer receiver for ControlPlaneCluster
1a1bdea6f747fa8600efecbfa5fe547748209d2a Use To(Succeed()) for asserting func calls
3efd98f2be0d39036971d602b2be2ebe7753aa4c Add docker e2e test for cluster deletion
386bc951711fd6439507f0d7b953100b47644cc1 Generate random kind cluster name for docker e2e
c71f7ee4c6812380076e26de48e23762bb048fc8 Add DeleteCluster test to e2e framework
98adce69541c67250d10fe19ba0d0f1d55f739d6 Use Unstructured to access Config Owner
c531036c20f03b8d99395ed607945a8ace042431 Merge pull request #1881 from rsmitty/issue-1686
af3407ad47c51a6ec8548e1e48e37a1cd3cd3f0d :running: support multiple release manifests with/without kubeadm
8536f42217617887b74c1a12d788a0e526a80d13 Merge pull request #1942 from ncdc/fix-machinepool-webhook
ef6e7e2325efac8bbd425f465fbb3679dfd60816 Fix machinedeployment webhooks
d5abb4d1657a73d711b33f0da27a9fbc6ab0e208 Merge pull request #1933 from randomvariable/cp-domain-fixups
a8fac5cf90606e530f1ccf2e0129d357f3b16430 Merge pull request #1939 from chuckha/kcdefault
c46d0f5a97ba0e6cc772240ee4b717b638fdb3a9 Change dataDir for local etcd in kubeadm type to optional
1707ee621455856d10c5b1eb82e6d0ea6ecedc4d Merge pull request #1940 from chuckha/capd-e2e-timeout
c0d5b60ab38159507bb83142fa6456fa4244f2a0 Increase timeout for capd e2es
7255ee8703e2c95c7acf9d81584ee2342c6b100e Merge pull request #1929 from juan-lee/machinepool-types
0e5ec3ece8a449a9f96cecb382f4e475a9ce26e8 Merge pull request #1937 from ncdc/fix-tilt-restart
eebe4dce1dc9158757613ba714fe538da288e9df tilt: fix restarting
a7c793b4a71bbdf3b85a3c5616f09d6877cc937d controlplane: Update finalizer and PROJECT domains
fc82280aaead21bb03d41ab38427dc735f20419f Merge pull request #1936 from chuckha/cleanup
c9a8d01381f7414ed316cf77491cd5ce8de173c5 remove outdated files from CABPK
a516a47e9df50e6c88afd0a1026f28762f7a7e8b Merge pull request #1935 from chuckha/e2e-image-loading
5a66be7b05abd8cf2d838fd7d95490ccd315c68a Skip loading images if image does not exist locally
1e5cf4d27a7430edfb56c2216d9e35216a137729 MachinePool API Types and Scaffolding
f766452c3776c16c925c8ff19a91b49a1cd10327 Merge pull request #1931 from chuckha/kind-for-e2es
ed22d6b3869f4796cac520399dae19e1515dd910 Install the kind binary for capd e2es
c2023678f66d8114ca79d054b4ed87bcb1ca3c5b Merge pull request #1898 from fabriziopandini/clusterctlv2-cluster
a0a59f3d906f323da0ec85ef4d92b4844ee8bc2c add interfaces for the management cluster low level library
b53dfceb3263e8ea2e7b2b9ac0a3f0e437eb9025 Merge pull request #1920 from randomvariable/clusterconfig-npe
a6df99d91b03ba51bcb7e9ce6fe1191b9209f088 Merge pull request #1913 from vincepri/improve-md-patch
732d6da245816db89cac392d225159a88e37c878 Merge pull request #1928 from chuckha/e2e-script
e3d9ddb10ab7b76b7eb55f5f7504fff02af18c13 adds capd e2e script
3ae91df13672640ca674837b51f808588f60e09c Merge pull request #1924 from vincepri/tilt-distroless
4494219a40a9786357c3331e034680506aa965fb Merge pull request #1927 from vincepri/gcp-tilt-docs
e7652cca1943173e0bee864865b88b9f1b3e4184 Merge pull request #1684 from enxebre/mhc-proposal
da772eac18dde617aa43af2cc8e8103b8f8b2f77 :runnning: Use distroless for Tilt / includes CA certs
cfac194056548a3ed388f88161ff992b86897ba3 Merge pull request #1922 from randomvariable/tiltfile-docker
de0a5ba5a28312fee0cc82bbe184c17588171539 :book: Add GCP credentials doc for tilt
100db94b27f92231b7b4660b93885f1a38ba2564 Tiltfile: Add formatter checks for buildifier 0.29 hack: Only download shellcheck and buildifier once
9704cb8f7329fa12e3f6225d1f2d95b92e78e178 Merge pull request #1918 from vincepri/make-networking-optional
67b0fa78f69ea4fdbe4645227cdc5eaf6f0f7867 ⚠️ ClusterConfigration.Networking.* fields are now optional
2536f6609cb018d1e11f9ccebca42f4693f888a0 Tiltfile: Support appended commands in Dockerfile Fix up for Docker
2ec001715d515dd43130d2f8b50c4cd174440704 Merge pull request #1923 from randomvariable/cp-spec-summary
9ddf808f97a899b2d190fe58f784618decaea35f book: Add control plane controller to sidebar
dc6659dfe8fe3d4c2a1bc50429a30d451a77eda3 controlplane: Allow nil ClusterConfiguration Supports Docker provider
365c7cdabfd1d7d450a951773b1924deb4a20895 Merge pull request #1919 from randomvariable/Tiltfile-without-kind
5a9f5da6832b390335250007d6eda2c45eb443d3 Tiltfile: Include live reload suggestions from detiber
d9fbc68d896be6fda376578a88a3fedee24e279b Tiltfile: Enable build cache
cc16fd20903d00d5d18bfd12b030672d9fb5ed70 Tiltfile: Enable Tilt to be used without kind Also, make cert-manager toggleable.
40d316aa57e522a5c2a725ca3e31bdd3a236b9d2 Tiltfile: Format Tiltfile per Bazel rules
5e74c7590e5113df3e928c45218e386263257e0c Merge pull request #1916 from detiber/moveKCPAPIGroup
74765aae49827b0ea214e7ef1a8f90d565f985b9 Merge pull request #1859 from wfernandes/e2e-tests
1a9e982637ddd90fd77047e32e02d1d1b7bb1434 Move kubeadmcontrolplane to it's own group and subdir
2993ceff496ca0aab79dcbcff7d1035fe4f1dae3 ✨ Improve MD patching with helper
7624d1fe6a8789046c37f6811a7c9a5f6981b162 Merge pull request #1914 from chuckha/capd-dockerfile
d0c12811b55d2f0562624f0948dd4178d570e6db Fix up the CAPD dockerfile
a45cc55502257671315e4c47fd4ef7e892b81cc7 Merge pull request #1912 from vincepri/fix-pprof
dd4263dc4cc6b57422b4f186145b8d6317a3caa9 Create separate namespace for each validation context
1e534196996021b47420d486b13def0b8818c3c6 Merge pull request #1891 from fabriziopandini/clusterctl-components
3e3e74be033b56ac34d776eafaa5033877802719 :bug: Actually import (and enable) pprof
0031f410707eca40787d0f2f8dcd41315b8031a2 address comments
1097ce5b5676260178ad54d58b10c203c1e2461b Merge pull request #1911 from ncdc/gcb-for-tag-image-builds
6b82c20017dd48a3731c2beb12fd136f4239b118 Merge pull request #1904 from vincepri/go113
d51e40f8c1efa5aa41fb290064b0b4830d756b24 :running: Update Go 1.13
546d56bea2b8cd9ac24d90ed7599d209dfe2ccc5 Merge pull request #1894 from ncdc/tilt
5c35511b6bbb2ca5d63415a56bf155c408398ab7 Let GCB build release images
6fdd5907febd76c9af350a26002f7d2b4a64a82a Add e2e validation test
3c2df5279fa1d4772b9c9c24f57f103e399cfd46 Merge pull request #1899 from randomvariable/control-plane-spec
540e0bfd685c43b467522d90d2b9e79ded3380a7 Merge pull request #1906 from vincepri/fix-secret-data-validation
5a26b12484baab74d378c178504b05bdf5187090 Add tilt-based development tooling
8f1fbac50c5b9034befd924bdbdc931afd27941f :bug: Fix validation on machine's bootstrap dataSecretName
8e57f0be14c03f9e13b0831a084bf8383ac6499a Merge pull request #1900 from chuckha/relative-import
cf2a6d2cd3e2445ca9a9c19232fdcdab16a50369 book: Initial control plane spec
820fbc20a1f895a47bd94b6350f04ff70e091741 add more tests
e5764ff1014b8f0806423ed63fd2f21d0757ae01 Merge pull request #1907 from vincepri/fix-cluster-label-name
b1ae3fad022a347763be04b5b5bfe320d4a65be8 :bug: Properly set the cluster label name on bootstrap secrets
8a6c3ea3eb4289351df3efc43b2e23fec101150e Merge pull request #1893 from fabriziopandini/clusterctl-contract
ac7c8d0c4351c71091b83978505dddbda543fe1a Merge pull request #1715 from ashish-amarnath/capd-verify-scripts-fix
f3551e5bffe4f7ac90c837637e5c6d08c3d63890 document contract for clusterctl
912cb3eac0a2a90be2d09272d0b064581aa86c5a Remove relative import from e2e framework
db9baf9ade0cf67e261ea7637722e3ff3fd38499 Merge pull request #1896 from akutz/bugfix/e2e-framework-apply-order
c5355e3327af0b16926b9aad916c89f6db541f2e Fix e2e framework resource apply order
46919c939793f666b0b63058487e2deb3f2e7417 clusterctlv2 add low-level library for the provider components YAML
454332444b69dd1120084f1ada5ab8a8752deeae drop support for reading /config folder generated by kubebuilder
1bb8132e8c034d0d24346e3138747e94a90f6d18 Merge pull request #1856 from detiber/kcpCreate
f248367309a112b021c95bd8747b17200739c18a Add create workflow for KubeadmControlPlane
ecca82b1e71c134cfe7b5677932669652309305a 🏃 CAPD verify script fixes
1d5e22104d69a6b6dbad03b585d632f83083c26a Merge pull request #1887 from chuckha/bootstrap-error
95c32705af71d4f7922d6c6bfe37ddf4b724c628 Merge pull request #1864 from fabriziopandini/clusterctlv2-config
e4125484217c6c5b532e2b0e0756f6346be14424 Do not error if bootstrap secret already exists
516215d590445826be05cf52f711203031531c14 Merge pull request #1871 from vincepri/failure-domain
406210989d77c1e9540db08f3d7b26526bdd6dbd :sparkles: Add support for failure domains
c784e10006bcaaf4e501860438563fa5e97987ea Update generated files
98b4afbeedf5b7d87fbf6f49859675d31bd903f6 Merge pull request #1892 from chuckha/framework-fixes
cab254dcb23a04800db921cb9ec303c411e69edc clean up the test framework
f2cdbb514a08f0677412139c0834db66f5b61662 Update changes based on comments
1a2054d7f6b62de018af61e570fdfc613e1754b5 clusterctlv2 add implementation for clusterctl config providers
229ca680f8ff29f228da8da07955eb173139e11d Merge pull request #1889 from neolit123/amend-troubleshooting-labels
c071b5dcae9ca6c206b01b05b36cd32bb44388f5 book/troubleshooting.md: amend the entry about node-role labels
1625f2b5eb2e5a2fae6094a9ed7cd7f6f1e58c50 Merge pull request #1888 from wfernandes/fix-capd-example
5b1f49399aeb31ad0c313b969128d255457adabb Add clusterName to machine spec
673f7c4ac1d39710c08b16b2c7163093cb007692 Merge pull request #1883 from neeleshkorade/master
67165391bd14189fd864606cea9cf508307e96f2 Merge pull request #1886 from wfernandes/e2e-framework-updates
a43edd419c447a5869d9bd62fb4283b38ae7a225 Fixed spelling typo
30c58a4017dda146955c59ea0a8a93b084bb6639 Update e2e test framework
3b98faabfa4a96a42bced3973ff34beff1efcd1c Merge pull request #1865 from ncdc/docs/machine-infra-provider
bade0ceda055f054f0727ef686ba11e32dad95a7 Add machine infra provider spec doc
f36877b99922de11e447357f53734da6d811a748 Add troubleshooting page to the doc
4fb707b1d2b942b471af206b567b60b81e7602d7 Merge pull request #1879 from detiber/versionitis
8d32202a72ed2409827b28b66c3b8873912297cd Mass update of test cases, docs, and other outdated references to v1alpha2
70074c7f58b9e50298b01165cf60489658afc928 Merge pull request #1797 from b2jrock/kind-doc-update
f2018745822b3c206304b40df493dfccf6cf5624 Update documentation due to `kind get kubeconfig-path` deprecation
20d7b505733fdedfc4ec43d019bc1796fe86c1e3 Merge pull request #1703 from juan-lee/machinepool-caep-doc
9d2584a5b0eb7da5953c8753dfd680dcbbb69630 Merge pull request #1875 from rsmitty/master
fe33be0905a924888a1462619af346e28670125f :sparkles: add flag for disabling kubeadm controllers
45efc9278a8e0652375130651b04ec91eb5f8425 Merge pull request #1874 from ncdc/docs/bootstrap-provider
ad39e36b1e8e4405d1170b5c5cfb206b2af3add6 Merge pull request #1842 from fabriziopandini/clusterctlv2-Irepository
e9ec746d84f34f45e23c48aea6dd9b8595d5c1b7 Merge pull request #1873 from vincepri/pivot-kubeadm-secret
f2cc62068887ecbe34788fcdc811ae5363446d67 Add bootstrap provider spec doc
d0840ed07b848d60d54097e7acdfe6959194f150 :bug: Handle CABPK secret case where status has been lost
0eae5c6b4427d372db9736eb503d9c35fccdbda1 Merge pull request #1862 from ader1990/fix_cloudinit_docs
66c8134e30d5c29a6e35d985fe5096afac72e5e7 Merge pull request #1869 from chuckha/dockertypes
a2592b604f79a6be587bdd2450667f9583b3a585 Merge pull request #1867 from chuckha/secret-data-name
af15c9050a1919dc774083acdc8717edea9c5a46 be consistent with dataSecretName
567ba2a78b3afc2ab3c20f0460143df345516241 docker fixes for v1a3
376597c58ecca22d5f8ffff97c49ff7fd7c988d5 Merge pull request #1785 from chuckha/internal-cloudinit
0624ec0790d1190fcb980c4816cd38aa430e4b87 Move cloudinit module into internal
1882b0152429da3cbd50aba9e9129e176ad26bf8 clusterctlv2 add Interfaces for Repository low-level factory
5ea5faa9d9ba625bea92f27a0da9278384e539d4 Merge pull request #1841 from vincepri/add-data-secret-name-cabpk
b4b7a1d0d266ca26febd1d113ca4786d664b1b9b ⚠️ Move Bootstrap data to a secret
c24f55e455795c8d5726dcb33d9bfa68088e2fa5 Update module dependencies
c2e85de347fcf249cfb43bc84b5184e8b9d7f931 Update generated files
03c7b1c1145234576ebc4c67aea380e3d337d0e8 Merge pull request #1857 from ncdc/capd-ci
cf6cdea68f54b089a00ab2ab054488bd3b0c717e Reenable building & testing CAPD
ccb217449658abc2c24777e556339f8189428070 Merge pull request #1762 from fabriziopandini/clusterctlv2-config
08a3b66d7a66244808ba457e742be166969a0e35 Fix cloud-init jinja templates
79a1b83a620456cd9c1c58c767cae7ca5802c5db Merge pull request #1817 from thesystemninjaneer/fixdeadcontributiondoclink
5b176459f67b62cbe88882e6bff8fd0cc97185d5 remove burned in markdown reference to branch
301fc1f19d3e4f1974d1d9370d4890a5fa81e139 Add contributing and code of conduct markdown to SUMMARY TOC reference section. Also add 2 new markdown files with repective references to source markdown files outside the src directory to remedy dead links on doc homepage. main README updated with link to two new markdowns within src dir.
9308db82b836aa9c49748f2932dac57c6e87c388 clusterctlv2-config
f6cd8d79e907c3c2f50b1bd4c83efcd5e5c2718e Merge pull request #1854 from vincepri/sync-cluster-ready
468a17f54fce75c0254c71d6216d22c17e00c753 Merge pull request #1848 from detiber/redirects
e05d0f0c94adea76f07771e52a40badcf268f4a4 :warning: Sync InfraCluster.Status.Ready to Cluster object
fa34da75ea62cc0ec12d286a90219ada20439a8f Merge pull request #1853 from vincepri/kind-06
f613b12ed5f54ec9f42c90c5ac5054991a576af9 :book: Update docs to support KIND v0.6.x
1d36bca691f30b84993f0be813aa860654af9a10 Merge pull request #1851 from vincepri/kubeadmconfig-groupkind
4be3fae7189667cd6a9eb617a86b6a21faac7f5c :bug: KubeadmConfig controller should look at GroupKind when reconciling
7b22d2e3eab4e353d7a94d8e486d82508934287e Merge pull request #1845 from randomvariable/selinux-build
996d98bcd7d8c7e516a163a602faf672a1836ea2 Merge pull request #1844 from detiber/kubeadmControlPlaneController
fc0b6bc84b1fe896c85e0168e5ced4a4411e7099 Update validations for KubeadmControlPlane and add webhook tests
b1d6d4b6a4c0aa5ec2db7d29da0380f7ae24ca26 Re-add netlify redirects for development version of the Cluster API book
dbd90a99ab5780fd06dbf6635ea1a9a2d857e661 Merge pull request #1847 from kubernetes-sigs/revert-1843-redirects
89432e3f5852dccf731aa67f8a3808f2a3e805cf Merge pull request #1825 from avorima/fix_nolint_issues
e535ec105d881791a5827d7ee211708415494e53 Makefiles: Support docker run on SELinux enabled systems
22138292a736a546fbb1710262be50fbba6a64d0 Remove lint comments and fix issues
6ed547bf65fc023f6067da50fc06bed7e898ce3e Revert ":book: Add automatic redirects for the development docs book to Netlify config"
ed1187266438908f570e3e1f640965cca9a65e4f Merge pull request #1843 from detiber/redirects
c58b772659359b4af0d9388d50a7def1e03951b0 Merge pull request #1824 from wfernandes/defaulting-webhook
900a2ff1f6688773ff48dc56c459484f22c21c6b Merge pull request #1826 from detiber/kubeadmControlPlaneController
7950aac2cb81754656fbde2ca1a2eb2b3d1cb177 Add defaulting/validation webhooks to cluster api
08fcb3220264e715a972c66339f91c33ed258cb0 Add automatic redirects for the development docs book to Netlify config
7eb721b3c5189e8fe7840139ee5e74056c2f94c2 Merge pull request #1822 from noamran/docs-error
ef2206b083b2104982712643ee13dee448c03524 Start adding KubeadmControlPlane controller
91efb1d28dcf44d28f10323414f570aaf2d3b434 Merge pull request #1800 from noamran/1783
de29af5fc341cf786c0c04c6f4e0f85d1fa7bb24 Merge pull request #1839 from prankul88/fixes_impl-guide
83e7704690d694b23cee8ed90495bfcbd4213695 Fixes in infrastructure provider implementor guide
cb708b6b6d565424468b493d352f7dcd66daf521 Merge pull request #1838 from ncdc/capd-mod
db1f2be2f0807f55188f3d76d00ebfef9d5579d6 capd: maintain go.mod/go.sum
ca630c33dc68087d8cd86e3b2bb3735607f3e0ee Merge pull request #1836 from ncdc/integration/better-cert-manager-wait
8b0a902ed1b034fbe2347de6723a5bc9c8f1055e integration test: better cert-manager wait
065e0e0cbe76dad75ecb72f7a45ff4d8ad1021d3 Merge pull request #1682 from liztio/provider-docs
8505b278435a9ec6e8c4322393c21f82a0891284 v1alpha3-compliant cluster API provideri implementor's guide
423d06eb5190e07c801343b2025c82cdf617cd2c CAEP: MachinePool API (provider agnostic scale types)
68dee2410189177ce6d50ac05ccb7b5981bc5a1b CABPK - v1alpha3 types
7a1f750f2913002db2019fd344b54bc585087ec8 Merge pull request #1812 from avorima/update_dependencies
85f3e88337259a3336634a5caecf2e45f6ef97ee Add missing preserveUnkownFields and make generate
3f6618c09faac99a36f7d5c3cf95066d13ab4e6a Merge pull request #1815 from jduncan-rva/master
e573c813f710b8dc007230510f78f3f60614f467 Changing ErrorMessage and ErrorReason to FailureMessage and FailureReason in docs
626cfc48d7ba6328b7977fb28341adb05f1021d6 Remove preserveUnknownFields
211bc0dc0c0e438c355102147ce31f1660df5966 Re-generate CRDs
4c9d8702601b0d176f38a7dfc2e71eb8c56892f8 Update tools dependencies
7a6689334d31bf2459c153b4a6b665fb20e5dd19 Update test framework dependencies
257aa4f8ba3c57b56a06b5e5d4acc582cad65b27 Update dependencies
e64b877259a9493f563fff7769e0498122a319a4 adding note about envsubst application
d8d2a8a58d0e4da4a855681c8ee6d38ff5ab4568 Merge pull request #1821 from vincepri/cleanup-bindata
7901e494e0b6b65cdc20df4c84e2b226f667443f :running: Fix bin-data binary not found in CI
2e649a03a24f6c12c4900162273a903c7e97819d Merge pull request #1788 from wfernandes/validating-webhook
9879d3f066cd058047cd89a35264a179b8143b5a Add machine health checking a.k.a node auto repair proposal
4d1e2fb874bef85780cd773b6178ff07773e4d71 Merge pull request #1738 from fabriziopandini/clusterctlv2-api
acf758ac642b3fa8ebb3cb625eab0d50b8a1c68b clusterctlv2-api
b88a9cefa7ef63895bf8619b3c76b8618327cb21 Merge pull request #1791 from ncdc/cluster-infra-provider-spec
62092ef72456f77aaf5a64d27be0c67346040d26 Add spec doc for cluster infra provider
97da628ea7c1954b4ff3cbbd564888acd00eda62 Add Validation webhooks to cluster api manager
14c81fe70f8ca6c6a81d27f56d6746b0f90bb71a Merge pull request #1805 from rsmitty/master
b11b570e06a46dffcaf3db8fd4082e9973134c9d external etcd doc improvement
6b9b7d785129e4934ab6f0bb870a691bf5a94be8 Merge pull request #1809 from ncdc/fix-webhooks
f9f21795f52925282f2639f1562922249f45d961 Fix cert-manager annotation for mutating webhooks
bf92f0709959b07d59bbb76eb5b9a81be4ccf409 Merge pull request #1807 from ncdc/fix-webhooks
af952ee9a012b110ca8a3444c3b408b1e2b49e78 Fix webhook service selector
c37997e37b78169530ac5210a7e4a2430d694383 KubeadmControlPlane: fix validation plurality
44595249c2f9041b59b3e8fc81a1d63e82ef44ee Merge pull request #1806 from ncdc/deploy-kcp
3c00a4f0011141a6066c8be4cd21fe20ff12f91e kustomize: include KubeadmControlPlane
4d453ae8751a389bcbdc2f7bc33c14e09f2381d5 📖 Add GCP provider instructions to getting started
b60e453c1f68600898d66273d9900f3564a94121 Merge pull request #1730 from fabriziopandini/clusterctlv2-cli
74c8cf37de8507f98a977fb2eff2faced72928dc clusterctl v2 cli scaffholding
0f4e6259d42dfec341f2c764d9759a18a1888d5a delete clusterctl v1
2ab0681eb05849f61a58475b0a6848fbe54dd44f Merge pull request #1789 from vincepri/cluster-spec-controlplaneendpoint
86b014131e13c592bb8b6b09483bcd76cf1bbb42 ⚠️ Move Status.APIEndpoints to Spec.ControlPlaneEndpoint
48729fd1380e982d840ebfd08accdaa3e2193bb6 Merge pull request #1798 from wking/upstream-DeletionTimestampIsZero
090741dbd7907945510d8b114681aabfff493e77 *: Consitently use DeletionTimestamp.IsZero
7ef40d712fa65535312d99c87f48994cf8064e49 Update generated files
87c9ead800ae9bbefb7ed520c2cc588a9531ad29 Merge pull request #1787 from gregorybrzeski/patch-doc-clarification
0d4c8cade0c9942d25294313ed4c8939e320f660 clarification of changed requirement
08b29593e201a02a9805b8f839e5e22b789b0ff3 Merge pull request #1765 from detiber/kubeadmControlPlaneTypes
bf2c98ff87315d4ca03572d2d448d59b01f0c902 Plumb webhookPort through to the manager
b11b0d8ddb9774841191db95241b65f75cc67a31 Add KubeadmControlPlane types, validations, and defaulting
31f119ce49479505c6bf9201316e4f9ef6a0361d Merge pull request #1786 from noamran/ct-0.2.3
5bebaf88b8e3e793559527151301a18c8aac9205 Update controller-tools version
ee8f353c7d9a9e9d7fcaf8081425e1af01b1ffac Merge pull request #1776 from noamran/1670
8143d3abe06599e2ad6b690de5c5e1ddcccd4c55 Rename ErrorMessage and ErrorReason to FailureMessage and FailureReason
55635b3db9cf706ee62821f8c3c3c4d2ef426c20 Merge pull request #1771 from jadarsie/e2e-fix
03a11d0af95401ba068f7a9b3559903ceccb3081 chore: e2e framework broken build
ce4ea5c522d511fbcedbc3c8dca3e36a78a40f41 Merge pull request #1778 from chuckha/go1.12
a4367f53d643fa1a6718f2c7b40b7e109af47b5b Use go1.12 instead of go1.13 for the e2e framework
3e9eedb5a24e56ed767cea9ef5e00e9d3d7a7b42 Merge pull request #1742 from chuckha/just-docker
3cc55f7c1b198fa7d183b6813cb300ec601dc6f5 Implements e2e tests for CAPD using the new framework
8fccd103ff0f205a03fb2702f4a13bc8181773a2 Merge pull request #1777 from detiber/updateControllerTools
bc7bbdb3a98952abd6ef2c69f3d1124d15d65e8e Update controller-tools version
80b9d58b6a079236553f5ea67f8950722b9bc541 Merge pull request #1766 from ncdc/caep/control-plane/add-amy
fa6fab8b99edf1709efad2c61eca7c9e5b96204f Merge pull request #1764 from detiber/reviseCPCAEP
baea96d55331346851838f7ad8d971cfc554409a Add Amy to KubeadmControlPlane CAEP
34f7eec6a07f22020c82dd5780db7bfc25c89717 Update Kubeadm Control Plane CAEP - use label for upgrade selection
409448ca3b8f8740b0983ba4e0f81d5186dff48a Merge pull request #1613 from detiber/controlPlaneCAEP
622d56ecdccba311c12a3f1c75ae11aa967f850a Merge pull request #1721 from vijaykatam/cluster_status_apiendpoints
4a481d60efbdae0d0e3e22a326f589a5f14e3c02 Set cluster status phase to Provisioned after APIEndpoints are available.
21b449a9ca5a9125640045fa20b532fdd6a25374 Merge pull request #1763 from wfernandes/document-metrics
6f5d51f78e7ebc3733f6312adf842cae65d3da92 Add documentation for metrics
663abe499eda1db6398832fb819f07179e609563 Merge pull request #1720 from nader-ziada/not-ready-node
c28d769f98f2a6624f6651cc2eef3190504b4a87 Merge pull request #1758 from antoninbas/fix-typo-in-glossary
81008c1f098487ee1ff653e03e02dd0aa6342cfa Fix typo in the definition of "Immutability"
4e80364012b808578a41fd761ff577349a2b4eb5 Merge pull request #1736 from wfernandes/metrics
2b72a3a53a7d2ecdd85244f346122a3f63ebf59b Add metrics to machine and cluster controller
27cc5ff947765976aa20607b5b35f9865c3801c7 Merge pull request #1752 from 1060351485/cluster-api-1750
973fe35bebe53b63c391e84f83ac81b93a5f6763 Merge pull request #1737 from chuckha/just-framework
b8a6e04f96927187453d8e9988b1617904272d73 update provider_components.yaml in Quick Start > Install Infrastructure Provider > Docker to provider-components.yaml
c28007c3b36928bd77be143a61f8d12cf04e8edc First pass at implementing an e2e framework
52aed197b43ab9ac8fd2d404b21851814c9b02d3 Merge pull request #1745 from oam-oss/ali_cloud_provider
8334d5bb80c3e6e007ace23777cf7199a35b8207 add ref to alibaba cloud provider
42eea5f5a5d569b44c628b8c9f1646465f244c10 Add ControlPlane CAEP
53cf1488183e0606e7d791c31cc0417241c55281 Update the machine phase to provisioned if the infra is not ready even if there is a NodeRef
86c86080fc55577960c83d68f24df385e8e1b476 Merge pull request #1688 from vincepri/md-ms-match-labels
36cf145127deb2c43b3e4a4180c13b744ee55b6d Auto-select on cluster-name label in MachineDeployment and MachineSet
685e7dc391996d30120e0139a85bca18db0cd9fb Merge pull request #1734 from CecileRobertMichon/azure-quickstart-port
90b4b20b83848fc58fed82a7ace9fa8b9e34ba42 📖 Add Azure tabs to quickstart book [port]
6995b336344d9bd5bdcf9c9fa1b2ea588785f732 Merge pull request #1733 from CecileRobertMichon/quickstart-port-forward
a50ff57d536bbe5a26b056ffe7e55b6d113fcc46 📖 Add MacOS instructions for CAPD [port]
f1f6030607a939b2e833f97cba84f8bca3882271 Merge pull request #1709 from tahsinrahman/fix-iscontrolplane
66abf9c65fe08ac0f2236b3ca6ec4fef369a38c3 Check existance of MachineContrtolPlaneLabelName label instead of value
9b14be0a06892743f7ff494ad307161974386f85 Merge pull request #1633 from noamran/1606
0f34af0a8bceec995dc46406c09bad7a4fcfede2 Merge pull request #1711 from tahsinrahman/add-ms-md-label
e9162ab88d8ebdae6f791a0538dcf53b7e7549a1 Merge pull request #1558 from fabriziopandini/clusterctl-redesign-proposal
5bfb8f559c04c3e80e3605bc6fddf1a1a93d5c9e Merge pull request #1571 from chuckha/caep-test
7ae96c283375e6404c289269a537425eac0b38f7 Add CAEP for testing framework
e1539fc97d81b0aefdba1ad83ca866575c647b11 Merge pull request #1717 from ashish-amarnath/fix-shellcheck
e4d321add654f57fb0809fd570ca16248a3c9306 🐛 Fix verify-shellcheck to report errors
c96c5c60017a63e49a4a116491e7d1b90f0efefa Change remote.NewClusterClient to return a controller-runtime client.Client
f869765493749d60c4e75afc59e7ddc3bdfc1c2e Merge pull request #1698 from ashish-amarnath/unique-kc-admin-user
b84b21e56e52fd901e9b65c48713c88b1f0d00dd ✨ Use cluster name for admin user in kubeconfig
9455dde6cc9bc0097ed0f7a5a7939f2502517327 Apply labels to Machines if they're part of a MD or MS
6f77ca5bd69611b24bf70f79352eabe9afe6ba5c Merge pull request #1710 from vincepri/remove-certmanager
f380bc7bf263d32f3411f60fbb2629d0b3a817a0 Merge pull request #1707 from tahsinrahman/cabpk-concurrency
e0fb83a839b2755b14fbefbe6f93db9a58c76952 Don't ship certmanager with CAPI
3ec5e9c587989f20c4e137330ee72aea765f7141 Merge pull request #1708 from vincepri/followup-certmanager
f37cae49d73db0791f87b2fc109111fedcbb7d30 :running: Fix a bug in certmanager/customizeconfig
166b4e47d81fc181ae11c357cc19ec5d4cbe525f Expose concurrency flag for KubeadmConfig (CABPK) controller
e6804f3272bc9dad0727e6be155f8a175b8081f5 Merge pull request #1706 from vincepri/certmanager-v1a2
157e4ab61fce760cd8beb0005011fcc094a78241 :running: Update cert manager to v0.11 / v1alpha2
d22b2effdafe55c7883165ddc106ed0318b8f6c8 Merge pull request #1704 from vincepri/bump-concurrency
133c7e84848248511b6236041a300ee8120bc8cb :running: Bump controllers concurrency to 10
00c0ad779268edac23ae8345959481aa22190117 Merge pull request #1700 from prankul88/update_shellcheck
de8991562dc3c012c75babcf33e3a28f7cfb04d6 Merge pull request #1699 from ashish-amarnath/no-nolint
414d95b75d580a522387e62d262d5cda966aa1e9 Fix shellcheck verification
412dce35795ecda6ae57751931c7f9adaab163a4 🏃 Remove some lint exceptions
3bed0c55bd8ff66538b485ebff675bf4c663bf44 Merge pull request #1694 from vincepri/simplify-makefile
52e5ec01fd4b52a8d7503fd93d2b99f2936b5790 Merge pull request #1445 from juan-lee/clusterctl-delete
30b81ea4fade869c4d064fbd70356dd479e5365f :running: Simplify Makefile test pre-req
24a1f812924cfac9ab6a5febc39b0e3232a4fd85 Merge pull request #1683 from noamran/1681
2b37b514deb85be52edca4ebb936e69c2437d979 Adding release-notes to the Makefile
8943fa9ba40c028183c54453d5c18c91c948ea45 Merge pull request #1678 from vincepri/remove-restmapper
8c9d6a460505026bd26519bd7c56dd696fa9718a clusterctl-redesign-proposal
fc8ccbbfffeaf2b8fc269e6f30a0b2022fafa98a Merge pull request #1673 from xrmzju/cache
742efb2fad53492f26a8752654e235288ec165cd use a client reads from cache for controller manager
731ca09eb092423e5e8a720fd1fe8a0f1df7be4a Merge pull request #1679 from vincepri/kubebuilder-fix-tests
5e2e006fed48cef45a1390579acf40425b6504c9 Update kubebuilder / k8s testing version to 1.15.5 & fix tests
cb0b57f84c570814b8a1df792eb82b8fb0f4d1a3 :warning: Remove util/restmapper package
7816c8704184b0243ca8c23f93f7bdcc8dc27f79 Merge pull request #1675 from vincepri/remove-limits-requests
f4391c5ed335c5573bbd5a67a2bd59bdaffe114f :running: Remove limits and request from manager definition
16f014fcae670f0f9d977f27a103828a16cb8079 Merge pull request #1661 from sbueringer/add-capo-cluster-api-book
eb0989956e5b6495533e1cc60147662f2eb798df add CAPO to cluster-api book
9558133d39ee6eae65bfb1a04e26243a441c3715 Merge pull request #1671 from andrewsykim/vsphere-quickstart-fix
0806427a84811f59701d57ea5c676b8bdf124017 use Kubernetes v1.16.2 in vSphere quick start
8a91058335cdf3d36fd2bc551591efc73ddcc6dc fix vSphere quick start installation to use stringData for CAPV manager Secret
4e878af0247adfcbc8c06fdcfb627bd0abd75851 Merge pull request #1669 from nader-ziada/remove-cluster-not-nil
0155dee13bf5395e2fc811745089bc738065a607 remove unnecessary cluster!=nil check
098155a9501c2b685be7f2ec114838cea1a3220c Merge pull request #1652 from chuckha/capd-release
c4a34ebedb8c4b8da5462e7f38447afb83b8f021 Update CAPD Makefile
daffbba1942e22cdb8411cf3cdbeae412ab821db Merge pull request #1660 from liztio/devdoc
a67e92088acc083a29f016cc5dcfd5a6b5abae9a Merge pull request #1664 from gyliu513/vendor
57600690ee3b6e189a3421ed89b971703924bb4f Merge pull request #1475 from andrewsykim/vsphere-quickstart
3a9008d763c1a980e713c6ff4df224fdc4aa8134 Merge pull request #1650 from ncdc/delete-cluster-wait-for-all-descendants
a193a179a38dc32e2c01e2722560131c65497ff6 Wait for all descendants when deleting a cluster
5c04fd3392179186dff3a20b353eb8faddd56872 Update docs/book/src/architecture/controllers/machine-set.md
acdda944d6d8074fa028bf6061bdb1f3ed38f6ea MachineDeployment docs
7cbc7fc34f4e45dee69b181ed26df17c0f77a542 Ignore go vendor.
f7e048646ae89c6e0ddf755c3760f233017386d9 Merge pull request #1645 from wfernandes/kubeadm-import-package
ff1d3cca6abf55d1f13bd5ca80e76adb17aa37b2 Merge pull request #1659 from ashish-amarnath/fix-capd-build
3739b6e9785ad3ef0f11dc7194326d51fd7d9c57 🏃 Fix capd build
da7dbb54792b490b5b08cb70142457a123dd7c77 updates to vSphere quick start based on upcoming v0.5.2 changes
6ad51f9fd4f91e61644c4b620992b4665cfe5306 MachineSet Controller documentation
96c783e392e5b82e3ed63423cf0113d677a478e7 New plantuml for MachineSet controller with Makefile
e3bfa1cd26212e0ff3d8f456badd2b57287a3a5f Steps to build the cluster API
61975b4696700ae0979990c807386ecb3fa362a8 Merge pull request #1655 from stewart-yu/stewart-bugfix
6aa25e056ea5a4f21badf00cd3fe362893515008 bug fix about pointer
297bb7dc5aa5645ab1b18d2bda8986f19c2454b9 Merge pull request #1648 from vincepri/proposal-template
217e86c182de8e26c2339a4b436c8509b6a1b43a :running: Add proposal issue template / simplify feature request
09cf13543984b9b88724ef27c441297c0e7aa1d0 Merge pull request #1646 from ncdc/increase-test-timeout
0c252b1ae6ec26a99abddf21bc92c4e7012bdee8 Merge pull request #1637 from ncdc/docs/library-stability
fd04b2bb9e670840c734c9aff06a6d3338df798b Increase timeout waiting for machine finalizer
b3004ab3b00f0f65c83ae29c7bcfaf56f39147d7 contrib: doc breaking changes
f428b39ce502a76122c831664172364a51e416e4 Rename kubeadm/kubeadm pkg to kubeadm/types
bad33a82c9ea5fbef94216103bac48515beea32b Merge pull request #1641 from aaroniscode/aws_iam_role_fix
a2e2795d853b9c3b34f9137d698a95a66708ee85 fix the quickstart AWS iamInstanceProfile
9d21be11e3505d10858f14d4ac7494a9cf122505 Merge pull request #1638 from ncdc/docs/remove-node-controller
fe6387e16bb32b7ac3a7159184b5f0b8b4ca415b Remove empty node/noderef controller docs
3456552501cedf276b400aa07830f761b695c535 Merge pull request #1635 from detiber/updateDrain
1c4357a35e3698d726b024bc0b4ca7774a4a2488 Update kubectl drain library
5d0462c124e1596e43c35f8f0463b530363fd7f7 Merge pull request #1400 from tangle329/master
84f06d7f6affcc2d94f2a6eea6a8917c0b19e4ba [machineset] Change ordering of template cloning to clone bootstrap template prior to infrastructure template
a767ac6e740d90c989c19e6099260ceace1d148f cleanup infrastructure configuration object after bootstrap clone error
6d41ae2513be29b071e41bf20990bbc989702298 Merge pull request #1634 from liztio/outdated-capbk-readme
d6678a7dfb9c4f2fe7118b5a373a819787a221a5 Remove outdated README content from when CAPBK was own repo
4a097d8e8d33ffad6e61883a21cec365728e88de Merge pull request #1621 from ashish-amarnath/add-shellcheck
01585c2dd8a6aa9093b64d192720f54f3c1f68fc 🏃 Add and fix shellcheck errors
6e55a31cc976205576f7cb716bba54e4b00cd144 clusterctl only deletes the cluster object
67d5048f4cd886c8a15cb76445fde1efffe6ed08 Merge pull request #1628 from ashish-amarnath/cabpk-unit-test
9cf693998ba0ac04d9cccccaa9b1052c53eb79b3 🏃 [CABPK] Add test KubeadmConfigReconciler_ReturnEarlyIfClusterInfraNotReady
7c6793da18919be9569d3116742fd1b6b9e197c4 Merge pull request #1624 from randomvariable/glossary-stacked-control-plane
bd254663e668c45b8de8db7e117fb61d6a816242 Glossary: Add stacked control plane
d3140bacceea81d85da9341a591bb87e0ed2d008 Merge pull request #1548 from liztio/conversion-hook
fcf63ec8459a2ad9e303958431e20362906554b7 Merge pull request #1620 from ncdc/forward-port-0.2-clusterctl-namespace-fixes
417ad77188811872771bcdb0b8f039fb5e433eec fix clusterctl pivot, update moveReference function
0642e8585986f38ff4b7be5b21356f33c5893f0e clusterctl create command namespace fixes
09d44611a3913f184e4c02c922b96273881ab86a Merge pull request #1619 from chuckha/cert-manager
55e5582fd2f750fdc47abee5f498bfab8eb8b135 Adds a tool to update certmanager YAML
b01a13ef030f12c71a35cd5bb4a179469e4448bb Merge pull request #1617 from chuckha/capd-fixes
b0df81e51fd5f5286fe3c8c6acc39cc313dac58c Conversion webhooks
4a89614718587c391dcbda8b06db906e254950af Fix CAPD build and Dockerfile
6c50054305c8b5036f15a809555827d8cb67ae0c Merge pull request #1615 from noamran/1547
41002505eff2aba6ae59aa51207ec0c8c1948f37 Conversion v1alpha2 <-> v1alpha3
56b8c0b8072fbf997c462bd4ac92983207ce7c1d Use Spec.ClusterName to get the linked cluster
0da8bded303aa68acc3eb5fe29d49cf4cba7abb9 Merge pull request #1614 from chuckha/live-update
7852a2c4306dec46a920e2ec9dd59a7cf730bc92 Add restart capabilities to the builder image
46a00a37441b42419ce38408bef0da5ac93fa17c Merge pull request #1601 from vincepri/fix-rbac-issue
bc8334791d089351b1457a99df1ea215197bcd65 Merge pull request #1611 from ncdc/debug-tests
b02a6dfcdd3fefb0019698f08594e80bb8662fc0 Speed up + debug cluster tests
fff508673f1620d327c65137fc9f00a4e9b2ea2c Merge pull request #1610 from tahsinrahman/enable-gosec
2734fb65ea19f9955bb3f996a459c7ec43006c53 Enable `gosec` linter in golangci-lint
2b01b82b380f6fd1eb72886c0a6b893cb9a92a57 Merge pull request #1608 from tahsinrahman/update-golangci
5ba17ea4973a83c88c65a36a534b1efdfe4792da Merge pull request #1605 from ncdc/fix-bootstrap-client
8a45bc8c5686599ec91d88b4057e1e28aed4ac81 Use remote client for bootstrap tokens
20c9dff58100fe99ddbb58a23cb9aa3609064951 Update golangci-lint to v1.21.0
9efec86053ff37ade997d40c750fc7744a6994de Merge pull request #1607 from tahsinrahman/remove-util
3ecf638f982cae510acdb44f1431e6cb2646bb70 Remove init from util/util.go
9bb9187fc711eae667c1ad0bb7803214dcf63692 Merge pull request #1603 from vincepri/readd-ctx
d18a9741eaa3706e2a01e8b5addf54198fa0e4d5 :running: Re-add context to reconcileNodeRef function
c22abe8ec6f917bf30c8e39884b05503f6098f95 Merge pull request #1556 from tahsinrahman/fix-golangci
399b37eaab1d642997f575bef862fcf3b912bd63 Enable golangci-linters: scopelint
f93b579abf455e43003d4ccb9464afe5cc8ca12e Enable golangci-linters: errcheck
f438fe6ea313cfcededd0a8c4a28de5a752ecfbd Enable golangci-linters: staticcheck, unparam, unused, depguard, gocritic
f51755915b4800d96f1644b565f2f63771de89cd Merge pull request #1570 from vincepri/set-cluster-label
12467ffebfae29daf5345ec7e11f35ba29e75401 Merge pull request #1596 from gyliu513/capi
09445bba527f1617880bdb6c427d8a507863b63e Merge pull request #1593 from noamran/1591
e901f30c6509b0fe080453f96044c1c3c38ba1d4 :bug: Generate manager manifest including kubeadm subdir
4e9ffff7573bff6ff9a145ed170eeb974b4e1954 remove command single quote
3abde9b41307ad868993cc6f7efc682146d4bf08 Merge pull request #1595 from tahsinrahman/fix-cabpk-client
382f976d4099d29d255e7c5678361e693d48b947 Set cluster-name label on external objects
6069b94654b350b5ee1dc25850751f6e6dff40a5 Added ibmcloud to glossary.
2dc84ff2accaa4a9604e007e91b40062c3137275 Do not use embedded client.Client in KubeadmConfigReconciler
cc2a737a2c371c802491c81e5afe14cdb0ec8756 Merge pull request #1594 from tahsinrahman/fix-cluster-label
9d1c04708a4918ba692732165da8b9cacafd857c Use controller-runtime client everywhere
2caa2d89ae504f20044c43e8ecc58f1b0a6e133a Merge pull request #1456 from tahsinrahman/fix-klog
a8ef35df8c8e6a993769673f84befa9d51a67d79 Rename MachineClusterLabelName to ClusterLabelName
b1651ae01990f52d62ff88185d7f00a8b6eb9b20 Merge pull request #1520 from nader-ziada/md_phase
4ee2782552e6c49a89e105c43f6fc46450523d8a Remove klog calls from controllers
b7707ce9b4d80c26a554591017bdae3f2498e0c4 Add phase to MachineDeploymentStatus in v1alpha3
b24eaa99d112089af532e7c374db133ea6cb9009 Merge pull request #1511 from wfernandes/add-machineset-controller-tests
165f5792ffc763969a63dda18d81dea9ae9e64cc Merge pull request #1573 from rsmitty/docs
faa482ae4b86dfdd56229e1a1c301ec17176b16a Merge pull request #1572 from chuckha/upgrade-process
aa6d0f0a42281d43b47a5b90f6558314fbca6300 docs: move talos from infra to bootstrap provider
ad2a3ee0d962d323aab1c5f59d3a3033cc41bd35 Adds an library API change to v2->v3 document
425c2197400d55f74d7162ee30b1efefc436a428 Merge pull request #1494 from chuckha/release-doc
e3ababe39dfb9ec30086f5ea2da0513394a53996 Merge pull request #1564 from vincepri/document-v1a3-changes
b14343608489bfb249964527742bbf24a230df4a Add prerequisites to release instructions
f4ab0a57b85460a59c412405c119974a2d5e494a Merge pull request #1560 from vincepri/forward-port-1484
5187feb3338716c282ea5272b16d553e84b48491 Merge pull request #1563 from tahsinrahman/fix-clonetemplate
8bc6fb22dcd8f24eb754064ebd16f09439b66030 Merge pull request #1539 from vincepri/cluster-required
595da123988a5bbd04d87289e3794fb445914138 :book: Start documenting changes for providers
1cdac551aca521799d8dd94d86ece122b40c8629 :warning: ClusterName required on Machine/MachineSet/MachineDeployment
40a3cb6b72093a6d888f53e8256fe07ba93f144b Update module dependencies
9853a1c1a7673f824c1baf870136a850d06e965c Update generated files
d9e09a7cd5343e6c4d296daa47db40e56b02d4f2 Merge pull request #1545 from vincepri/batteries-included
79a71b8f69991e2f47316a1b968e72e7525afeac Use context as first parameter for external.CloneTemplate
d5ebbdd5c9d048c96e81455ce257db60dbc9df8c 📖 Add quick start for the Docker provider
23a891785b60dcdc3bf1775d6ccfc100d9ab9d54 Merge pull request #1555 from tahsinrahman/fix-external
94f8cfa757bc29e3937e75c73010f4e38db675f1 :sparkles: Ship CABPK as part of CAPI
214c917acb802d98b336ce4b4dd1afd886d46c3b Use context.Context as first parameter for external.Get
6ae7aac4149c2f34f7bfadcc291309115a623c67 Merge pull request #1440 from Nordix/APIEndpointPort_as_int32
46a78e72c177e488baf2bc4f69d4761d3351e71f Changed APIEndpoint.Port from int to int29
94c87eeb4d410f73f475bf89150e915cfbd2461f Add unit tests for machineset controller
b23a29efb5bb2c9d14288b4f4d8c30b1b4289e0d Update module dependencies
dd2e52b24e7d4645a3e2f807775e09d42e6742f6 Update generated files
031bbd88170202aaa7d7f690b60423ee5cb096ba Update Bazel
1dca5eea774a41c15b7e33521573bd507e3875af Merge pull request #1483 from chuckha/cabpk-merge
3b732352ac3ae02038245b85b980425a2bfc3ca9 Rename module
1534aac10487f214434c014d6614ab5c6182fbb4 Fix OWNERS files after CABPK merge
941019f22e0d044cd3084d9ad2b9c2aa285d094f Initial commit
20da46b4c73cc64c90ccc355b21d20abb4daf8f5 Merge pull request #1531 from wfernandes/add-machineset-ownerref-unit-test
c01a8fb1be5c9c8c042d31d0cf184eaec12577b7 Merge pull request #1532 from tahsinrahman/update-status
a1e84b5b0f65c15e7090efc9c0d7fae570615d13 Update Cluster and Machine Status.Phase values consistent with k/k
76d0947153d85d53b6d69e4e1156c396f1613b6a Merge pull request #1516 from tahsinrahman/add-cert-manager
286a66f38106ab6e05fd568d0d59481e9828e8b7 Merge pull request #1473 from vincepri/add-book-reviewers
d3e2e807ea7611c9f5b1fb8aac995995f26a8484 Add OwnerReference unit test for machineset
86bc5e462f792b74bfdb1cdc2da60fa407786001 Merge pull request #1529 from chuckha/remove-dockerlib
6c215922190350b099530c73167d2897844a4826 Merge pull request #1530 from tahsinrahman/fix-duplicate-scheme
1ec0f08de2a87f6ae582acaa3f7c3f096c8e49c7 Remove duplicate add to scheme for v1alpha3
98553a67e156ba379276c71ce86c550e065b8314 [capd] Remove dockerlib volume mount from CAPD manager
3d9baf3610ae90781ae85fac4ef8622d35378c5f Merge pull request #1523 from noamran/1502
ff678f6ccbadba9286461c31b161616f759262a0 Merge pull request #1485 from chuckha/single-commit-capd
aa3d2c200147e18e1bea289b428037d0c91bcda0 Creating v1alpha3 API types
112951ee033dc182efd061302ac600fbb6107de2 Merge pull request #1512 from tahsinrahman/remove-v1alpha1
44ec2138173d5a5a80504f9be6be1cc520f9dc46 Remove all v1alpha1 codes
2fa1614805d04986390b43eb9abf4afc8855ae7e Merge pull request #1519 from detiber/updateControllerRuntime
ba392bbf3ea0058d2a7125caed89e288261432d1 Update generated code
504fd7e16ce37eafd127479ad2634562ad22bc12 Update controller-runtime and golang versions
6d17469ca028bb8b91a1aabb19606c04203dd9ce Add cert-manager
7c427f9d7870c1ec168908ad95c6d3575e3dd49f Merge pull request #1517 from CecileRobertMichon/add-io-timeout-err
5d9ee5203c1de347ff75c5b3d43edde6b63c33e4 🏃 Add i/o timeout to retry errors to acquire kube client
30869b7469a60fabfd6ea641228543819dda0d60 Merge pull request #1515 from vincepri/followup=1096
651d7ce268e5249d9e4fb0b3eceb76d59609828e Merge pull request #1318 from moshloop/master
ff3357dc454a7c44563d31ce3f4a737f56f000c7     	📖 Updated docs:         * Copied over some concepts from glossary         * Added certificate management page         * Move abbreviations into glossary         * Added bootstrap controller         * Coped some diagrams from CAPV into controller pages         * Created standalone installation page         * Moved quick start up a level         * Moved clusterctl to references as per docs.k8s.io
b651ba4efe1c4f184350b0ed6e5bd2ca87d17823 :running: Address 1096 PR comments
d56415d2e670e4296937d91275bda62260cfc133 :running: Move external code under third_party/, in line with k/k
3dd3506005c5d43cc1c4ca231a29bbf9aec5ceaa Merge pull request #1096 from mgugino-upstream-stage/node-drain2
1ec39a670244f9ea46e3a5dac9512a506ec4f5a6 Machine controller: drain node before machine deletion The node draining code is copied from github.com/kubernetes/kubectl/pkg/drain (at) 75fdf29ade9e535ff5801a9321d55d1adf6a996b
396c6fcc3ecc53afe3489be12e2bdc5dedf58a27 [capd] Update go module name
17e038182bb434c867219df2988b9c4eecb23932 Add header to Makefile
36d67cbdb9ad56851b0f64083e2ade3676eab569 Remove extraneous files
66c1f64f82355a86fd20024349caa828f7c9cdd8 Fix OWNERS file for capd
e7994d4cdcffae5bd5cb04ce00e10e73463b2d30 author Chuck Ha <chuckh@vmware.com> 1560208528 -0400 committer Chuck Ha <chuckh@vmware.com> 1570720504 -0400 gpgsig -----BEGIN PGP SIGNATURE-----
3914739796f6688e8742329b747e4e7f771b4389 Merge pull request #1513 from vincepri/build-master-tag
d3f450d4f91008498d9acd26366b4502c4a8d1a7 :warning: Build `master` tag on master instead of latest
0b70358551c437ae7e695a207d438b903276c601 Merge pull request #1501 from vincepri/caep-proposal-v2
986adb47f82ec1f95c6a0207554100a4d554be35 📖 CAEP template v2: expectations and timelines
55fe3cc857495c86b2a193885ff89c7975ef0113 Merge pull request #1500 from vincepri/ignore-pull-policy
7dfbe5242b78211a858773e3adc90bef27a630a7 :running: Add manager pull policy temp file to gitignore
b470a7425510a2dab1017cc0f2fb6bd63b7ba20d Merge pull request #1499 from chuckha/machine-doc
79fa40e6095a981cd96710b941ac5b5eec7dd86c Improve machine controller book
fb2a8a81965b563c379ad75571d45f289f51fb38 Merge pull request #1498 from detiber/fixHelperPackage
0f08a8cc587ef2609d336f171429fd86b8a6fe09 Fix package for test/helpers/components/common.go
1b3dd72c277a22aac7d3e80bcfe8b32fd7654743 Merge pull request #1497 from detiber/gomegaReadability
9b17b2e89cbccaa031b174c0355dad569ca98447 Cleanup the readability of some gomega error checking
aa86af24657672ebca641cf7c76da7eb305faa39 Merge pull request #1493 from wfernandes/add-machine-controller-tests
73af52bb076dd0a6b8b85a1b88aef75cbbb727b8 Add unit tests for machine controller
839a3c21d31b7834da83cbad2702e665e7f07160 Merge pull request #1495 from tahsinrahman/verify-codegen
65228439acba58a5ee0bf690b1c1420663332bb5 Add rule to verify generated codes and manifests
7f1890e4ebd9387491493b8018470b1155bba018 Merge pull request #1474 from detiber/commonE2EUtils
fe3296925b39d60e18663df309da88757776d694 Add helper utilities for testing
cf29f37d64484acba49c563f5dedcae5880c3a21 Merge pull request #1492 from noamran/1488_uniqueID
4b41effa13597e2f7ed3090929ca30d825780f64 Setting unique LeaderElectionID
e88948c1f4c07a896dd72af0d272ab71a5b64580 Merge pull request #1487 from andrewsykim/tolerate-manager
b149185e0d2925af9920ad48e0960d66f180680b add well-known tolerations to released CAPI components
6a0574cc431266f1b41b4599ed1303f356d377ad Merge pull request #1466 from tahsinrahman/requeue-only-cluster
102d4f33e6663ee95cc5a6b3dc1009858765d423 Merge pull request #1479 from wfernandes/fix-cluster-book-doc
8c2a90d54de83a32d0b6a791842415a3ea3a4ec2 Fix link in Cluster controller doc
a6b5ba419bad1af4ec9f294720d5c61eada297be Merge pull request #1476 from keleustes/outofdisk
388257619f3dc01eccf9dc331dde8a6a5830d3da Add unit test for `reconcileKubeconfig`
25b6af7de805762138b2f4c3d44a2765e91c1336 NodeOutOfDisk conditions removed in Kubernetes 1.16
fa022bedb9169cc10b2d73296daf7bb5aad4ebb1 Do not requeue forever if only cluster is deployed
1b49d6fb894671ba7f4eed45a9f1a0b0dc05a613 Merge pull request #1472 from vincepri/embed-aws-prereq
fa7274016cd4a15cacf124217e09ead4f0afa334 :running: Promote reviewers for docs/book
83a404878d62df40a4b545cc804e0fcbb4c2d37f :book: Embed AWS pre-requisites document
cffe2d14ecffc24bf82fcc310511cfbc560b54f7 Merge pull request #1391 from chuckha/machine-doc
c27acbda947cfd7e151ad2ded00980f569c0ca60 Create documentation for machine contracts between components
3046e2f692410761eeb3a8687e80779d21b3e496 Merge pull request #1458 from Nordix/bugfix/infraObject-deletion-Kashif
c62129cae2a266fe22ba9eda3f35431e37ebacbd Set Machine Error Status if infra object deleted
bf790fc2a53614ff5d3405c83c0de0dd3303bb1f Merge pull request #1462 from wfernandes/fix-api-conventions-links
c124348ca703fcd826a36d0b85faa0ae19ee861c Merge pull request #1467 from vincepri/bug-status-patch-helper
dc1512973e0fc34b36fca6892552e969c2688154 :bug: DeepCopy unstructured object in patch helper Patch method
25bf0c06cffb305ba75206e5dc9c1f4e8af8f263 Fix broken links to api-conventions doc
0ded052baa49094cad0f6b2846ae39fd60ae7fc5 Merge pull request #1464 from vincepri/fix-patch-external-object
ea238975bc49091f2778dc0fea8e9aebdfa0fa21 :bug: DeepCopy unstructured objects in helper before patching
d6f32c7b642366337868197f6dcdc93c564a1dfe Merge pull request #1463 from tahsinrahman/remove-unused
3ef94e1a2fefccb1f3c2524d8cf1d00e3990ce11 Remove unused function `isScalingEvent`
16a5738adc030a890481b715d305729e521d853d Merge pull request #1457 from vincepri/fixup-additional
24f642d6afb91c3e3a90fe53b2cc8e7713ec940b Merge pull request #1425 from alejandrox1/rm-redundant-check
deb4790c58b8278ff7565b241000b0769d34e956 Removed redundant OwnerReference check
5983d67a403c8cc8181cec6328b0dde2489d0fdf :bug: Fix reference to PULL_BASE_REF for image building
6fc621a1c6af7f9265098b554db344ecbaf2700d Merge pull request #1452 from tahsinrahman/fix-delete-machine
7f82f676284ef969e0da060bf7ff18bffb8cb2af Merge pull request #1454 from vincepri/fix-objectmeta-comment
872349bb258f4d27ca896d110eb7b81ccf29d54b :warning: Clarify Machine.Spec.ObjectMeta use in godoc
a396f028214cc0f63588d2b0e29ef2e625113161 Machine deletion: try up to 10s to delete the Node, then move on
90cbdd174b1753926e26ef1393356d030139e176 Merge pull request #1453 from vincepri/remove-todo-ms
da6a1d75f4054258b8908b21133925ebaec02ef2 :running: Remove for machineset concurrent delete calls
ecdaa4ece0647040a5b7746f44d6f5e7e0a728cf Merge pull request #1447 from vincepri/tag-branches
92ed320763bb9b6cf5a270d1e90830e27414a9e5 Merge pull request #1449 from vincepri/fix-css-table
cdc5ad7354d31f193dcc27bd4c9262486b04fa86 :running: Fix table CSS
7fa35caba1ba0c1696a94e06229c9202deb4fd33 Merge pull request #1448 from chuckha/caep-template
b67aa05a983bfcb1f7e20900fd03597fb4bfa947 Remove confusing langauge from CAEP template
ee32d7eeb648a9d20deebf0fbc68d6556fbacb8b :sparkles: Tag branches or latest when building images
122e6051bc36e19eb8116b063d1ceeee5d1d26c4 Merge pull request #1409 from chuckha/maintainers
10ce53a10c8258469e1d42cfce9b3ecb9b2fe8c4 Merge pull request #1443 from tahsinrahman/fix-go-mod
b0e9d37385f9c93c4422b74fb3c0f456637188a0 Merge pull request #1439 from wfernandes/master
7e3152db08818a5934cddcd001865dbe198be6d1 Add deprecation message to clusterctl commands
69f98cc970b6095f904768f7b6227bc3f7eac183 Add go mod verification in CI
6258ff3ae2812b25b5988938a3335e8331e930ce Merge pull request #1437 from kubernetes-sigs/vincepri-patch-1-1
3e064b3c6944b09b0f8a5826df9db7e48c2d9edd Update feature_request.md
1a6ec9eaf29129418967d78077f9eb851cfb427e Update feature_request.md
9855b1cf8a02335261d75d31ec563f25b15aff22 :bug: Fix the issue feature template
da6b992616f49ec9c56b9e366a9024ef091861b2 Merge pull request #1435 from andrewsykim/fix-secret-pivot
8b06770322f0834fd89c41e2f1f2c7ef06f2f64e Merge pull request #1436 from vincepri/rev-deps
60d8231440c7c56bc1e542a8d6618da5b6ba8b92 re-apply secret OwnerRef on pivot
51c72f09da4eb81e501f62df8a92d1e0d8f3035b Update generated files
833ab4534bae9a127a9396b30a3fa5baabc9804f :running: Update controller-runtime@v0.2.2 and controller-tools@v0.2.1
5f781b2d51bd60c386ec21a0bbeef1dc3702d252 Merge pull request #1434 from timothysc/issue-templates
a8bc544d4d2a9d300bce8cec4f5e661a948c3105 Update issue templates prior to v1alpha3 mass submission.
427fc72b736e5d7b095d773eca75382ade366513 Merge pull request #1390 from chuckha/cluster-doc
fa96a1dcc40042d68c4b96b7d9284e2b4f2048a7 Adds a cluster controller document
2c4cbfa482d3bc7857333aeb1a0eb0599e2320bd Merge pull request #1432 from erwinvaneyk/add-cabpk-abbreviation
12d403d41df36c84201d6b7e7d996521b9c98fa3 Add CABPK abbreviation and v1alpha2-ize other abbreviations
2b0b75ef2cc54453b5258ea1bcc9876950b3967f Merge pull request #1424 from alejandrox1/docs-release
6128d8d232b3aed312259b6b730e4002c69e6cac Merge pull request #1430 from vincepri/fix-ms-adoption
be14d06870ab33a928c0e95726520c3b8dcbc4fa 🐛 Fix patch in MachineSet adoption
44491e485ce206f8e5203f858e9f8672b0763168 Merge pull request #1426 from dims/better-wait-for-the-control-plane-to-become-available
862a0a458643eb44fb768f6712940f026f675f5d Better check to wait for the control-plane to become available
a16446fc382bc60428c77df5a61d19d31400a95d Updated release docs
9bb49677bc1d8cf97cfea09d1cb0dc3b6d8fd230 Merge pull request #1417 from tahsinrahman/machine-cluster
03abc642adec3e7a0cde45e5496f667a413f35ad Make getMachinesInCluster a helper function
0e2e9fa8f27144b1447688b0a59b912b7edeaccd Merge pull request #1420 from vincepri/releaselinks
b6c9d1751987d6eba6d584de041ca1e3467aac1a :book: Automate the release links in mdbook
5cd7261c53109d1af832c2f26eb969cfe4b8e9a0 Merge pull request #1411 from tahsinrahman/secret-ownerref
a15c012acaebec2a5bec0d6d50304ce4e492586a Merge pull request #1415 from tpounds/golangci-lint-v1.18.0
18a5daa427b0e503a4caab22c4ceaecbd083fae2 Remove the Secret's OwnerReferences before pivot
f3c5735ee50b30a792bcd160dc008fe201575ed0 Fix max reported issues per linter options.
d9e04d46467a0b0334295da0424eb49ea6de047c Invert enabled/disabled linter configuration.
161ff622b3966d74982289005971f704843ba8e3 Fix gosimple warnings.
cb5ae72e9db071c5bf10a6c0f44ee992091d6ada Update to golangci-lint v1.18.0.
1d7c4b90564bea3aa3e9126ac2aa915a0631a95f Merge pull request #1356 from tahsinrahman/cluster-status
fba571db15cdc2a4a9abf33a775faa196a1e0a8a Update status.controlPlaneInitialized from cluster controller
fc4f55e0af781b9552c3a83e715d1ee912e0e764 Merge pull request #1358 from tahsinrahman/track-old-ms
1202244af3feca8e9394182958c6a12ee18ae074 Merge pull request #1413 from vincepri/record
498973dd7e24c1df8c008842976748eea3d3b4bf :sparkles: Add util/record package from CAPA
e1115135911296085ef17535366da0480bf0ca6d Merge pull request #1410 from vincepri/fixup-docs-add-util
a2e233cfd8b5a0f4f96f4e9eac3f8e07336483a5 Merge pull request #1397 from kikisdeliveryservice/docs-clusterctl-to-book
b98fc1578d976790697849d599f2ae025feda0b1 docs: move clusterctl to book
27ecf35047b709a46e4157cf24f4c1b0aeec44ca :book: Add embed util for mdbook / fixup prerequisites for CAPA
b3cb6fce6f78f9eca9565cf682952ba7750cf8b1 Adds chuckha to maintainers list
af25429c805eefa98b63cc7d0a2d2357eb4e8305 Merge pull request #1380 from detiber/ImprovePatching
feeea0c874d47a864ed0608f9eaf50cb2606909f Improve handling of patching and updates in MachineSet and MachineDeployment controllers
32d7146237375518a1d6586f881dbbc9a65f58e0 Merge pull request #1406 from detiber/updateCloudBuild
1e6df6ed5f98aa4531737cdd12511aac41597f74 Update cloudbuild.yaml for PULL_BASE_REF substitution
2e530c1edf3542ef6c8e1066cb2912a414d1b7c2 Merge pull request #1405 from ncdc/use-our-restmapper
c6f4c59ca29a943b7543c072180822e1e9d127d0 manager: use our RESTMapper
6e40ca2368f25e37c959ec791c57cd6346a74b62 Merge pull request #1403 from vincepri/remove-secret-delete
8723cca473f0e8df244f941d5605c4e5b32c86b6 :warning: Add OwnerReference to Kubeconfig secret
9a50a4375db7d0ecf41dd84c9af7ee8175b2bf4e Merge pull request #1401 from ncdc/wip-docs
e48ad4370ffbf19378fc96d6fcc19e1414d2b043 Add WIP for various docs
7d6959bfe3db32a83cd05f2fd984a7a004ee37d1 Merge pull request #1396 from vincepri/improve-quickstart
f915aafcf9906cd8df0979265fec1139ce554954 :book: Improve quickstart for AWS components installation
589e45ce13dc51e391f0e01df9237fd07cf8a71d Merge pull request #1379 from vincepri/structure-book
2e4a53f30de0dea3ecb5490d92ada99b346ad3f7 :book: Add MachineDeployment example
635a9e7f823b9cc924a5a9da9a70683fe35fdc44 📖 Quickstart / add other sections
15915e80c9648ac4bbd270cd97000efcfc4f801a :running: Add tabulate util for mdbook
a2de6693061c9a5693c9e10dd6b8bf71f16d050a Merge pull request #1394 from vincepri/mark-implemented
5432ecc926c9aaae415170ced08d68557f913881 :book: Mark proposals as implemented
d1079f98c390297bc7ad63aa51ae6d7acc8cf1c4 Merge pull request #1393 from chuckha/fix-notes
4153b17d6a8b2305b8ec7a9e1c86c182458540aa Merge pull request #1392 from detiber/pony-prow
9d741d1368ded67dd16021de4d63a9c31a4114e6 Updates release notes generator
335118c061b41c3915619f2e9344ca9a1956c196 Use prow/GCB for automated image builds rather than GitHub Actions
203d8f7d66b2a9058012a10fb08e69eaafe11dcb Merge pull request #1388 from tahsinrahman/explicit-client-machine
c5952ee886066c3920b3cdbaa944b8906cd0b4b3 Merge pull request #1386 from tahsinrahman/explicit-client-ms
44cf8e247d010a37e41f1a96691754db6b2b57d8 Merge pull request #1387 from tahsinrahman/explicit-client-md
c0438c3709d4bfda24613975b4794f59a78f6f25 MachineReconciler: make Client a proper field
92d0cc5d683cdd08273a36ccf6da5e520750f492 MachineDeploymentReconciler: make Client a proper field
55a34aaf5b7479378bb918d1b9c78cbcbd92ae1f Merge pull request #1385 from tahsinrahman/explicit-client-cluster
763697825d89e70ce69bfa52fb7596707cb3fd9b MachineSetReconciler: make Client a proper field
cf7ccaa61d4e495c97cddd4320c0d6db99fa8d59 ClusterReconciler: make Client a proper field
bfd65dfc8bf23f3485348673a271c1d7a7ead6c3 Write e2e test
9bf7c28ee75b3f20624d8f5d1eeb655bfcfb0fc4 track MS with old labels after updating MD labels
b9b33c70648af001c533c3be6cdd5608fbbfba05 Merge pull request #1325 from vincepri/better-reference-error-handling
571399033b1827c6802f9c675abb6de9a7d53f52 Merge pull request #1378 from ncdc/fix-md-test-flake
bbdd2bc49c63f23e0c2460b25da915c3dceec99c Fix MachineDeployment test flake
ca112ae5f76c874c804a05e2ea2d2775d194cd39 Merge pull request #1365 from vincepri/mdbook
a813ecb77dd1d7c786a08b9db595c0346b017cbc Merge pull request #1376 from tahsinrahman/upadte-gitignore
2b8c8e4b7b357b3522087b324e4fd5fd5d8c6522 Add .DS_Store to .gitignore
f32de9ef9bf24979484b7277b021fa5b0e3bb993 Merge pull request #1364 from vincepri/update-release-docs
36aeec556559995d2d322009190e1160151dff5c Merge pull request #1363 from vincepri/add-release-binaries
cf3564f2c4f44f0023e2637b691fbdd38421be7a :running: Update the release docs
4c50999664ca0f194d5a051b468c7b68a43fa048 :running: Add release binaries target to Makefile
a03e688ca83b48472efe5a2a49a6f7f227ffe894 Refactor README and other docs
2a58ded76631869ab335cd24fae3193efd339aa4 Add additional SUMMARY and expand introduction
13ecbf0897cf6ecb8ca0eb24b0fbc53a00855270 Merge pull request #1367 from vincepri/bug-owner-ref
2296cc943becd2243399ba4f602d486a47b24ed3 :bug: Set the correct OwnerRef Kind in MD controller
340aba88a519809392fe2a508e10f942e420ad2a ✨ Introduce mdbook
80033f1255165a01be2e9ae0876eb98ba4537a8f Update API markers to mdbook style
62d19c7250e5afdf871780ddf4c2d41a7246c6ea Update generated files
99b3d81a7589aeb1698022ba52ae1adefba25928 Update supporting files
9e748f6e18444a2901d722dd0c6e7b002c68e58f Merge pull request #1361 from ncdc/release-fixes
214199181e3846d8e4bbec675628d24b164b8e0b Release target fixes
fabe6ef772a8f50d0390f64f63be1593fc44da47 Merge pull request #1360 from akutz/bugfix/update-api-endpoints
cf98e810afdd93ffd05bbc0170aedd74e9024193 Update API endpoints if missing
af7f7d74e93bf893eb9576f1294dc62f6021a590 Merge pull request #1355 from detiber/fixRBAC
39330b6908c3f7405f85beb9aa6e9562cb7c235b Fix RBAC for kubeconfig secret generation
93a90cfc476f8c048e7a3e005a6a513ee0649b8b Merge pull request #1353 from vincepri/delete-cp-end
0a462b83edd35f3a576c9c9e58e9623043d36722 Merge pull request #1354 from vincepri/non-deleted-machines
29c1e5699a8e9896473581dd86bb013bd0127c53 :bug: Retrieve only non-deleted Machines
00ae4c18c36f9a762f6d51bec266c3a791b52992 Merge pull request #1348 from vincepri/release-goodies
9265a724a9169dcd9993e60a2567a4c79b0e9bf1 :running: Add release targets
42350aed94d170a5f14f592543327afd0c859f38 :bug: Delete control plane Machines at the end
67d897059593c3fc8c3a304b031573c516ba1dd9 Merge pull request #1350 from vincepri/add-kubeconfig-creation
a59289a513e83b700578e6acdd93865919e3d752 :sparkles: Create Kubeconfig when APIEndpoints is populated
d495192f76e0095113358c88cf76f93cc2e1e2ee Merge pull request #1347 from vincepri/release-notes-pretty
3b1e9cdedce9ef662f549263ec8ab18b36b9ad99 :running: Release notes tool improvements
c4b86d69d8b504aefb40cf28f706cde6762998b3 Merge pull request #1346 from detiber/fixScaleEvent
37d22f6edebd3993b86066d65e45c34000608ef3 Fix output of event when scaling a MachineDeployment
82b282b06aafa90a3a40eea0899269842194c68b Merge pull request #1344 from joonas/name-v1alpha2-imports
11f4fb13223a40afe848782eaa2f175012a27002 Name v1alpha2 imports
9df715fae8ddf396959eb31782de115a7c0ef19b Merge pull request #1345 from vincepri/cluster-ready-apien
bde0ab5391f64f8ebf29b6daad3c32d8d3ef4ecf :warning: Set InfrastructureReady before APIEndpoint
1597a1ff16ea99cbdec958bab253ba340abfceee Merge pull request #1342 from vincepri/add-cert-utils
34ac829f0698c66445e97a8f946b0ca9c5924186 :warning: Add certificate and secret utils
fd6068e332b20e2edb39e8e16fa477c94f3ab893 Merge pull request #1343 from vincepri/update-container-build
c5d6bb2c1dd4176a59c50a9bca684619f717fe3d :sparkles: Add tag to action, update Makefile
58b8460b80c53c7ecc0e99d42648cdb1a8c08745 Merge pull request #1323 from vincepri/easy-template
1063658f9b58bbb490575ea2af1efae34628f45b Merge pull request #1340 from chuckha/emoji-fix
4ddb03432cbee56d3f44e78e4b2cb929030aeab6 Fix match on others
e65fc3aeeae29fd8ca09274926a1bce45e3b0366 Merge pull request #1339 from Nordix/feature/move-kubeconfig-functionality-to-util
98482cd2c047a9f0304535961cc12ca486f8d49d Merge pull request #1338 from Nordix/feature/1322-configure-syncperiod-flag-via-flag
8bbf43b54f732fb91c798a66c7f0dc064c2b08aa Make kubeconfig fetch functionality in utils
4a731fe9a0e87c9768ed969be89f61f4a3aea946 Configure manage with sync-period flag
64ac1620218dd1f3e1c628b2d5afa273cdb07c98 Merge pull request #1337 from vincepri/allow-override-goproxy
cd8cf4d9e8a50c9085274e7d641be685992d1c92 Merge pull request #1334 from vincepri/hack-sed-bye
f281415ad3696582c014abd507eef104e6a494e3 Merge pull request #1335 from chuckha/rel-notes
2f88d6214c239fe61163de46d6b506bc082dd27d :running: Allow to provide custom GOPROXY
129916a68fcc6b2c5cea6450ddaebb1a3b269948 Merge pull request #1336 from liztio/conversion-nullpointer
3dba06ade7ef076164e6cef3ed2a21eb009d7f3e Fix null pointer exceptions in MachineStatus conversion
d76ea10ffbc9ab697f56ece40ec6b67ca252f423 Adds release notes generator tool
bd74699c08526a91d015796f97ea2a13aef048d3 Merge pull request #1331 from vincepri/add-cp-ready-field
f2ba458ea70cf41bf4a3cfa711927668cf31843e :running: Remove hack/sed.sh
52a00ddff06477bfaa6f0eb8a6bccb96a46aeabc Merge pull request #1332 from vincepri/kustomize-prefix
bff10dcab854495c8064cd1cb4a2875748b45dbf :breaking: Change kustomize prefix and namespace to "capi"
8853c3c85961f9e0a4c52b467a669d28449d3ec8 Merge pull request #1299 from vincepri/vincepri-admin
d69b90586edd19d7abb529daea14d8608a9c0f57 Add Status.ControlPlaneInitialized field
947658c0db870ce019c6afc9900be435fb5d8feb Merge pull request #1327 from vincepri/test-github-actions
f9133ae543b8348e344715473ea1f5ec5aa5ea79 :sparkles: Add github action to push on master merge
ee3e16ba2cc6111580d688864d933dabf961a298 Merge pull request #1260 from liztio/v1a1-a2-conversion
3b230d30d2b7b87e511c9e38c19ed407e735dd05 Auto- and manually- generated conversion functions
5a9f993515bf235af0c5d9b408aa6eae62daa303 Auto-generate conversion files
80572d362ebb77e580b5a3ef4dd59e2130dc1daa Merge pull request #1321 from vincepri/remove-vendor
f6c19234debff782b6b9082c4f3fd32a11c39925 Merge pull request #1330 from joonas/restore-syncperiod
ff15f34406f5ebbc18a7049f4caf2e0f2906e783 Restore 10 minute default for Manager SyncPeriod
ad869db89d2830be71fce91e7f9ee2794afdc956 Merge pull request #1329 from roberthbailey/owners
e5323ca568aca19b211cb5bdd41e9c420bd12727 Add emeritus approvers to leave a trail of those who have come and gone.
4e77f90e18aa6b3158aa0ef4c35d1064ca9bed79 :sparkles: Remove Bazel
f339487ab32321792edaeb3b4a7f0820f811e4b8 Merge pull request #1326 from vincepri/remove-examples
744692ee4d5b5fb7544127a93cfa4b0dd541f689 :running: Remove broken/outdated examples
11c5525de81bad91ea827f9396714ef653817d08 :sparkles: Improve ErrorMessage from referenced resources
0897c71ac927f5824b3e141987e7ce4810820c23 :sparkles: Update scripts, Dockerfile and Makefile for vendor removal
3c725c42fe514d520fdb3db6261a4b48f451d5ac Remove vendor folder
47413a956cbf55a0d89a3842ae78b94ee8385955 Merge pull request #1324 from ncdc/flakes
efb83d3deab873fcb6bc25ffdfa92a4df23705d4 Reduce MS controller test flakiness
15b58ee1698a8b9dbc99b7e9c460ee9f435846e4 Merge pull request #1280 from vincepri/clusterctl-support-v1a2
b015cb75cd3d975feeaf900e6609a723f37332ad :sparkles: Allow for easier UX when using MS/MD template refs
9a520827870a4fa307d4c5a3d94aca17c07234a9 Merge pull request #1309 from vincepri/cleanup-machine-controller
98360f0e4ef05d2d7562698813a85b44bb2e27a0 Merge pull request #1307 from vincepri/cleanup-cluster-reconciler
8c79239b0a641877d8f84f7684c75eb78d4e94a1 Merge pull request #1313 from vincepri/add-port-field
c50d701a6414e6e878d0a92e7852e2637fefc049 Merge pull request #1314 from vincepri/fixup-nits
17c81f7e42b4d030e13180b08ca719325f5e6d9d :running: Fixup nits from #1312
d3d30d861042b09fbdba4b273f2ac0b532e9adf7 :warning: Add APIServerPort field to Cluster networking
c12cca2c1f8cafec0fd5551850ed34a0852de923 :sparkles: Add custerctl support for v1alpha2
97965d12bbf6a67afe73bf09809b037ef62ffe67 Add util/restmapper Cached mapper with rate limiting
dd975d736915cb4b7911d9b67aee6c32780f1e47 Update vendor dependencies
615fa8b750e1edcde9140f03ad8d258b57c1aef5 Update Bazel
3bc1d296e8bf73dd3e9ecc2b1627173e0b36bbc9 :sparkles: Cleanup machine reconciler normal/delete
e8858ef3fe0f66efa58f467f78c09ac698131797 Merge pull request #1312 from ncdc/concurrency
4bb12402d921a86abc58a724537e4e4d036a2e0d :sparkles: Cleanup cluster reconciler normal/delete
e9b4fe126db1c45a2e3fd26f6b5b3bc1982ae65f Support concurrency in all controllers
f0a7aeb8f83ec7d27eab33dd36b2ac0031b091dc Merge pull request #1310 from vincepri/allow-nil
7e46078a8cd475e2a9d702a534ad23bffeb6c79d Merge pull request #1298 from newrelic-forks/rudoi/deletion
8e4dcdf12362fe9dc4a6c220a6cff78673ce3664 fix: clean up isDeleteReady logic
5eaef899566e7db4da386c9782dceb3276098e2f Merge pull request #1311 from vincepri/update-deps
3902aeaef586dfc7eb91e23ac2e1969e05cc8f3d Update controller runtime and tools to v0.2.0
ea79cd98f754c1752d98eab0f8bbf1a4ff3c6b34 :warning: Allow nil for ClusterNetwork's Services and Pods
223a3f3833b46086335133863b0854f4fbd0617d Update generated files
8bed7bad63b6c67aea75c40ce53bb28bdea4b358 Merge pull request #1308 from detiber/moreOptional
ba12d8f258fd6671f38bf735bfd4858cc9cdff5f Make all ClusterNetwork fields optional
b7b6070a10d689f77b135993c858b688e31600ba Merge pull request #1301 from joonas/kubeconfig-util
23ef7a8a48c2d21d85393c5ca04237258f99b2ac Merge pull request #1305 from joonas/remove-dead-test-code
6b43a1abf35b8c2225fcde9c6b5e265e10219e9c Remove unused test functions
48571367b5ed3dc3610160cbda8f2f9ccae1ea2a Move kubeconfig functions under kubeconfig package
a0ed23de256f6ae4b498b4c6f425870c45eb5788 Merge pull request #1296 from chuckha/kustomize
72e08101782d496259fc527941e54c79792ea488 Merge pull request #1300 from vincepri/remove-release-note
c053ff2eaa074090d815847693bf5f9d1d915695 Remove release note section from PR template
c23b1a0ef4b86e1582e5df98d7ef7324d24e7554 support kustomize v3.1.0
5e6803e85e029d6899bcc9d43e0cd005f9a770c4 Add vincepri to cluster-api-admins
636a336cc6b5598efe3803da932aca4074e437ce Merge pull request #1285 from Xenwar/rbac-per-controller
af0ff206f668361703b166648cc39675a30400e7 Moved RBAC kubebuilder rule generators relevant controllers
801b1c1a99d0218d1f6c8cb291b16ea3cc3d4ea2 Merge pull request #1293 from vincepri/upgrade-kind
fb31bb42ae043c92ee1139e751038a1a48f61cdd Merge pull request #1292 from vincepri/retry-acquire-client
599bfc30e122108fea73775134c24030a2ccae5b :running: Update KIND in CI to 0.5.0
fbb3776b567ba33682ec42d6c66104623153b6d6 ✨Add retry poll when acquiring a new clusterctl client
10a3b18b2213fe707fcfd8c26d80014281accd4e Merge pull request #1282 from vincepri/generic-yaml-parser
7ba6ec9f26ee2f7bd1c25d4aa1d0eed827b0e734 Merge pull request #1264 from newrelic-forks/update-klog
f393121112ddd609cec40829b4bcce34a66a4b9e :sparkles: util/yaml: generic Cluster API yaml parser for clusterctl
e57768190b8c06c153b27d555555ed56a0a6ac73 Update vendor dependencies
9b234ba73c9a626979358c1ce45bd16929098cc3 Update Bazel
9fc80f1a60c6addf0e80681a1d79853d7b889708 Merge pull request #1291 from vincepri/fix-reconcile-bootstrap
113a87e2a9d2474d1173deacf102653e9ee7fb4b fix klog update flag to false
126e6b4fe0c0c754b8f5700e4e0bfba9a34e6779 :bug: Call reconcileExternal earlier for bootstrap resources
331a6cc329f3332d594c721e9d9e4359cd25ca9c Merge pull request #1289 from vincepri/improve-reconcile-error-logs
9bd14aee4132101b826fe02c752d511e0092fc9e fix klog update flag to true
1d214630bf96b87c7645e9f64554d2585dad1866 update vendor for klog
6e2027c9c74974eef1a439a5412d96a0292ad6fe Improve RequeueAfterError log lines
00da5a5a75bbfa1a7bee4f0d90bcb64b9d67876d Merge pull request #1288 from detiber/noRequeue
06279762f3e72ec46734dee7f4756c34d3415b23 Merge pull request #1287 from vincepri/phase-printcolumn-cluter
0a41d9d2b435cc10f567e5585b07d7645e586c8e Remove unnecessary requeues
d3a4a0d64f37c7d147bc22ae884809183cb7edcd ✨ Add Phase printcolumn to Cluster
81b4a6de9240f172e4072ffd3684a581b074927f Merge pull request #1286 from vincepri/remove-provider-flag
c9a81cb9c0f9a988aec4f79ac4a71dc8019c9e89 :bug: Remove provider from get-kubeconfig alpha phase
822c71132fadc65ef8f2a5de4a73eacb51e7fac4 Merge pull request #1281 from vincepri/fixup-crd-scale-subresource
457e0c57d4b0ee4bb3bddc704519501cd8cfdb5a 🐛 Fix wrong selectorpath for scale subresources
cfa09279e8ffb7932f11785fb5ba72daa3d6aa1e Update generated files
cb0d7a8fe5a5f61c84ac4744f72556c95627b0c0 Merge pull request #1284 from newrelic-forks/capi-category
60933cb23498d0621f57454c208fc3a8d6e18bf2 add capi categories
5c3b9067cace6e4525b93a02f3df662de2e37a27 Merge pull request #1283 from vincepri/raise-golanci-deadline
ff1e7c8d105e9ec36fa0ab323dceb06d07fe1747 :running: Raise golangci-lint deadline to 2m
9fd8e4cbea0f36399189db09ff4e8521603f86dc Merge pull request #1278 from imikushin/const
f1999a34af877cf6f6e289378a6f3a70b8004d6f Merge pull request #1275 from detiber/patchHelper
06bc1f1f12ca5b63ac29060a64d3306d79cab402 Use const instead of var for string constants
09d97641a54085462688ed4a42ae81b8473fad4c Merge pull request #1277 from newrelic-forks/rudoi/ms-recorder
e214871fcc931e5f725bca62a62cb7209e669500 Add PatchHelper to utils
4bd7eadf4b100514f1f1cf1d2752b60433056b78 chore: set up recorder for machineset controller
38edf8b4497ed4d3966580d68a8119140b8926e6 Merge pull request #1276 from vincepri/add-versioning
3b251870fd4ab85c55442b20566f0756de1896e2 Add VERSIONING.md
e12e3e5a05aaf6fd516da910239b0697425b13e0 Merge pull request #1273 from vincepri/update-go
e0ffb7e634f83215fbfd505e5293180479fd356d Update Go 1.12.9 / Bazel deps
9831c6bdfd178be6ceafa285a541c8272036f85e Merge pull request #1267 from vincepri/migrate-md
6fec0ec516d09a449b5e055a5a2c2e550265d7ac Add controllers/doc.go with RBAC rules
9191f228f77160fa1eea31bc968229bc14f330c5 Migrate MachineDeployment controller to Kubebuilder v2
f3c86cf1468a2830375d474a2fad272c0f196ffb Merge pull request #1270 from vincepri/fixup-kustomize
abd3b0d061e75e16d844e9226a57ba588f17186e :bug: Fix kustomization files
4cd3981188471f563df60a591c3b588e721345c3 Remove cmd/manager
2ea2000a619bcd1b805beb049ea3bb0cd0c3aa2f Update vendor dependencies
f77be4463b38e31a71413775c0d73f7e6471b1fe Update Bazel
f1c8056b2e564eb0dc7403ded069dd3ce5af53b5 Merge pull request #1268 from vincepri/update-deps
ef61e2cd03ff9b8892bb070196e45fad3a5a22ca :running: Update controller-{runtime, tools} to v0.2.0-rc.0
494eb25f7f3c6eb78e65b8b0a576ed481e0b80f5 Merge pull request #1248 from chuckha/sequence-diagram-v1alpha2
5f1e8af32d6e78481c88e8fccaf95a5eedc630ff Merge pull request #1265 from sethp-nr/patch-1
d6196f1e603bc942104bc11231ff15461b446f2b Add optional pprof server
96cbdbb7bd1a2fed5b8ae71dd98bb41fa47c9fd6 Add optional pprof http server
b89bf104abc286f9018f03e16340e1c130cadae9 Merge pull request #1263 from vincepri/migrate-machineset
acce679ffd6b7b15aa8ed19bd0bb585c2f70aa96 Migrate MachineSet controller to Kubebuilder v2
bc3fa02aaf96f035f99616677d71f03c772b4713 Update vendor dependencies
3f505bc8a795847fa17c2b52765521190b1a25b1 Update Bazel
27d548311363d51977c75b09fdc0b7f8f8ffbaf0 Merge pull request #1254 from vincepri/pr-template-update
56bd7d75229ab87599f1d5788c9058d0cb50c968 Merge pull request #1261 from chuckha/status-workaround
f4f51a8f38c118c70166e6e89501ac62a4a32e29 Ensure status updates succeed
34f670dfc8a33ce9eaada7414bb1ecfc244c9f3c Merge pull request #1262 from vincepri/move-machine-reconciler
68b6f9f4b04b5c1165a84ddc798a237662b4d0fa Require PR title to include typed emoji
717674f19999d183b9a8ed797ba62e2175a8aa8f :warning: Migrate Machine Controller to Kubebuilder v2
f744af846a531d6e01a83b242f6cb30a735bdc12 Update Bazel
6a8ed7875e3d18979f0dd2df230f78cac23a4d8b Merge pull request #1256 from vincepri/move-pkgs
02b3e4e7197899cdf06eb5fb67980156bbd2f1a3 Merge pull request #1257 from newrelic-forks/dennison/verify-generated-files
ed5d3802d45273ce39caf1d181529fa9634dd25e Fixup ci-integration tests
d7241317171aa2e66414ddbf3e72f53bb8c78a44 Adds sequence diagram for v1alpha2
aa7704e4f5ed1e0e8e2cbee93775413f1cd0dd94 Merge pull request #1253 from accepting/fix
ac18c61e212dbe6e818834e58a85b550e02e811c Fix: update cluster annotations when control plane is ready
a713b7555128d8935063ea6081b110dce907d08f chore: verify-generated-files
fcc770df74fa0c5c7e8d6e0a5e7ca20c87bbfd96 Update vendor dependencies
b321a6c56de8d765a6f06cfa102ffc4059f5ad8b Update generated files
75d377c2b98bd74f220a9632382066d6c3d4703c Move external,noderefutil,remote out of pkg/controller
33b68215721e66a3d1d071caff170756898a2dbf Remove unused packages
787dd698d402cd957355da577f2aec9f6e1359c6 Update Bazel
1f6bf657568e3806ed89725d06222590afba11b5 Merge pull request #1255 from vincepri/fix-make-verify
3eacfef7394b615cb7e0e13f04efc5e9604f99cb Remove verify-clientset, fix verify-doctoc
7356a99369108c415562485704a7e235af32a633 Update vendor dependencies
3bc8f6f406e2c012374ad5ec911966c5e769142a Update generated files
b257e984a4673f2116794a51a2547f1beec5af65 Update Bazel
7dc552af10741df8a35348304de575eff1f7ee46 Merge pull request #1252 from vincepri/move-cluster-controller
fabf8a44997c7ceffe6e91064f2093c5c5307203 Remove extra RBAC rules
cc0ac057f64d605b2b903715515ef9f318457c66 Update vendor dependencies
911499045d1d88480762f9e68b5b8da8763d04a2 Migrate Cluster Controller to Kubebuilder v2
22dcb05b624cfb14b20f6f16c250bc87c8b91ffe Update Bazel
65800b3b20e8405fd07be8c20ff0a56c9f952056 Merge pull request #1150 from dongwangdw/setup-doctoc
4cb93778a9a470b38ed44e5f1ca47e7435deca9b Merge pull request #1249 from vincepri/kbv2
4e9e7b53f288f92c54efd647f73459e13c069bc3 Update Dockerfile to include new folders and files
f0861bd9d118892548a31b8f378513889303c064 Update Makefile CRD generation
30233dd651405e78fac367f42ea6be89f58163db Update import paths and breaking changes
8da4fe7ca70920448d3c01d187de06432e7f0d07 Add /main.go
b7be1351a598c7f78fac6750b97c10e9fd38d06f Merge pull request #1209 from eromanova/ensure-namespace
61dcfa926022604db783620a186f9cb3869eee9c Scaffold controllers package
41b2515eecbc7a3301239c8aaee7380dd69a7c5b Migrate API types
8f67f5d225d7e829861a7ce10a8b4db24ee51fb4 Fix ensure namespace function in clusterclient
7d800225055e04862815ebfc66c77d35d9b4c4d3 Update PROJECT to Kubebuilder v2
633988a2cd616f0d1faf5329b5fa5015bad4a441 Update vendor dependencies
411f3d56d915fbfa2d317f02ae7f33e2d8016a2d Update generated files
20219c1d6453d26ba548c3d0141f7baba136d67b Update Bazel
59350ecc7253a8f64210d4f6152b5b4783eed81c Merge pull request #1247 from vincepri/status-phase-plain
09cc4b5c6f402eef1e8b22a75bc57e0ec298da3b Merge pull request #1251 from vincepri/remove-sample
578061f9acf53c5ecc9ecee788a96f87ad2e0cf9 Remove sample folder
5524f527fdf28d0cfebea249965495fc802d3402 Merge branch 'master' into setup-doctoc
cc9ce92e17f40641f668e4a864e98f312d4eae49 Merge pull request #1246 from vincepri/improve-hack-files
b4a6755c6cbd21f49a0931adbacf117fea0fb9be Update generated files
5fdfa30e69be644a1dc4f3ddba22e9928768350a Make cluster.status.phase and machine.status.phase non-pointers
5e6e3f4ec0b8eb119e5e0436468d6d0b08e15f05 Merge pull request #1241 from vincepri/remove-pkg-client
74ed1085965384f31510f9a8c757eadddd1ef7c2 Improve hack files
72ab98b868fc50f4974bb8fa94f382593b6d6f5b Update Bazel
8ac3587cfdd294ba74265c360c5521bf17363221 Use controller-gen to generate deepcopy
2571a2564a117a58c30cf21b30c21a5df4b03d44 Refactor clusterctl to use controller-runtime Client
b1d03f4da16bc41967543db7bf873eaf32c03985 Remove references from Makefile
24a7476deb0a1a647d64c9ab03f9df4bd2efa337 Remove code-generator from hack/tools.go
1d98de064f57669f309ad284ef4ba96087cf0c8c Remove pkg/client directory
c1475289366f3da2535ee60a6df92e0564e6a57d Update vendor dependencies
b56060090117f0b27e8d5c1784d5a0daab4ac6f7 issue-934: Add doctoc for docs updating
b90e680d6b7ecedc637e71737ab480311af6d8bb Merge pull request #822 from jichenjc/fix_log
b8af96f0a42a9cf68bb21f28a81ca14b04840cf1 Merge pull request #1239 from vincepri/update-crds
052e7ef01289fde1b04aaf484b7f00c29fa6a49d Update CRDs
f22bb08e2e88732822565be1693b211e3b9ab5b2 Avoid get machine when it's not needed
e2e5934b434cbe02783e194609685ec5816bbc64 Merge pull request #1238 from detiber/NoGetMachineSet
1c21ae23a236d73d58f8a1855638bcba6687c4b7 Remove unnecessary get for MachineSet in MachineSetToDeployments
3e0cfc573145cd8152b6372f9fa91397575c6e19 Merge pull request #1236 from vincepri/controller-runtime-beta5
94f9f35c429a7890197a9b02d50dc8aac9e6e1fa Use ListOption
8eb56b38817fbab27f24c0af2e2b634850cc6978 Update Bazel
9916fdf011cd50feff8af5f4d2666a2e222878f6 Update controller-runtime to beta.5
0c3c102885e6697e43c9c65168677a970aa00bb5 Merge pull request #1235 from detiber/fixGetOwnerMachine
824065d884458a13411ba44efd7677a554da9d93 Return correct Machine Name in util.GetOwnerMachine
30301140f8e4505a2d0685d18294178af59a8411 Merge pull request #1230 from chuckha/bugfix
ce149a505c96168a4392d0888103c54b810e89ea Merge pull request #1232 from zhuguihua/fix_cluster_not_found_error
34a89371eb3aa494cb9f9a1e7c1d8216b0c9f00c Merge pull request #1233 from zhuguihua/return_nil_when_bootstrap_configref_not_exist
dcc229e7ffa15860049f594d6ad7270030ce96d7 Fix cluster not found error
fc62c246c21fa272c438698bf6bd677a60718076 return nil when Bootstrap.ConfigRef doesn't exist
fc3a5955442f0b372393a68a067b3039b94d085b Fixes a bug in GetClusterByName
62582da077611649856cb2a88ec73c957e8569f5 Allow optional addresses (#1222)
7023b3fe000ccb35a545b9c364615faf463ca3b0 Cluster: delete children first. (#1225)
126717568f32064762d63eed4cc452913acfdb1f Update controller-tools to v0.2.0-beta.5 (#1224)
04304d3b23717c2fc1c84f5e874a4416da1f9ef0 Return early if InfrastructureRef is nil (#1223)
8525a09626f9eb8cf9869b0700da9c1f52ed8d20 Adds a v1a1 to v1a2 comparison document (#1211)
49ff335399d78cf13aa4ce613f727614ba90d4f9 Adopt conditionally based on owner (#1214)
e6d2d5012e89e9b4a671b949e03ee00cf03bc5ed Add openstack acronym to gitbook (#1216)
f61e86b163b976a572e2f529f674c963aff6e5a4 Document procedure for creating per release books. (#1215)
83d4c2a2eeca217f7af3c9f4f485fdbfab39e89b Fix jsonpatch go module (#1217)
9b9bf15a9f6c02728c4c78ba4a1905d80b0b7667 Add section on conventions in Cluster API (#1213)
3be3a5776b374743fb7ebee643f22560a73c5b14 Code Cleanup- Remove sample config files (#1171)
7fa92e285480906d5db3ce74e4e979146d5ebffa Add Cluster helper funcs for infra providers to use (#1212)
3f7329dda10f3d3e9ae1867dbe2316c43e10d135 Fix GVK in Machine Controller (#1200)
835ee872f98d1ca1ef6b9cc07235badabd7f89e2 Cluster controller and types for v1alpha2 (#1177)
4007f4288d8c35175bed9908377b664d890ef52f Revert proposal change of ClusterStatus.APIEndpoints to APIEndpoint (#1193)
d8b90c56ad73bff2035264e450ddd1cb42a8a1f6 Update plantuml generation to use CAPI-managed image (#1194)
5ad23f19328fee293e9dbca75048277430f6bc50 Add Packet to cluster-api provider list (#1189)
6afa7aee7f42a6f306afb52617984a48f75f1850 Use v1alpha2 as version in tests (#1186)
8d4cb92c5c7ffce28750f74a47bbddc10efa8688 kustomization.yaml: Use patchesStrategicMerge (#1184)
bf8541c6acdf96bdbd55ce551424923cd1268783 Add logic to copy Machine Addresses from infrastructure (#1174)
83077786abfad573eef43ae59d624f6cb610c51f Switch apiGroup to x-k8s.io (#1182)
edee832e7baef9a8e39176c2f6ae6b167a8f558d Build manager binary inside a container (#1170)
6efa4ea92d368fbb4740e4a6f8aa418b103202a1 Improve diagram generation / fixup cluster proposal (#1181)
5dac9ed7191376eb79463c739e868086aa1129f3 Make clusterctl provider agnostic / remove deployer (#1179)
cbb820d5e3960de956485f506b7084e2d605bc44 Update bootstrap proposal: document Status.Ready (#1161)
7303333fa3bd40aeff46ab04a28c7574ee83e66d Externalize provider specific specs and status in separated CRDs (#1137)
61735cbb8949e2872b1a17498b9f52ab5d2128f4 Update controller-tools to v0.2.0-beta.4 (#1178)
b1999e334c61da0982b504a3008cebdb70a72819 Always Patch machines on defer, requeue if finalizer cannot be removed (#1175)
4d3d5cda028cae1a5f966546c491aa2a66d70469 Set control-plane-ready annotation on Cluster (#1169)
d09d51c5094c5b4db8b9b37b8d2e1812e97646a8 Update docs/book/GLOSSARY.md (#1100)
ac0baea674299850dbfe0e0a1735915100aabde0 Convert {Bootstrap,Infrastructure}Ready fields to plain bools (#1160)
3256e62914839012e620ddd40c156b039ecb07e1 Use an inline decoder so we don't constantly have to marshal and unmarshal (#1167)
345409ee6ef9991f70915b05120d51b23c3b1b14 Update lodash version to address CVE (#1157)
616fe79572f813bf94bc7e495efb69b4651021f8 Adds a trailing newline (#1165)
5b905b77f0cd3c8084444e73235c2a3d968289b7 Add MachineAddress type for infrastructure providers (#1162)
a0c249c4812aaf1e68959c568c86d1d7ffaa44e8 Update Releasing Docs (#1148)
c48cbe1dd3505e644057121a08218e80f7917d0d add log to indicate cluster/machine mismatch (#1151)
4b554569d2d2ba69102e75cdee325e26c96cbdf5 Convert bootstrap Figure1 to platuml (#1163)
a507c44fc106d87825720f751890c825aef4e9a7 Add util.GetMachineOwner (#1159)
f1af714c4c2eedb8e8a11d05a479f22b2a3821cb Add util.MachineToInfrastructureMapFunc for infrastructure providers (#1153)
61aab24dde2e7d22339db5ee93db133b76bd427d Add util.GetClusterFromMetadata (#1152)
fa97cb41ada4f6d64b1b89807ceaf754b26afc43 Add GetControlPlaneMachinesFromList and remove deprecated function (#1155)
49136c83cd6e0b0832225680040f95a3ef68273b Doc on clusterctl. How to use and how it works. (#1131)
4b496fb3733c4e3d4510577a406773bef186fbb8 Rename controller name with - instead of _ (#1149)
5ffab93802d780ba4fa7f529956b254b552aa86d Add gazelle rule for grpc-ecosystem (#1147)
7f2c2d561010c31795953655d7c5f2eb486a9caa Add full vendor utilities for gomod (#1134)
68d2eba83817f39d134025b9b66708679e35a490 Remove NodeConditions from Machine.Status (#1081)
09e491e49d7c91862fbb34da0ba42b2f593d37cd Update controller-tools to v0.2.0-beta.3 (#1143)
092006bd15d29b4b7649129838da8f49845b5ed0 Add section around backporting patches (#1139)
a12e02202df6a19e2180d91a32f56c9aa8738197 Embed NodeRef logic into Machine controller (#1128)
871f4b4b73a247e0f1ea5eef28c95866729b64c6 Do not delete NodeRef for last control plane node (#1110) (#1135)
188c646fe5551b724efd253689d56af2ce1d7689 Rereconcile machineset if not all replicas are ready (#1133)
1bc7d376a1bad103fafbb8a9deaee15137ebc646 Consolidate error packages (#1129)
1c653f0700b284b593490e5d442421d37f17379b Use template references in MachineSet controller (#1125)
35a86b775bf0e1702657f0bb9de203eb2d20bf41 Add Dockerfile for plantuml image used to generate proposal diagrams (#1108)
c1ec21073f04b28dae814f1461a6190d11726d2b Remove pkg/kubeadm and pkg/cmdrunner (#1130)
2a280a3c5734c6a2a14a25b6ec19473f7b004828 Cleanup Machine controller tests (#1126)
0278a56068a9815819a0c0813804fcf24d84ad47 Document Netlify based OS agnostic testing. (#1124)
76ad211ede3d8a67e97aa5bdb8d1d8e0ba4c9ce6 Don't swallow errors when reconciling noderef (#1117)
61ad9c27607f3e09729ef3a215eade20ac4079ff Match ncdc owner aliases with k/org (#1087)
28a6e8b84a22fa64734a1eceace39fc0635fe678 MachineDeployment controller and test hardening (#1116)
464e9b86af10168156930aaa4b301fffd6d529b5 Fix ProviderID handling of scheme://oneSegment (#1121)
2afdb44e930c7af5257063fcf5a8aa1ea492d489 Scope MachineSet controller Machine listing with labels (#1111)
ece62e430e59f10cb8cec98cf1d3191991f73b43 MachineSet reconcile test hardening (#1106)
dc8ac4c82ac1577bdf3fdcf366ae3389dbbfeaca Update controller-runtime to v0.2.0-beta.4 (#1107)
062597042d3613233cf611479855ddd840940885 Add templating support to MachineSet (bootstrap & infrastructure) (#1098)
b37cf11c05acebee2ffd0c8a845c2bc3e1c1f7a0 change controllerError to lowercase (#1101)
e9145e9e45876a9c409b70e989af31f64c6ad555 Add external package to work with unstructured objects (#1094)
6c10af96b01554890ea0788d068103a3afb54687 Add RBAC rules for infrastructure and bootstrap resources (#1095)
554a3a15cbd8dfeb4bfcb7de65b652d0323d0015 Use EnsureOwnerRef in MachineDeployment and MachineSet controllers (#1093)
5653faac5da0426e7bf1c57bedeea00ef247cb97 Update Go to 1.12.6 and update build flags in Dockerfile (#1092)
8d0153218143e72e71e5c16dfb9fdf80cd44e0e6 Add dynamic watchers to Machine controller (#1089)
bddbc39d07953fb8c73c1312e38460a28fed6494 Switch kubebuilder domain to sigs.k8s.io (#1091)
5bd98f997e21cd56b54885160b1727fef6d1f850 Update controller-runtime to v0.2.0-beta3 (#1088)
65c5a8929e96f32dc0b3d8373a5c6be9b178c4c0 v1alpha2 Machine Controller logic (#1083)
5a82701777403d72f18f909b9c74addc3a8b0924 Add MachinePhase type and helper functions (#1080)
52e4b8af49135c65a4020e5edfa0400f5a9ef93c Update releasing doc for better go module support (#1082)
0a3d842c1d93590ae18c3c3c4065011186e4189e Convert Figures 3-8 to PlantUML, add make target to generate (#1058)
fabb25e50f7ff5fc4306da045af6e0b41bf69ec2 Improve Makefile for clientset and gen bins (#1079)
377ad4ef90b7960664efa45266cdfbd1214fa62c Add v1alpha2 types :tada: (#1051)
831e2ccb1505396805f8b688590de48667f34838 Add noderef controller documentation to gitbook (#1066)
027822a4f75c06c7e329bed0b8dd5fca46d84fbb correct word (#1077)
337ec9ce036d04f41e87d0a2ecddd3d8fc0482e6 Link boilerplate.go.txt for kubebuilder (#1068)
1eaf864bae1717e707373c4afd97225e7cb59d53 Use remote NodeRef in Machine and MachineSet controllers (#1052)
814130408c655984e6b2b10d698243aa226fb43f Fix register bootstrap options in alpha phases (#1064)
82c49a93c17f23af844ddb5121902e37ad109f47 Use go modules, update controller-{runtime, tools} to v2 (#1054)
320b7f4f734af4fac121615ac4f59b89be5a7752 Improve generate-* targets in Makefile (#1061)
c11ed81ae6f38307c5bf5e10676d5fee9809c357 Embed only a subset of metav1.ObjectMeta fields (#1062)
78ae00d4a50d7cb5e895370486ab04e3c4b88632 Use development gcr.io project as default registry (#1060)
554edc45b67aaaba0650f98ab88d8209465ba773 Machine States & Preboot Bootstrapping (#997)
aecec29bd9d1180631bcc0742a461f9b3409b91a Update dep check (#1056)
1cb3deba7ad6b0df8eed27d722aaf76a389f9489 Update controller-tools to 0.1.11 (#1053)
1c10a3f67527313e9b384c077e6991404d9e65be Update generated files, add workaround for controller-tools (#1050)
9e8954651b45960301e304aa2ada26657c68b573 NodeRef controller (#1011)
9e1eb5617f3f3be70c5fb52dbd3b7eafbe6a6898 Make ClusterNetwork ClusterNetworkingConfig field optional within (#919)
97f25c964841e989ed61d05aaf214504c7cc3ae0 downgrade log of util.ExecuteCommand (#975)
c2faf86f1e185c2d837f005242df06a71bf173ef Update k8s/code-generator to latest release-1.13 (#1048)
f1461325ef33371cb52e0b0522bcdb4efcd7906e move hpa to the correct spot in the glossary (#1047)
d63d4bee4854d5a4580b20581b27e6183d3c10ad clean up shell scripts in cluster-api (#1045)
2123eedbe0f50293b5950b2dd667afbe91bb30c3 Bazel updates (#1043)
1fca3cae427b6cdb514a645590e7c6b52f6c0d13 Added use case for Cluster Health Checking. (#933)
0ebf07643f5180359236d3f07b86e9f8035dc235 Use klog in manager and setup controller-runtime logger (#1022)
bd0628f9aa808db1fdeed5c8bfba07ee2ecb1406 Support for wrapped RequeueAfterError/interface (#1020)
da61280866e1b66aa7abe07e824a9a3cb88a53b4 Update controller-runtime and controller-tools (#1032)
91179deda81cc4b96740a1d182f64a293844dae5 note about membership requirement for /assign (#1030)
76955259c1671568e7bb38664899d2188ad3207a Fixup glossary to match GitBook conventions. (#1029)
e83667e8ea9393a1694433ddecde732d08ef0302 docs: fix cluster API glossary page (#1028)
a5e5fdb36d5e3ce77e03a1cd5ad6af3728976c82 Add events to MachineDeployment operations (#1014)
9cd85f7b20c544bc127ca75582535d8601332754 Add CLUSTER_API_KUBECONFIG_READY_TIMEOUT to clusterctl (#1026)
0b215f4d102edd23977f04383eb8d2b028bd315b Update boilerplate check and generated files (#1010)
77836d885f581f60a2f2191e6bcb0412a1df3784 Update some bazel dependencies (#1019)
7365154da39c9415d69fcca7f20e932ecf4d11a1 Add patch to events rbac (#1021)
b0170a09cd9cccd60e5b67cbb9b3971229e8b02c Add events to MachineSet operations (#1012)
5f71f0b252f58e0f074212232354740aab04dc50 Update GitBook URL to point to netlify served pages instead of (#1013)
f0fb1107004691f9361294bafa43e72c482e2d07 Fix links in Architecture documentation. (#1008)
280e527f82b4bbb683c8df1a2740b35e09d0f4e8 support random generate cluster name (#984)
0b25546444bf41579dd3ea0e788e678f7dd88eaa Add remote.ClusterClient to access remote workload clusters (#1006)
f96ac27b355e8ef15722b4050691b0b768b48e2a add glossary to documentation (#1001)
d48025dafe37451aa3f28deb7c7954d95e4cc25d Add remote/util.go helpers to work with KubeConfig Secrets (#1004)
f88835a86ebc6f7633a41f4876f18d6bc4d38fde Always pull distroless/static:latest before building (#1000)
eafafe868684092d83250531b8ddc4d9f1825b76 Rename pkg/controller/controller (#998)
aacb0c613ffb5f0196c7cdca0c615162c70b14f5 Remove duplicate checks for deletionTimestamp (#987)
5fd25dcfb83a225367933ee32b65f59e1cbdfe27 Add foregroundDeletion finalizer to Cluster object (#988)
42f160db7ffc51cb723a9c28f33b8bb19d6f31e8 Update dependencies (#982)
30a65322ccb84b04712af87d14b43d2bea1a174d Add more log for cluster deletion failure (#978)
76b4b9c91aaf5d04f7ba076e0b4184d852e5bc39 Add versioning and releases to README (#967)
54593075a7a1526ff25aa38211b89695b7267e50 Update Gitbook release process (#659)
ee3a60b7d552286b9a0c273fcd70ff7e8235f179 make cluster-api-manager container run with a non-root user (#955)
2ec456177c0e8f0a903f4e746d44baaae54cc591 Rename controllers test files (#968)
a7a0a93a8052fd08a8fb585746f99d107227f521 Allow to use foregroundDeletion for MachineDeployments and MachineSets (#953)
30d2ec8731ee76c9024642a33d5291f73656e242 Cannot retrieve machine name (#960)
6608a1b6249f2a0b477445af9f334de5abf83558 updates Google Cloud branding to mach other usages (#973)
4e465579634471d0a2ceb0e649dce733308299a9 Cleanup controllers (#958)
a8ab9b58cc8d6900b259376dc51e01dab4e5a3a1 Quit MachineSet reconcile early if DeletionTimestamp is set (#956)
f19aa238ae60a8eda4e3f100e21818a6cc5c7b24 Added comment about cluster API vs cloud providers to readme (#954)
3d06a0237b2ee4eaef29de1ca5bd8f8c07929221 Added ibm cloud to architecture diagram. (#946)
69c25202ae06fe976d0f06da989015b8636cf546 Remove workstreams from scope and objectives (#948)
16b5da51c5e8337155c54061dabec323587faa21 [docs] Update RBAC annotations for example provider (#947)
32f755e7788f65c63b647cf0e79d57ba8b6ed97b Fix machine object pivoting to the target cluster (#944)
9f53a3abf65c22ac8c98c2904946cf02f1038b4c Add shortnames for crds. (#943)
c88a4ff639f99eec9391f947f66d80930aed4e04 Update README.md (#941)
2559f8139977b2b92eacc9c4e8cc8e0326137849 Attempt to fix integration tests (#942)
2461be4bcef798177d17e67746abc6dcb7767053 Update to go 1.12.5 (#937)
afa9d8e879c3ac3fc199284ffef5deab2438a05e Used doctoc generated toc. (#932)
5ce51badf46a003f8edb507a0801f1382cbcd5a8 Updating release docs for branching approach now that we are 0.x (#862)
60ad1689e531975234a52b211cdbff54537668bd Adding Reference Use Cases to README. (#931)
537dfee50e59f57b40e497b6d98f7d82a0f7fcde Add Cluster API logos from CNCF (#916)
cd458b683691a02fe84cb0b3aade47738a1bf5ec Update documentation links to published content (#927)
28b9e158ff0b3a766f9306c8a29ad3da193676af Added IBM Cloud to Cluster API README. (#928)
3a3c7089ac71ce78900cafd6faeee8ed07659e05 Add /status to MachineSet and MachineDeployment kubebuilder directives (#922)
d5a6ae878c81499376596feba4deb705d03e90eb Bump kubectl version to v1.13.2 in ci (#923)
4ae283625138e24a0eead7f163deeb1607830cbe Add missing bullet point to staging-use-cases.md (#920)
7b6bf1e92845a19eced5da9166275513a25b29ce Add reference use cases for Cluster API (#903)
a77427fe8dffdffcf3e2eb218dfe3d2c704724bc Add Talos to list of providers (#915)
f941ddcd29b537d80724a0263f565c085a7bf96a Add support for passing namespace cmdline flag to the manager (#914)
71ed12f850401b9fd80739e0bbf23aeb4abf1e76 Update github org for the baremetal provider. (#911)
77224b1d1add00376769b3eeb70a4995e8b22577 Simplify util.ParseMachinesYaml (#909)
5e2e91dd6f9b7cb90cec3059da0298e8d1458cee [clusterctl] Do not fail in waitForKubectlApply if error contains "no such host" (#906)
9485c7097bbc01778e454d89280161219f10f8a2 Clarify MachineDeployment watchers' comments (#887)
abfd18620fd024a48e1a53db448527e871966f23 Clarify log message for machine-controller isDeleteAllowed (#905)
cb69cde1c87ec90c6e64dedc228c6c1ee8584314 Fix API group name written in kubebuilder's annotation comments (#883)
541d1518bc43217e0f9d0b9e967e45cb44575983 Add Cluster API project scope and objectives (#882)
1d065aa1e9db9546681f55db3079b16896f97a6c Update OWNERS_ALIASES and SECURITY_CONTACTS (#884)
a493ad0b33e5b215154404674e7861f2ebc710e8 Update Go 1.12 (#898)
8c86b5f2ca72c378a69f798c0d08dd71d64d0482 Fix a broken link to Cluster API KEP (#900)
cab42a08030087070ae4179153de97831eeeb097 Build mulit-arch image and push manifest (#886)
f7a375095db59eb69d2736c123cf70529c0fe554 Update manager-role ClusterRole (#901)
c262415ed392fe4091391ddfe69d17e1c47bdecb Normalize clusterctl options to underscores (#899)
a918956a7660bc1a3058d7a190cc91e09be8612d additionalPrinterColumns for Machine, added correctly. (#897)
5e4123c16a4fb57afb53c9dae84f15ba4746ce9e Add NodeName to Machine's additionalPrinterColumns (#895)
e325dfa6ecd8ed3ba68e2b07d645c8037c9fa09f Add missing namespace to Get function (#896)
d21d1828e2f640886cbe735faf0e5571da089af5 Update klog to 0.3.0 release (#890)
171ec1ab5ec6727e6c7bbba1308c74432fc3a1b2 Add discuss link to README (#885)
3534230079bba03567975f266f4b8aa01727bdf7 make clusterapi wait timeout configurable (#865)
b03dc0e6daead3398035f7f8734a901e1707eacd Clarify how to use kuebconfig. (#869)
d6418fc3a618e2c805e1e3ec8fee42c7d619841f Record machine sync error event (#880)
0b731c568d7e0c2315cc8ff7cffc710471f1d91f Add proposals template (#879)
2d14f02268f6f42d762fdb7b00518dc6fe122f41 Adding steps for how to use existing cluster as bootstrap cluster. (#877)
767e4ba9a06fd1d2519af97f4d4534892616e9bf Ability to deploy multiple control plane machines (#878)
b90a4cc5f7d73cbe195ffc450bd09bd5a837c652 nit: fix log to replace Creating with Preparing (#872)
bd4bb26d12430e726b7f1ee05937af9e44f9ecd0 minikube: use --profile instead of --p (#875)
9df3ba8b7482f638270b60b4571928cef38448b1 Fix error message in getCluster (#871)
c63bf6f67ab631a449b6eb76dfe29458441051e0 use gnu sed on all platforms (#867)
114dcc2a531cc7f69be76578ae3474c307d5afbb fix various shell bugs (#868)
92949fa167b6b631a7b02fea1ec9ce126c76534a Update CRDs (#863)
7344ab551cfcc0051683fcea1644cdd75dc91d19 allow machinesets that have clusters to continue reconciliation (#836)
9f67debf87223b4bc03cebf0f0500be9fae050f6 Update Taints field comment in machine spec (#651)
f6aa237aa9764423a39443a27b69e63c158b42a6 Adds Oldest and Newest delete policies and annotation-based Simple delete policy (#726)
02c89a0feb7c34f60d51aba7d34e51066a60fe33 Update sample provider implementation (#850)
a1bfbd3796270faa48c411ff9174a5fd219dfa50 Set the resync interval to 10m, instead of the default 10h (#824)
c28db3292c5bbabbcdcfbbdf7bfc45f01ee97177 Fix openshift link (#856)
d63248ec0199cdab1246da8b0ab1d3bbc50cc6f6 Add status (phase and provider id) to get output (#851)
0c79e05efbeb7ca2f9d1e5b132279d7e76ae0954 Added diagrams illustrating the controller logic (#834)
614aceb8c72c5bfa48081b4c41fa669ebc2e6877 Added more spec for machinedeployment. (#835)
f0fd0c578fa8facfc2c6f09624dbb48a3ba2f3b2 Added kind support for README. (#847)
5bf3f7edf03c12aa6876ccf73eb5805704d8f0b1 Update to Go 1.11.6 (#857)
c300b03e15122644044aae3d0c02ffb983e1b5d4 Fix doc for --bootstrap-flags usage (#846)
7323439381456c3dcd5ba6f774db14ec4aae6f1f update docs to point to relevant google groups (#854)
3f43912fdb392b6f8cf824401e0a3ddb7590adf2 Add missing BAZEL files for client-go (#849)
9caadd6c85dc2706b59b3ea21ab78d472596d79f Enable setting profile for minikube bootstrap cluster. (#845)
59bc50ec3e3d1053ebabbad803fc3e93cf2acf0c fix: fetch cluster object inside kubeconfig ready loop (#840)
2fd99299a0f419566cdcd1d8fa53a2448b3579f8 Honour the KinD --name flag (#838)
1a28b088968e333b35f5fce771f26f308554456c Add --wait to ignoredOptions (#837)
b37e61d5e0beb0ce263d52e4e1dd43c41557ad74 README.md: Add bare metal provider. (#832)
bf3618689ca9a05b91f6087c3364083a2ff2fd65 link to the gitbook published version of the docs from README (#765)
116e0e3f64498f187d0cf5e558136ef09a7851d5 Updated github bug and feature template. (#830)
be022eb328e75b4a941c1dc48475cc07e0d3ba17 Deleted cloud providers for clusterctl help. (#829)
26aa37ad8bcffd5b69e2a514b5e9a8ac30744134 Update architecture diagram from AAs to CRDs. Fixes #786. (#792)
c488193251e8e0cc557cbe9bbf09a61fb97bd8ba [clusterctl] Fix delete across all namespaces (#817)
a0272c47dc545bed703555176fc291e0cce8fe15 add error log for machine update (#819)
09b15f6a7934df079eef90bfdef1c7aa5296b006 Integration test skeleton (#800)
abcf6bf17e71600ca611f38b213719496aad6348 clusterctl: check EOF contains in kubectl instead of == (#818)
af298a2a480fb7143786cf4f9990e741855f08e9 Fix GetMachinesForCluster returning duplicate results (#816)
b59602c29d9d9d045d52deebf351a91fed09a951 Handle EOF in clusterctl kubectl apply (#814)
4708f8e5c699f26f2dfd1380ab0d52ece456ec94 Delete node on machine deletion (#809)
fbb97871c2fae9f3b4b4848b97385f50b536aea3 Add pivot phase for clusterctl (#731)
ca5119c1fb5b90a4b3455a63e7bce58fe35a6fe6 Allow to record machine update error (#810)
a2f5862d32c6c6600f60a2104eb4aa655aca720a Integration test to verify controller pods status (#811)
d2aa1a2866adbcdf42dfad6ecdf6676be3a44062 Update RBAC to allow node controller to set noderef (#813)
f73aacf58e67013ffe0a0e69065ff8d896931df3 Add missing flag to manager (#780)
bf5d7f45b814f45d4eea77fb17f360b79dc8638b Document release process (#768)
a7f1907b558e9d42517d83fa5a9be3d012b055af Rev the version of golangci-lint used (#806)
ff7137164399548f77d3a64dc2649b5e3fbdb0ee Fix an issue with verify_client.sh (#805)
e9f80414db98ed2bf35f23100f0da15a601a6fc3 Update Bazel rules_go to 0.18 (#804)
c66fb349d0104b45de54c148361f99effc5bbf96 Fix `make verify` failure after #802 (#803)
c51a9c13aa0ebe6d2d7bef869094b9b78bebcd48 Run gazelle after updating generated clientset (#802)
0c2107f9df1d5efd650f80e397a92c8622d979b6 Support MachineDeployment adoption of MachineSets (#799)
1695a9da6140bab4a869048cac6b866d96a47804 Update gazel and rules_go bazel dependencies (#801)
813b1fec840d79b37fe86778237b6db6d1cb959d docs: fix trailing period (#796)
2e84891d7f7b45bd3ef91357ec1cc13605ab86d3 MachineSet controller: Expose errors (#798)
163dc4cece4de696f4dae09fbbb18b00f45ac31d MachineDeployment controller: expose errors (#797)
b6e166eadac82b7690478d341540b509aaf82628 Set ownerRef / foregroundDeletion on MachineSets/Deployments (#793)
545c1dc7763576c10cb432c7f3b31364fd130100 Added bootstrap-only components to clusterctl as an option (#790)
f8d548b47e444972254fa23a91e626ecf7589ee2 Fix rbac of the provider implementations in the book (#779)
c077c33e153abdff6b173d58bd548d059864e9c5 Clarify kubebuilder minimal version is 1.0.5. (#782)
fab4c07ea9fb0f124a5abe3dd7fcfffc23f2a1b3 Add Kubernetes cluster validation (#679)
b0b14bc7f0b3269b7e9e3152f8d3db9258680ff6 Add foregroundDeletion only if cluster is nil, move label in types (#785)
a16ceaef0ccbda2798300d8540a2ec528092be03 add exec bit to integration shell (#774)
6078048472c1bbd2b1ed4cf4f458a683e3c6372f Move kustomization.yaml in default and use bases (#773)
7d71193de11511ef59f803d28e5c2750ffe27544 Fix Kustomize2 usage after #755 (#771)
acc581f1d965547ced8084e7e8df88bddec3c2c0 Cleanup machineset/controller (#761)
862bb3528cc48ddfbeed73fb386cffdb9a70831a Cleanup Machine controller (#763)
07f69ff164ed05b153ce06d95e0e76bc0cb3988c Cleanup MachineDeployment controller (#762)
3770c4b3a86050d05bdee066407047733a5cbac1 Load auth plugins for client-go for clusterctl (#769)
d4d6eaf9d677c6ac11694015b351244f973e6fa6 Integration test with example provider (#755)
6ea418254f9d60afb9695e07fb34415576c60c53 Cleanup ownerRef on Machine upon pivot (#767)
f46cbbda3491549af71fb50dfed5b679eff87463 Fix Bazel after Kustomize2 update (#766)
f888eedffc1e0b909f9bdef48782d08c22b27340 Add util.GetControlPlaneMachines (#760)
c64edfe8d97d91a970f48ed8d12fa5a114e5a566 Set Machines ownerRef to cluster with foregroundDeletion (#757)
0252bc656c708250bae308111b5fcbc5f25b5a80 config: Adjust to new version of kustomize. (#759)
eca8ab1849974505761a4c8b4b9fca53e0bb4569 Make APIVersion/Kind mandatory for MachineList (#756)
770a417aa2b56901e44a38c90574ecfbacb3de53 Add directives for setting ClusterRole permissions (#750)
e621840570ee7c8a3737cf8510f9fc07cfb9bdb7 fix of sed (#754)
256aac9982feb78e1790339f5b8945762dd3f056 gazelle: specify proto disable_global (#751)
0f315e945d5fabe0c805ccf30fa6cf02fac6c0b5 Simplify cluster-name query using Get (#744)
4b4ec3beb11a12335a3dc03169ee105f3b81e125 Index metadata.name for cluster-name label (#740)
a9f44d06cd84074d41d177482e3712346f961c3c Validate MachineSet and MachineDeployment labels (#739)
a3f503ff2a2fa4b3be612fab9edaf4f7eb7f1e27 Stronger link between Machine* <-> Cluster (#728)
ae564acc7c608c90d51684e854d3ca8fa36b1e68 Fixed creating clusters in different namespaces when pivoting (#736)
0985c76210c7d52f7757ed320a4ca671abf6a2fd Fix passing context from run validate cluster cmd (#737)
9153bcfbb6c08984cf5404c170c8c49100f01657 avoid hardcoding port in clusterclient.go (#734)
77046424d9b9b394c4f3929aed9605ba80d92715 Remove client.ListOptions.Raw hack (#727)
e8e1ffa4627fdc5d236a28960ee2d9e1e9fcbe1e Updated link to OWNERS docs (#729)
14b40f350205ba47664efa4e7c3ca34518dd92ba clusterctl - Add phase for get-kubeconfig (#624)
76f00bd582752e47f08fb6603acc1b01996a3a98 Use RevisionVersion field instead of CreationTimestamp to decide which MS is new/old (#722)
ef6f8fc12d32fc1646f231f6e39dbef59ad2e4dd Add golint to CI linters (#725)
e89a0e93c284a1cf1faada46b5e8cb1119f98c6d Make CRDs public in Bazel (#724)
4ddbf1af10642dfc862ea88f1728d6df92c606a7 clusterctl: kind should ignore some extra flags (#710)
3e0d97160821b7bbd000ebe29a9ed0cc871e472a Extend MachineStatus to add ProviderID (#565)
9d16c16ede4ed343ba8d2335243d2cbf1fc1d87d Improve YAML processing in clusterctl (#716)
86f4e2c49ab9cbc377f12a2e6252bb3f9a490e90 Add CI linter (#699)
6205b2ff434e2771b04cee21c9ff4d02d3e4ea47 Correctly initialize klog in clusterctl (#715)
ad8c7f35998e141466d111659e1a89e3acd212c4 Update bazel rules-go (#714)
f289c730dfad922d8e7f80bc138499df719efe9b Require providerSpec.Value[From] to be always set (#684)
ee38e8a3e04de08a406aa820fcf57e083a084257 Update controller-{runtime, tools} / Kubernetes 1.13 (#709)
76653f4302ca4eb3fb853540bf041f416849a2d9 use latest security patch release of golang (#708)
379c9ea63467a855f8dedcec39364c02f17dff77 Cleanup command runner (#647)
a735d786d4cb0b3d46b65cf3c95ad0de0a1b759e Update project maintainers. (#670)
40d9d12e7bf4e1d0c6a3453e018c4eed1007ae0a Attempt to fix TestReconcile races (#702)
cc36e01b54a36a3376730919ae0c4773cdad1dad Fix some typos and dead links in the documentation fixes (#705)
e6602cb5709957f9ab9f4c2a1b71226daed26cf8 Fix the GitBook link in the docs (#704)
2aa88253578695ddb71aee8e6f36b83f31c4bd38 Rename existing bootstrapper (#700)
2cd5299ae2ae92cf82177ad1dfed7f5b59824a39 Fix for KIND kubeconfig returning with newline (#703)
ca1e293c506a5ca10f46fefa86dd22e48d358430 Update alpha create phase with bootstrap.Options (#701)
5d44f738d01bb23f63a6c684f0e43f440359540d [clusterctl] Fix create cluster workflow (#698)
3b5183805f4dbf859d39a2600b268192a8191950 Use pkg/errors instead of fmt.Errorf (#690)
8ee2c91f4f0284b0c3889b2ec8cb543a2005db24 Add KIND as cluster bootstrapper (#674)
1cbe068126c7d2b0707986f2f4dfa84e616574cb Updated godoc for machine_types.go to align with best practices (#694)
47e12f681ebe060f881c9743dc2fe39898f2a1c1 Master -> Control Plane (#693)
c0744df028f2439f72ba33cea36097e219d87417 use the new link of the cluster-api KEPs in the documentation (#696)
3650286e9b87d3ba1c0f2a6a6638c892a6bd4544 update golang docker builder image (#695)
986acbe09bbad0df62e884114b86ca8615d2d05a Refactor bootstrapper flags (#686)
bbf595d53585a84b89797e48dd4afed5d122beb4 Add Make dep-ensure (#692)
302479ecef8149c5a05e0a4955b0871f85b7d991 Allow machine controller to function without the need of a cluster object. (#644)
361d0e2093c644834ca3faa38360203da04446d8 Fix pull-cluster-api-vendor-in-sync presubmit (#691)
de39827e02ae0090df1362f456c9e878fb327f34 Update meeting notes and zoom links (#685)
750b02221cd5c61afaf86d4a6f8e69c37266a681 Add JoinClusterTimeoutMachineError (#681)
3a856a4bbc6eec23174d1718573e215faa643259 Fix format of Resources section in book README (#680)
45f1c93260140936c610e56575d7505ba3d52444 Init klog in manager properly (#677)
c276229a1f7b2e833eaefed5a82c444ecfbe6247 Diff in testing (#675)
45386cd2120f2951c4268b8e110a5a8f54d9d914 Switch from debian:latest to gcr.io/distroless/static:latest (#672)
3ff8ab1ab64901a6e5c9ba787d78e5ad28aff9ae Replace remaining uses of Poll with PollImmediate. (#673)
633970eb5367f7e18a553c915e2616a03c423f5b update link to azure cluster-api cloud provider (#668)
63aeb2752b5f250636358b795793f2f53ce1c077 Export machine annotation key (#663)
59a129bbcaf29aa4354da68a7a8acd2085e4a43a Add unit test for machine controller reconcile (#650)
647ea14f19c946ae4e94e27dd9a151e99b651a6e Mark flags as required explicitly (#637)
f9737d633684817830056c9ec47a39fc6b34c826 Fix typo in gitbook include (#664)
25f6ea40d99f1ea8f4812ab6e5cc9fd8db6db699 Fix broken link (#665)
f03f47c17d09c4765a1bfdd204f8d814196cb3d8 Update controller-{runtime, tools} / Kubernetes 1.12 (#630)
cba244b06de7d29777036551e6b32817878d1fcd Short circuit return when adding finalizers (#627)
0e54da1ba15c4746e96bc9964049e048c7d7745e Fixed nil pointer crash in machine deployment controller (#649)
f81dd4e6f07954f0f6a31a51e4c43e1f762286c0 Polish machin controller (#657)
d19e6b6bc1d50383977e8f6795a06b7a3bcb14f7 Deployment unit tests (#646)
e3ee58fcca49a75349a98597860d8cc46607a2db Fix clientset verification (#633)
2f6ee4fb96fba5df833caf20966f8dc0102fa276 Re-queue delete machine on re-queue error (#598)
178b99aca9fee5a8bc33f737c8fc0c1985fbe655 Update Bazel to Go 1.11.4 (#642)
3405e6fb3ec73bb02e70c465b678604bb39549c8 Correct KEP link so that Gitbook will render and Jekyll will build. (#653)
307991045ad3d6fb497143ff5770a9b72f0b4cfa Increase machineSet unit test coverage (#643)
9c0f9874a7d759a8a7d714dd9073947eca53bb24 Typo fixes (#648)
4073f33f67178702cd1cef654a6217355e425730 Set the image version back to latest for development on master. (#636)
3547f8dd93078c0b0f0b221ee1c2a57f96673081 Set the image version for the 0.0.0-alpha.4 release. (#635)
2edce9534dce0be00f9a519d5ac64fca009639bc Refactor Makefile with help (#631)
11daaa39f21ccb6edbdd6b6c39f13423ded703f2 Add machineClasses to default kustomization config list (#606)
0173ea2753b7cca0fad8b05e04545edd7a61b0c8 Kustomization needs to work with relative directories (#629)
d01c13a6bff4d64a6b7a918581071f0f5c2589a9 Add a Bazel rule to generate yaml (#628)
03e4ed8c40c6b7c839fc4c864e6e39077170d353 Report only non-nil errors (#626)
b7724ad60a3b384ffc1f5aa423f0a4f02eea3e32 Re-order provider implementantions back to being alphabetical. (#625)
a5f9e61802c9dc9104abd41755d05be49dd42fa8 Local defaulting (#599)
473460ec3b6e95ba656fd7804b049b1d56fefeca Add template for GitHub issues (#620)
8d48d8f52dd509761a3531bf48e19179ee537f05 Don't swallow errors from ExecCommand (#618)
ca6843008b5c54b54843254cfbbca3440543901c Add {update-verify}-bazel.sh scripts for CI (#619)
8031e855bc89c4dd95cd8f83e1a0b697f4b94e5b Enable dep pruning (#602)
a29f9c42f491f569f5d7a385f4fbdd31b82280d7 Reintroduce bazel (#601)
eacf8b6b3eaf9a18cccee8d80727f4193b21bc26 Included context into docs of Machine Actuator (#597)
be43930f3c575b6774e1d1f6587553b3cd7d5b0e kubectl apply: warn on unknown errors, not just known errors (#617)
ae7f112366857789b654f0856ebf24d518ff01af Fix typo in filename: should be existingcluster.go (#616)
8d87e567c5fa30ad9ce1810d5f77124b91a40aa6 Initialize klog in clusterctl (#610)
4fb34c689c84186c586da058cb15ce98f8dc6ee2 docker image: move manager binary to root (#609)
b648dc103513344d5d33ebd13f1f1766fe3492a8 Add -f (--fail) arg to all curl commands (#608)
a2e81cff3ecfd85834298e855be7b5674cfbaa5f Add cluster api implementation reference for Baidu Cloud. (#604)
c413616bcea47a0548de6b8743389777ef21981b .gitignore: ignore emacs temp files (#600)
5a27d984f9af41aa4f952e7c36a11bfbfb042b83 Add APIs for machine phases (#531)
299c318690e526b7d8c704ab40a813c00ab7b0b0 Migrate from glog to klog (#587) (#590)
a2d800f3b12208a4254e305991d02f06d8238227 Add Machine API Operator reference (#596)
f8522af25c3a1cbcb304cf1034ec8d40d7153a4c add more specific machine annotation (#593)
0cf3e178cb103ee1d2324918695fefe4bb09a1e0 Rename ProviderConfig to ProviderSpec (#548)
0734939e05aeb64ab198e3feeee8b4e90ee5cbb2 [clusterctl] add phases for apply-machines and apply-cluster (#581)
05cb1e663eb4085fbb92321dd1235377c84567f8 Verify clientset generation (#589)
28783167a1ff3fc8c3a2605b36bc3409e1e83931 Fix the build comment for clusterctl (#591)
1fe6faa57da68399a785d49119cd8e539edf61d4 Create a phase for applying the Addon components (#577)
c82ed1236b6d596d1176a0ae2cac1da8e6904a41 Implement Scale Subresource for MachineSet and MachineDeployment (#580) (#582)
d7622d225b58c194a488c2f1491ba5262e85625f Add MachineClassList type to fix client-gen (#586)
a14157b8a1dfe78abb1a874dbf5055aa07a084e5 Add Context to Acutator (#579)
9f86c61769dced58fbc5b148209dccbdb1cf9687 Default kubebuilder test controlplane timeouts to 60s (#583)
d99e05c1fa4fa0dfefaed8e49d27e39510d860c4 Switch yaml package from ghodss repo to sigs.k8s.io fork (#572)
bb728b1bff29d376c3cd68ce2a1980421609dc95 machineset controller only add deletiontimestamp for one time (#569)
e59a4c76737aefaa2c7e32c8637ba132e830e5d5 add ref to tencent cloud provider (#584)
06a3b491efcee1126266faf3e2a8255f9df3d61d Update lodash to 4.17.11 to fix CVE-2018-3721 (fixes #576). (#578)
0dc85d0e4549d8dcd0c67e9f9482868a9f2b4f83 Invalid directory path in clusterctl README.md (#574) (#575)
df337dc437cb264283932914e67760d74af5ca8b Initial draft GitBook. (#566)
38096d689e4c045d400668cda72c9518c79f4ddc Create machines in parallel in clusterctl create (#563)
118ee9f08f78e0462f1d4a5756eafe6baaebfdc4 Create a phase for applying the Cluster API components (#573)
571cb480e561d1b1d49713e0a1db09de152dff69 [clusterctl] start adding phase support (#553)
fee897706a82938117591515fbd4e85e667299a7 Add missing flags into cluster delete command (#561)
14e43ea5a0a17e0dd3ea14c1a3d3a06e780ae8ed Add simple machineset delete policy (#558)
fa906f36843b065c5294501efe7d78ebd85c3c04 Remove ginkgo code (#562)
6fe3ecb17bdcdf096ede34104af87f79c2e90e68 docs: Update link for DigitalOcean Cluster-API provider (#564)
cf502e7bea904894770e6c1fe9b5170ba0cd4c37 Make MachineDeployment.Spec.Strategy a pointer (#551)
852541448c3a1d847513a2ecf2cb75e2d4b91c2d Add apis for machine-class (#488)
f80969d1a60cc19ecce34bb9f8db4acda369a11d Fix machineDeployment CRD for kube 1.12 (#549)
2d88aefcf94fcffbf647fcc1127a642112714b2f add call to return if machine exists and consider requeue-after error… (#546)
0a0313c785b36a81ffc74c486128ac8b0c12ab3b clusterdeployer: Apply addons before pivot (#550)
a33496d73d0a8091573b953a43abcc8fa54f1e7b Set machinedeployment status (#544)
19551f1e342dfef3c73657de8cd7db54594e95c3 Proxy cli params to minikube (#485)
438fe678f4cd9bbe0faaa436e8eed0e29c0b2017 Test MachineDeployment controller scale and update (#541)
3d2b6073ab61c4b617437419067e48a539f58dc2 cmd/clusterctl: fix broken links to "provider implementations" (#539)
4a2e2ec35a48d1694713232996d8bd7cee446cd8 Fix machineDeployment controller tests (#540)
70dec6624df750599dbf25b206020dca640fc761 Remove folks that are no longer project owners. (#538)
4ebe20374e825403449fe884e78ae4f852d077e5 Updated broken link. (#537)
b1a743eeebec45b0cbf1c08cfe2266a3e4c7e919 Bring vendor dir in sync (#523)
c06dd269d1f1927ea3027a0493db4d108199248a Add Kubermatic machine-controller to API Adoption section (#525)
a30de81123009a5f91ade870008c1a35f7ce4b35 Fix fmt strings (#524)
340f236eda654676d92439718417b72725cb3b29 readme: remove upgrader and repair (#521)
80129c0ca4eee12c47be0c04ea551fdd6f2cbaba Migrate to kubebuilder (#494)
f31486484d5b33c785540eeaffd47fe57832aef5 Change requeue after to requeue-after (#498)
b14c4f1f09fae544de7f5bf5a3bdeabeb33273d8 Update the error message to be object neutral (#515)
5e5c19e356b5b63912d62509d395d83eb8a04e78 Fix json tags for API types (#517)
f302034cfa525bd57a891532e761f742687e5392 clusterctl/clusterclient: use correct namespace in helpers (#514)
3f53b7acbf7f984dc8e5cab52d0dced4b283ee4f Cluster-API apiserver should be namespace-ed (#509)
00b1ead264aea6f88585559056c180771cce3815 Include API adoption in readme (#511)
d99b7630cf7803c40691b86f42ea99eb0e9128a3 Check if machineDeployment queue exists before using it (#504)
7db708b5df567c79e2e46f9c37cdbf001bef1302 Refer to gen* binaries using explicit path names in Makefile (#508)
21433b4ebc2db8b1cb6cc18e94c10ebe805bf851 run make depend (#507)
d9002c29dcfc69c0bc4060c221ecc81e9c3a9979 docs: add link to digitalocean provider (#506)
beba44a5e8329a274ef5a0cbb4a4ff1128f177c4 Fix machine deployment controller revision annotation update (#499)
5b128c0f9ab134087d1331be8176099201055a36 clusterctl: match kubeconfig by path instead of content (#500)
440bdb8a34a7ae9ef5355656662f21eaf6b78ee6 Moved clusterclient to a sub-package under clusterdeployer (#470)
ba672fe598bc56a7fd155cf959ca6ce6d1882cb8 Add vm-driver to the delete command (#496)
3b6365b480ef09006adea2c4f3131b824acff706 Support cluster API objects in multiple namespaces (#481)
eef14f32d16997c88815d66eccf86955a704506f Add requeueing support to cluster actuator (#489)
b52ca6c202221a19cfe504b0325b0698a90aff77 Fix bug in machine controller enqueueAfter. (#491)
35d26d068f82830253eb24eb659f4babb22380cb Add support for actuators requeuing machines after duration. (#487)
211cb357ea5f6d249857b3bd1d6dc0acd86df364 deployer: remove priority from apiservice definition (#486)
2d1ad4ce4a02270e38fa959f25c7810ece46939d Add node-conditions to the MachineStatus (#483)
3603557f635f6d0da0b96a035d618d2ecfcdf70f export getApiServerYaml (#477)
bbb8cdbd80b0090206a4075579b971c7a639e35f [clusterctl] Rename external to bootstrap and internal to target (#484)
e1903be683739379be57f78a4095cd51726495fd Expose the "--kubeconfig" option in the kubeadm wrapper (#482)
051f338bdacb76117d73a86258bc58c946add7b5 clusterctl/cmd: improve error message for not implemented interface (#478)
32c2e4dd770643207b1f92be442aec2f4c5af5fe Fix a broken link. (#476)
a67bff65fa3387b067c3b973305e403c4829ba3b Update links in the pull request template. (#473)
cc0efd3baa96d396ac54d2e4cf6b0d72e46ba87b README: Add implementer office hours (#474)
029d2bb3a51767d7fe3d6188dce9bf2e9f144521 fixed errors from running: make verify (#469)
db54bbbbb896e0e8919f95b7f7921b12461e3624 Reference the official git repo for vsphere provider (#472)
c8f5046fb0b9a3a16b7f8b92f6dda7b0f65b4f55 Makefile - Fix VENDOR_API_DIRS for Fedora and add openapigen to generate target (#466)
af7ca338a20ae7d74c9f96c13c975556b33be679 Openapi gen (#464)
fdbcdd0c7965941971f195be43d0e1389ec265cd fixed missing apiserver serviceaccount and clusterrole bindings to make apiserver work. (#462)
8b0d9949f196d5e5edc20e7ae4f63f591e99bd38 Regen bazel rules when running make depend (#465)
24c7b1bc913f62f4e67a53d3c7ecd41c0b20961d Update docs to record `etcd` requirement for all unit tests to pass (#456)
213e59ef76b7eb18f318e786ff0031c7df36f684 Add the google group info to the README.md (#461)
f17f564b95d074a09cf034c7071c7ed727cf3d44 Allow to use existing k8s cluster instead of minikube (#442)
2ec8be38bec1a53404362273ae059327b14a1c83 Only log a warning if there was an error (#459)
597fe239184f6593f9cd083ab5411e9fa2bb140c fix wording (#457)
4cd646d0a760fbce0e25a370b5fac4f200344f9b Add goflag parsing to pflags (#454)
977b11a0e9006feac85090aa8ee32481f46e94e8 Move clusterdeployer_test.go into clusterdeployer package (#439)
28cf28fe792e1c7d101c0565fe8c0f526e573215 Update bazel tasks & regenerate BUILD files (#451)
472c6f6d48756bdf4b8ea728a65e0463c84ee367 Add glog/flag workaround to controller-manager (#453)
1b0db9b0a3047aa203949c0c537cb6a0af2c3fba the rolebinding resource version is missing the /v1 causing the cluster deployment to fail. (#455)
0980af3dad42d3d1c4e2e605a7b96560331e8c12 Update documentation now that the provider specific code has been (#445)
0b2f26f79437b89020123187ee87c1a2a15f479a gitignore bazel symlinks (#452)
3b8fab15ea41e1b799e2247695ac7403a4513dc3 Bump the image versions to include api changes to remove machine role. (#444)
cd629be6f02b0a2d19cb78b16fe3c26b0a1000d5 Prune dependencies (#437)
4d5326bd92ec2e88ecfff7488deb27492f99fb74 Fix typo in validation cmd options (#443)
b90c541b315ecbac096fa371b4436d60ce5715a9 Remove machine role from the MachineSpec in the Cluster API (#405)
cacc2838944e0c226eebf0c3fa7a98dab090f4ff Delete vsphere specific code from the repository. (#440)
ecc34cd5701c179a556f5f82d382c4f1ce5b0906 Validate cluster and machine objects (#298)
754ae19804cf21e42449acb0ac3a0b8507e113d3 Machine controller spelling fixes. (#441)
83ca2bcd9e9141b907a7817fe74e78e310526a88 Delete google specific code from the repository.  (#438)
ce93d949fef1c4547c421c016955862d600857f8 Updated pointers to repositories where provider-specific work (#433)
a7e3b5ab5a9cbfdbc5288e03df92f0e862c292d9 Delete the deprecated gcp-deployer directory. (#429)
babe91030553781cdf12192a2875f90dac5b5a00 Implement clusterctl delete cluster (#406)
05cc4dd79151b6e5d2f484498499178ee5e0abe2 Fix boilerplate and gofmt (#415)
7f897d33754ff939d2327296e7b6127f2404fa1f Change PR template to include a note about image versions changes (#407)
012aa2d0bafe135676ba931b61f32cbbe571d1c7 gce cluster events (#401)
6fd6b3dadec91bb95daab62c9a927641f483938e Make a deep copy of cluster prior to calling actuator (#426)
46520acea98ba02861b2feb51f425952b7b34828 provider/vSphere: Fixed case for vSphere in README (#428)
029a374fa576ab5be2b22ede20b64308afc839a5 Better way to register and lookup provisioners (#360)
b770dd7b06fb75834ead5169db85ea79b6215563 Include links to known implementations of Cluster API provisioners. (#408)
dfa371814c0b39a284662b897ba9b5df4749e973 Bump vsphere-machine-controller to 0.0.11 (#412)
f74e110cd9cb4b24fd8dee6008cb8fd79485dac1 force http port in node startup script for vsphere (#411)
777bd0885d504ac59eb1857187eed0839637c29a Make addons.yaml optional input (#404)
ba6caeefd14f292bb8f69d38b7712be31c2ec80f Add service account user on master node service account (#403)
62a8fea5b877fc390eb0e655a4b9e2fca1902346 Add missing Get / List, Create, and Delete methods to clusterclient. Add (#399)
ea56da472b4e36607f2ba4812a16721b32617888 Add create and delete events for in vsphere amchine actuator (#381)
05bee7cbfe431c2bf18f1a16ab3bf68eb89ded62 Add MachineRole to the GCP-specific provider conifg (#400)
5275e59ea67903e63a282fc369027ad3fe01b525 indicate azure provider implementation is in progress (#395)
7539ca9938a145ee92ee8efc8fcdf0dd00385662 Fix an issue where cluster actuator was incorrectly using the kubernetes errors library to determine if an GCE error should be classified as NotFound. (#396)
90d79ea06ae5819e7132f15c6c431a5b6472f5d9 Generate api and deepcopy for unversioned cluster API (#394)
3784fb37e847e17b6e5972c74fc8125ef54c4727 Add 'cluster', 'namespace', and 'user' options to delete command. Enhance delete to load provider components from cluster. (#384)
3d9767cdbbbb9f5c7473e6130df5d9e1730a43e0 GCE machine controller events (#387)
e4074127f7fe12506ca8cb9c7a25c2c73c7a7025 Move from (f *File).WriteString(...) to ioutil.WriteFile(...) to Fix a bug where WriteString fails because the file is closed before writing. (#393)
4d8056541f2a63389943aca373baa3baef5a7f30 Bump gce-controller image version to 0.0.15 (#392)
4c5bd3cf799587a33bd4b9a9140775289da43b27 Fix an issue where clusteractuator.Delete(...) would never succeed if the firewall rules it is attempting to delete do not exist. Move GCEClientComputeServieMock to an appropriate shared location. (#378)
138f08be69a918cdc7a7804791fdfc11bee2422f Fix an issue where clusterClient's temporary kubeconfig files could persist after the application terminates. Add comments for the clusterclient New(...) methods. (#390)
88b61a30880687286e2080ccb225c7ffb446c9b0 Align api generation utilities version with other k8s dependencies (#391)
206c730a237dccf733c2e2b8c746c1fd6b3ea424 Protect against initialization race and switch ETCD images (#388)
4254b785009138d1692a1cd20327db43529d7fea Change machine actuator to stop removing finalizer. (#366)
96a45c7b283f486ddfddc47c23090cdbf66a6d9b Update README to add credentials for clusterctl create (#386)
f7cec809b21900b6cf59fd99ef495dcfacb33e82 Add images to "make all" target (#382)
42a94cf39928a1f5c11e0c7438ba87255d277496 Add network addresses to machine status. (#346)
7dd04a1d55f616984e6934570a32821d77063cc0 Verify boilerplate (#359)
a9881d5c9c5d20c193c90dfaaec697ce30c2d1bf The cluster name in generate-yaml.sh is now a random string. (#370)
91dabb684df847db401363c40819f0cbff5237fa Plumb addon support into clusterctl. (#376)
ada5f05359a2eab27e86217289c7f48ed3e1d8ea ensure dep is present && avoid images for now (#380)
987646fcbe6f036f28d15ca64eb29b467bf02cb4 Add "all" target to Makefile (#373)
dbc1c953581a594a6923de638d422a23774cdd98 Generate deepcopy by deepcopy-gen (#371)
975036fc27c10590b23f9b4e06e82f7a9e762e19 Fix a copy / paste error with GCEClientComputeServiceMock (#377)
76577fde95b6f845fa4cdf1eef5791afdfa0297f Improve reliability of saving provider-components to configmap (#374)
58ebae2a09a02c5938917782a8a662cd66e479f2 cloud: google: inspect error type to determine 404 (#375)
9f861145386c5aac01363650785e1263dc1c3b9c Add firewall rules in cluster controller (#352)
eaa3c8e9bab001a5f8bc600b3243b3c26a6c269e Enhance `clusterctl create cluster` to save the provider-components YAML (#363)
bb90552b819d5d1b40533857de96dbd524986374 Add "reviewers" list to OWNERS for auto-assign (#368)
9b8fee24854c426643b5652cc8a7893d4a1283ca Generate clientset by client-gen (#367)
96b45e69c2cf8c802214c01cf47a9343c8738656 Increase clusterclient timeout and retry intervals (#356)
6fa53551f6d317c4682b24cc4559d341635e2d78 fix node startup script where it wasn't base64 decoded (#369)
67f25654d60d462567cf3619610b1ec556a807a7 Refactor serviceaccounts.go to make code accessible by cluster actuator (#354)
cbc610ddc55fb85bb552df0e4cfd385f66443003 Add an optional provider-components flag to `clusterctl delete cluster` (#362)
9d967f1dc58dd7f09ffc3a7f32ed63be2ff73f84 Move errors, kubeadm, and util under pkg. (#361)
e9dead97849736dadc67ec20c815265dc5b58ca3 CLUSTER-API-159: Enhance vsphere-machine-controller to fetch kubeadm join token. (#291)
e8c516948d48eff984120eefa44e71b37aa19035 Add copyright to the generate scripts and enable better error checking. (#357)
3a38a8edfc20d38f7f2c8f24755beb5a932b9869 Change default image to Ubuntu 1604 (#351)
0ae30e844247fbcdb1f3b9138847c534f831bf73 Refactor: move clientset / rest.Config methods out of util and into clientcmd. Add convenience methods for loading api and rest Configs and creating clients. (#344)
b3ead881813f619b932a4145ddbfedb7c4ace970 Use 'tr -d' instead of 'base64 -w0' to be compatible with running the (#355)
5997a0180f13725ad1f6769e8263c426b15d2d96 Improve machine/controller.Reconcile to intelligently block deleting a node associated with the controller machine. This will enable external machine controllers to delete any machine/node, including masters. (#350)
a331adef2ed7ec5fac4ef305df8bc165cd5145cb Add copyright & license to kubeadm.go, improve comments for Kubeadm struct and TokenCreate method. (#334)
9e0c2decc55209e26df1c6bf70c4f6b2cb805f6f use variable for startup script path, to avoid collision on machine controller (#341)
796717b1015443923da1a26537d1dc117bb4e6c8 Remove dead code. (#353)
90be184c47d54898f6dc48f02f87e8124ea017a4 Update minikube driver information (#313)
bfdc22a0f3d30eb85b0f0ad4d2f748a7ca64c0d0 Change the reconcile logic to include machines being deleted (#342)
3b00279761c7222ca4a4e5ddd4dd088cea171a2a Add creation of a necessary GCP firewall rule to clusterctl/example/google/generate-yaml.sh (#299)
800864e72e2f2c5f9f165eebf497ee14a89f5694 Port commit '8168f74afc2508e5b10fba5fc4eb1c69e89c32e4' to the new controller main.go (#349)
a589fd0262295170d2291064475b378407bfc5ba Add the node's UID to the machine's noderef. (#348)
62c58dfa8dae1b2eddbf58cc9000e4ec8b6f8f77 Add mkjelland to the cluster-api OWNERs file (#337)
c639337ce35a27101e8a840f0aad023dbbf921b7 Increase clarity around external cluster cleanup (#330)
ca0cee6dc55488509894d94697fd00d4df392581 Reduce total duration of clusterctl tests by switching from wait.Poll(...) to wait.PollImmediate(...) (#331)
011bb82049bfe9278ef91744b8e89c6355ed750f GCE Cluster Actuator (#242)
264cdcf9789eae783adc14a0008b07d71a3d18d1 Add wrappers for GCP clients: cloudbilling, cloudresourcemanager, and servicemanagement (#285)
64491c9e5f5b20126991b0bd721375c48100d644 Fix test race for non-default namespace test case. (#329)
fbc85d97affbf5c9ad97054c66b23ad2bc0ca097 Update vsphere README for machineset (#326)
a2d82314583c02d557927446779b292d9f66642f Bump memory and cpu for etcd (#322)
1419eb20816262f0a89711629902bf0ffd73cffa Add machineset.yaml.template to vsphere example (#318)
3ef823a3ee9d7be5f2bd1424dee22e5cecaeb8b6 Bump controller manager rev to pick up machineset controller fix (#323)
367b3832e4eaa8aa2f1fe4f5dfca5b0bca63896b Fix the race condition by confirming creation/deletion of machine objects (#316)
7fdecc5cc4b4174ab5c540a027fcfccc7183f66f Fix a bug in ClusterClient's GetClusterObjects() and GetMachineObjects() (#321)
ee9a08e8ac0b52357c0aa7d81e86ca6c82d88d7f Remove terraform provider (#315)
fbf5762c04b2d2b0a9a7d2efbb3d4ece3ade6993 Change google/generate-yaml.sh to generate files into an 'out' folder so that the generated files can be easily manipulated. (#311)
870996535a86202e2205e05d02298e78f105cdca Bump memory and cpu for apiserver (#317)
51b218c4c63856b04ca44c919a7243c43ce6eec1 Add Parallel Queue support for vsphere machine controller. (#314)
594c00f94e0c58629ad63da223ea1eb30352ca55 Make vsphere variables map type (#309)
06d3b2eaf8fb7fc5c691dc57c3d1116d156d7c02 tiny typo (#310)
730ea2d3be765d7f8cd71ed68e1d8c3bc163a3c1 Update vsphere delete docs: no node labels. (#308)
8a21ba78fd3de91a6c92b6c27241876941369745 explicity use bash (#307)
982993b1e5d906e9190b3e5d3e8fe8c12d0fc1fe vsphere generate-yaml usability changes, timeout for clusterctl (#302)
578ec1b4f1585aea6aa2696b8ee3fce8cf209743 Fix Test race. (#303)
405008c06ce7d80627bd9bf0588ff49789711026 Enhance the error messages returned by minikube to include the command that was run (#295)
f05ed08d3ede1948c4f146a6ceb8b2199d5c6830 Remove the NewCmdDeleteCluster method from delete_cluster.go to match the other Cmd implementations (#300)
86ffc8e620aa02a5842161a0b2c969b5c999d490 Delete vsphere-deployer, tf-deployer. Add deprecation note on (#284)
6f1708e989c7c9871f9a5d2f041102f4360da952 vSphere master control plane upgrade (#294)
67ad3f7e94660ea26fb85e400df56d35bbea7478 Add docs for deleting a vsphere cluster manually (#286)
d66f37ffc900d704b178ed1973fd82bc41f05aaf break out provider deployer logic (#293)
57efe550e628a67d782bd2de34eb2b02db1f90e9 Bind cmd/delete_cluster.go to 'clusterctl delete cluster' instead of 'clusterctl delete delete' (#283)
a047a3f9386b5480fe9b562d664825dc62237988 Remove hard-coded default namespace dependency for machine controller. (#156)
03620400c949a0a157ee7c0369df6d3dfd00932b Deletion guide for GCE cloud provider (#261)
9169950b97458947b5e268d018492168b0bc488f Remove control plane version master set label on node in template (#272)
6aecf9c80a1ca29b45cb43ebfd50ac0d57eb7132 Make delete node work for vsphere (#282)
5a03ce32ad36794c886cbeeb340d88f6da146e04 clusterctl logs, tf state in no files, base64 encode state (#280)
099b4e2e373df6732b65f8a63250fd114d6de373 Small docs cleanups (#275)
9fa9a542dca575f942c2e6270ce93357fc72a8a2 Add integration tests for clusterctl's basic 'help / usage messsage' scenarios; update the contributing guide with testing instructions; remove glog from usage output. (#237)
b966a2842282030eee2abd10a1cdc9163e8777ab Move test_cmd_runner out of the 'cmd_runner' package and into the 'test_cmd_runner' package to prevent test flags from being included in binaries that make use of cmd_runner (#278)
77096e1c8ef4fd7f238a6e0978ccaa4aa7cfd1fb Add more temporary error cases for kubectl 1.10.1 (#277)
8f83ba01eb3df00555986c1f8631ffbabdb606bd Ensure machine path exists (#271)
0ebed4afaa26bce89ffacd60d80e607442785747 End-to-end functional clusterctl create on gcp (#268)
1b8d698cf3bfd837a8326944f4e3caa45e844ccd Bump gce machine controller image version (#267)
6ef7148c37f4fdd84c77a550d2b641c0a1b12b03 Working vsphere clusterctl example (#263)
f104e0edbed3c426da116e233bfff6ad5ecdfecb Move tf-state to machine object, and remove file system dependency (#264)
1f11e62bb326cf42469640c87f77fde6f44c3ade Fix SSH issue with in place upgrades. (#247)
a3b39103e3f0233b41729bd48bb38738859005ae CLUSTER-API-159: Enhance gce-machine-controller to fetch kubeadm join token. (#199)
8a7fc1d35f96ce608c2a5563c8d96376ddc05b58 [vSphere] Move vCenter credentials to Cluster provider config (#257)
25bbb3f305111359e5b38592f5e1b1e8b222efba Rev the controller manager version to pick up machine deployment controller (#260)
cf9bcf60c732c2ceb9989c78a9144ea25c369e93 Initial version of clusterctl create (#219)
66a0c117af408e28b26952aea26a98cfff0e35b6 Fix a race condition where machineset reconciles too quickly (#246)
e929a2fc09f20cbf2f1f4e80146257ff69456d0b First pass for machine deployment controller (#143)
7efe24b769e0421c9c50acb4b3c5dacf18f46955 Use Calico as the CNI provider (#194)
a9086b6b6919c534f200d016fc1ba74183dd7a93 Enable integration tests and verbose logging on the continuous test run (#243)
bf96e6b29ad866083a47c776dbf68629d300b61f Use the control plane version for kubeadm upgrade. (#251)
bf2fea154a5a170a2d24919ea40d6ecd5dc0c01f Copy terraform code to vsphere code (#241)
84813dfbfccbfa0878cb770412fdbe919763039d Bump container versions to pick up the recent api changes. (#248)
b28d8a6277e7a7acd5513f8dce78b64071fc5953 Remove container runtime version from machine spec (#240)
90100b15453a4a711b03548ad2bbe37cf5829e06 Update generated code (keeping the manual edits). (#239)
f69bdf5fd0b0ea4900003ccf4bb9a90d4a5eae7f add basic validate cluster command (#203)
e4be6af77215fb1a598332afb12c97ec9216ae33 Cluster controller implementation (#190)
851a4b40eedd60ffaab6ab25d5ba40412523e4e7 Revert changes to generated files (#231)
34f4e2223d947aadb6655957dc11bd4c7b429eb4 Move cluster-api/node/util to cluster-api/pkg/controller/noderefutil (#229)
ec20d6aab66b4073b039a1b07c1a278d3071ff5d Remove the terraform binary (#232)
107e3b3e7fe474f95b49a0bb7966f4d3be2e1018 Standardize location of AddCommand(...) call (#228)
b455dcef27b36688221f39b6d3aa36aa872894ee Have machine set controller watch machines (#186)
c146d3b811944ce0cf5b0c0e95808cda64012f86 Expose Kubernetes scheduler and controller manager to the cluster on Terraform (#220)
ae0ddb3f1504d5d0e75cd407b3af8e6cba660eb0 Fix bug with deleting machines in non-default namespaces. (#189)
b4e5feffc55202cb60885452d13b89cdffbc0073 Parallelize deletion of multiple machines to reduce total time spent (#223)
ee0ebee21459fc2be65a030c47361f87303985cb Increase the the polling timeout when waiting for machine delete to complete. (#222)
dca6686d61173e370ab0f297f06dd1bdfe8a48ad Expose Kubernetes scheduler and controller manager to the cluster on GCP (#214)
5354cb37c4661085224294b0b9d922b099bc83f9 Typo fix:kubernets->kubernetes (#215)
8168f74afc2508e5b10fba5fc4eb1c69e89c32e4 CLUSTER-API-205: Initialize the 'flag' library to remove error message from glog (#206)
d53f94f37eb6a071e536998441dae2f3885d2672 Fix the meeting times in the README (#179)
a082a277bceaed15ae79f61b2ebba66201828ac4 Switch the base image to debian stretch slim. (#213)
79f7f6ae71ae7332558ceb175933489923fd649e Fix typo in minikube_test.go: call Fatalf instead of Fatal. (#207)
9545eb3069a84a977806987b09bde2e17f6ec69c Splitting GCEProviderConfig into GCEClusterProviderConfig and GCEMachineProviderConfig (#183)
2461d32bb4f6a8988410fa47a08bfcccb4cab971 Set up node and storage management for vsphere (#212)
d560c7bd8be3536bae598ea92866861d6630f334 Add SECURITY_CONTACTS file. The list of contacts is equal to the 'sig-cluster-lifecycle-leads' alias from the OWNERS_ALIASES file. (#209)
b18e725eb70057a28f03e216caf4db300006a3b7 Clean up adoption code, parallelize deletion. (#193)
0be24796eaf4d56d37f81b42d6393f592a31968a Add @k4leung4 and @spew to cluster-api-maintainers alias (#210)
a1ea634ddb1c46777bb46e68e56488b27321a9e9 CLUSTER-API-52: Allow CA and key to be provided on cluster creation (#153)
4f4785c16212fd80c8693cc4cb1ff96051f1e538 Add provisoining of external bootstrap cluster to provisioning logic. (#195)
59410e28f2172038cc970282798d1fb2ad1c601b Implement machine and VM deletion in terraform (#185)
44dc88db087416d1c84f784ec00a853d26e4f17d Basic create cluster command with required flags (#188)
cd39d3261e5c0a8267ddef3f7b4ecffee196dd9f Populate machineset status (#180)
65f050f503192b4918e689610a124d03cc05a895 update machine status if node ready state has changed (#178)
69140e0a31c09d31de34603d293bf7b45fe9478d Update README for tf-deployer (#184)
1ec9ada77db0ff2616a348f412f416f7ee3bff6d update Gopkg.lock (#169)
b5655d7348fe817b7ce5b0de60c115d495b997c6 Add instructions for iterating on a developer version of gce-machine-controller. (#170)
a81a73fe840bc970b7b9668c913c10006c228f7c Merge pull request #77 from spew/kube-deploy-638
c0ffba966c0b12d08d775058f4617c4bfe03712e tf machine controller needs private key (#173)
ac9edb9507e4f4fa7be5ec852a94af8fbd617dcf Bumping the GCE controller to add ssh and pick up other changes (#175)
c0f2510456f3e02bfe468c4e97406785de3db0b6 Bumping the controller manager image to pick up Cluster API changes (#174)
30eb6d1b5dbcf0069a7fe6bf2a33cd7ee70ec32d Add the ability to configure disk size and type for GCP clusters
4e00ee98ae98dad17537f83be729f2f4ca31dc61 Merge pull request #141 from mkjelland/gce-cloud-provider
d1e212fec256e2037f874bef3999d11057275b84 Make terraform use a non-dev controller image (#171)
3d9c8e17db2d2d16e389a9882606930fda481830 Fixing typo
5da5ef38b05c5b3c87690215a0c31a5ea91312d5 Merge branch 'master' of github.com:mkjelland/cluster-api into gce-cloud-provider
bc25028fa50abc1b531b54801fcad6e2411d50a3 Bump GCE machine controller image (#172)
8bc47be796d39887075ad2f7be2eae6779f5133b vSphere k8s upgrade prototype (#138)
5e323ca383afc6ddb4132b4fe80bd08ff3817374 Merge pull request #166 from spew/remove-startfile-hack
2837ac5a15308497b542f9f86ecb57123411ae40 Fix machine deployment defaulting logic and add unit tests (#135)
a819585acdd31d18737018e87879147ab691807b Fix a typo in GCP Deployer (#155)
268ffa32620285385f970e9761d435011dcef72d Adding the '-q' flag to all ssh commands and remove the 'echo STARTFILE' hack from all ssh usage.
d5f110c5f1c8acae7e6a85b31a17ed68a962445b Merge branch 'master' of github.com:mkjelland/cluster-api into gce-cloud-provider
068787c6919447f0e24dd311e43c851877a34e4d Adding post create step to cluster creation to allow creation of ingress service account and ingress controller
fd68ff1f9a70c09db561216f5e2abfe8cb28487a Add boilerplate for clusterctl (#119)
4e08c2f75b1b4308647fbfd6aedc3200690c9fb5 Fix service name and namespace in cert generation (#148)
407cffa957dcd54254f0510cb969226d3691c7a0 Leaderelection (#134)
9da56b2d58d1d4acba758145eaa74fcfb50946c7 Update gcp readme to remove openssl and fix command indentation (#150)
6c5568373236e51974134fd2ded9bd8957026e7a Add prefix to error messages to help determine in which step it failed (#149)
40197e8671cbbd4e96e7bde5c291aaaadb0281d1 Update branch location and image push instructions (#123)
fc4dc6a5aada32bf1d99cfa95cd867843a4a1c26 machinedeployment boilerplate and remove internalversion dir (#142)
4eb0d896f23f5a109086a9841bbc0a0f4a205486 Addressing code review feedback: - moving ProvisionClusterDependencies method to machinedpeloyer - Updating ingress controller service account permissions - various small cleanup fixes
3a8f44a9091ec726b8f2c89b4fe58e06673ec4ae Replace openssl with client-go/util libraries for cert generation (#144)
7bad547e531e86eaa2f639d063989a679d40dca1 Refactor GCEClient: wrap ValidConfigs in an interface so that unit tests using machineactuator.go can inject their Configs instead of having a dependency on machined_setup_configs.yaml (#130)
9e19e0bb24cb2ba0ce9d7d845cbdffceb8374687 Fixing build issue by adding new actuator method to test actuator
1c94324bd134515314d70fad43415fcce93e663e Fixing build issue by adding new actuator method to terraform cloud provider
3e3813ebc8e7183aed1996a7303cf011648859fc Issue #81 Adding instructions for deploying ingress controller
62e051616cd4a4275ce83d2785ef3485adc384d2 Issue #81: - Create service accounts on cluster creation for master/worker nodes - Add default storage class - Start kubelet with gce cloud provider configuration
5d5cdec6cf1208bfb4f63e3b2cd48154a12d52a5 Use ubuntu cloud image with OVF (#140)
7e593cd16e76cbd4162ce8e1e212c9b0c1b7aeb8 Bump for #133 (#139)
2c50f7414b69ea2940f418eac6244784332c54db Use RawExtension for ProviderStatus in Cluster type. Add ProviderStatus to Machine (#133)
a2163f420d88162d68347f17661fe1a81871f5d6 Add/update documentation for machine setup configs (#120)
ed967099d8f326318f07a15c85b2ca034b9fe5b7 Update sample/machineset.yaml to use os field and match docker version in machines.yaml.template (#126)
3ff99ac48dfdc0bc2a222dd6ba99e6f4b0995519 Bump version for controller-manager to pick up #108 (#127)
c406f69ae8e149f683de3d209576397b66c204c4 Remove docker version check (#128)
818a6d1521dfa9425ea84a53b37e55b80da7b494 Move cloud/google/machineactuator.go's version of GCEProviderConfig from internal to v1alpha1. (#125)
5ddf7788f9addf3788666f151bdb73133ef5a731 Bump machine controller image (#121)
029f15be7c227663cdd99f80ec4bca499b66ae57 Add worker tag to all VMs to open firewalls for load balancers (#117)
bc5a8d37b08d3ace68808d30c8a0b61442183b12 Bump machine controller image (#116)
ec53b5b32946270f48f382e7295c631fac530623 Use kubenet instead of weavenet for GCP provider (#107)
79317f9ca55ea2f8b626f6c2c4ff342bcd17c5a3 Refactor GCEClient: wrap compute.Service in an interface for mocking GCP compute (#73)
a4f58439a3f93d8884e65dd595c0e0f9d6614819 Correct the network configuration to allow the master to come up successfully (#114)
fbf0415a101dea6196ac9893449920e39191faa9 Bump GCE machine controller image (#113)
ac64a124f588ec75d990466a85b8cc4991e81511 Add owner reference for machines created via machineset controller (#108)
01546946a9de60dcc724ed7b6599351b16871708 Prototype of named machines for vsphere (#110)
70c282dbcae4ef9a6b9d7012491150f2d0f1a650 Implement parallel worker in machine controller. (#74)
925c784b3ea6fd13f67d9d714ae909869915e396 Templatize the zone in the machines.yaml.template. (#105)
262113e72fb0857d5289e5b804a5ee3f639a6ea6 Handling configurable machine setup/installation (#104)
180cbdcf74ff8c6e9671d6dcf2f7d8910fc4e8f0 Add a vsphere provider and deployer prototype (#103)
df991ef535792b2bbec5242d63316cfd153ab5e6 Change references from the 'kubernetes/kube-deploy' to 'kubernetes-sigs/cluster-api/' (#102)
3799ce25112013c1bb740ce5e470d52b355d7083 Fix dockfile to new repository location. (#78)
a591e9a19f6debb0a078e96e6d930ee1b6556d54 Add .gitignore for gcp-deployer files. (#76)
0291e83e9c4c39958bf5906dc4e0c607d8157748 Merge pull request #71 from krousey/move_repos
a38a8740ed3e7a16f4f50a2a2d212d6ec1014996 Reverting the removal of provider specific code
a9f06b0f4871bebd8a3f3fb555dccef676605cbb Remove google vendored dependencies
e5c0ffc24ab683decb9461ee014a35a86a9977d6 Delete provider specific code
0596954320e8bbdf00003b325ab03eff4b60b894 Fix markdown after move
fa549fba8c1596341b137f462d4a2e3160d1d608 Moving everything up a directory
566da0d436b40fdcf7a87dab253c17cf671103c1 Removing the imagebuilder directory
797929e9ecd41b38493ebb1676c1fb231dcf2ba0 Fix build files
28ff7015f366be2debd3d6cd33b8009c472aa13b Fix markdown
3cf25650bdece7f326741f771e31794a484c6966 Change all references in Go files to sigs.k8s.io/cluster-api
7cd3a9e95cb0c8e56a2c4a70a133dfce79ef5e35 Porting owners file from kube-deploy
e3015ba3ff32ac649e66ee10d7d1217c64553544 Create README.md
f3ce6eb4d827898e8a2f3efdb7e8ae90ae9f3651 Initial commit
5b2cb44970b3d3180a08682b706dd37e5687ed33 Merge pull request #684 from rsdcastro/master
58c69592c0010462c008531c9a2fd813b2c40710 Update link to OWNERS doc to new location
676dbb81bdddcd62240a866f2d61e498730216f5 Add reviewers block to OWNERS so blunderbuss can assign issues
214883e7445d5556d95e5bfa2d37a4bdc3c9c338 Add more collaborators to repo maintainers list
de6c8ce68985ae942ed24d3e1f6ea6301864c7c3 Merge pull request #682 from jessicaochen/external_stack
5e824036b7ca6fe2eb99d4588a2feb26263081de Bump for #679
2f88565ae4573e8e660b24f5b8d251fa95f6ac7b Merge pull request #679 from karan/cluster-fix
23ca053a60f60729f6aac458753a71ad7db98134 Fix cluster.yaml due to providerConfig type change
15d6c662adcb28a2a81bafa4e5f3b093194025a4 Merge pull request #669 from k4leung4/delete-finalizer
8228e1d8247cfe24e46c0a7949103fba671b002e Merge pull request #673 from jessicaochen/bump
e131c0e475a1be75a7042b0487f6b2630961d1d0 Merge pull request #672 from craigtracey/cluster-provider-config
82a6d2267229b09617f9e41e7f93f79bd0909481 Add check for whether finalizer were removed by verifying machine updated called and machine object no longer having finalizer
d4ed9d1e19b7a1032db6f0efff559841c1dbe3f8 Bump machine controller image to take in https://github.com/kubernetes/kube-deploy/pull/671
43761b4e00335e47adf698948c299d385f38161c fix imports
5bcd9803c27f768237e64ad573dc7ba6e491d457 changes from review
cee175d40e5b9c8902ad2012dc3adb722a4aee92 Merge pull request #671 from jessicaochen/no_uid
4a266646f434e3e33b14e1a7543e42fe57e3fbff Move finalizer removal into machine controller library
b2d0e0f1c34ecdacd167d0bbe7f6a791dbc67edc Remove GetCurrentMachineIfExists
384c644860d14e6629cc98aac6436a515c7c3c54 Update comments to reflect common type adjustment
78e85840874776387baa570866481fc60012082f Update vendored dependencies
d62e9485b3914f141a8849f1e9cab0163f651734 Update Makefile to lock api generation utilities
bc2aab49513c726c91e03f5162a81c0874d230ac Standardize ProviderConfig for Cluster and Machine
3f38f610363a55a277deba84b251f5e290cffbf0 Remove use of UID for identity checking since machine finalizers prevent machines with same name but different UIDs existing at the same time.
10af41c92fcf32ff9b16cfb4d8d014e7f67ef652 Remove machine finalizer if underlying instance does not exist
74a18bda2a0427be1c3774b52f2abdee2ab9963b Merge pull request #668 from krousey/fix_permissions
1a199bf24825ab351864d8835be52f45705b4c0a Add make rules for correcting permissions on GCR public images
ef2f9f85b5384afad2057fd3cf9cb7ce7763e4d4 Merge pull request #665 from k4leung4/delete-machine-set
759df761f5e0b4d8370daf655c7036812a5f71d3 Include step in prereqs for gcloud login for creds
5841a611617ddce8d06d013bbae469659c42d0f8 Merge pull request #658 from maisem/md
f50e9d6a8b678ac53d473c6afb628d446675d193 Changing the machine deployment strategy comment.
a3a36ca4db8c214680f69ce3a47818a5170d9290 Generate code.
2d01a3c584f632762ff559b05f8b378ab96de435 Introducing MachineDeployment types.
c5d9082b477b7ebc45dc7b2c330a89ae29fc99bf Merge pull request #660 from maisem/dep
58b5d4bcaaaadca55dd8c907dfea6c30ed8401af Regenerating files.
1d15e0a5f8275dd206cc1d855de90b31d92ba0bc Update apiserver-builder to 1.9-alpha.3
4778d1dc52caeef88c4c2718a1ab9ba773ed5e53 Regenerating files.
a046fd5d4727effa3783298c9cf6e305e452d6b2 Update dependencies to release-1.9
5915eb07cb1f7e8fcab1dac95423df5167f11e59 Merge pull request #649 from krousey/break_cloud
7142854c55e72a8a8cf24877f7b69d06d58b0a0b Merge pull request #648 from medinatiger/dev
39cf2de32c630902256b5d94a1b42e878d6b45c7 Add a positive test case
085b6cc77f67c11de1e24687b3d17514f1fe7c4a Use a test util function to return a vanilla cluster resource
d384a92dce5b28e73fef2b31fc22ce0fe66b673c Break the machine controller's dependency on Google Actuator
7609988ab8739fe2c3f2e0d505db6199e13e45dd Add Validation for cluster resource type in apiserver
4a0341fce3a490494f452c336f60de1757d47b40 Merge pull request #657 from roberthbailey/update-sample-machineset
0c54a939c850a335c8f525d19c13d2e0832001e8 Update the sample machineset config with the new provider config.
b9cbe2a774490067674b6b6c724f7d32c725ac89 Merge pull request #656 from roberthbailey/provider-config-type
aebafcdec59e42ca27d2ea46431503200778429b Use the newly generated code for provider config (fix compile errors).
aaab479af8f873e11a8737ff86aa493aa53b28e3 Generated code for provider config change.
3421339d404898a8dd033070047befcdd9acfa78 Change type of provider config from string to runtime.RawExtension.
c6a4431a80759d756664e28eaf432a686a3b88cf Merge pull request #655 from roberthbailey/directory-rename
58906d61cacdfd257d51073f8360b315d5ae5a78 Rename imports for the directory move.
79def32119f32ff56e1e85f4184506328f19bfd3 Move ext-apiserver -> cluster-api.
90efd821b03e2f34447f5b9d7dc5e54cf1ec38b0 Merge pull request #652 from roberthbailey/updated-machine-controller
648b0c660f3247e677079f26071556d0af243262 Merge pull request #651 from roberthbailey/delete-client-side-machineset
243f34121beb58d0007c03273bbf26be0178bb35 Update the machine controller image to pick up https://github.com/kubernetes/kube-deploy/pull/644
f752d5b128268e57735ea5f119fab5a92dcbb885 Delete the client side machineset, now that we have MachineSet in the API.
ea2d9cfa51cabe5e2249665c6cea6b4cb15b468a Merge pull request #640 from jessicaochen/bootstrap_doc
98cbfe32443f4bde8152d93e04f48a258aaab0c2 Merge pull request #644 from krousey/servicedomain
1f4cd7064aa1d3b6b54cebf7917da2dcae2611a7 Merge pull request #647 from medinatiger/cleanup
51273814a53f97b3c65474b5d32701829b7c33aa Fixup dependency.
e4f55b853bdbb48058921bd81614bd7e66fd84c6 Update CI scripts
05647507eaa4f9005e479ef7b0d310005b8adfbd Delete cluster-api and cluster-api-gcp directory.
136cdac3cd60f0d721fdda528274f048d996bf70 Merge pull request #620 from p0lyn0mial/initial_machineset_controller
fbd6836517c00563210d91b4dfc220ff1ba080b6 Regenerate code for service domain change
40d225f044ad8f9143b7a6f45ca8f69960aa9d7f Change DNSDomain to ServiceDomain
dfbb3e24d2db80294accb3536dcf20f91c5adbab Add boostrap guidance to contributing guide
e48c0b7823ac755c26e9212d8e72e2351ae9aab8 Merge pull request #641 from roberthbailey/cluster-lifecycle-leads
4a858b5f730b14e8ec0423e3e354d6aff9710192 Updating owners aliases to reflect changes to sig leadership and the github teams.
c6dd38f2aa7effe5f8bbb92f5f566b093ebe6782 adds labels and selector and removes OwnerReferences
4d8e94db3c530816249edc367ba817a6d22e5893 initial implementation of machinset controller
edf4ba7cb64997234cd9746a3daacdb703584e2b Merge pull request #630 from karan/retry
02880155fb191e80db248b8df36544f73d906e46 Remove apimachinery/wait dep from deploy_helper
40ff83b8b2ebda791e6c1544df03c9d0e740b301 Merge pull request #628 from karan/retry
2af4f8a3bacdad1ab9b1618cfb9dc792cf75732e Only print error during bootstrap if err
96cd040279247e0930a63a0929ce286ab703325c Merge pull request #624 from kcoronado/os-image-config
f46a90351f597a820e19ac870f620a0d464b018c Merge pull request #582 from karan/retry
f635201cd721f9815bff81f9c07c5d69e154bf3d Merge pull request #618 from medinatiger/readme
96b9d731a8824fd59ffc448c3d3a2a5e4149961b Add .gitignore file
159dc37f063c1172e1ec578dbf95daa0edf1a1e8 Add retry logic to ext-apiserver, port PR #559 as well
a40d723e7081ba7dc636b9b007aaa0d7b42607db Renamed imgName to name (can be family or image)
ba63b52ab040c2f693d2d24900a630f2180917a2 Copy the documentation over to the new locaiton.
ef4bdc88ca07e227f804d141c2e6b90247484f99 Set image preloaded to false for all cases
42069f86eba43135de056d17e859df8bdd1a0254 Start adding a 3p retry package
201b26a1957af113f69d2c29865bdf133cdc6a00 Get OS image from provider configs
9fa1e1f9450120f70b5c2ea25ef332184fde7c65 Merge pull request #616 from medinatiger/machineset
f2c929b3a38e6c75009f2b1d7fc92b60550a3d31 Cherry-pick the machineset API frm clusterapi to ext-apiserver.
d90cb4e0c37a27afe4cb940e93d00d6e9aca0964 Merge pull request #599 from prateekgogia/imageConfigurable
d0639422e91590f8496bca7c0687a99590bca41a Merge pull request #622 from kcoronado/convert-ginko-tests
16b5a73a1a5939298ff9e58e0fa31cc1cd9b12eb Move controller/machine tests off ginkgo/gomega framework
7fec0678d8963c118900add5ebfeed37a6348566 Move controller/cluster tests off ginkgo/gomega framework
eaa5a3388a79fbf83c683f597d7e9e1218f6f132 Move v1alpha1 tests off ginkgo/gomega framework
f17c5ea49833d495c22eaa3589fca11eeca7cc9e #571 generate random name, if generateName field set in spec
790edace43552f8861463755243eab59b49508c7 Merge pull request #617 from medinatiger/docs
aa7eb75dcbe08cc97ee286c83826a97b313b7af6 Port the tools to use new API.
e5440d03d67265429d9a0069a1d5820fd0b67b6d Merge pull request #606 from medinatiger/cert
3e8e72bde8e290e6c439213195c9e1f5a3f29500 Merge pull request #614 from medinatiger/merge-machineapichange
32101b97894ca49e0a0ce69136ec77e18513643f Add missing machine api proposal.
054793894a2b6277b675cfa2ab83ab2ca3c8764e Merge pull request #615 from p0lyn0mial/regenerate_client_code
3f0c08f9712e9240ee7ef43bef487cb0243432dc updates generated code for MachineSet
cc39e4f4c7f597f3bcc84e9649a2b64b54603d4d Use openssl to generate certs
f39fc27bb8ca212a224fff5254cb539a9ed889bd Merge pull request #605 from medinatiger/dev
45eb1919f7453a79f658dd28bc04f72e5bae92b4 Regenerate code for Machine type change.
f729862db3a740ade4ec1654393ae7985d5a0a77 Pick up PR Minimalistic Machines API proposal.
9c4feaa54a8dee36d62c47035a437b6ccd31932b Merge pull request #603 from rsdcastro/update-readme
20d3e150d98616dcdbeb437f5d7acb677359792f Merge pull request #610 from krousey/fix_tests
c5f0660934bc9c7d0ecaf06b3f590ee319be9b80 Switch to listing clusters on demand instead of caching them
3ad33459e765d89932bb252a81bba762c4f0d8f3 Merge pull request #607 from krousey/fix_deps
31f86826f081fdc606bc61f0c83a583910a10d0c Update client dependency to fix a race condition
6a36c97a98255dc4bdfb45a366d96ace4d9e81af Update architecture diagram to include connection between controller and main API server
3b0d0e63782dada8c9ea31ab1ad9d5c8a75ad9c3 Update diagram to reflect the vision for bootstrapping machine
16bdc447fea6e716857eeea229fb9b35b02025fe bake deploy template into gcp-deployer
19f6c076ebc99d0ccb5b937e15ea2c258af35cf7 Merge pull request #602 from krousey/fix_deps
82d5a30317fd3b7738c8be4eaf26676043f1caab Add architecture diagram to README.md
4c347e1b73e181e0a400f3b44a2ca7a6f5914309 Update vendor by running dep ensure
6b65d02ce4b89fbb75229619acdfbe744c053da0 Switching from Glide to dep for vendoring
1c1e306c94c79062cfc7a1a1da556eb4d3592331 Merge pull request #577 from prateekgogia/mergeKubeConfig
b88901b774866a3b4c7202e015a8cdbe8cf7f09a Fix missing bracket in deploy_helper.go
2afb7dee42179836ace4f4ec18c0c324532629f5 Merge branch 'master' into mergeKubeConfig
b8bb7a9ad863f3d2f8259e34ecec6ac14bd3cbf6 Merge pull request #501 from kubermatic/add-machineset-type
04dafdba6db0102496e770a4c06a182b40883ebb Merge pull request #588 from medinatiger/nodewatcher
c3a7bd92f76792bc90f394a941062787b06ce1d4 link node and machine resource.
2bd54716feb12d31a526bc35cbbddf00b26eb01a added ErrorReason & ErrorMessage to MachineSet
6a526faafa4d39206c0be8084b9b3cb1778bc909 Merge pull request #598 from krousey/fix_tests
d48e775b48bc772452058e30117e71c74e43106d make machineset.spec.selector required
22a1e8f6cd2ec73f18770e8677a25406158e66e6 added missing fields
3bbcbb42bc888a454690fd50217a3083c08f2667 add MachineSet type
bdad1224330badb3e144a11332c09f2a55aed850 Clear finalizer in test so it can actually delete
337c68f87ddb6487d16262ddb101da08aeca722b Merge pull request #597 from krousey/fix_tests
b448cfccd6871a5bc830d4bbf467a0529d84bd39 Merge pull request #581 from medinatiger/finalizer
6a14eb192a581b139a5bb49b34a984c15d40739c Implement Finalizer support for machine resource and controller
b6b4ab95acb521eb9959470829f53b0bd2c2b8e8 Merge pull request #572 from medinatiger/dev
173c6133582b7060e82000d95451817f44c5f2f8 Fix the machine controller tests
252cf1e51dea24883276bd766fab101f9def8964 Plumbing the new apiserver and controller manager to an in-cluster deployment.
9ebe70e6789e6593929e872aa22def6644e8f326 Merge pull request #586 from rsdcastro/update-firewall-instructions
619a8d7ef72f2c7c110fbebabccfc6690a5a36e1 Take a copy of cluster-api-gcp util code, change the API reference.
676e9f291628dea287a92b397c96bcc0eab5fdcb Merge pull request #590 from krousey/buildscripts
bbb7a7250e239407d841c9b9acaed632b637e61a Remove newline from test script
48cfa97024c02ce3e17a5e038df0671228e8671d Merge pull request #569 from indigoid/imagebuilder-ec2-instance-role
e9af43f815210ac6e97d856d16801b855257bbcc Merge pull request #584 from krousey/buildscripts
8d13e3da1c3a4689d059edf69cb6bc42f8ba6705 Firewall creation should be after gcloud was installed
4eaccd6649a50705dfc04c36c4ff90a7967d3992 Add a couple of scripts for CI
dfcdb553268d9f9ffcf0cdb23205bd7063ddf4a8 Merge pull request #575 from karan/unit_testing
880a554f9f360930e48271d65b6001a772962141 Merge pull request #583 from krousey/cleanup
b47077a44f6331a8adfd6bb0923c6e0a17eca773 Delete internal informers and clients
c7e2f623b1e46a25e4b853b1817d39b4ba7288be Add google API to vendor directory
ca3c25b7639e02fe8813906e8ee73051140c5ded Start adding unit tests for GCP actuator
a53df90a2efb1ac6fdeb15c1f786be45eae2da27 Merge pull request #298 from pipejakob/machines_proposal
ff3a7fc44c8bd6f92e62be38b55ce93d5248539b Minimalistic Machines API proposal.
b3e1525d0df7a2b4bffac131acd1c7b55fb5e03c Merge pull request #580 from roberthbailey/pr-template
c9a9c463af337c8aae4887fa55aaa13b4179ab84 Add a pull request template.
8dcceaa3ff8a599dd0ba89ae570bd4b40146595c Fixes #424, merge new kube config with existing config file
f09968eb28d8033595f0a3700131a3fe836b0e77 Merge pull request #557 from rsdcastro/update-readme
d9298804a6589b9acd731296262c241fab4aedc9 Merge pull request #556 from karan/contributing
31b784178ddc42b96ac4ae8530f2eca7f2cacbd0 s/cloud provider/provider
6259bc5d05e8591a811f7e3f1a961ab278bd9cb4 Merge pull request #574 from karan/unit_testing
f03daf57701cb573cf09b72ab9e404d0d2364755 glog.Warn undefined
d2a3c6b00659e3fce3549c844543076130b849a4 Merge pull request #568 from rsdcastro/revendor-kube-deploy
da370ebff71e07cd2877f6c65e80ebcdb219351c Merge pull request #570 from rsdcastro/update-service-account-message
f8a9cadf39358da6f77b3324ebffb20916634e56 Add instructions on updating vendor directory & move some sections to prerequisites
02784da55253c43940bfe456a7649c05de94f798 Update messages on service account to be more explicit about GCP service account
7ea3858b6bdc4d025560241ce8439251aa65cc90 (opt) assign an IAM instance profile to EC2 instances
ebdcd671e583c953320c157ee8b42873b6a518f1 Revendor kube-deploy
3bc110fb7f736d515d057d0d8dfbeaa599d2edd3 Remove indentation from other commands that don't render correctly
d7dff8eacfeab1950d1baa7884c44eec7510ca6a Remove indentation from command that doesn't render correctly
01b000d87021c1dcf29f67a587920bc32757ff1f Add option to use GOOGLE_APPLICATION_CREDENTIALS back to CONTRIBUTING.md
a70a18bf02eeafda8c66a69dd700b16bb41ad715 add note about label selector, change MC steps to ext-apiserver
764096ff061911563fae6f196b46fa1a366d06d6 Merge pull request #559 from karan/wait_sa
96dd7bad0a6197e35a272e2a98e882d04101c3a0 Check for config file, readability changes
8b1447c0fd6628476387b93dc9a4c0245e98b25b Merge remote-tracking branch 'upstream/master' into wait_sa
760c8e423e826f61afb7b7748bdb1761c8a30bed Wait for service account before running machine controller
eb3330811e571f228e1a8b27449825d9e2014ca4 Reconcile README.md and CONTRIBUTING.md to avoid duplicate/conflicting info
777bf5c2c4c48d20cb864e702098a3eda0bcbea5 Add docs explaining basic instructions for adding a new provider
413e1a6d03b93d8878e1ef7d51d9e4e67b7546c2 Merge pull request #552 from rsdcastro/fix-owners
afb1766db46dd6c48e557b88856e92fe6d31b7d4 Merge pull request #555 from rsdcastro/use-gcloud-for-project-name
8f650f1ad098167a721bf1f814cd57f41e422f1a Update help message for force-overwrite flag in generate-yaml.sh
fcebb2ecdf0dac0d21158234b66f399a9da8904a Add details on forking repo and flag to overwrite generated yaml file
cb42479ef394268882d9fc7cf31e252e441680c0 Fix Makefile to the right gcloud command
bd785f0444d1524b3820f8771465901be6f0a84f Replace - with _ in variable name
a04f4fcc4502080d96dbf2849b76e2b58e42c1fb Update case for variable github-username to match the other variable gcp project
9d0b5e6c1809912cb988af2eca576b99b309d968 Update git clone to use forked repo
7792a2c61dc8fab6e3e341be32dd7eb557799720 Revert "Add me (rsdcastro) to the list of repo admin"
5ab6a5ffa79ba2b11912ad2fdf4afa9610ee6a7e Revert "Move me (rsdcastro) to repo maintainers rather than admins"
c53d4c0089a10ab7b5cd0cc1f1976a020f4872c9 Add link to Docker installation and tweak first instructions.
1626a31e74d25420d4241cd4f23986b4c2b7acf2 Use gcloud for GCP project ID info in Docker image generation and machines.yaml Update CONTRIBUTING guide with more details/steps to get started
e10470fbc65c06ea7b8d71b48fd3996ac344fa8b Move me (rsdcastro) to repo maintainers rather than admins
5fca9ba36ad68d994c4796b5062aa6b5a0607d8d Add me (rsdcastro) to the list of repo admin
33f130d366774283caf9581938195eed68a09c6b Move me (rsdcastro) to repo maintainers rather than admins
fafc50e6420783179fd5fc7d73c7453f1de68eb4 Merge pull request #551 from rsdcastro/fix-message-missing-kubectl-config
765803e7f39529b978240e1671115c51858cfd64 Add me (rsdcastro) to the list of repo admin
9f66b4c73160de4c646d08c4e80e2735e2718c8e Add more user friendly message if kubectl isn't configured
079a33ce38af294e6caae7f021ed34de7a6f4b6f Merge pull request #549 from karan/contributing
549a7ee63fbff5adb29f1b90645b43ae86df775c Add contributing guidelines
2350ba6ead914bfbd826e043fdf9866a35fc6677 Merge pull request #519 from karan/machine-status
fa3d2c54cc92279929c934b6aba569201c5eb78d Get the GCE VM machine type and zone to update instance status
c7cec0fed858900ff381c065fcc70dd1d20d82f9 Merge pull request #517 from medinatiger/dev
69ba6d4f2e5d25682c99b9c150476e12fd42249c Init hookup for machine controller with cloud package.
d57253dae7577c56e81961c146cf26e4f3ac1a1a Copy the cloud package over to refer to new type definition.
998b9d2941553441f522f1a29341cfba85fe21a0 Merge pull request #513 from karan/deploy_log
94f0fad34a3a33bac45a6350771777048209918e Update OWNERS_ALIASES
7701ced3ec7c85a2334d99e3822d14186a9a8229 deploy log should tell the user about node creation latency
4017a6f8223773be3aafd1c2fac373012715c64f Merge pull request #512 from roberthbailey/slack-channel
16da8bce002eb10194cea5f54147c6be07e90f4a Update the name of the slack channel.
f001e36c7d2cef44f9cd2945be13940aad942ec3 Merge pull request #511 from roberthbailey/cluster-api-readme
1d9ff0ae7e7202471c01722546eec1dd6883d47b Updating links.
2b5547e32932381c1adc73cf7ea6500c1d9288af Merge pull request #509 from medinatiger/dev
b831e47be103d57ceb5bd9affde034df1a845d26 Rerun code generation tool for new type consts.
16218bc249015d201b3773832ebb63065b54a075 Add Status const in typedefinition
c05f006348f3de67a704693b1ccd797b0e685bf8 Merge pull request #507 from medinatiger/res
b4742b4faf6c9e0a4ff4a7666338ddf79e3e7589 Rerun Code Generation tool for the machine and cluster type change.
99ba03c78f679c4ee48c5480833936f3505d283f Copy Cluster and Machine definition from CRD to ext-apiserver
cf9763b46fd27e26998ef4ee905cb4d19628357a Merge pull request #506 from medinatiger/dev
99d8e921892a1752913e33488c440f472e69a986 Build the apiserver and controller-manager executables for local platform using bazel
b4af69c8ad4b61964be8ad157eb35b9d35ec7fc6 Run code generation tool to client, type conversion, informer etc.
3727d00074596c4e596b6c9ebe0337fd48baece1 Merge pull request #505 from roberthbailey/owners-link
5d0aa008f18c957f705e3596f9155f8bd68f7e53 Merge pull request #500 from roberthbailey/gcp-readme-repair
e624aa73834c9870266544f6f4c6337f19894926 Update the link to the community owners documentation.
012ec5cf2fe458d47c5d619d78d63d7b6a2cd2e5 Merge pull request #493 from medinatiger/dev
1344a042b5864e79a11a55d055db7e85bd3de2ee Merge pull request #498 from prateekgogia/kubeconfigIssue
480473e17a423bd864f616a797ef289e108485d0 Kubeconfig env variable and alternate locations for kubeconfig fixes #495 #497
6182b2a768066f26c66a6f885858ab0101ed5e1d Fix bash command for picking a node to repair.
cdac7f1c5eead40bc2939043b9e43ec768915972 Merge pull request #496 from kris-nova/flag-typo-correct
b8891eb1624fad4e8c1444622b686ef5a6dd9d1b Merge pull request #481 from spiffxp/add-owners
7a78b730d12fa28a41c92a228910171faa239fd7 Add OWNERS file, OWNERS_ALIASES based on current github teams
0d4ca1d740e96030edfdc5ed0a2fac067e1f996b Fix typo
3aa4fe2f7659352f4ff655bf2f644e4fa9d6af7d Change the domain name from cluster.k8s.io to k8s.io
45d06d7d4ef0904c368ee06a500fa2aebb43d359 Bootstrap a new api resource cluster.k8s.io/v1alpha1/Cluster
82b0934728ed827fe107322fb19a7279d0fadffe Bootstrap a new API resource cluster.k8s.io/v1alpha1/Machine
64407ead8574e539fa55e020d08f910cf6f44367 Merge pull request #488 from roberthbailey/delete-binaries
545ad2d76713e7047307b6ecb59dc860ae414dd0 Merge pull request #491 from jessicaochen/master
26a8a6539ecdb2edea184708cc48a797dfe42870 Merge pull request #490 from pipejakob/remove-bins
9e23ec335dbe7c73834ed8e3383ec2982c8f855a fix gitignore
5fb6e3a76224804642df98ac1bfb85fd9968c3e7 Remove binaries that were committed.
34410382eb92bea4e258b11ebb26d61732631828 Merge pull request #487 from roberthbailey/gcp-readme
c2d89ff9a5b117c09f69f64246dc3ef8d4a5061c Remove binaries, since they shouldn't be checked in.
ff9db7d7c506f9e55d405747fcbab4fb81b20791 Revamp the gcp README.
0261206598c988a38320518067666ba8e1b83ff7 Merge pull request #486 from jessicaochen/firewall
16c0f0d266e0c03b9cd1438ebda16d547a3e8e75 add firewall rule instructions
a5b2c7e180fb0f4d75532f9216fe2ef30eaa10a4 Merge pull request #485 from roberthbailey/tidle
33524ee4cb7ce0c1655c74204ed1ed6c8ad7bda6 Remove unnecessary file.
3b55277dc04b8f901511832928ffa8488462a9dd Merge pull request #478 from medinatiger/dev
ca1d236af13751b6373a0f2f2091e0dbf69670b4 Merge pull request #477 from jessicaochen/seperate_deploy_interface
97b1922bb8c958980b6fffd26b477e57cac5cff3 seperate deployer provider interface
9fa65b6b0d6a65a78b6757952e1df8c82fd198da Remove Makecerts, which is no longer being kept up to date.
b57733043cc5c57ab4055e15067d74e7433a51ee Init clusterapi extension api server project.
ded7a935db3e0c4d6a3a5c50e9c781d24371a366 copyright bilerplate
036253c41a51467764d944198ec5b1595d8c74a9 Merge pull request #475 from roberthbailey/makecerts
f8fcd866d8e149bc47b976d53b84dbe3f6bb5dbc Remove Makecerts, which is no longer being kept up to date.
24048245c524b2142e76b0f580fa40185ef5c631 Merge pull request #304 from roberthbailey/cleanup
084a33b96e584ab112c6cc56ec57fd30ee70d970 Merge pull request #450 from justinsb/image-1.8
519af810b7d25112a86edd900a74bdee7ba82013 Merge pull request #462 from spiffxp/add-code-of-conduct
3d761c0ac8c39e6de79318ac74d7f6686881ef01 Merge pull request #466 from jessicaochen/master
68e27e43894efebb45f5f014aa5510c11015c3b3 fix packages, vendor and network ranges
84b510217c16360bdda5f95dbd08bba3b21da61a Merge pull request #465 from jessicaochen/organize
6d2d75afa095ee6d5b99a519bee0218dd5f9b6b7 extract gcp code
4941352d4d53348385ddddf5ad0e1ebbce77fc05 Merge pull request #464 from krousey/cp-types
fd3257dcd802a46d5c0a33ca25b1640bdab8469b Making network ranges more flexible in representation
6bab1fbf7a0164625fc2c83c82a0038aa641904a Add code-of-conduct.md
7ae471ab04238448b55e3cb9bf321fa2d2671976 Merge pull request #461 from jessicaochen/reconcile_machines
c3db341170e98a10fd26cfe9244b3c82dae40aec Reconcile machines
7740d8ed527ad5804e60864443aab28b7aefee56 Merge pull request #458 from pipejakob/landing-page
9abf2c4e0fd497d9a4501bb9e5f92e06ff8557aa Iterating on cluster-api READMEs.
fd4ee45e6493bac5421cfd0a849f6a82bc4f49e5 Merge pull request #457 from pipejakob/landing-page
e85ae005558759438c11d1c6dcd69f6e1fc6038c More README cleanup.
f974bba32142a596a9a785b017b96c0e513ac00d Merge pull request #456 from pipejakob/landing-page
d070de7a382040a0cc81eb342dd5c81c4e161f78 More README edits.
68dcc0de39bef635c735136f63709f8ffa9fa38e Merge pull request #455 from pipejakob/landing-page
b1383bc7bfed08fe48fa3f1f6c91854b73d4f053 More context links in README.
0999818c9757e058b36c8bac044186c62ad76d0b Merge pull request #454 from pipejakob/landing-page
c7cd8e2884d19a7b3ca101f8ced292b5df947d27 Linking to Cluster API doc in README.
42fe221265088b2a3a21ffeba8a485537f3f9930 Merge pull request #453 from pipejakob/use-prebaked
5367fbec61feb706920904d63fd8dea5fa598847 Use a prebaked OS image for GCE instances.
660cbad716558473c9ae8130273098435d5fa3f0 ENA driver is now installed on jessie
6021f6f3619baff74e2eb2300afadf136c1363ee Merge pull request #452 from jessicaochen/safety
0116feabf24f081ed4394b0bd705be758343c507 check for CRD on machine create
f33b50a8f95a52b150c0a6b668841b6a373e2508 Merge pull request #451 from medinatiger/dev
00ff0a49c09e98ba8ad58ec828c3e2ed4ed8e63c Add more information to the landing page
6d6828f43e32b371ffe457a782b02840f80e642d Separate 1.8 AMIs for stretch & jessie
538ae0e9e9386ccd003da589d1b4f6eab2832be5 Fix dkms for older bootstrap-vz
0c9a8423b1f45914739d670b9ea687da1271dc97 Create 1.8 AMI
9472e033552e627969f89e3b81c405a6257c35ab Merge pull request #449 from justinsb/copy-snapshots-in-parallel
57cb00fad2d73fc743342edad09e5a744a9992d9 Copy snapshots in parallel
4762a98569dc4bf77ea3da6c3eb32817c019b126 Merge pull request #434 from justinsb/stable_revisions
c87f1c09654012f3d1885cf31d0a59e901fa0b79 Merge pull request #447 from jessicaochen/delete_clean
939f69c29e4d948ad85a6d39288c8a57427c4e08 cleanup nodes on delete and annotations on clone
a02bba68a51730edb77c08965945126fbddb87be Merge pull request #446 from jessicaochen/clean_scaling
ef93308413be6d0e103ea00034715b7a26ee0845 Fix missing returns in node watcher
55107cd91690228876f780bb89418e871f8c48de Merge pull request #445 from medinatiger/dev
11caa3a6edde4f6f9955eef2cc662f28b098096f Choose correct master
2d04811eba456cda510dce647265d8c8fc3c0007 Check NodeRef if it's null before pulling node status
ccc8d0eec0bdd579d16ab82a71948023b0c4de25 Merge pull request #444 from roberthbailey/repair-typo
02081a2baa58c74a64cf00be553317e5f2396bd1 Change %s --> %v since node isn't a string type.
cd2124f44d274965a80e2bc6dedb922fc61f1a33 Merge pull request #443 from jessicaochen/uid
d8eda011779b4f97ce7df4cdc425c2e46136baf1 Cleanup uid
61f28178bede0d4ff2a4438014d726957f205ec9 Merge pull request #442 from krousey/split_templates
98a950ec02646c843eb51ed583430b070fcc1c39 Separating script parts for preloaded images
607a79445f5587e8cb8c2f747e4eb4ad70f268f3 Merge pull request #441 from jessicaochen/parallel_machine
fdf30cf5e0a462927f843caa8dd38586d9ea9e45 run actions against a single machine in serial fashion but against different machines in parallel
068b7cf9036b7a9befdbceb8edeb64a718c760b2 Merge pull request #438 from pipejakob/build-repairer
6eab5058010e0a309113fa93d32aed119ceb8482 Merge pull request #420 from medinatiger/dev
f313924b414cd0fc20271ff15d5f0e3164ee3e82 Rework the output msg for upgrader.
642dda1b4fab7ebaf24f5e44e8d52ef2fdb6915d Merge pull request #440 from krousey/repair_flag
1b8070c7b110ca250379e0bc6a258e8e17ac6f63 Change repair's dry run flag default to false
58a2b108f5087a59c1ff14c46d08ff9f3542d901 Merge pull request #439 from krousey/combine_apigroups
ed139455ab9a4cddc555f11713439b06269dd91d Clean up metadata generation and general validation
cd1dcef78dd2021e76a48401e57324b2f3997721 Add timed wait for GCE API call to replace busyloop
578a91e24e903aeba8dfb0c1fa2707f7535b87fb Add "repair" utility to Makefile / gitignore.
cf31c4de8eaf984aa25d58da99a158c093e769df Lock to specific branches of bootstrap-vz
d1538eadb83612dadf433f65c44e5b2be3f170ae Merge pull request #433 from justinsb/tweak_imagetype_in_other_region
752a685336c37bf8e98b18ace8231d12a8dc5112 Merge pull request #432 from justinsb/imagebuilder_goimports
258c9f6561d4453cac39b8bea7ac50be5179968e Merge pull request #431 from justinsb/imagebuilder_fix_replicate_snapshot
3d298b89651d4877d895b77ed2d43019d6532faf imagebuilder: Use a different instance type in us-east-2
5778f5fb81fe52cd8b69c83073bcdfc14e1d511e Make imagebuilder code goimports-clean
5cff3e5843b5de4ba43b4c4d45dd352264b5b457 Fix for snapshot replication
4ebe7e8bbf2079bf2cd30565444682e67343f310 Merge pull request #430 from jessicaochen/node_name
ed04939ba1acec3e6a2baeae47b47e2aedb77ddf Label VMs with CRD UID for later retrieval
3474cd855277172fbc55c91bb33a05bdce328d01 Merge pull request #292 from bcorijn/ena-support
d6424f3e0ddbcb118ed9d222c82315d084bccedb Merge pull request #295 from gekart/master
504cf67a35effe4dfa0494ae937bc2039e6d1278 Merge pull request #268 from fate-grand-order/master
9af7847cc7b31b15abca07490336cbd23d514bf5 Merge pull request #429 from pipejakob/delete-redundant-file
5716c5066222ce8a4b4e4bdb690bab8cd69001fa Deleting new-machines.yaml.
b986853325a2f8cb6e3fb4ca25cbe55b922a4bd1 Merge pull request #428 from pipejakob/fuzzy-pkg-versions
17b1887a7dfd9aa7d214952d11a48986b55621bb Use version prefix matching for Debian packages.
fef29ddf7cb9936d7c363430b8b644bb104f8370 Merge pull request #427 from pipejakob/ignore-upgrader
680a7510a505fdd766da737c8840deb0b5d7bd00 Ignore upgrader binary.
fad0595bfd188943fde5752fc4ddfe23534159bf Merge pull request #426 from ajitak/master
d980fbcedc4782cec01822a8676615e54e1cd5fb Delete master vm, service a/c if created, if cluster creation fails
798c05cfc3ff9648f11007ece4797407116202b4 Merge pull request #425 from ajitak/master
f3325523cf123a0dbe58a82a7e7423884282a732 Create new service a/c for each create
637701a3b377bbda9af6e8ccfbef4330103e1963 Merge pull request #423 from pipejakob/delete-using-annotation
7d09dfd9ed7c1961fdca4b7bedfa7c4088420212 Refer to annotations when deleting GCE machines.
9cdb6879a015c75b8caea27b725f1bdf82bbc9b5 Merge pull request #422 from pipejakob/gofmt-l
133fc8fd06168e2598fa275f2ea5e95c9e049429 Merge pull request #421 from pipejakob/state-annotations
b8a61d3b60f2a6d62f7ed0926764ffc83727bc47 Show changed files during "fmt" make target.
72970c9fb7ad5153dbe4350f21dd36e5d81923cf Annotate GCE machines with project/zone/name of VM.
55da8d2415a223350f2cad9f4c2330c83fe98947 Merge pull request #419 from pipejakob/debug-logging
2649ba24867df9756c177bff0926a9f60db05fb0 A little better logging.
be9613f475ac762cc6089f9cf9d850671e3f23ac Merge pull request #418 from pipejakob/bump-machine-controller
b4e6bff324f98ff3886a7806e0b2abb855b636d9 Bump machine controller.
13c64a97a645902cabe402d919e3a36468a8b62f Merge pull request #416 from pipejakob/overwrite
7a17c5aaa152083c68c1cb370040b72d5d7bf145 Merge pull request #417 from pipejakob/typo
2d3da8e4c1f4e32fb368d57029d5fa0ed51c4cda Fixing minor typo.
cb1ebbd324a4c2fc46e8432009e5f5aa11181c67 Overwrite annotations when self-annotating nodes.
2acdf95d58a3739d8bd90ac373814bc2bdeef688 Merge pull request #415 from medinatiger/dev
73729f87982cbaeb094035f56e59cd2f2d8f6dcf Wait for control plan upgrade to finish before upgrading nodes
6f6d8d55754f28bf40c701a1ae0a39a5d53f6ea5 Merge pull request #414 from pipejakob/bump-machine-controller
d509ca9a1af10e822b8dd94a15745ff6a03586b9 Bump the machine-controller version.
2e01361f5a360d1884294dbe28d95cec0908b348 Merge pull request #413 from pipejakob/respect-the-spec
7b7e0330b21c53626983d19f3c072b5578029af7 Use "new" machine object when deleting.
bfedc416600e458bba313942210405a3232836c4 Update Machine status with errors on invalid spec.
fb4df2e77e27c1d82b2760a157a779e73b8b4af4 Merge pull request #412 from ajitak/master
b41292bcd616cf7aee112cd411b2b2fa42ab0f9a Skip master for repair
a03b9f0e5aca9f6da7640595f913a18f3e9c9a0a Merge pull request #411 from ajitak/master
5e33cf7896c8336a0205c3235e4bb95034e28267 Repair code cleanup
6ccc625badfe6a3f8bcb625e0a98600285174302 Merge pull request #410 from ajitak/master
f2c409dec0eec1b2e407a1fea04590e6245e91d4 Fix logging before flag.Parse error
3fed252a5ef6e67f155a855fa9ba919a18bba574 Merge pull request #409 from ajitak/master
2ba5e4967544b58d8be4d5bcb397d46f448fc36a Move repair to a separate directory as a separate utility
709c82cd37157d2ce1747a8594f516084ed84808 Merge pull request #408 from medinatiger/dev
1d4f642612a804d090fe0008ed525864bda454c5 Merge pull request #369 from mvladev/client-generation
b47855abc68b3d89ff4d0693f1702ecd233bf246 Add routing instructio for non-master nodes too
3ec233aad11827944a0d4ed9689f9ae8f3c9496b Switch to wavenet to replace calico
0c217988e0c6990f1d852fea68cad1533c80447e Merge pull request #404 from medinatiger/dev
e47777489a102ce6ff5c383e2fdb3c87b8c3b59c Move the "cluster-api upgrade" into a separate directory as a separate utility.
75075e19d0c29a9eee27eac477acd7cd7f1e429a Merge pull request #403 from medinatiger/dev
8b6c3678449e7641265466699eb0c51a610536e5 Use the latest kubeadm to install k8s cluster so that the configmap is saved
cfe39b6805fe69fade278f376ab521fd22f56e1d Merge pull request #402 from pipejakob/more-fix-image
dfb22260879cf041c5d77eb4f56b30b752906027 Add another command to fix-image-permissions target.
f31066bd938a7b197d39a188892f484beffc0175 Merge pull request #401 from pipejakob/gofmt-target
d71b832016985b1be86ba45b7e304910cd494a01 Add "fmt" make target.
422bbda2528e383c50a64adf2fb715b87248223d Merge pull request #400 from pipejakob/makefile
df475cdd2179e095724f8ac0a8647b77c530df7f WIP: Debug 1.7.4->1.8.3 upgrade
6396e235dc9e36ea189954eed6db592fb1b64f6e Ignore machines-client example binary.
d10b4aec19a9102378992e1486cfe0d3a2461f58 Merge pull request #399 from pipejakob/makefile
bd0f6475458962de61cdee39ec0e66eba84911ad Minimal Makefile to help test builds.
4cfa930e18d178f298ad13f47234e2b06f2c1e19 Merge pull request #398 from ajitak/master
5897a190e0d1fc2a99fbc09cbf8c2d7cd526f48a Go fmt
aa166754193860e55c2efe556a8d9a4e7694f589 Merge pull request #397 from krousey/combine_apigroups
d2a1c8b1634fb007df922dd47f38d6d5971dbd6e Add the ability to specify machine controller with env var
719cbd6248bc83440199e449010050373fcdf17c Merge pull request #396 from krousey/combine_apigroups
174967c543c3271f8826cbe71131805882144b0e Bumping machine controller to 0.6
4f60c77e914e6aa98be9217e9bce246898b2ff3d Start using Cluster API type
35e6dcb871ed6a3809732a2d9e1367e30e3df0e2 Merge pull request #395 from medinatiger/dev
49db8d374fd6c42924155e2c54b5e4349b73b6e7 Automate ssh key configuration.
c44a40a48478850ad3a144dd6b11a0c2f277c2b6 Control plan in-plalce upgrade
2dc8ea929c24f21e6511c875e88b3e9b8eb8fc7b Implement master in place update.
de5eacf96e1ce03f8e4ee50c1a7e7c71746676c9 Add some logging for Upgrade code path
0784296d9db8398f9cc99ef2b3c2df2cf0e87ad1 Fix log actuator to include update command
8150bad3126d7029cfa48f2030569c3d41267c3e First cut of upgrade support in machine controller
7ffd9ba19df6423b2d1f50e7ef266528795c03ae Merge pull request #393 from ajitak/master
50120920ac776f87c111bcbfcc99f5888e17b360 Fix cluster name in cluster yaml
699544f363c0cf61ac7fc9a44f81a6e8f86a2079 Merge pull request #392 from ajitak/master
8e3d7946d3f4e084affd70ff3e021258ef24dfc2 Add repair command
92db013b4b8dad5d70848100122d7a33bf390508 Merge pull request #391 from pipejakob/link-nodes
8ec46deb816cbcec099db4cb01c382958b882138 Watch nodes and link them to machines.
affc6a67c12b981f6eb6ddefea87ea4c73ec8acb Add code-generator to the project
c0da131dc2c962ee3a03608c7b758728293ef088 Change api's group to cluster.k8s.io
c22972431650320a9fd1e367de9ff4706da6724a Added Kubernetes license boilerplate
b9527c9342862090c4e90806ad00dd20dad8b6cd Remove kubernetes dependency from vendor/
d822c08e47d027a84f935ef642ba84f387d3f872 use versioned types for ObjectReference
3057f55bfaf2d8552f025fb47c71165f17b745d1 Merge pull request #388 from pipejakob/machineset-usage
4afcf94a02535376a2a6a4fbee07e16d1ee2e2a7 Friendlier output for "machineset scale" command.
a2d336df5e84c869bf8bbfd9380c5a226ea64a7a Merge pull request #387 from pipejakob/machineset-usage
fd6ce3bd9a80af9f9900ac46b018bb05a5ce6fb0 Cleaning up machineset demo usage.
f655f8ffbc07152bba7bac593337bdda4d75f948 Merge pull request #385 from ajitak/master
3f1ee1521fc39bf4278af080fb1815d995aea60b Remove enable machinecontroller flag
15df0c2ce8616593cc7baa72129d8d33ed9bfcb7 Merge pull request #384 from pipejakob/use-control-plane-version
39a53aa31aa14af2400a9a5b9dc6a7b8ed81ea5e Actually honor kubelet/control plane versions when creating masters.
94c1cf919ba5e0f7afeca0d28dcea47735a1345b Merge pull request #383 from ajitak/master
f1dbaf00016125525779f3e6a32a94abd7ee6439 Clean up service accounts during delete
6e92b09da842ce5e0af3774d9a11283f902b0f6c Merge pull request #382 from pipejakob/healthcheck-master
df043c094e3e470d38ed0306257d05845a451fbe Add health check for apiserver coming up.
f1c42c3be555b2d33e01c36e6af4e3003a3fbc3e Merge pull request #381 from pipejakob/annotate-master
5c7d0b183c2be9f32b2ddbad143589943a497eac Have the master annotate itself as well.
f62d65eac260e4492168dd9f121a70af806b68a3 Merge pull request #380 from pipejakob/retry-machine-pod
24248ef33f2d51a9f459aacc1e165b9f0f538b1d Add simple retry logic for machine controller creation.
f48c6b533657a4a7c51a059dd6b50ba1e5560fa3 Merge pull request #377 from ajitak/master
f8aba2afe151821a67f353526971dfbc4b54eee6 Remove unncessary cluster flag and use default kubeconfig if not provided
e15d4702d54422428c43d8531d9b3e869069ca80 Merge pull request #376 from ajitak/master
4bd96d95c8f62c3fc40b144b93f2be47db2108cc Add node command
662cdfbff90e1c232938948ae710920de5b324fd Merge pull request #372 from ajitak/master
314dde6784dde08049ebe2aa0ca767d36c4c9704 Add a provider flag
729410b80c59e59788560e5e3d743548b60e31f7 Merge pull request #370 from ajitak/master
f734dad5b9a71bed3f7c8d60da7e616d2fb4a15f Replace log with glog
59a9888c3ba0d474dd7e895ff5d212d7bb493e30 Merge pull request #368 from ajitak/master
6da190deaaa36b6d34d269cb7c4d58273a494dd6 Implement delete command
3e05efc9bcad18b6166e816753886b37792c7f6e Merge pull request #367 from pipejakob/projects-from-machines
008709581e55e5b288831d9728965fd2412912c4 Get service account projects from Machines, not Cluster.
6e0bd8b94af4dd6b94eb66852eff52e1dee983bb Merge pull request #366 from pipejakob/fix-crd-creation
6ed43c6137277293a857f36d15a7912e6a5df2f2 Fix bug in CRD creation code.
965e0033cf6c06ef4f7782749b1f22752dfdb91d Merge pull request #365 from krousey/combine_apigroups
5ebc559ee40d92a852b3a08189b06207e49950ff Move the machine types to the cluster API group
618829fa6a724c89f2ad15b1d3316be0babfdb2c Merge pull request #364 from pipejakob/fix-yaml
d33c42f2ea5627277783c7dbdc27d6e4d8ea70b2 Fix our example yaml files.
d1adea22a567950bfb29aad314f7271f2facce54 Merge pull request #363 from ajitak/master
bc765fc3557e06122cd20f57f9b7411c556beaa3 Remove kubicorn dependency
94a851c8c536f1efa36d4fef14458164a19d93a8 Merge pull request #362 from ajitak/build-fix
9bb68955c8632d99047155518f85d889f53c75af Fix build, add more methods to logging actuator
d66c41297f62082851948464bf12eaeb1b43f627 Merge pull request #359 from ajitak/master
0f6ee22817e25cdc69fa8b49ad00233660a2ef68 Use clusterv1.Cluster object to create cluster and Update readme
a5bd0591eda077edb713acdcef5c0fb7cffb0ee1 Merge pull request #358 from ajitak/master
d36997752f2d1b0504541c11ae3d30f70b16d26f Create VM for master using GCE API
9ddc5e67e6f5b33d1673b2dafd36b8fa16a8034a Merge pull request #357 from medinatiger/dev
f36c0f3a8b68e1d2f6ab83531dd0898d17d8ea53 Wait for master update completion before updating the nodes
6f54a6db3e4549327131c1e57014064f363ec872 Merge pull request #356 from pipejakob/annotate-nodes
4e4a2ac7c4daf6bbebf361a83adc037d6526ee97 Have nodes annotate themselves with machine name.
a94a1c0697907ef6f77bb1211f818ba6a6566d73 Merge pull request #354 from pipejakob/honor-kubelet-version
f6dc3d1ec354665607e96b08d4ef68f9aee37ea3 Honor kubelet version when creating GCE VMs.
017239afbccaf79e2e654328beeca255e593b761 Merge pull request #353 from krousey/cp-types
54aa48d2ea0003966bf3421c8b3f75f86647266b Updating the cluster API from the review and fixing cluster upgrade
102dec16b3896d721ebd8847d1e4bba33913ad36 Merge pull request #346 from pipejakob/make-images-public
22a17a7abd2138b324da9b627884488fb519de10 Add make target for fixing image permissions.
ab46ae08d87080478fa45f5f20a18d0d2714c3c8 Merge pull request #345 from pipejakob/skip-masters
77614f7233622880738bf67d98ba6e7c677b921a Have the machine-controller skip masters (for now).
ae745b53fe809a900442b2a7b1df4e5e98238b9a Merge pull request #344 from pipejakob/default_machinesets
2a44992f8b840f7f360e05fdab242fcc84e8010d Add default MachineSet labels for demo purposes.
c8543c6cf3b97b3e8e20d139b8608a9ccfd77e49 Merge pull request #343 from pipejakob/gitignore-update
aa57e662272ab250452d343ad3021d5e2b94fc0b Centralize gitignore file.
4ad6df903235e719a83dd150500c35d6f9386dc4 Merge pull request #342 from pipejakob/license-headers
a29f1e6467884ea65bf99309df4ee08899382949 Add license boilerplate to go files.
bb0ec5e3e72bb5106eea24f0cccb544a83c2fc8b Merge pull request #341 from pipejakob/controller-rename
055fdfbac414b11519a1a562d8907add32a0cf92 Rename machinecontroller to machine-controller.
b2ee19148770ef549a99732ee06aaa028e6a8358 Merge pull request #340 from pipejakob/install-machine-controller
6b938f145e3d2e2993f8169db1eaef02794e8119 Install machine controller on cluster creation (optional).
b578437a456f210d392770c1385cc9fc4aa2a9c2 Merge pull request #339 from medinatiger/dev
3849f9582bdedd3d767176a96fa9a80e4b9b2dcf Highlight experimental nature of the code in README
c2850d261efb1c462019055f29e5586d88663be6 Merge pull request #338 from medinatiger/dev
2ad39a07704f2f4d8d86a30c2073d6bc3b15c6cf Remove panic in deploy package
0b6cca636fdf925aa2c584bcb8cccc3787216bb3 Merge pull request #335 from pipejakob/kubicorn-master
41e463ffd89f2a473948910e5f7a7467691235e6 Switch vendored kubicorn to master branch.
3371ff33e03f929c70bd8aa32cbb3b38889d2e5e Merge pull request #334 from medinatiger/dev
5f39fc444476040789c8af8ce924d005df8eb123 Move/merge the upgrader into a subcommand of cluster-api util.
52000e76b1d9b777b200e04305ee8d105089f1f7 Merge pull request #333 from pipejakob/controller-image
d989a7da8f86aa628e73de9818a91177dbf6925e Make it easy to build/push Docker image for machinecontroller.
6e0cb502a0b5c9f11fbff700ae2fe639956de061 Merge pull request #332 from pipejakob/machineset
f7ce406e64bd95bdc62279b7b2fc1842a721bb5a Example client-side MachineSet tool.
c826e3167ccfbbfe849d3bdbc0a8b64e0ae36d7b Merge pull request #331 from medinatiger/dev
ea1327829f9c73574174da666f97b81774a41b55 Some tweaks for the upgrader.
ca84873c535bbee25070c9c2d86248d4c25628ba Merge pull request #330 from jessicaochen/controller_node_cleanup
23ad3057db298bbbaaf9bf9aec8ea14774b2ec40 cleanup node before machine deletion
ca1167847236d487322f7cb3f4c69ec838947331 Merge pull request #328 from ajitak/master
425aaf6d42816bb94669b6ce3b17cc027a2bf59d use objectmeta for cluster name
651f98d0f98ea717b5597d2b7f9d45af8ba3f3c0 Merge pull request #327 from jessicaochen/controller_update_selection
c0a641a80e153388a90c207cdf9dfe92982d51b4 Do not update machine on changes like linking the node
4c5ca864226e9a80b2f096686db215e250d5d6d0 Merge pull request #326 from jessicaochen/controller_node_membership
63146e0151c636e8ebc09be6b6cb2eaa0a2cf6c9 add structure for upcoming machine controller work
0e36a42826f855ce620347401705486cd770fb6b Merge pull request #325 from jessicaochen/controller_flag
8b92c290c2c40b9af3cda9d2cfd6461827ef67fc supress uneeded warning
b86467e994a6bb3ad410d24ecb464babcd0553f6 Merge pull request #324 from medinatiger/dev
73902e7902d315b3fefc51b13b9d0a7960003538 Merge pull request #323 from jessicaochen/controller_new_nodes
ad52b6ab1918fa9906b39b0ef32edc11c7717197 Use global scheme for client library.
6629d7db8220cc57be73126b0590443980ce61ed Add new nodes to kubernetes cluster
66e0ee1a6701954e694a49a86f8dc2554560d724 Merge pull request #322 from ajitak/provider
bb92d156bcd284280861c1ec2e14e9eb6ce8261f Move cluster-api/machinecontroller/cloud to cluster-api/cloud
8cfa9a71ddab9eab0afe146de01588b4ef7fb4f9 Merge pull request #321 from medinatiger/dev
b0881067bbe8ea78c1b5bc46fc053e37fd3c3ea2 First cut of upgrader
6fd78203fdd2fde0069b8e0f63788f8e7fd63c52 Merge pull request #320 from medinatiger/dev
71be3e1f4960a8ed79fbd09c6023643446c6180f Implement client-go library for Cluster{} in ClusetrAPI
5ce4ffb1c4a9aaf728fe1e565bf4fb6c7a751911 Merge pull request #319 from pipejakob/cluster-deepcopy
b4e08e29821dd8a34b48d64a670d52bd2f6b6fc3 Making Cluster types more useable.
6363b901d56b825fb6a660715e70958b8ee4d45f Merge pull request #318 from jessicaochen/controller_gce
74d6a8217fce13504a9d8ea9241b23f397c8667d concrete google machine actuator
0c1be78efd1ce7ce444ea7d95b35537564d4d709 Merge pull request #317 from medinatiger/dev
1a17f93e588fd6d62aaa313c02ac85f58015d50a Add an empty upgrader place holder.
6ffe21133e49b331ea390e80ae27cbedc9e98bb1 Merge pull request #316 from pipejakob/invalid-config
ee6aea6462a93715b5bce2188147fa1dd099d671 Example error status on invalid configuration.
008fc27d8e30d1cac2a55630cdc6726c6bc552c6 Merge pull request #311 from medinatiger/lib
1bded4d4f2c6ee331d6d2ad62526616c4c292a72 Merge pull request #315 from jessicaochen/controller
56780ef17dcaef0133b8d8101e61d13a1c60eafe Merge pull request #314 from pipejakob/startup-scripts
c33d6deca39ed92ace6507eb213abb4984f587cc machine controller logic with stubbed actuator
7850c446d38e57b358a8b608755e9b16f11c4be1 Quick plumbing for GCE VM startup scripts.
947942b79d260da423809e19942d9553bec7f68d Merge pull request #313 from jessicaochen/controller_actuator
b3b1c5c0a0ca471a06c99af202cf89188c9c18e3 stub for machine actuator and vendor updates
d59163845534fc8bfc43a93aca071b78911f64c2 Merge pull request #312 from pipejakob/gce-machines-prototype
3c999871df730df8f4616c49574d120a9bed270e Super rough GCE machines controller prototype.
eacd53585ff6428610fce61aff5f7bd31e2441d2 Updating dependencies to pull in GCE client.
f7c545de272e37dbff495f804888f309cbb409d4 Implement a client package for CRUD access for machine object.
1679e24f46c7f5a638fd8024f084d35af134cdc0 Merge pull request #309 from pipejakob/machines-controller-upstream
68b0c3dfb1dc666b7576e8e7e19527d0f969a07b Tiny patch to vendored kubicorn to fix build.
2b13b6032a3b782d857f4684d9ca69638f8739cc Add example CRD creator and Machines controller.
39317ff606fcee039d15f58753a8fb734665bed9 Making Machines types more useful.
6c538b3a08206bea854a87ac8afb89d25f02ebaf Updating many vendor packages.
2cfffc3ae5220beb4b1fcba39edc69e47b6b79c9 Merge pull request #308 from krousey/cp-types
8e8faecfa5bf762dbe52848379ea7dc400926bd1 Merge pull request #307 from jessicaochen/controllerstub
e09da34ccec6d75174185f2c5ef010b5d8e60c39 stub files for machine controller
ace558e0edc0d429631aaf40193509f975128430 Adding types to temp location so they can be used
0ee93187234961c784fe97f76bd344d2b2ce84c7 Merge pull request #305 from roberthbailey/remove-addon-manager
f3de191d31bb8033807c78848d67345d03d115e8 Merge pull request #302 from ajitak/master
5cf21ab76fce090ea41f82b7d0b6e2bf86c87f4f Machines API types.
898e828ff3cf5ec1f5e25b3436f286592cab5100 Remove the addon manager code, which was copied here from the kubernetes/kubernetes repository but has since not been kept up to date. In particular, this code was prior to the change to use kubectl apply (https://github.com/kubernetes/kubernetes/pull/34513) which pretty significantly changed the code flow.
0d3a9a5f588ea3090538b89cc26667d40cfdc537 Remove the navops documentation, since it hasn't been updated in nine months.
797472ff64eca4534414f7a4389592272d06ffd4 Merge pull request #303 from roberthbailey/cleanup
feb75c212a782d2eb651cfd63f6662d3cef78980 Delete directories that only had placeholders to new repositories, since those repositories are now well established and the forward links are no longer useful.
cecac0a788272018960db1c21ad33ac85194728a Merge pull request #296 from roberthbailey/cleanup
a73a2a2774898d437424863f51a0362c9db8effd Update cluster-api/README with build and run instructions
ea7a7fdbcfce14746c7cf4c3ede0637932a1c43d Merge pull request #301 from ajitak/master
5422ae87c5e57a006ab5dbbc7d575d2eb26d2531 Add delete command
7a59080257810ea757d81d2cc3fb75164c45820a Merge pull request #300 from ajitak/master
bec87eb5fdce4aa55802664bf2af25b08f6b7586 Remove binary file
f4ce372809308f952e083f79bf69ca95178a3eb0 Merge pull request #299 from ajitak/master
ae190c57f080da079ac105c936de8852554eafc3 Cluster API init
82a3c5d740dfb9e8b413ea53c6f45ec20b344c35 Merge pull request #297 from roberthbailey/cluster-api
01c9ae718a5da552ff886a44beaef2228bb85cf5 Initial commit for a cluster-api directory.
935c83cde95b53c6fc7b838a00c30f67715e8b19 Remove the docs directory, since each subdirectory is a standalone project and it doesn't make sense to have a root level docs directory.
d3c352a10b65954b722d574a72f250f87cfea05b Add support for Session Token
2dfd92e76f7c19e90abea01f8ab38e747f25fa50 Added support for making snapshots public.
7e09bb743bd3fc95457d1c47d558ec1e3d9e5f5e Revert back to upstream bootstrap-vz with newer base image
b7474dd2050d0dceb36cfdf0966d593c1be635e6 Merge pull request #291 from justinsb/k8s_17_image
de5d476e2fd5aa37d09a0224837b6b2781bca728 Create k8s 1.7 image
92879552d1cb0ca488201b524805810e16bbbaec Merge pull request #270 from roblalonde/navops_update
b17bab61cb34f31e85603f01a307be35d2a56ef0 Merge pull request #286 from justinsb/aws16
10e1cc04861b6d3aaa618d62bc8af3c3bebd2be3 Updated AWS template for 1.6 image
46f61490410d20d89fc18d1ec5d99321f4258302 Merge pull request #283 from luxas/remove_docker_multinode
2a1faca59fb6851a41457501ddcd5e1e4350ddd2 Remove the docker-multinode guide since it's not working anymore
c8d6fbfc0ab7512a9896da325cc14b9a9240146d Merge pull request #265 from justinsb/1.5
45ee68ae00e1cc97ab2d1ba8b1a2fc1db48bc7f0 Merge pull request #273 from sstarcher/fix_setup_aws
e573386471964bda2414611adcd5fd76da3d7522 fix directory path and ensure region is set
54a109d9bc9c915023e80658f852901b5187fe99 Update Navops Launch documentation
5e053956f1fe62858c4b9469b73c4d182a133b3f fix err information in local.go
700300ff0a40d3709aeef5f7b6cf43ed809ded25 1.5 image: bump to docker 1.12.3
a798e1b3b06761bf9f534f128256c3b9721d4374 Merge pull request #258 from DualSpark/ethtool-and-admin-tools
45513196496f8dda57aad48b9263f28945562097 Merge pull request #248 from bassco/add_kernel_headers
1a0df742a422a73c48f81b07998a4d3b7d7d0230 updating scripts and build
c938939a60741c8a8ec975065000475e894690a1 adding setup-aws.sh script
70a632044c5eebc2426b0857ebfe6c2025c795c3 adding admin tooling and ethtool which is required by kubelet
5f6a8c3861c490d2cc52f280383ef0ed2978f0a3 Merge pull request #250 from justinsb/image_add_linux_headers
e69bb43df31c2f585423740ee55d53312ea82646 Merge pull request #151 from mikedanese/makecerts
c3b9707d66c7e20c1b4ebc8051d3434f4c2444b5 Cleanup bad revert
0ead8f7f70fff16181fb384343090b45af7df73f Removed redundant comment introduced
4fa2afec37049c71f073118db6e8fbf034e5371f Fix introduced formatting error
a8c4f818f00e3bc8dab12b0ddecae9914009944a Add linux-headers to image
4a7df8f7dfbdd5b324a59a9a4bd9d8c05ac886e3 Revert dkms changes
dfba9b21d08bab3998faf916288303066de1bef0 Add linux-headers-k8s to allow sysdig probe kernel probe to be compiled and loaded. Do not remove dkms - used by sysdig agent to launch sysdig probe kernel module. Fixes #245
3666ee0cb0d6baf284812eb53f506967e54d6750 Merge pull request #234 from justinsb/1.4
dd0c16a6fc752759b728c36c7c68c700ebb4757f Only try to read SSH keys if we're using SSH
1a37112972698cce89412dd98ca6f145de517659 Able to build (AWS) images locally
cc32aaac849cad6e966804395b08d1f5e90fe770 imagebuilder: create an image for k8s 1.4
10b8f8c3f2d1a5f8c677f2aafcd42ea949144197 Merge pull request #233 from justinsb/aws_ignore_stopped
6cb54610426ce9bd4d590cc86603fb5f72db1694 Merge pull request #232 from justinsb/aws_region
152bb4338c548239afb429b9f626009f7813476b Merge pull request #230 from justinsb/imagebuilder_makefile_gofmt
a6052415c2bc3b40b577a8f401023326c4481b2c Merge pull request #231 from justinsb/tag_images
b318a1651172988598d1f58be09d2869c4f86a2e Merge pull request #229 from justinsb/fix_171
2c55e026e721b4e0121557ae3e012cceb2a84533 imagebuilder: ignore terminated builder instance
efb693b289921b7e40abc503e4578c7a92e67e28 imagebuilder: support building in non-us-east regions
755a14b08a09cd5a026b7de2bc33007eb16a7e19 imagebuilder: tag images
7399cbd0fb37fc87ae7a62d162bb34f4329ac915 Add gofmt target to imagebuilder makefile
4b4e0ccae9e326591a9f4736b5fe9e77b51397e1 Improved README for imagebuilder
b422dd3882d8ad8d5474ca59be7eeb9def8ced0f Merge pull request #227 from jonboulle/patch-1
492498f5a7148672f22e69d296227a106542a07d README: correct minor typo (it's/its)
e4c1bccca6897e4df6221af6b60fbb80e5b6708f Merge pull request #218 from luxas/stability
41f3d6fc7ced019cb750f2e915a6f89b06177cb0 Small stability improvements
8c6e6bfa44f6a83afe9b129f3ad78334beb680f1 Merge pull request #217 from luxas/containerized
7e77581ca9382e75156bd2fbf0ed225f9e9a6aa7 Make it possible to use the legacy containerized mode.
67610cad099ae9312cc7fab37f491b42221a37b8 Merge pull request #213 from zreigz/checkout
7baec29424c4c7f53b65bc2e989a5e68df41cc34 Merge pull request #208 from luxas/proxy_ds
37f30a7b5a4f54ab4eb543ecf56c7933447023ab Add zone for nodes
d3ec4adfce5a8dbf906b0b1394b21bfa33e018aa Run kube-proxy in a daemonset with version v1.4.0-alpha.3 and higher
d19e4fcd92eaeebf04d24f1d5fc9d2ed491ba817 Bug fix for git checkout
775bf0731a5f9cf25603514ac83cf1c157c74d5f Merge pull request #207 from zreigz/libvirt
47647d329f7560d06715495025474ee519915e93 Add libvirt provider support
3ac202bf533f2702e2d0938c990427f0db9ea0cc Merge pull request #206 from luxas/disable_etcd3_arm
a8edeb8d1dcd88a86c639c11974ea6cad7dca20b Disable etcd3 on arm since it's segfaulting
57b33d24211ee06d56e8b9aac0615cfb5cf658f4 Merge pull request #204 from zreigz/new-flannel
b057a16a7d4058185ac66294d6a5dea7abffac69 Bump version of flannel and etcd
c6f2b55f8fc2cf9c3e53130ca9cfa19126a63063 Merge pull request #194 from zreigz/ansible-tests
3eea812d6014561a44175d20c62cc8ec939707b3 Merge pull request #203 from kubernetes/revert-197-bump_versions
fe1fa76e73fdb90621da42176b6ecd67ad9e2730 Revert "Bump version of etcd and flannel"
0e5d14bd164e995c89f676a16efb72964ffeb6c8 Merge pull request #199 from ivanilves/deploy
14228aa18f24f522014876f6bdb1975909ee5e82 Correct path for cd
59d9a36fe7fc0a9329844df37c6088d3f6730885 Get rid off ansible from tests
452cf548e4ad2289441fcf556f8cd8cb085cd396 Merge pull request #197 from luxas/bump_versions
86f0e2dece9450e3015e12cdf5e5f34a1f31e1d5 Bump version of etcd and flannel
135cfcf0340e6cab01a55c773d30935f4321f2bd Set flannel net config ONLY when running on master
ef30cfe1f6705a1d125b59116c01f43ff1384739 Merge pull request #189 from zreigz/e2e-tests
0bdb7f02aebd47cc71c02c2deea1c8e280af4913 Add Vagrant enviroment to execute e2e tests
d200292416003c18af628afe429404f2d813989d Merge pull request #193 from luxas/refactor_and_check_for_deps
326a634d42425a9e9d49c0b1c8d7c70b4e9adbb5 Refactor/cleanup in common.sh, use curl for posting flannel data, require ip and curl, remove NET_INTERFACE
b7d9ee5b80b15337cdb7df030d90149b5f594891 Merge pull request #190 from luxas/remove_install_deps
969086b076e8f6feb6e9d8c351e620d46bb0b65e Use the ip command instead of ifconfig and brctl
91a29be41445881856d6d909b6d1accf91a25341 Merge pull request #186 from zreigz/remove-os
43759ed4ceb730e24a929f2ce37b9fce6d2a57a9 Merge pull request #187 from luxas/bugfix-1
bcbd9245a1c2fd1ae16e7a94234d75142f421111 Bugfixes for docker-multinode
5f041f9c1b0271ff204d2a80782677efa8cf59eb Remove OS distro dependencies
7c5c29fc6a04e6bab94cd2a27e178c1ab6677d0e Merge pull request #180 from luxas/cleanup_things
27213f7289c85c7656db25007270583a0201e96b Merge pull request #183 from NamPNQ/patch-1
617851aa0bbbefa4d1e1035c7a58d255a9a91072 Many improvements to docker-multinode, and some cleanup
ac90c4e2afa00959852cdc72c41d7ee0a9d97a48 Update README.md
d4792f24d813fb76426f8baa281ee8ef31f6214e Merge pull request #115 from zreigz/cni-plugin
43b3b8c14e10f665dce704503c2166f40dc85e4d Use CNI plugin
341492e7b58ddc603f8b7804a958d5d2805bf06e Merge pull request #178 from isavin/raspbian
a0b09e4a949dd1d225a3e853d254d07a0a4539aa lsb_release raspbian classified as debian; return non-zero error code on bootstrap/etcd/flanneld failures; override service start timeout from env variable
04431672403202d9f535a43f34f0899bc8fff1a7 Merge pull request #172 from zreigz/fix-adding-mtu-bip
fa907597c1bc9f40870a9816bc984073b55127f8 Fix changing mtu and bip in DOCKER OPTIONS file
0a22c4dbde635a8c06ace876e8bdbce1c53f8f68 Merge pull request #177 from larmog/fix-etcd
0ba74d62fb66213c26f36b2632d9637a066d848f Fixes that etcd data is not preserved on master.
9ff58bcaa1e846da0b32b069f5e60eb2cf45f75e Merge pull request #93 from isavin/fix_grep_dash_args
6b487427136d850f912b25ccf3165ff7bf836a36 Merge pull request #170 from justinsb/imagebuilder_docs_1
8d031a1db43eafe108d8c061d575d6d67518502c Fix imagebuilder readme: go install -> go get
3b88dc235a50c1e29e08150e31bb16f6916cf2f5 Merge pull request #169 from justinsb/imagebuilder_vendor
26f1bf4590313f9c8282faa9d0fb03ae6004852a imagebuilder: add glide dependencies and vendor
28c64a0ba3407172f8518811e144c9eb7bd75f73 Merge pull request #164 from luxas/ready_for_v13
eb1f29aeb75d61fa86856118aa9ffa6a492c951f Make docker multinode ready for the v1.3 release and update docs
712f2cb076046c9fd766b6742ffdc849218f0efd Merge pull request #166 from justinsb/move_upup
65d20106a05ed6532369ddafb285bc073e56d187 Move upup & protokube to kops repo
16834026d940680b5759e3c02d45a527300ef418 Merge pull request #165 from justinsb/upup_polish_14
0860415babd65d98b1571cf01812a2edc6b81964 upup: add doc for philosophy
6eeedc9c8e1a0c015d37fea7bb3b6203eea66cea Merge pull request #82 from isavin/fix_kube2sky_domain_flag
8e49156bcb7e6b8f0f602256fd6559390e34ee5a upup: workaround for secrets problem with upgrade
8c2d92842a7851111e9999134955d1848de3aa68 Merge pull request #114 from justinsb/docs/delete_cluster.md
5d6b35d883a77ad7fcf1682dde4d57414f74fc2f Merge pull request #163 from justinsb/upup_upgrade
1be04fb2d5d5c76daff55ef198617d28605db101 upup: Add get commands
0a85df77b0b2116dc7c592fc2b1e0b593aeac644 upup: improved upgrade procedure
60478685d5721e044e7dea3957fa50c038d9e07b upup: More delete cleanup, use statestore by default
b93927b5488d4055ecab30e0a8b44c4c9afdc826 protokube: apply gofmt
5acf4d8213bc79efe287286aba5c4df7d10b2af4 protokube: avoid doing redundant DNS updates
beebc3229afe13fa262fa34561ac6d9f5fcb2f2f Merge pull request #162 from justinsb/upup_polish_12
f95fd358a57b08b69f93db32fbbe3ac951425161 upup: update same vpc docs
f943ae7a47ba1cefb4a6bfe5cc3d023c2a3731d4 Merge pull request #161 from justinsb/upup_polish_10
ec4b521ec219c62b63d787e575f3f4559fca4621 upup: fix terraform docs
f41bd69b60d2c0e9dfd15141341b088d26f7c119 Merge pull request #160 from justinsb/upup_more_deps
6ed05b317ad4a59bd86e463bf77ca39b72a6d244 upup: More glide deps
ed92f9217a0b36282618dc5ba18b3732e0dfb002 Merge pull request #159 from justinsb/polish_9
94bae427b2736d31d648c0546ce35432b94c08e2 Make StateStore a top-level concept, with subdirs for each cluster
b465c8e64db3a127a6a110811536c12fe9912b3f Make IAM permission abstraction more generic
51cbe4a0cb84700f2ed4c9a35124c9770ede8787 Remove AdmissionControl from top level
098247591d5f7de7dbe5150aff5bfd6238378f60 Rename DNSDomain -> ClusterDNSDomain for clarity
4c1d91b1ca96f3f0489f876a3db76b190606ecb9 Move options to common stage, so that it works with terraform generation
e4dbdeef3c30897ecadacd4cea1968cc3ad0a063 Better shared VPC support: more validation
98e0001194ac0eed3c69a98d6c5500372494ac15 upup: fix error message to reflect correct flag name
f091142db9e101dd6114f732058a470ed0ffe3b2 upup: infer --cloud from known zones
4a80a6f6f8c2520a20f99dc38f92b1753557a4e4 upup delete: don't always print dependencies
565ba44f138bc0ba4f6508741ca6df1b5f9ebe0a upup: group DNS properties
672486099b3447cf6294f0e3ebb2e9ff8b273007 upup: add edit command
af0e5cdb0fe808bbf5d85172e303a7d1aa3efd9a Merge pull request #156 from slack/protokube-dns
cbd8c0faffe29f7205fdc7027b346f3606bfa010 Merge pull request #158 from justinsb/release_1.3
61220e0dd97a8cea4dc2690ef99918079bfb2b12 Use default handling for CLI tools for parent tasks
fea4029d81f683a20174b2fe84f5f0439b6066c4 AllocateNodeCIDRs need no longer be "bubbled down"
279b22ba90cff998d2f77310bc5a560758c06ff7 Rename `kubecfg generate` to `export kubecfg`
b17ceee208f33d6b7f3309ef68756ec3a798e4f5 Make sure terraform output is stable across runs
65c5c6edc3a3daa14f0bd1668fa3e9a0e3486fe5 Remove spurious errors when deleting a cluster
f4f163f4a2408dc215d408c978286180434dd139 Apply gofmt
146f0c7448664af10e5ad8869fe37fd47735de93 Rationalize API to something we want to support forever
e28155a44174c82310b394cec1e6d036d99c0f7f Rationalize properties to the minimal set
b89a0432cb9074f7ebb70fdd959b45b0a4da636e upup/cloudup: use configured URL for nodeup location
08c317f1ce9c2466fc80fb36a123dd84372a8bce upup/dns: lets protokube use sub-sub domains
5dc04590cbaea7eaf42b3c3a21efb34c6bbaaf3e Merge pull request #150 from mikedanese/delte-minturnup
469c2dc755b4fabba2edf67e182dda31581143ee add Makefile to demonstrate how certs should be generated for kubernetes
ea8152bb88f3645571f5e1282373aa09f6a540c2 delete min-turnup
db4c7f8193ea5388a26cc90559547e9e60bd00dd Merge pull request #148 from justinsb/upup_docs_1
a50f1789eef15bce6faa4afb307580ec62395320 upup: add docs for statestore concept
349efac86a4fba3a14f73d78401f4e20d6b45c51 Merge pull request #131 from justinsb/readme_is_markdown
9bb6cf81cd55e7364952e1b16b652beaccf67cc7 Rename README -> README.md
a1b80600f4ecb8a7e59acf1865338f546833db73 Merge pull request #130 from justinsb/upup_vfs_context
2983165b77cacbff27e67bea2ab5e5bffd1a7d9a Merge pull request #129 from justinsb/upup_mark_gce_maybe_borked
779fafcb7db59c2dfe932518850580219d875230 upup: temporarily mark GCE as not-necessarily working
4f674f45e28b5af16d2bd086d9ae6becd7430ccc Fix upgrade
3865c038e899a67b858cbc02c232417533760397 upup: Add VFS context object, centralize usage
54db43ac54140f5d30b3cea97f338742eb0fe551 Merge pull request #127 from justinsb/upup_upgrade_tooling
d4fdf5a30f72e1e198bf5d9949b7967e97572219 Merge pull request #126 from justinsb/upup_use_vfs
d4d633278f2c50a08faab61ba6a142449a333509 Merge pull request #125 from justinsb/upup_updates_13
1ecd571a63acaba937ff2310710fda47a2b1147f upup: improved delete; create upup export and upup upgrade
ef5a16643cab755bf3fa27576be778caf6392f79 upup: use vfs for secretstore/keystore
7f924a36d8167c0813ac39884b799b748f3b2e85 Updates for 1.3: Docker 1.11.2, 1.3 image
4afc4a8f65296e42a23def5f2aedaab59ce0d682 Merge pull request #81 from isavin/fix_comments_on_multiline
22a56f91237b44acaae3b6066bb34df20f9079ec Merge pull request #119 from justinsb/kube13_image
c558018dcc9bdcc51a11ca01359d64d7a82b2b7e Apply gofmt
21d8927996beb96b004d514204db821ad548f388 Create 1.3 optimized image for kube-up / upup / anyone
20455d9174036144697e034ece3ccbcdd68545e8 Merge pull request #107 from luxas/remove_old_docs
5bed7bf540c3eb53db7498a92f3b19ea54cabaf9 Remove old outdated files
36e77df0d140879af3037bdbe5bea26570a8c1ff Do not deploy stand-alone proxy with v1.3.0-alpha.5+ and improve the README greatly
6a5e12b85a26082a07a28847f5ce2d6bb8802f90 Merge pull request #116 from justinsb/upup_polish_7
1fe1acf74a1f92695eb5cdbfe6f4a4d9c89de0d0 upup: rolling-update add mutex lock
73f2746e8eb9202994749e15c5075a916e3b09e5 upup: detach internet gateway if vpc is to be deleted
77eaffa605457e9358c09e6948d1104bf5977549 upup: uncompress gzipped data in delete cluster
e1b1dcc78e25728e43beb11b70925346d170e977 upup: symlink models directory for people building from source
15efb53bd939aca0a56b1426117e7b66b3b6f278 Quick first pass at docs
27f5544c6c78220be4a951f43cc12c5f4be85cc7 upup: enable subnet changes on ASG
2eb76c65b33513451f654544716f3d3048616d62 Merge pull request #113 from justinsb/upup_polish_6
7b8a961e630d7838f0e9ff3f08a4bf7408fc38de upup: Assign subnet CIDRs based on AZs
1d3aaccf4c9406e93ef28554d1367798ac758630 upup: fix dryrun when adding a subnet
52364e503bc7c8a36be2069bb2d06327f5f2b490 upup: prevent spurious comparison failure on VPC/IGW
6aacf2f1a7006f00b6f2e12e6818aaadf90d4d1f protokube: put etcd data location in same place as before
e1667bdd2c78089112559a9d20d54d1940e34f8f Merge pull request #111 from justinsb/upup_polish_5
fe03f882337ec4375ce9ee1fd2e80931f3918ec4 upup: rolling-update should take --name, not --cluster-id
58acf8f0def6d18c5dca8df66f6fd3bd72b2945a upup: glog flag parsing with cobra
efcf9109c4f32897169e727888d96e9503703d42 upup: turn down a few more logging messages
237a645c450391b55ad238bc5b3e92d53158edde Merge pull request #110 from justinsb/upup_share_aws_vpc
7f1771f672c9a46fd2635d81d07a4bbe8c257d57 Merge pull request #109 from justinsb/upup_addons
d72b9d160829dbf5375cefe68bec30d346ff00af upup: Support for shared VPCs
c809be4ee1ead369fedc40b7a79f7b44495d8b02 Merge pull request #108 from justinsb/upup_kubedns
220ed91f82b31c1709d4205b80636b74a4066d05 upup: experimental addon management
a09e435a6f1ea9003e1843ea52a5e42a8bf0a527 upup: switch from skydns to kube-dns
29dd6fa62015274fffd910c110167971a7387f84 Merge pull request #105 from justinsb/upup_polish_4
598e149ef66177777b6e761ac0f53e22e8b0036b upup: rename zone arg -> zones in README
25b861b3b89e48a4841dec8ab57ef014bf4ee17a upup: set GO15VENDOREXPERIMENT, update docs for 1.5
84cb49507bb276793962c1039dcf6ffdb357dbaf upup: build tar distribution file
d4ed46069f55c2d4d9ec26c6c876f42a18cf6d54 upup: apply gofmt
0e65ecf8125c186c045de39f08e65e45f83d84f0 upup: Fix log message
1fe76d6cd9d5517987a3b2a2b3796bc6b81b0a70 upup: allow master-size to be specified through CLI
c28e2ded3a7217160310bd1a60ecc9a560710e67 upup: kubecfg generate can default the master API name
f94291a6e5d3ee2affd134fd33fdd13dd4196899 upup: delete cluster should take -name to be consistent
a459c8cf9c92e23b22081672b1d903a734853b43 upup: increase etcd initialDelaySeconds
3629424c5e72ebd2050647b7bb3fbe76a4e68628 Merge pull request #103 from justinsb/upup_dns_zone
44a7713621b54c1c34f1636e1a6e07144eb39a01 Merge pull request #101 from justinsb/upup_fix_delete_asg
c3ddfbdcad7b82fa9b3259c2bac2d5199f6e5b22 Merge pull request #100 from justinsb/upup_zones
1ee8f930c1cc3518f17e05083df4dc274da53827 Merge pull request #104 from justinsb/upup_fix_rsecret_race
3f673b362de8999a6b214fff669f8bb2d4751bee upup: Retry if race detected in FindOrCreateSecret
56cf5bcc55f9cae35d9bc45f0e6a16bb6c756d8d upup: allow -dns-zone to be specified
3bd28e5f0605f32bf888d1ef3c7e9427c16a2504 upup: delete cluster should check status of ASG
42c3c01f2c37663d0421daf92027f4a0db45fd4d upup: delete cluster should eventually give up
135ba239ee190e9c4c317d901a7fb05bb36ce61e upup: separate node & master zone configuration; validate
cf4aeee1aa49e63b30531d9bd901ca831753965b Use -e grep flag to match patterns starting with -.
09c5d3c80c424d15c34bbf36624d15cb85e0369c Merge pull request #92 from justinsb/upup_readme
c65fa1975989f6a7f25487cdc84b77cdadff084d upup: fix typo
aaea4d2cfe7c0d435852fe808d95139bca2a2037 Replace -domain with --domain in the kube2sky cmdline.
841966e5681f58fe6184cf396f60951e8fed76aa Merge pull request #90 from justinsb/upup_polish_3
f73e5a880e0a640a27505ee4797cb417852508cb upup: make NodeConfig be JSON-clean
4a21e9b30e53cc48d21c44b6e074469381d1b6e2 upup: make LaunchConfiguration compatible with terraform
1d7a4a6635812fd6db3d851549291bc57144abbb upup: support Base64 and raw-string JSON encoding of certs/keys
e1ac20092b93097bd93a28963321a9da96f4f481 upup: Allow node-count to be specified on the CLI
ab35d961d787c0d59fba7eea16876f4737127129 Merge pull request #89 from justinsb/upup_gofmt
95f6aad856c1253e96ccccab39f80373715b8ffb upup: apply gofmt
7fbb57f87ca24b06096b25c19cfabfbcb4c952c1 Merge pull request #88 from justinsb/upup_dryrun_print_json
aa39fd339afc90237b78eada18277b9c58591735 upup: use JSON as fallback in --dryrun printing
c2db980c5242108eea772ef2265c5d4d833a1c47 Merge pull request #87 from justinsb/upup_rollingupdate
ebb06b62d952461fd40754b2561e87a183ead14c Merge pull request #86 from justinsb/upup_split_launchconfiguration
2cbf55966eb2da421e1a980f00c09f675c9fa71d upup: add experimental cluster rolling-update command
9bfe511888e7fb847929324d40c5cb96acafdd22 Merge pull request #85 from justinsb/upup_options
936f88bba3d9d6b8c207760494559bf4da699be5 upup: split launchconfiguration from ASG
b790e6563a557be10e032c552164959c75444ad0 upup: fix options processing
765047e831553053083f6348454db5adbf8b8e8e Merge pull request #84 from justinsb/upup_tags_and_names
3859f363fe2ddc332274500887de65e7c8d78a9b upup: Simple tag fixes to avoid comparison failures
2bde6baa63ab0b301c28267fc1789c7f4e432ad3 upup: populate Name, to support --dryrun
e115371f99be47ad78e571bf7e9fc9afcc897295 Merge pull request #83 from justinsb/upup_node_sizes
6c372fa30ad79e0b7701f9a438253beda5328ec3 upup: define m3, m4, c4 families
aaae9123856e984b29899768982e369abc592798 upup: allow node size to be specific on CLI
decae3db7daa5f5c38064ca06af0a1f80da197cb Merge pull request #79 from justinsb/upup_official_types
18b0e6a9280991947c8e6cd1ab1704a4ae54fa68 Fix comments in multilines.
48b46be313d953f41301d33b9bbf651f49525b3d upup: harmonize model with official config types
88b38a2866c4be1e5ebd633d5e617509e69fa614 Merge pull request #78 from justinsb/upup_multimodel
0e50a61602e7bca073b6abe12270ce8b83bac5e1 upup: split model into two parts
64d5922e56b45de2051aa22044c99d96cfe63a28 Merge pull request #77 from justinsb/upup_default_release
97f215c4038f73a544597b23d05b4842c2d27221 Merge pull request #75 from justinsb/upup_vfs
71ae430969224f6d9da8d5233643b88da112c605 Merge pull request #76 from justinsb/upup_terraform_prettify
41157f4c14886016266eaa7e7a32072665d40594 upup: default to latest stable release
ea1be6b3290844d77576fe615e6313a4676eecca upup: Add VFS for storing state in S3 or locally
2b90a23ce9e813a76a378892dcfad8cf73194ea0 upup: reformat terraform output
999c5e0bba55a0ba6aaba9f4d42403ca06a05c69 Merge pull request #71 from justinsb/upup_terraform
18502e87fd474b4fe12b162ba7aa68fcefea4f9d Merge pull request #72 from justinsb/upup_polish_2
812e7d66edbf6b981af6f6c299fe3047689b6bd0 upup: support for terraform on AWS
e13cfc8c6ced1088787976fe5f52166fe517fb9e upup: avoid warning when building filters with nil name
9690b59cf78eecaeaf0b4ca241fe5d074b029ffc upup: protokube is launched from a container; asset not needed
5428c1d46619f8f7eebd3fd686fb1054dc53df40 upup: use bare binaries, instead of the release tarball
83d51ddcdbf74c12153ee634c33a08c27a2980c3 upup: include kope-routing, but only if _kope_routing is set
1a01de0aa9196d82c7b236300dabdfdef1d23a61 upup: include count of tasks as we are executing them
aa98a1d8b81152a96c7eecaa0f42ddae27460ce2 upup: Reattempt up to 3 times when no progress made
23617d48e2fb514ba19c90d572232ffcb27ac609 upup: remove some bad logging
83b00d0628af52f024f4a1db3432cecbcd7b3b94 Merge pull request #67 from justinsb/upup_polish
10bdbd83912a7d37be4dd7992ffc479af9d0a8f4 upup: Update makefile, readme, deps
0fb006af4d354ecacf6e22e7b91f81c68ea5b24d Merge pull request #66 from justinsb/upup_ha
8ccc64e47ed689579ac9dcfa84bb706315366bba upup: HA support
4671249f745906c74dc2e3153cf34f4f213a8c51 Merge pull request #65 from justinsb/upup_fi_comparison
c8c7fd42efdd2f7cb93be16236beeddaecf37446 Merge pull request #64 from justinsb/use_protokube
bdef2ca6bef94b57be7d46825abf945e0a2de5ec upup: Add back in CompareWithID functions
81ce3c722317dfc2994b7832efcab95d73cafc26 Merge pull request #63 from justinsb/upup_parallel
ff906dcada51f833960712bda26967b2eddfbffc upup: use protokube
a203d5ba16929efb3358d4da6428f52d29fef6f0 upup: run create & delete in parallel
0747988caa969101d8d83e1e560a6919ccbbe89b Merge pull request #62 from justinsb/upup_iam_fixes
c86703dd9a05752dd8aa190cce7494953f5d0d98 Merge pull request #60 from justinsb/protokube_2
b815a3f0c24cf2b9061d112d2245b68b681cda1a protokube: DNS and direct etcd support
b7301038607b00643d415914d138ecd542e1d266 upup: apply IAM changes
f3c5718170499fda0f29302840e671f6d4a3c9bd Merge pull request #61 from justinsb/upup_elb_healthchecks
59badc17832f39fa540f1786c668696a2e8f3e89 cloudup: Add support for ELB health checks
2f2332e37b2a859345856354d36cd702f3899880 Merge pull request #54 from justinsb/upup_protokube
b8d0e3dd08f140e6a184187ff2b043f7343c614c Merge pull request #58 from justinsb/upup_smarter_delete
37e0aa81f36ff46a668435da2a5a3f480a37c248 upup: better cluster delete
e8d9014787abc96ef60e5706eeaffa9aee3dfb7d Merge pull request #57 from justinsb/upup_resource_tagging
f7bf0d038481bc7b6c04f8f969321e77cbfab696 Merge pull request #56 from justinsb/upup_fix_hasdependencies
0c716f8d576342601162f5d0a360ef60f51c2517 Merge pull request #55 from justinsb/upup_dont_hardcode_122
8429aeb9a9fb105684c851383cb467c9f12c90cd Merge pull request #53 from justinsb/upup_makefile
209e3a2431cb1b193ce13b30e00b8a9c3d71d5d2 Merge pull request #41 from roblalonde/master
bd897d81dd949392e0e7a80c0417a7044529afc1 Navops Launch Information
afeedb4e5cabe4f8f2a2d49735012509d2e59ab2 Merge pull request #59 from luxas/fix_path
999d8da587b6dac699ed8148786126d71d281b8b Do not hardcode the path to docker.service
3343c7d379413fd151ce9216e80a07fa7bc437e1 cloudup: better retrying around resource tagging
5682b76a347ede75cab1c8fa662a8c69233368c1 nodeup: make sure tasks implement HasDependencies
f402bd4d90c29500542a6a8bfde31e9f1c001b53 upup: don't hard-code v1.2.2 in image names
482f6e52c9813e62a45dd73100b12a7470a97977 nodeup: pass --master argument to protokube
352d5239d4e38c156dc5c7f1e3d10a8ac873902c protokube: only try to mount the master disk on the master
730f66a5d03d4b0675f38c0618bad9e1389304b9 upup: Add gofmt,codegen command to Makefile
bf6189664414e2beb07e54bcfdadff0448364bbc Merge pull request #50 from justinsb/upup_keys
51af6f2cd3069dacfb772127cc87d86690edb2ff Merge pull request #49 from justinsb/protokube
4f94728b1278feb24ff7e1d2c1a3130ba8e25cee Merge pull request #48 from justinsb/upup_elb
af6b16ad33981e550b71ea2eb5f4ce9a61bf9bbd Merge pull request #47 from justinsb/upup_delete_cluster
b99d00dbed664c5e4410c3a83b4777b060bea20b Merge pull request #46 from justinsb/upup_route53
a56fa84787a6e1d82ec015bb42f00904a52b3682 Merge pull request #45 from justinsb/use_generator
6dca45ad6e3a53937ba2cac2446a6704e2c30cbb Merge pull request #43 from zreigz/fix-volumes
9b8534a1bb6b24f00c80533a7685b81ff6767ad7 Fix mounting volumes problem
7a718eb0345b078afab23bc7ff7d8f4205d90f81 upup: better secrets support
ad46ba4e9d6c4dcf348266ddf2c2780ce2a64288 Protokube: prototyping the 'missing' kubelet pieces
5df985b4d4b0dce70c83d1edd97edc1d11f68d4a upup: simple command to delete (AWS) clusters
9d8ca71dbff457030ec6337edfa81e0a4c6f6ed1 upup: simple ELB support
42abdfea4f4fb7ad02fa856edb9665a9a512bcd2 upup: Simple route53 (DNS) support
0b06fadf0484e370a02db7ef2e53502e0cc95780 upup: move string-slice comparison functions to utils
a89eb68bfd08d02f0487d98fd7d76e74275c1548 upup: replace parse code with standard json unmarshaller
0fff7ab87e8c80c4a59c2d9e745e9db28d7e5850 Use generators in tasks
4d6c96284237ba5cb22848f326429a0f9e775e84 Simple go code generator for fitasks
4acec57608ce938a7623913e9f78f47c47ef4815 Merge pull request #38 from cheld/auto-detect-iface
1abca3dcb30b81f4067fc88e0805bbb4ad6b3f43 Merge pull request #39 from cheld/fix-doc
99ee4abea598889eceafc131ee5ddc79b9e5ea31 fix link
75c6ce681817e125bf44383ccf0863428f1e15c0 automatically detect iface
aacaf3a20494ba751ccc7c0af5f8cb23b1093cf0 Merge pull request #36 from zreigz/add-interfaces
853ab8fbe79ab060aeeeb2f55b039ff4dc041cd3 Add possibility to set interfaces during configuration
b3c28aabaafbf0198063bc764783f5543dfae4b2 Merge pull request #21 from justinsb/upup_executor
06bf5fd48964029dfbb004b8e0dc85df883ab233 upup: Executor that performs some retry logic
68e532fa1425b234bf98b7064839f4f99f9eb9bf Merge pull request #20 from justinsb/upup_export_kubecfg
9a4751217311fcacfcb0ba11c27c1c39a37b1ff6 Merge pull request #12 from luxas/docker_multinode
623d9c7cd0ddec97c66183df2548049a51ec83aa Initial commit of docker-multinode
d4491c9fe66f58166c6cfbb4dd0b3def0ef69108 Merge pull request #33 from mikedanese/generify-phase2
310c447052598369ee2b69b2a3d0d1d68aa0702a min-turnup: move gce specific bits out of phase 2
c84f5d33004a53fab669c6f33151b949f8ba0bfc Merge pull request #32 from mikedanese/kconfig-cleanup
7ba7cc7d62b5a29379a6fb4e2f35ed07679eec9b move the gce specific cfg.jsonnet file into Kconfig
7d69de806f2dcb901374d1fca73c431a8819fc6a fill out the basic Kconfig structure
9a6121f69fe0becfa92794fc161b8ed4850c8316 Merge pull request #30 from mikedanese/reorg
e39026cd2dbde8d6c3e2824fe8ea7822c4924793 reorganize turnup directory structure
5bc80a3fde2121c0cc69a7f534b5ca43dbb56046 Add glide dependency on cobra
b9a93e54fe290bc66bf180999c31bfa1890b877b Add upup command, with a subcommand to generate kubecfg
a9a690259ed5f097e4957f8e154446dcceb72ada Refactor Certificate and PrivateKey to implement io.WriterTo
f8b81bf51814373c528010e9ecf0ca9afc7f78fd Merge pull request #28 from justinsb/upup_aws_retry_tags_on_eventual_consistency_error
2e82f8894ab3d515961bde8891db5dc2a86bfd82 Merge pull request #27 from justinsb/upup_aws_image_aliases
48ca01e2fd9dea6c018b43558f4f0a443adbb877 Merge pull request #26 from justinsb/upup_aws_instance_userdata
e802890ee08134c617470670d3caeda5bfa2dad7 Merge pull request #25 from justinsb/upup_dryrun_print_interface
9468ba0b45b32515d4adf1f7a1a5668fffd8a69b Merge pull request #24 from justinsb/upup_aws_iamrole_policies
065731338a43e8c38538ac1eaefe02bd9f2c9fc4 Merge pull request #23 from justinsb/upup_aws_instance_tags
1408fb912fe0e19b178fc3dafe92037bd120c320 Merge pull request #22 from justinsb/upup_aws_keypairs
f6f9b4c3416391161c3981e3b5e3bb0f33bec6c9 Merge pull request #19 from justinsb/upup_keypair
61ef026502a2085ee8d5b567d2ef51f1b0315a70 Merge pull request #18 from justinsb/upup_reflection_redux
2f8009c0428dd28454062b0c2cb0c51905004165 Merge pull request #17 from justinsb/upup_gce_metadata
7e53237537b9f90f7c3c1b7009b462de449e9170 Merge pull request #16 from justinsb/upup_image_url
ad32fb3d26a917722dc7e0a32867d8c5e3471597 Merge pull request #15 from justinsb/master_pd
0e1fa9bc414d53061b807920092c3ba2030999d3 upup: tolerate aws eventual-consistency errors on tags
a148ee0c898903831bd541edaa7dd5ea49d34680 upup: Map matching image ids to source name
19abd363f33a1d2f6edccfe78b26a2ba764e881a upup: Fetch instance userdata on AWS
b7e22ca0fce68d7a8da991ae05866632cc1fb3b5 upup: fix dryrun spurious printing of interface values
12ffd59726ba3fda8a520e06624595a67b131e20 upup: Perform JSON comparison on IAMRole PolicyDocuments
1358acf581306377368d01eef45227bbb7e1f19f upup: Discover tags on AWS instances
3cccef5f2be5cb293a57929418a485555c4c9cec upup: Fix fingerprint calculation in AWS keypair
5696c340875666d9febd964a6f64ae7506117f68 Rework keypair to fit our change model
38e04fff00fab5a345ac0f5fcb8cd8aba4380e6a Support changing GCE instance metadata
1258b37f68ba24c35c1162b26ca52efdd4a93435 Allow Render methods to take fi.Context
bd3156ded02b8491d19b924ecbe14b17bbb0ce41 Create HasAddress interface
da78a6aba97139c3d7dea9c6c9b77876ecad0d70 Make reflective walk more logical, use for dryrun change printing
46f394d0e7b69f2861489e1df209194cf0613e35 Discover metadata on GCE instance
8359ec6192e426162052dbc39429b84318998bde Map GCE image-url to string consistently
d54b621568718c9b94d562f955c0b3dc3abcbfae Merge pull request #9 from mikedanese/cluster-v2
89ac8c133a7ad37732bf86eaff314661df388da6 initial commit of min-turnup.
f72f09b09359d99256b9764fdadbdfdd0a739a18 Support for persistent disks, users & symlinks
61e78583db6c615af76e7751253062e47e1f36ce Merge pull request #14 from justinsb/fintegration_aws
caab4af5afd0fccd1733d26c12cf7b78401a0936 UpUp: AWS support
303cab2e387a592eae83d32c466b147134d29f32 Merge pull request #8 from justinsb/fintegration
0c79afbac45f8a7c5afa0c7d0c46b4db05877908 Initial version of upup: cloudup & nodeup
8fe843bcbcc7bb3ae53b7f404bffabb63a7cfb27 Merge pull request #11 from mikedanese/readme
692dae3720199fab9ee2c121d094811e0b98a5af add to the readme a description of what this project's goal is
80507f1aa9aa6d6541aef0b570f68ebf4c1da55d Merge pull request #7 from justinsb/imagebuilder
337ae3baacec2396fe4e69fbdbc63ca1cddfb5e8 ImageBuilder for building a jessie image on GCE or AWS
ae893476fa53a875fc4c9ebeed1b63c1064f8d6b Merge pull request #2 from mikedanese/addons
7141fa4410939f3795a6275302f21ee25380e859 move addon manatger into subdirectory
5eec0fb93f632da7899b930789f83ccc0d201cb4 Removing versions from deployment names.
90f046e9078fefe773ff074fe9927803f895a3b5 Support addon Deployments, make heapster a deployment with a nanny.
0ca684752af09d24cf78fb33ef4a2e6165a02e16 Set kubernetes-dashboard as the default UI addon
2c7fa3c243ab1a348b9efc7008138eff04a33b75 Support master on Ubuntu Trusty
e9f32808dca40e702f7163e5e1b7905c17a89309 exit if unable to query status from apiserver
8df36f9eba8e5ef5cd3f0f2bc7ae9a5e808f4383 vsphere support
4a11aa3056934f1647e70e9e1827bbadd4d647b2 Change repository references to https://github.com/kubernetes/kubernetes
09cb75f3dc97d02d83b60584a60d5595af23f96e Salt: force service provider to systemd if systemd
f5df2c160d3ea33e14951fe423e238501122d230 Fix issues with Python3 and bring up a dev cluster
4c0c99033d5db60c19a0bac1bbc3523bc8fcda8a kube-addons: Use python container if python is not found on the machine.
65c48a79fc5e14f5b133f51d3f31ba920bafbdb4 Cluster-loadbalancing addon
66d200a7515444b4e692e514be45b699e20628b0 Make heapster config creation dynamic
d0f0177ae4e3ca6aadc4d76e5fdd8e05025977ab change -o template to -o go-template=...
a2f3dd10d80733a5a6e7eb82ba2dd56d3415954a Use quotes more consistently
c934df29a8a96841c9a15a0a7718343bc1257469 Use a persistent volume for the docker registry.
f66ca094f7dc98a70a789f6dd1bf2285f4672e0c Launch a cluster-local registry.
3e0affde9ba9b4c739d3a27c97e8953f71790d4e typofix - https://github.com/vlajos/misspell_fixer
ed33e20824feb90cf0e147a9d9adf06ed30694fd Respect KUBECTL_BIN in kube-addon-update.sh not just kube-addons.sh
609eec02fe8b8ce99acbc4e4794b6e6f05f092d3 generate-cert: allow for alternative paths
2d64a4c911630ad041022493d0bbbd8eaa5c8eff Made enabling Kube UI configurable
6b070f69d224c03348dc83abfae71c7f31faf785 kill child processes of addon-update on stop
6ffbdc1708fccc18ab446d84188ff9452ecf8f5d Wait for service accounts in the kube-system namesapce
3d28c6cbabcf0ad1da51a4548d92aab06ed6813d Move things into a 'kube-system' namespace.
914ad5c63ff8ac59989cfa9e43f374c45a5a948c Salt: have kube-addons service depend on init file
7dee33b12d2b7a53bd3cfaac0d625902e85a2d5d Salt: Add more dependencies to systemd services
400d9a894053f987593d7a3061e2f98ad60a2399 Salt: support systemd (don't assume Redhat <=> systemd)
224e3ca9c52f242b13524bbc244bd714b57fdb69 Stop exposing v1beta3 by default
6b30c23527b6492af2afb20d441fb643b47380bc Add kube-ui cluster addon for serving k8s dashboard UI.
8532e34774d5b985723923485b9516b2eefd0167 namespaces in addon update
0eecf63fb45ec55077d3de4db933de44a094fba9 addon updater should not retry too many times because specs may be invalid
cd8d6ae832b47ca3e3960e305bc7cc09bd81bca9 Fix issues mentioned in #10520
95f8c2d6c093e91764c3c9823717ca3086c0acd8 wait until a token shows up to start addons
70bee7b6060571e3caf8c4bfef82d794989d7926 Updating heapster version to v0.14.1. Adding a standalone version of heapster which exposes stats via REST API.
1e507fe243d954b2861792fd6ce76c968dfd544a Enable InfluxDB/Grafana for GCE in addition to GCM/GCL
232c76de4c5cdf20786edd4315dd428c187831d6 Updating heapster version to v0.14.1. Adding a standalone version of heapster which exposes stats via REST API.
6e8e1d877edbd52b946d1dae85d571219448d470 e2e test for addon update
d7c72f79ddd3fb0681a85e0acab2a7c74db689db kube_addons - Adding variable with default for kubectl bin. Fixes #9599
8e425f508411ffbdc30ae909691135702845946f Distribute the cluster CA cert to cluster addon pods through the kubeconfig file. Use the $KUBERNETES_MASTER_NAME from the kube-env for skydns, because it can't use the service name.
534a8d6f72b74e99a02c30efacb8175e32567d5b kube-addon-update.sh
8fd21e459fdfe89352cc1951f5027960895a24e6 Enable InfluxDB/Grafana for GCE in addition to GCM/GCL
06d3aac90e2222808d4f07720cd027bf6ff9bda0 Create LimitRange object for cluster before addons service
107cbc92a5f3da326acd0570a1d349629aa965ec Updating /cluster to use v1beta 3 specs, and change a lot of polling to healthz instead of api endpoints.
6a907b1135278f9eaef8983fda754002fedfa54c Enable Google Cloud Monitoring and Google Cloud Logging instead of Influxdb for Google Compute Engine deployments.
8f7090bce12194909ad3126bdd2fb52480838730 Make copyright ownership statement generic
68f9aafe0f7ca0f7e7b12937d3d45c5a18b43c70 kube2sky using kubeconfig secret: take 2. Point system secrets at https://kubernetes. Override in clients that can't use DNS.
1d533e43a38321fcb0a9844b5a5f3e028fd4d998 Convert Elasticsearch logging to v1beta and de-salt
8a926f2aba842368e8783ecec0028cc4ed23c9ee Create system secrets in kubeconfig format
ffe3ee4472d66cd04a80a829ab0bd811efe76943 Fix kube-addon retrying.
2ca3917fcb7f31de2a5ad790ad2a597ad85df913 Make secrets at cluster startup.
93e34c6eedeaecc5664e1695dd2bc14a1529392c Use same addons script for init.d and systemd.
30944057bcb5b975242615a6b3748f9ac373c2d7 Retry kube-addons creation if kube-addons creation fails.
f6caab55f860a0e0e14d03cfb72f4ca70866a351 Retry object creation with --validate in kube-addons
e6a85857210134303f8eeb0d51032a8ba03be806 Missing boilerplate
ca6a76a5ce88bb5937c0eac7f1395c3e937dedb8 Various vagrant fixes, etcd 2.0
e4119f09125cf314ec4ac685ccd94b3d3f0370a2 Deferred creation of SkyDNS, monitoring and logging objects
6ad30a0711466107edb3e91c51f50355cdb49c8f final commit
```

Status: Fast-forwarded successfully.
