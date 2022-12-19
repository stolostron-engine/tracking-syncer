## Syncing stolostron/registration-operator with stolostron-engine/registration-operator

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 383 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
c7bd5f48a96df6ceb1a55e21e3723bf5b24b9e95 Merge branch 'open-cluster-management-io:main' into main
c3baabeec29f1c2dc183ed5ebcad298204ecffe2 use crd manager to update and clean crds (#297)
4264c7d22c75f9c2c17f5cac6cf0fea0fb65846a upgrade github action (#308)
5459ac86e723237b0c5f9ccfba7c9a74d69f5043 Add test case for hubConfigSecretMissing case. (#307)
1ab08bd6d7e372f952acea8f682af37145c379ba Make work agent feature gate configurable (#303)
e12657c501561f9edb26c7867846d4686427a46f Refactor klusterlet (#306)
94f17dedd114a625adcc23e7c1cbfae9112574ad Refactor clustermanager controller (#305)
7c8d71e1949b601d42b962dbc411646f938feb28 use controller-runtime webhook (#293)
fbeb0e224df54daa61cc3c3b8b807c6be5a8b65a Upgrade ginkgo to v2. (#301)
3d591bb11b9fa04f5c51ccde71c173370343306e update clustermanangementaddon api (#300)
514fff1469e223a9696ba467b520651f9f6b8e26 upgrade appliedmanifestwork API (#298)
5e11092b0ef375336ff2002beed1d9896c1aeefb update changelog 0.9.1 (#295)
3f119fdefe3529edfb68823b1bcb92c2d69f9df7 Fix the paradox description of the klusterlet condition (#290)
b963a76b85805cccefed393ed28d1dff935f6c8e bump to 0.10.0 (#291)
7e12d497ff0f8bd5245fd45d3ff0f113c21a5e33 upgrade go to 1.19 (#286)
29011c8e1719d2b2029911abff657866fd0d6ae3 correct managed cluster lease name (#287)
919dae608dfe9cba54810770165dbb16220c6765 add changelog 0.9 (#285)
820d5b0149bc45a6097e0555b88a662fd3737bb2 fix conversion webhook in hosted mode (#280)
fbbb5d9f48c0aeeaad02bf88bd0c026a5a3cc8b2 Fix token path in hosted mode (#284)
432fac361695c5a03aed8438124d97e04e4dc06f Remove install mode detached (#282)
8745a76e6b40f7704a9e597e0d1de33299a8332c remove clusterrole/role cleanBeforeApply code added in ocm 0.8.0 (#283)
57463accd591668d129b79cdb3d9cd71ab2ed5b9 update clusterrole in olm-catalog (#281)
6bf6df2f2c6859aab66a28e88526fee274a24c72 add conversion webhook (#279)
eb6105dd080d340179011a9f2ff3271b61b00deb remove API Placement PlacementDecision ClusterSet ClusterSetBinding API version v1alpha1 (#278)
79c6b55faef94d1a456cbfaeaa67f2d9f21dc89a Fix: delete addon crd at first (#277)
0944f98904182172983c4e121960f578dd0b0beb Make work webhook feature gate configurable (#276)
e1bf8191f3852ec4671cc7c4a3cb7717a4c24758 Allow work agent to impersonate serviceaccount (#275)
3d0b5cd21979efd2ddb89709ed35b0f9d8b2755f Allow work agent to create subjectaccessreviews (#273)
ca32de775bb7c170cbcc836b21856b5c4fd318d2 add skip-remove-crds option for cluster-manager, to choose if skip removing CRDs when ClusterManager is deleting (#274)
0f5141c5fc1ac8896050e399256e54348e5e9985 update add-on configuration apis (#272)
4306b7849a14b36aa25704d8fb83c643f2f352e6 Use the correct managed cluster name in the apply-spoke-cr-hosted target (#266)
b004bcc6143e745bcb47d5c05e8ca30ccd7a6b9a Apply only when having finalizer (#270)
59b5e56fd32aee42cb9f4af1f708599028392290 Refactor to split two controllers to handle klusterlet deployment and cleanup (#269)
b14e41788a899eabe138f3f8b77864d75a059483 upgrade go lib to the latest version and bump csv to 0.9.0 (#265)
291f465601a8c81e21d2e6bd8f15efd167d56ee1 Allow OCM addons to setup metrics collection with Prometheus (#262)
c1fb03baf1c9af3da34d7ef5ccdfba19bc8403cc Fix release yaml (#263)
6c64bc33ca130ef0b3a631b30128ebf36c3d9fe6 add changelog v0.8 (#261)
79d280ad8a82055848a25bc9bcb83717f8db27e9 Add HubApiServerHostAlias for registration-agent and work-agent (#258)
de7ab7ad242fedcbb96a9a6356c1a353f843e9ec Add controller to sync image pull secret into addon namespaces. (#253)
a7dd402db878b3e40bfb95d1d35582d129250ea0 Use token request to sync sa (#259)
4b1061dda0a69ae5be05750f4d3f95621c1f0148 add permisson for registration agent for running addon in hosted mode (#256)
5ffe3b8a8bfb68e9e4a1588a7bf2e1b3397ed824 leader election needs to operate configmaps and leases (#260)
855199ea435914994296a3cd7f52e013a8968722 clean resource before apply new (#257)
91bc2dc7c70250061957b9a4dd7677afb53cf307 keep appliedmanifestwork & clusterclaim CRDs when unstalling klusterlet (#255)
803bfb374805414222e2aff669b73588dffe3537 split work permissions (#252)
54452f060af0a365ce8484ba724808a814f88204 split registration permissions (#250)
3401c8e4bdb09cd72b8bc628e7fed1b837b28d5b support hubRegistrationFeatureGates and spokeRegistrationFeatureGates (#230)
a6bb10cb90f7bf3eb2a909908113dfd9e1f7b15b enable log flags (#249)
9304a9cfab6236be369543adf1f8f161fdf11449 remove set join permission for registration-controller (#248)
5655fce48ea7b211f0b22a413c3a4b5215e5e130 Upgrade library and api (#247)
7f9988252c2acd8c16739db572a48b892ee4dd8d Upgrade golang to 1.18 (#246)
4f8ca8c6e3d18ee55d48f4fe5e0ab1b7a99314a2 Update file name to reflect the change in Makefile (#245)
11efeb18b59109ec015a4e7974dc9823f577acf7 Add goci lint. (#243)
25373ddab3527d79a824a29b820baff6306cb549 use new clusterset api (#242)
8503c1bd13a81ab200d15fa0e16777df5ebad5ed add all clusterset join permission (#241)
0637aee32bb6a8af0f5f427c0b8e3d745c6304ea Multi-arch support (#240)
796062f0c59b4b856ae2a9de0ad2b2e86c8ba226 passing IMAGE_TAG to make images (#239)
d3034fb33830412f1fb13f60187a8c4f106eaebf chore: prune unused dockerfile cmd (#238)
9f709acc2d11d57c8c7d296e2eb9f580a095a23d Update golang builder in Dockerfile (#237)
2d5ab901d91ea22e8642ed364d0e9297ba211168 add join permission on default clusterset (#236)
c93f5cefd28bb3807d238554915381826dddc37a add missing permission on kube v1.11.0 (#234)
d501691f1b609b9234a982506def3feda58f4802 add lease permissions for library-go update (#233)
fb61c5d97b66d62a25bdd8d8803f243a8bc01aab set replica to 1 if kube version < v1.14 (#232)
51b9c703f49db19e747a9120bd7693587903bc05 add permission for leases.coordination.k8s.io (#231)
dac47a160a3c4c232ad23bb66cd67355942bdfa5 upgrade lib (#228)
812b48298a92a8bc605ffdbca7eba1a60cef57d5 Add lease permission for leader election (#229)
ebf48bc123b476dbc589f724bf9df9fe69a8b273 support Klusterlet.Spec.Namespace in hosted mode (#227)
dafd1b5c4750d5cc84c94fae9963324b07cffaa1 bump csv to 0.8.0 (#226)
af313bb01cb4b748a1fbaf14ce2589d6c0e35f53 add changelog for v0.7.0 (#224)
fd1ee4950b903d5ec2f2a1d64df1ce6b759387db avoid building latest image in relase branch (#223)
7ecf9754aae9d0eabd4b102e250008e5e586abf8 Disable apf in webhook (#222)
a45f8bcc4be1ec48aeed52601ef7f4edffc39f0f Add disable-leader-election flag (#221)
7aa41cda650f229614aeca84bef06f82539b81af Add hosted mode in klusterlet (#220)
84e12c9197b49a0e482142127e6a292f5f2727f5 Change to hosted mode in cluster-manager (#219)
db866a58912a53be1e63d28f1bad7d2c9c0cc4e0 Upgrade api and library (#217)
78f2de10b1bf2fe90b5de3d1c3b8c5b6175a9f85 Add finalizer before creating clients (#216)
4389af934441dddcdf00e197f663e185ae3f249e Reduce resource request (#218)
30c516b48578eb781596a1edf0be9c5d81160dda fix typo (#214)
a67f11c21e5d591e10e0767f686f41a198ed766f only set work-agent replica 0 when hub-kubeconfig-secret is missing (#213)
bb76f8cb7c4047ca8793be2a292830e683ae733d trigger new build (#212)
cb5edd022267618bd264f2a2145a82e93acc66c9 Allow clusterName to be configurable (#211)
55bc274d795ad0befc71f05aecd08810a4abfba1 enable feature gate for registration webhook (#210)
c1b1067f54be39473b189b0aa34100814995e198 enable DefaultClusterSet feature gate (#209)
66e65a2fb7333284280d4353a44324a44ea4ff81 upgrade clusterset api (#208)
00fcdcd30ae0092336a5d3a34f998fdaffeff530 add detached mode to cluster-manager controller (#190)
71fcc78d5f3d2b4cf18f8095b8bed220a160382a Make the klusterlet install mode optional (#207)
c369b40475c10b4374fe012300d78e2063043fee Add ApplyEndpoints in helper (#206)
b14296345da7c2bb783838a4bd648971e2338c58 fix default mode (#204)
54b11ba5d9f22bfd826511c320ac37c85eedd2d5 add addonplacementscores permission for placement controller (#203)
61c96873b3ab6150c1d495b0e3868b7f550090ca Refactor on connecton check in klusterlet (#202)
d67b0fb905a0c8a3a905d7bde5bfd233f704fa82 Fix wrong replica in condition message (#201)
bd3c2bbaa643eafa7c7bf42bed98c035d63df871 fix csv base replace version (#200)
8108c8d35571981090e362c9b511bcf5e93b56e1 change a community builder image (#199)
e697e47989df36438ac8497d78ec345dfa58ba76 fixed can't get sa token secret when secret name is long (#197)
2c2316fafaa1b913474ae207ecbfaf68abb669a5 update placement and placementdecision to v1beta1 (#198)
9332a9dc04476c86ec9bb25c15e4c5b175191e50 bump csv to 0.7.0 (#195)
c24b2b845ffa2508cd090f7d6c25c39ead75b659 add changelog 0.6.0 (#194)
156867faf578802d9334e3004759605c20092aa9 Disable leader election when replica is 1 (#193)
68149432294161faf3f539cb16f053e5b0271024 scale up the work agent deployment after the hub-kuebeconfig-secret is created (#184)
06c7a7af058224e1bf0dfc87fe7a740ffe02acb7 upgrade go to 1.17 (#192)
e20d45af5968d696374a5ab69a24192c4e70c6b2 add nil check for nil clients (#191)
bdb3f3f37a53ca492a9373cc410834d7fc867878 add detached mode to migration controller (#188)
4fb63d020f3427734b9f075d9b51c86c3d89ba92 add makefile commands for detached cluster manager (#186)
b181f4d6dda82d7dda1838f890a64ba9a5dec2c3 remove unused field in clustermanager controller (#189)
50f1e8410a024fe9e0ca179973ad850fa5b5414b add addonplacementscore (#187)
00c6bb1d89393eb93acf7141d70efc9043223f61 adding an option that skips placeholder hub secret (#185)
f7ff0557dfda3730844d7f912514942eb777e975 get the namespace of klusterlet from helper (#181)
672427f49c25f299a61c02d5781d49d6fc0ea6d2 upgrade api and support managedcluster taint (#183)
f456cceff3385ca53a152ec5cef36e79a1488e4c update README for running klusterlet in detached mode (#180)
7b1f04487528e336c6b30b0563d252a5a858ce86 support customize cluster manager namespace (#179)
dcf93fa3b9d6a55dd7f800b2af6a9e42d3efa01a support deploy klusterlet outside of managed cluster (#172)
de480a025000f0030d595a2a736b12a9cf60787d fix-apiservice-always-reapply-issue (#178)
c90d98e6dac14b2907aad9d2686e7dad600ab958 update api dependency (#177)
d8cd7736fca21410cdc97fdecbf6f00e8b7f2f45 add sa syncer (#176)
f8309d6855f59816f311ab2196d1f0985e4c1028 update open-cluster-management.io API (#175)
4b1593db741b68bd1c97cfbbb323f5e97a9b7811 line 48: modified the assignment symbol for HUB_KUBECONFIG (#174)
4ee4d15544b43ece144776c5e6fe475f1537f9d3 update relatedResources in clusterManager and kluterler (#173)
95b7ef4fda818d499732603dd51336982afb62bf Modify <What is next> approve csr related content (#171)
15b74555fb278b068f4e63faf344297d3878f492 reduce the sar request when hub kubeconfig is valid (#160)
e95536e76f3dc4aa32defeea5ab918f9b30b6d73 Update securitymd to refer to the  OCM community security md file (#161)
b3b727d8d7e59a768bdf7c37e4e9bcfcfd2943b4 bump olm bundle to 0.6.0 (#156)
9d26a497a683de1fd93660815b75e8eb10a1b5ac update changelog v0.5 (#155)
9c5338b282bef2bfef410d20596504ff849c3e23 fix resource pressure on hub when too many managed cluster registrate at once (#152)
5194011a037c03a93a989b249be011810e006988 Merge pull request #153 from haoqing0110/br_placement
34cca64b37bb5149bf96b202795a393e53248b5b update placement API
be297912783d42ab116fc44542e507d3934f699b Merge pull request #151 from kim-fitness/main
d56e34f53dabd4605c583b184a9ec0612a70b9fa fix issue #150 and add related integration/unit test cases
c55fd03c8f171efd4045f0b650ae36d7969518d9 Merge pull request #149 from elgnay/add-migration-requests
9f89842463a499cc641104d3d753837666c76f35 create migration requests for clusterset api
74f6dfced30ea4940d8af1ec72c51fb7fce5f873 Merge pull request #148 from elgnay/upgrade-clusterset
3f8699284b2c9e56d7f1ff4c4119480100d27786 upgrade clusterset version to v1beta1
d3c9da08e254c6e5823ffe8c01a58192898fc8e7 Merge pull request #144 from zhiweiyin318/add-owner
2a7934d73c6fdc010f6871e72c0259c86e6a6c65 Merge pull request #147 from qiujian16/addon-ns
4e812fed37bf4ac465e7de1984e263ea7a630534 Ensure addon namespace and sync secret
fa89c56b89e2435aa2aec6511debd997dff4dc63 Merge pull request #146 from qiujian16/remove-bindata
0b749401de5aae17705b668666116dd01598d1eb Remove bindata and update api
23ea13283a9078c6be1c7a5a3a27f64c7b3399c0 Merge pull request #145 from zhiweiyin318/nodeselector
a9128100fabff821b5a7d117b13777aed8719e55 add nodeSelector and tolerations to deployments
7d057ddaf547a64c409196767936f9c9dceeae47 add owner
13d51932a71232f3b7645ed9f82f01e0269785d9 Merge pull request #142 from huiwq1990/fix-comment
f77604537552efb3d5eea4ef24ff903d6bf9a759 Merge pull request #143 from zhiweiyin318/fix-typo
ed751da6e50f1df788fa6cc00b04acfa5e08641d change comment
856b149ef9aed77a3b19405692a2d17732206ca7 fix typo
5872bf1942d1d2e6f94d74010c471bb14af88316 Merge pull request #141 from zhiweiyin318/update-e2e
7df1f5afa3ce05e798ec33c5c0ea132381eed8bc update integration to trigger new build
e928f3d690bf5d45e0c358cbfbf1c7d8c2ae1a45 Merge pull request #140 from qiujian16/update-work-api
4fdc63ffa8172f18652cc83a287c53b251b56d80 Update work api
4ad5e009e2ecde1b173570926dde916a74e40336 Merge pull request #139 from elgnay/update-permission
d84378e430c752cdc8fff86f574a4746545a3d3c refine placement permissions
471cda573ab28a38aa322f824ed27cf58ec56d32 Merge pull request #138 from qiujian16/fix-webhook-rbac
52b1fc4b5ddcac1216cd218010b2aa2238d8c307 Fix webhook rbac
23f10ed7b0219217663150952990fc2267ce2c7c Merge pull request #134 from mikeshng/gitaction-name-fix
4502f0835bc8877fe2c6956f9f01bb04e6197242 Merge pull request #137 from zhiweiyin318/release-0.4.0
3002a11a75b4b9d8dbc7f8f79a320aa4bf0b0cea release olm bundle v0.4.0
3c9b5c00107d20fbec5f62c2daeceed76707578e Merge pull request #136 from elgnay/add-permission
d46ba2ee89c25f5cf6f9bcf84501d92e838d5667 grant work-agent the permission to update namespace
3a37a4917bd9d94942a4bd97a2289c82a7cd0487 Merge pull request #135 from zhiweiyin318/release-action
d2d10757788a61f8a125e28ae90a518b4e26504a add release action and changelogs
51e6b46c2e7bd61f69c84db38970a34f620ab54e use a more appropriate name for github action that publish the built image.
810dfacdf1f9d8c0c999b015d3026b7a2135020f Merge pull request #133 from xuezhaojun/fix_makefile_readme
6a2950d8d0ad8d7ec931ebc56fb9e9c1b020a2f7 Fix no managecluster after deployment and modify readme
7add43cf71a0f9bb3a74eeb913e95e3ffdd1597d Merge pull request #132 from xuezhaojun/fix_clean_deploy_failed
3a879bdd5edd6b45af1ea15b3259d3c38368f324 Fixed clean-deploy failed
c6aaca4e1296f86171a43a9ea2306d2f0d9b6359 Merge pull request #131 from qiujian16/image-push
1453d66831df76fefd9dbfe1547e29b4f1ceca44 Add image push postsubmit
f70f21658c4520eaa5f41ed40d43ecbec551b7e2 Merge pull request #130 from qiujian16/update-deps
ef338a1b0b58e9b37cbfcc7914dbf4f8e6166fb9 Update deps and enable action
c723e190c454110797d89e67bcb33250b35e1fd7 Merge pull request #129 from qiujian16/change-deploy-e2e
76d6096be826b48e4bd7520bd08889ce4e0d5de4 Change to use kustomize to deploy
dd39fbf4ad01d406f021d38a9f284e9cc59d4d18 Merge pull request #128 from zhiweiyin318/fix-typo
7060d4e776b34afce91fc7196232ae1ed14a4e70 fix typo
c5471b1ebc1c31654ab2358631c5156bc23645e9 Merge pull request #127 from zhiweiyin318/update-readme
5b74a3a3ac5c9fe572c48c39abb6207887b5108d update readme
06cf9b1f04b98073356464bd4284cb0f22f6c6fd Merge pull request #125 from skeeey/issue-12899
8db2ecf7e18ca4f89e9626bbff992046b07ba356 support to check hub seceret expired
1057c3403b3bb7b8914268b6cc795b04ce1c4899 Merge pull request #124 from zhiweiyin318/update-crds
0199e6681b5a4b9cc4250ce970a438816faf5ab4 update crds
ac12bafaa46b7c90b76f94bbc3abba5ac8345575 Merge pull request #122 from elgnay/add-placement-e2e
4ffd69c577a7acb17a3a79a79c4fbe8994f23c8f add missing rbac rule & e2e test for placement
d38c9d627b256dbf2a4dac07392953340560865e Merge pull request #120 from zhiweiyin318/update-gomod
3f2386f75e25cc88874609252e42499ed3ac60b5 Merge pull request #119 from elgnay/deploy-placement
985dcf71cb145b9dadbf4409487908c4fe75e359 deploy placement controller
aa15155a9364ca87ccf99aa4776be2331fa118f2 update go.sum using go1.16
714ffb79d1f0ed3428f2e100adb01c39e59cf73c Merge pull request #118 from elgnay/upgrade-clustermanager-crd
29e8bf4daf16ee2750b95e6f92741f4a6e90348c upgrade ClusterManager crd to support placement
813609193cd75487a9451c86ccd66e9e3e7e4c2b Merge pull request #116 from imiller0/workload_partitioning_annotations
6b1686e9531cd85cf86351756ddf50ca31c53f38 Merge pull request #115 from xuezhaojun/changeGolangVersion
1c836c1f5d3d62d753f654dbe8ae0bc494e93e53 change go version to 1.16
893d73c2a5cf4d3c4d9f44057efc37652b19265b Add management workload annotations
42d6dba78d9d851f1076a154e456cf93049ed5c6 Merge pull request #117 from qiujian16/adjust-replica
35d21457dc4647b4ffa3dc228864e0a9381227e1 Adjust agent replica based on infra api
f3b028757e3493944ce6e81040703363fb86c2ba Merge pull request #111 from zhiweiyin318/sonar
389008f7f2e743c22186ddbb8e5a0179c2fdf123 add sonar project properties
4f471e3df0fd775c56019634f1e8db08f80f5cf2 Merge pull request #110 from zhiweiyin318/non-root
9c4a96ba845e6192676b4fbece33fd39f8d7e520 run as non-root
6fe5197eadfdc1838ff15da5caff9be70915404a Merge pull request #108 from skeeey/update-addon-api
522174a9bc59470d346d6171bb80f76eda0e5b86 update addon api
0e540f0e50d420da15a42d9c86f2b664a16fd925 Merge pull request #105 from zhiweiyin318/upgrade-v1
4cd18564e80476b4876107279fef026b22c73333 upgrade CRD to v1 and k8s lib to 1.20.0
fb28c38365b93e0c7b2bc93b7706da266cfec587 Merge pull request #106 from skeeey/enable-addon-manager
42f10d0d1b29ac4954024fd6439a3c78fbc592ee update e2e addon available type
ff7fddf8ee7358b85e2047371c771206cb272944 Merge pull request #104 from skeeey/enable-addon-manager
03c5a708426541f8dea0fd0c7d4786e3903838f8 enable addon manager
3abcabe83840841bd2021046660b200be03b84ab Merge pull request #103 from pdettori/kind-updates
81dd5c77460c95c797953eaf2d01290d24361bb1 update README with  MANAGED_CLUSTER instead of KIND_CLUSTER
eaff13d3645302ebd3568b539956c725247c7114 fix makefile for passing e2e test
cee798f8d6752064276a440a928140d5273a7b8d support kind version >= 0.7
b49b80b80c3bc67973e29923246bbff86b2620f2 updated to use kind v. > v 0.7
daf5b5cf51a7da18243c6f99cee94f8197f53b90 Merge pull request #101 from zhiweiyin318/promote-version
8cb958d9b5ab315097631dc2e96c0a06f88a2ea0 promote csv version to 0.0.1
9cccc75248af0a7ac1d3e986ee46ae4b96cfe96c Merge pull request #100 from zhiweiyin318/promote-golang1.15
50bfd2d908827b63d8a5748ea2079a47bdc1f271 promote go to 1.15
cb2abf6370e6b7e42c984ceb431f95aa69f3b796 Merge pull request #99 from elgnay/serving-cert-rotation
be2d2e6e44d936c12e3ce78206425c0f42c9c6c8 Add CertRotationController
4cf775c00df01c37df3d7d4b552917e42e00c8c1 Merge pull request #97 from elgnay/issue_5475
d1ac331414f08ff8c5d8468e516c4cdcc563ec86 Merge pull request #91 from qiujian16/fix-condition
5fb1cff007cae01b9004ac74e52ed81e4752abb5 Fix wrong condition message in klusterlet
c6f083f3b91565785804205bf5a716c989fa7e4f Delete terminating applied manifestworks when detaching cluster
88746beac61a8d3786ba2eb4e28a82c925497660 Merge pull request #98 from ldpliu/fix-image
ac27b2e57ec1f0f356cf2aea34e0571a2a8019f9 fix image path
406a7acc31fd4fae647f84cb17b7b35177f9985c Merge pull request #96 from elgnay/clusterclaim
db21924ec52767c7720cb72069d74114a1299c8b Add crd & rbac rule for ClusterClaim controller
992cb56ea96a344b2c8a64ad87a542fd6bc54ae5 Merge pull request #95 from mikeshng/fix-kind-spoke
5e8134e3e5c908d02724f8856f7b438f902e6da2 fix kind spoke deploy
f58d0a9eb0a4aaa5b02b644851e41668054a00ea Merge pull request #94 from zhiweiyin318/upgrade-operator-sdk
28c2843e6eedebf7c202429880635dd3c5bff883 upgrade operator-sdk to v1.1.0
b315f9d1ccc0bd5983bbe3b41b6fcdbb219fa4bc Merge pull request #93 from skeeey/contributing
2fa384f08330440ee3111282c39b985a1fd5db71 add contributing guide to readme
69ee9b14488c0d3ec4829934eede7a9915cf2b3f Merge pull request #92 from skeeey/metrics-permission
1d42ab6690bd6aee1055cc8d46e4377c6199b7c3 add metrics permissions
93bb2271f96db428b8d6e5c5bf6e3d3c73c423ce Merge pull request #90 from mikeshng/update-makefile-kind
2324c6cd47391b1c893bfeb368eb19b8088fe432 removed redundant sed for apply-spoke-cr-kind, renamed cluster-ip-kind to cluster-hub-ip-kind, pass in the kubeconfig for one of the  kubectl commands that was missing the kubeconfig param
ae479bdead983f5e0338cb09a4a98825508cb544 create a new Makefile target for spoke deploy on kind
9b9b44fa4577e50d06c6a79d35e8d2c826e3767e Merge pull request #88 from zhiweiyin318/upgrade-operator-sdk
a415e2aaf9a9c860bb2d835950cb8faf021f67ea upgrade operator-sdk and olm
104b222cbdf9872fcac7372be12bebf5c3af9bd7 Merge pull request #83 from skeeey/bootstrap-secret
50e71ae74ff53702d0d3e694a0da5078b52456f0 reconcile klusterlet bootstrap secret
e98b51a8668b000aa5ea9d1b717acea36a978dc6 Merge pull request #84 from elgnay/issue_5475
7f8620babfc5b7079b14ee5a80694e937eaad001 Disable cert rotation for temporary kube client
f5a12acc4d0ab2b6100853b956e13e7c8f582db9 Merge pull request #82 from zhiweiyin318/delete-imagepullpolicy
73f6dcfb8ef1199ac9148c1bf6415dd58d2911cc delete imagePullPolicy
26900e92514847ccf3ad6309bc9cd19fc4aef1fa Merge pull request #78 from ray-harris/readme-update
3cc29bd3faa39d65ff2990e505282d1709ed71cb Merge pull request #80 from skeeey/webhook-timeout
a939eddf23f566d6b320ded667ad8c15cb19cdb3 Merge pull request #79 from elgnay/clusterset-exclusive
7902bee238845f24642ce1f7cc24e811e3b07852 increase webhook timeout
4d7ea36bf49bb5e3e5cbe017aeb40a51c7a27f80 Update clusterset api to make ManagedClusterSet exclusive
f2776dd331af305091832eddb3ec566a8d4357cd readme: add license info
6c8511ad98995383c135e363dab704ff9e31827f Merge pull request #77 from skeeey/registration-secret-controller
9276e9f24af525103f42634839a46e429eefdaab using hub kubeconfig secret controller instead of mounting the secret
4922ad06ce1d2a7b83854ed8cbf6687be87a9130 Merge pull request #75 from skeeey/fastforward-test
ac7bbb5cd9fae20813b88ca3e19149fd33177607 fast-forward test
928c2fcbe52af4c28e354de2753078770c391906 Merge pull request #73 from zhiweiyin318/fix-codescan
609465f787c59fe5e77ca31a396ad94a72ab0178 fix Remediate Static Scan Findings
37ce732ef67c9a750e9cba19fc6cc632d6faaf51 Merge pull request #71 from qiujian16/metav1condition
ecc34091965b681f2c851e9a5e6c07ff37a14293 Merge pull request #72 from elgnay/webhook-install
24f9bab01ce2bbc4005746bf39cf583e1b85bc39 Correct the webhook cr for clustersetbinding
7bdf5a0f0708a138e5b4613f7ed3fda252f70511 Update to 1.19.0 and change to use metav1.Condition
50041938bbf1f701bb841f572311b55a807c4dd4 Merge pull request #68 from qiujian16/delete-ns
bfaf3bb0e849d32a90e4a725769b8c25975f51bb Delete ns of klusterlet
b6e676e619ea76833040453fd91f7f5964fc7e90 Merge pull request #66 from skeeey/enable-clusterset
964b4c561b66cd87c120a7a937d7f439d27ec183 add clusterset controller role and enable clusterset webhook
e4ac84ea5bdcbf238bbbd9066efb374eb8b38b74 Merge pull request #65 from skeeey/add-clusterset-crds
998d8899a07fa1ef847c81117e9e5264e19e0896 add clusterset crds
5ad2e7addd7cfc67a99ca2a915694be0d796e374 Merge pull request #59 from zhiweiyin318/refactor-e2e
4c1a25feb4122bfe86837db093929cc0b348dc95 output logs when case fails
676b785c09308a96389668f7970dc91d2c044aaa Merge pull request #62 from zhiweiyin318/update-csv
d5d6eb45f2091233216332336a4069da6dadc324 update csv description
724ee7fbfebf0106789d0189762e499241555ab3 Merge pull request #63 from qiujian16/work-webhook
4d588c353b02cdbf9729329660096c0d27a9ddbd Install work webhook on hub
30abe467084eb0851057dc8b030b1cb3c985589a Merge pull request #61 from zhiweiyin318/refactor-deploy
3bb0871012a5e5a652232ebb682ec510b1b89805 generate csv manifests
c32082f4cf259f01710081ecba82aaf2c16f6c31 Merge pull request #60 from skeeey/enable-mutating-webhook
6730b9ac8d7800407e159c2c49bed27180555618 enable registration mutating webhook
36e0425ac5e386a4a0df58848b172fd6cdd6823e Merge pull request #56 from skeeey/issue-3589
232f2152f4406420245326c2670f9af7cc34b8ad Merge pull request #55 from skeeey/enhance-degradedcond
11f0b32440f706f5952785adb52fb8af89b52bd1 fix issue 3589
351a0ad27e38bd19c8fa61c2ce09941c6b8fce84 refactor degraded condition logic
4040bda0e61719bec9b50f5f05ae39bf02ab8de8 Merge pull request #49 from qiujian16/appliedmanifestwork
3c70e5a9254b5932aefc8f441635d3dc7b839d41 Add appliedmanifestwork api
13a434f5e3b189a042e42ccff48bf88a65b13033 Merge pull request #42 from zhiweiyin318/add-e2e
8283a16a62f4dfe2f610541b53fb6a0aeb3282fc Merge pull request #52 from pmorie/jqiu-owners
14e5276443f0a0230bc86ab35d05db64a7f95f66 Add jqiu to OWNERS
1408092ddc019b2b3e77272af6e37365000bc4e1 Merge pull request #51 from qiujian16/sync-pull-secret
97d68162c2961143405bfcce18f98f33e5993219 Sync pull secret
70830f152e4affd18766d95bb1fbd201feee4920 refactor e2e code
d4c0f0d4545fea7661d5e327cbf814a3ed5f1ee8 add e2e tests
7d8dab07e777ad5ed92ed92ca8c7fe199e1fd7e7 Merge pull request #48 from qiujian16/add-crd-description
50ad8efcfed96731b1c25f406a282d28880da550 Merge pull request #43 from zhiweiyin318/rename-role
b499ad6e7b1069597e49581bc781bd7288938611 Merge pull request #47 from qiujian16/work-clusterrole
3264e19a0067bc6794a40421dcf7955d99659587 Add description for crds
b6863246e89d619a4713e0ee044c535939b88f1a Clusterrole on hub should be able to monitor manifestworks
4dd3bc022e9352fb549f03687555f76587185cec Merge pull request #46 from zhiweiyin318/add-resoure-request
f014ba5ca4b044fa0014e3e365fcf75cba386c32 Merge pull request #45 from qiujian16/handle311
45c1950a7e06118a02688e891aa0e3bf1456757b Handle kube 1.11
d7ae4c4ab618e2933cf55056350ed4657c800e08 add resource requests
57a1d9829253bce6be7ff9d56ab800760209f439 rename clusterrole and clusterrolebinding
0b374144a63bd42d2f3776c80525131c86fa6b31 Merge pull request #44 from qiujian16/update-apis
e7b13a0e28b49038403aee4f9af45d82ed06d4e4 Update apis
3882bcbca1fcad7a922ffc8411c6ea47f23b74fe Merge pull request #38 from skeeey/hub-status
df2a6ca4dc98e4029a292cb76d7f3c9249ca7930 Merge pull request #36 from skeeey/deploy-status
6007d35c0270076f5ea4914bc51b32f740143785 check hub deployment status
2b1d134d91c6459ecf5a749554074e64f5778e9b check secret and deployment status
1f56801ef4854475aa5d09aab567ad5a33d1d4a0 Merge pull request #40 from qiujian16/update-library-go
1a2217205b11215fcb126bb65f899c4a2559e645 Merge pull request #41 from zhiweiyin318/update-csv
a5e6de4616265029e501b1446fc6b93c113bac04 update csv
0efbe995303454f3943e8c40c1af17bfbebd9649 Upgrade library-go
8c130fd53102862fc89352eccc2ca514e7c05a62 Merge pull request #37 from qiujian16/fix-typos
15a42dd726ba484598696db715829b60cf9b88a1 Followup of pr33
1a42d7f232cea55e2040b5d4ec48b1769c247079 Merge pull request #34 from zhiweiyin318/add-anti-affinity
303c7fd18871e03981fcf3d9386bd5d5f2e1a2d4 add podAntiAffinity for pods
bc15ff9e75c10e01753fbaf70c6efcb628d86a38 add lease role for hub
714777b5d2b272a21a0b52958dcd92270fce7381 Merge pull request #35 from zkayyali812/split-install
3e79551028af669110af802f55b7359154160457 Merge pull request #33 from qiujian16/generation
a6b1a696172512c055aee03aaa8cc16645206073 Merge pull request #31 from skeeey/base-image-update
dab4bbf081ed514687a8aa38887f3d6b34553d98 Use generation to track update
82130cab4c7e434eb69d204c4f3d43aa3aae5cb9 Merge pull request #29 from qiujian16/klusterlet-status
dbc14f132df739844871a1ae97a12dc0305ae2f5 Merge pull request #32 from pmorie/readme
fe5f958ab204178da345f5f62fb57254a4938e48 Rename nucleus -> registration-operator in README
d6216562574d8adbe641bb97270e192e41ec45f1 update base image
83b53da4dd98b2e45e1b68f38383eaa6040ba35c Add klusterlet degraded status
f0b23259289fffe844a5c237b3c4789df503f0f4 Merge pull request #28 from qiujian16/empty-server
235c337853f27ef8dc81a6220f81e5df692a1a65 Fix issue  when externalserver is not set
da7c7eafbca3ee069e6f0fd5356e533dc8ab1b6f Split Install of Operator and CR into 2 steps
9d37db13db2bafa2ca79bd117b8872492e9127dd Merge pull request #30 from pmorie/operator-operator
7bb1f2ee2df136c9ca8529b5548f538def6a6a2a Rename operator-operator -> operator
a234b633ea70dd6264ac1cd1d7c833de52f81df3 Merge pull request #27 from pmorie/registration-operator
70bbbcd855d2095b721af9fa254d99e539b48352 Rename nucleus binary -> registration-operator
b7127872cc6c6b0b2429a4052607cd0d3bf93eb9 Rename nucleus -> registration-operator in other files
626b1f0894ca7f3d31dcb3abcb34051d78fa8f26 Rename nucleus -> registration-operator in .go files
69e30f4d00886ac6b22e079e46d64f795370e39d Merge pull request #26 from qiujian16/deploy-instruction
b4527a2326859c9a488e1da8028d2b543c0dd03e Add deploy instruction on readme
1329267d34f6fd65788c2af8b0b4076cf91f7048 Merge pull request #25 from mdelder/mdelder-adopt-managed-cluster-api-1
fd589e99f28dd2a63b92ef5068e932cbfba62a23 Update some manifests
399a6b9a73271b0a0b43aac2f086466d874ed290 Adopt ManagedCluster & Klusterlet API in nucleus
7e75b02a923b0dc8e8925af91dea110a9be5d381 Merge pull request #22 from qiujian16/security
462df7647c3cf8c5d9744a078a99ce3f6396a6af Add security policy doc
1eebfc59be604cf19e38c14f0c8354bfc2684e37 Merge pull request #24 from qiujian16/mdelder-adopt-api-1
eb0d088e0353f94ba6bf4a161c6591cd8fdcd23d Adopt new API updates for operator
249448baea60bb7d36bf7ea1c432e54623de372d Merge pull request #16 from qiujian16/webhook
840670eb85efbdaaee79274c7047cd2e6d908b5d Merge pull request #21 from qiujian16/munge-csv
8434bc8b1d2c4701e484c53f8e063dc8f03f2e26 add webhook
78c60895a2770ac4ad09d44c2f6ba34df48289ce Add munge as dep of deploy target
9ae9f2b4ac0566fa2f3b2495dade4578735cc67d Merge pull request #19 from deads2k/tweak-conditions
6944deb352a05db83f17df4febd7cc7803f45155 Merge pull request #20 from pmorie/munge-images
62da4fb9d981c304ddc6b9332e4c08f74589c246 Add image munging for deployment targets
f1dade330c7c704565c6de3db68f0f9036257bae fix missing conditions, tighten expression, reorder application:
2ff2e6c64b96cfe4df3a1b55ab9712dbf46a8d26 fix message typo
3a99c07c799bc9ed3cfbf12e1e70677ee52f20ba create the spoke namespace from operator
24c2e1b863d8c37e75921377dde1886bc1301ef9 Merge pull request #12 from skeeey/enable-integration-test
9c4f2307fb6ed3b63422d28fe10df0fec2cccac7 Merge pull request #15 from skeeey/deploy-test
1b65fd077d04cfff67c471471e8405a88c35417d Merge pull request #18 from pmorie/e2e-bootstrap
6203ae00e969ecc4e2e179490583ba331816fd26 Add e2e-bootstrap-secret target
842cb478cc042db77d84d11e788105c226ade043 Merge pull request #17 from pmorie/test-csv-presence
ca591ed9203c214b0156db228ba41cd4efe554f7 Test presence of OLM by CSV resource instead of op-sdk
137d0682bf3f1394bcdd828a8ba5cf84b4634550 fix some deploy problems
17e7f1eeed0903b05acee1c3e2da61df9c67b231 Merge pull request #14 from pmorie/create-ns
894ffaaed2ae489b1d91db407c0faa73fc98b6eb lazy create ocm ns during hub deploy
dcdb940c93f0064790386e80bc54e4c89d14b065 Merge pull request #13 from pmorie/ensure-make
85e25551880c9371e0b699563db3307175c6f7f7 Ensure operator-sdk is always installed when referenced
e9d92a4f3c50327ef9284b568a5d3359a82ef6d8 Merge pull request #9 from qiujian16/gen-csv
d7e358074d8c8b09a0a72fe5b4e5e0d441f337e5 enable open-cluster-management nucleus integration test
abc1af28495b9d3a4195007c01e6255132a3efa3 Use operartor-sdk to generate csv
0ffcea11bf44522c8483f50c26bb2a906bff4202 Merge pull request #8 from qiujian16/updat-cluster-roles
5773ba86bef373621abd7e86bc1088ebdeda0dda Fix clusterrole of spoke agent
7cb11e256c2271dd9a199c3e98ae54384f5e737d Merge pull request #11 from qiujian16/split-hub-spoke
4e8f44fdd6455decd01499eaf50d027ad990a9b7 Split hub/spoke operator to two cmds
5e4e71e88c3b74d7990624bc8a2eb6b960b71c15 Merge pull request #10 from qiujian16/fix-dockerfile
5d36c1632eabe623b79f2c50b985cf6be9bd3cd4 Fix dockefile bug
37402d792e0dfed38ae7b39631d8757b01b614f7 Merge pull request #5 from qiujian16/spokedeploy
36fca6e11fb8d96bebd3e85ecb8371a9043ed8b7 Merge pull request #6 from qiujian16/add-verify
5c897b0433312ce6dcd2b00fd974f6a8e3186d49 Update crd and add verify
0a90144d42dac5f28a7e494ca3832d4dd367e497 Merge pull request #7 from qiujian16/dockerfile
897a280a9f1f949dfda66ccf808a6fbfff4a24f2 Add Dockerfile
ce565e6380a0aafd9fa2036d81e0cfc8a05ab642 Add spoke operator
fdbe918b1b4095e490b40f276e43af4c0c68945a Merge pull request #4 from qiujian16/hub-deploy
b1016774b16145664c0c0feb61390f2def311197 Implement hubcore operator
eba7ccaa9bfa7382dd8b97991a08628118b5f180 Merge pull request #2 from pmorie/gitignore
9effefb2e30554eb19f9ae6fbe8064c100fedda0 Merge pull request #3 from pmorie/owners
cb0f6200da79d305b3118889c56197ebf5dcad95 Add OWNERS
0acac02f29f1fa5445c63b0d4993583f3717ba8c Update gitignore and deleted commited binary
c53b7bb6c841a8f202d89bcba5a246fde415c387 Merge pull request #1 from qiujian16/scaffold
1f05d9bd968be2246b1040f26946d83823e50f6f Add scaffold for nucleus operator
a0427fa098e5a8fe1446e6f988ee107f811b16de Initial commit
```

Status: Syncing successful
