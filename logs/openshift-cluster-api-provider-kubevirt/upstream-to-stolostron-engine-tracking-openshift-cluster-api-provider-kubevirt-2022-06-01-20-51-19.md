## Fast foarding of openshift/cluster-api-provider-kubevirt into stolostron-engine/tracking-openshift-cluster-api-provider-kubevirt.

## Status Summary:

release-1.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-1.0 -> backplane-2.0:

New commits (first branch sync):

```
dc1e52ea3c5c2d55673be4d48c2f9b4aefce07e6 Merge pull request #34 from nunnatsa/sync-main
a278f8d014d661261a8b5fc7b47f5289a719283e Merge pull request #32 from davidvossel/auto_sync_upstream_2022-04-20-17-35
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
e6855602600e681a78344192adcbbd2762ada0c4 Merge pull request #29 from nunnatsa/os-release-1.0
f148a9e17f4083537ecd3c626ea327352994bb5a Merge pull request #28 from nunnatsa/auto_sync_upstream_2022-03-17
aecd95423ae7659db009b8860b8f46ac96df3a09 create PR
0fc14619a46870599c0ca385a8ae6db8e0114ff3 add script to sync with upstream
86301ce6d6d6fe1267d84ae54eff54a8c5cdbee9 Automatic sync with upstream
23727f2d40065f8ed9413e09c3e6b095650caa7c Change OWNERS file
51bcef99f79a56f0c24e64d0cc99262db96564f0 Merge pull request #26 from nunnatsa/os-1
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
83ba9317ca7820b3a81f3b423efedff4a7627a35 Merge pull request #13 from nunnatsa/os-release-1.0
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
3eef5aa90d3c40c409e2c8bb479ba254dcba8049 Merge pull request #11 from nunnatsa/os-release-1.0
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
0ce0e6361043b4874e842afe08e818807e560273 Merge pull request #8 from nirarg/merge-to-release-1.0
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

Status: Fast-forwarded successfully.
