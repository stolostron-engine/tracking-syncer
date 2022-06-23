## Syncing openshift/hypershift with stolostron-engine/tracking-openshift-hypershift

## Status Summary:

release-4.10 -> backplane-2.0: Picked up 1977 new commits.  

### Branch release-4.10 -> backplane-2.0:

New commits:

```
3847d161e8ce06b787017a5c24ad967d61137822 Merge pull request #1475 from hasueki/cp-pr-1304-4.10
7f89c6824fa637b6e8a72b9355b7ce45a68731d5 Ensure that everything uses imagePullPolicy IfNotPResent for resiliency
2b2ea3b54dde93c12d7a5746691432b8ce0962a7 ensure imagePullPolicies are IfNotPresent for better tolerance of networking outages
c2864b6c080c9e45cfc020929e851c4fc4984a4b Merge pull request #1461 from openshift-cherrypick-robot/cherry-pick-1460-to-release-4.10
ccd42a9e1b69f28f542481077e405d5f2e7eec70 Ensure cache is set during token rotation before reconciling
1db3a63c75e98bc95072cc99107a4b50bd7a7cb2 Merge pull request #1416 from openshift-cherrypick-robot/cherry-pick-1388-to-release-4.10
a7f35112ab7274624636e075ab75393ff7869268 fix(cpo): set tls cipher suites flags on kcm and scheduler
dbad583d854c22c6b161ac9cc2cb045cf02043fc Merge pull request #1410 from openshift-cherrypick-robot/cherry-pick-1322-to-release-4.10
7c7b9daceca1ab7bcd264c3dfc426e3b04010fc7 feat(cpo): adhere to upgrade order from kube version skew policy
1beed181eb15e1c1508b191fbf9cdacc512762b0 Merge pull request #1387 from openshift-cherrypick-robot/cherry-pick-1365-to-release-4.10
a65c56190e0d8abfb313c1440ff6710517ab5eb1 Update config.go
6e66f15af86b40a5e88e8e55143366feca913af6 Merge pull request #1378 from openshift-cherrypick-robot/cherry-pick-1349-to-release-4.10
a147a17b47c61b1d605fc1ae1fa3b2ad1656696d fix(cpo): Scope down secrets access for olm collect profiles cj
330617fef79a7494308b437573fd8ebb7efcb865 Merge pull request #1361 from openshift-cherrypick-robot/cherry-pick-1350-to-release-4.10
69f82526f4494d53c4121c05d811f580becf9a2f move to ga apis for all components now that management clusters at minimum release boundary
1118d766068e6a1d6cf36d64bad35c4db6d699a1 Merge pull request #1359 from openshift-cherrypick-robot/cherry-pick-1357-to-release-4.10
9909e92896c80a93a90cd03a546cc7b965844d5f configure cipher suites to prevent using medium strength ssl ciphers
0b12697f1e0333f99c62238db21c110a095fda0e Merge pull request #1333 from openshift-cherrypick-robot/cherry-pick-1319-to-release-4.10
c03a2f6f020920d41de3d0de016069d99fcf58a5 Use apiserver host/port from InfraStatus in reconciling Kube API Server
085bc8565ede48776f921f932576a550f06b9dd5 Merge pull request #1317 from openshift-cherrypick-robot/cherry-pick-1312-to-release-4.10
25ead48bef082b0ed1fdbb592fefa7de40e4000e Ignition server: Actually use workdir
820f413dae1a29e46c2bfc69f05da4325637e16e Merge pull request #1311 from ironcladlou/ign-refactor-410
d60f5849b6e107b961def42cda61de8e395de057 Merge pull request #1309 from openshift-cherrypick-robot/cherry-pick-1305-to-release-4.10
7712095e0cdde035fff3fbb483338bd7c51b4c27 Use forked processes instead of pods to generate ignition payload
8f84c508f9ea658de95ded6cc27a5e8f09f307d6 disable reconcile of registry config in IBMCloud deployments
d0ada577709afe4f70d4105185a13739a37a1938 Merge pull request #1289 from openshift-cherrypick-robot/cherry-pick-1287-to-release-4.10
1c95287c49686bd30c131e1f7f845357e129b677 feat(cpo): Disable PodSecurity for 4.10
0522fa44ab30e18e04f59008a45c964ed52b0b8e Merge pull request #1286 from openshift-cherrypick-robot/cherry-pick-1243-to-release-4.10
28c428a5566f26e7de5f7c33f265600497d678ce Disable PodSecurity admission in 4.11 as it breaks conformance
1967de8f7854d205c0bf8e5b521f66f712dd92f9 Merge pull request #1265 from openshift-cherrypick-robot/cherry-pick-1259-to-release-4.10
00c02177ccc4707cf3f992664732e5aca93a92ba Expose a service account signing key in the API
f3e0ada7a5e9bd6f8219b1141c115bc933f00291 Merge pull request #1252 from csrwng/route_fix_410
8f55e7cbe3b24010ac7446db207b8a64686eaa95 Enforce hostedcluster service route immutability constraints
ff937ab84d6ca21e8ff323af22e620999b8d9285 Create valid route names with long namespace names
c6ce37a46f61aa3b639c9c6ef4aeb2947046d5b4 Merge pull request #1233 from alvaroaleman/ff4
f63e3b74609967d9f290e5a780fdcfc2236ff598 Merge branch 'main' into ff4
c729c427274617986c451c0b78b0f900a4f851c1 Merge pull request #1231 from ironcladlou/disable-uwm
ba2ce8d3affd4f746fc3923d14dda371ab14643e Merge pull request #1226 from alvaroaleman/priority-class
ba6b9c2423112fec0f30537d8230adde8a51fc57 Merge pull request #1230 from ironcladlou/none-flake-fix
9ed6c336213c8c21e9f73165615259229fcdf94d Merge pull request #1229 from alvaroaleman/prio
334489067a9a5bcba6cf9e90166e4835af095f7d e2e: Don't enable user workload monitoring on management clusters
c49ee9edc13d266bd8e51a96353270aa45567fcb Hypershift operator: Give a priority that is higher than any controlplane component
c430b2565eacb119b2186e4734564960d89761e0 e2e: Don't fail test on transient recoverable API lookup
337698c921070731bfe9318b834f5df9b7d2f900 Merge pull request #1090 from enxebre/images
3c027a8311b0ee0b636b9e344a7e6867c43ca786 Fix priority class for olm cronjob and verify priorityclasses in e2e
5598e5ceb71bddd5725180f230ae3da9f7cdbf30 Merge pull request #1213 from davidvossel/doc-kubevirt-ingress-v1
2d3945f6779a0eacbf06a859a94fcbd2348375f2 Document KubeVirt Platform Ingress/DNS options
3a3504644cbc72c1faa559d388e8c42f894420b6 Merge pull request #1218 from davidvossel/vm-default-affinity-v1
9706cfc7e9284c7abe9d8aa1fd2f1c0d9924fd53 Merge pull request #1219 from ironcladlou/tagging-retries
9d35cf86468c996c9df013529fbeecec7819bcae Retry EIP tagging failures during infra creation
d505b9ea1ae1827cba6c3ed10995f0583c4eb37e default AntiAffinity rules to spread KubeVirt VMs across mgmt nodes
f36feb4620747e475f7807463aae199ccac00a9b Merge pull request #1217 from alvaroaleman/fix-4.11
2810e6e221f9c5d9271f07a9817c5522a34b3d97 Fix CPO to work with 4.11
cd441b82623e97ed909566e7076a316590cf33b2 Merge pull request #1215 from Basavaraju-G/apiserver-image-from-payload
da5972ca6f3509faae2f89ccba0b0b42a1cec82c Update to referencing 4.10 disks and documentation for KV guide
59f52f812f985b25f2f7f0aea62d80690363e19a read apiserver-network-proxy image from ocp payload
b9418cb392b94bc6682c76ce21b5dfd2744b9e8c Merge pull request #972 from hardys/additional_trust_bundle
32f8fc49348f07f388d3b2aa453cd2aab1beb12f Merge pull request #1208 from sjenning/dns-docs
799822b2d34bd73ee905fc606e04c31e1c492b7b docs for DNS indirection
a4fdbc50d50cfc5e9fcbf53acd3a44d31381e3bd Merge pull request #1212 from ironcladlou/docs-build-fix
9251dd99978f2c63d8d60ad539d073509c67c13e Get autoscaler/machine-approver images from the payload
7f4d2366f8d61201be7b0bed8744611b4e86bcea docs: Upgrade mkdocs/material to fix Netlify breakages
1b39da183aa03e807fdda9806e42b16324abb17b Merge pull request #1204 from alvaroaleman/dump-archive
276f01c3c6d321a5aff2580884ddaa3b216f820e Merge pull request #1207 from alvaroaleman/upgrade-staticheck
7b735b890cd631f0a5221504e3081b8f5b52601c Merge pull request #1206 from davidvossel/kubevirt-vxlanports-v1
e43d7b4f2e2db3a40fdc0fda1fc0b14842838ad0 Merge pull request #1202 from csrwng/fix-registry-config
35f8381d25be3a6fa02b41da6529b16355b644da Add default vxlan port for kubevirt clusters
386a79164d358b112bdc93695bfc4c0db3ce572c Update staticcheck to a version that works with go 1.18
1f86391969ad83fff0a25a92b6e4271b28b0799e Dump: Always create an archive
f61b3fa278e23139420867fcd103652a9ff8beb5 Registry configuration: reconcile only what we need to changes
8fd5d43d7087e167557a125031f33b083a167c13 Add install additional-trust-bundle CLI
5626d38f9b2354e200db3fb767a2a4e4f6555ec9 Add trust bundle to hosted-cluster-config-operator
cdfc64bdd0151ad4fe03b881dd3f0f05e152b4fb Add trust bundle volumes to hostedcluster_controller
0dd4049ed85237fba892cf90b7c6984d17f5958b Add create cli option for additional-trust-bundle
55c08f80338048892fb48e0d0256a395aa53fb7d Add AdditionalTrustBundle to MCS bootstrap params
12773d4e587f2bb1f2d2f96eed2d280fa886f1fa Create HostedCluster user-ca-bundle configmap
40d4dbc466be320fee95d62fb0fc2a6c382cbbbc Copy HostedCluster additionalTrustBundle to HostedControlPlane
09dfcbb730b295148222304c86322cca469b2952 Add additionalTrustBundle to HostedCluster API
339bea987f99c6007e7c8f1c92ffb9c6ba92a7fa Merge pull request #1198 from sjenning/dns-enable-registry
82dcf2195d218eee4f611e53638ebfc6cfb29472 Merge pull request #1199 from sjenning/sync-worker-count
f3e420e93843d5a9a8296d2e2458b8c185b8334b Merge pull request #1163 from sjenning/dns-e2e
e506d367409e87a929c755135ca6d021ed939a59 Merge pull request #1200 from alvaroaleman/fix
3f84cd07e182da1ae354652424eea567cb4070b7 increase MaxConcurrentReconciles on AWS PrivateLink controllers
13d71738070731a63bb55e96d58dec98cb4cca73 KAS: Set proxy, but exempt pod and service CIDR
3bb8c5359965429d091ae72f47780cb827dc8b2c Merge pull request #1192 from alvaroaleman/fix-logging
32fb19153f95af92d19eb37129aa3ac497bca0db enable external-dns registry
85affa2fcf7b840c67f2c6736cfd3aee58288fff Merge pull request #1190 from alvaroaleman/ff-2
cea1fc8657092c3cc361c6f154eb2f394a3d4164 Merge branch 'main' into ff-2
bf6d41f367c955d75c27dfe89ccf702adcd6b6d4 Merge pull request #1195 from sjenning/revert-1167
5e71fedfa396d3267d2cbb8ca4117062d0eec9ae Revert "PKI: Use ECDSA keys by default"
6edb0bb910544ff8d0b0b7c9749e4d8121ca9d18 Merge pull request #1193 from sjenning/add-olm-hcco-require-apis
72cbf3d1c22f5f410e0a010aed097d189fbbde5b add required-api to availablity prober for OLM and HCCO
0a1aeb56a8dbf37d6cb919e786d0024a5dfcbe56 Merge pull request #1184 from enxebre/paused-reconcile
c356b8b72d66db98789717689803dcbc3df18054 Merge pull request #1191 from ironcladlou/ko-fix
87bfc950c87a2301901f2d9dc4cd859df6ea80bd HO: Don't report NotFund for hostedcluster as error
912f900fc1c656b0234a45956613fb2d0d635cea Fix `ko` entries and update ignition-server dev docs
d9885b8f4e577ae6f71f23ea0087141a2dc753d0 Merge branch 'main' into ff-2
0d38480f41c0fa35cc13a9eb492277a3f488d990 Merge pull request #1169 from alvaroaleman/converge-utilities
9f11c9ec02216151d7a7a04a4520e644e0e19ba0 Merge pull request #1187 from alvaroaleman/proxy-apiserver
feb0c99be4546dddcb665a462ace070087a47f55 Merge pull request #1188 from sjenning/fix-external-dns-fixture
7b5e1b0e4c0093698562d07e7366fa7ef3dc3902 Trigger reconcile when paused time is up
e8cbf5185e2fbd3516d82ced433ac7c81d1498b7 fix AWS HostedCluster fixture to set hostname in alignment with endpointAccess
de937192e8d2ca0d46072708c0d29d846a291cc7 Delete Cluster API Cluster Role binding (#1143)
e787444e94630a29c01c528146d664da186dd2cf KAS: Never set proxy
1b0164e5ad384a99e208f48b16ce8e68354e207a Merge pull request #1186 from csrwng/patch-status
e401c098c5b314921c2913f9da2d05408e95daad Use patch instead of update when updating HCP status and finalizers
7d5d1ee01dd29e6fc6393edb066637d34c31ee75 Merge pull request #1180 from ironcladlou/oidc-condition
8242a4bfbb1eaf30739ac78c245d419f6113e9c8 Merge pull request #1183 from sjenning/adjust-budget
64494682f2bf9ecc04f0cfee6a494d36a65e7eb5 Introduce `OIDCConfigurationInvalid` condition for OIDC setup validation
d494314d31c752c84ada617fd7502731fa3daf69 Merge pull request #1185 from sjenning/olm-delay-live-probe
eeab49e4ea1d86ecb1a5e66b52bb40f9c0ff9e83 add required-api to availability check in olm components
3c773bca2ad29a081f7fab160feeeff483378aee set initialDelaySeconds to 60s on olm operators
fe045fd56f45102333417749ad332fab2141f284 Merge pull request #1178 from alvaroaleman/ff
4879310b1ef30b4e393e17cf4231c74c26b4c77b Converge helper binaries and ignitions-server into CPO binary
b86b2668ef5e93941f76e93b6acb3834fe6a8661 e2e: adjust budgets
c7fe2eee5165a46a26eb2ace0e08099810812352 Merge branch 'main' into ff
c2992b9b250cdb7e870f127aac218edf4f3f3b2f Merge pull request #1179 from csrwng/optional_cluster_id
9394f6ae9e299acc24e131e0c727f57045b64f5c Merge pull request #1181 from alvaroaleman/increase-worker
48d0080cd2a1da72c76afaeeeac49becbabaadc0 Hypershift-operator: Increase worker count
3ff160464dc0070390806d3cf1e7d4a53a66d2c9 Make clusterID optional in HostedControlPlane clusterID
cba874144c0a04dde863284ecf4dd5ece4713182 Merge pull request #1151 from csrwng/cluster_id
a0be78d4252affff636325c21bc547d6032e3c4a Add ClusterID to HostedCluster API
255072ce26ff1326c9293e27e04578718ae6a77e Merge pull request #1162 from eranco74/MGMT-9591
bfe7b2ac2bb0f7a506b2faaca33398876aa399f1 Alow hypershift operator to grant RBAC permissions for clusterdeployments and agentClusterInstalls to the cpai-provider-agent
7d8ce65ead182da116f39d558366511a71b0baae Remove CAPI-provider-agent ClusterRole from hypershift Agent platform
7fbf0adf74c8edc2117b4e4389ac6c1947837e2a Merge pull request #1174 from rtheis/pause-reconciliation-fix
3c3c4e15ef3b46a755cd3543f82c7ed920e18e95 Fix typo in how to pause reconciliation doc
a9a5d7d45444f8f81a24f122455b00116d3e6caa Merge pull request #1173 from csrwng/update_410_0318
7217f78ca82f85a48807356befa93298082b7027 Merge branch 'main' into release-4.10
5687bf65aee099a5f34929cb166897508ab7de3d Merge pull request #1172 from csrwng/add_pull_secret
2ef62b6fa7b2c900aae2cf03f3958b0c810a4968 Merge pull request #1167 from alvaroaleman/ed25519
7e1dcf5ac49f412375e346c59b9b5c3038126429 Merge pull request #1165 from ironcladlou/ko-fix
e9fe0d67a3d261ed2aa608fa44e9bd6781ac021c Merge pull request #1171 from sjenning/combine-hypershift-install-targets
ebca35e12216df0f0fc23575aa247bbd8ad25f4c Merge pull request #1166 from alvaroaleman/unitests
5bf830b2aebdaa5c58486813983a7b1249b22369 Ensure that all control plane pods use the cluster's pull secret
66536e86498c6ae715fae37e4515b83c56edfa12 Merge pull request #1170 from alvaroaleman/dump-node
9aca9303850db0b3fafa7c797b20b6a26f3c3d98 unify hypershift install make targets
2a59e6c6c6b69b16d849292de19fee7277e0321f Dump: Dump guest cluster nodes
0551cb0da61d7a79f9f51a40f569909cfd559598 Merge pull request #1157 from alvaroaleman/proxy2
464b572bcc53ccdc7d2d44cc2172adca6cac7204 PKI: Use ECDSA keys by default
e0586f26bd6a698ed9bca3c496f38045757552f0 Add proxy support
56545494ba65ed7298c7520bf6c2ef04a7515525 Merge pull request #1168 from alvaroaleman/resources-test
58b0baa215ef151b0b83fb0d7166528b8c95a02b Merge pull request #1164 from relyt0925/use-cpo-for-controlplane
9ad97e10b157637a19047e2eeaab9cb3f141330a Merge pull request #1154 from relyt0925/add-clusterid-label
f5cd0f0c9dfe1a96770203b36bcb4f7c7f4963ed Resources: Improve runtime of test
35aa7ea0f7242a007a5cecbccef624416fa0cc4c Run unitests with racedetector and -count=25 to detect flakes
882b5e46684d86b0ba40a131613666e4b33ec499 Merge pull request #1161 from csrwng/fix_ut_flake
fbd327b3bf58b9d18113ad13df4787174ebe9dfb dev: specify a more useful `ko` base image
e78e09aeac38b3df56690e4ac3bc4e348f93892a     ensure token minter, socks proxy, and availablity prober are versioned with the control plane operator to prevent large scale restarts on hypershift operator upgrades for IBM Cloud
325c5a1693022bd32040d48f15abab08e0b855d3 add external-dns flags to CI install make target
b0dcc9a11a2285f98a7182a795edbd448b4e87ea Merge pull request #1150 from davidvossel/kubevirt-nodeport-ingress
7b4b22d1834a9cfb62193507697f5df9e2ce6456 Merge pull request #1160 from csrwng/update_410_0317
4b0637f8f6339fa503bb3f6760eafa19284a405f Fix events message unit test flake
64b8dae31db4596bf416126441e2b69dbfb2c706 Merge branch 'main' into release-4.10
279233add42c14b24af50c3a2dfa3c730ca92a20 Merge pull request #1149 from sjenning/dns-e2e
d7828261f5572b2f491cc657886c7a04e950ddfe e2e: support dns indirection
44844971bf109f9814b035d0683b98eb58364e6e copy labels from HostedCluster to admin kubeconfig secret
28741c07eba6a79417333b2f57d526020248d07e Merge pull request #1135 from csrwng/surface_status
67316dbb8a3552523ce3783740ff678f1033e828 Surface cloud error conditions for HostedCluster resources
a004e930737d921b9aa463a092fbf7bba6965824 fixup api docs and nits
eb89a6ce1c655d3eba0b80a2884198c7488505fb Merge pull request #1139 from hasueki/olm-catalog-placement
5d3f08b6b95601d2cf72956695273baf8fdc5343 Merge pull request #1155 from csrwng/image-refs
012eb206c5244efccde28f1f9f0663995a7fc610 Merge pull request #1148 from alvaroaleman/forward
478be4ff54b589b753b393282446f8109974485a feat(cpo): Support OLM catalog placement
c61331fa8b5bf0062b3e7e32cc2ee90e9e575a4b Allow overriding images at the hypershift operator level
29dd02eafb26bad15406c14f8bfbdcea11a236c5 Merge pull request #1153 from eranco74/MGMT-9633
bfb2f9bc391abaea897d929066be451eb988064c Remove the role allowing capi-provider-agent to list agents on another namespace from hypershift management Create the role during cluster create agent instead
417c9e859f55968380ca7e0653d7a495c90c7272 Merge pull request #1147 from enxebre/restructure-how-to-docs
2ef77aa626ca85a9d0a0652a3211b876c44f5359 Merge pull request #1152 from eranco74/agent_RBAC
fc6849ed671af40ab512610d97ccf12072b3f80f Alow hypershift operator to grant RBAC permissions to the cpai-provider-agent Note that this role should be removed upon removal of the role in the agent namespace from hypershift management
86bc7faaa1591a79c3fd034a6c58fab701279387 Enhance Kubevirt e2e test to ensure HostedCluster completes install
854919d1066118d879fe74f6566e8470d2a69ef2 Enable wildcard routes for OCP cluster when CNV tests are being run
721d3b14c08ac30eee55c827fb985c9a0b9ae42a Default to using empty dir storage for registry with kubevirt platform
d92a06f2df5d8ad77e7e13dce85e09196e60caa5 Kubevirt Platform: Make HosteControlPlane be aware to KubeVirt platform
cdcf799215cc415d4fa097df867547878d657a5a Use NodePort for Kubevirt's default ingress
73646179df2ef9005a0ee21a5f8a7c181f45c84e Merge pull request #1145 from sjenning/external-dns
b1c1ac1525b7305d852496c646daf9039a8d519b Merge remote-tracking branch 'origin/main' into forward
9b646db35bb5a4c6dd455512406d8c1bccf8e0d6 Restructure how-to docs to categorise per platform
7e763f8b89cbc38ecc8c2eb77f10eb9b9662624b enable DNS indirection to control plane endpoints
67c39df9018db1c74d761945bebacddbecec0148 Merge pull request #1138 from avishayt/avishay/MGMT-9399
1bf112960e25989a9c1c262ebab807550092daec Merge pull request #1137 from eranco74/agent_role_binding
a282fd5586beee2773aa0a65f50a196e8d1e2286 Merge pull request #1079 from e-minguez/baremetal-hypershift
8e98513d1587e7a907c360dda832628d0d8831ec Merge pull request #1136 from relyt0925/priv-escalation-fix
f4323b7e701108313b85e10ed96ab1300e85da6f Validate that agent namespace exists
0a494bbf60122839e280cb2eab2127086f2959d1 prevent privilege esclation by explicitly not allowing the escalate and bind verbs with rbac on the control plane operator
65fb827fb8f697d088da1e94891dffa2d6e1e285 Merge pull request #1142 from alvaroaleman/konnektivity-agent-host
596f64355874c8aa6248e15e71746c65f81b47b9 Run the konnektivity agent DS with hostnetwork
835549cbc295e4fc33e9c34419a5c96afe86d320 Merge pull request #1141 from alvaroaleman/fix-image
f9291373afff6e7e83025089175115bff70c215e Azure: Fix image name to match what HPO expects
0644b16e86cb1b544c3eac044a5a9299b1fd8b9e Merge pull request #1140 from enxebre/rename-variable
4929b1b528cd669568d7605d42f4a7e4450cb1c8 Rename variable for machineconfig and pretty print message
87e7b7fa4b92c3796d647be62b13ba4d4fdb69cf Agent: each hostedcluster provider should have it's own role binding Cleanup provider RBAC upon HC deletion
9fd6e1d072961734bee491b898660fa81a15dfdd Merge pull request #1131 from relyt0925/ingress-operator-konnectivity-sidecar
c5b082708863ba6cc8058364cee9af92f7e22487 Merge pull request #1127 from alvaroaleman/multi-az
4f19ace4c44085b669e1e08693aca21153b67511 Merge pull request #1120 from alvaroaleman/log-retry
28546dc587dc028dc8bded715847346ff99d65ea add konnectivity proxy sidecar to ingress-operator to ensure it can properly perform in cluster canary healthchecks
98f299831f93e7d65240c23812315d3b874264d0 Merge pull request #1133 from alvaroaleman/workaround
167727d5ee50f04e6924a6dd6bec08a70a31f539 Azure: Use an apiserver port that ends with 443 to make conformance tests happy
bdf04d7d51017e6265f1e17332253d2f0b4e71d3 Merge pull request #1132 from rmohr/add-pull-secret-to-control-plane-operator
37c058b09136c69aca328daf2f6cf2ab9c15324e Documented howto BM agent/none
460b71e199fd754028365f5ee7d6c2220ea32a44 Azure: Add multi-AZ support
f29e5dfe76bae7f96d4bff6f904ca5860042acef Give control-plane-operator access to the pull secret
4ebc7e1217f3da6e000d4fef2dac45ee34e7ffb3 Merge pull request #1129 from relyt0925/https-prefix
ca740f980c6fdf18f2cd1cd6319404a94223b0c0 add https prefix for proper redirects
3af3c625b01c7c18b03d526760d891e6ab844e39 Merge pull request #1128 from alvaroaleman/re-add-install
1c654e502744f43529f47b50d1b3548ae5bc8619 Merge pull request #1123 from relyt0925/fix-dns
20d7125a89f0a275064359b601346282bb192fe5 Move oidc configmap management back into install command
cad2fc1cccc70cc44d4a08659a15d62927a1010b Merge pull request #1118 from alvaroaleman/fix-nodepool-create
02f3c5fe1862d58e74aa13b33e95d937f519538c Merge pull request #1126 from alvaroaleman/fix-log
6887ebda428ffc6426461d727ff8813ab2e92cda fix dns reconciliation for ibm cloud or providers that provide a subdomain
0dc31266db811458bf5f75f5f93fd972380190ad Merge pull request #1121 from openshift-bot/art-consistency-openshift-4.10-hypershift
37f689960304e4b502c85553591c98dde7ba225b Fix create nodepool azure command
2c6a40c611f702a2c7909396aedd3d8fdd3f4039 Azure: Fix credentials log
5138bafbab2be1ad020a0d87681d41223eb4750e Merge pull request #1124 from jzielny/main
85bd6367074179e1dd0cfaa876c21f4b05178dbc Updated secret permissions to 416
b7b0f0f2507a62c620f042f51285c91edb35ed7a Updating hypershift images to be consistent with ART Reconciling with https://github.com/openshift/ocp-build-data/tree/4942debcc90598c22828c946d9c07daad51b4584/images/hypershift.yml
930c35642383025c5fb8ac053bd3924288c8570d Merge pull request #1113 from csrwng/update_410
1e81ea19568f83a6fdc5af86ca9b6b52d47df0db Merge pull request #1106 from michael-topchiev/missing-readiness-probes
ee961a28a0e32f6aac3e8f872a1e42d27dd27165 Merge pull request #1119 from jnpacker/fix-azurecluster
9fe542e68ebcfcc0afdc2746340b55fd530cec66 Azure: Stop logging errors during role assignment retry
0d560e63ad88e71ad119992cabceeaa0a62e1ab7 Fix type in azurecluser for Private DNS name
df8d07046be415b1a579b430961404dc576cdeaf Merge pull request #1097 from alvaroaleman/rootdisksiz
63dbe5a6cdba4c4ff55daf5d13b793f81e24c75a Merge pull request #1117 from enxebre/fix-broken-link
e020146dd5396c3258d9f056b675e34d7ae16433 Fix broken link
3dd972e451839a14e81fe8687d608f0ac6015777 Merge pull request #1116 from enxebre/multiplatform-support
151d28fc5728da393309d8edc5defab310cdedfa Add docs for multi platform support
5ea4205ee7c332ddc8d46ad84126f42606a3a58e Azure: Make the rootdisksize on nodepool configurable
ca08c873e871cb32343e99f891141686485973a0 Merge pull request #1099 from relyt0925/token-expiration
67d49002a920e81e1f9f0f9e87a7849e9abeb304 Merge pull request #1105 from alvaroaleman/cloud-config
27690f349238f15ed3a180d6411e1ffa0f95a878 Merge pull request #1115 from alvaroaleman/defaulting
ae6817e651a8a629e6577c4cf0665ed22348b729 Fix defaulting of issuer url
a0a1fc92ad7ca81bbcf7929b869cc74da44da475 Merge pull request #1114 from ironcladlou/cvo-servicemonitor
321bd4d5b30b2ce584f109e56bc05b0f2215b9ec Add ServiceMonitor support to CVO
239155928655057d7b5d287ef196170ec739c918 Merge pull request #1112 from ironcladlou/olm-servicemonitor
34192081b21fbc34e53a95bbb0f84ab100f88e5c Add ServiceMonitor support to OLM components
88d22ffa132628a51f879202d5eaf07634329900 Merge pull request #1110 from jnpacker/azure-credentials
97b93567db499c63ede505952b54372437869449 Merge pull request #1107 from davidvossel/kubevirt-base-domain-fix
2fb3e29a8b823c0ad98bb296ded0c697feed3c3f Merge pull request #1109 from relyt0925/automount-fix
cf1c9f3d633a0d1ae474c9f38df3b73d4f5de7aa Add support for azure.Credentials * This allows Go functions to call the Run method without having a local credentialsFile * Optionally allow the input Options to contain the osServicePrincipal information as an azure fixture. * If credentials fixture is not passed in the options, default to looking for the credentialsFile * Support options for Azure destroy as well
e36da48d7308c9c1d9bd5f379e1743e983f4d791 don't mount service account token for cluster-policy controller
5c9b77ee4b22f2d654787137311dc7aa7a832cbb Make --base-domain cli option work for kubevirt provider
de5f4ea8d43a6e72bb84aaf950b47124ec587281 Merge pull request #1095 from enxebre/add-nodepool-conditions
a7f29e4067ac584946bf2edda79e4c3fe2c1693f add token expiration support to prevent nodepool upgrades from killing in flight provisions.
ee60f74c38179bda8fd97ed77ae35c126578d1ba Azure: Deploy cloud-config into guest clusters to fix e2e
467006beb4e1124bc5efbf4b127cc0b33aabf7cd Merge pull request #1083 from relyt0925/hypershift-pause-annotation
eec759e5b6096ffc2ba823665bccce6e1c54f99a Merge pull request #1100 from alvaroaleman/azure-management
8ab9402b76c5c805ae1c075ae60d24347019f43b Merge pull request #1104 from csrwng/config_documentation
6a8df4177fd3fca942a968aff9baa5b66edf2739 Cluster configuration documentation
fa667d6ea41dcb17357f7cf8e12e3e13c5e57612 Merge pull request #1094 from alvaroaleman/reload
3d61bff4b7ca10bccab7b5029f49a8d314b6af2a Azure: Work around a bug that lb services with port 6443 don't work
9c96fb48a87b93e9c9e2fbbc269fc6d2e16fd1cc Merge pull request #1102 from sjenning/adjust-budget
8c28028b83063329f41585037ac1233b23f549a1 Missing readiness probes
37ad6e1dba82cfda779c09b58bead1c20d19b932 e2e: allow up to 5 DELETE 404s
6214445b9956d4c99d120d7cb8291fbb259dfd21 Bubble up MachineDeployment ready condition and print current/desired node
eb980b554f13868e4cdedc74f8e98fcb6c167c87 CPO: Remove redundant kas service definition
7f2805bbd631a8e0d1e2e7b4792d54f255c0e0f8 Merge pull request #1098 from ironcladlou/os-exit-audit
5e866531ac7dd942ac25480954a83acfe45e9e89 Purge all non-entrypoint calls to `os.Exit()`
5721770e191c6980fe78b8b3f55d5b465f120cdb Merge pull request #1096 from ironcladlou/ocm-servicemonitor
f2fd0e3728dab4544f263fe8e98bde8fbcf5cf46 add pause reconciliation support for hostedcluster controller, hostedclusterconfig controller, and hostedcontrolplane controller
819feb1f565db6f718c7e7715a3b5a5767daae97 Add ServiceMonitor support for openshift-controller-manager
10dd862fce286acdf83b3190c110cbc88104397a Ignition server: Dynamically reload serving cert
c2e4755f36a1feb78897e30ce53fa3095db6f738 Merge pull request #1082 from hasueki/preserve-container-resources
a9eefe5f1cee57dbdceb63d4817a923956920f9e Merge pull request #1092 from relyt0925/up-leader-election-duration
05ce225019abb764a5781f337576235e30ffa91c Merge pull request #1093 from alvaroaleman/storageaccount-name
e2ca5a3638112a61f0a1652abbe99459b4fb41d6 Merge pull request #1091 from ironcladlou/oap-servicemonitor
4b5cb2d56565529bbc1101ba47ca4d858640c373 Azure: Use random string rather than infraID as storage account name
61b641c3c059b6b2e1186c95764e212319887880 reduce frequency of leader election for components in the management cluster
0fe56fd8a7cc660d0c81ab290813364e32827da8 Add ServiceMonitor support for OpenShift API server
afe81b848cf8e4f1d58904c56ae02e380b8e8aa0 Merge pull request #1088 from ironcladlou/kcm-servicemonitor
da2079747b7e4d737c733be276dbf8bb68d58631 Add ServiceMonitor support to KCM
71405b361ba370c9e0146357d9c417d4f0922e7f Merge pull request #1068 from ironcladlou/check-budgets-post-teardown
f9c9affa2ab6a97a9f6a7ffc0c18d2745d406e14 Merge pull request #1032 from nirarg/service-publish-strategy
c0428f57a9116ede4df59c40f037fe01265e418e Merge pull request #1087 from alvaroaleman/azure-compatibility
f2319105e205359a35b643f114c24c6996b54500 Azure: Use same credentials file format as installer
7b6c744683cc6c38d796c4899b7ea8cae1c5aa21 Merge pull request #1084 from michael-topchiev/no-automount-service-tokens
b50779e2b7f54af83c4f2169a4350ac29ba47223 Merge branch 'openshift:main' into main
e69e26ec3c3cf9ff2f89643e9b7cc9c319aa1e94 Merge pull request #1071 from alvaroaleman/metrics
8c2d71dc6861ca93815f003edd3b4cb361dfff4a Do not automount service account to seven deployments
fc8a921ef45e53c15f2445e797c3a7406ae2175e Merge pull request #1060 from ironcladlou/servicemonitors
15e1a3475b0af3523d4b4e078f029f88a72298c8 feat: Preserve container resources for control plane components
9df846eab0f803999e98d351d6af72055111e349 Merge pull request #1073 from alvaroaleman/dry-delete
d769489d24e32f099be660b8bc6214b82dce3bde Enable ServiceMonitor support for kube-apiserver
c2ec50098c14c84997a7467966deb15468770a67 Merge pull request #1080 from sjenning/exclude-catalog-rollout-pods
ba21a018c671431ac89a6ae198ee472c001124c6 Merge pull request #1081 from enxebre/fix-docs-ign
3300641511ad4c2c83d362a80ecb35014fff4720 Produce config metrics for telemetry
cbfffdb4905068adb3dfa7ad0088f52473cfbfa1 Fix ign server docs
b6959f8d66cd3da2a7c1fe8e0c17bc2454d0309b Merge pull request #1069 from enxebre/fix-getname
fa00332013a4de32c7769735d8a95c0d18802f18 e2e: fix API budget assertions
d85f5993ea6fd2171989139b4ca4a0c1fe13378a e2e: exclude catalog rollout pods is EnsureHCPContainersHaveResourceRequests
d01aefc3ea9db9ed08a2ac2a8173e24a1b891571 Kubevirt platform: Add service-publishing-strategy flag
4c8a4ba97fcec63eb0988b813bf6f9b6df60a16a Merge pull request #1077 from avishayt/avishay/MGMT-9423
661c9a329064250a906c4165ec13b4c99d0b1a97 Fix getname func
c5b1c66dc25a488f889f9f2b5ba884c0861d936e Remove choosing Agents by minimum CPU and RAM
e22efad790bc9116c8835b7a3e5fb889b96ab60b Merge pull request #1072 from alvaroaleman/redundant
0e928895ed38886d86ac46a2d131b5c3a8fdbb11 Merge pull request #1070 from sjenning/fix-oas-trust-gen-anchor-script
1a06e4a95897a64e31b47e34eae4d1d1531fe6cb Factor out repeated code from delete-if-not-deleted code
21eb34e049bc6121dab239e7d0c6892c7787e86a Merge pull request #1063 from sjenning/fix-unchecked-deletes
aa01168206f53b6281f44f0c6f6c71558dd099cd HO: Remove redundant watch for routes
e9580eea83351e81edb79e10cf6631d06afbb944 Merge pull request #1066 from enxebre/nodepool-naming-fix
31dc6e54d7586a978528199949643c5af5dbd7f4 force copy in openshift-apiserver trust anchor init container script
3bb612e9feea5102517d2f65de466d9e7de49028 Merge pull request #1065 from alvaroaleman/azure-creds
c34a1c5aabc7bbd71a8a89987feebf0ee9682e97 Let NodePool controller wait if infraID is empty
b3b497bcb8dede8b97ac6b379b346b21e7c597d2 Merge pull request #1064 from sjenning/fix-cpo-budget-queries
2c644b405314a7a3bccf47ef0eae80b4cf1814b6 Azure: Validate cloud credential secret is valid
7d6a637cc543ce499397203d0f99dfe0c20adf82 e2e: fix CPO budget queries
0bfd26421ebce24dfb8f0dd802f2bbedfee02d71 Merge pull request #1061 from enxebre/func-docs
4623c207f12e0d619da853b4f72e5698552f37bb fix unchecked deletes on CPO RBAC resources for ingress
80883659ca1d4e68623d3cb8a046118050674bec Merge pull request #1012 from enxebre/ign-token-rotation
7e1fe6f68641583fb387a1517ae2ecd6c8376bea Add comments on Azure cloud config funcs
0371f8892dba747a28bc2110b9839961be3c13e4 Merge pull request #1054 from alvaroaleman/kcm-ks
f3570d74c000d7ed381ee67ad6a6b92c2695434a Merge pull request #1056 from alvaroaleman/creds-2
7f780e7ded8439b5835013b71aabe5d01ab414dd Merge pull request #1055 from alvaroaleman/default-infra-id
ce281010c070c0b3f1e1b010ee808960b9e93f52 Merge pull request #1058 from openshift/ironcladlou-patch-2
3e1b4c8cee166ab1f476d2765753a152bba5eb63 Merge pull request #1039 from hasueki/reduce-cpo-perms
3fdbf0a95d5fe767e468a014bd94f2a7c8c804ba Update ignition token rotation flow
246ae2daba5746fb7a33f46502d305756e4780a4 Merge pull request #1052 from sjenning/add-resource-requests
4e28842f2598802afe1cbf4e7697a5a11aef7e55 e2e: add test to ensure HCP containers have resource requests
27b125159ecebd67f595ddd285c9e478ae221a54 Remove outdated binary from ko.yaml
36c5d9aa65013c6843fe1dd16e9c24d018c16828 fix(cpo): Reduce CPO cluster permissions
fa58e9e1e04a33f3cfac588628274748175daa55 Merge pull request #1057 from openshift/ironcladlou-patch-1
d4cca92d136a567861e7910b00e7cf53a08e52f2 AWS: Support all properties of shared credentials files
ed5c1e031427788e1bf028e31f0d1b8c0fdd2c0d Hypershift operator: Default the infraID
de80b53dffd05351b30749821ecebe708166a435 Fix CPO shutdown to prevent leak of lease hold
1bc8d59c8fab347a22455da3183c68a06061ed82 Merge pull request #1053 from sjenning/loosen-cpo-read-budget
d989a5183e03c8ca67b6a1f4472c0730b530785e Azure: Deploy cloud-config for KAS
3630ea167dcb1ccecb85961634c9036d5149afd0 Azure: Setup cloudprovider on KCM
28cd2757781c0cb1f8d38c1c87e8addddb23c806 e2e: raise CPO read budget
857daa714c6ea69050cc9637a138592078f879ef Merge pull request #1045 from tsorya/igal/cluster_role_for_agent
16433b383571d69fdeae19de273e3efc83c43557 Merge pull request #1049 from alvaroaleman/io-minter
f906086f606d15e9d5445fe3666eef229c8cd8c0 Merge pull request #1025 from alvaroaleman/azure-nodes-join
0623eece746a923572fd6be05d4f3375c3a8e64d Merge pull request #1050 from davidvossel/fix-kv-network-interface
ff91a05dbf34bfa8ad12913099ea57a3d37e392b Merge pull request #1047 from alvaroaleman/private-dns
d70633dc74d2918d6fdf75d6fb8d04b7e4de6052 add resource requests to sidecar containers
0caf0290617d1d67abda579fe414ff0eeb546741 Merge pull request #1051 from sjenning/add-request-capi-manager
56f0358392218a6a1598a3979579a6bb2ece9bab add resource requests to CAPI manager container
397ef88f6e25e66d94b1545c688a6610e9928109 Use bridge binding for kubevirt platform
453068ad091ce0368d144eb1e4e541e8a70d8484 Only add the token-minter sidecar to the ingressoperator when on AWS
9e57060258f5d8b622a4f09cfd27cfcb02163337 Azure: Setup the private DNS zone
02ff93e3ae5c85eb7f8b060b9fb17663ff20f646 MGMTBUGSM-108: Adding clusterrole for agent provider that is required by ACM to create clusterdeployment
f3d0630f782056fd6914101234cc6b04e82eb82d Merge pull request #1044 from alvaroaleman/creds
1cf7d81ba5582b496f3fc0bf4f0311bb374550a8 Merge pull request #1030 from sjenning/api-budget-e2e
ab061103290ebf779f9489fbff944d89af82715e e2e: add API call budget check
3a192a7f1017d12fd08c85471338aee481d37525 Azure: Create credentials secrets for in-cluster clusteroperators
cb83060e5ab9299f0aebbc8e56cafe2c91fa385b Merge pull request #1043 from csrwng/fix_cache_client
aa2c387cc511ca83b6c7b4af120928b32f5eb654 Fix RESTMapper used by HosteAPICache in Control Plane Operator
d36b669d8c525054690cc760957acca17bb7c7b0 Azure: Add node management
93ea4702f95271ecde304f0b0e7b3035b44c146c Merge pull request #1037 from alvaroaleman/public-dns
cded9f5c2053fb0609c02b1aeb7b7284a6f87f3a Merge pull request #1036 from sjenning/include-pod-rules
8e1add5ebf43c47c3b4074aa4a0fc771421dfd91 Azure: Setup public DNS
81bd140eeffadd0bad22dbf643392ea4fb8697e8 include pod in CPO recording rules for multiple CPOs on upgrades
20612e488ecc2f537653a3843549ff41622ea26a Merge pull request #1035 from ironcladlou/dump-nodes
6da58b94e5c86a739c557a5f7379b22d79517b42 Merge pull request #1034 from alvaroaleman/wait-subnet
a6b4fb9f4451307c2d4661ac9943b0497e1f822a cli: include Node resources in cluster dump
021e9e8ba9712a7122a4acae5711d9287c6bd3eb AWS infra: Wait for subnet after creating it
b5aa18d25e66200cd541ddea4eb7ef644c3f4374 Merge pull request #1033 from ironcladlou/dump-panic-fix
80cf739e894a55a540c74ceb674af82d050bd9e8 e2e: fix guest cluster dump panic
f3b29fc7043dfc47ab7a0899e097ba30d2932419 RBAC manifest creation for Hosted Cluster admin personas (#1014)
a7f0d329d28a38e527d3261c53e951651308a122 Merge pull request #1027 from sjenning/avoid-delete-404
8fdaf5bb8097bf20020548964feca577fe383cbb Merge pull request #985 from nirarg/kubevirt-quick-start
9dfa0c380fb7a3140be23ba6ab9af12d36bcbcfc Add Kubevirt platform quick start docs
b22a034c30ab1a5f109dc729077d56504358f6f7 Merge pull request #1023 from sjenning/refactor-upgrade-race-protection
fd5e63c51fb9e7189d88614f6eece3c7206e4e73 Merge pull request #1024 from ironcladlou/bucket-name-validation
add41fd0575416ae375701eda4f7c88ae2f08b7a reconciliation race protection during upgrade with OPERATE_ON_RELEASE_IMAGE envvar
76e5b4e9ec92173b520d2a6dc2e14643bb873e02 Revert "add logic to ensure control plane operator and hostedconfigoperator are at expected version before reconciling a release update"
bb1e9c23916437a252d6cc0d665d67ad7795bcf2 refactor delete to avoid 404s
24b93b9ab55f4c846def086e9bbbfd1bdd2b753e install: reject bucket names containing dots to prevent HTTPS errors
e4b844b9d2c545f24b2ea64bad14257661162407 Merge pull request #1019 from sjenning/cache-services
736b23e5fb6fd6f78871e3f3c55194c0ddc1ac51 Merge pull request #1017 from relyt0925/no-capi-ibmcloud
e6ed75c8b0735a7582345dc0b4329fd71a5014f8 ensure no capi cluster is created for ibmcloud platformTypes Classic and VPC
240f0f2628155a76f70dd982dab5723e41f94f72 Merge pull request #993 from alvaroaleman/azure-create-destroy-api
35e8ab62421588639dd8848ed6bc9945228f0e9e enable CPO caching for services
197707c836329b3573300e7fb10a51601c245523 Merge pull request #1018 from sjenning/fix-olm-direct-create
1d34f339024a8699effb85a14429ce78d18afcc1 use CreateOrUpdate for OLM collect profiles resources
f806c6eb457b5ca2324c7a97767b48bad96f6fea Merge pull request #1016 from alvaroaleman/minter-init
61efd0459d69874a90170ddb2a433149e4e3292b Move the tokenMinterImage arg out of the platform interface
67e8c315a6a924701a3b62c2c57132191a2425f6 Merge pull request #1015 from sjenning/ha-upgrade
4fe096c9677626ed79942b8598dcf96576f6c81d e2e: make upgrade test HC HighlyAvailable
413f0e8190b558bd7405a3be45c467b591df7c25 Merge pull request #1007 from alvaroaleman/ap-aws
bbfde5bfdc5781691bd64152d2d04a49b40ea8cb AWS: Use availability prober in capi provider
c036de9df6f1117b72c9e0bbf588ff659c06f95a Merge pull request #1005 from alvaroaleman/re-enable-guest-dump
62d2ab5750a935e0512a40cfe3fc68b2fe66ccbf Merge pull request #1006 from alvaroaleman/add-gotestsum
bf1e3883fe0e720b0efe987cee44fa81ad7f219d Re-Enable guest cluster dump in e2e
331af4ec5849b749c3f47e4e7f77054bd0617319 Merge pull request #1003 from csrwng/create_kms_key
e5d868f8b777d2937080ac102a86e168ab9549af Add gotestsum to e2e Maketarget
4e2310af5ab9b58383a1f3cfcfbe8c8acab230bd Add token minter for kms provider plugin on KAS deployment
064ffdd3bd4c41a56da388c579b1afd87464fc7e Set the default AWS KMS provider image
c44924b24377d976e42babb374b31d8fdbb2576f CLI: encrypt etcd by default
ee1bc3f4bb15ac50acc9f0a857c9d8ae0123c743 Merge pull request #1001 from sjenning/adjust-leader-elect-tunables
9921d225d06f9895ed71a1321a6433ba3e481c59 Merge pull request #1002 from enxebre/upgrade-docs
74d4579eb787300f9b834e04684ff34481e1236b Add docs for upgrades
cfacf48ed6ab28b33a2226a63b2265d2185e5007 increase leader elect durations
03c6098d32c52f31b5459857171d19a0b3b7dde8 Merge pull request #997 from alvaroaleman/allow-version
a9fc4a58cb8aa1d095a06f16c8eff64eb5be082e Merge pull request #995 from sjenning/fix-create-nodepool-aws
033eb51811339c0eaf1a4ea1b1dbf314c5667e1e Merge pull request #999 from sjenning/fix-recording-rules
8427644fff0de9bc60c6f4d37e4be4ad1a516f4c Merge pull request #1000 from alvaroaleman/skip-es
e392e978a9cf06910b5a41b6ecfc7c6d1ccaebdc Skip endpointservices in the loopdetector
6a6fccd83fc5692cf0adabe0a3709a95f5f7411d fix recording rules to work with multiple HostedClusters
bae70a90c61c99a3edcb58bfc7ea7f72732af1a1 Merge pull request #998 from alvaroaleman/dot
390372fe531a38daafa47c051eb38a854f915206 Add Azure create and destroy commands
b9cbf7ee26aadf75eab1c16c238055f26dacfe09 Properly deal with hostedclusters that have a dot in the name
05da03d3088723b69807e2cd868b3a7d67928548 Allow OCP minor versions > 10
bc16b7c25b1f4580a1f7756ec6aaeec1234dfca9 Merge pull request #996 from alvaroaleman/leader-election
b2188b7294f0dea0a74c3ddc209bfec82a18c171 Hypershift operator: Enable leader election by default
15182296112ad498e67184b4a05b2d4336dd8efa fix nodepool lookup in create nodepool aws
1f3f30bf78e8e377c64bd905eab3c4feaba2767f Merge pull request #991 from sjenning/no-tag-cluster-scoped-resources
e6771b642da49fa8f9d1305698b5a377ab24bebb Merge pull request #963 from relyt0925/gate-on-releaseimage-rollout
6785174a1a8f401b3b881bf826c4f3f887dc75e8 skip annotating cluster scoped resources
7e64db2b6d2e70b9fac4f6fec507c1896b66e0a0 Merge pull request #992 from sjenning/ho-leader-leases
243fdca5fda48247405dc3470a5eca6129c587e5 use leases for hypershift-operator leader election
3bedad795354f47bd2e18ec970d23d2430c070af Merge pull request #989 from ironcladlou/render-yaml-fix
a9ca68529112195d9108af765dd79e05c331b909 add logic to ensure control plane operator and hostedconfigoperator are at expected version before reconciling a release update
2058f9a3ce13bbaec6eaacf126aec4165d5fbb7d Merge pull request #987 from jzielny/main
3deea20772a3bcc21143b732238fb679459d0db2 Updated saas_template with make update
a93b185bc9028f5138133daf57f2f005433e5089 Fix `install render` bugs
96f0a6545776048836ca6db18a50420c9bedc9a1 Merge pull request #979 from avishayt/avishay/MGMT-8469
be1ca865141da65c3bdc538d4063d18680a1c365 Add agent platform to docs
84cddcaadc683c44d2209d0cef49fea471eb6a0b Merge pull request #988 from sjenning/move-subnetid-reconcile
1f64572847f056841899cd3680e14a56eac4973c Merge pull request #953 from nirarg/cmd-logger
5153d380024064dc297b37838475b6f3f7417381 move subnetID reconcilation for AWSEndpointServices
60ab6874af9d299753e44a267ea43716eee98919 Normalized the resource requests for hypershift operator
b403a7c617c46a152245161e2aca189b2c0282cb Merge pull request #982 from nunnatsa/add-ci-kv-install-script
c1065f44a48b29fbd3ea8e9e94beeac401752b41 Added Resource Request objects to components missing them (hypershift-operator, machine-config-server, openshift-oauth-apiserver, control-plane-operator)
28995b0e2f4c77fb858af8a13fadbfc3f73c8124 Merge pull request #984 from sjenning/zone-e2e-fixes
98fb5b89a3d006ac291413b838cd49d79c39c78b Merge pull request #981 from enxebre/personas-docs
e40d3edf3ef6b80cd7cb4e45741a9cb1714138df cmd logger: Change all modules to use the same logger
9bce129ea051aad71149cb7630bd17da24c1326d support multizone in e2e-all tests
6892590194c9586124772955511886a504b2c92a Merge pull request #978 from relyt0925/add-nodeport-for-upi
637c31fc7e36cd55083f9eb145db4ac2cdfe1354 Merge pull request #938 from relyt0925/reconcile-oauth-named-certs
12495d9e5d79549af8832defd8ea45724037ea71 ensure ingressController exposed as nodePort for IBM Cloud Satellite so ingress operator rolls out
a6fd26e38e6a1ad886af0daf95259e66f59922bf reconcile named certs to oauth server as well
17effaaf1689d05e536863941d3d56e1e65c02b4 Merge pull request #980 from tsorya/igal/agent_cluster_changes
8b28de4a1011da2efd14f4a0afb8a52fa33c4820 Add a Script to install OpenShift Virtualization on a CI cluster
6b9ea9576dffa2c1503f5ec0332f65368e844283 Add docs for personas
a5bfdb7f0f0fdcb71407f764f1c04b3119b0a2e0 MGMT-8860: Update Hypershift to create the AgentCluster with minimal spec We are removing unused fields from agentcluster crd by updating to new cluster-api-agent-provider to new version and removing set of those values
cb6c00d0c6ff0e651ffaaeac223d933986bf296f Merge pull request #976 from sjenning/make-update-target
d005dd23e209b589bd3724ba0406eece82f97b4a Merge pull request #975 from sjenning/revert-966
0aeaecfdb5a143e3b83795df4b461a302d132d49 add update target to Makefile
d4120826004472b027035390a845174e00c0aa2a Partial revert "bump 4.9 refs to 4.10"
57170bbdf5577260a1f6fefcde9bdcdcf5eed4a1 Merge pull request #973 from sjenning/docs
6f2e55c3cbeb58019a0ca2fd4248469ddcf60e42 Merge pull request #964 from sjenning/multizone-guest-e2e
8738ee68b657eb621edd0d77243feca85df4500c docs: how-to: create aws hosted cluster in multiple zones
f9c008c963032f2dd9073b24275548c1819a2279 Merge pull request #967 from relyt0925/removeError
6882c6c0b9a165d49a1a9d79623fa001e8702692 Merge pull request #965 from relyt0925/fix-install-regression
0648d8c59cc675addbd3e73912514ad8b8f63806 Merge pull request #971 from sjenning/docs
317c9d5c378f5e1c76cfe2b7d221dbc64d3dd24e remove invalid error return when KubeadminPasswordSecret not found.
ad59f29d1fded917c12c500af93c9c9e184942fc clean up docs for restarting control plane
a8248a9b7bb3eba3ef5e7b8c229278d316f1d32e e2e: add AWS multizone support
027e963325b006f974e1ae21278e36b1219abfed Merge pull request #951 from sjenning/private-multi-zone
70bae148a291f50aff804539a0378014558ab71e only add oidc mounts and arguments when they are specified
044a2a50c02eced7b9712b94507ef0c6ed49920a Merge pull request #968 from enxebre/drain-timeout-api
b98adca60bd4752a5801d54d4a4a213956cdb763 Expose NodeDrainTimeout in NodePool API
e52e236a2524dc903ceb280fc9acf9585ea2ca28 Merge pull request #960 from enxebre/fix-docs-rendering
9f5c83dc4740c03b7af179e5cf26b37085d827d0 Merge pull request #954 from nirarg/hypershift-install-fix
ab978565e89fafe160afc812ccb5f492e5d90e48 Merge pull request #966 from sjenning/bump-4.10
963d7a90233406d6add360da19e03b2326a0ae70 Fix issue of NodePool not created for Agent and None platforms
cde148a62307d04de30416c2e8552a044a216aea bump 4.9 refs to 4.10
b9f78d00f275fff8f75c4ed36089f4e7dd3938f1 support private multizone guest clusters
0fd930af5d7a8455db87f5f8a9926bbaf9f4d764 Merge pull request #962 from geoberle/tmpl-replica-param-fix
258c7b460439ce47e0d05ee1797559bcb87fc3ed Merge pull request #959 from alvaroaleman/increaase
08e1450508a49ebe4d856298071bcd5803c2f54d fix replica param quoting in openshift-template generation
088e3241d2d4cbd645cc8835d22b49fda9933176 Merge pull request #956 from nirarg/nodepool-platforms
d939a5097f6db7345476ddd5cb765a5389f87cae Add Agent platform type under NodePool cmd
220af547529fea722e05c2188b407e6d7a03fdc5 Fix Priority section rendering
1906c42f846a077893c2c27d5e18da25c645bd35 Packageserver: Give more leeway in liveness probe
61272973b6134cb6ef9702779912c2eb0aee76c2 Merge pull request #955 from enxebre/etcd-workload-distribution
12c31f3e0badd69e1453a88a9b53b45672edc41c Merge pull request #958 from sjenning/fix-awsep-error-handling
830b76ed86d93daf558e8bd928f721b707b43396 improve AWSEndpointService controllers error handling and status reporting
492fc17d8f0e5e626329d1505426dc55bb562604 Merge pull request #939 from geoberle/template-generation
7ce9594c604a0cbae05c4146f0d9ada9d84cc76e rework template parameter patching
afc6c878b4b589e44b83d4b1360fa82d9fe9d6ff generate openshift-template for operator installation
6ecf9876fb6592644b75282081944bdffccdba5a Add priority classes to Distribute Hosted Cluster workloads doc
ee39a61051cd4f5937e59767b03c12e01a5e6875 Merge pull request #952 from nirarg/hostedcluster-platform
8937caa930977054ed94421349a4a424e6df7258 Merge pull request #950 from sjenning/fix-awscluster-hot-loop
17c95eda2bafbc901c8db069e5e182f4ec69b06d hostedcluster platform: Add kubevirt validation line and remove mockgen comment
25d75f452f9909467f3154952036806195e5c0e3 fix hot reconcile on AWSCluster
8db88cee3ed02d5e0a6246196637df602f263e52 Merge pull request #949 from ironcladlou/install-oidc-secret-flag
dd74591d5631688d7f30dac3969a0f0874b507dd install: Enable user-provided OIDC credentials secrets
c96eec9211eb6805487d9d4f047ffe6e002c330a Merge pull request #947 from nunnatsa/fix-nodepull-name-in-kv-test
91493d704cd498bb3eaaabd434901cb3c4d4982c Merge pull request #948 from enxebre/aws-nodepool-subnets
72815afd1074290b656bad28853f192516b2b3c0 Reconcile AWS infra CR with NodePool subnets
912f8ede8e1e69dc12096381dc50f4d4cb10fd3a fix the node pull name in the kubevirt 2e2 test
685db7284a8b9ab6adc4c1c41e9741c6efdc9883 Merge pull request #941 from relyt0925/ignition-server-2
3092982fb4e5dcb52ef8e51d9d21b9b3b6546485 Merge pull request #944 from sjenning/multi-zone-infra
9ad8663d64ebb34ce2e25991881181345d4cfb43 Merge pull request #940 from openshift-bot/art-consistency-openshift-4.11-hypershift
2c6e6dd1461be51bfe8812c5a0ef2261244bb142 add multi-zone support to create infra aws
9dae9158c42618e6c5df30044cf04ff8c2aa42f5 Merge pull request #935 from relyt0925/shutdown-in-parallel
a1435479eab0424f349d4f4815e3b93fb279e1c1 ensure all components respect the restart annotation.
a014f7325baa9e152dc7e372c2677b19bc170989 enable leader election for control plane operator to prevent race conditions on upgrades
00997c4011d501a700fda7099f5a034421c20d62 Merge pull request #943 from nirarg/kubevirt-cluster-update-status
0a0330eb650f2c7b9a8aa5e331a7b2ac9d2f53e2 Add KubeVirtCluster to HasStatusSubResource list for CreateOrUpdate func
e08bae01cfc0e3b085bd5f285c633feddcc0c77b Merge pull request #928 from csrwng/create_cluster_howto
e35b31b6a1d957331257518e6dc51ce6fd6f4133 Merge pull request #942 from enxebre/agent-creds
82f326459cddb06214cb517de1a6a80574d4f321 Rename creds rbac CRs for agent platform
9cf1247c9bc19f5ad2865dfc3054d19cc550a5d3 Updating hypershift images to be consistent with ART Reconciling with https://github.com/openshift/ocp-build-data/tree/0059e470a61eba28225165168b22d9e77c33c926/images/hypershift.yml
9b0c2afbbaee8e4330d8a388498d6023e7508c7f Merge pull request #932 from alvaroaleman/otel
00154e2f27100633ff1fe90aa0f177c3461aa0cd Remove opentelemetry
3a1bedfe5b1a1081b1a3653d9c9cf329b7256759 Merge pull request #931 from alvaroaleman/cm
c11abd59224ab8c66d962dff91d262bd8445d2d1 Hypershift operator: Ensure the oidc configmap
3ac5f71437f256860389756e711213f899d65dd9 Hypershift operator: Fix default ingress controller reconciliation
20f42dfc728c7bf86d0e6dc14c1d009db061c1e9 Merge pull request #927 from alvaroaleman/infer
8859e19e07f8eaa98cd316b9adb138d9e6a7d928 Merge pull request #929 from alvaroaleman/improve-world
239336bccc3968f24b8bfc2ba6dd191d8648c17b Add how-to for creating infra and IAM resources separately
c4724d7afe2d9e8588d84ba57d45a812483704a7 CLI: Simplify provider-specific kube resources
1b87fec6e10073dd4831827af4d1e283397a31e0 Merge pull request #926 from sjenning/add-nodeport-networkpolicies
ed514151e469ad668b574bec4f72ef9ab5e0b69b Automatically infer infra cr GVK
9a6b831e1444a2d7914ea4630e2465b528ced1fb add NetworkPolicies for NodePort services
a42f4fd1c6e1a15951d7e3197c3b39d0522874f8 Merge pull request #924 from ironcladlou/docs-link-fix
2e78bfa6fdbe80b8c39c5ac86bbebbe316745a83 docs: Fix broken link
8aa1ed34facb0bbbc482a4ee11a21d440ca960ab Merge pull request #922 from nirarg/nodepool-cli-fix
29d66cab9e3ad59069605f3c8554471fe78793d9 Merge pull request #923 from ironcladlou/fix-log-timestamps
5e42a1c82e9835f458d325dd0709ea521d1d4a53 Merge pull request #905 from nirarg/cluster-validation-fix
170b0dfb03bb3f521393e9462c87c5563f15c03f Make JSON logging output in RFC3339 format
a0ea828a7dcc8d054debae953c0143d1d34fae50 Fix NodePool CLI
9a6f13b0b027cd55cf7a98ee8ba8ce4a4bcf4e26 Merge pull request #917 from nunnatsa/reduce-image-size
6f8bd2e1c477eaf6212a8d8576fb41719e746188 Merge pull request #883 from nunnatsa/refactor-context-CLI
a0bf0ad952492790a1429db2c8bd6466b8abceca Fix HostedCluster doesn't exist validation
dfc9415708ec46020b7ced4e27576672d66be79c Refactor context usage in the CLI, to reduce code duplications
60c80be8fef5896e9eb5d9ec5b7b8d01e27a6869 Merge pull request #896 from geoberle/app-sre-template
ff041d9f6cc3aafc39df9106ef07b2e46fc4445c Merge pull request #860 from jnpacker/add-new-awsconfig-creds
03813d7adddce6180cdadcc38791ae7357e08521 Reduce the number of the docker image layers
8c3a36bc6dc0e473824774627ef1a706fce47034 Merge pull request #919 from enxebre/hc-wokload-distribution-docs-improve
6e38efce4e102df3b234186db448d958160c0874 Improve docs for distribute Hosted Cluster workloads
1257be0581390fd5401ed863e073f20cd50e6682 Merge pull request #918 from enxebre/pod-distribution-docs
6d594d1e32a41d0b5d454e59510b730073dbb0fb Add basic docs for Hosted Cluster workload distribution
12c92b28e5f56bf729c04077bdc59997a678ca39 Merge pull request #916 from relyt0925/release-annotation-propogations
2769c3a4210a0eed95d7ffc9410871aa7ddd4e5c app-sre artifacts for image building and saas deployments
a7597abed6299c97e8dea82d9dadd8f6a332c3c5 add release annotation to konnectivity agent deployment
036ac65f4636b07a640c0e692f28654ed00e8046 Merge pull request #914 from ironcladlou/api-wait-for-etcd
ca5f6d63171b2d4a3b9b3770b2378ade5e47e464 Merge pull request #913 from alvaroaleman/bump-feature-gate
0a56ba906ab5847890465390fd2f5f5f7171487f Merge pull request #912 from ironcladlou/periodic-fixes
1f908ad7c2af1853688a7b73bc3d6bf55b5f6761 Merge pull request #911 from alvaroaleman/fix-sa-name
d9b9d165fadb729d30b9d1101e9cc81a0f6d7df6 Merge pull request #901 from relyt0925/update-hypershift
d43db8ea09464da36136f3ddc1957d9f4f0609d8 Merge pull request #899 from relyt0925/fix-machine-template-reconciliation
6f6b63d2f302006b543cf6f6300ec17ccaefdca6 Merge pull request #898 from relyt0925/use-combine-ca
99e829fe4e8e08b9206c008c254f27b71463f546 kas: wait for etcd client service name before allowing startup
54e6bd40fdb924a874aeeb2e2e690cc46f91aa9d Merge pull request #909 from enxebre/TestReconcileKubeadminPassword
3dde82aa80b3ffc133100ee2c8988c2308222970 Add AWS Static credential suprt to some AWS functions when vendoring. infra.aws.create infra.aws.create_iam infra.aws.destroy infra.aws.destroy_iam
ca2698207365d13ca716f69f3085d44332167ade Get current feature gate config by updating o/api
d544a24c7874ca8cb6b2199b11d593162954b1bd Merge pull request #908 from enxebre/github-template
68f3b4efc905416c9df92d23d78d311af9436a12 e2e: ensure cluster dumps are separated by test
1969c792e56c2519383c3b4d06bd2c9c87a50897 Fix serviceaccount name for AWS CSI controller
dc4127ca11f2c3b065852251efd3853a228a6b79 Merge pull request #910 from sjenning/fix-monitoring-network-policy
8ec82738ec21f10c36355ddfd06eae7e29c574fd Merge pull request #897 from sjenning/remove-private-zones-with-force
1de49d0425aef8ea8d1647a72a5dce4aa6d0cb76 Merge pull request #893 from alvaroaleman/destroy-dns-first
93fc22cae6c96e3e9d0d00a12e5686d30af36d5e ensure hostedconfigoperator kube-controller-manager CA syncer uses combined ca to properly support ca rotation. Also ensure combined-ca set in pods service account's ca.crt field
596ede1712ff64c9244380d6612c08d60501e0c5 add release image annotation support for extra metadata that can tie downstream deployments to a given release image
bb3dab61a4032e71c67a83a512f1d1799fa6cdce Add github pull request template
03159df1648c49a09cf4053766ddc6fc7f3f8e15 fix machineTemplate deletion logic to prevent panics in the hypershift operator (fixes IBMCloud deploys)
65d666ca7c9ca1013a0a41dd87da84ae6e5e1562 fix monitoring network policy name
ecf907f6ea4dceb640a58ed5dba6ac81e393807b Improve TestReconcileKubeadminPassword unit test to use real config
291ec25e43ed98d96bfb0e5083f446861f0ed65f Merge pull request #907 from enxebre/fix-explicitOauthConfig
afd0fb5d99abc509cd2e52cc772ea36e4742af04 Set explicitOauthConfig as true when .OAuth is not nil
70ef5fe189b178fe3b12842ad02550ba53785f74 Merge pull request #904 from eranco74/watch_route
d87aeab090692664b8e8468cab23a5b664a82335 Add routev1.Route to hostedcluster_controller managedResources based on Routes capability
a30847fac0e93585550b168df3a01457a17b4c94 Merge pull request #895 from sjenning/allow-monitoring-network-policy
13b16d0fbdf86f2b8b0e7ce84251ab8bc89eacd3 Merge pull request #894 from sjenning/adjust-network-policy
abc85bc3158f4fa5d4dd48b81d519e51eeba334a remove private zones unconditionally on destroy infra aws
27c226932eab0d76d806451b3a32a0f58abfc82e Merge pull request #887 from alvaroaleman/wip
f78c735f8b62ff58e007bc3c7cedb7d54a86c3e9 AWS: Destroy VPC last
a3f4d909ff30a0751341e6ff4f4c101dcf52ad10 allow monitoring access to HCP
c9cbf1b235bba6c94702c6af1066de21b4443c95 Merge pull request #884 from ironcladlou/namespace-cleanup-fixes
eed644559ea88ac3cfafa0cb6738ef7f8c47ebe8 allow custom apiserver port in network policy
57bde242ecca2b2aa39c05ccee2a4436d089f413 e2e: Reduce abstraction and fix teardown edge cases
97de6f506b9355c514317a70e9b3a0d5a4193cf0 Merge pull request #889 from relyt0925/fix-endpoint
e54daea9394bf3a7d632390a935bca130842d337 use globalconfig when specified (fixes ibmcloud deployments)
9ebc886dc367c3c244b5369d65c71dd1c933555f Merge pull request #890 from sjenning/cleanznoes
cdc52dcf0d5fac4d3debbe961b8c10a1a7090cc1 Merge pull request #888 from alvaroaleman/dum-agent
48a691bb139a1b55631cb55a1d5318fa8595144d add cleanzones util to contrib
895b8c1f2f57dcbc5953ab804220ed072c30f0ce Hypershift operator: Add missing watches and unittest correct watches
06122d4932737ca441641022b6146ec8da3482d3 Merge pull request #806 from csrwng/reconcile_incluster_config
5bef28a041fc5b9338dd875bc221f0a7d2a9431e Merge pull request #880 from ironcladlou/hypershift-image-refs
98456ff9ff0c363bb7520842c36cc0fdf5668c0f Dump: Don't dump agent-specific resources when there is no agent NS
cc49602be4c88e86ce9fb97c71e1c93df01a503b Merge pull request #886 from alvaroaleman/logger
61ec59867bb4dd613baf2b8706260010118d54cf Merge pull request #822 from davidvossel/kubevirt-e2e-test
214f9122ee60bdd6e9754dac86000f15c708df03 Reconcile in-cluster config for openshift apiserver and controller manager
4136dc023e9cf73ba7827fd6ca490841c13a4650 Merge pull request #885 from alvaroaleman/exit-err
669d15b6857ecc3e0034d1e84ea6da8d00b2455f kubevirt e2e create cluster test
0f9e74729c88a5a09fbc2435e6b4df13b1ce1fa3 Hostedcluster controller: Don't store log on Reconciler
035862174f71324190521ed2ab0cc5cd300c8405 Update hypershift image reference
476ffa2949421332713a49605e8c5fe4c73c55d9 Dump: Only exit 1 on error
9f730ad442b455207e946c0a5eaf6e1ec7c39742 Merge pull request #856 from sjenning/network-policy
153cece68ee79a5a2e07f4fc92bdbf635af0b607 add NetworkPolicies to HCP to block inter-namespace communication
e784ed2e7ec8081f37cdebe775adfb1145ecd0a3 Merge pull request #877 from avishayt/avishay/agent-dumpcmd
13084acc1460225e4243a51379e97868ba44464e Merge pull request #881 from relyt0925/ingress-operator-healthcheck
36d5fc420ff3dcf68f25621a0b481882b31a30e6 Merge pull request #882 from relyt0925/machine-approver-healthcheck
219b679e10f2bd2d37858d53b541a731eea61d70 add probes to machineapprover to ensure it is functioning
23bc185fc5d22482c678c3261af42efaefb80fef add health probes to ingress operator to ensure it is functioning
71106752a4f2cc97ace5b56a752bce451fa1d613 Merge pull request #878 from ironcladlou/fix-cli-timeout
48f95bf97aab71945170fba18474e3f15b5a9785 Merge pull request #787 from SANJEEV-Choubey/kubeadm_opt
55b0480574d150eeb3c15f2a0c4954caac62ecd1 Merge pull request #879 from avishayt/avishay/agentcluster-groupversion
bf0d7ff6cacceb5dc9423101875f0a15b69be772 Merge pull request #874 from alvaroaleman/limit-iam
dba0707954a0737a17ba512f737a883c35b1af7a Missing GroupVersion on AgentCluster
f2ea9fc0079e3ba58da0526e4f0b2b1175806c17 Fix CLI --timeout flag
f594a45a5942266bfa67be1b9c9c9c42e1fe7e5f Merge pull request #876 from avishayt/avishay/agent-basedomain
3f93a3c48649a5b929c2dc7279e07301856054a0 Generic dump command plus agent support
875b5035f67cb34642154f79767bd275a9a3dc27 create agent honors base-domain
fea72ea42cee2b8e52ac9f85ca706538e8c8eaa9 Make kubeadmin optional
b3b29fa139ed234d300b424f40b165fbafe65db1 Merge pull request #875 from alvaroaleman/fix-grammaer
767e7abff226c8559935a13b1287d377072e1633 Merge pull request #865 from avishayt/avishay/MGMT-8586
0b772c8aeb9bdeb65f9900abcc64bca913191608 Merge pull request #872 from ironcladlou/e2e-dump-fixes
7260130841324fab9ba3ff5748a48525488b6920 Fix typo in README
8c6868d5b822e194a76a5565d3e15e75f673ff60 Limit route53 record permissions to the clusters hostedzones
f563d6d223966ea1dcd0c18f502f03f6fe8c3860 Merge pull request #869 from ironcladlou/token-minter-stability
0cd04f1086e54b492f6a9b4adf09551524814ec3 Add options to AgentMachineTemplate
fdad1b719c59a9bc4da74ae510ff23fdb0b5c0c6 Merge pull request #824 from sjenning/none-base-domain
d0c48422ad89bc808dc84595ca4a057f14a6ab89 Make token-minter more resilient to failures
40d1c0e6e5cfe39f539899f4613f6618feb9f347 Merge pull request #871 from geoberle/oidc-secret
a3b7812c2841d411be3d9458d10e076a7f4e1245 create none honors base-domain
3652cd1d713443f032c7865b3afaaec26350b99c e2e: Fix cluster dump issues
5429bce4390c8b006695150d5d9eb691bdb4bb78 Merge pull request #867 from ironcladlou/fix-periodics
b804e39d1950398e49e1b169658d1080f7c2743b Merge pull request #832 from nirarg/nodepool-cmd-refactor
e7e80dcb1658bd1cea1651e589ba80a96eb8d64a Add OIDC bucket and region to hypershift-operator-oidc-provider-s3-credentials
ae6859e94bb005eaab8a36e1c7530dc3a79bdf64 NodePool CLI: change NodePool CLI to have platform sub command
6a0440636faeb213b57e0814f86e0d69dbc9609e Merge pull request #868 from csrwng/fix_scheduler_probes
51648ffd430a3eaceb306fabde097cfd38f79273 Merge pull request #861 from ironcladlou/clusterversionconditions
23057767f588c02c6e5522a0346159fc5fb89f7b Merge pull request #870 from sjenning/kas-nlb
48da6fd0574f75ef7b746f27666304d5c73a6ecb use NLB for public KAS service type LoadBalancer
7cd9004e34aec7f5f18a3088eb04f2230523e117 Merge pull request #837 from alvaroaleman/io
97bf5ec2d9ba3d6079a9035adb35981a404f23a2 e2e: Fix periodic tests
05e9fb0f4d801ace88974b86d5252ac348c15692 Fix kube scheduler health/liveness probes
4fb80f8e18d6ffc0dad2f17bf51b1e7267f64cca Move Ingress Operator into management cluster to speed up creation
87b1f4bd8873c9d2020774d41f9537286f0bf416 Merge pull request #866 from nunnatsa/create-timeout
a3a4bd924d8b8c4dac1d7fdf9fa8d75d99318653 Merge pull request #834 from enxebre/refactor-reconcile-machinetemplate
294c40d95e4ab583d3bf5834ef424aa2dfed2a21 Add a ClusterVersionSucceeding condition to HostedCluster
52b2efaf762ce2053ecd5b50fad9f10ad8f41d58 Add the `--timeout` to the hypershift create cli
c8758f1bde3c6499e3137e0ede13bcd85a77a4d4 Refactor code to reconcile Machine templates
8f72d20bd9a3d956729403007692acd073541a55 Merge pull request #863 from ironcladlou/accidental-hc-deletion
01c44d81bf4bdb380ddc827b3383285dbab06ade Prevent accidental cluster deletion
c3a576b51f34018d16cd537d3e147d4cb1caca5f Merge pull request #858 from alvaroaleman/fix-wait-option
b5c79110c91d7a2dbd57eb4973ddd7f73de078ba Crate cluster: Fix --wait panicing with a NPD
0c257b9fa95dfb00bf732c35e5eb0a089950d8fd Merge pull request #850 from gregsheremeta/replace-m4-with-m5
a302cd8341bfe9eba04b5c904f1104feb8bc9b34 Merge pull request #854 from gregsheremeta/use-more-region-in-getting-started
9c2b611e5e8f307607853449f1c0a8736bfaa971 Merge pull request #849 from sjenning/rework-oidc-controller
f85b2d152d4ed95f1a9a9d0a30e161548a07121a docs: add region flag to the `create cluster` example in getting-started
1f354fdf76472126b4bad380d5ab3cf4fb6ee971 replace m4.large default with m5.large
e0dcb236be55a2429e1d9c9ad86a927cdec050ba Merge pull request #853 from ironcladlou/verify-docs-edits
14a04902e4070125aa730be51aab48b7402b9efa Merge pull request #851 from gregsheremeta/add-doc-for-instance-profile
dd2e7c8fb3005d0c5043356aea521f2fe1b139a2 Merge pull request #846 from hasueki/vanilla-k8s-scc
f9a09eea77e0ffa9b21d2693d47c7f3bcc8663e1 Merge pull request #852 from gregsheremeta/replace-gp2-with-gp3
eed288c584db5fbb52d3d7bcb76ae9c9dfcd9dff Add generated API docs to `make verify` target
ad3912ab98d44f3c6b0b7ff616febea7610c416a add API doc for instance profile field
17ce8dfd35b79c1f5224b8356234a6255fa5f023 oidc: generate OIDC documents directly
76231cca1f8ca6d39a1782443b9a88dc75b55c7d replace default usage of gp2 with gp3
0efdda785c11ca8f53d905f7d65eeb07ca49c017 feat: Set default security context user for vanilla kube
b489e0bcbad2a999b1424c9333179bef1243ee51 Merge pull request #848 from ironcladlou/dev-docs-update
611828b48392d96e08ba44bc5abbbe9599f4dfed docs: Minor update to in-cluster development registry login steps
ba7ec93536d8397840e2812dc42cdc5fc57c68f9 Merge pull request #847 from ironcladlou/teardown-debugging
ecf13ea66a0eb6677485d77edce7941855b3b93b e2e: Dump artifacts if test namespace deletion takes too long
777ba97b8a6841d79a2d2cc0c662934a91f8c16f Merge pull request #845 from ironcladlou/missing-image-overrides
ab8211759e1acc0eb86e92be044fb15736fe4a0f Merge pull request #844 from ironcladlou/add-to-ocp-payload
76e6de28466035132d61bd10594d11f609de755a Add missing CAPI provider image overrides
e63a6493810233936aead344e37cea2919dd13c9 Add control plane image to the OCP payload
1cb533fa4788b696842ca656fb92c4f8dee76aad Merge pull request #838 from csrwng/update_schedconfig_version
a451775ffbfebf992987508f28fd5e1841421d4f Merge pull request #841 from alvaroaleman/fix-cleanup
b6a72d9f5b6505afa3c3f6cc47ad177c90a3c798 Merge pull request #840 from ironcladlou/token-secret-finalizers
8e50266b6061395ec5b5266ccc4a71731ade3172 Merge pull request #842 from tsorya/igal/multiplatform_image
13c3cd9b4872bc3b6f4104108685e309f390a04f Merge pull request #843 from ironcladlou/update-bz-component
01b7b859dec3bf70fd38fe12f0ae43b517be328d Update bugzilla component to hypershift
7c078f67ffbbec802ec2f446ec5562669c6f4c1d Fix control plane teardown race with token secret finalization
2c275c8d73f4b77fc4afc5003caabc3005ef9a9d Fix route53 wildcard entry cleanup
1b27e14de7232438f496830b08c555f819283a4d Merge pull request #835 from rollandf/MGMT-8604-install-agent-capi
9dcf50e7438961c5e482fcd1665082ff98f06481 Allow installing multiplatform ocp image
2c0499032c58d394b01295428bcccea710ac25ab Update scheduler configuration version
4a4630f8b2eefde09483683c9c6d8b085a8dee57 Add Agent CAPI deployment
3fef5f7461e1763ae641cb3ceeea3260a98361f5 Agent Platform: Add agent CRDs
d3c0601d3ebb42b183a40932e7d591fcb56ab072 MGMT-8604: add Agent Namespace to hostedCluster
57304054e10cc523d2bc8c3ad23372a5eab96f84 Merge pull request #829 from ironcladlou/payload-compat
a624188ed9c7870e6cb9cb8cf4e7a0ae1b6c618f Merge pull request #827 from alvaroaleman/route-53-log
2957c6d44cf4fa59c8eaf407a39f7f02bb61e67f Merge pull request #828 from alvaroaleman/extend
d2ea6db68b2f9be8a1166340d69f218c076243e6 Merge pull request #836 from sjenning/adopt-existing-endpoints
63c0b63d7016848f3128ef1fb889975477da7869 Add support for control plane operator deployed from an OCP payload
f3d3702bc21c8d6d94333088a125844edeca5e92 Merge pull request #830 from csrwng/hcco_loop_fix
4c09342b16cd8ed13bb639fd539a770385822798 cpo: awsprivatelink: adopt existing Endpoints by tag
af6e5207e87247db7db96baffb8e9767cd5c4c8a Fix update loops in hosted cluster config operator
b7631284498523433f6949997fd0f60eaa58e77c Improve logging for route 53 record clean up
ea7c33e42964c862154fb7c37edc8b9c52379fc4 Packageserver: Wait for availability of catalogsource api
9fba0b6ed55808f86b1f9d5d13d2837cf5107b5e Merge pull request #823 from ironcladlou/relocate-hcco
adfaa2d20c6e0aa00db00866b0cfa41400fd9da6 Convert hosted-cluster-config-operator into subcommand of CPO
1ecad27fb28f1d23fdbf7321ef8dd8cb0c6b74ec Merge pull request #811 from relyt0925/wait-for-controlplane-deletion
ec365d73759688a375e80d3c9d58609b9d3332d0 Merge pull request #814 from relyt0925/allow-kubelet-config
a6c7ef84e75eb401b6fc7bd3a2f4a5d0d1ad0588 Merge pull request #790 from openshift-bot/art-consistency-openshift-4.10-hypershift
cb4f19f96d5ec10dfa006d673bbc683d4baad9c0 wait for deletion of hostedControlPlane CRD before removing namespace
7fc93eeb1b952d2840ae4a640d153f0cf3f149ae Merge pull request #794 from csrwng/remove_manifest_bootstrapper
98acb1f8bf5b82baa0fffb3e98a2e3c612c8847a Merge pull request #819 from ironcladlou/update-image-refs
033523a8a1fd5c70234d5756db0812315acd34d9 Merge pull request #821 from sjenning/base-domain-flag
987177b93d4be21af79c7d0371691f1bc74aa793 make base-domain flag generic
9df991ab03767d1e32f97a90d382ad2b3205a9c7 Update documentation for hosted-cluster-config-operator
1d822d24125667ab16728626564c5766264ffeaf Merge pull request #812 from relyt0925/cronjob-schedule
347caa928f9815236cbd1db0ad6539d2ad7d4198 Merge pull request #816 from alvaroaleman/wait-ns
00d26ce29dbb5eae12f1b3b4a9d2fe12aae1cfcf Merge pull request #818 from sjenning/add-tags-hypershift-role
eb0cf007d270a3b05e1c792d1e1104300e1cfa5c Update hypershift image references to new location
20f499c0758df234b7b6c87c98d9b5f40be17d64 add ec2 CreateTags to roles
7b798a1ec20d9709f779b59845d634dc09d8e04f Complete removal of manifest bootstrapper
d110aa30f5174339c16e9c3139c6c4a7034bc0f8 Merge pull request #815 from alvaroaleman/es
ad7bf21cc078248495ae60f708d247adcb55790f Cluster deletion: Wait until NS is gone so new cluster of same name doesn't error initialy
4ee110bc4a3e0adb712119bc448c6bcbc870325e AWS infra destroy: Also destroy endpoint services
7d4fa7c4aaa261c35cc6d0096eec3bfeafc1d8e5 Merge pull request #779 from nirarg/kubevirt-platform
dea6ec3a1c27a4b5e51491076d24e4aca10ec521 kubevirt-platform: Go modules changes
736f588e6c0e372858b8b3cf9c7133a60a2aa8de kubevirt-platform: Add "KubeVirt" platform type to the cmd
ce62aa52330e90d445336e943c5c000190fdb13b kubevirt-platform: Add "KubeVirt" platform type to NodePool controller
6c7851f4f82e0e3aed1b4c963473900326456e1f kubevirt-platform: Add "KubeVirt" platform type to HostedCluster controller
1441f0d10e285b1e2788bd0504889a9ab9aee04a Merge pull request #813 from relyt0925/update-timelines
dd43a7c24a47a311171870973128c687b9cbdf67 kubevirt-platform: Add cluster-api-provider-kubevirt assets
4225750d7ac93e8ce308ad60f117edef10fc8ad1 allow kubelet configs and container runtime configs to be specified now that mco bootstrapping supports it
c0502fea068ac0c076fe29d5cbead21b6f879bde update cert duration to match maximum time allowed by fs cloud controls (2 years)
10f577cd1547fc28de1d743b809546b7e6bc2799 add distributed cronjob schedule to olm-collect-metrics cronjob to prevent management cluster scheduling overload at specific intervals
649df59fddcd30f533bf292dcd141763c2eda634 Merge pull request #804 from alvaroaleman/hypershift-role
c29d00805807825455ac1871831e1adfe07eb497 Merge pull request #805 from alvaroaleman/certs
27c252a207dfe84bdd1b846d796adf7642937b2f PKI: Properly reconcile certificates and keys
bc6e81ff4ea32bcd7c3ac6662ca6b7c18c12252a AWS: Create role for cloud-network-config-controller
d923586cfb28c5fd26fc2f51b02c650566fbf494 Merge pull request #802 from avishayt/avishay/MGMT-8471
e330ef04cde566745134cdb73d4879c84cb5c16a Merge pull request #664 from rmohr/none-e2e
ccfaa6ff4a345ffe2e915d1016405faaa45a85fd Pass CA cert as secret rather than string in capi-provider-agent
d57ed28d4030c07f359d2406fcc014c3f816f9c5 Add minimal cluster-e2e testing docs for new platforms
8a5e225a4c5f90d5e056305c5f7a9b9f2c37eadc Add a None e2e test
23cad550c1113a2abfa6552b4a6705cbfee64ff7 Merge pull request #800 from enxebre/drain-nodes
5eec293d499a8ac67e6b2c7ab892f8b4ef7f9530 Drop exclude drain annotation from Machines
c30d0dd62cee652c069ee72552bcf78fb4095283 Merge pull request #799 from csrwng/retry_vpc_ep
275c9529fc5a8c7c998b53ee8c2008106dce69f3 Merge pull request #797 from csrwng/fix_oauth_container
526e2cd60897d4303451bf18278060ed2c95cb6b create infra: retry creating s3 vpc endpoint
1df13b9cde220c50c80289f6f02cd693013926c6 Merge pull request #791 from relyt0925/proper-provider-flavors
e38ab6f3eb086d243929c0eff4b2d66372f3be5c Fix oauth server container name
6e041118284b39b1a2f49e4542405b2aba6b11e3 add field to specify iaas provider for ibmcloud. Don't reconcile capi components for non automated machine workflows
68ba55db902fd9b95dbb7e850c1c28200d775c9b Merge pull request #784 from alvaroaleman/create-wait
4edb3e38dca01e83c09d2a01986b5d998ac77b1e Create cluster: Add --wait option
b7017289c16fdf928d2ded7ebd69c8dbb21e2a47 Merge pull request #785 from alvaroaleman/dont-allow-create
c2cb4a06b362ae2a88295770bbbb359e9a1aa5b7 Merge pull request #786 from alvaroaleman/extra-tag
2a7a21555a90b02ae02183ee5947be45df9f49e1 Set resource tags on endpoint services and endpoints
db2096cb0ebbc1969a6a8c43f19d681495d1a71e Merge pull request #792 from alvaroaleman/no-name
93c95dba865968731b08bd8ed81b0e516ecdcf8a Infra destroy: Do not require cluster name for route 53 cleanup.
e68665fbdc62729619cd54a530b9c0eae1486da4 Merge pull request #788 from mkumatag/ibmcloud_betav1
eb0b55f1ffa17d2dc3d871dde7c027a59c779f68 Merge pull request #753 from michael-topchiev/liveness-readyness-probes-for-openshift-components
071e615acb15aad3eac83f9aeed108d47cfb3daf Merge pull request #789 from alvaroaleman/add-flags
f645285eef3430edfbf14d0d18258a29732eee07 Merge pull request #793 from csrwng/autoscaler_exception
3c561ebc24ef6309303c030ec3a968238a66a124 Add autoscaler exception to pod crash test
b67cd4c446b6bb3b466088569545e2606425e637 CMD: Error out when hostedcluster already exists
6dd2d2d72660695bf1c90918efbe532875612b6c Create cluster: Add flags for service and pod CIDR
436f0ef72b70361b8e7017f5623f659b2c4023ed Updating hypershift images to be consistent with ART Reconciling with https://github.com/openshift/ocp-build-data/tree/60942ca7fe050ae91646bdfa30329e7c0ea7c84f/images/hypershift.yml
a93b738c8756630f9911fd4623ed8d29e357fc72 use cluster-api-provider-ibmcloud v1beta1 apis
c16455da20c504f6e0032aa93b1892426daa463a Merge pull request #782 from enxebre/reduce-platform-skew
ecaa1bd94b4aff23261d6c8b1e3bb0df5840d7a9 adding probes for cluster-autoscaler
b558edce1af3fbfd9612f6a75555b6b39d9ce0b6 Merge pull request #760 from avishayt/main
77086bda77988516c2136360c33506b9609ebe0a Merge pull request #783 from alvaroaleman/fix-namespace
c812de08fdf35183e50537b4597acda52cb2c2d4 CPO: Fix cache selector for ingresscontroller namespace
95604ccd271c0f3e841b451f90184789e78dd255 Share code between None and Agent platforms
3aaa355308b5b3fcfe85b94fd351dd07c9084542 Introduce Agent platform
1c8bae05456f7b40ddb66628b3e48c39d599ef76 Drop unnecessary platform check
00adce7d48de9ef58eae07f695089ce9597e4904 Merge pull request #774 from sjenning/oauth-route-public
63a6587375ff046bbc8087ba99338a25ee9517ba Merge pull request #764 from hardys/none_fix
7444ef97abf6c194195d0b37d0641c3095472e45 Merge pull request #781 from alvaroaleman/dump-es
27c3431505e28fd2fb336f7e42c3d6b7fb4b66a1 Dump: Dump endpointservice objects
22d2c68d7b44bda9214db4f5b45500ec005d95c0 Merge pull request #776 from relyt0925/no-reconciliation-of-registry
f7cb3ca0752b799b03c3ad82a7491bd49c269fb3 remove reconciliation of registry resource for ibmcloud
b42f09fe6ba180203646ba3b95fff30452fe0e7f Merge pull request #775 from alvaroaleman/fix-servicemonitor
715ea064d8a7fe640f08711185867a7315360f92 Fix kube-apiserver servicemonitor
e67d56bcd52c67ff8cbf749027fb4453233ea4ac make oauth route always public
80e509709d0cf81b4bb906b7b22060520be507fa Merge pull request #773 from sjenning/fix-publicandprivate
d88847b31f0952cca45a807779a3da7f034e3304 use correct apiserver host for kubeconfigs
622af007bfd494abdb62f9a6ea06dfa4067d87de Add None platform infraCR
5b09eb85a1fe21bb094c0fb18aefcdaa186ea59e Handle None platform nil infraCR
8876a9d64ce081f941a1f0709358c383da362874 Adding None platform to hostedcluster allowed platforms
8585a6694069ac963eb3c874a1e4da43a154e0cd Merge pull request #769 from alvaroaleman/watch
271839b90eaa53f51b96dffebc4f1902d7172fa2 Merge pull request #768 from mkumatag/patch-1
396cbabb1a0997a5be26be3957de23aaf950cbba Merge pull request #770 from sjenning/private-ci-support
e2bcefffba847ee74082c5221991fcbb9a722214 add e2e support private clusters
fbfcf63e25fe9893d92aeaf213d7937dad22fc49 Update controller-runtime to fix cache selector option passing
770cc832b2cbd2d894a6c5e857e14177df20e61d Merge pull request #766 from sjenning/fix-private
e915ff1ba2184717a41c618711b2a82eb26166f0 Fix edit_uri for docs
51fde78c8c9a2ec7ab71aaa84c058a41e5188512 make ingresscontrollers and services uncached to fix private clusters
1ee8d17ff6fc4186c454fc6b48be8f438fb5dd10 Merge pull request #765 from ironcladlou/cpo-image
692b6c0e87256991dae45cf4c6f3e7b6a6e7848a Add a control plane operator Dockerfile
6feefbcc71fce7bc34e7d494a5e6eccd85487e2b Merge pull request #763 from alvaroaleman/sane-root-volume-size
a841cdfe9ced1c2e20b62f86ae1169abc97bc5c8 Merge pull request #762 from ironcladlou/private-cluster-docs-updates
454f16a41fb511e78bac6740d0cd9fda19b43379 Default root-volume-size to 120 instead of 16 gig
cff563e1cb7fc4c8724e4a6fa2548821ca9792c1 docs: Update private cluster howto
fbb7e8dd516ba7a1dec65a15f47bcd2c010f5d21 Merge pull request #761 from ironcladlou/readme-updates
ad15878bd82c56c84b7da94b5ab1cf0e82b40a1d docs: Add an overview diagram
068c48d04af9e9b8099064697a3d65ac3aa3e175 Merge pull request #759 from alvaroaleman/prevent-flapping
d3afa2105b5a8312d63d6fa1382c3bee7fad5f38 Prevent flapping of nodepool config
7ce75f4e06624bd491c0e2417b27ca049957153f Merge pull request #758 from ironcladlou/doc-contrib-docs
3865900a80847799a97dfa277942538c42457bfb Merge pull request #757 from alvaroaleman/konnektivity-proxy
a9b098906b12ef2fc3f07918329427381bba497a docs: Improve docs about contributing to docs
5d9b3026e887d234cf64d2f9e12b08795058e3eb Fix konnektivity-socks5-proxy
39a8a150151e27d776481a213d9289dce58f14aa Merge pull request #754 from alvaroaleman/simplify
7306a9121f751fc752751a604276f8e40216da01 Merge pull request #752 from ironcladlou/readme-updates
fb99afb9229771da3faa45a992c00ba9cdeceda5 Merge pull request #751 from alvaroaleman/timestamps
23cfe60a2393c4e8d2fc56a376c9dcd067102e89 HostedClusterConfigOperator: Avoid duplication by using DefaultSelector
2c44ebacb64b09d37ff77a16e7e91c0b9a3d3267 Merge pull request #744 from alvaroaleman/converge-2
2b0d3c62c31bbbf0bacc66f9caff7bee8e523669 docs: Revamp the docs and link to them from the README
13156331014536d901cf2e71c5ec754be0631d13 Merge pull request #750 from alvaroaleman/noproxy-aws
b33a8b4bd7c1933069111eee961a7f063c9d9b38 Log: Use RFC3339 timestamps rather than unix epoch
b65dbfa2a639205a1f3a1f4a186d391117b25865 Fix openshift/tools:latest imagestream import
71f202d72385f53185497b300078a87aca9ce92a Merge pull request #749 from ironcladlou/quickstart-updates
1db9e8d6e439459d86c8eec7f4b1bb438c3d051e Merge pull request #740 from alvaroaleman/avoid-error
4bad0b7f4ce0cb5b6b12c2834e8f63251c56f37f Merge pull request #730 from sjenning/hypershift-operator-sts-token
66e6c05ad6dd1f9a53d4af48fec1f1d5b9592169 Merge pull request #742 from michael-topchiev/liveness-readiness-probes-for-hypershift-components
5029296bf4824f1ae8e1468ab88509b7d3e7ebf7 Merge pull request #716 from SANJEEV-Choubey/hs_cred
d4ab2bce0ef09c72520cc7d0fdba1c2ca064a409 docs: Update the quickstart guide
7514176dd863832e3dc990efef09c62db0ac4c70 Merge pull request #748 from ironcladlou/incluster-workflow-updates
35535674c6907e66804d4a62b31af946fb913708 Simplify and clarify development workflows with better defaulting
a3383d4dcc418abf6ee48ee4ba4fa5a8d5830a8b Avoid "core ingition config has not been created yet" error during startup
f73cbe07ffe8f04eea7b4ae8d5e075958b2a165b Move clusterversion reconciliation into resources controller
f0049254cf08c2423760e480bec490d12a2c41f5 Merge pull request #738 from sjenning/add-endpoint-access-flag
8bf621093483f20ed506d8fe1cec83ef65c0f649 hypershift creds mount optional
f8a81b459de062b120aa8c53370e81a69fa65154 Merge pull request #743 from alvaroaleman/converge
564783ef1a961bc28301f17f6e20c1bc280c3bdb Merge pull request #574 from alvaroaleman/fix-patch
d19eb9d8f9392c654020e8a9f7c66f469f2c677a Merge pull request #746 from alvaroaleman/linting
868bb057c4119b76ec3b4100ea88d55664c92715 Fix some issues found through linting
2475c3b18cb8607dbd76e056cf3b3403bd3111ba Merge pull request #734 from ironcladlou/skaffold
de92f4aa1bd29cf748d3a5f99a588fdadb19a8a8 adding probes for cluster-api
8d02e4c289a2f8661f1b4ee58eaf9d7ca704b334 Move clusteroperator controller into resources controller
d80612d9d46d7e2e98e34e3bd2ffee0d3f4c1ff1 Add more developer workflow tools and docs
e51c66c575c1213ffb9db49d84db2d3c0f7ba983 Merge pull request #741 from ironcladlou/fix-contributors
82b430a167861046ec124cae8626d083c1749b51 Replace contributors symlink with actual file
1dc879c319307eee7cdc075783440f7ec14f8491 Reduce patch requests by replacing SSA with CreateOrUpdate
61785baf1bf56a34be906a5f9286bd895b001bb7 Merge pull request #737 from enxebre/mco-rbac
39c7e8b3cf5bfbb317203a8a964c244c1499186b add endpoint-access flag for create cluster aws
54923b9464de94656f1e1053a4cb3a14391adebf Merge pull request #736 from enxebre/consistent-signatures
efdc151db3ed1c1a586208cceb6e2fb0ec042dde Scope down ign server rbac
e5e6356f097f09df45fa8b777452802b62d457d8 Use createOrUpdate in ReconcileCAPIInfraCR
d334a14224770845e7c1c0ce10985d404e37bde8 Merge pull request #735 from mkumatag/fix_ibmcloud
0175e99f396b3e308fe92b414bde10de0a1a0ae2 Return a valid ibmcluster object
b2681476dda1fe50ad0748f74ae547f2a302a48a Merge pull request #728 from relyt0925/ibm-cloud-fixes
26eaf7416c25c67f611a4766451150ddea5b54fb Merge pull request #733 from csrwng/kubeadmin_password_secret
5c486e73c7304440ff34c06c317d1c28d1b9870c Merge pull request #731 from sjenning/remove-custom-exp
1a6b21d48f93ca57ea374f0035386de22c277abc Merge pull request #729 from enxebre/docs-fixes
50873cabf5973dd6989a4697e9128c0ddf320560 Expose kubeadmin password in HostedCluster status
47f6f1764994906a78894d7ad707e3d50f66d5cf token-minter renews token before expiration
c52b5d02337340a6b76a140ba061da4a44df50ca set ibmcloud capi components to proper v1alpha4 version and properly reconcile infrastructure resource for ibmcloud
af0ba8b339f231ea19f473db55c90f66382463c4 liveness & readiness probes for hosted-cluster-config-operator (#698)
d667330e22f2868c152aff11f87a3202e6d3221c Add projected token to hypershift-operator to use for STS
157c26ca918e69307d887b4783f802fc18510bcf Refactor the ExampleResources (#723)
0f665995ad68d7f4c8625090748c8f386bf373ff Improve platforms docs
54a586055009aeea4e018969c6e9cbf14ab3ba51 Merge pull request #727 from mkumatag/fix_render
619fa67e24a1694b5dc302ef80443a27e7dbc4b6 Merge pull request #719 from enxebre/platform-extensibility
e19504d64f6657d5ba89e016e8f4204759d7b454 Merge pull request #725 from csrwng/replace_konnectivity_user_manifests
8a10ccd80e8c96afcb1bc8035d941aba65b77c14 Replace Konnectivity Agent user manifests
37c45b83f9d453578e05bbd073bcb12437335efd Merge pull request #726 from mkumatag/fix_bug
b5aa26e0c8a0f69431fd727a21a749ebeaa3193d Create platform interface for HostedCluster controller.
7f907394db52b258168981a7ca5275b20fac1b37 avoid talking to kubernetes cluster if --render specified
bc51cbc6060053c2289994b0d2551ec58066a731 Remove redundant MarkFlagRequired check
931d53d86c6608831ad8f94fe35ca249716ab2c2 Merge pull request #724 from sjenning/use-private-endpoint
13b86f0d410389428fc6d9fa7beafda2e07e970a use VPC endpoint for controlPlaneEndpoint with private clusters
91515c7cdbc0d2faec8486aa98dbbb2de476b030 Merge pull request #710 from sjenning/private-cluster-dns
e5fe91137d351821d7ea71438a16bb73361c92f4 Merge pull request #689 from alvaroaleman/cache
654bb2fe5a02b3721fb41f4b4e16b46f13f46d56 Merge pull request #713 from csrwng/refactor_hcco
fd52d5f4b3e372c55532d4e114341a690ae5618f Use a cache-backed client to reduce number of api requests
01a55bccdfd62642d62c1d25759b0c633e5f2f85 Upsert: Add status subresource support
7d51669c34f69ceb6eb6a44f8f594d4137c9e690 Add private DNS zone and CPO record management for AWS private clusters
03af2bff0d528ffc090ecd889c44d114fba9c992 Merge pull request #720 from sjenning/oidc-use-svc-net
28d18953048b8dfaab1bd643e506ffec51080444 Merge pull request #722 from alvaroaleman/json-no
4c0119772150f97719b933d769dfde71dfa41881 switch OIDC controller to use service network to read from KAS
63b4882a100810c2d7dd00a0078021f4e703258b Refactor hosted cluster config operator start code
57041d565c37b1695ae1dfbd60eb4db0014a7f58 Hypershift CLI: Dont use json-encoding for logs
58cabbac00c541b55c7e7925fe7e46f0a55b5ceb Merge pull request #708 from enxebre/capa-image
a6b686d2baa5ea0f96fdf13857bc843ea15ddc45 Merge pull request #709 from csrwng/fix_readme
2cc596b58803ec5d4b24e3c6e4763b74d98d1ce2 Update README to reflect default 0 replicas
94ab101b644735726aafc2e67d1f3e8466071378 Merge pull request #706 from alvaroaleman/annotations-take3
c1d388c6c0d732bb651a6345873ff06b0b23f82a Merge pull request #707 from enxebre/hack-tools-golang-bump
5f43065f72946691ebac15f2edaa8b1dea5a0f24 Merge pull request #677 from csrwng/replace_icsp_user_manifest
708e31e28851f10b64bb73a6708926260074ed3a Merge pull request #672 from csrwng/replace_ingress_user_manifests
8235c661e6bc2187009232d04c477c9460054a30 Hypershift operator: Ensure created objects are annotated to trigger reconciliation
1548e046e980f2dc91f0cfc88717205adc9667d1 Update CAPA image to come from internal openshift CI
00f22cdaa35662b7e16810a03de06ecef3f95d59 Bump hack/tools golang version
7e5a3cf91bf0e3978a5c990a5f642275bb52d83c Merge pull request #703 from enxebre/bump-capa-and-golang
aaf4fab84f7ec66fc231f235211e2a45032b7a03 Replace image content source policy user manifest
0c77b1a3636897f304e9e158540047769e019781 Changes to update capa v1beta1 and support golang 1.17
5cd9ada42d4394a4befd8d928d502ee8beea3f35 Bump CAPA to v1beta1 and deps and Golang 1.17
3a9a241ce045324a52fc542bc3ae496d330429bd Merge pull request #690 from mkumatag/releaseinfo-powervs
0945119c7db030cd5c3a64e384ccb575e07f0dbb Replace default ingress controller bootstrap manifests
905f2510384a28b46947f5e567a946abad8e5a12 Merge pull request #704 from enxebre/makefile-verify-output
626c61f6c8780244546256e80ef289e075fb0c6c Merge pull request #705 from csrwng/refactor_util_config
45029a401b4181956bbb47ff47f2146d4fe2d657 move api,util,config from control-plane-operator to support
117b9cb44511bdecbfb59a42962e55219c6798bd Merge pull request #702 from alvaroaleman/re-remove
8b10204cde3b82963d6c4bebf8d2ecc0934c8686 Print git status output when verify fails
b3b2871549c74a6f072c714754c49cfcf3692f83 add test for the powervs platform
2c7c86927a0d516a8a7233581da86d5cf148bf1a Merge pull request #699 from csrwng/doc_updates
dca82a2daec09b01ffac4c24371131ff8a5b99a3 Update QuickStart instructions
612d658d71b579e2ba015f5760471775d234943e Kube-Apiserver-Proxy: Re-Remove limit
500817357d737421dff45110b23d9c8a4fdef0e9 Merge pull request #692 from alvaroaleman/no-noauth
13f416c464a84b2e84e3198aa5745b14f3a1bab4 Merge pull request #701 from enxebre/replicas-fix
d0b571d5ac7661c2fbc4bb0595afa47534d33f36 Default MachineDeployment replicas to 0 if they are nil
6786c4ec968565c4ebdede2285ebda3343b1ee50 Merge pull request #686 from sjenning/cpo-endpoint-controller
2b6053678be6a04fb1f71bad1bad6b8d005c751c Merge pull request #697 from alvaroaleman/add-ns
d85a730d5778fd218c9efe53e668f9b106ec8b49 operator-lifecycle-manager-packageserver: Add namespace to related objects
e50ea8c21710dea2a4a031da7939039a953b982a Merge pull request #583 from awgreene/run-collect-profiles-on-management-cluster
2dc73d0066ea45618efeda65bf7cc7f515f73b4c Merge pull request #539 from csrwng/infra49
522ebbf4d8145939a5437ca84318a8acfbdcdf89 Enable cluster profiles, remove master label from nodes
29346d9caeff1d87bb73d0e6ea94950aacd03cce Merge pull request #696 from alvaroaleman/contributing
975b1a58c208c0a3ca4dcd84dfceeb579424e430 Add a CONTRIBUTING.md document
3c51b6ff75f74fb4f575743aa83ba43df8601424 Merge pull request #688 from alvaroaleman/create-metrics
0bd8c69da57c1eb9eb7d4badcb4abe0a8f49a02b Get rid of the anonymous auth rule for the OIDC
e267fc38d26768cb3f1b3ba40268d276195f6a78 Merge pull request #671 from csrwng/global_config_refactor
43de60d1603269dbc85f827e8beff092f055b53d Run olm's collect profiles job in control plane
901e4f0d2f04aeb96c6136430ccddc2d733c929e Merge pull request #691 from alvaroaleman/kas-graceful
2fb5dcb993270ad58132ac9afaf16b3e314e0a7c add AWSEndpointService controller to CPO
72fe0d39572dbc0630f5bb3a8e5c9fe639366b7a Allow the KAS to finish its graceful shutdown
80469ce52c44690519b1710fc5ed68094f956790 Merge pull request #684 from ironcladlou/api-docs-updates
abe306569744055a2bb4bd8192d7309725a72514 Replace global config templates with go reconciliation code
96f30e11f134d50585f6cf157bc9aca1025778c2 Read PowerVS images from the release stream
db79df089a76ed19903e71ae754cc0c88dc8ebfd Merge pull request #687 from alvaroaleman/rev-make
2e6b2113460e24bab36844ebf540820bd27f7a54 Gather cluster startup time metrics
6d2365b2d679bd2d99ad9ce983df833fc4e5125a Improve the API documentation
9ec9c3a7a8559c30d2a3b1fc026f80ca2701a792 Revert "Add make to the promoted hypershift image"
7039f790e959f7daab7234f45697b9f6f0fac017 Merge pull request #679 from relyt0925/reduce-keepalive-timeouts
fee248194f96216a06c71a3ea0ff912276f77b6f Merge pull request #683 from alvaroaleman/add-bash
940ca49626b0b113b33b3474084c6f6f86c6afad Merge pull request #670 from csrwng/mcs_config_refactor
7615f2430e6e3a458648f73fb8162651466336cd Merge pull request #682 from relyt0925/no-proxy-wellknown-registries
f3c7bf45e40c60d7f4faf7882b6daeac8161b535 Add make to the promoted hypershift image
2f953568e87fbc4871ea42bf6e1a08c29c7b6da8 Replace MCS config templates with go reconciliation code
1be902f56343bdab5cc6e906139b13939fcf9f0a do not proxy well known registries for samples operator
131e51b157453b67aeed3ac1940fe27d92609389 Merge pull request #675 from alvaroaleman/fix-volumes-2
7dff384a9365f15cf3d317d563247e1c32467234 AWS: Fix volumes by passing cloud provider creds to KAS
bf1675dae8ad988516adbb2bc902a68e8619b2dc added liveness/readiness probes for hypershift operator (#676)
3bd15fdeb3f5e67962486a36330b16f46f680b68 reduce keepalive timeouts to ensure it is lower than oses tcp_keepalive timeout value
4c3cdaf7173cb2a2dbaf414f19515601c47c052e Merge pull request #673 from relyt0925/remove-hostnetwork
6a4a2eb0c4300173cf76dcee53bbb302481bd215 remove need for hostnetwork for konnectivity agent daemonset
a3780ec67527c66596dadbaacc069d58944caf23 Merge pull request #668 from csrwng/ignition_reconcile
8b0b3e7a606ce7fbd87cb811ed8d12aa2b5dfd3a Replace ignition templates with go reconciliation code
2fb6fff4258fe5f5eae7ffe010c6359229a8c73f Switch ignition types to v3.2
ab5c99b29636a11aa9b5dbf25c91f8a438590a9e Merge pull request #636 from alvaroaleman/oidc-bucket
c854b78cff12bfd504a77d69e46c13155ec71d01 Vendor github.com/clarketm/json
5cadb9cb5d691bdc296ce0fc31d343da7c51461f AWS: Store the OIDC documents in a S3 bucket
c105604b03e4424e7685cbd3b194adb9f45456b0 Merge pull request #642 from alvaroaleman/dump-hypershift
64271f366cfa8a933f2c469b27690d9fd6bf178c Merge pull request #669 from sjenning/fix-nil-deref-cluster-destroy
59dd587b99383751e8511f84323242cd3cae026e cleanup GetCluster
c9456943814a4bfb93b216079d8f793a8cb97aa0 Merge pull request #389 from sjenning/hcp-sts-tokens
f8379fbf9634248018d1e986abb145d8fc2088b7 Merge pull request #667 from ironcladlou/api-docs-updates
92bd870ed0c1249fe8ce148cda93b851b8dfbce7 Merge pull request #665 from ironcladlou/owners-fixes
0a3dd12cddcffc194cf75571aee299dc480a011f switch HCP components from IAM users to roles
c99d62e05cd12ad53e4ce45dd43d57034117e52b Merge pull request #666 from sjenning/fix-nil-deref-cluster-destroy
32f870eeb1b4f584ffc1a82fab160cb6f600d522 Improve API reference docs
54bfeaf397a815de0909d6daeedbf81ccce517b5 fix nil deref on cluster destroy with no HostedCluster
0bb7d4f57f8831f7b70f96d08782abcc5ed82608 Merge pull request #660 from sjenning/hostedcluster-validation
e25e1231ead110cbf1c4e98befe6c21d70839cec add SupportedHostedCluster condition HostedCluster
b2f2b1cd30b577265b7f34ec963a2f35067e2b38 Merge pull request #663 from enxebre/infraID-openapi-required
2a512edd11832a4af8596dc180bf21a3ebe39a87 Add bz component to OWNERS
b29f03e889afd95805c7fe238baf4670feb41dbc Merge pull request #662 from rmohr/fix-set-infra-id
c26fe02e7b68819d293feef080843ccc25aec8f3 Mark infraID as required
a9b81317749c66755557e940b7bcf7b0d0d47d55 Properly override AWS infraID if not specified on cluster create
85a35ff1511981b05b5824e6d6aa01c7e872f5c3 Merge pull request #638 from relyt0925/registry-overrides
70ed230a1d233a73bb3555b7d8f8606bdd3d648c Merge pull request #645 from alvaroaleman/indent
9e3c6f8e1dd789ed2d289e166703cdb828477d17 add registry override support to support image mirroring translation in non-crio environments
883f454d85672a4fde42c3274306e66f04152faf Merge pull request #659 from alvaroaleman/apirequestcounts
3f57d4830ea1d7f9217970c0b51cd8a6baab5673 E2E: Also dumb objects and logs from Hypershift namespace
70a75b061b5b366943ef7cc8e9979559ce4c372c Merge pull request #657 from relyt0925/beta-resources
82c122e53b5e46d56074c10a69ccceb2c13db1f7 Create apireqiestcounts CRD
44d1770d0cda425064a29b0aad682bbe7b33c750 move to using beta resources for pdb and cronjobs until all management clusters have the v1 resources available
7be6789815e56636c3a59d55effb6c6913e88bd5 Merge pull request #630 from rmohr/none-platform-commandline
cdf29161899fdf42e4f0655daf988121df1d6650 Merge pull request #656 from alvaroaleman/rework
64d0e4953812a4d410e4c009986f288a4c215af6 Merge pull request #655 from csrwng/availability_prober
2f283fcfcf782cbe0e3b3a384ebe09889e6398cd HCO: Use a labelselector and manage kube-control-plane-signer CM
dd998bae29b5a6fb1ce5a9ab35ec985754191544 Add explicit flags for auxiliary images
9ad95e76c5185ba2272a9737bec03ecf76d3922d Merge pull request #637 from sjenning/awsendpointservice-controller
4f85588cfad79df8fddbed2d97a0597154239ba2 KAS proxy: Fix indent of priorityClassName so it gets applied
69b7568878533568a1df2c49f80581f50df6a77b add AWSEndpointService controller to hypershift-operator
5ff434bf7b06c505548f7d1be2690346f679ff2a Minimal commandline implementation for "None" platforms
6411565039a5d696f6fd8e6113b57dc5bbe909e1 Merge pull request #646 from alvaroaleman/remove-limit
d8c13c7704d8e3af870015360108c56eaec18a88 KAS proxy: Remove limit to satisfy arch test
94fe8dfe2605975a69a15fff4fc215f938cce03a Merge pull request #644 from alvaroaleman/ingress
126ffe57053475f95ea90b6e63446fe1417aaf2a Add missing rbac for ingress-to-route controller
390b8044de9ae8117bfaa24fdb53d7a47174774a Merge pull request #643 from alvaroaleman/fix-ca-2
81609b789a5752c0ffc5e30e71faacbae0c178ce Fix the kubelet serving ca, its cluster signer not root
30f451393f8d683fdefe84f9be1e84ba085c7050 Merge pull request #641 from alvaroaleman/fix-ca
bd97e9252b07181b69f9cada3135b2879f59b4ad Fix clsuterautoscaler command
aaee89ec7f555913950cc027191beb402578dd86 Merge pull request #640 from alvaroaleman/reduce-noice
58ab04bcc3886946a031f3f845120e926023416c Merge pull request #639 from alvaroaleman/fix-volumes
5989afcc05983658fddc2a9075018334debb0b22 Kube-apiserver: Reduce v level from five to two
0973c9952988d55f26864852691153a2129c360c AWS: Fix creation of pre-provisioned PVs
79a4e15e70fa5896298a0417b30c77bfc3d43478 Merge pull request #634 from enxebre/openshift-ci-images
738545296a3a914a920f793f28e8b3ee2b58ea8a Merge pull request #629 from awgreene/introduce-olm-e2e-tests
6127eb6a9977011de62592d05bf8f468c4a04c3a Merge pull request #635 from alvaroaleman/move-2
e5387e033d57ea9f9dd98d098b445dbd7aa33078 Add ci-install-hypershift Maketarget
7dd06ffc3e5fcb1b7bb77ed3690f6d1ea765b44d Introduce olm e2e test suite
e309af1b779e7cc55fe4e005903d6f710b84889c Add images from openshift registry
bc3a26edb7953f88a40e3280f9f95137351f1812 Merge pull request #633 from sjenning/hypershift-operator-aws-creds
3d4f129135fd2d1c0d17cf54b8a9c5ab5c4cf177 Merge pull request #631 from ironcladlou/oauth-pdb
81248f07544229c8f3d6e4a8e10c522c01341989 Merge pull request #604 from rmohr/cluster-capabilities
cf8973570889bdddcec47589fbb5b1567353f6d4 Verify if cluster capabilities match the config
09fb819853c144fbc1229135f5df9d01187918bb add aws-creds flag to hypershift-operator
06f63b869a2d162d64f51a402fd2ee4056f0db73 Add pod disruption budget to oauth server
5a087edec5d85753cda0c521ebdcb7b1349ba719 Merge pull request #628 from ironcladlou/reconcile-util-fixes
172b2df1cc8175ad1c94da17bb9ef356271f6b11 Replace upstream CreateOrUpdate calls with internal utility
e659a40951ae68ce8cf3501b93212ae6361de197 Add unit tests for DetectManagementClusterCapabilities
80bd484053fc228e9a3465c8818e006d66aba666 Move route detection behind a capabilities facade
67d7617ca6ef95f1fa73f7af89c1305593747bdb Merge pull request #622 from sjenning/create-awsendpointservices
9abb849e07188faf216454631082ce5b5a7b7cf8 Merge pull request #627 from ironcladlou/oapi-oauth-pdb
67d23c09d0531cd0fd93f9789bacdf1f48ea6c57 Add openshift oauth apiserver pod disruption budget
da5a27eb0b3e8486fcae631a7a0573a8698f7a0b Merge pull request #625 from ironcladlou/oapi-pdb
3641beddd2bb6431252d8940eb2018b7aa216632 Merge pull request #624 from ironcladlou/apiserver-pdb
d13d9f649928c73b50a840f7e4c2655bee1d3405 Add openshift apiserver pod disruption budget
b9b7e2a7dabad169c390bdf5e8647d37d1f39f96 Add pod disruption budget to kube apiserver
dfce87d62f125a853699a0f35ec1f251982e1f0e Merge pull request #621 from ironcladlou/pdb
2b319ec3bad715aadb36a14801b17485671e2529 Implement pod disruption budget for etcd
40217e2c5224d326d8813139c302613b079e48c8 Merge pull request #623 from csrwng/skip_journals
6f1de2d9e817b9f227676705e7b5c5fa85684ba4 add controllers to watch private services and create AWSEndpointService resources
cb49e2329c04da2f13f4fe6cf3e36d7cf32dce1d Skip running journal dump script if there are no workers found
539a0aa02b0b9be41eb7bd4ef57e146a009355cb Merge pull request #620 from ironcladlou/optimize-api-doc-gen
d72ba28fb41febb986fb8e760a0dd4370215bd43 Merge pull request #619 from alvaroaleman/empty-bucket
a1d4f1deae18151d3ab3ea6facc20c6d1538b434 Reduce API docs generation time by 97%
09b230626f0237bf624e6875cd67eead95ff005c Destroy AWS infra: Empty S3 buckets before deleting them
2b961b57be8e1ce114db82239da3e176a249ebb7 Merge pull request #612 from relyt0925/fix-ingress-check
5953b000e7ad1d0ddcce84a7f3a0dd66c1194048 Merge pull request #613 from relyt0925/fix-availability-proper
742aae0ec8f5839ef5beda3c56a84d994baa5794 Merge pull request #609 from ironcladlou/api-docs-gen
ef59be01eaf193a550ae2d07821f8c715157ea4a Generate API documentation
f2ed3c4bae9f396b98a964f85f6c9c13be64504b ensure specified api port is used across all availability prober images
d5dd1d9b078835ec584b9638cf291c81c5d5d3ca Merge pull request #607 from sjenning/add-endpointservicerequest-type
1cc9c2796fca444c9dc1ccc403b21430ccc5fff9 remove replica check
346fdc270c8649028cf09fa014b1eb61f08ae80e Merge pull request #606 from alvaroaleman/pullsecret
c01d71718df65cbd5d722a7fbb4054fd1876cc6d add new AWSEndpointService type
8de22837eeedac515f30fe09a7830d8a0e515db1 Merge pull request #598 from ironcladlou/mkdocs
e74f48ecd9ae02845dd217bf79acfa8b75b49042 Openshift apiserver: Make the global pullsecret accessible
e668a6ce1e7d4d574c2a599e3f710a25207a6f50 Experiment with mkdocs for documentation
a4fb36bdac5d303c752b2cbb887a2a6e8bb8ad56 Merge pull request #605 from rmohr/no-etcd-storage-strategy
cb3bb2c0777b11ebb272a13233ce025de4663997 Properly default the etcd storage strategy for managed etcd
955ab950a6424af6bb7f2554cd29134d65689d51 Merge pull request #595 from alvaroaleman/job
892d3887488c1dd82da166e3ee78d5287fdf3724 Merge pull request #600 from alvaroaleman/cert-2
4cdef86ccd3e03c715016e8c816a38fcece06fa5 Merge pull request #602 from csrwng/marketplace_catalog_rollout
8a16d2fed28ffc48eb7b54d998e29a48eb86b6c1 Fix marketplace catalog deployment name
cdcc0cbe04a7281a9dd3fc63c0caf1377f68d2b5 Allow to CreateOrUpdate the manifest bootstrapper by making it a job
b8b7c9d6f8604144dc2f690457009e8533b587e6 Merge pull request #599 from enxebre/fix-make
16cfdc85ceacf2936793f19eb7b2c53dd93a66d7 Merge pull request #597 from sjenning/update-staticcheck-target
8a2aeca1239cbf2bf7e9601a96281f0febd660a9 Openshift APIServer: Trust the service signer CA
d2f24a98430e66605c4b0ac38c04183d05dcead7 update staticcheck target with new binary paths
a98c5434bad5d821cd3243d1c23dd7545548af2d Merge pull request #593 from csrwng/machine-journals
18c89b88aec6914c77a962f9a802af5cc3af57f1 Fix Makefile
91f1ed91ab90ea7672d971aa489555432a90e061 Openshift API: Allow connecting to the registry
b71e887d9797497d70f0cee868ba444f62d84587 Output machine journals on e2e
32dcb547e36e7ff025fe865df6af5d1e8d89b2b1 Merge pull request #546 from sjenning/private-aws
40853c7eba47530d9ba61bbe39ad30b9abe55ded support endpoint access profiles in AWS
1fa7c83798de6b1f23924dd75f355850ce6d41c1 Merge pull request #592 from ironcladlou/e2e-cluster-refactor
3a6eb800492a57af16a11b484eb7bcc3195fcb18 Merge pull request #584 from rmohr/optional-routes
9861a3b76b778bebb7f9d2d94b240697681d41de Merge pull request #579 from alvaroaleman/registry
68e1718ccf5211ba5373803c721428dd49904677 Refactor e2e cluster setup code
f4d7c71cd79350841a3d53915822b183f4ec69e4 Merge pull request #580 from ironcladlou/etcd-operator-mvp
6ed882b19b07ae0ffc2482124f74baa97cec7935 Minimum viable HA etcd API and implementation
31ec41b3aa2a670c2a8dbfbe93634de97ad1ff85 Merge pull request #585 from rmohr/none-platform-machine-deployment-fix
4d6bc369e5de30dcd3a9e0971446cf23a3feae7c Let the hostedcluster controller succeed a reconcile on None providers
5d012528e7d5e3f94274bcc9182c2085af0dde71 Tests for route discovery
74a6eceea741a79e37f0c7879c08288d855e3137 Only watch Routes if they exist on the cluster
5b0f4f8517bfaf2cf0172e402263490c841e7253 Merge pull request #588 from alvaroaleman/idempotency-3
9c6556168e3d336545967688c51d823029cb3cb8 Merge pull request #587 from csrwng/kubeconfig_name
1e0c49a613e62af489a72a4c96843d1c6f140fa2 KAS and Konnektivity svc: Fix idempotency
f01be26882d22d7b2216ea770e404ab4d36ea7b2 create kubeconfig: allow name not to be specified
dc9b0dafb3ec68c21a3da25523b7eeaa165efd1e Merge pull request #586 from alvaroaleman/idempotency-2
07e4f1fa4f54619784234ed9d866d10ec8cf6f9b Make management of bootstrapper SA idempotent
b98bc43467a73921891ede7d6477757b647f1985 Merge pull request #577 from awgreene/package-server-custom-catalog-sources
1206aa1a5a865b0d56a4ded60d742d023f0479b3 Merge pull request #582 from csrwng/410_compat
646041ebf4a7a50ea447738e85dc3a82894da4c6 Merge pull request #572 from alvaroaleman/default-ns
74b70c6fbc593e9bc02b389a755408383076a902 Merge pull request #581 from awgreene/update-catalog-deployments
cd3cd9606bbc292ba871f9596f9a0e1982cce8f4 imageregistry config: Don't permanently create new secret
22e79c314df8e510977d79ab013caf8e5854ed08 Convert mco script to template, conditionally include mdns publisher image
a9d2ff74e471fee14036d46fd916c6436f2ca116 PackageServer supports custom catalog sources
24a43f2b1917d15fbd48076b55c0e09545932c68 Ensure the default service account uses pull-secret
aac43ae9a712e956ae221190a3b974ddf0f8c97c Update default catalogs to v4.9
100e58b9f6777f3c7a9596c773dbdfd3a9d6af23 Merge pull request #578 from enxebre/recording-rules-groups
064203c42a25a17e0c11ea166b9445887255897e Add promtool check for Prometheus Recording Rules
f8ece84e6be44cd4f68ac1384951427b5a8b84fd Add hack/tools module
21f5a44a98fb2919195086b51abd2f1bce936237 Drop controller-tools from root module
63472acb3b536a1c2a35b95e8efb4ad4843b3935 Merge pull request #571 from csrwng/fix_nodeportip
9aaf313393e7d2091e37edaa635e07398ad410bb Handle numberic IPs for oauth external address
71686d55266f3529b95d9182d88854603fa865af Merge pull request #573 from ironcladlou/fix-operator-image-flag
d2e30fac0cdcc9d606e892b17cfb977160dced45 Merge pull request #570 from enxebre/recording-rules-groups
7115055cc25b434fa455ce7525f5c019b3c0fee2 Fix local hypershift operator CPO flag regression
d0ee02e1e03e193e34f567b399165099bb8a0a83 Create kubeconfig: Default namespace
199c1568c6d245e92b4f47cc6e7cc660e19e0bc6 Set generic name for hypershift recording rules group
2b3d4bbd04096efb9fbbf7534200c8d95de705ae Fix port range for nodeport-ip script
68fb30a046f13639e9523570b420f1f3779d4479 Detect numeric IPs when creating ignition server cert
33c936ba1cbe5c44108a1258027d938a6737cd14 Merge pull request #477 from hanqiuzh/use-machine-approver
d25f5395541af0719e912daa67d08ad45505f3ad Merge pull request #563 from alvaroaleman/fix-metrics
b6332c3bd6be484b2cd36c0edda1a724a37f2b15 use cluster-machine-approver
03da8592ea894e168e1ef23eb92d2068cf7854db Fix metric relabeling config
f4cd2880f9e888703527d40498b4d35b2b7e7ca1 Merge pull request #560 from alvaroaleman/e2e-counts
1a49cd311cbe0c7a42c7fe5c7c0fb17e6890196b Merge pull request #543 from alvaroaleman/default
c8e79c95af758192e9bd1f7fb0f57c6487e3c3a3 E2E: Verify node count in cluster matches nodepool.spec.nodeCount
82f3730ccad293f57ae5909f09a722fcc03e73f8 Merge pull request #558 from alvaroaleman/fix-machines
5cafe96d1f0fd664a3844a3146bc1bc9e34a3b49 Prevent no-op updates of Kube objects
19c759461bea57f82940d5879edc05d014a9bca1 Merge pull request #551 from alvaroaleman/get-requests
ce0df6f74eae60c06d260d7045593c9c6b3f7f42 Export api request counters in CI
f547aa81b4c596e79cb23140f167ab7cb14bafed AWS: Fix recognizing existing intances for a machine
4741069c9b398fdece75d341402fda14d908b536 Merge pull request #553 from ironcladlou/kas-deployment-update-fix
33ea0eb6f7eac645a5899883f5a6cef01cfb84fc Fix spurious KAS updates
a2eed1b632aa95565fbefc968b7de563f96e49e3 Merge pull request #482 from taragu/set-useragent
0d25a3e92b19cc2bb3e35c821d03099b80eb00ec Set user agent in controller managers - Add user agent to hypershift-operator, hosted-cluster-config-operator, control-plane-operator, ignition-server
4edf06784ebd204941907e26dcf2bc87f2b00d4d Merge pull request #550 from ironcladlou/cpu-metrics
7676a8b2ad47e18912d23cef79932206647014dc Add control plane CPU metrics recording rule
58284c1cfec6e1bea8a59a597cb33f3a44eca9bc Merge pull request #549 from alvaroaleman/json
ada9a42d2dc38b2326aecf211ab021aa1deb5e96 Use JSON-Encoding for logs of components that run in cluster
8c07df94d95a554002841b3c7fcf8f3c0e36a8d8 Merge pull request #542 from ironcladlou/makefile-out-dir
a2185250c7249569abeee3f890b609ea6d718cb8 Merge pull request #545 from csrwng/port-forwarder
1fe09b2470918a34987fbaa4472d4ad9a9ba8e3c Merge pull request #536 from ironcladlou/external-metrics
640da666add959e4da1816de0c50c1445c7b6536 Testing: scripts to setup nodeport public IP
45ce66d4201f66b30ef455ca4c5215dae68056d5 Enable support for control plane metrics collection and publishing
1730ba723988ec22868152fc65204c7743683ad1 Merge pull request #544 from sjenning/pull-always
d70f39416ef6ef6ad7bd2e15bdc505535017369c set imagePullPolicy to Always for containers using hypershift image
eb0c02d3b7c30be272a989347938dca73f0ba79c Merge pull request #541 from alvaroaleman/idempotency
16784f2f3260287c598f91065f943eb65367550c Make binary output dir configurable
7f84118d49253358d4e9920ccac18e2ed81db62e Make reconciliation of user-manifest-konnectivity-agent-secret CM idempotent
c68fe837f68638d683c1c2047deb63ae43b550b6 ReconcileBrowserClientManifest: Make it idempotent
afce271b8fda1cf96ff35ed77afa25d4a0133b37 Hostedcontrolplane SA: Dont overwrite cluster-added pull secret
3d9f85dfcee9edcc3b09ce53a77e9f12c5608013 Merge pull request #537 from csrwng/bastion
c4f32ee1f8c109264bbbfc46a0b4b840f748ebf7 CLI command to create/destroy AWS bastion instance
d16a5adb1baa2a628401652fbdb3b3e649518534 Merge pull request #540 from enxebre/capi-v1beta1
7c7d5a7ce2d63b75fe600af392234c894d69f547 Add changes to use capi v1beta1
d24b3684da40e5e50487a9619ba326578c142ca1 Revendor for capi v1beta1
ed508f81b8e68d60c0ee59d12c441047e28b31ea Merge pull request #534 from alvaroaleman/add-exception
84a83088cb45683f17732d2231b935a59b6d2e21 Merge pull request #535 from csrwng/approver
cdeb879977b559b300cecb3125fa23bc20c4acc5 Merge pull request #524 from alvaroaleman/scrape-controlplane
f64fb2ba38d739823495af6764c924d5e663d271 Add Alvaro to the OWNERS file
2af7cf5982f455eea5f4859498c180c247522ca8 EnsureNoCrashingPods: Add exception for packageserver
4a8e4f07664ab44730e5efd7813f3170da2f031f Scrape metrics from controlplaneoperator into UWM and dump them in e2e
23f88f3efc464babd24bc14d80fcc4f8b73da4af Merge pull request #533 from alvaroaleman/except-capa
55e52e361a435eae34f279868b94819b1e4e27cd Merge pull request #486 from alvaroaleman/immutable
01fa83e012c59567e4aef55933315d62a930a589 E2E Ensure no crashing pods: Add exception for capa cm
cb42acd30c6fec59873f1d9ad720d43ebc6564e3 Merge pull request #517 from alvaroaleman/init-wait
0bfbd33acd6e41455d935ad2a45fe70aa5e83bcd Controlplane: Wait for kube-apiserver if needed
138fb0f473eac40ff43cd12b32c55ce3f1011b84 Merge pull request #520 from alvaroaleman/podtiming-ready
76f7f4ce3c7984dd5db533b5ac8236bbd8f3152a Merge pull request #531 from csrwng/generate_ssh
5cf3fff045ed86ef9c2dd5dfd7b781f2ed7c5dc9 Merge pull request #529 from csrwng/console-logs
aa18bdd0a82fd7d6016a4b932c7afa152e102eb4 e2e: save console logs when nodes fail to join cluster
832d789fb686cb971c170e922cb5e5035c262c6c create cluster: automatically create ssh key if one is not provided
bf07a33d54d3c0edfe5c96a52a6315865de05792 Add command to fetch console logs from instances for a cluster
47dede3c3a944f9ca2963d815a88755de798adba Merge pull request #483 from awgreene/socks5-proxy
8161a0b75dc763868e5d0093b788bbeb7e893cdc Introduce Konnectivity Socks5 Proxy
0c5eef1fc00082ba008749464a104240a08896f0 Fix OLM reconcilation
06df274dfe548343220a9282b91615fed77cfa99 Merge pull request #527 from csrwng/bump_openshift_api
60847b0948d40653eb0f109dc3c1bd5291bff52b Merge pull request #519 from alvaroaleman/better-handle-errors
fe5257b774508667e9f1d744802742ccaea54da0 Merge pull request #526 from csrwng/enable_hostedcluster_dump
8f55021cafc4a3727011fee5b588c3efdf9fc77a Bump openshift/api to release-4.9
07e70acb0d16ffaa8907da38d351c5bc39e6feec Re-enable hosted cluster dump in e2e
76b9f387503ad0db0956be34a813571a129eaa25 Merge pull request #523 from enxebre/cleanup
76e97956fa978b0ce5a398ad64129f6f36220bd6 Remove unused code
a190ecd34242987d528e8aa6296274cedfd67a6c Podtimingcontroller: Track readyness condition
838a8b63bc7d4d805468ff777c9ba9510417cdc3 Merge pull request #521 from alvaroaleman/update-cr
b427cf5dee50a794349f49a59551c49acdee0f90 Merge pull request #522 from csrwng/olm-fixes
3d3ba5b3689859a5b6e4b0df787b76bb4506c2a5 OLM refactor follow up
dd8192da1b0f797b014c931b0e127819c843e14c Update controller-runtime to 0.10.1
9df0222f948a735f0b009259ea63429b66f5d1ac Merge pull request #518 from csrwng/refactor-olm
450b43712adab5580cc88a1796d4e370140be018 Destroy cluster: Better deal with invalid credentials file
ca01b41a715bfd7374109cbe826ec5125bdb5f4c Refactor OLM reconcilation
0a0c2139c5791a4271f53d358a158ae1dcf54cd1 Merge pull request #491 from alvaroaleman/pod-timings
785f4b233f75688ffb82acde334241a4fb2ad33a Merge pull request #513 from csrwng/refactor_config_operator
b0e61e5399e29a8df12c9463a939b634a7a56245 API: Mark immutable fields with +immutable
e4d5a14f0fd73ad20f8f98b07285c829e2ea3e22 E2E: Collect pod phase change timings
81c32a40e35e45281cd87349f88665d9d4947a26 Merge pull request #485 from enxebre/token-rotation
9192198739a0c5ba279dff747ba29a1cd7f63085 Add support for ign serve token rotation
efd7577169a5c148de921e93dcfecd9dc6d4652f Merge pull request #512 from alvaroaleman/add-to-infra
69b26bc9d3f181ed028bf39834320abe5133d950 Add hosted cluster config operator reconciliation
c9af0f31166eb98408c2e1f8718d52baea4d297d Add AWS ResourceTags from HostedCluster to clusters Infrastructure
4e765d41371f7a25d5caa7761689007cde51f88f Remove unused roks-metrics manifests
12c012a1d48c5cce8abfea33b121820057b97fbf Merge pull request #509 from alvaroaleman/tags
ec61a4afa01a0ad320d7f8ab383efb38032dcf11 Add AWS ResourceTag to HostedCluster and NodePool
6e5f517e0c549959658985b2a0c8ce3af66389f3 Merge pull request #507 from enxebre/fix-nodepool-deletion
667353297fc9c2826520d4fd4106c78a5e433f5d Fix NodePool Replace json tag
79b2b1cad275884163bed5600fb5cf98b0a55738 Merge pull request #506 from sjenning/avoid-lookup
205edf8f5138628f605f5f348206537995458013 Delete NodePool secrets fetching by annotation
08f0dce73c5171470509760fb178455d5c7426a8 Merge pull request #502 from alvaroaleman/additional-tags
813b3872927bf996867b9dd3345518ee8f47b1f6 avoid ocp release image lookup on non-cluster create commands
4aeb92bfe211c58d137f6acd0b410c97f2bf08c9 Merge pull request #473 from estroz/feat/olm-catalog-image-cronjob
d3e80fc62ba7bd689812f63468661cbb2f2a6026 Create cluster and IAM: Add AdditionalTags setting
90182e34624b734f91930e5adb172bf35e2e15da Merge pull request #501 from relyt0925/portieris-enablement
68a77a9b858b4d71d79d1a02c0c9c9aa8e756990 portieries support to verify image signatures of images in cluster (important for ibm compliance posture)
913f24ab90feb278b9dcd6dafc26924e7323cb5a Merge pull request #500 from sjenning/adjust-component-priority
00bcf1572a60d313d9c61f518eed7f7c0ba64ca3 apply correct HCP component priority
7818706cc2f74e7db982216220b9725942b7c996 feat(olm): replace ImageStream with CronJob for catalog Deployments
35a343a7760b7273d76da75a6b8ce05c6ce344a4 Merge pull request #498 from sjenning/reduce-e2e-complexity
2dee6e84933db2a0a70cc0966fd26fbf718619a2 Merge pull request #495 from alvaroaleman/support-multiple
811d46e3a0820c8619f819e228e646d96afc35c6 reduce e2e complexity
5cf06ff57c8731279213bcf48a8a8275f9c32e71 Fix ignition config template when multiple ssh keys are passed
32b4dad46561ee67bb12fb824e6757ad5602420b Merge pull request #494 from csrwng/cpo_image_e2e
9dde01175da71786c691d35810e4ae3ff907c7d7 Merge pull request #489 from hanqiuzh/fix-default-volume-size
cf499929837ef1ba91c0708fbfde61519761c7e5 Merge pull request #493 from alvaroaleman/update-hacking
8467a8626c092814c91547f1920f63e000e43cf9 Merge pull request #490 from derekwaynecarr/availability-option
ad4c6e1bb5d6e3695e51b75c5d4f270393813b98 Add control plane operator image flag to e2e
e67db0c131c733c064a1f8240337ed213f8ebff8 Merge pull request #487 from sjenning/auth-token-webhook-config
124fab9c242a4b4cb526443aaab6376e64ea266b Hacking.md: Add missing mandatory param for running e2e tests
483e50eb37ee83ca5e742fd0e047863b02de0e69 Add flags to hypershift create cluster for availability policy configuration
6ff8ff8eb5525468b8774ce615ce52b061120712 set default volume size when nodepool root volume is empty
beae67fbd26559fd24a9a85b2c5073d502b05346 wire up the authentication-token-webhook-config for the KAS
ef3e648b9236e61b0935778e437f4032a513fd28 Merge pull request #422 from taragu/ebssize
bfecb01fe8aee63791ad182d8b533755cf94985e Merge pull request #423 from relyt0925/encryption-support
8054547df1edf383f612d99832179b59cc76b494 Add RootVolume to NodePool spec - Update NodePool spec - Augment permissions for NodePool to add DescribeImages;   in order to customize the root volume, the controller   invokes DescribeImages at some point in the process.   Without this permission, host provisioning will fail. - Add CLI options to expose nodepool volume customizations
19f33f418460358cefcf9a576f7f47607601eb4a Merge pull request #484 from sjenning/cpo-image-flag
f82b00f6a563d1439b0d495872dd35fa9e833af1 allow CPO image override from cluster cluster
f67b30bd9b82359793d06d63ed7f55de1f33d632 Merge pull request #474 from csrwng/healthcheck_e2e
32a29c24ede79ffcd92086be28fea5b7db5cd82f Add autorepair e2e test
b179fd88093ba750ad3e25c7eef68c64b635cb1a Add autorepair option to cluster create command
4e71a9f23c3e272ea52874817f8bdf791a167e9c Merge pull request #480 from csrwng/fix_create_infra_aws_flake
61736f4d43c0d7b4d50d348a0803f049c7803834 Ignore Duplicate permission error code when creating security group
921a45bc9f57810d5a1ce54536eee3565ac40582 Merge pull request #481 from taragu/update-hack-md
ca454c999a1fdaacad98a2fd264b904cfae953bf Merge pull request #472 from enxebre/capi-image
bd65cf0520ac7dc19c418d0bcea223b29a123f3c Add instructions on using private repository
9089e5f19e988edb54d60756f03c72ed6597a73c Merge pull request #479 from sjenning/multi-version-cpo
24cba3416a68ced50654726df19be7a280a931ad hypershift-operator support multiple CPO version
ca0d2a296e38060618d38d4dca2e1c03deab1e45 Merge pull request #478 from sjenning/dockerfiles-4.9
1cca1d1b6adadf33a85dc18bb31f68f625c5590e update base image to 4.9
32c92c7faef8768c5872604dbee4c69aa49945ce Merge pull request #475 from sjenning/compat-4.9
ef5ca27dcd294f8ff85357cd35ffae71d58b2b6e Revert "Hardcode cli/e2e to the latest 4.8 release"
d3eaea9a2fb2ef219f67638abfbdef5e2a38fd78 change control-plane-operator to work with 4.9
12929088f92d4fc7b4e9d9543b8f074efed55bc7 Update capi/capa images
895cf06c1277434498aaa3f20b1ef8e5582c80c6 Merge pull request #469 from csrwng/fix_worker_machine_configs
46ff5e18762b5e7cc40dc66e34cc550c401ad103 Kubernetes secret encryption integration. Adds support for 3 providers: AWS KMS, IBMCloud KMS, and AESCBC. IBMCloud KMS is critical to IBMCloud's Fedramp strategy
48ee2c17cf48d09eb38d543b181dc1ad5cb1c474 Merge pull request #470 from alvaroaleman/wait-status
d0323f85aec1c5ca986179845d5a6feea351cef8 Controlplaneoperator: Don't set status.kubeconfig before it exists
22659c7582f806a72d322f300d4d3fefddc927cf Fix mco/mcs script bug that renders master ignition
f1ee0c4f27269200579a23e8136bbb323122491f Merge pull request #468 from sjenning/staticcheck-fixes
248598181a0e01ce86f59f62f2c226879dae5c65 staticcheck fixes
f600e8273b09f73dd2fc46bd2898db1bbbbd5e41 add staticcheck to verify
1b800846b35944fbef7cfbc53496a3ed590f1d41 Merge pull request #467 from sjenning/staticcheck
dd71a84b2537f4a8e0c7b4dc3767e223798ae261 add staticcheck tool and Make target
fbfc9e831711a8f92898a7cebe8fdc01977bf039 Merge pull request #466 from relyt0925/ha-konnectivity-agent
f2a5a3db8b80477020a876204b1d30dee515edaa Merge pull request #465 from hanqiuzh/default-infra-ha
e15f78fd39cc21cf2be809853ba7bd55069b3a3c ensure control plane konnectivity agent deployment ha for traffic failover
f1004c11b61a27917a329ed74da04615d459a03e set default infrastructuretopology to ha
18120ff35493fc0d71d9892a7356031d34095515 Merge pull request #464 from sjenning/image-to-4.8
4c92ea3248a97f8b5e3610d64520ea07a57585fe switch Dockerfiles to 4.8 base
1a4214946a9b73633971e8baeb391c401568bfa5 Merge pull request #463 from sjenning/etcd-pod-priority
7ac96da165a07c98059b6344dfab2a6fbe877e89 add priority to etcd pods
41d9587c557ddd7e96840b9e3edccd9564ee4621 Merge pull request #455 from enxebre/capi-capa-ignserver-ha
f1335833d2dddaa0dd79bd0ffec07894ce64e35c Merge pull request #454 from hanqiuzh/infra-topology-support
24c138d0a7a38a589a4497d5ac7ecc3b95b35d01 remove unused variable
42c35f4307650e78d4f6bae87905995da4917ed3 Add HA topology settings for capi, capa and ign-server
73b48a41303cd00261a76ec1412ae8aa192afe08 Merge pull request #462 from sjenning/remove-signing-key
772653d7a4fc16722431cf4736ded1ca6af158bd remove signingKey field from HostedCluster
b52c4cc9e129b093ecaab552a58cf5696f8adaf7 set default for controlPlaneTopology
e9d184093c8c5c8e7561cb1f415279ca56af4076 add infrastructuretopology
75ae2fd24bd81f869d0bc99fc8e7823e88e6a317 Merge pull request #461 from relyt0925/add-cluster-toleration
9714d03d1d5972026292152f033d27f5369fa990 add cluster toleration to mcs pod to allow it to schedule on nodes that hold control plane components.
199022ef64b0c643f18840c867a91a252a48567f Merge pull request #460 from relyt0925/mcs-download
0411b820bdfce268a4a6b1496f67e2e7adaa4bc6 To enable tls for downloading ignition this creates a headless service for the mcs that the ign server can reach through https. The additional domains for the certs are also removed as they are not needed.Drop toleration from mcs pod
ba14fce46e097c4e525b01e48c65859e30f012b5 Merge pull request #418 from enxebre/parallel-e2e
d03219e440da8235174e744f7a8d16d2e9a450b3 Merge pull request #459 from sjenning/etcd-storage
0d07d25c90b078cfeb422332feeaf3b0ba825365 allow persistent storage for managed etcd
cc8b41468e03aeeac31765c377715c3bd175d85e Merge pull request #458 from sjenning/konnectivity-route
97f069d4684d32b23795d01da973bee81eb96eed Run e2e tests in parallel
fdea1fb9cd3b3fba7ce74574e5f8358c6c3c367a add Route ServicePublishingStrategy for Konnectivity
baceec23098d39af089b06c503425c3bbee554d3 Merge pull request #456 from relyt0925/fix-configkey
2f2ddaa6f72fd075380c548d21a707ac619ac790 adjust image content source policy support to conform to new core config validation standards
c55a88107a53158a374bfec7ff5c1bc01c923fa4 Merge pull request #449 from derekwaynecarr/broken-upgrade-test
aa6bf50a791a4c3a7a79ba6d343f59877d2d3b29 Broken upgrade logic test
e633c5d8f9d0f7cb7b10d8d17afe0045b4919248 Merge pull request #357 from enxebre/core-ign-config
9c6d07b1a9013934f5fd40509895e38f7e264997 Merge pull request #451 from csrwng/scheduling_fixes
6f5f240e9c657e54a9dee8594fb9913e54e04a9b Control plane pod scheduling fixes
4bdb965d75f691884a0170d3555da3ef78a946a2 Merge pull request #447 from mihivagyok/konnectivity-duplicate-config-fix
39ff0d7207c22b0d1372074af8e92444ab3f466e Watch ConfigMaps for NodePools config
d4dcdc4708ff1b7fe8f925bee62dfb5ecea57044 Move core ign config into NodeNool controller
4863c143a3083945853c1788671ceef9abfbf521 Merge pull request #448 from enxebre/enqueueNodePoolsForHostedCluster
71b7ba9a1e2a000d72faf45f44689d33a0793691 Narrow down enqueueNodePoolsForHostedCluster to the HC namespace
2fdb9d8662654a11e4b11760f5364c08e5044a7e Merge pull request #446 from csrwng/operator_deployment_scheduling
49df5a415139c0b75d3285573b0a4fe108f15478 remove duplicated mode option from konnectivity server
b1956b821012368d2c6106cc7f1004919738b88e Update deployment scheduling for deployments created by the HostedCluster Controller
bd0715270c7a2646e4339f2222d210237b05f39d Merge pull request #442 from relyt0925/one-replica
cc6c8e8eedbecb50d718f39f1c61f86b136dd2d5 run cvo with only one replica and account for multi replica deployment without rolling update params specified
d63c0f29919c8bdec4eed416b3f4b5080f6ead6d Merge pull request #441 from ironcladlou/vendor-capi
8ce4ecb4a85d232956e290af4eeb31ec006e9554 Update vendor directory
c0eb13ce5ad24997ef886572d84afcae78787983 Vendor third-party API dependencies
64315a851a64c05b355a037e9517393e90a707b7 Merge pull request #443 from relyt0925/konnectivity-priority-class-fix
c9cf6e17a04935d505989deffdde06af4806c7d4 adjust in cluster konnectivity deamonset to use system-node-critical priority class and not control plane only default class
96e8445edbb970c5fe2e7159eb9e2328ee072aad Merge pull request #437 from ironcladlou/unmodule
addf73fc5c9efb5dfbec4c23f9cae7b0f2d433ce Revert submodules
9e6982f7554ec10cb2e6666a804f68601e7e89ef Merge pull request #438 from ironcladlou/consolidate-e2e
b6c12f8b960d55ede43966b702126970be70b4ca Consolidate e2e scenarios into a single test for now
d5d4a7b4886171280d664c0bac6bfa1e096946be Merge pull request #403 from relyt0925/konnectivity-proxy-oapi
8e9ed1d91a984b6f57c1d90d79960ad84fc18ea3 Merge pull request #420 from sjenning/priority-classes
c504acacaaaa77d838baa0a692302f7535cb2341 Merge pull request #419 from sjenning/staticcheck-fixes
0f530633061b87f5720c0b7519f4ac3b01bb3da0 addition of konnectivity proxy to openshift apiserver to properly process webhooks/in cluster traffic
c92fe2f34c49a81153b6ec575fd41e6f123f9c23 Merge pull request #430 from csrwng/kas_resource_req
b3774e43b2999e7554f09992277954a234d8198e cleanup: fix staticcheck warnings
39aa0a5decdb079ba77e5712c89861f26bc9897f Merge pull request #428 from relyt0925/add-imagecontent
5101aa61d2000588ceb52ed248d0e37710875adf add support for hosted cluster image content source policy. This allows mirroring of release images to other registries besides quay.io
df7d8347d8d5bb76f344d0b355414fb69fcdffaa Merge pull request #416 from csrwng/refactor_cvo
027680d71dc636c7b5b5d13b83baafa56447ad1d Merge pull request #431 from ironcladlou/support-module
11e4f9da0343db537cf47cd6b8b49a6f12b2c8c8 modules: Clean up support module usage
82efe088c993c8697462cc3b230078950e2a1467 Merge pull request #425 from ironcladlou/submodules-2
854db1f82b00950ae247048aab7f6bf105bce382 Merge pull request #429 from csrwng/fix_48
b1a164236899b141cf529244a0db6cc16c432540 Preserve Kube APIServer resource requests
d7c2eeda5b29cdc7c912b85d2a9942120392fa83 Extract API and control-plane-operator into Go submodules
52cedfef7461ec957599d41949b30d8853950990 Hardcode cli/e2e to the latest 4.8 release
7c1fefab59e758c34d53541b35b166d78cb490d6 Merge pull request #421 from csrwng/control_plane_tolerations
a424cc272d2f0fd54483f05668fcee27da02c344 add hypershift priority classes
63cf115c88598026772619c505fb62fe2bc1585d Enable isolation of Hypershift Control Plane workloads
4190c8b9f3433b28b22db922ab6434873f2b133e Merge pull request #413 from relyt0925/configurable-images
0f80bb8ecfb7f1fb3f32f41cbb96311f694cbd3d Merge pull request #393 from csrwng/nodepool_defaults
6c085686707148648570bd61691d53032535c007 Merge pull request #374 from enxebre/autoscaling-e2e
3997f1aab9016e6e4e61babb80af7153a307bdc4 Ensure cluster autoscaler and cluster-api manager images can be configured. This is a temporary workaround necessary for compliance reasons on the IBM Cloud side: no images can be pulled from registries outside of IBM Cloud's official regional registries
f45f678386925f6ff7d60d3ecee899a7a05ba713 Add autoscaling e2e test
9f1b42e90dc54f36bfe9b6a2e41baa293835f468 Refactor CVO rendering in control plane operator
04dff9084c45d5bc74b35dcb793c6c61c7e7a527 Merge pull request #407 from relyt0925/livliness-probes
ab3933415124abf2c69afd28f98bcebe68b867de Merge pull request #405 from relyt0925/restart-annotation
e9b179abe86734f450197733fb83498fba69fee5 adjust resource requests based on values from running standard sized ocp 4.8 cluster and ensure critical components have Liveness and Readiness probes
684603343666f7037b9885bc74693e9ead01ce04 add support for rolling restart of control plane components through restart annotation
eb369f05255a61e287478fb45c5943f48aa2f503 Merge pull request #404 from ironcladlou/colocate-components
4c3ad7d95c86190befa80a3e3a34471bb0747f5a Prefer to colocate control plane components by default
257cff17da76efb91294a96836948f11ec3374c1 Merge pull request #402 from csrwng/multizone_spread
e7025173f4a9fd8c9e05d3f299942301a5a87704 Merge pull request #380 from relyt0925/add-nodeport-support
4ccbc964bbd69b84cf1c744f106960276b42ba32 Use multizone spread anti-affinity rule as default
a42a44b61d90f5186cc0fb250049a91499b7ea5e add suport for exposing ignition service as node port
0815c7a506327746c6aa7ae646569af8f3bae358 Merge pull request #387 from csrwng/registryclient_provider
1f4b9fa73cf2968534d74ddbe235b7e5228d0c8f Registry client release info provider
2ef3e1348080c63ae6955050f623855aafde9d71 hypershift create nodepool: add proper defaults for AWS nodepools
beca991c04ada3fe26520be501a112d0ae847568 Merge pull request #392 from sjenning/docker-build-fast
b7566016fc3a287435f32d625abdf447e458e301 Merge pull request #391 from csrwng/releaseinfo_provider_pullsecret
9ee69e98c0ee1090194e913ffe08c65b9881ecdf add fast image build for development
14e68b94aabd569cff2f011651192b304dcbbea6 Merge pull request #367 from ironcladlou/operator-status
19bdf8461685f7afdee8687799f571d5fa241b70 Add pull secret to release info provider interface
b4bdd226e2fc7bedf26654dd589c27e1e133a7f6 Improve reliability of release version rollout tracking
3f1929c1cb5602c63cf4469192c3acf21c7cb0e3 Merge pull request #388 from csrwng/move_releaseinfo
7366356c89efaa2940b4fe2db0f1f6b1ce31efb6 Merge pull request #390 from ironcladlou/remove-mco-dep
c7985b38a472ca2006c91bf94f18715e446620a0 deps: Add MCO type to thirdparty and prune dep graph
466e60674b35fa89238fecad860cc52d307e6024 Move releaseinfo out of control-plane-operator
4fc9a8e2c9ecbabc9b1671b4c55951bae6cb019e Merge pull request #384 from sjenning/none-image-registry-config
c2a5c065eb1b63d047afc5cb3c7ed5b5484fce95 default to emptyDir image registry storage for platform None
529e1a07319a28d1d4304e60fdcac4e4e7091397 Merge pull request #382 from relyt0925/fix-catalog-operator
3f7568e8daf60908ed588440e8382fe754a21903 Merge pull request #383 from sjenning/platform-none-ingress-endpoint-publishing
60a211880a2022bc84b27800373e8fd036ad5776 fixup ingress cert plumbing
8a8e1a4507861f7ba04d679c680c7216cde40025 remove dnsmasq requirement
8027f3452e711dc4923988f9b1cbeb9b2dbec19d Merge pull request #381 from sjenning/platform-none-ingress-endpoint-publishing
aae990cd495f44cc38fcc71980b3aed8a70ae3ca use HostNetworkStrategyType ingress endpoint publishing with platformType None
a78aa6b1e2f536cbe6b8f915c5ac5a0969f96119 Merge pull request #379 from relyt0925/add-resource-requests-1
88ed2a816937375c4d7ed278b6dcec198f77fc2f add resource requests and enhance livliness probe to issue https request
c2b188e4e5d7217fd6c9b5a008045a012c2e0dcb Merge pull request #375 from relyt0925/update-priority-class
824424418f8cf621168f745c8b2b3d634190570f update priority class of kube apiserver proxy and add a non root security context
73462c9b5a6313aa810db4005010a48f4f2b4817 Merge pull request #373 from relyt0925/priority-class-kon-2
114a07a551907601f7c59d2431882ebaeaf421ad add priority class to konnectivity agent daemonset
42fd20b1792468e0ea41386d0f08644b2d8aec51 Merge pull request #372 from relyt0925/priority-class-kon
83b1ae77b914545244daf215d63961e9ce3db5c8 add priority class
cfad8946f5c73aafd7cc2b774ec7722ad2f56f47 Merge pull request #366 from relyt0925/add-leases-rbac
a466dde8cd584439e77899dac0051242116be43d add leases rbac for leader election
de9cfc23f1c1f5bc0fc40c21cabf93d96ba1c1e4 Merge pull request #361 from relyt0925/konnectivity-image
9f64a30c6daa872febbe9a60fa97bb36e23d7080 add konnectivity image annotation to allow the specification of regional konnectivity images until the image is included in the openshift payload.
f8e378f42697ea503dc49336ec1a5c7167b1364d Merge pull request #360 from csrwng/fix_registry_iam
31f94f75b72ee9c3b6531ec9cbb76da3cce2b4bc Trust registry service account in STS policy
f4c19a7943d9be66da578762e4063bd15f648af6 Merge pull request #359 from csrwng/fix_builds_service_ca
fb43a54328f073364bb13ee62b5db898a710a16d Fix reconciliation of openshift controller manager service ca manifest
e1ed769119e61728335d0165e7d605bb20776594 Merge pull request #356 from csrwng/kas_endpoint_api
b43120df16496abc57a02f5bd776b399a4aba0c1 Add support for specifying Kube API server advertise address/port
d682f45cfd6f6dbffba353b2b8631f874742870a Merge pull request #334 from relyt0925/oauth-identity-provider
0cc7fd246274c90d47a62506e4b0ce4149e94024 Merge pull request #355 from enxebre/tests
05aaffb59b410f56410723c463e82dd342a6726d add ibmcloud oauth config overrides. Enables IBM Cloud Red Hat Openshfit integration with IBM Cloud IAM. Solves https://github.com/openshift/hypershift/issues/224
e2c50612fb40dc6b57817b447475e6bb595e9ffb Add unit tests and config validation for NodePool controller
1e87ac13151c506f1a6b970988291a55236c2b54 Revendor
8befec266097ffa0ea17530890b57ccbd97e4a68 Merge pull request #332 from enxebre/refactor
a86c74d2528991839e09725660b56dfa5fddbca3 Merge pull request #325 from csrwng/global_config
7748f085d6a345f2054473072bd5cd522206d27a Implement global configuration via embedded RawExtensions
e5b684ef80c6e50daf4ca62aac6f2c223eef20ac Refactor NodePool controller
4efcd2781f0a9501eab98c9d077dcb09e4c7680d Merge pull request #352 from csrwng/pull_secret_in_openshift
b45ac4562cde0aa3273da8f28363cb8f92ea82f3 Merge pull request #331 from enxebre/upgrades-api
f88137e20839255049eb987909719270303fdf89 Expose API for upgrades in NodePools
fa81bfde8dd37e8e41ffa6e999be60200fb75bed Add pull secret for out of box imagestreams
f8225f23476f0f4a825bc9dca8fe30cf26062165 Merge pull request #320 from enxebre/machine-config
87bd754d9dda516acfd7c12a92c74c1e7a49ab74 Expose machine config in NodePools
5d4282c93d7c77bf01c2f2c7552512a56b3225ba Merge pull request #344 from sjenning/add-fips-flag
92395c71720e3ea4b8318289401e0524906ae8f3 add FIPS flag to create cluster command
84ada8d09ee2a8890a58e3ae4031494916f3a0a9 Merge pull request #333 from relyt0925/network-type
c5e31f2916e069a82c9bac4e7a6718690c3ac962 Merge pull request #342 from relyt0925/konnectivity-ds-nonroot
756321d18ad0fe92796fe8c598f94200fd8dba0a Merge pull request #211 from sjenning/fips
0ecc69129a1d642d221db637862d3803a2160930 Merge pull request #340 from csrwng/separate_oauth_cert
2cee2f06d6928b237b700cad591338a59caeb63d non root daemonset
ab49dea36356a0fd8323b410685e5753fc60f5db specify intitial network type support
db8578b56933074b6e6a2784753f0239241ef27d add FIPS support
07270990bbc26c9d68e608e7721798193047bba0 Merge pull request #338 from ironcladlou/upgrade-e2e-version-checks
034d8f25298c7013750beafc1731263d81dcdf58 Create a separate oauth server serving cert
1abea454ba6574b1f98693a2911b65f755d0195d Fix version reporting in control plane upgrades and add e2e tests
59de57094536feb3d63257db8d85be30222110f0 Merge pull request #339 from sjenning/use-ci-konnectivity-image
76f61fd9202f70f94b0af4b3cb9f97b2cdf173d7 use OCP konnectivity images
175e3f057c1e704f972618c51b0f95a696db5dfa Merge pull request #337 from ironcladlou/upgrade-test-improvements
7b2d01dc2dade7c2763cedea8975fa85025ad1c7 e2e: Improve upgrade test assertions
53504eea6359d5fb5b69153eb51ac00336ad4131 Merge pull request #336 from ironcladlou/artifact-fix
f625fdad4587eb6d770a1caae24e37a4a13b3cef e2e: Only dump guest cluster data if artifact dir is specified
2ae11d1aa099f727ec81c18e10f6dcd276302d4c Merge pull request #330 from relyt0925/another-nonroot-pod
f4042b0dcee1fa3a2ebd069638a4a5336dda2039 ensure control-plane-operator and hypershift operator are nonroot
8ee30bb13f494d228208828a95d6de3c2c93147d Merge pull request #335 from ironcladlou/enable-upgrade-testing
e3e8ac7f82d72aeafaafe290e792ed4515dfa174 e2e: make upgrade test enablement configurable
dddfab0cd9ff20c6bcaed9bc35525e018b708e5e Merge pull request #326 from relyt0925/disable-bad-deploys
b658b3f52d8a4327c18b4f698299666a57bcd74f enable initial deploy with proper image to not have a dependency on image imports
88ec14b8a31856a398b2ac72a27dd2c89f32e253 Merge pull request #329 from derekwaynecarr/fix-reason-typo
379d4c9848a55535be8a448d45d4a91cab46bcd6 Fix typo for UnhealthyControlPlaneComponents
6215900baca77887f5120da1b83f96bb1e3b3603 Merge pull request #328 from relyt0925/fix-nonroot-container
926e10128d775a9cb94109ceb4273ba0aef506fb Merge pull request #327 from relyt0925/stop-deploying-dead-pods
23868ce0df4d07d336d6dc765c2e9b99b71c3467 fix nonroot container for security
d4c8ac0b016c799351ca9dc5f31f8c2bbabc0453 only deploy aws cluster api components on aws platform type
3f66af62a7ac4a7479a31bf13c0d20442b203c6c Merge pull request #324 from sjenning/remove-s3-buckets
0e1253ef829ed6ceba0d7a77a6ccb9cffd6bf1b0 Merge pull request #321 from csrwng/refactor_ocm
d1c6188a6546acf6f5439ccfd786aa37c1a3469a remove image-registry buckets on destroy
7800b3d413e498060e345ccfca211123ba8de13f Refactor openshift controller manager and cluster policy controller
d2352ffdc816ccddb68e8683d6b7e06fa195f1cb Merge pull request #309 from sjenning/remove-openvpn
34456f5b62be8622a66379e4ffd57d921c57d907 remove openvpn
72ec643313c67c50b25e5c04ad572a559a1c064e Merge pull request #323 from ironcladlou/e2e-must-gather
5dc20389a9330bf418e327832c16defa4b470731 Merge pull request #322 from relyt0925/disable-pki-rec-annotation
af1dd8d9d09ff878b70e507c4efd8b7be0aa86e2 e2e: Refactor and improve diagnostics
3da459796addc7a2c565e5380f272bc9b9c070ae add annotation that will disable pki reconciliation
8aa56bcad43dfd7fe01157d9d5bde36e3f3cf873 Merge pull request #319 from relyt0925/quotename
9c3e2598a59fee1b856aa51bcaa91c3556301b2f ensure name quoted
b513732c5c7656bfc537bf8168180ad98a6fea3e Merge pull request #317 from relyt0925/reconcile-oauth-clients
e82c1619b8c3331d93cd76c32f55d51ef477633a Merge pull request #304 from enxebre/ign-proxy-to-server
9adacb4a2aa3b60f59ff1034ae29f8b16e3649c3 Convert ignition proxy into a server
22e0133566351af643087332ddf6f0e8cb4b1ca2 Merge pull request #311 from jwcroppe/fix-readme
d6c7c29cae7ae2c69c1ff101f747598898599e99 ensure in cluster challenging and browser clients reconciled
c83cb9407435dafd4d372a67dc15ed90c6ced612 Merge pull request #314 from enxebre/hcp-Initialized
df1f1e471d8829f35033bee9fefac3cbbae11b46 Set hostedControlPlane.Status.Initialized = true
6c66a6b447c0fc3382e47f7531491c84311cbb8e Merge pull request #312 from ironcladlou/etcd-status-handling
2e7dfca5c83f55763af197f48b1768a9ac3ce107 Fix hostedcluster availability calculation relative to unmanaged etcd
b782191ddb75d45b47a4809e3c25506e8f320062 Update README with latest spec structure
a34f1881abe0730c0736ee4f8dee7d05eb0eece9 Merge pull request #305 from relyt0925/unmanaged-etcd
9f12da6341b36fdffa6ca187c37904c208da6b93 Unmanaged/Managed etcd configuration
22ebe6637bdf56638efe45e78e18bee6671145ad Merge pull request #310 from csrwng/refactor_oauth
53a2d0322eea5b864a52ea070ec065eb1642dc02 Refactor oauth server rendering by control plane operator
8f0d9723927ed4454441c165c6c9040cea479daf Merge pull request #307 from ironcladlou/cpo-etcdcluster-refactor
e2841b137b082f7b369a8526969c09e993bbe74f Merge pull request #308 from relyt0925/fix-ingress-resource
4f79cf07732949aa5fae9941f56e68c24aae108e WIP: cpo: refactor status handling
3881b4bfc830f476a9fb5d01d8603a00413f440e Merge pull request #302 from sjenning/konnectivity
1fba1a68393015d0ab802b04a35cae097189ebc2 update ingress fix
6418d2dc5aab3dfec7d87170a334118135fd05ce enable konnectivity
c712bc64482f6b57f08c5754d8c1d7b9086e02c7 Merge pull request #281 from relyt0925/api-auditwebhook-addition-proper
69cba2337c6ab0d2181a933004d017f9d46f2b8b audit webhook support
654d8d7fa105a4c967b61b7c32664fb43a29a7a1 Merge pull request #301 from relyt0925/project-add
f87bd6d29a6d0db28862b45625d5d2fd9c5f78ac add project group
6966925ecff2cc9cacb31e1cfe62811404606fa2 Merge pull request #300 from sjenning/konnectivity
5c58d9711893f2144729bef18ff9df2391383e7f add konnectivity agent to hosted control plane
0b28e7353fc79165651de2baae55290e842c7eaa Merge pull request #299 from ironcladlou/e2e-timeouts
31470d848a939320f8d9ff91b0527f412373fa0c e2e: remove explicit fixed timeouts in test assertions
8e145f67c1e86f92cb0673671be2c3482ca66727 Merge pull request #296 from sjenning/omit-e2e-image-build
dfc67a8fc071a9c7bd192eca0699092ca4f3a3c3 Merge pull request #298 from csrwng/fix_infra_warning
1307f34d43bfbbd2c09c0a73f985885487a65562 Merge pull request #294 from csrwng/refactor_openshift
95ab557c21134c3d77f9d8736bcbf25e431bcc88 Fix warning error in infra/iam destroy output
2e9d5d2aaa6c1756d4c333934bcc59b042aa7e69 skip e2e binary during image builds
960760047d25481355951f16a41a23531be64941 Merge pull request #293 from sjenning/konnectivity
04df49e7355c76087f1196961550d42d226063b6 Refactor openshift apiserver, oauth apiserver
f5eb3ef0810ce6e9814c928c73aad35efacea02b add konnectivity agent to guest cluster
a5a2acaa2f14a6edabde78e3d0f012a58cfb6bea Merge pull request #287 from enxebre/pin-thirdparty-release-images
01d5c88d78b7372e0d955454be8b1541b9f697f4 Pin version for third party release images
bfc0f680c13d8ef4adc24214ec19e4592574b6ba Refactor scheduler reconciliation to be stateless
62584026daf92274277308985ca6de904aaea4c8 Remove unnecessary scheduler manifests
c1069d564bc7c9094b21bce8f2a8846564ee5394 Vendor kube-aggregator and OpenShift controlplane types
fa453498fb91fc2764dd6ef32f65531fa316585e Merge pull request #290 from ironcladlou/otel
dea5e3c86495cdcc7b1e79bdadba7fa4f061726d Introduce OpenTelemetry tracing support
1230dd4706ff8a394645f0976ced121318ddfeba Merge pull request #275 from ironcladlou/ign-auth
0d9d48742041e768b3127434aa2114cbdb0f4d2c Merge pull request #289 from ironcladlou/nodepool-defaulting
55f5953f3d803a1c21377cc33924265d4da3b18f Merge pull request #288 from ironcladlou/release-image-lookup-fix
18948d98162f8da487b2869b58b8a2fb27b57d3f cli: always create a NodePool with the desired replicas
3588145398178eb1746100020eafac271e3010fa cli: fix release image validation
37dc8c91af6009e1d24520dd4dc0721d600fae0a Merge pull request #280 from sjenning/konnectivity
9d4b840ea172a8830b37eee72ab48a9378b21e3b Merge pull request #282 from relyt0925/small-fix
5852b02e4adc843cf09742aa18a421de485ec113 add ibmcloud cluster providers
a20392c592f83d23df910f0dcacc1002b8c275bc add konnectivity-server to control plane
034f5dd8cbab5ff66192835724bf9f1fd8623e77 Merge pull request #284 from relyt0925/olm-fix
8b42a0835aa34f1ce19a64dffb08c58cefc23f9d Merge pull request #286 from ironcladlou/fix-image-lookups
f3d1a4baaf21ff18969c4671bdcc1ff35199d4e4 Fix broken OCP release image API URL
2d2f598fb50bc7d9017a0bfcad92083b5539292c fix olm deployment
04e0ad5b1f68ea174f22be06e096908d15e06da0 Implement ignition authn/z
e0d222aa3f60d061ab545f4ede02631d1eca9ae1 Merge pull request #276 from enxebre/clean-up-aws-api
1fe1b823bad1bc310d05ef93f33303b732da6ddd Clean up AWS platform API
64958e3a768b9c7b6ac6435b55910f3d3bbaad56 Merge pull request #272 from enxebre/aws-external-infra-clean
0ef36e111b7ee893474b169ab3a2a52638a70ba6 Drop ExternalInfraCluster CRD in favour of AWSCluster
c35b217329eb32f06374e51058d98c05006cfbee Merge pull request #274 from ironcladlou/move-ign-server
d74122f6037ee951550ad1cf9a9310b4d0d8b1ac Bring v1alpha4 CAPI/CAPA and drop externalInfraCluster CRD
ef947609587ae097b3760c7100490a71c0c8cf83 Move ignition-server to the top level directory
0497bebd5eae1928e7947eac40ed8e753dd4e7af Merge pull request #269 from enxebre/ign-proxy
62b597ed8100615c40aeaad47df7ca4831ed06c3 Merge pull request #273 from derekwaynecarr/mgmt-cluster-integrations
1e495b7f09f402ef8cddb121f308243e799f5c70 Introduce per cluster Ignition Server
a916e84c21ac1d8a4490a1c1a7c4c5c48b67a138 Merge pull request #264 from csrwng/stateless_reconcile
7fa2c9e6cbf17540a4860b2965ce8289cc1e64a4 Add example integrations for cluster logging and user-workload-monitoring
2f1e153f43d295a6d37f4c4da24637456bc4e12f Merge pull request #265 from bparees/rebasetest
6ab9aacbb8536005fe95f21dac575ca82d5f2016 Bring OLM to control-plane namespace
95ea5199cb0f3e7793966436ccd1dc1e964d258d Merge pull request #270 from relyt0925/haproxy-update
7ab49da8bcf215a0bb9859ed7aba70ca7c25c0d5 update haproxy with logging and ability to specify multiple configs
8252e478c92e88cbe92c0f351ce415d5fc359903 Merge pull request #268 from ironcladlou/initial-metrics
7ec3ee9744be041749fe87c25a373604dae26206 Integrate hypershift-operator with user workload monitoring
0f1a772df9936142e990b1f51050a5607c014040 Merge pull request #267 from mhrivnak/support-platform-none
7c090ad03b2a5dab7212f537a72cdc24dfb75b1d Merge pull request #263 from csrwng/different_etcd
96e76ee58cf290e6f1f7b901e5cdf2ddb8d10115 Make recocile functions stateless (kcm, etcd, vpn)
521083ebc0f4c36fb80f263ad8cddd55fdb0783b Makes SigningKey and IssuerURL optional
e3c57559209332e240e941eaf7e0f830ef4bd65f Temporarily change etcd operator image to one that works
c26577d5b91862a5b049c085f3464e6440c8381a Merge pull request #257 from csrwng/stateless_kas_reconcile
e619ee59b143670a3124e7f79f774e35638120db Merge pull request #260 from relyt0925/ibmcloud-cloud-provider
33ba4fec0964ec0b27f49c665118c010338ba492 update changes for cloud provider
1ea4396dcb7a9f895d2a2328e6e31bddaa9adeef Make Kube APIServer reconcile functions stateless
1c1e5838282b91ba92585b5d18edbaaa00d56f56 Merge pull request #256 from ironcladlou/make-e2e
4323fabd0477fb3c81a85bcddd43c493e7ab528c Merge pull request #255 from ironcladlou/cli-create-labels
550ac858adf7d7bb81a33d0cbdf2e044465a8c7e Merge pull request #254 from ironcladlou/oidc-discovery-retry
f2945858c0140cf555ba9502e0a66db3a345b94b Add e2e to the default build target
c0fc8cc8c796978a86bbe58745a2c95ba2ee4d3d Merge pull request #246 from enxebre/let-capi-use-internal-network
9c40680c13ad6c6d56a34df4549b1e62cd25d918 cli: Support user-provided hostedcluster annotations
9ad656f4e33156aca777749c34de1d2a22204d2f Let CAPI use internal network kubeconfig
8d123a86fb16a19382e17e5509a2b5f761947140 cli: Make OIDC discovery retry until cancelled
8d0619de7676454f68def5b2d51f229057c5011b Merge pull request #253 from ironcladlou/fix-e2e-clients
6a8d7ada0c251dec53679e5c14cdaeef1d343af5 e2e: fix broken build
d24cc4ec9cf8dd5a9bd4cb377f32f1a6607d0eb1 Merge pull request #252 from sjenning/fix-kas-bootstrap-user
870bd28449243cb3281bfff6b06b74abaf46ef59 fix typo in KAS and boostrapper users
ef404a47cd4250833b47cd79796a06a63bad5e97 Merge pull request #250 from enxebre/cleanup
305644106e1f9a30966c25eb6496b1fc205aca5f Merge pull request #251 from ironcladlou/stateless-fixes
68eb13b5fba800f370c902cbb1faaeb3017ce683 Revendor to drop s3 client
200149baa3077212c310600c72877663084b8c03 Remove unused s3Client
8ab5fe6c2147e03986b3c4ca3b04377c9d08c083 cp-controller: make KAS reconcile functions stateless
d360183e4af38165b6b84f5387403a524fe04ec9 Merge pull request #200 from csrwng/refactor_kas_kcm
b2e78a4f7382501a86687936205bcd2febe2c0ca Refactor core control plane component reconciliation
d061be0197193756bfb93186524f0d0106f58ff9 Vendor additional kube components
9db19cdedea23a14b0d29391c396a20eb752e600 Merge pull request #213 from enxebre/drop-4.6-ign
ff4788e8788991275b974198e229242a10ddf2fd Drop 4.6 ign support
46d3045cf72bf0ceb19dcca3f2d2528eda1c96f6 Merge pull request #221 from ironcladlou/secret-cleanup-fix
eb24f63169c2fa76811f6b392f1740508a4ba9ba Merge pull request #217 from ironcladlou/secrets-cleanup
0eb9c3be2c4ed15d38481aecc11a4ec067829137 cli: Fix secret cleanup when no infra ID is specified
5e353275a5bb23ef2802d477b8a67903939ed117 hypershift-operator: Ensure owner refs on controller-generated secret
d11e493a3cca3c64402f655fff3e132f33115956 Merge pull request #216 from sjenning/add-ingress-config
12b085d07c1f7693138fb6a7ef3efebb171d6b2b HCP: add ingress global config
a2f97c09ef3b03bfe55123789e36138428987c98 Merge pull request #214 from ironcladlou/kubeconfig-scoping
03dec9a1c8cbddce7c6caca5ab9437f0d292f89d cli: Enable rendering a single kubeconfig for a cluster
05b10ad5810dae8c77a515c2c79eb2598909a8d5 Merge pull request #212 from enxebre/mcs-userdata
362ebb14b2361b761a6ad9674bef7f446ef8c11d Move userdata name into MCS status
ee1347392b458dc56d2884eef4b7d82d48a9fabf Merge pull request #209 from screeley44/cli-secret-cleanup2
7d72efa8f53c1aa391be950b8e22282b7f09a56e tracking CLI created secrets
929f3427dfb2b58f0627ff6e5dcbb636e5909f9d Merge pull request #210 from ironcladlou/nodepool-controller-panic
73da1bc576c46d5a45f440a79b3b17717f5a3243 Merge pull request #196 from sjenning/oidc-rework
4d0127e77017f50bfa10d078cd85f488fa93f999 allow KAS-provided or externally managed OIDC service account issuer discovery
595550509b1543528235ad669382183ef770dbf1 Fix node pool controller panic and release image API validation
fa7adc7a3dd1b611964baaa81a8cd58463198caf Merge pull request #206 from derekwaynecarr/fix-haproxy
f24ca1de4f30893f555013bf05295c701ac74730 haproxy static pod cannot reference a pull secret
fec57f340bbc2133218fdf134c1a9685bb90e866 Merge pull request #205 from ironcladlou/discover-aws-images
bcd7de40c95f06422f37fad4e4fde6d0f9e5fab3 Dynamically discover release image OS metadata
899b5d40e72f0ae73d9c41b33ca81c625ba9fcde Merge pull request #198 from sjenning/baremetal-workers
e294289922ac2e18da8014dc2bce109f4584fcb9 Merge pull request #204 from enxebre/remove-function
436db2ad5bd9388ad651d449c05e16692c67545b Removed unused DefaultNodePool function
e56b20658ff6a0a6bd5bb04a7bb08ccafa657f75 allow baremetal workers with Platform None
d15ea1f33e11c53a1a9124c98e8dadacf333234c Merge pull request #203 from sjenning/remove-initial-compute-replicas
ad0e4fd9ccf332e3e51884346a9a3bbf1b47baa9 Merge pull request #202 from ironcladlou/missing-pull-secrets
d130f909e73c3f0fd23508f06e57542e19698c61 remove initialComputeReplicas from HostedCluster
4f16bd4c501b621d069e31cf8d00657334d789d5 Add missing pull secret to deployment
7e1f9acdaaab7dcbf88a7dc3d44dd98e29aafd1f Merge pull request #201 from ironcladlou/fix-missing-pull-secrets
5136cb24356badb47d526a572e793db1a8e78082 Fix more private release image repository issues
822b86c8b2e999800ab29083ec4a644afc158a64 Merge pull request #199 from ironcladlou/control-plane-pull-secret
c9480a1be93b1b26838a8daf08e23d305acdad1e Merge pull request #197 from ironcladlou/cache-release-meta
73ddc4fd2737043446d8294e818bae7db5f5df9e Fix private release image repository issues
d83b65a6d8452ca72429f57d1d76888b3e9ef83b Improve release image metadata lookup efficiency
a3b101c5fc0c8c68ccd470d5b142a842843ab5e0 Merge pull request #195 from ironcladlou/test-destroy-tweaks
1fb4586b6c011514b673ec6775fd21e822582cfc Merge pull request #194 from ironcladlou/image-lookup-timeouts
f599278cece2633ac746ed2211e5c9479123df13 Merge pull request #162 from screeley44/oc-phase2
05e0b428e16f15ed4f743dc1050f4936c951ac50 e2e: Improve cluster destroy reliability
22dc51074c6ec3b49acfb6f4f81f2cdb04ca20d5 Prevent release image lookup failures from blocking deletion
bdb08c001e3c920a0047db42b5e8ca951a60317c Merge pull request #193 from ironcladlou/none-platform
51870f49d5b794b01ad69a1104df3ebb170ff066 Initial API support for provider agnostic control planes
e21690df5e8fc883ee5105a5eb013a356eac4db2 Merge pull request #192 from sjenning/fix-vpn-nodeport
334ecc963342203e8b8f783505e9bba7684f6797 CPO: use nodeport in for external openvpn port
28159131cc1c38a87f756936ce9e131bd238024b Merge pull request #190 from ironcladlou/timeout-lookups
2bc2ba9f20c651c7fc7fa2351a87b98eb30c991a Add a hard timeout to release image metadata lookups
31c814fff11779f5a648b2c87b6f46f502eb1f2e Merge pull request #180 from relyt0925/reconcile-services
0bb17944a54a3928e503e8655864ffd9a2fcbad3 Merge pull request #188 from ironcladlou/destroy-cluster-infraid
d51b06ae5c072af8e4356699fc721059410dd843 cli: Make `destroy cluster` useful even when the hostedcluster is gone
b6da14e928de6ce5e08ecbd9dd5d4c4fef05f061 reconcile all services
092014981aced1e304bb07c1ced7c40b63d983e8 Merge pull request #184 from ironcladlou/route53-retries
6620b2e966accf93907b25a3476cbe804b8cbdb8 Merge pull request #187 from sjenning/fix-imageregistry-config
588c5ad3d2e1626b80575c3a48a0bcef4821fc04 use image-registry managed s3 storage
257079e7a1bc497c2b831ec1dd5fd838fafd4ae5 cli: Add explicit retry/backoff handling to route53 calls
8c0beaaa85604bee70260f2697bc0c7d1a6490c0 Merge pull request #185 from sjenning/update-cvo-deployment
1717eccef9e08632b00c1677b4ca7cd6fcb749c2 CPO: update CVO deployment with empty listen
24a81855e28aedcc4f92ef456a2252d490f5d2b3 Merge pull request #183 from sjenning/remove-old-access-keys
fc87229261fc1d3587f59a520a9cc89c994e517f remove old access keys for existing users on create infra
d635975f6de20c077f1c4f614d1edf8c1e2a177d Merge pull request #182 from elmiko/update-autoscaling
597270623d8ff868a902f19e22e4eb9d376a343b add optional tag and omitempty to autoscaling field
ce927ffdcd1219313bd6ed51fbc1a52312576938 Merge pull request #143 from elmiko/autoscaler-api-impl
f8f8f33a4cd9cfa223e539f50d707a67183dac8e Merge pull request #181 from soltysh/silence_usage
1ac2d9a63167ca8434d1b0a1254678cbdc1faf21 Merge pull request #179 from ironcladlou/retry-throttling-errors
e2b9e9c11a6da95d44801b5fa3d7b4175d99d401 Add SilenceUsage for all commands to not to print usage on error
62f758b93b648c135958535eb4ad38bd0754cb9d Fix small nits in readme
14efdf34e6311f13336c367adcdf21990c704d91 cli: Add AWS Go SDK client retry handling tweaks
52438160932fd8f4ec17da5a01ef5a68eb7c04cf Merge pull request #177 from ironcladlou/destroy-retries
de53a22497748ea6faf71f73f030e6e3d3d0ae62 Merge pull request #178 from sjenning/idempotent-users
1daa0010b42569e5da8ddd568a42bc283bdf5a0b cli: Improve destroy retry handling
a6ec639fdf4b566e77362a2219df623ba3a861a5 make user creation idempotent
d3b06201d977b743b120a468b423c9c57721da4e Add progress and reason to hostedclusters
79a8da9e873b37c3f1454d600ace309e05f2abaa Merge pull request #175 from ironcladlou/separate-iam-users
68eeb629b7ec43036d265cbd8ecafa7285cf84cf Merge pull request #176 from enxebre/reconcileMCSServiceNodePort-cosmetic-changes
dd92dfcb11820f5a54cc5bb4981b86f0e3828cd2 Add cosmetic changes to reconcileMCSServiceNodePort
e39531394891c549fc4b813b0d76000a130d5043 iam: Create IAM users with policies to inject into clusters
69515707473c496aef01501356f2e01e4e8ba335 Merge pull request #173 from ironcladlou/e2e-grace-propagation
5226aed25848818ec74519f475fddca9971ec925 Merge pull request #172 from ironcladlou/restrict-roles
f249f4688049e0f4f41ead1fa0bd9efd5f213906 cli: Add more guardrails for cluster destroy
8fc520dc80a5927c922cdd64ec46c1158602f87c e2e: Improve deletion handling
d3d98ff572f54e6f82ff58027ba37cca4a2f3370 infra: Restrict roles to expected service accounts
daf5d495a5afdca11750d7fd88be68c60b2c2c18 Merge pull request #171 from ironcladlou/revert-cf
fea362bacdf8e250c9d69c46b2ec9fdea188074c Revert "Use CloudFormations for AWS infrastructure"
97ec98a66b6a43f17233044706c22e26770b8225 Revert "Use bespoke, narrowly scoped AWS users for guest clusters"
03f4d5e74d7e02a7fcb86f61791f93e43486e939 Revert "cli: Try to improve AWS client retry handling"
4a4f2278925be8435df422a44f2a111abf7de685 Revert "cli: retry failed deletes"
3e53e72262a8994b3105a66d1516f4af4c85c11f Revert "cli: Improve failed stack creation handling"
69bfbd5c71f19d47808edd5af0d30c521ce93369 Merge pull request #168 from csrwng/apply_on_create
ba0a0f98188b8e5c16b64de19e0789d9e1815925 Merge pull request #167 from csrwng/increase_burst_qps
20295da31e6ba344aecac7068980d7b5a8879348 Switch to server-side Apply on cluster create
0da555555483a08dc9977732e3aa345ba1302df1 Use common client function for CLI
4fb18bf101b05f54c5be8307a478269a62010c41 Merge pull request #164 from bparees/version
fa97ab2feaab3ea881fe0f4d3691b529e4ad3b3a Merge pull request #163 from relyt0925/node-port-support-v2
f412b2bbafd7d27bb37bb9cf4cd8d2d70fd63eec Merge pull request #165 from ironcladlou/retry-deletes
ba7c0484b2b9546a5c3db83ccaba536d1fd67331 cli: retry failed deletes
7f6a5694c67cc1a5146a78295ab6931c6eccb27f implement service publishing strategy control
c2efc90f7c9d12a3904f45f332e8cfc4bb8fa377 Note requirement of go 1.16 to build
398300880d4c28d5d9025b098c5f4fd6aacf5105 Merge pull request #153 from sjenning/restrict-roles-to-service-accounts
11e0b926705dfd012e5a77538bfccce7f11119f9 restrict roles to expected service accounts
6b38f5716856c38d0d680d1c81c21bacad00d8fc Merge pull request #160 from ironcladlou/aws-lookup-retries
a449b50e647c0baecd3b087f1e0dd71dfb68fac9 cli: Try to improve AWS client retry handling
00de2ec09be5208c8d14b3403cc6f1e5efc81c83 Merge pull request #161 from ironcladlou/fix-e2e-kubeconfig
a46ac3d034a0ff229f69c54bd140d21b8ded5ca2 Revert "cli: add a --kubeconfig flag"
e122aa3acdd291250e95aedabda25e32ff69d819 add cluster autoscaler options to hosted clusted
58dda0701879ad2023d046d5624626ad76d7369f Merge pull request #159 from ironcladlou/kubeconfig-flag
2b1920278fc7cc53597dff0f167a3e5866ceb468 cli: add a --kubeconfig flag
d80bfc845522396d7c6c30a0477b1bcb439cd24d Merge pull request #151 from screeley44/small-readme-fixes
57313e9c448a91c365136322093b46bc4f7c0083 Merge pull request #158 from sjenning/fix-destroy-infra
1a5263a2cd76b5980153601b2590b1b2ebf6fd52 create unique AWS client config for route53
f78082527fb5b7f353a085fb387a3e8f93cefbcd Merge pull request #154 from ironcladlou/iam-refactor
b916c11e95d0d3b417e39a2c46e127901e5a1ed8 Use bespoke, narrowly scoped AWS users for guest clusters
dac6b433df18416400daa310f97840e3ed8d8806 Merge pull request #155 from ironcladlou/dump-stack-events
d682f0ce185b1e336e886735bdacb747208f0922 cli: Improve failed stack creation handling
af1f688d207b2195b5e7625a0d0d97d49a310f96 Add troubleshooting to readme
3a97fd9b1e64d6b5b7f0bd709aaa405d2ddec75b Merge pull request #149 from csrwng/remove_required_basedomain_flag
e92249a2a5e58d56839bd1bfaa0b5ba1d2c7867c Make basedomain flag not required
b75fd7d6bf502a5ca98c38c00862c135567e9570 Merge pull request #146 from relyt0925/fix-scc-removal
89eba739317441b5cb8392de9af465733c9da9d7 Merge pull request #138 from ironcladlou/cloudformations
d875cdce669ca25bb3364499d699df9ef4171347 Use CloudFormations for AWS infrastructure
92a983308c740cb1456499c24dd8d2c053affc4f Merge pull request #145 from enxebre/awsmachinetemplate-lifecycling
5d8607f72638b0ff5bd89b104ce5d74b414aa569 move to using cluster role to eliminate removal of privileged scc on cluster delete
5754743adb602e7367cae5581664b8afb8da1cf7 Trigger a rolling upgrade when nodePool aws values change
ba5a814989da5ac0e93d56974d7233eed86331f1 Merge pull request #129 from csrwng/control_plane_etcd_refactor
1e0dd0676bd0090f797606c0928e83fef4d40ea8 Refactor etcd reconciliation
d086da164a0b4ae04686181cffa6973846f32454 Merge pull request #144 from elmiko/add-container-run-script
8362d2b0735975d5aa4b52fbb8826cddb5ee7103 add container-run.sh to hack folder
dbf3724e99f020bce50af90edccefb6024dc9ab6 Merge pull request #142 from enxebre/refactor-nodepool
ce9a6697c01fc6a63cd17707e61abd306ea21e86 Refactor nodePool controller
19d2c4d538ce2014da0554272395079c74c343ef Merge pull request #140 from openshift/sjenning-patch-1
bbf855628f1097e9180995af1eb3b0a463e6436a Merge pull request #139 from sjenning/nodepool-create-cmd
79fb87c4ca0f1d5725fa758d7c38c69466d644ff remove base-domain from cluster destroy
977a6aa3bb6fe038d9271d1f08961fc0ac0c4221 cmd: add create nodepool command
c2edfcf919ad89fafe9b789d91d6e20cb1597a29 Merge pull request #136 from KodieGlosserIBM/qol-updates
e5fa311194dec8425ea5715c58ef0fc365f71622 Use non-deprecated registry for base go image and explicitly define empty array for status conditions on cluster create
26a531c52fe52e342a22e4d55dc44455aa0faed7 Merge pull request #135 from enxebre/mhc
daa681723bdd217f387b2593043e287c557dd67e Add support for nodePools autorepair
52f402db0a32e24f44e16b97b4ab4c0519b0c664 Merge pull request #134 from sjenning/update-readme
42053d5edc26153446e6d901e147e5cebe3f9ecc readme: update for required direct ingress flags
c166356229d808bc373436cf7f41534137ab248e Merge pull request #94 from sjenning/direct-cluster-ingress
3add1d00148ff8c4383999a28613e500195e234b use direct cluster ingress
95e4a75c4bfcef85ac0d0bdf18c1648d8a411a84 Merge pull request #133 from csrwng/retry_sg_lookup
97c2c359e6e8d95f72d55c8e1094ed6402246cf5 Retry lookup of security group after creation
fce938c09164491fd3addf6bc82014719db0446d Merge pull request #132 from csrwng/watch_for_extinfra_controller
527d51b0bf6d94a5c5fbb641934cf1e82fb757a8 Merge pull request #46 from elmiko/add-autoscaler-api-docs
c85e6fdf05e8763158726d4441d1697642d2f742 Add watch to ExternalInfraCluster controller so it doesn't need to poll
1f1a9a19de2d43cfe6db1a165c97186ab2878279 Move hostedcluster manifests package up one level
21c0b19ebd7568698b6670260c83132ffe5cbf89 Merge pull request #128 from ironcladlou/provider-creds-api
359ba8bcba46b771d360c5ad07d1edd9319c1b88 Update API metadata
a97564825351ccb4f28b2ac13c53ce71ef4d3fec Various fixes
fd9452602c02c934d1f5c662ed6671134bb43e3f Separate cloud credentials by context
977f457232c086f7594efae81578e6133af8f0f3 Merge pull request #131 from ironcladlou/dump-more-resources
ed07dbd7b584f06e8829346bb4ed6ccdc6927df3 cli: Add more resources to the dump command
661b7cdfb6913a059ec496f0c0fa20913f15b890 Merge pull request #127 from ironcladlou/remove-unused-cred-usage
422688a9388e88ce4f41ddd4cc37c9f223355319 Remove unnecessary cloud credentials usage
442835786bdce050d4e5d8284ba32cb428864b2b Merge pull request #125 from ironcladlou/nodepool-refactor
a798e10c489b158ed45ef09139c41efc158bf2ae Refactor machine config server controller for consistency
e3a7082fae349404eaeaa6570f9ebab1151e44e2 Merge pull request #123 from csrwng/hostedcluster_controller_refactor2
a385d0d402430401b93e49b486dabcd62b6567a3 Merge pull request #113 from enxebre/machine-config-server
a2d2a689d4b8b421b016d4157066aac038f0a70a Merge pull request #124 from ironcladlou/log-destroy-errors
d98c7a7ae251a62c682a573a6ad43261d2da5a81 Introduce machineConfigServer and nodePool versions
9bc18b45cfabe8c05a428edf242c895ae1a888f6 cli: log errors during destroy
3c34ba97dbfe5027fcebe9625158c07465eb25ad Further refactoring of HostedCluster controller
0e7168e4dd741b61c49cca2801c9d2312301b548 Merge pull request #112 from csrwng/e2e_dump
d6f599a936ccdefc0431517c8e9545abfa7010ff Merge pull request #121 from ironcladlou/e2e-teardown-timeouts
c8e7bd0d99075c4975b88b909f3d1a60a9f6566a cli: destroy infra after cluster deletion grace period expires
66efc75bdb6ebd2737028c4d806379c5e7772df1 Add dump command, dump cluster resources in e2e
0c6e7f1df9724e52142d13566f41d1e86b170a27 Merge pull request #119 from ironcladlou/complete-manifest-refactor
ed606fb50dff3953b1c91d1e11e5d53e34ad6b41 WIP: Make hostedcluster reconciliation logic consistent
a0583f87bd73d377ed8c277446a0333691b2b011 Merge pull request #120 from sjenning/wire-roles
d3378f95e07821aa5ef4998f51fbce3ca55234b0 wire in AWS roles
b3cc1890fad515578772a10657438b50f8fd6e84 Merge pull request #117 from sjenning/iam-kas-wire
1f6a9260969065e1eb61ac6f616c40b8c77a5700 Merge pull request #118 from csrwng/destroy_iam_fixes
f2d0fc4eb0e6ee79a93e05efc9d03b3897a28b5d Fixes for destroy iam logic
c734b8be8a58189244de14c59fcd4ceec826b8ec wire in KAS signing key and issuer URL from IAM create
eb3959ecd35eac60cc0340d7906d824d7b63d0c7 Merge pull request #116 from sjenning/cleanup-applied-logging
63182ddbb0ec2430c617560809b839736108292e Merge pull request #115 from csrwng/fix_create
a3af4b3bf35b6bdfd9600428330a949c7e8ea0c6 clean up logging when applying resource during cluster create
e47303cb38c0d71c96cb519724befd0801c34de7 Pass information from create iam to create cluster
0063367b030be3f120e04cf141d5c95cb087d0db Merge pull request #111 from sjenning/oidc
f3aa84e031cfedbc30abe6a464fc131ecef66094 create OIDC resources and STS assumed roles
aa3d93d6d65026441976180235ee8405934dde49 Merge pull request #110 from ironcladlou/transition-time-updates
b5b1e50b2214af822963df5dd87a676728fae8aa Make HostedControlPlane image transition time field a pointer
21be6be5a51a765603b91d59bc00370e567c503f Merge pull request #109 from ironcladlou/hcp-delete-fix
7f7cf7a006c37a4178cf1ca7410e98161ef290cb Fix namespace ref causing HCP deletion to hang
32ce1daf41f834042b8e003b69b2e661262f0f3b Merge pull request #108 from ironcladlou/hcp-namespaces
1b069d107f47ae783419e98cef9f803367545143 Place control planes in unique namespaces
5bfad167741378c4bce8370910c4757df186fc36 Merge pull request #107 from ironcladlou/automatic-iam
260faa00edde5388d03dc4ecc99b574d2f22e755 Make create cluster generate IAM by default
1b9dbba1fa0bdc144bc6dcb70ed3d21b33ba6e7d Merge pull request #106 from ironcladlou/e2e-cleanup
442491f8ce2baf695f29f39b9f4b72c2b1728815 Expand e2e to exercise CLI infrastructure workflow
cca2207db7e467e2263d74cf68a222829aa3b518 Merge pull request #105 from ironcladlou/rollout-complete-time
1e70ba5a93c2456772bc8cd7c43ac5871562084e Implement version history completion time
edffa73bd4eb881cd99c9703cc49e538e9769637 Merge pull request #104 from ironcladlou/hostedcluster-ready
82c3e0ff2e095b59302d34181c7de2e3379bec47 Remove unused hostedcluster ready field
e8ea235b108a290fd969829c781b852f83cf906a Merge pull request #102 from ironcladlou/sync-control-plane-version
5b7e2cb3c78f048eed320c5df640fc2dfc2e55fa Merge pull request #103 from ironcladlou/refine-readme
216108f39b0831f1283c8f187d2300ce286b2455 Reorganize the README for installation clarity
0ceb93bf91f9d92a1d03a67e5652fc72c33e7fba Merge pull request #101 from ironcladlou/streamline-create
7a1b49e3f83904b67cb7d09979cdf91b28d5ee8a Mirror control plane status onto HostedCluster version history
6477a3a9e931d0c3f894f7cdd969726f8760d54e Add a `destroy cluster` command which can delete infrastructure
5d059d364650f670aa02db3676d8e1b1052ecb29 Merge pull request #100 from csrwng/kubeconfig_ref
5c2a042b6a5491e002403f8fe1d38a148bca8f5e Generate kubeconfig secret based on name/key spec
83a4de75dcf1abc505ac117bfe8afcbd32e7b108 Merge pull request #99 from ironcladlou/bootstrap-pod-race
d31f89431ce12c47a49f53e51881e23f6339a5cf Fix upgrade race that stalls rollouts
e1aee57ecdd3b56bcbd91890e7b107cea10e3587 Merge pull request #97 from ironcladlou/optional-sshkey
714da933be6089b531a7e3627460169646b77458 Remove HostedCluster SSH public key requirement
56af8de9ea9ae7e5544033876b496aea79c89414 Merge pull request #95 from csrwng/capi_cluster_infraid
bbc60a31ec4ad9c87d135ffb59be85d713747eda Merge pull request #96 from derekwaynecarr/fix-logger-opt
451138e255b8bc49e915b4d74e32033d0b7e6557 Hack logging to work where create infra is composed
76d53e774857b4c43ce76504747ca48c5f834836 Use InfraID as CAPI cluster name
23f540c2e734f779d8ddc3facd5c8d6938b00ca8 Merge pull request #93 from csrwng/cli-logging
17c68add1c0bdc5c98f4b88e9dfdd7f88fef6c50 Merge pull request #90 from derekwaynecarr/minor-typo
2e4d90c3d9f151c3df07cf151007e55d478a8a18 Add info logging to infra create/destroy
359256080515347610079e505b4ea158f19e7c07 Vendor logrusr
cbbfc03dcc3d9b5b8ef2feffdf73ef5d4a289563 Fix minor typo
baf9d7f9e5540319b62427ec9656df50aced61bf Merge pull request #87 from ironcladlou/create-kubeconfig
a7f44cf0dfd7523d853c66f4e90a170ff40f3fb3 cli: Add a `create kubeconfig` command to help working with control planes
2965f4c9f8113643a6ba3327ce7db84d52d21078 Merge pull request #88 from sjenning/cleanup-api-types
39754840d2cd8cfacbd5df0ea13655748aa925b0 api: cleanup types
52bc6798585c6cf563388e4c4acdd942fc74c89f Merge pull request #81 from ironcladlou/cp-operator-reconciling
134fc3537e072e49a7d7b30c66483114ee53320e Implement basic control plane upgrade orchestration
6eb9d93871b7313359261c739906db5117db95f4 Merge pull request #82 from csrwng/e2e_infra
19c1f24887796270b3fe82e5f65624dd02997544 Update e2e to work with BYO infra
a0b82488232697057a80508190d20b8abdccad5b add cluster autoscaler details to the api doc
54b6538355e329f7aac1b3bcb90c7ba36fbadf78 Merge pull request #65 from csrwng/byo_api_changes
6649fe86273cabcf5f535e5589c1e042003bc754 Merge pull request #80 from sjenning/convert-oauth-to-route
708226766f6d8c857de6cdff2e2c8fecd8969cfd control-plane-operator: convert oauth endpoint to Route
b6f3f6dc2a7d4bcff41fd9b47dde463a5600cf4e Update documentation
c8e361754d681085642ba900acf7804f89849878 Add destroy infra and destroy iam commands
162906eada1dd3ca37ef94a123f02d2503d1136b Implement BYO infra API changes
d5611efd9e9ad9e4e0e38f915f06d4ec4a39c19c Merge pull request #75 from sjenning/check-ops-e2e
9a3c036e700863a8f5ec5a73e9542fe905621099 Merge pull request #79 from derekwaynecarr/pretty-printers
5298f4ff8d89b828408c1d170f45d5c525d2053b Additional print columns for CLI
76b02fd1726b961445d14bdbfd5a344528dfc4c7 e2e: check guest cluster operators are ready
e7e14a211606707feddc17033f96fa62607c676a Merge pull request #77 from ironcladlou/e2e-context
05041284980077b51f7275125bd8749368650e9b Merge pull request #78 from sjenning/remove-ic-owner
ca005e1b0205cf63b2ba30b5926315e20dedeaa8 HCP: remove IngressController OwnerRef
0ae45880d9b59bc86fa33707083cf0b3af686523 e2e: plumb a cancellable context through the e2e code
6ad6a7078baa8e2c2a667821d53e359964f4876a Merge pull request #66 from enxebre/rolling-upgrade-api
4a3b5fd91f521d76ff58bb9c0e8f19cccb24626a Merge pull request #74 from ironcladlou/no-ginkgo
ae72bb7629efaf5b47b1c7b9f00ffdaeb8b801dc Add deprecated ginkgo flags for compatibility
42e73c2b0fea6315c72e76adaf0ff81c1cc8dc98 Replace Ginkgo with the stdlib test framework for e2e
7f74ad535b82b0ae11fa2322fbc3c53eb1a50ad5 vendor: update dependencies
e823d98dcd487b80e0243d2b83da19bfdc860de7 Merge pull request #73 from ironcladlou/update-readme
5a1edbc09ef9c3da7f5d31515f44eb8ab33b5562 Expand README with more accurate guides
5c52cdcb26f1d6089836785637f2d85a8703cfa7 Merge pull request #72 from ironcladlou/rename-module
2f090b29cf8b66368ebe167e616b2a4d31da231e Rename Go module from openshift.io/hypershift to github.com/openshift/hypershift
db74c08a7acaf06e2735705ed6086c4d2ff56aca Add nodePoolManagement API
698f948206dcea3d18c62ff1f757b96a78c13fd1 Merge pull request #71 from ironcladlou/operate-kas
49b73dac0484658d4b8bca341ed5aec0754a401b WIP: extract kube-apiserver manifests
8adf09423586332768385d513c46f8a9aea2b53f Merge pull request #70 from ironcladlou/verify-target
4b2eae8f92f1013906f075e86b8111e3fa185b74 Makefile: improve the verify target
5442e03286eb3d2b8bc4c027fbf4f8d4263f7d6c Merge pull request #67 from ironcladlou/fix-api-target
23b384d646d4ba672d495a3e7f813444b1e2c95f Makefile: fix api generation target
d7da5e7a46271f2594e66cd14a784c6e27989143 Merge pull request #62 from csrwng/infra_cli_refactor
26763d33bfed3bd01269bc18050a329a46d50ac2 Split out IAM creation into its own command
9bf1c960b719a35a5f0666f0ee2044899c10d246 Make infra creation idempotent
ec360a66bb1e8982291666925109d19400eec1ab Refactor ec2 tag specification
eff66e44e810cf0ae8c5a9990875458b10dad28a Invoke worker instance profile creation
847c5a13cca64c36b0a46fb6c5a7d76a63a8ab40 Separate aws infra create code into different files
284ceae71b795094a91c325a9e5cac6cea4ab46c Create aws infra subcommand for aws-specific infra
e0d4255ff942840f96014ebd7bc216904a576a84 Refactor CLI packages so each type of resource has its own package
e462164e158c75a2d845a2c81d6de4501b3cc80c Merge pull request #61 from ironcladlou/update-api-deps
b1121a35953bc19749b907dfea953d98bf576d45 Update k8s api and controller-runtime dependencies
6fcb0e4bb0363c0c7f79585f83ec047dc3190a6d vendor: rebuild vendor tree
3953c6c9e76a5c761c1f687d39c39329009b997d Merge pull request #60 from ironcladlou/remove-dependencies
25775db7089a5888b9d980456035b6c1140832b0 docs: Add docs about how to manage third party dependencies
267385206bb7988271fbde5d19c6301e6c89c23f Remove all cluster-api Go dependencies
b511bbb80554257d6a9b1c34e3de5522d2d9eedf vendor: go mod tidy / vendor
ef6b2999b6147ce5c6d3a784132ffeb3ee5307b9 Merge pull request #53 from enxebre/machine-deployment
2467aa23e74a7caa42d6f4cc4be0fa1bb134da01 Merge pull request #59 from csrwng/infra_cli_worker_profile
e90b03bedef2f278c9054cf5a8f4343e52393bbe Merge pull request #52 from sjenning/ignore-kubeconfig
be9af339194cdf3e401c45cc3c051c2ac63e0380 Introduce machineDeployments
e6e30927c95f737d24f47a7b73d34d682925d0df Merge pull request #58 from ironcladlou/optimize-codegen
a4e105d9aa7805efaed575e329b6e5c6761853c3 Infra CLI: support creating a worker instance profile
fd7616a917f93272e6439563bd6fbe4c00f6d152 Vendor AWS IAM client
ca623e0f0623094aa4f99886498a0dd69b261996 build: optimize code generation
7e87078f99523902b7708825a0d2eaaa9a448769 Merge pull request #57 from ironcladlou/remove-bindata
30850d4e328efd16e3bc55879b35b440cd3a0b91 deps: remove unused bindata dependency
69ffe4fc76b367ceccfb3b3f6ed35f5c916d9b01 control-plane-operator: replace bindata tool with embed package
22dd64e6ceaf54d2513b317c7fb1a9396bc7b5e5 Merge pull request #56 from ironcladlou/embed
826a7cd1d4f870eeb17c631a4ce0cf9b1f15b0ef cli: replace bindata with embed package
7c34a0d1794dd62a5b8482b67f3cdf8e377a1c9e Merge pull request #54 from ironcladlou/go-1.16
2ef8511be4b702ced21fda2ec9d93663c67357fa Upgrade to Go 1.16
2349e4230083ca3abc4e3e03b27b84c27575f997 workflow: ignore kubeconfig file
a4f4bc3409060731a7842b2c43f83402f09e7f58 Merge pull request #49 from csrwng/create_infra
f71b3c965c35e576f448fca1333735520ab5710f Merge pull request #38 from csrwng/byo_infra_api_changes
d223b5e0990e15ab1bc22320910c5abd068c4c89 Merge pull request #48 from sjenning/avoid-collisions
37132d8d38ce2f885aa199eb157fc5dba74a5389 hypershift-operator: minimize ClusterRole use
262b13b53100951657a5d6f0878681907b70dd27 Merge pull request #51 from enxebre/fix-autoscaling-kubeconfig-key
ec93cf0d2761002da19b8a8f17b9c99a23c07d04 Merge pull request #50 from enxebre/set-ExternalManagedControlPlane
396a1c5aac1055c9097d4da8b1a26273d537e1d9 Set back right target kubeconfig key for autoscaling
7e48b2a8be7802ee4b9891d649e4f1a7d2f84cca Set ExternalManagedControlPlane in HCP status
7b64a25961bba4af71ebd2f04e66ff91cdc625a5 Add CLI command to create infra
fd93bc822e711cde746c891cd76f59fd909ddb49 Vendor AWS SDK
76c1882edd1990d51ed7e2e1e7a3fec217148424 Merge pull request #47 from sjenning/avoid-collisions
d722812fb4503927fca9805dbd91501e0ad872a3 Merge pull request #45 from sjenning/fixup-hc-delete
492e13c30880c720e00de73e5776a06f3226525f manifests: suffix per guest ClusterRoleBinding names with cluster name
d2e401ebe2cdc763593bace2410ab8d5a1fb7a9e hostedcluster: refactor delete
d57e59b8b26a6a4f202525d6c478f9c9104ea465 Merge pull request #43 from sjenning/async-cluster-delete
f9c49b784987b524ee87cebd56b446e813f8d7f7 hypershift-operator: async Cluster delete
fb26c5d750786b4252e8ef21b3ec851fd43389c6 Merge pull request #41 from derekwaynecarr/split-ha-policy
f343d75abe014c9268bee4ae4e8a2de439d50ff1 Merge pull request #40 from ironcladlou/kubeconfig-status-hostedcluster
549e8c742132e7b46c03d813568e00540c153c40 Surface kubeconfig via hostedcluster.status
42aba1d19c0395b17abbe1409b7ef38716f1d9f9 Merge pull request #42 from derekwaynecarr/bump-etcd
6ad0146dbd012d45afe5b70d189ae555171c90f0 bump etcd to 3.4.9 to match 4.7-rc version
d8a7061a9eb754fb6c3f9ea29cc726f69ad97b2a Split control param replicas into availability policy
f4519eedd9ebac2808afa824f6f2b9f7490e0f95 Merge pull request #37 from ironcladlou/kubeconfig-status
896ef6185ad1ea473f2fbffd7ce78aebfaa2be8d Publish kubeconfig via hostedcontrolplane.status
9455f23065bc9b11871fa727ae5ac06ca8d66022 Add networking field to HostedClusterSpec
eb36b098cd123b8b4fa1e746e391a8f3b8764c95 Merge pull request #34 from ironcladlou/cli-dockerfile
936403e774364e911fad60eb116e9463e6347b94 Merge pull request #39 from enxebre/kubeconfig-name
0d5ba4632566301ab70c2b39796745aab0e34a0f Rename kubeconfig for target cluster
31fdcdd76b32050cc8179f6e3128c2f8a5800a93 API changes for BYO AWS infra
444718daa0ce84dd66cee0525a32e7b42b5b15ee Merge pull request #36 from csrwng/api_doc
2e98e9dac9fafdf2cd6429f80f50a7c0abc68c11 API reference document
6e5b389b52db9a14f81ff266d4f439edd5a5b2d0 Merge pull request #35 from ironcladlou/hcp-controller-error
0b99ccd6b12b63f7251334a400ddcb8e96b2dff5 Fix unhandled error in hosted control plane controller
6abfad429bf0f1754059a69990a7766d00781f3f Add CLI to the image build
8a9f3d64a4f1c61d9c7b145338ce9868480c8f7e Merge pull request #25 from ironcladlou/hypershift-operator-manifests
c9fe9bcccd4d3b38d4d1d618c2e91c686e157091 Merge pull request #33 from ironcladlou/e2e-node-readiness
b148779ca2c5f170556bd47208d2336d49ed2d53 e2e: wait for node readiness
7e8ee70c5155fb92818ee8f0743103c73cee0ebe WIP: port yaml manifests to Go
a7c7cc3dbc5c37ad989256daaa9c1238897463c2 Merge pull request #32 from enxebre/condition-fix
b9525c307c5b7d678a26d525a5a25c3f57dc45f5 Merge pull request #31 from ironcladlou/cli-replicas
400bec47bdef6305c6a78d2afc8b2053329c37da Add CLI support for overriding replicas on default cluster
6d8a43811b8044a31145d1905bfc2e33754887bd Drop autoscaling hack label and return early when not enabled
40ab35f1c5f92010246aed638d45f2842dd48705 Merge pull request #30 from ironcladlou/nodepool-autoscale-ptr
8e6dfea7355971398928a4714ed3334ad15f056f Make the optional NodePool.AutoScaling field a pointer
40629633c42732e3b5c7f73d0d90a0c0ec763e3b Merge pull request #28 from enxebre/nodepool-conditions
8ce0261d0a9525d576a930d4da02d35f53c57016 Set autoscaling conditions for nodePools
a5828c70d202bbe2ccf315d2e0f6523c04f002fb Merge pull request #27 from enxebre/deepcopy
96f9e146c086bd9eda1fbeccd8d8b14d499392ae Run controller gen deepcopy on builds
0e0dc79c702e6cf8be42c230e94ea64d4b30bae7 Merge pull request #18 from sjenning/hcp-status
51f2a042cd54943445af070b1ab81fdcec78d372 HCP: add status conditions
c9b9e1db81402bf8f0520bbad483f1b0b7b9687e Merge pull request #24 from enxebre/autoscaling
352bdc5d5b9d597f8ee9b2a3b9e092fb09e0f59a Add autoscaling support
09ea5d2cbd064babb62c2b347f9a5d80736aa5ac Merge pull request #23 from enxebre/kubeconfig
662706765797d8a6f0dcff80a60a40ae9fa4f396 Rename target cluster kubeconfig
66e1d2771b8259598ca2c31530cc06fa981125da Merge pull request #22 from sjenning/cleanup-cli-flags
314f2c1aff3815c318b55f8ff6b0fc03b9eb6980 Merge pull request #17 from csrwng/versioning
ba97d851c5267a368bb1028ca583608d47215b94 cli: show default values in help output
f2d7a3fba3ffbc50b4bebd0f6ad123c074aa9ecd Merge pull request #21 from ironcladlou/required-flags
622a2187389c7ac9c49ee764384d788b65f041a8 Track version in Hosted Cluster
e5d90ff9d828ac50fdf029214df9fa883b2a855e cli: mark required fields to improve errors presented to the user
64fe0620e9a3430142445b14586230c0e02c485e Merge pull request #16 from ironcladlou/cli
7beb9a8da235ef8812567330c7fce7dcc31a8d15 cli: replace baked OCP image reference with dynamic defaulting
71b0fec27713b67005e350d288ee12f856f615cf cli: clean up gitignore files
2ab0ba7212d8887799422b66bfadee4ffa5ee071 cli: exclude Go files from bindata generation
67854e65fe653c4edeb7b7d35f396f6593997746 cli: remove unused function
c918ae05440d50d2c198b9c70beef2f1e054854b cli: update docs
9c7dd156934ef970a1f3b58fb150047afff47fbc cli: update docs
cec184be555185ae1c1d0bd0337b58c1385b308b cli: make create cluster apply by default with a flag for render-only
70162888feaa300651bce9e50d7273060b281794 cli: make install apply by default with a flag for render-only
ed752d426ac661ac38d717e7dbc8964d202832c9 cli: add a simple development option for install
a029b50d242990a64fc62ec27cfdf548b949e8a8 cli: rename 'cluster example' command to 'create cluster'
169ab6a86404c0cccd234c0ca2d6b2b12edbe29a cli: add SSH key default for commands that use it
0cf816abf88fba53851bd98b4b064c7b0e222c22 cli: move command code to top level cmd directory
3d628a1f65b3f6a803cdaabed7173464db6add45 cli: clean up scheme references
137353a05c6422a34b3295ceadeb4aecf625ffef cli: remove unused ginkgo vendored stuff
c7df3b4ef09da3963f4deda1f343599751256ba6 cli: remove ginkgo binary requirement
ff14c2537ccfde8d946118e27d5c8d0326863be2 cli: remove remaining kustomize stuff
1c9ab8f938edb4d1a8870f9c3b6c17684136426b cli: refactor e2e
11b0740e4034212b3e43ace8102a073f1f9d7eec cli: add an example cluster generator
9cf2f1df345300f3e6db081fc4ebf6c4fc44d0df cli: convert more resources to Go
c8ffef98902e854be529211fdad7a7536bdf11c2 Replace Kustomize with a new hypershift CLI
ae1d0f6df8e4f83be1cba23dffe8c79ef9ff250c Merge pull request #19 from derekwaynecarr/fix_readme
cdfdb3ad5418626a6f256a15ea4acbfb6f8e4bf0 Merge pull request #20 from sjenning/add-sjenning-owners
af49e993d7c7dddcec167b9547f41e8a5d946e81 add sjenning to OWNERS
928262081755f1d46c5208f6955900c33c1d935b fix example-kubeconfig location
054191c448e6fc0fea752d9110227356eaa77b13 Merge pull request #15 from enxebre/fix-delete-cluster
1265a4f57dd36f287798896d52f92198a1d586dd Fetch nodePool by clusterName
0111445cf87ccc7ed3272f56178836d6c76a6f4b Merge pull request #14 from ironcladlou/control-plane-operator
2a79d49de3ca231c944958885ac483b5a8e374c1 Introduce new managed Control Plane Operator component
a207c619db39ad578466116d2a3b4ff5fd78a514 Merge pull request #12 from ironcladlou/rename-control-plane-operator
50ec715db02e17f7d632092e86031a2958c9bc2f Rename control-plane-operator to hosted-cluster-config-operator
d7b33f239d20a7d235179c176bcf2105c4731cad Merge pull request #13 from enxebre/delete-nodepools
6eb4f299881de8f3b8d04a23770b61338c4c438a Add support for hostedCluster to delete all nodePools
d535edda09dce1292de06207afd58c3e433f6b53 Merge pull request #11 from csrwng/rename_openshift_cluster
920518c63814203ec640890c28b722ac6fe95fb2 Rename OpenShiftCluster to HostedCluster
68b5328635a8e35fd5e9d94c24feb43254dd95c0 Merge pull request #8 from csrwng/fix-delete
9007834cd3240038a43ca3c887b6d095f0db03f6 Make hcp delete more robust
4f98ae1457f3217a3f4ca59f1e04df86dfdc22b5 run go mod tidy, go mod vendor
c01d9413043bf98ba6870ced1896f01efc3ed98e Merge pull request #6 from enxebre/namespacing
15539193a3f3305e5be8d5deb55594117893c150 Move CAPI resources in to target namespace
632aeaab03aacc096f5d7500b31e2e07b83d98bc Merge pull request #5 from ironcladlou/merge-hive-41
4f618bf698bb485c98b8438f1eac4bb58202141c operator: allow NodePool to override default subnet filter
6353f8f7f3eb90c1ce0a830979ffd6ad8764bd28 Merge pull request #4 from ironcladlou/ci-repo-images
19c881ddf9796e2633dea20ebb9b49e1bc030224 Update operator image references to CI registry
5f5dce9f57eef79b5f2b7ca9e9da28c0955181b6 Merge pull request #2 from ironcladlou/owners
19b8e41a6b1b42d49b14244db8abf4de153c6b39 Add OWNERS file
4db5cefd168eeeab7ef12ddad540b0b8daab9b7c Merge pull request #1 from ironcladlou/update
174817b1ddc449a5d43c812dd3c2ab1ffb77f3f0 Merge pull request #39 from sjenning/update-release-image
c5530da23a9ca2af1eaeb7d8307ce8a89bfac256 Merge pull request #38 from csrwng/fix_kcm
c136bd002d5be801ae31e674725188f23e2d57f1 Merge pull request #40 from sjenning/runtime-select
7e948b37d4512d00e4e05bc5bd3dea7e023c6ba2 Makefile: make runtime switchable
eaa39c1af38d10cbb84d0debba743044d39ffc5d config: update example cluster release image
faa5439f08f7c0145b17b2a19ef9169c368c7fb9 Move kube controller manager arguments to command line
a627081def40ab6dfd4de9651eaa45c15cc1bdd4 Merge pull request #36 from enxebre/fix-delete
0d0f67e8e55149f73750f11569f56bb5840122cf Remove foreground deletion and relax timeouts for e2e
f6c4e17304c7ec5224ff7d9643f9f584174b275f Change ignition server endpoint check
ed9310f638a11301bda1e048454f0757559e24d3 Fix openshiftCluster deletion
e2121357cdec3f09cb1838987583447e18af9c16 Merge pull request #33 from sjenning/use-v1-rbac
60f5e69dc0843a5ea9c7a7dddbdc538ab3224fc5 Merge pull request #35 from csrwng/47_updates
9972b9488cdfd88293b4e7c7feab05c84fda03bb Merge pull request #1 from ironcladlou/47_updates
89c0ccce1a75fb1ce4662369b60a1eb6e01d4bf1 e2e: fix broken guest kubeconfig reference
3b715248d4309a4ba4edf9b2ed8d2ff77af56fb2 Merge pull request #34 from enxebre/external-nodepool
6f3c6256bd4500da3a8e1747cdd67c486e52914a 4.7 updates
e4be07130039e187fac39dc092f89cc36ed5afe4 Add instanceProfile and subnet for nodepool API
59698816de81050a87d298eac7d6ee1a94ddbb4d update rbac apiVersion to avoid deprecation warning
d12d2f59eef8275fa5f7bf03a534a7c91c7ee652 Merge pull request #31 from enxebre/capi-machines
82722f8bc9a8f3c1f857c41921cbf4e5283ae5a6 Delete release-info.json
596b3e340db483349934debe16bcf6ed2691a68a Add capa-controller-manager
2decf3843c3456fcaad938e2fd1ebeadefb6935f Enable capi machine management
bbce000cd2473e0eb6914bf3c3747859bb08500f Revendor for capi
88509e1a1155ed253ddd265bbce36e64c8cf85fb Merge pull request #32 from csrwng/cp_remove_filesystem_use
8c502eaca0442fd4ebc0bda6c3bc93777250dab2 Remove filesystem use for manifests
d2235df91ec44c1a7198cf2bcac67aafcef83d78 Remove filesystem use for PKI
161b6915a11a95e7c5933dc9b6cda99d662b448f Merge pull request #30 from ironcladlou/e2e
04769f95765d08658c3e1ba916f7db72d09a0018 Add a quick-start e2e test
f6a432f458793f84138094a34c3e235f7b5a5f84 Merge pull request #29 from csrwng/merge_assets
74e43b1c92003b7b93c3d80a850783a3fdb69ae9 Make changes to example cluster for it to work
f37369bfcffb01729d8f91673da75bceaba68e35 Merge rendering of roks and hypershift manifests
bc6420622dd0618d93b7c6217645e6b808069545 Merge pull request #28 from ironcladlou/imagestream-lookups
99d72d89d130a60fda2ff7bf3dfc116baf68c1c8 Dynamically discover release image metadata
053d91bfee5de9418d2cd9355b7262041281275c Merge pull request #25 from ironcladlou/control-plane-image-detection
68763e33e102c869ea3c4138922182a456f392b7 Improve control plane operator image detection for local development
1cc846dccd68dedd2b3f3ec573b66584f18f1f76 Merge pull request #24 from csrwng/remove-dh-params
ab3441fb06e2f7bea8cdb093603b178775813b1c Merge pull request #23 from ironcladlou/refactor-manifests
d91566c888a008c823384446646176fab80c21e7 Improve installation
4e0e2aa9c6e962f0a44174a3e64c6f7b8238646f Remove code to generate DH params
ad9c8aeb44215b27c20c2a41065e014a64342b23 Remove requirement for DH parameter generation
a6c191466e837cb383bcead0085cb5cfe1f7a2d2 Merge pull request #22 from ironcladlou/managed-capi
d98795e2ea5c072a6217ac4aac66500f3009b70c Add a cluster-api deployment based on a published image
b63f5ed740c078205d29f05e4c9e1d59c313e86d Merge pull request #19 from enxebre/mcs-platform-kubelet
27deef2c31d4035a9ad9eb9c42e2915a70d3f6d4 Merge pull request #18 from enxebre/scalable-nodepool
1a183838560021d1eddd06301f302ee804dd49e9 Merge pull request #21 from openshift-hive/gh-ci
27b338329805222b86e2cabc3cd18534d7e2e451 Update go.yml
b22229f8ad7b7316ae9dd380213e88265649f0df Introduce simple Go CI action
cd7173ced43097ce9105431e454b7582fe9929f8 Merge pull request #20 from ironcladlou/revert-konnectivity
6d941b48f8a589daed1f11bbc7486e8a98566eca Regenerate bindata
2bd534fd7b04717ca684a86de01d41ae596afb47 Revert "Add konnectivity server and agent"
7d62bb595f978512f15dd7a824968d3ea0b72c57 Set platform status for machine config server
a1f213e94dfe4494f3ea00c62fff68677bd935ba Add scale subresource to node pools
245bfbf9a9bd7065e3704b73115659de7f2693d2 Merge pull request #17 from csrwng/fix_nodepool_base
fc0a97e71d7c60bf441c129b2f5a3d8c217688c1 Add missing nodepool CRD
f5a8192460724649a28e2ac487ffc343e9f20862 Merge pull request #15 from enxebre/nodepool
dec1f7952ac6ed3a2f71e6952bf76a4ca4a61f83 Merge pull request #16 from csrwng/revert_capi
9055809883b4a5ba77c55d98a694e0d797fc1620 Revert PR #14
a3fa357af5f5b17cadb6f4c25fd2eb80b0f5ca38 Merge pull request #14 from enxebre/dev-capi-machines
206eb84cb0f38a258db644916312cc0c6f9a265e Add nodepool basis
f4e91149b8cfc36d49107c38bc1a15d36ed5e450 Introduce capi machine API and nodePools
db2dbbac71d121c01db33ae72c3411aed5b01825 Revendor for capi
109bd0cd07682fdbab85b663f2fc4c9b5320b225 Merge pull request #13 from csrwng/konnectivity
cfd9cebbfdb7339c32cdeccaca8f7604e2be5805 Add konnectivity server and agent
24bda339efe637c92d010100f20af6de42a93649 Merge pull request #10 from csrwng/fix_subnets
3f05668749dc35edef8dd3a305dd3583989fd3b2 Merge pull request #12 from csrwng/update_bindata
78b2df8e95cfa140d7b6d133629ddf47b66d9ba4 Merge pull request #11 from enxebre/revendor
b506f183818573c3bde76baedb6b1923d94017ff Merge pull request #8 from enxebre/delete
5db58cb9dcabf0a6e1c0ea1f40e2b39c3d4b5410 Update bindata
c583239c206a423860849a866b45e68ed21c3ff0 Revendor to bring latest controller runtime
95f5f253373b0a6b597f4efd7eeb8f1fd673cb3f Add ability to wait for resources on delete
c2b11d53589f7143cfc8b07fc7287a9cf99f8aa5 Merge pull request #9 from csrwng/fix_readme
ae3150e153af8f8e63d90efb248948fa716c9831 Fix README subnets to not overlap with default OpenShift ones
24cb1fd4b4e5c6b7014a8cbc3f2db61bc2802821 Use automatically-built control plane operator image
66c20e0d8446fd95e65e5ddce42b5317519c21f7 Merge pull request #7 from csrwng/fix_oauth
11204ed974e07a5ecd22f0a5cdaeba83942af052 Include OAuth deployment in ROKS manifests
cd54972de688df46bf28c72570c7034324eb7504 Merge pull request #6 from csrwng/fix_openshift_apiserver_ip
a334d691cd85f2e0aae22d5d0356bce56105a3ab Include OAuth deployment in ROKS manifests
ee650cb9008f48c45ec3a63f035a2d0c117301d8 Use the OpenShift API service IP from InfraStatus
45877f2e3011548a598130b1b6e388b8c381dbe0 Merge pull request #4 from enxebre/capi-resources
1d5534a8087a41fdebd597457ba632f082cefe98 Add CAPI CRDs and controllers
d4ab76072003d7293cd263abda7f60098f92026b Revendor for capi
67c88449640b643071f665ebaabcf802eb02108e Merge pull request #3 from ironcladlou/server-side-apply-manifests
5ed315785c5c52631c39582871e0dcf9cc09fcdc Apply manifests using server-side apply
8ae41cfc041a5248e42819bf6bdb77401934c13a Merge pull request #2 from csrwng/fix_dockerfile
452a953dcdd74146103492891f0eaa6e3bab4f3a Fix image references in Dockerfile
f64685f9807e4375677dadcb6df800d335c83942 Merge pull request #1 from ironcladlou/consolidation
6c8223fb0c7a04c46b56e316465fdb954f2eba49 Initial commit
945f86bc86ac4bde3a0c4dd8f0ef0e7dd9098cac Initial commit
```

Status: Syncing successful
