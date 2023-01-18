## Syncing openshift/cluster-api-provider-kubevirt with stolostron-engine/tracking-openshift-cluster-api-provider-kubevirt

## Status Summary:

release-1.0 -> backplane-2.0: Picked up 402 new commits.  

### Branch release-1.0 -> backplane-2.0:

New commits:

```
0a11acb9599d847fd285dfcae257cdee6e590ad8 Merge pull request #42 from davidvossel/autosync_upstream_2023-01-17-20
8e6cce8a91b0d3c4aa599863e48f47d6a640808f remove tmp file
ae0761be42fdd05ac1044e9245e70dbe99876bb8 tmp file
9c053af24c6ab9ecf9faea79f6a4321f5fe40faa Merge pull request #40 from nunnatsa/auto_sync_upstream_2023-01-08-20-06
8554732044746c7937ad687719dd3d7c0199be05 Merge remote-tracking branch 'auto-sync-script-upstream/main' into auto_sync_upstream_2023-01-08-20-06
e4372d30043eff505ed0f2bf5af3ce1ff1723a61 Merge pull request #215 from nunnatsa/fix-release
d1aee70e30beec4618f48de414f8845180ec5914 Fix the release automation
6512a4cb2d519bd9c04927b9cc0c7434b6060ab3 Merge pull request #213 from rhrazdil/passt_binding_2
cf2dd64bcc74caa2be99a8a7551dffe50bd78772 e2e: Test create cluster with Passt binding
d03c80b9ae208d0823cdf2948dde4f7d53ee5712 Merge pull request #214 from qinqon/activate-net-multiqueue
35cd1c502a4d0022aab25ff94895296067de9936 templates: Activate net multiqueue
939d397d8123163be6ecc12e67ec7cbb506cc458 bump kubevirt to v0.59.0-alpha
b3985bf5d477237657ec9c5ee4d5eff717501444 kubevirtci,passt: apply recommended config to infra nodes
e15fa8640893a28939036b64b7216de0aef624a8 kubevirtci: add CAPK_TEMPLATE env variable
eea13f0f07dc18e95b18e5d61f2a72cd2223eca2 passt: enable Passt featureGate
32123fcc667e7b41909891e908d970a65de9c95f passt: add template with tenant nodes using passt
e96f47d3ec3f11610ce15b7b0568fe9a7f0d4511 Merge pull request #209 from qinqon/add-all-templates-to-release
5d8762be2eac429a6f9236b5bce8ba5f425cbb56 release: Add all the cluster template flavors
792dbff84f80f93d98ba6209a21e6dd51a968dcd Merge pull request #206 from rhrazdil/bump_kubevirt
b3e30fb78254befb5a49a3fa8f53c28e1a2da90a e2e: fetch VMI before removing test finalizer
6a77a49da11bce48c0c1739f76a77a32c6acb48d Merge pull request #208 from brianmcarey/allow-insecure-registry-podman
47796bcb1e2edc616febc3667a4748050f84dcdb Allow podman to push images to insecure kubevirtci registry
2e924bae28012a7d023c0c99e5fd0faaf736adb8 Merge pull request #207 from nunnatsa/remove-IMAGE_REPO
58472fc20e7c5b63aae922b98db7ed1adfa13851 Change Dockerfile syntax to docker/dockerfile:1.4
1c308f387c6c84536bebb6ae204b2774c6ec80f4 Remove the IMAGE_REPO env var from all the temlates
a91a2b153bcc123e5d12c1afc902397e916044f3 bump kubevirt to v0.58.0
ccae28797861a0c232685823e4f58089b2d75433 Merge pull request #204 from hiromu-a5a/docs-pci-passthrough
475ad691da2ef59cb0f6439f4a31d7ed8eafa862 Add docs PCI passthrough
9c5f8565ed56298801120f61fff92bef0330d000 Merge pull request #202 from nunnatsa/cluster-template-lb
e44e0429025ca234c8bed12f586f92485bca02a4 Add the new cluster-template-lb.yaml file and release it
cdb7a4cfd3e7b9e4291c142045825eeaaf473382 Merge pull request #195 from fengye87/main
fd908e4baa5553bdf6dd7707db1d37c4a504721b Merge pull request #188 from qinqon/radim-quique-collab
3967130045e5034d40bed7d469e4d906c42d59da owners: Add Quique
622baf93517c8d6ddb5c36e8ed971265e30c750a Merge pull request #182 from rushyrush/main
0dac7c2482d32e0d9cdb1d0bc024c0e6b5ce591f Merge pull request #194 from davidvossel/update-e2e-to-k8s1.23
8b5a2b6434e17980a36d57c200731533610ea8dc update e2e to k8s 1.23.10 guest clusters
4c887013cef47b18702756b0d2ac0a3a84ee193d Merge pull request #196 from kubernetes-sigs/revert-183-passt_binding
3204b1f60c3bc9b52f76c9c43cc0c85046bfd524 Revert "Add passt template"
a87d15241579d7a76a6247e84956b68d61dda9d5 Merge pull request #191 from qinqon/kubevirtci-call-fetch-when-necessary
57f35c3b0726bf0e38a54f30d816e290f806e21e Merge pull request #183 from rhrazdil/passt_binding
6b52ac1356fb3daeb810687d86c7ccc63732f50a templates,persistent-storage: configure static mac address
eef8e522dcf5766ccff794c2baf1cc3be7366d5c kubevirtci,passt: apply recommended config to infra nodes
3bb481b9b38a24439453a58b92216d4b6bb3c4a6 kubevirtci: add CAPK_TEMPLATE env variable
37dfe775c5c53d269752e4c3cb8f4f6bdf0ab916 passt: enable Passt featureGate
d04a7dadf265d2631c1beb044caa72f87036bbba passt: add template with tenant nodes using passt
3efa36fde19fc89343bfd2631dbe33f52d3988b4 bump kubevirt to v0.58.0
6a503203bf5abad6f6e7fa77a9955d753a85db04 Fix CRI_PATH var in template files
eeab6464351cde302af186e847dd5bb18a86adc6 kubevirtci: Refactor fetch mechanism
bc265c633a5b7a16782255db301d2093ab800957 Merge pull request #187 from qinqon/check-make-generate
f7bfd29ad0336c840400695c38ac5eb973197966 ci: Check make generate has being call
586d578d8790c3ff91c9192936fb5a20cf64b9ff Merge pull request #186 from qinqon/update-kubevirtci-guest-image-k8s-1.23
273c6c5c2d05f02e2cde28ca40c9b1a524d2eae8 kubevirtci: Update guest image to have console
03d6f013b1309fada53ffd3276532f52f8b03199 Merge pull request #168 from qinqon/poc-cloud-provider
7e0222240f425dee1f25e839c243ea690c177493 kccm: Create tool to generate kccm flavors
1b45e02b47e1e20ee7fac89228a76a9f7c39f5f5 minor docs correction
dc0cebc612cc0dcfeb37fe29749b8ea6123b27a9 Merge pull request #176 from davidvossel/fix-secret-reconcile
9d57dc958dd8e0d41e32f47760f294a688e5c284 Merge pull request #180 from qinqon/test-artifacts-fix-dump-version
b5c008529a196af347be5e82a8aae6b502688668 tests, artifacts: Fix the version to dl kv dump
a9938fa155360086cd1d33dd36e3d3f1b11dea5c Merge pull request #177 from nunnatsa/add-file-to-release
725371a0898a1928490eb85cf7c86bea35fedab4 Add the cluster-template.yaml file to the relrase assets
e8821007d999dadd091bb708330020a2873b0ba4 Fix unnecessary double write to ssh key secret
09e50a0d19bf32b41359edaf29ce91dc6550ef40 Merge pull request #174 from jbpratt/publish-multi-arch-manifest
13f0884ac042d80ac51c586629073a4bbb7a82d6 build and publish multi-arch image manifest
43916429f4417c3b18ded7052768e5fb4265c0a6 Merge pull request #166 from rhrazdil/e2e_sonobuoy_conformance
5ff4ba0cf9eac83901a0340756f923d079e9c473 e2e, conformance: introduce conformance tests
48146e1c41d730c13e159b11d147c9f0f42361e6 Merge pull request #171 from isaacdorfman/update_clusterctl_metadata_version
05f7f2e0ef9b44a67f8af49284fd680c8bce9d27 Updated metadata.yaml major version to 0 to fix clusterctl problem
2b08d6d56dafa0916352ef8dd00df62a98e135ee Merge pull request #156 from qinqon/integrate-kubevirt-dump
b60493361bf3dae57676c7711832252dc136ffd3 Merge pull request #146 from qinqon/kubevirtci-add-curl-lb-namespace
657f0755cb2368de238925ffb327cacd7a4c6ecb kubevirtci: Specify proper namespace for curl-lb
ae33230569cc137235f5a6e049194e8969d8261b test, reporter: Integrate with kubevirt dump
48c632eaf202b5a6eeb508ea559cd6d03293a248 Merge pull request #145 from nunnatsa/drain-node
8a5e0dfb46832a55a703596ca2cb4bac4dad756f Fix code review comments
8c89b7c2c458d9435bca51bde8db16042dcdb67c fix bug in the vmi eviction controller - wrong predicate
d8b2b98c12f530e11001e73c9ce2ff8616db5565 Add VMI eviction functional test
210fd52c7a6cdcbd96f60593923ceb6e9095673c Drain node: add timeout
b9d14c972c1c759bff545a0c590de47d27f3f8c1 Apply code-review comments
160f5dc75f6f4832a97523858661163264ea8729 Graceful deletion of a VirtualMachineInstance
5aa3a3d351970f31df0702ed499a764177518f1e Merge pull request #167 from pjaton/fix-infra-secret-lookup
f64858284612a4bdd9b9358d0d1af9761e966356 Merge pull request #164 from pjaton/add-secret-labels
a9e7e115a5c04c4be7903be4da5ae0bfd7fdb0a4 Look for the infrastructure secret in the owner namespace by default.
abde9dd09f4a9c93041f74c4510c497365c383c1 Refactor setup-scheme into shared functions.
58dcd707d39d772ac87918cb3d580f9c78f0b738 Merge pull request #159 from pjaton/fix-capk-user-add
528668f3ab311adff6816154d623573039078a2d Use gomega matcher to check labels
fe229f76cccfd528142636857662622a894523ec Merge pull request #154 from qinqon/wait-for-tenant
ab5ec822412a093702d6e71a01abb58ac07e207b Copy Kubeadm userdata secret labels to CAPK secret.
7229ee49f4359f7f1ccf668fd7ec726a31c618d7 kubevirtci: Wait for cluster and calico
a8097c471d38aabe38179cd187a4d95618a834d2 Merge pull request #160 from pjaton/fix-namespace-logic
a167f931bc9c8925c2fbc914f994f33fbcd61614 Select kubeconfig current context namespace before 'default'.
46a88fa2a3d40bccd41f707a67442ee4613e3ef6 Add capk user properly when users already defined.
1aeca5160094199b11ea955d41247962ed8fcae0 Merge pull request #157 from pjaton/fix-patch-of-deleted-failure
749147a3588ead9c426c50432f2d5af689c9aad1 Merge pull request #132 from agradouski/issue/90
821b0a8f31782fe11d788bddaac40e3e8ee1ccf1 Merge pull request #151 from pjaton/fix-external-deletion
5528680adad6b9f7915651a1e47f9572aff8676f Avoid reporting not-found errors when patching resources under deletion.
239dbcc7745da9c77159e173bd3f8ad3c6c6f184 Search for external VM to delete in correct namespace.
d6c15cf26999646e0e44aaad1a25b0c157c4e461 Enable specifying namespace where VM and VMI are created.
f10864009872a596c01baf5d5aca31d5cd509a4d [e2e tests] Cover creating tenant clusters in external infra clusters in the integration tests
1dd643483079ba639de1ef7ceb61b792fc729995 Merge pull request #155 from davidvossel/pin-kubevirt-release
cbc09acce08668779fb5c8cd3dc8f4cf3916c94b Reduce memory usage by using local storage provider
33930bbe27893ce7dfc4fe6fb3a82ba637464c93 Update to k8s 1.22 guest cluster image
d463f340402d21b7a372b72752d19a2f7f4e0780 Pin kubevirtci to a kubevirt release to prevent CI regressions
41c77a793ccbcaa21a05d9b76fd2d4f02c4934f5 Merge pull request #148 from davidvossel/revert-144-e2e-test-fix
cce88a057c5fab2135d308779230d0b0ef02cffd Revert "Fix flaky e2e test"
3fbdad97b90f6dd4cc691a213f2d86f992d39937 Merge pull request #144 from davidvossel/e2e-test-fix
d534fcb93ceaa63b6e437f191c29a0c375d6a4c8 Fix flaky e2e test
7bc78d31ddaad7f2d357c04bd770570ff78d8fa2 Merge pull request #143 from davidvossel/network-fixes
7c2ee63569d039bbff60d4e5a60a717819ac7c1f Install cni and verify pod/node status in e2e tests
7880b04a3adab6892239e20381f8756542ed43f4 offset tenant network settings from default infra kubeadm settings
a6e458474331f680e908e7a265a47c2982735bd2 add install calico to kubevirtci and update cluster-up git hash
3457e8e7d217e5622d0b29b281c25fc7b4008647 Merge pull request #139 from nirarg/e2e-test
435fc16bdf9876fd8b799798f158edeab2db617d Merge pull request #141 from davidvossel/kubevirtci-metal-lb
138541efad28e4b1705e9a02febd5578c957e1f6 Add kubevirtci function to clean local cache
80990677a2a0beeeed80f543ae5d5c72924b9775 Add kubevirtci command to install capk from upstream release
f7062846a00d3d14f50eff487bbabc91e061b83e Adds command to curl a load balancer within infra cluster
c6207576b42f2275f7d2e8e3722cb6826fccd98e Add kubevirtci option for installing metallb
62c6aae698496a5e9e96d58697ac8c0e17581d65 Add tenant cluster verification to createcluster test
4c4743db82f5e5ed3a74a1e807a5db9d3b5e33d2 Merge pull request #140 from davidvossel/kubevirtci-updates
60a0162cc8f9a1f9dbdd17c2ab61eeb0fba3637c make separate kubevirtci command for simulating external clusters
f01885dc9eb2b58a6c26c96fd7f43478d5574cfb add kubevirtci destroy-cluster command
0857b5fd51fd2314922b2470db8fef9879dd4e5e Add ssh commands for infra and tenant nodes
ed7eb9e9f5e039c6529b629c5060adf8e0ce4cde Add namespace to kubectl-tenant command
27cedcf60090763cd8630c6e44b953920bb7306c Merge pull request #133 from nirarg/kubevirtci-tenant-access
a6326da5345df60d33eb0244cd904a76c141b994 Merge pull request #136 from nunnatsa/move-to-go-1.18
cf80b5aba2674a4d252abfc232c02baf606b1141 Move to golang 1.18
682b649ef9784b99db9ef31803c4c4b92348b8f3 Merge pull request #135 from isaacdorfman/image-builder-docs
879a4cb01ec526aa2241d1099f86faa23acf6857 Merge pull request #113 from isaacdorfman/clusterctl-integration
7f597e1cff22843691817bf88c77e1495f18ef0d Fixed a linting problem
e5c71d00289bf2cbad41b2dbff084ecadb72be24 clusterctl integration
93595d8f92d29838e96a0f3229388e8c2e32d82f added docs for creating the image-builder image
f89a85c1cdd9474f19ab578607a1fe9e8eb4d1b2 Merge pull request #134 from nunnatsa/debug-e2e
fa1c7cf7d5b3996cb82a950984eaa437bcc809f6 Add failure printout to the e2e test RunCmd function
a278f8d014d661261a8b5fc7b47f5289a719283e Merge pull request #32 from davidvossel/auto_sync_upstream_2022-04-20-17-35
c5b9ccc0c67c90b98d3fb50cc75abd0d8f3e421a kubevirtci: Add option to interact with the tenant cluster and improve usage (help)
5850b3372674503ece125659bbd671f5252a812d Merge pull request #108 from isaacdorfman/image-builder-integration
9d7d45da12860abd95ad058a946ea28e0f9096d6 added integration with the image-builder kubevirt image
8bd4fe1a3aecf9f0e37fe75788e1ad065529689f Update the sync script to use merge instead of rebase
004c1a53f674595b30a3047285b0a7ff6e6853b5 Merge remote-tracking branch 'auto-sync-script-upstream/main' into auto_sync_upstream_2022-04-20-17-35
7874a579c45894764b968c3b788fdc2a76192e1d Merge pull request #131 from agradouski/refactor-e2e
134621305347b10549e0b9c05274eebbbd8a982c refactor e2e tests:
167006ada52114a31e0cca0777a107451fa771e0 Merge pull request #130 from davidvossel/failure-reasons-v1
8eca681d09122d6208b84d5e4be3b60e4fb3026b Merge pull request #129 from nirarg/clusterkubevirtadm-kubevirtci
5016900be2eca0f814be429fb2cbcf27b31efffc Change "./kubevirtci create-cluster" command to use clusterkubevirtadm kubeconfig
2065d825c3d4115abc973a7b808497a2d1151eec Add e2e test for MHC and FailureReason processing
ac2b012db4a9ea48b6bebd4a97e4291520254d25 Unit tests to detect terminal state
b8f770ad22ec4d20febe70142073b022535e4fce Set FailureReason on KubeVirtMachine when terminal state is encountered
ae3de67b9d8942b1d5f977d03939c07fc60407c9 Update KubeVirt API mod dependency to pick up new fields
e030c972664a14e9f1731d14f3fc38facb4c0cb7 Merge pull request #126 from agradouski/e2e-env
d7673178221a83ebc4f58562c6641f04178cf335 Merge branch 'main' into e2e-env
5fc433736357bc5f9478c6ffd634493bfb58e412 rebase
cc7a4f1c397d54b3168400f506c8be1a514db889 rebase
5931818884646f2ebf580648e850ab57ad5d680b tiny change to trigger e2e test
7070ec18e5e2a6b4dbd70b3c0fb26daa272e241c add printout to e2e, to check the golang version
e8822db3c65e6b36d834a4f25e621de4417006bc Add More permissions to clusterkubevirtadm Role
81d966cbddfaa2951c0fe3a4b19fad2204d8e2f9 Merge pull request #127 from davidvossel/switch-to-rook-storage-class
62cea3229ecd84119742c6cae1b5475ebf4310df Merge pull request #114 from nunnatsa/fix-e2e-test
e01e18de69896d001d3bdb42da74f14c6b34d94b Merge pull request #128 from nirarg/clusterkubevirtadm-role
5b655a36dc7dc58fd551e89ff241a04762e2e29f Add More permissions to clusterkubevirtadm Role
c354cf1dc0fae51ce9e95416507772404e1c4140 Switch to using rook-ceph for e2e storage class
24f3704eb11554c70b886b94c11a50d424d53411 refactor: move environment context out of e2e tests logic
ac59574e3119dcf19f11d700dd8396f569372f2c Merge pull request #125 from nunnatsa/fix-e2e-test-lane
44fc5c4922b949e24f71dc73c31ad404b890af48 Restore the E2E test to not use clusterkubevirtadm
739ac3615316ebf9dccfbae0840f4326ef073f59 Merge pull request #123 from nirarg/clusterkubevirtadm
ccd6e430424640bcb09e8e0e458e043a6a09d2da Change clusterkubevirtadm to use --kubeconfig flag
0e0271b6d6020e88d22afd790a18694f41e5a59a Merge pull request #122 from nirarg/clusterkubevirtadm
b70c5ca57d1137d41a3630fe9fdf70cd3b648f50 Fix clusterkubevirtadm-linux-amd64 calling from e2e cluster creation workflow
94808f836cee565f0630c99b5d2da4119b69685e Merge pull request #121 from isaacdorfman/clusterkubevirtadm-fix
a36c7730039a895f65cf4cc93f9a2953463c4784 clusterkubevirtadm-fix 2
82d4736497e58bcba3e405d11af248e369963e46 Merge pull request #120 from isaacdorfman/clusterkubevirtadm-fix
6769e5e4afa2f997a70ac796d7307d2aac1d8b8a clusterkubevirtadm-fix
7d91fc3db849e27de75e1a3949f93cd0c077b04f Merge pull request #119 from nunnatsa/fix-e2e-test-go
0d6d351529f9fab2cc125a98c3a4eae1095b3524 Merge pull request #118 from nunnatsa/add-nahshon-to-owners
70472036b2386e7182b9ef6ad6b962fe9e3f08e9 add missing go compiler to the e2e test
00d4123495ddabd33734bc4f53e1b9961ed12432 Merge pull request #111 from nunnatsa/clusterkubevirtadm
4cf5f594f0b43308b5454d140bd94934a4b6611e Add nunnatsa to the approvers list
79a28d6a0be18b48bc37e5cdd1cd0de0e10e897f Added new CLI named clusterkubevirtadm, to manage the infra cluster
ec9b80fa7edf9356204300e2625c884c18ec5045 Merge pull request #117 from nirarg/approvers
d9f57d9df2ef59aa7eca87a19d7f2e25d593ce87 Add nirarg to the approvers list
f148a9e17f4083537ecd3c626ea327352994bb5a Merge pull request #28 from nunnatsa/auto_sync_upstream_2022-03-17
aecd95423ae7659db009b8860b8f46ac96df3a09 create PR
0fc14619a46870599c0ca385a8ae6db8e0114ff3 add script to sync with upstream
86301ce6d6d6fe1267d84ae54eff54a8c5cdbee9 Automatic sync with upstream
23727f2d40065f8ed9413e09c3e6b095650caa7c Change OWNERS file
29dd04a6c4087a614415c04787724056fa1356ff Merge pull request #116 from davidvossel/fix-external-managed
93fa3b2b3dfd416f2f84043c85e6a2f022e1e3a0 Add e2e test to ensure finalizer isn't added for external clusters
51202f7f41dacf45b955d52377396e601946301e ensure we never reconcile an externally managed kvcluster
12d5e52b58144d6a0469e5c5a30c7ff225a644cd tiny change to trigger e2e test
12b18e29267996ec028f61a0b0d8723fef0a7d3b add printout to e2e, to check the golang version
e456a2756ec24d751ce46c96254863b92ff7289f Merge pull request #112 from 0xFelix/patch-1
09da20fdab19bb8feaad86b560d95fc7ef5a20ac Fix the ginkgo dependencies to match v2
c989b8c64686d3266094de5f9b8b4c9da752dfa4 Fix typo in kubevirtci::fetch_kubevirtci
0eaaac76ce351a2e74dca30cf3e5e6730db36526 Merge pull request #23 from nunnatsa/auto_sync_upstream_2022-03-09
e9096d9f8ca40ebafea3ef4c621eb299e2b0a9c7 create PR
db36d7d1a45ed64d3ec143e133a4e9582a51d489 add script to sync with upstream
e77c8202eb0a97c07fc0adb8ee81ef2a62013b9d Automatic sync with upstream
9efb50f4a55621878fb5ecd6addd0ac8b8e29e25 Change OWNERS file
ef87d137a7b9a41e5facec5c4d62b2b879c912c7 Merge pull request #109 from nunnatsa/move-to-ginkgov2
905ff1506faefe59458ffe65fe63d5b04b08e353 Move to ginkgo v2
ab8dc6f953e081120d3effaec8a9a52e60a1ff4a Merge pull request #22 from nunnatsa/auto_sync_upstream_2022-03-09
15507d5f577fe21e49c964a7f6652c627453136b create PR
23f89692875e11f71bef42c7399b956fde2f14d7 add script to sync with upstream
7372603529b2dc7fb16fe15879214f2158d48c8d Automatic sync with upstream
4f88c71024b7675fe453362fd720ee7aa4f107f3 Change OWNERS file
00664282b28fa22e9cf50f8340a3263c08ebef2e Merge pull request #102 from wangxin311/lb
4c6c2377b17b908a08812a96beb00302e1b4c292 change from sleep timer to requeue
6820c0a8d7f5e0701ded758ae6547bce8f213e51 Merge pull request #16 from nunnatsa/sync-script
f160e5f2563017bfae2ad35ba89f3b95e9421f3b create PR
d0ddb839d91ba74907bf84f4371b8e09ed0909af add script to sync with upstream
dbdc825088513dc962ba2103efe2c1a4eb3cf524 Merge pull request #14 from nunnatsa/auto-sync-upstream
51e1a65ae339c8f28041b2b8cd8ccceec18a7219 Automatic sync with upstream
d15f2107e126cdfd89a979fa2259a0bc5a5a4f7e Merge pull request #15 from nunnatsa/os-main
769d670cfd07410b4997f2f18e1a35488b054a93 Change OWNERS file
3cf57f4d26a81b8ef3c2dd0521e8f54f2b05fbc2 Merge pull request #104 from nunnatsa/fix-unit-test
c37c12d85dae07caba5b6d08c00c713753935604 Fix a unit test
e362695668045133074783877baa6b90f8b94887 Update comments for timer
8deb7b9713f3eafa5cc8d53491f05dfa3d4941a3 returen external IP address for loadbalancer
af261492fc33a45a47a9f5ab5b87b96822bc3995 Merge pull request #99 from davidvossel/issue-98
8f4f0163f3b4d478e5d244135966a9c2b2385eb9 Merge pull request #93 from davidvossel/cluster-deletion-race
40fa14ed09916470353cacd1849a4c590fc0d484 Merge pull request #96 from isaacdorfman/issue-84
acfb0625b7218fe8a6b1359d1ed033516255ae5c added github workflow to build and push image
7effa0e109c5d5ff25d7e1b9a6939995e62b90d5 unit test verifies machine deletion works even if bootstrap secret is unknown
e0a3bec278f98617a2abe6a4ab35053ec9f9fc40 Fixes segfault during cluster delete when bootstrap secrets don't exist
c074cfd84127d16613603784dbaf5302217aca05 e2e test that ensure teardown works independently of deletion ordering
261dc35281620ebbd4f4503af4381061f8ef976c unit tests verifying kubevirt machine can be deleted independently of cluster objects
78de9f38ced34d57f593c4f17d72fe2184453465 Infra client is generated from kubevirt machine secret ref when set
70be0d828348c44d9b7742ab7cca4daead248ade Add infra secret ref as an option for kubevirt machines
9b2836499b51b0c49012bdb1b17f980578fbfd01 Merge pull request #81 from isaacdorfman/units-tests
a72d00a7e103627ac863b4c9a7f6521eb0a01baa Added unit tests for kubevirtmachine_controller
86615e2e99b96e5144ed0c2b1d826b44649e47ce extracted kubevirt.machine to an interface and replaced direct call to NewMachine with a MachineFactory interface
ee414f21b1ff80322da2ddf597bfe98f52e34300 Merge pull request #92 from wangxin311/servciecidr
bc06912c626126484f0b3e14610414f761964159 add serivce cidr in template
5f96cf32c9745c72e2d829ff7458dc14db7b1afd Merge pull request #12 from nunnatsa/sync-upstream-2022-2-3
b902ca02cf900361594755cc94bef0370b160a7f Change OWNERS file
167a13af398b141a3fa57956fbc62aef309f2005 Merge pull request #83 from davidvossel/externally-managead-fix
c65f77c2130d943866efb495cdc7eb795f116bc5 Merge pull request #91 from davidvossel/append-owners
e5408bd233d4018cf8432e3bce3ce8719cda8113 Add davidvossel to approvers list
28bd8faa1261b795c7cd496eeaddb9645d8a02da Add workaround for clustercli issue https://github.com/kubernetes-sigs/cluster-api/issues/6051
be3488e8a621e0d5cdcb9aeb52ab205ad9db664e run make sanity
f8aa69806f36340ac79e4eb0021c50723411eea6 Revise e2e test code style to conform to advanced gomega builtins
4ab1f58652bc2478ca0e921850cef7d6c15af1e1 Ensure node provider id is set
77ef2c15eb91a2484e244b49c3f8e460a03a626b E2e test to verify externally managed cluster
90a1197324c473a0d8068ae9eef1c135f8105a54 Add unit test exercising exernal managed clusters
88d9dcde9703c925447e38a05d8dac1bb58489d6 Handle ssh keys properly for externally managed clusters
8d7bb3c3755c0fa68d05fd37abd5c987f7d0cd3a Merge pull request #80 from agradouski/issue/64
bf5d6c66d6e3a4ce4c5b742c7a7b95120c2e5b8c expose cluster load balancer spec and metadata via KubevirtCluster resource
a7f054e9449f13b083d139ef2ac93d1d753beb46 Merge pull request #88 from nunnatsa/goimports
36312a99bfc51674d522e471dae361545155f36b Run goimports as part of the sanity test
7eedfc52b316fd6bca503311e2474f6e4698b889 Merge pull request #87 from nunnatsa/golinter
0658cd929a445e25180a2fc3f9e02f811c92c0ee Add go-linter to the github action
972ba7f9b479a41551fcdbed22ff583d6040b6f5 Merge pull request #86 from rmohr/test
40a075848a69e80ee609e373479521c89c50b883 Quote GOPROXY variable in the Makefile
5475005277175538f26b5cc229ed5ca4f7d507dc Merge pull request #10 from nunnatsa/sync
0087a9e42f91a599c84c4bb3af8b887acf0bfc7f Change OWNERS file
6ec57de19dcaaf4f63649c365627d242d8beb22f Merge pull request #79 from nunnatsa/fix-bug-kv-cluster-race
621bca203d67bbffafe6a5c8c15502ff585bd11b Merge pull request #72 from dgovinndaraju12/controller-unit-tests
5d5edb99e3670233fbe598d73d9a4bafbeddc2f3 Merge pull request #75 from wangxin311/lb
fdb4dbcdba60adfa15c1880e752fc08623275fa6 Fix bug in KubevirtCluster Reconciler - endless reconcile loop with external controller
4819782b3bb31deec61cbf1ce30d3bf101d2c1d5 Merge pull request #77 from kubernetes-sigs/add-approver-rmohr
cb696210f178c749e776b7c6500bc1d7c44c39fc Merge pull request #73 from davidvossel/persistent-vms
70020e2039a4f5ab6cfd18a0ac176d4accd2f616 Add rmohr to the approvers list
4f0ae8d3038055af5a5e79983ba944b59658b060 Merge pull request #69 from agradouski/update-templates
62c12f45087b0bce3c9a08117ff0627bb2bddef5 fix issue #74
f9fbb812c2c0764998cd2578465b1f3354d42478 Add namespace var to templates for VMs hosted on management cluster
0622335f80e8e00a6beba21451312acc5a65c61a Add e2e test validating VMs with persistent storage
14b374493f29735bf8997094fa44bee5cfd205d8 Add template and ci for testing persistent storage vms
600162872db364af86da2de0d4667d39c4e8a69d Unit tests to ensure VM and VMI are treated independently when determining if creation is necessary
dd64540ae30b6f9dda7fac9f4972b152ba703bd4 Should treat VM and VMI independently during reconcile creation flow
947fecbd303a6102eefecba3488bf1783e1cd915 Unit tests to detect when VMI is no longer ready
4778d9718cc8e45b19869a5136347b2620b983f1 Continually reconcile VMIs
86a9cdd7fb378fbe3e842ef0a8bbeacbed30f90a Merge pull request #68 from agradouski/fix-issue-62
b725e10075fada44e0fb2d20c2d73c948fe41026 Add unit test for Kubevirt Cluster Controller
3657f5d7a5910858b19578085b1c563260524655 Merge pull request #71 from rmohr/ok-to-test-fix
5d1ecb640744902d8edf996b797b83ddfd6af94f Run e2e test also on label events
67dad9ed40789f5f473e1a823d59b59a48bdb37b Merge pull request #67 from rmohr/mkpj-fail
9a880287cf4062e60982031dc605e6acc6593e7d update template
bad1ebbabc8f9031569beefe32d25744ef356cbe 0.1.x version of kubevirt provider is compatible with 1.0.x version of cluster-api
be80dcc0e964991c4ed331b0f6d08f97cfc61b77 Merge pull request #66 from davidvossel/e2e-testsuite
b5f7468766a8608887fa0f0c20e55ddfb488432c Add the new --fail-with-job flag to let mkpj fail when the prowjob fails
afa904e42cd32c2f9340cd11d36d9dad09bc546d Add comment and link to issue regarding cluster tear down in e2e test
3d093bf46f4bdec1fc848b549ce4086300a87eee Wire e2e tests to functests.sh script for kubevirt ci
25baf6b2d0dd7f7651bcc0455d655284d3ce2146 Add simple cluster creation test to replace hack/functest.sh script
8284ae47150b1d9f30240bb3992e5064c63ed568 Auto download e2e test dependencies
d58cfc4799ef04e7ff430086c09ac1cc8874720e Adds basic e2e test suite and makefile targets
287d88bfd43c3a3a2f643cc3d5d0a3ba0cb7634f Merge pull request #59 from nunnatsa/add-coverage-file
6f824851c63f8adcd96cf362b1eeb4be0b197b66 Create coverage file on unit test in CI
ef64d5ff1cde84ee41fa4534c24beaf35a30da62 Merge pull request #7 from nunnatsa/sync-with-upstream-2021.12.23
ece741da6ae27dc8b4ffb69bd41e7a9073bc934a Change OWNERS file
6aff381714e8ae9c01e58911b8a4f432e4ec839f Merge pull request #61 from davidvossel/vm-template-api
f84fbce6847b64ec9828455a0235e8a0ed4ecb51 Add unit test to verify creation of VM's in custom namespaces
6067909da7a9fe3419ff9af1502a029f35e22c0c When set, use the VMTemplates namespace when creating the VM
7d0e4162268a15829dd7e35ee6196b67f0f8e600 Unit test that verifys unique dataVolumeTemplates are generated per machine
a18259202212c139776658cdcc26409ce5e566c9 Adjust example templates for new api structure using vm templates
5d3c8a80be691be4642b622ac5b22cf106e7a147 Make DataVolumeTemplate values unique per vm
27a13cd3c20a2ec264bc3601592cd921cc14f11b Adopt usage of VMTemplate within controllers and unit tests
a7d4f69046ace0ba84eb79b6b9bd41a0d3bc9649 Modify KubeVirtMachine to include entire VMTemplate within API
6a2ce8da5bf334ad06bdf03ba7ef0a3509a95d14 Merge pull request #58 from nunnatsa/test-machine-create
fd3f9d2f5ba4248f1e216b221bfde8d009ec96da Merge pull request #57 from nunnatsa/limit-ci-repo
fca933601d88ef0840dd2de98721a1425f71964a Add unit tests for machine.Create
10e4986996010c5102c6b4a2e9a13e799b011d88 Merge pull request #5 from nunnatsa/sync-with-upstream-2021.12.22
09bac6c690338b1b0ab9d80c909ab7ae2ec5fb2c Change OWNERS file
a0804dfeba174f8ce3dcf0dd0ef75a85ba5240c0 Merge pull request #50 from nirarg/versions-changes
3e08364719e69a49432d801d38f38a0137fd4ae7 Merge pull request #4 from nunnatsa/sync-with-upstream-2021.12.21
b093f7feb9991f018b7d7b0529bfaeefcdaadfbf Change OWNERS file
e07656cbe235aa1ad564117ab32fe9b4321da3da Limit github action to run only on the kubernetes-sigs/cluster-api-provider-kubevirt repository
d967dc4206f1606d38ced91775b625547fd91b2b Merge pull request #3 from nunnatsa/sync-with-upstream-2021.12.20
64686630542bbd704b809083dd5578315c99f816 Versions change: "make generate" results
0849c35dd226b1b1f8e8ca6678f8821ca3f05dff Versions change: Go modules changes
15c9f57466301b6c115c382c1c4df64f66bd0126 Versions change: Change Go version to 1.17
d2f65fae96b9b005cba659bf778b327eadf3f02b Versions change: Change cluster-api version from v1alpha4 to v1beta1
353694f61daecb3e4c4ea78d13477a2fc209a4a5 Merge pull request #54 from nirarg/decrease_version_v1alpha1
f390ca9f6b333719bee472088e6bc32786ee7670 Change OWNERS file
5328dad7e4215d01a298aa80026054fcd0979e7a Versions change: Change api version to v1alpha1
5dfba0edea2d6b82e4904b988156372d2c32fc03 Merge pull request #39 from agradouski/main
64bf9b76931ce9ced10513c9ed60b625e599bfbd fix unit tests
6886064e2dbcdb7eab843c8929b6387696c443b3 Merge pull request #52 from aaseem/main
5a942450cbd62126f14f5305847f0b08eedbc61c Merge pull request #53 from rmohr/integration-tests-no-external-golang
eecf38e4b4ad08cc99d94aa3219f1122dd053ce6 Merge branch 'main' into main
236502285738ac7c35edc71e621cadc4351adac7 rebase
0d74fd553fa8a713bb7f117167521ffec6592f4a Give github actions better names
abb3433806071c856df7de172f2e6c8f53ef0d5e Make integration tests independent of go version changes
ed6b197f2bcf76d3d3a9c514d15ecbc120ae0a87 Update README.md
807b26c9b263595f6e008bb28f5452525e77aa4b Merge branch 'kubernetes-sigs:main' into main
2b9a3bd003372d31bc7985bd85f7f2a6dbcc670a Merge pull request #44 from davidvossel/reconcile-tests-1
9cd5367da74ad8734167c957f44c22dc28c33eb4 Change OWNERS file
327d1591d88d4c459eaf91fa4f974878fd8fc11f Merge pull request #46 from cchengleo/update-dockerfile
2a371d4a1e32a5fba95dcc2d3f8c2e802e1dad83 remove race condition when searching for vmi immediately after vm creation
cf2189f576478d1593c50555e45efd1c93944d0d kubevirt machine reconcile normal unit tests
09129f5ed770d647d8eee7deabad149dbc77da17 Merge pull request #49 from rmohr/make-secrets-available
37a448ccf50474f34523d12db3505755588da35d Make secrets for third-party PRs available
55619c9c9f9ee2ed59267c77d548b1f2dc79718d Merge pull request #48 from PranshuSrivastava/meeting
7ebd2f570412d439bbe6e0ba9a4115aa8ed9d027 added meeting info to the README
0c46a6b0bcfe23437783475bb0efdf673a5aea4a Merge pull request #38 from rmohr/testing
c1b56692aa82cf08428d86caa56904cdd8caac3f Add dockfile to build manager binary and emit production image
defb61bb69f244102cfb91213e9f386d0f39f82a Merge pull request #43 from TheAbhishekS/abhishek1
75bebc45f6d7125c3ace195943e01fd1c33f6d43 Update README.md
2b5ff01c6dc619a53003cd97d5f1440a68b53b09 Merge pull request #30 from davidvossel/cloud-init-fix
74fe54cfb4abfc2be449cc70b61cb25768d43739 Support for external infra clusters:
9ab2197a3926f0d381ccc7071b4137828dcff2a3 Change IsBooted to IsReady in order to better reflect what is being checked
2f4bd065111c0926bd58588e891329e03db2d5f9 Meeting details updated
fc65a8ce3a5817c09216a7f2a8af4e4c35f2abe8 Update README.md
67148ad6f06593123ceb4e5b8485615e537e9a97 Support for external infra clusters:
bf8fd23ba6f4c68da0c39c591ab2cc3a8460d19b Add e2e test lane
13a7315a048ed88bd5495b99ff97b868cda0a525 Build and test the code with github actions
a1686998739c30e01c7aac915363136d5cce6e34 Add unit test for detecting cloud-config user data type
64dda53a76239931198fba44696b3db3801e4004 Add unit tests for determining if boostrap detection is possible
fc8a193f538ed9a3252f4219641d64472e5847a2 Ensure that bootstrap exec condition is set during functional test
b3d1a9afb150d4fb8d7dd601e8949ff692a489bb Removes spec.Bootstrapped in favor of conditions
0da77153301d8875d6144d971ac5eac708e01164 Update machine unit test to require ready condition for detecting is booted
05ca8dc438bfebe7f23c547e65829a825d6fda57 Only inject ssh keys when cloud-config user data is used
6870e0a501db5597b9fa24660ce9decc4d614617 Merge pull request #28 from sayantani11/Readme
4967b397a610b96cb2ce76af14a4396775f0fe38 Merge pull request #21 from nirarg/fix-node-patch
623549ac9bafbca8fcd302567a8f251f65162b02 Improvement of Readme
bf15d9a78e19115f08a071766403b6ee8db09849 'make generate' changes
fd66b90336d3965ea0d86ff6a39fe9502d9eb90b Add unit test for new patch Node function
3b649595a8133ab355c93cb6ce20351945fd35ec Move WorkloadClient creation to its own package
9acb475e01dfd6603658d602aea2be5a8b1dfa83 KubevirtMachine Addresses: Wait until IPAddress is valid in the vmi
3cbe30fe2428b3b0b56f0647b73127a4c17f6444 Change patch node not to block kubevirtMachine status ready
4dbc3a3e3713dedff8c4960b2d17ce41919b6520 KubevirtMachine Addresses: Add MachineInternalDNS Address
d9c840ae569a8780f4bece5df9709055aea3dd03 Merge pull request #27 from rmohr/ssh-test-fix
b910e6d32259cb3a5ae9ad107a0b5a102359d537 Merge pull request #24 from davidvossel/backport-changeset-1
708cc28e5414a408ec6486035efac866a330ab99 Remove non-existing make target from the "all" target
9e90933e53f287d0e095da41c3f054c7f3f41abd Fix an import error in the ssh unit tests
d868226fd6a981e32f825fb224f64faa834c09f8 Add new kustomize layer for kubevirtci
7f426613ef6409afb8eb751cdca8923975d68d3d Add minimal funtest make target
fade7c3009853f7727a5e3f6e921ab83b700841f Merge pull request #15 from dgovinndaraju12/unit-test-1
ebfa9a0f93cb02a82a65eaea2cda392fde4083a9 picked the right commit
3a90904507aa8512294f0596164889fa250bdccc update go.sum
f37ec65cd8feeacf48315bcda3c743cfd690b861 Add a basic verification script for e2e testing
faec1f5a9c537e28b6a68915adfc009defa87c61 Add kubevirtci refresh command for cycling capk controller
78efdae18dbc2e7845dcfa967229c7159896b924 Use kubevirtci quay.io image
1d5b73145e4537f01a078c72ae4a5dbbd17ced8d make CRI runtime a variable for cluster template
af8060038eaef5b47e2d848eeffe1c8a0b2b9b81 Add custom clusterctl path to kubevirtci helper
3e3fc389165dce71485bbe61a0abab303e8f755c Make sync work on fresh installs
599589b9124fa714337c132df1b6783d1696b742 Add development environmet and e2e testing script
6a2e8ab43a8fada35c890429ba1e8715ea908f61 Run make generate to generate missing functions
14d1ef5f3ecb5d78f7514f42156d5bdf13e99493 Add a minimal Dockerfile
98d36fc0c8d03cac3fe2e6422d71e9e98d0c73c2 Slightly adjust the kustomize manifests
1998fa05ff520137fad25db879cf64569ca7f0af Fix complaint about wrong import paths
f8b1df85744131efd017e5e07806e88e9ffd5297 Merge pull request #20 from rmohr/crypto-update-k8s-sig
8c217a7fb5f11d8cc09bd56e5b48aacbca452120 Merge pull request #17 from nirarg/kubevirt-client-modules
b2c8cb21080cb18b9a0c920564c657f2ca2df005 Switch from RSA to EC keys for ssh connections
f8883807e606fe45e61da1fb5bf5a6d244fda5e7 Bump golang crypto library for better ssh protocol negotiations
d0c586cd52d0eecc2b5e37b72372fde6c452e354 'go mod tidy' changes
2cc0ef879daece15cdedcbdcb9ca2a2c5a69137a kubevirt-client: Change use 'kubevirt.io/api' instead of 'kubevirt.io/client-go'
b230e85e1e6afdd3940d820eed8e6813c84729a5 Add unit test for cluster_node_ssh_keys Signed-off-by: Divya Govindaraju <dgovindaraju@apple.com>
83c693883aa96d7e1822b8d25166cdc6ffa5fdae Merge pull request #12 from nirarg/manager-namespace
132eae75488e85ba71ce8343e4cc1ebbb04bf0f0 Add namespace option to manager start
b2596562416cc548ce9775a203e42344fa5d46ec Merge pull request #10 from cchengleo/MIGRATE/clusterctl-setting-metadata
76197b5a716e992a52fbee77cf4a3a45da83469c Merge pull request #9 from agradouski/init-commit-makefile
375fd6876a7e210f62b768ffa0fb895ec9caec5a Merge pull request #8 from agradouski/init-commit-main
f76ed1c9012dc5506975ca8d236510934f68acf5 Merge pull request #7 from agradouski/init-commit-controllers
c8d39cc66b4ef7f4b4f2803adb75436814e9d552 Merge pull request #6 from cchengleo/MIGRATE/utils-packages-machine-controller
202a15be10227155de26feea80c48b179f8caa25 The initial code migration for cluster-api-provider-kubevirt by Apple Inc. (#5)
08c87ea9e2c23172e5ad9014f1fd25993ccc4b62 The initial code migration for cluster-api-provider-kubevirt by Apple Inc. (#4)
311f015a6547bec71e29a8adb8daac77a65d3197 The initial code migration for cluster-api-provider-kubevirt by Apple Inc. (#3)
0ab30515b3df49681bd2b65b38efd3e96f1fc39f The initial code migration for cluster-api-provider-kubevirt by Apple Inc.
0880ecbc9d6bc9ad8b92a7f1f0730b91212487f4 The initial code migration for cluster-api-provider-kubevirt by Apple Inc.
6ebd07dba2ec0d5d3c76f2a6cde963fd81d68776 The initial code migration for cluster-api-provider-kubevirt by Apple Inc.
fba3b2e25eea87cf5066d256aa53407f94477ce5 The initial code migration for cluster-api-provider-kubevirt by Apple Inc.
ec0ede9805ab56f059d2893d24a20bf4d0ff3c14 The initial code migration for cluster-api-provider-kubevirt by Apple Inc.
d6389182d7c06da9b4a9c01a6c3cfb27eae3de5c Add .github templates (#2)
8521df9b21568c7b834f59b4d688a697c285e953 Update OWNERS, OWNERS_ALIASES and SECURITY_CONTACTS
db321f7fb629f19e3c917060183dcab53880ccf4 Initial commit
```

Status: Syncing successful
