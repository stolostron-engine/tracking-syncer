## Syncing stolostron/registration with stolostron-engine/registration

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 415 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
7962dae77237fd8b568aedc9c9ddf9c8bd075e3c Merge branch 'open-cluster-management-io:main' into main
f39b00d4e735e2dfd1ad34be5f60f7a1e53e8d60 Validate metadata.name of managed cluster (#304)
8791e8e4f867c55933205d23c7e7e16502223232 Remove: work directory in github action. (#303)
33525a94ff0ed81c5852d9fab22c86d933c80d86 upgrade kube to 1.26 (#302)
caebefcf83974a05d58b49a02dc0d7c99bba1161 Bump golang.org/x/net from 0.2.0 to 0.7.0 (#300)
cc7a5cdd96981c285669ea912148b1be75b622b3 Remove anonymous check from managedClusterCreatingController sync (#299)
28255f6a9d24e31004721595ad13c11c2096b94d use latest api to migrate clusterset (#297)
6f94ec28dd724390410daf9eebc1ab0334719036 Bump github.com/emicklei/go-restful (#296)
2d41babbb3a729f31005dfbf85d14d549e00cf6a update imagebuilder (#293)
ace1bdc1ccb2d6b221d761699a5e6db06e3aeefc add v0.10 changelog (#292)
177f916c0650ef4a9aa47bd2753b6f068f1423c2 use labels in api repo (#290)
9bf732aab38b98dd76b97bdd8a3c0cf4aa0a487d roll back code to support lower version k8s (#291)
923cd19f379aecfa46037ce2a7e8426f475a3e07 using requeue cluster instead of resync lease controller (#288)
6fca53a9e54f644fc38287f4c9978895cf473a62 upgrade github action (#289)
18e798299b3a78ead5075c6db4a6bfeea9d10e4c exclude add-on csrs (#286)
4d8c5c599577ea1364eebc2d7708041a0bcfc890 upgrade clusterset api to v1beta2 (#273)
ed8faa7c7d4eacac391c73365a01639bed475cab set min tls version (#284)
ca4fd4345e4b50e74ccab95a66780f17f9e96f38 Upgrade ginkgo to v2. (#283)
9878ed071a3b4e97b9c8372c5e4422e12f60fd38 fix validating webhook (#282)
2e1c039a8e1769496237c9827f43b2b181394452 Add SetExternalKubeClientSet to allow injecting to APIServer's admission (#281)
d8dd24899b258a5096bbe3230599b7b461119222 ensure a cluster lease is updated after the cluster is restored (#280)
1576fb0925677409edeaf876e5d5be24504e1eea rewrite webhook using controller runtime (#278)
3d4e3377fa5515ec725ec19d55165d1308bdfb5d Avoid frequent CSR creation (#277)
3c49c03e884fa4114025e5a787aeae1309226c32 update golang to 1.19 (#279)
960b2690d16858c4b7349fe9857334d595612f86 add v0.9 changelog (#276)
b391219017962ba5e9c22967a1bbabb03858269e remove the support for checking add-on hub lease (#275)
fd7eb39cbd0d878a10c103ce67bdf17630cbde64 stop to discovery addon when its managed cluster is not found (#274)
883295b635462a4cbe9cdcbc0d540a99186fa12b add conversion webhook to convert clusterset api (#272)
1194172bc5d8936311024b27d7081ec4b73bae52 decouple bootstrap informers to distinguish the lifecycle (#271)
d6081f91f381eb602e228daeb50d7cdafe941ed8 update serverURL and CABundle if ManagedCluster is created before reg… (#270)
b43a54935f3ea1f5d2cec852283bb3271954eb61 reduce log print (#269)
1612f1017e3667697cc7a8e853580651ca68ea15 check e2e mutatingWebhookDeployment replicas (#267)
95d61544251e2c196dacc51bc56350e7d2526692 recreate the hub kubeconfig when addon deploy option changes (#265)
5b9fe1431d168de701181b7ea3facfe70320a80d update libs (#266)
e7d98d0a975b9bfa3ec1656e3c7cc382f2bfde39 fix release yaml (#264)
1de5b58db14ad2e278d78c4fdd78fd2fcc328a9a add v0.8 changelog (#263)
7de42a03a6636f9f22573a3ff88c99bef2341da0 support add-on lease on management cluster (#260)
077793fb37ef58a4ef09c7e69d6285e7ae86c5bb Add V1beta1CSRAPICompatibility feature gate for registration-controller (#259)
84012648dc4b05ea7d18693021c45fc4722e793b leader election needs to operate configmaps and leases (#261)
f758ff586c34969f603b8738b2257bcac9d28d35 Support generate hub kubeconfigon on the management cluster for addons (#252)
483f44389846207973bc0ee74a59ce820323b6dd split registration permissions (#255)
2dcb530b9185cef3d433aa1717b6b0e46874defa update qps and burst (#249)
d37ce9d58cc2318e96e47712a9972d6030d14068 enable log flags (#254)
364bce97eff17c9730671571c8ad8ce6d4a365f3 use registration feature gates constants & variabels which in api repo (#253)
5b9b4a2c080a671554bdbe73c18d782c7a5bea03 add global clusterset (#251)
dd2c3fdf1960c89ce6ada8bac3f43a620e3b8fb6 adapt label selector in clusterset (#242)
215429b94cd15712468c1cccda05fb6aa1b46bd0 remove add default set label controller (#250)
fd33e20727c4d295f49b18c249d279369426c230 Update binding status (#248)
9271969e315f029a3fde47d0339ad6ad0d02ff6e Add client cert condition when cert is rotated (#246)
52b5857d21bc0180bdb1e2c2df5308c5c709cf71 Upgrade go to 1.18 (#247)
b849d2c83849d7af953c5a95576c8ccb98341a5a Patch status and finalizers (#244)
186bbcabd8a3ed360634277ab6c6e5df502b946b Add lint check in make verify (#243)
9ca206b5e5872562d5a73ed526d78fe7a8bf9141 add all clusterset permission (#241)
4cbc2d46de2c03f396519a660ac18a60353adfc7 Update golang builder in Dockerfile (#240)
4696a9545e012b042086f1d5672dd9be1c6817ce add join permission on defatult clusterset (#238)
4a8be951818eab95b2c2b39b0b495e59951fc600 fix kind create cluster --name (#237)
a243379343175efb12bf331a20982ed180f01f94 fix clusterset sync issue (#234)
7ff623a3395f1ceecf7feeaa7c687c35c638feb3 share release job env (#233)
29f55c944b5c3ab023c7f2983ccd91dcab565cfe fix webhook error (#232)
ffbac91e3e2eeda0cb479e8d29ec6ad5d216483e update libs (#229)
9d52c0f4979e45afc639987c4705903d08e13d7b publish release artifact after image are built (#231)
922fca0015d99cd2d2b643cb6b60dedd2c6c635d fix workdir issue for image action (#230)
83aabb4256d25722ec8680bc61a87ee6c60e63e6 Fix make images targe in post submit (#228)
927a8b92cef6611bd1f63b85752164d26ff9a6f6 Support multi arch image (#227)
12bef6bb913527d59f7ad43482936bac91d0dbb4 reduce the get request for managed cluster when checking managed cluster lease status (#226)
9279f318d72f6e4dd5d138ed89bed6f2a98e1159 Reduce queue size and add filter for csr informer (#223)
eb0daa24acb97b39c1e280698986e2417842f387 allow ManagedCluster creation with taint.timeAdded specified (#224)
560310e8aff8fd4c052b41358ce9cb9d393fc7a6 set clusterset to default when value is null string (#222)
59d2cd6a3ea965e80fe8aff12a53869e6068f6ee add v0.7 changelog (#220)
69129afb57ca99b72c1c9236e2ea729744fb582a Avoid building latest image in release branch (#218)
892a6ea78295bfa3dc012b890f80017cf9172e8f V1beta1 CSR compatibility (#214)
ed904328370d9e1b63556b5843c419b7aae664dc Disable apf in webhook (#215)
65606b7c29276b04ded004ea6c42ebdbee6ce6af add taints e2e test (#212)
a86fa506c933b43e0ef0e23661e6fb1120d16697 chore: suppressing log verbosity for test log clarity (#216)
20f60635e90d7d892fc98934e9d87380a3d3ef41 enable feature gates (#213)
0ce5210162681f2086a587e96d05b9519e90771b add disable annotation detection for default managed cluster set, ensuring users have property to modify default managed cluster set spec. (#210)
41c81be5f2d37020ed33c4b1cb6fa5226e368f61 fix override cluster labels (#209)
9b07f772c1d8446e4446c1df786e64a860d5da36 remove unused code (#207)
9d006722d8c2a45e00c16f5ce62b08d36b1b0509 add a controller to set default clusterset label for managedcluster which not set clusterset label (#202)
b8a1f9d676a3d2aeb68482d96ce53739c3fc867e set default in webhook (#205)
62e8879e5b8b3e51c3c2b2be6696bca9984fb958 update clusterset contoller to ignore non-legacy clusterset (#206)
92178adbec3f835b2cabb58b5bbb1b95e102e49a add-default-managedclusterset-controller (#198)
f3b18aa21152ba803d4227895605954577892911 Add hub freature flags (#204)
832e296a2fdcb346c7dafb77581e556c844e5ae6 Update generic addmission server to support run webhook locally (#200)
61dea84ea626480ce05c1252a1e79720e628dd96 trigger a new build (#199)
acf2ee2cfcd7cf73f0bf1009dacd50df7b85ca18 add taints controller (#188)
a9ee5e431f598212b41873677db4dd1c2738fd24 support run webhook server outside of cluster (#196)
3df450099a657e1840b92aa579ee49719db73594 add v0.6 chanage log (#197)
dd4bf2558a36e978200fa2e2168c57c2fa5ea877 add a link for LICENSE (#194)
4494da664eb8a1bfe62483a16816b49f83cb88f3 Update builder image (#191)
983391ba017e7fb6e2dc85b172624bdc3eea4b50 Add leader election flag (#193)
3d5b61375fed680d0e015a08080c948fbbea32de Update cache implementation and remove logic for rbac update (#192)
ffbb2b9744f547a23a85ca5eda8697924f5b3f76 enhance webhook to set the value of taint timeAdded (#186)
751c36b6f9480ce7944e3581c6447cb5175aefdc update library and refactor integration test (#189)
6331fe46291cc235d223a8d22a343f794a2e95ab Skipping customized health check (#187)
3afdcac894d00d006b70355a11a552007c258f83 fix lease interval value set (#184)
e5722d507f46d309cf428ab5d020786577a08f8f support run spoke agent outside of managed cluster (#175)
c849951f90d233975d95009dba8129b721455ef4 deploy control plane and agent in two clusters (#182)
d331716ed6a879e004b44261ea540a3b58ccf3c4 re-create addon client cert once bootstrap kubeconfig changes (#172)
50b92cd060dd4d84cdb8eb14fdad1e23cf56761e avoid recreate lease when cluster is deleting and remove old code (#181)
53b1c343cc0522026487e67cb738eba5c56aee2f Replace bindata with embed (#180)
86952694e1b74e46ad8fce2f740d413bb6db0371 Add push action for main (#179)
fc10d8c17de1b0e8a7070045c2507ba966a1a3f5 Update security md to refer to the OCM community security md file. (#177)
85abcfb07e246fbb63565fa4fece49ef577a017e Change builder image to avoid pull limit (#176)
7bb4b6864dee695026d2d23abf09bd65289095cf exclude the cordoned nodes when calc node allocatable (#174)
ef7c23ededb2f886fc5e799d2125637709ba1688 add change log for v0.5 (#173)
5ea8794d68642a6d372b236028ef5b489af7d326 sync the original clusterset firstly (#171)
4e7ecf37417432946c751d2cc462aebca51096b6 Merge pull request #170 from skeeey/trigger
723811561a423de0156384126ec019e07c2f3128 trigger a new build
a5462670342aad9c45b84d561361760c09518c23 Merge pull request #169 from elgnay/upgrade-clusterset
6f8ca332f9d8871b3f8e56917cd5babdfe9b314c upgrade clusterset api
26a9e5e59d6b4935685f9a1e693803a4f3a5bf49 Merge pull request #162 from skeeey/owner
095b4206136426f7f2f315ac7683a65d47e6deb8 Merge pull request #167 from hanqiuzh/update-api
659cad8426d98598f0cf1538b7af63a92c819ee7 Merge pull request #168 from yue9944882/bugfix/deploy-hub-clusterrole
14879508f825319edbeb85f0eef961568187c282 bugfix: fixes insufficient permission granted by hub clusterrole
ac1e0f0297b5f4a0d758fc1ba7451fdb21b58f96 update open-cluster-management.io/api to latest
3722e2b996154ea078eee77c793b11a5aa728293 Merge pull request #165 from suigh/08301056
80b5f416e79b7e5c261ddf19b9451cf97ccb954a report all resources
759265d36a4ef4e7f10f1a3530b2c5b7cecce326 Merge pull request #166 from qiujian16/embedfs
d16a89cd6cc299876dc3bc04346a75314cc14c8f Use embedfs to replace bindata
64b63fef7db9bbea7fadfcce47299aff6aea8162 Merge pull request #163 from xauthulei/output_fix
2fab616935f96c24899a8f98d503431ae553e9f5 Merge pull request #164 from elgnay/feature-discovery-addon
953dfb325df98b1c5db6635bfb99ca9b1af2a49f Add controller to generate addon label on cluster
8f40126c3209b99aa68967159ca4a19e892f3b85 add the missed step and correct output message
a61896395f4bd6156693def26a652d6ee2e5442d Merge pull request #158 from zhujian7/test-clean
8361b012faf212ae6e9a40870d85a6cc3e606f69 add skeeey as owner
4a429051a7631ed09c071201cd14c98d417eff9b Merge pull request #161 from huiwq1990/bugfix-cleanup
d9653368a277dd451b95b8a3851fb06f3d473873 fix spell
4cecc9c399e3ef62c390a45004a33371115a51cf Merge pull request #160 from zhujian7/flaky-test
c74d1b95219862873dbbfe62d28abb511c49f7b3 test: address flaky e2e test
44ae449697523c25e670a070fef41cc1b5eb3c8e test: clean up remains of the e2e tests
d2e5e11047a1e7d062d36a32dbdd6172b67ce1f8 Merge pull request #157 from zhiweiyin318/update-readme
c8d94d058d7b31eeed83a4d9d6ce76e757d9f507 update readme
3ef70f7804615bfbae597a9780bb5feee6f7eedb Merge pull request #156 from zhujian7/rename-demo-cluster
b31f842424401ec1ec0f9fe34584afd536701181 change demo cluster name to cluster1
85f1e3d26445f34f0ea4f5d0f73a69a04d21ba53 Merge pull request #155 from zhiweiyin318/release-job
9fdd9f7abe2ddf82dee16e686ee2a54226ef3e8c add release action job
e6435f32a3ed877b974f3299bd26db1101162f7b Merge pull request #153 from qiujian16/update-deps
f3ea6c5d99ad775bfcfba4b1af387cc4702b4fa3 update deps and enable action
994e91d6f012e166287b02b9b2a83bd1e453b97a Merge pull request #152 from xuezhaojun/fix_kustomize
05249c53565fefa487694fd947e3a83e09f431b0 Merge pull request #151 from xuezhaojun/fix_auto_code_test
954492b65e77945f166c0df9a7bb0664fbfb2e9b change related path to absolute path
d0f6fb7c84d30ceb07355a3151bb2c6fe090a17b Fix issues in unit-test and e2e-test
59d53a963f66f973c4ce8051ef29ec91356b5e92 Merge pull request #150 from skeeey/update-readme
2429fa3a19af7e904bf197b3a8533ac8b1a5c483 keep compatibility with lease API
65bed99bb5a71e5826d759b4ffc715ef9cc23035 Merge pull request #149 from skeeey/update-readme
5a2ec4d0d517de6b40409c773ad49ee31d21964f update readme
f04906dad7106a81be9d32be0d0d3d62e91f2a58 Merge pull request #148 from zhiweiyin318/update-crds
1a8ebccf52c47a50944f80d0c655846ba824d2b7 update crds
11bab943e6671e781fedef4ab19d3c055336a534 Merge pull request #147 from skeeey/update-addon-lease-msg
b4ee95f2c60e711b59cfaee3c9f9a6b1635f6d4e update addon lease msg
081083f3da8987cdb073b903989ee425aadfab15 Merge pull request #146 from zhiweiyin318/clusterclaim
e89b80796632ab5dd844ed1e1d45e78c7d8410ff expose clusterclaims by label customized-only
e83faae5f8b9646e0244f180839e38e186dcffc4 Merge pull request #144 from zhiweiyin318/gomod
726c0fd7220ff8589b21422aa6fb76336caaf416 update go.mod using go 1.16
0e7179dd1edc1d35325fb9d657de959cd71902c2 Merge pull request #142 from xuezhaojun/changeGolangVersion
49164752be9d23848949c59c6a1de4b28451cd17 change go.mod go version to 1.16
6527dce420bcace21b80d8c7f8e023a5f8a98f6a Merge pull request #143 from skeeey/fix-typo
4cc16e3ef90ae98761168a7e6a2c4d773bf041a4 fix lease update event reason typo
1532cac576a87cebd65ce1cfad3459d70d872cce Merge pull request #141 from skeeey/merge-managedcluster-status
35a86574a70c08abb1fdfb54a2c6b922f2441316 merge managed cluster capacity status
a2bb6439160edafaa94610883cd2f582485b5298 Merge pull request #140 from elgnay/issue_11821
0422969592a1fb27b1009fbd677ba3d1b05df107 reset csr name only if csr sync failed or secret saved
74be9e3e4ce39734c2d39b195d71306e12028f33 Merge pull request #138 from elgnay/addon-resync
5cde8b5021eedb964b42e49ea0433cc58cb1b71a add resync logic for addon
18c612cd5850ca698aeef8c4f7bb181360292e33 Merge pull request #137 from zhiweiyin318/sonar
1ee7fdf8e109eaf0a8a32e60e430f73cf433c65f add sonar project properties
eaab210e7fa58e79944a5d5557bc1341de9b98da Merge pull request #136 from elgnay/update_controller_name
63bc28fa1ea298d8bb2a8bd06d55cf39a6c162d2 include cluster name in name of client cert controller
f6d45dab3c8888ecd2e27571f3b52577c87e53fd Merge pull request #135 from zhiweiyin318/non-root
54160128dd9641f37196f8dd3b89236df0ccb557 run as non-root
a427380e48fc899511584e37265c714c6a0255c5 Merge pull request #133 from skeeey/update-addon-api
1d1bcdc1ddf8771a5ca6ab2198c82b4597e15ba9 Merge pull request #134 from marcolan018/noop
e0d9377341a60ec691bee0f6179d722ec6026681 touch readme as noop Signed-off-by: Marco <llan@redhat.com>
a9f8c56a918cf1e8180c0b43730786d2b070e18d update addon enquque ns and addon  update message
ea0875682b8f9e522269141b11d32ea959122518 Merge pull request #130 from elgnay/add-dns-names
ad99b65e47e8181cafb1e36f71f0ca57bc29806e Support DNS names of client cert
c3338def027bac1816fa3b3cda503498854e7fd6 Merge pull request #129 from skeeey/update-addon-api
7daeb081bc7d0432c440e1f6206e67ae4c9f3b77 update addon api
96b77b70f9d900ac31d18cc0699ef517648f02cd Merge pull request #127 from qiujian16/csr-v1
1c73301a10ecf8233e77659ac10d9dcc7375cf77 Upgrade csr to v1
8d11c41855565ca8edb0c4993087788eb6df18cd Merge pull request #123 from elgnay/addon-registration-part2
cf82b7805982317867771ce41c285334fe7b165d Support addon registration
4fbce67b4651cbfb209aafe4dc39592b5a0a5482 Merge pull request #128 from skeeey/addon-manager-lease
b245eac0aaa442d8c56d5ed9f790a6ca50478a57 addon lease - compatibility
9e9a0f1c7ea4b7a8b663aaab7d06944adf77cd06 Merge pull request #125 from zhiweiyin318/webhook-v1
0488389c698be1825014fb8d9dfd258e4c0739b8 Merge pull request #126 from elgnay/issue_invalid_cert
f89bc0033832077e7266798fab53369c60bfb189 upgrade CRD to v1 and k8s lib to 1.20.0
0d6abef9a0253552dbafede8aa9189366e5a99f2 Fix invalid client certificate issue
3c442daf803013081880aa7457fe0316e5f73354 Merge pull request #119 from skeeey/addon-manager-lease
2b4c9f1abdb1a7c29d2959496d5185b766c9abd2 addon manager lease
21c59fd18cb2093fba08f3078fc6ccc5a39bc82a Merge pull request #120 from elgnay/addon-registration
097defd9009249e009308419cb5c79fe36579e13 Merge pull request #122 from skeeey/encapsulating-cluster-name
e60ca0e385c9387fa2cea481bbeabb392943e33c using double quote to encapsulate cluster name
5b80d01b7269e0d8767ae5098ad47459a23099c8 Refactor and make client cert controller reusable
9a7a613a54cb81974cea5c08ae78df1f353fd0db Merge pull request #118 from skeeey/livez
5626eaa6cd9c86c13e546bdeb2d16570cb93d891 using livez instead of readyz
08d8569c94bedfbe355e4d8a3930fce1bcccac8b Merge pull request #117 from skeeey/roles-replacement
2006c4ed4bc03587bfecff8c6ca5e68941a49173 update rolebinding name
dd31f33946c0195901d58c6ee86b36d590f4889e Merge pull request #116 from skeeey/roles-replacement
cc4f6687b60a42307d794bfd976893bbe7177ecd using clusterrole instead of role
3366326fbf70b2e91cfb80bcc82c3291f1f4cbd7 Merge pull request #115 from yue9944882/cluster-claim-feature-gate
b4097f91bc3fb52eaf4333edf06658932cb73ec0 introducing ClusterClaim feature gate to opt-out from list-watching cluster-claims
fa938afd0d56ff2e2dcbfb31a5b09ec7c2f8ba14 Merge pull request #113 from zhiweiyin318/upgrade-go
f99fc592b5a30b471cea3eeadee7b3870503e333 promote go to 1.15
4839ac6a02e203bd4efb823d4d9f7ec38bb0aacc Merge pull request #112 from yue9944882/adding-spoke-cluster-common-group
842d4bb15e48952cc52afd290c324cc135440510 addressing review comments
a13f3780cd23d923a4da1d19d61fad2ea48e2fca defing a common user-group to match all spoke-clusters
a51d4fd48935c78674682d080a10402a85c45795 Merge pull request #110 from elgnay/issue_8687
1649df933e54f0882a8aeb02b8ca2d9f2090a59d se Lister to reduce the number of calls to api server
0e19e9fbd39285e15d45ec9d282700c31fdc2a4c Merge pull request #109 from yue9944882/feat/namespaced-secret-informers
4bc194d7912ae6d245d4a832d0c512d5a5aad21c namespaced secret list-watching
fa7af8541ce2ea30c9c160ca43ea3e6d6d568541 Merge pull request #108 from skeeey/enhance-doc
52173e687b4a38a1d42e18e114c59764cbabe6fd Merge pull request #106 from elgnay/upgrad_kube_lib_to_0.19.5
43212d5fbb389ab05cd762ba59aed77531c4e203 add doc for clusters time synchronous
9d13cd52999cac810ae63df728c46dbcddb287f2 Merge pull request #105 from elgnay/issue_7679
382594e4aad3f924f26088919526d6d27933b9fb Refine the logic to get agent name
83ac7ef0bf86224708f2c43e393ad1107cd9f08f Upgrade kube lib to 0.19.5
cff030cef86d505d4151d631d704e55a84b9c491 Merge pull request #104 from skeeey/rbac-accept
bb9f76595a491dc15ab53d4df7a38d091a6fe3c0 check resource name for cluster accept
cb5438b24fe104fdadf6fd0532a8c1d84fdfd023 Merge pull request #103 from skeeey/update-unknow-condition
dfb9db8f61ae0e50be7aa28d47ae1b8724a695b1 update managed cluster unknown condition message
8ea6273fbec207d5d235181a7eb320968a11be25 Merge pull request #92 from qiujian16/eventfilter
e6a8104c70e2fd9edd8d58fc0409960c9c6693da Merge pull request #101 from qiujian16/fix-panic
efc2acdfb28e5fd2bd4ff144ba0de655bc8df6fa Use eventfilterinformer
b8d551acbd76536c43f361e88dde1d1a229ddf39 Fix panic when cachesync timeout
7a90dd44e2bacc85dbddf7aab56edc5c103d0bde Merge pull request #99 from elgnay/max_custom_cluster_claims
dea3c48998309d5e891ba489a539eee26153c2bb Replace flag cluster-claims-max with max-custom-cluster-claims
9970e648ea2c61f6c0e11076e32383a246b38a68 Merge pull request #98 from elgnay/update_clusterclaim_doc
2a4b575ea83ec0be149866ebaa55b1be9dbd8886 Update comments for cluster claim controller
f309670859238d0bef128224086f5ed9560f447d Merge pull request #97 from elgnay/clusterclaim
521391447a11b3df546dd6a66adbe3ed9f8a12de Merge pull request #96 from yue9944882/rbac/managedcluster-rbac-escalation
bf8ab7504d1cff1efb8ec45823d14e53bc7ad79b rbac escalation for granting per-cluster rbac-rules to managedclusters
0d23f35e03b8a054daa56354a598510ad509c753 Add ClusterClaim controller
5ffcb4a63a03034a450284494c559bbd5e481583 Merge pull request #95 from skeeey/contributing
03b02f2cf289144a8b6fecf9f337cb5cef87ab07 increase qps and burst
86c110e488642ef8d8ab09fc67fc2f2cd0831e38 Merge pull request #94 from skeeey/contributing
979f3b6e77a582d4d3f613cddafdb48ac0d576fa update contributing guide
f63d3f83651a8d988f1968c920c61c6a29ef31f0 Merge pull request #93 from skeeey/metrics-permission
06496a4bebd271dfcd02528fa0cc593950f9d9a7 add metrics permissions
c6dda84ad8f1811a9090f43111b593bbe443c4b6 Merge pull request #89 from skeeey/updateapiserver
7bc76ce2df367fb8f98bb23913d01a1ed8bc98ce temporary fix kubeapiserver issue
7982eb0444482219d29e8abccff5eebb04ddf49a Merge pull request #88 from skeeey/addwriteaccess
6986b0bbf35946c9bb8854517bc0b73e48e4cde6 add write access for hub kubeconfig file
a8c48690ac57f08173a8198047c29cfc7fbffd93 Merge pull request #87 from skeeey/sync-hubsecret
a698532361fc5bbf4d208fcba5c21b247f85869b resync hub secret
e87ccd2295406175d15ace01a2a90163f322c486 Merge pull request #84 from skeeey/enhance-recovery-integration-test
f1007e3eac5dea3f7f208fdfe543fb826f3373d7 enhance agent recovery integration test
8c0865cf3cacfb173064ef49a5e0fe5bb8c65ff3 Merge pull request #82 from skeeey/code_sc
4f0bf3487a33e370741820a1f36a7a035a5f5220 using get instead of list cache
90cef8848bdb6ed91e54e945e0aec8dd79adaaa8 Merge pull request #81 from skeeey/code_sc
cf83b2e2332fc7e2b0fa6d3d4fd02a7fad8a041a fix code static scan problem
515483ab4705a54b3a882dee012f9323e5960de9 Merge pull request #79 from elgnay/clusterset-exclusive
605e99100f0296bbb2f1d659a84cf7111081511b Make ManagedClusterSet exclusive
63a5936bcfcb26a3fec408d8b1158a8ea30c600d Merge pull request #78 from skeeey/backward-compatible
3584194d1681264cae0a3c93b3d54b8537f31df7 rollback LeaseDurationSeconds code for backward compatible
bfdfa033e1044dd1b2ee8807730617aede8432bd Merge pull request #77 from elgnay/separate-e2e-build
772bbcad161a736429e27a2297b9deeb87a2d032 Merge pull request #76 from skeeey/performance
54dfe6529d993ded13e6dfe0a5fcdcc398d4e57d Build e2e binary separately
c1977526e005232df46155075047cb989d9c417f rollback init clusername and agentname in secret
ce8a848e7f428d5a654e5c0afa7d2922e5d4d392 Merge pull request #75 from skeeey/performance
cc0823f8fbc08f21668d217b5b6126733c3a02dd add secret controller to fix performace problem
e8bef5622ef5ac8902ada437a4be8e676d53e32c Merge pull request #71 from skeeey/code_scan
a01b1783be6e8d5889c9bde0b3acd69bd0a162bf fix code scan issue
58409319bae01b8e30ba69a95418cbcdbf6320a9 Merge pull request #70 from zhiweiyin318/build-e2e
b377b16181a29511d49db2d712d7ac5835f05302 update build-e2e cmd
53c88c8053f5d3e20c2ea883a8da4ab443e638a1 Merge pull request #69 from qiujian16/adoptmetav1condition
8eee196e80a73cac43bd37b3fdb421bdeabbec90 Adopt metav1 condition
27b78f7f48588a09db9aebdb81089f8f5bb0097a Merge pull request #68 from skeeey/fastforward-test
9f23b69f31f489d5b7b62521e804cc3c87b4db74 fast-forward test
bbf3bda0a10cb2cf217d1cfa337ff6d65e66f8c2 Merge pull request #67 from elgnay/csb-webhook
ef4c17017d1113c01b9c8ec62dd95d68f1baceb6 Add validating webhook for ManagedClusterSetBinding
72b3890c7b55a462090200d622c912fd8cc01178 Merge pull request #66 from elgnay/clusterset-controller
74f73db5844a6555ae8d8729bcc650a911908332 Add controller for ManagedClusterSet
6de37157d99e499b7c7e80b1889034a06295aebb Merge pull request #64 from skeeey/add-license
398884541b6005bd1f72b9f2255ac143cfef89a4 add license
cdcc6a0d820dfbe675257b2ba6e725798631837b Merge pull request #63 from skeeey/mutating_webhook
973eb321ee3436450b2ee9646f1a28da7c053c1e add mutating webhook
24f1452943810a72bb75e51ff2545b928497ba60 Merge pull request #62 from skeeey/update-readme
8a571edce547237df6f7e6d3f00275266fa28e22 update readme
03a8ab3837a3018882e0458db3e845dc4a17a8f5 Merge pull request #61 from skeeey/update-readme
7365598b8a5aaef28702fa06bc70aed48813a7e2 add how to deploy webhook
623ad025aefab3ba204c7b3e85aedc761ca9c5ee Merge pull request #60 from skeeey/update-readme
38ef972b755fc130d030cad219ccfcde5d62d3bc update readme
a16b934a039dfd37936dae5dee02be97ed391797 Merge pull request #59 from skeeey/approve-cert
41975226d6ee813696f91a0d9d51128632622090 fix issue 3589
23d973209d124637f2cc304a6bcad76f076cc867 Merge pull request #57 from skeeey/refactor-unit-test
13bcbc7396cfd62927ed892c9ed8067fdbcaed0f reorganize ut common functions and improve test coverage
6b1700fc1145348adb96f59144ed3a369f8ac669 Merge pull request #58 from pmorie/jqiu-owners
b933f37db796259f46218d8d9a269d92fa47b9dc Merge pull request #56 from skeeey/replace-cluster-admin
cdeae2cadbad52f3c21f64445db9267ded9531ce Add jqiu to OWNERS
556ef10019381e218a52dad38847d54b8ce50d79 using specific role instead of cluster admin
55523640c400003e552c4cd231c9c6875cc0d269 Merge pull request #55 from zhiweiyin318/rename-role
b9ac928b173ba49556c5f5852d589d12c6d84293 Merge pull request #54 from skeeey/readyz-forbiden
69b1170862820e026150e021f3d17efcc20d7184 rename clusterrole and clusterrolebinding
dcc1b27a1419b5d2f00474cee7f19c9638f529fc try healthz api
3af1c0a2896b7a367c6df7d9c89c523941505cda Merge pull request #52 from skeeey/try-healthz
93375a25771514ada034244166cae809849d4142 try healthz api
b43524d31513ca161d4769fbddb1fb4d851963a8 Merge pull request #50 from skeeey/keeping-namespace
3de9f2f2e57733775eff73c53a280d138d569629 keep namespace
64968c8f022065b813e770a92478080baea3303a Merge pull request #48 from qiujian16/managed-cluster
ad1d18368c45a913e80363d7b321684db55620b0 clean manifestwork when cluster is deleted
560cc6a2f90ac7b1a21c87fc1c5a7fb3f3a71702 Merge pull request #49 from skeeey/delete-roles
8175ffba1b92b96d757cc5ecf6c8ba1b14d43fbd deleting managed cluster
47720cd0268a81989998deb282de6ae9acc682cb Merge pull request #46 from zhiweiyin318/fix-conflict
cf4f96310b47e8f4fee3a4f620a29ad6716d7aef Merge pull request #45 from elgnay/add-finalizer-to-role
0a74648f0fcd2754511b036a36cf950068c0954d fix fails when retry on conflict
2af30730842106b13415816c2ac894cc6b6811aa Add finalizer to role/rolebinding for work agent
4c6c28ec97a6b1523b468b19fa9a90b642b2f525 Merge pull request #44 from skeeey/heartbeat-e2e
c87bf16c987b5f7c44630801dd085a7b7e4affa5 add heartbeat e2e test case
f6e1aedaf4a59a853fa980845ded6ee7971a7873 Merge pull request #42 from skeeey/update-image
f1fdd1c7c1094a788aa4a4986306e00696d06468 Merge pull request #43 from skeeey/pr40-followup
dc1157baace9fcc7ddde8d4bf5e5909f2a011cd6 resovle the remain comments in pr40
9ca71416ceaefb9c06c06b3033887ab0a14e29a4 Merge pull request #40 from skeeey/heartbeat
da22ced80946ca6fa00180180dbb4316f713db82 update base image
eb81c7fe3e0d78b7ca649d00be0872e3801ad022 implement spoke cluster available check
1802ccb34e2e83c992428976455acde84aa8914d Merge pull request #41 from qiujian16/managed-cluster
b7ea8a2eab11ab67dd5c49a45cb9ef1f9b0ef3ff Change spokecluster to managedcluster
ca3b83c1ad7af9f9ba8e5b3f57c182e0624251af Merge pull request #37 from skeeey/webhook-e2e-cases
77fbb76450732cdb1e424feddf97e768cdc1a2f6 add webhook e2e test cases
dae105b06d28f06698b63766aba795fe642a48a7 Merge pull request #39 from qiujian16/security
af5a4f75a379ae6b67dbf32fffca839e0614131f Add security policy doc
fd1ee8b4dc5469941d0d08d50c188e36c4e7ea83 Merge pull request #38 from pmorie/wire-e2e-image
14ca44721686b1b5d9466819d54a825885a8e240 Fix wiring image built in CI to e2e test
1b39448e2bc5fb4ab24b734a5fc437181fb7eb98 Merge pull request #36 from pmorie/prereqs
3da09886916ce6d9ca14d83b34aad500ddc14adb Add information about prerequisites for running README instructions
9abef05cc00c8c9a3bc06839c7fecb491186032f Merge pull request #35 from pmorie/e2e-image
07730dee845007c1eb9f411b83f81136b60b1d90 Add e2e binary to registration image
d570bfedbd358564beccf7870bf793da342542f8 Merge pull request #19 from skeeey/adding-integration-test
0a6f161017cbacb8a1c0730baf77b944cfe0a017 Merge pull request #27 from skeeey/webhook
354e78e1a3dd218a7653cd58ddf70870156a1dfa Merge pull request #32 from elgnay/update-spoke-work-role
ff2a3ea5a98072e7dde6282d48e156da547ef7ee Merge pull request #33 from pmorie/kubectl
065e130b3786f2c3c331e72d1d50b706a70fcb5b Fix some missed invocations of kubectl
496a8476035b1ddaf6edc12dddcbb835943ab665 Allow spoke work agent to update manifestworks
cffcbd7691f14227f8010ccea59603b6ca445b8c add spokecluster admission hook
a09ef1620f168d220bf4a2370346228b8c175696 add integration test cases
9eb1f2cd01e6e31f16224614c7b0ee7035e4a488 Merge pull request #31 from pmorie/e2e
df7c586bca9c52b147a5a1c70fd7c7f5688a9a86 Merge pull request #28 from qiujian16/update-agent-role
270d5c58de4c74d3d417d72fde00daa743aa3088 Fix a couple missed kustomize invocations
c95ed71a827f9e08323cbc995ef069fa5a34f134 Merge pull request #30 from qiujian16/ensure-kustomize
97c25433c26410fcc1322f662a5e54a6d84b42c0 Add ensure kustomize target
fb20b5005ab50ae5f4ca0a1da06e5cfa0ca2e8f3 add spokecluster admission hook
b6b71113d5ba3d95bf6583d0a53ef6c9380a4684 Merge pull request #23 from pmorie/e2e
0347ec747fa36f313d996e5403ddde6c0b0bffd3 Add simple e2e for local deployment
766ed5fa7d3dd42220554ce68dba461c343ebf4b Merge pull request #29 from qiujian16/set-images
72b7a2d9acce4ffcafac9e567f3d04e00324917f Update image when deploy
9b8b810dec919b93bc7cd275e901f6b383a76037 Add rules for agent
1e4da015679134f13c2482129e018d197ae4733c Merge pull request #26 from skeeey/options-fields
66b600c9a7c891faaec240aa1d3715f2ac6dc017 add field selector for shared informer factory
319b53409cc0278b39e469811e8fb04869000d66 Merge pull request #24 from skeeey/fix-clusterrole-error
8bb40e273969189ef326e754a7bdd928681efb6a add field selector for shared informer factory
722f0197452c9fe721a4841b9b12c0776f0aee56 add field selector for shared informer factory
d05b0158e52b424bf6397de71d25c75a148ddeed Merge pull request #25 from skeeey/rename-component
4c5ce24eddf8058d140c78f835506e512b5deaea use a specific for registration components
e925c1e48b185f7f83e19b433584c7ab15946b11 Merge pull request #22 from pmorie/gitignore
23fd1f7ee6823b9415d217137bc768719f18be94 Add integration.test binary to gitignore
277d54d672fbda1bbc71c2d7ffaeae813b51dd65 Merge pull request #21 from pmorie/dev-deploy
f2855617e57dacdebf60c8b3a4121794d78fafd8 Streamline dev deployment
55b5f85568e081f9d823ba8b9c883b902aa52ede Merge pull request #20 from qiujian16/deploy-manifest
2e87d3a92c9404e709b8ed77a9f4ffaacccc7611 Add deploy manifest
5aa4136e75635437647117ac52d42d080e572d1e Merge pull request #17 from skeeey/creating-spokecluster
ecfd72cf7026ebb62c90c0e7f6ad57c95a45b680 rewrite spoke cluster creating process
e4f98c1d4086a3eddbc28504da358176336a07ad Merge branch 'master' into creating-spokecluster
77c646b9a14a428101be462bda4cac2f646bd343 rewrite spoke cluster creating process
e62c5cb68970a6863a0bfae2e8cfc98a9fbcaac4 Merge pull request #18 from skeeey/prepare-integration-test
bb85ce25a376ce2e96c36d640cb13d7bf5e49642 rewrite spoke cluster creating process
70bcc1e1a61484129829310794be42c6f6972b79 prepare integration test
6dc650cd53b6f23989b2412ebceef698519db42a prepare integration test
64f13d666402a673c77b09e21ce3e7ba1ffdd3c2 prepare integration test
6d1cb006ba30effb10a10ebd71cfadfa3cdc0c03 prepare integration test
6584baa5abd06426d6732ecb56558a36da0efb79 rewrite spoke cluster creating process
fed340aca8bb99e60891817e0b74de925183a78c Merge pull request #15 from skeeey/agent-controller
04192b6eb3ca93f8d704768fe3363d807e468d3a resolve comments
2e3e5b0908d678478698f082bad3982ceae1917e resolve comments
777555aabba4c9f77975252ffec89d455fe790f6 Merge branch 'master' into agent-controller
1f334864eb112064aa56b6b371392a75db1c01f7 resolve comments on pr 11 and 8
697526b8eb8ecfe6fd0ce3af592a42b9d9dd237c Merge pull request #8 from skeeey/csr-approving
be939d6db2991c2ae29e670ceb66a8ab6b8030b2 Merge pull request #16 from pmorie/readme
9c2a67e79b1a27b3fd4eee2c01304a44b675f2f8 Tiny update to README
db1efe7f826b110718c13a0833c3b4740f6153a8 Merge pull request #14 from qiujian16/dockerfile
ec4451570a58690b094b298b55a64aa0c4cb40dc Add docker file
11a00af2d76d1f984db0115e04e65abf001f05fe csr approving controller
3086bf0aa6b5e281605aa28d159eb1888cd79edb csr approving controller
b9987b4ec29ba168ca8e2c88e2682915fede974f Merge branch 'master' into csr-approving
abd503efddc6ea92bd20a096a89a9add3fbb53a4 Merge pull request #11 from skeeey/agent-spokecluster
eb601547e7f8ca8641990689094e9c822576e539 spoke agent spoke cluster controller
ccc2a489e7bea16a941c813fabfa8b11b36ddbc0 hub csr controller
050e191e73777e47e14809878917aea298fa1bd2 Merge pull request #12 from pmorie/doc-fixes
92900f589a9f7542746915a47782bea7db03aa25 Add / tune up godoc
15a0c82c2c087d2880f77b697ec54e7786b2f409 Merge pull request #7 from skeeey/master
6c93f9fbdb40d00ebbfdc35190fb98f6a36e1df0 implement the hub SpokeCluster controller
66e04ddaf4dcddae1b1c8779c306863a2550d20d implement the hub SpokeCluster controller
1fc7b29a1eef272fa1668d8a4a94c3af4c1ed17a Merge pull request #10 from elgnay/bootstrap-fixup
ef9e7118f69bae934a950c22189efee4535ff8e0 Merge pull request #9 from open-cluster-management/mdelder-update-readme
0d2c23bbd2129105198219272d6ddc126aee6452 Update README
64ac9f6afbc7c4bf42d16093428790e91bccc9f2 Address the remaining comments on PR #6
4eff354d2a8f440768596291b14b6981ea114503 Merge pull request #6 from elgnay/bootstrap
e2c4053474e3d9f1139750d9b6fd4dd288365bf3 Remove LoadClientConfig() and add fallback for fetching csr
08e5e70c65c9ab213756d8f6f3bee3d00150a69c Correct typos & remove time.Sleep() from test cases
521a1de694a62b8ac0bcf1d95b30a2ec08e98ef7 Refine code on comments & commit files in vendor
438c562e56fe4ac857287985786a0676044733b7 Run ClientCertForHubController twice
ed52cc9c530678a16e91c8d935be98e64a980c8b Simplify the controller logic
2fad764a1277a32e6eaa0b406796d6ef3867c5d9 Implement bootstrap & cert rotation as controller
ba7a116b9c133748d58d1a106cde254645869b70 Rename bootstrap package & remove waitForServer
8cdb59f01b611c2a510ef0404ad5b08e83dc7cf1 Add unit test cases
185bb8750eb2c4e8e5f1c605c4c616fc18abaaa4 Add agent bootstrap & cert-rotation
0416a6b1f415800b48fe76ba5c42ca6b0ef8dd4d Merge pull request #5 from pmorie/owners
2487c6fac4d8dd236834e874a9a77af84d5b29ce Add owners files
0fd557261be54f6910e47abbbc74f6be7b21ad53 Merge pull request #3 from pmorie/missing-file
a5a780c5561b9d84f58d3ff475dbb664bfd48335 Missed test file
73571031870fd48706e35bd48b2538aedc95b981 Merge pull request #2 from pmorie/build-machinery
39c01a03415ee849e54568ecbec1713a31b1a5e4 Add build machinery
8730c7cb848ce8794315e5893191598dabd47187 Merge pull request #1 from qiujian16/registration-ctrl
aacb7b4293a27d9f9d69f4021ba5c0226264447b Add basic cmd and pkg for regitstration controller/agent
b3484a7ee64d3a44a7345bffed0d6c3d93c71fec Initial commit
```

Status: Syncing successful
