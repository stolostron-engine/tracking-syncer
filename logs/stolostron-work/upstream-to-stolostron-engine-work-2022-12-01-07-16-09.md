## Syncing stolostron/work with stolostron-engine/work

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 216 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
93c0efacf7137f30211dbed877bfc38e55ba2aca Merge branch 'open-cluster-management-io:main' into main
1a95b77fee6dfa5e3596723794070fdb027d7419 Delete resource even if it has non-appliedmanifestwork owners (#170)
922fbd90c3764bea9af5c006cbae33d214a59ee1 cache the executor validation results (#165)
90ef24d93be7de3b4082bcff2fc8c1fd5bcec21e Update ginkgo to v2 (#168)
3c6511bca9b47669170a38b5a14c2e6628009bff set min tls version (#166)
467124210cce26212bd141ddd8c059e3a9db0315 use controller runtime to implement webhook (#164)
f147a7c53e9046a98d7b8c1e5129531f9d2c0126 Delete unmanaged AppliedManifestWork (#161)
f8d1857345c72042bbd645b16f9eab2c802f9317 upgrade to golang1.19 (#163)
d20928e2bf62f1252af2197cbf36040a4674d48a add changelog for v0.9.0 (#162)
6820f68d81a307d02feb5a364d31b9c3dbf87d96 check the executor subject permission for delete (#160)
3947bd293bab565bbc5e7e532db483f24af9d843 check escalation for executor subject (#159)
60d622078b6e09b1669a0a33e95762da6744c551 validate manifest work executor permission on hub cluster (#158)
78c39cf7fb8974f1e993dbcc6277c2d34f3bb01c check the executor subject permission for action apply (#152)
2a7edddedecbb10fe7c07741fcf8054ece7560d5 Fix nil pointer panic (#157)
6a0f69fd47131a979600b6e4042e375164066840 fix Missing filter (#151)
787d7c5d456cf5ea2e0968ad0b9c04c024ee6d71 move apply method to seperate package (#149)
8f206974ddc0bb239e014768dbae19d0f37cad74 upgrade go libraries (#145)
3d0c8cd275e33eceb4b65957ba9add9e7c6aee4d Fix release yaml (#144)
0a87b7c6742152fa982560a89bf5289ef0d071fe add changelog for v0.8.0 (#143)
1a7686ee47b85ceabc4e64d64eda4a62e58fb4cc support update strategy in manifestwork (#139)
718605172ffc4826ba1e599cce3aeb338876f888 split work permissions (#142)
6f534125a7f2454e5f2d3e04a5d0904e49a8104a update default qps for webhook (#141)
10b572b2a601ba5299ff94233ed1cf36654c80d6 enable log flags (#140)
ae6b2c5ac6f754d4a43206479e2c54057c528699 Refector apply manifest code (#138)
320b657d6d1ebe8f6899485429715a0ac6729fba Upgrade go to 1.18 (#137)
a7145fd2b5f300b7b3ffd53cf5ec8534acb99319 Add lint check in make verify (#135)
70d6369be44157c81f45fba0e37bfe954f80ae44 Remove unreachable redundant err check. (#134)
2e587141998d4b569b380886688d9a580aaf716a Update golang builder in Dockerfile (#133)
806bb383f5b684584e3a07c4cd0afa9af992049b share release job env (#131)
75a02d18fa452ca77d2b05788887510a64e6b4bd enable multi-arch build (#130)
9e9e6b2eb6624379b8670c0a94b701191fac5c5a Keep the finalizers unchanged for unstructured (#128)
ed589b9cfd115a100585e5db160d560a68dd1c16 upgrade go libraries (#127)
018d51a59689c12725594e056ce83dcb32c70d6a Merge label and annotation for unstructured (#126)
084d9050366424296c74329bd0a5b39e465f3af9 add changelog for v0.7 (#122)
68bdf83a4ca7e0485eb69353f04fea82039f0fc2 Avoid building latest image in release branch (#121)
a042fb22cc73ed6465b31c4bade779b6bd635dc4 Disable apf in webhook (#120)
61c038e3f35a770cc4736689a9a491f4b0fcb5ed some code refactor (#118)
7aed123b07fb99e3ed35f359a711a6d5ca501bed Add an integration test to remove a resource with orphanDelete (#117)
d3dd5db4985a652fdc2f084ed8c4019515c69dc3 Update generic addmission server to support run webhook locally (#115)
f5ca2e675140d8d9caa1bd2129083c28b23b5d27 add job and pod wellknownStatusRules (#113)
1edddab8a88c513eee2ac88317c650647cfa9bcb support run webhook server outside of cluster (#110)
9a20b91430fa2af2fc66ef7ae164a8a5e3782232 add changelog for v0.6 (#111)
4334762add602df8e02c0be272cc86054b28ef2f Add disable leader election flag (#109)
5d86a958cb5bb109d83014951d34f5fe886d0be6 Update go to 1.17 (#108)
260cd94d85946492831df76af1d6fdef04e5330d Add interested field (#107)
44e5c786e4697326968fc4dcf130c29b4b5d0383 support run work agent outside of managed cluster (#104)
2f5ecc5750328697957b84009bcecad67e6d1561 fix flaky test (#106)
f18896b897ae877f041d5f6b5a04a8bff49995fc Update securitymd to refer to the  OCM community security md file (#105)
0a4850b9509247679da2e40346c9fbd3a604c4fe Set default propagation policy to background (#101)
03d0576494cc1c81e65c37c0bf001e7bdaa1da00 add changelog for v0.5 (#102)
ae50da649aa992f06de34c2ba4b79a052a39cfed Fix deps of library-go (#100)
cfa676cf806e415f03976acb73862321ffbe04da Merge pull request #97 from panpan0000/main
30eac35995e74f21419fb13a64d0770662cd8bcd fix typo in doc
a1ca4f2f99341f1c1caf379d172aefce068f2464 Merge pull request #94 from elgnay/update-owners
d517ab2e88611de17b26d638a30e43dc359123ec Merge pull request #99 from qiujian16/fix-merge-owner
72de5d1594f0449fc05a6eba915cae4dd150c7bf Fix owners merge in apply unstructured
f260e0b135a6bfa58ccf3ebf5803e8a576095488 Merge pull request #98 from elgnay/issue_14616
9073cd283ed8bcae9ceeb07047c4cae1f6a8d747 reduce the numbe of GET request of manifestwork
bf09d147a4b62c79d9402154cc5b557dfbb6cdf8 Merge pull request #90 from qiujian16/delete-option
c993830f25b9a30c66c223b10870f13eeb014d7e Support delete option
38f298bca6309e063b487b823326a9eb21929f47 Merge pull request #96 from qiujian16/update-deps
fa038178d1ac9cb150a09cbba0ef95bc090ad953 Update library-go and api
76a80accc6f4a8fd5ddc78f6da83c1de93a0e5cf Merge pull request #95 from qiujian16/generation
562516ab6399760a7c05f61dae2091a9b9bf85a1 Add generation in status
fda9acf360d1519845fdc7d5ce7a8898166f8914 update OWNERS
a61cea406f124ef03deb5ffc316d90db1d588bff Merge pull request #91 from zhiweiyin318/update-readme
a2d4bfd9664e65b62ddfaad9bb9e1eeb0605e19b update readme
02670266de35e3a64df4cd7c344c5ba943d805ba Merge pull request #88 from zhiweiyin318/fix-typo
93c8fefb1607063d72d2d67058b8d55dccc7a4f0 Merge pull request #89 from qiujian16/resolve-conflict
0ccab23cc2d569e149af97e01223684976c000a3 Resolve apply conflict
092179d1a4e9d2eef629d4f55e74bbfb9d8e17c6 fix typo in changelog
2a9a4aa091b962419066f8784d94f9b3f30d9e3c Merge pull request #85 from zhiweiyin318/fix-link
0c2101631af9f00b2055b4eb7b89b1ef46bc85ba fix release changelog link
a25c855bc0d25e468cc52e861c1296ba496c28ec Merge pull request #84 from zhiweiyin318/release-job
bd590fbb7f6cedb45e39bda52bcd03947fb164c0 add release action job
68d83afd31b0ee2549e9410c03fa1b0ad7174066 Merge pull request #82 from xuezhaojun/fix_controbuting_doc
c997150d636b2488293480f3629f0d71fb9c5c7c Fix no docker-images load before e2e test
0fde53e4fb4caac9dfe24119fbaeba45d888b0a3 Merge pull request #81 from qiujian16/dockerfile
c9d71ff42be19d7daa5352fc64f4cc7f6a716ddb Update dockerfiles
6cef6d3db0973ec722f5543a47c520584df28979 Merge pull request #80 from xuezhaojun/fix_kustomize
61326e212a6c7fa4b51f172a80274cf22438c7ee Change KUSTOMIZE related path to absolute path
7ee111a1b9065c2b5129b67373aafea15a97edbf Merge pull request #79 from qiujian16/image-push
8675aeba9dbbd9d8a015ecfaf5c2350897bb21b5 Add image push automation
180e81c52a33b6fa68b83873ad2d745646144e53 Test automation
6ccdd098811e97e88e71b65dcaa55cfed1e8b6b0 Merge pull request #77 from qiujian16/enable-action
e56f18849fe55eaa988cd2c712d1aeb5b37e95e1 Change deps and enable action
7c48ad8d6a775746ec9a7164fe7b356bd53b1abf Merge pull request #75 from elgnay/update-readme
4af2cb0ce9251b596721eedff9b06a541268ade8 update readme & makefile
7da3b0410d22a74bd8bd412670efdc681e81e041 Merge pull request #76 from elgnay/issue-13265
1e839f26ed877340ee559b5d0158ad41a206783b increase qps & burst
11688af42ddcf9911ea68b348974fabb684e5e2e Merge pull request #74 from zhiweiyin318/gomod
c906c169e6c10725e42a2a0c9f1b364d3bb040cc update go.sum using go 1.16
fa3f0fb96b2271a5573c8c667df55f4908ed11b1 Merge pull request #72 from xuezhaojun/changeGolangVersion
c96dc0e69e2f15ef01642aa1d829924b8dc8ec0e change go version to 1.16
9f7c45d088290d2d2f519493f2552819d83091d0 Merge pull request #71 from zhiweiyin318/sonar
9111fa7be42bce6800c63fc7ad12983575f7beca add sonar project properties
73bb3186878da0994bdf9e485237e75a4dceef19 Merge pull request #70 from zhiweiyin318/validat-size
30b03bec3252a16546f70077abbb363f217ceeb7 vaidate manifests size
6655e14ce7ae2a02237e1d19ee6420a959585338 Merge pull request #69 from zhiweiyin318/non-root
20b00f59afae3cc1ec36c89ce7901b18bfca2ec3 run as non-root
4832b07d4da99a4dd2aa075c8945659d51171b88 Merge pull request #68 from zhiweiyin318/upgrade-v1
ba559f456c2bbf197ca8e6f224639a8b60aa8fb4 upgrade CRD to v1 and k8s lib to 0.21.0-rc.0
861b390c2c5c6b49208a912762861c0ffd7faa4f Merge pull request #66 from qiujian16/ignore-version
c360449bca908c36f8fc2704fca369d0de091ec2 Ignore version when finding untracked resource
11f530f467683e5b8d6daaff80d32fad97cf54b8 Merge pull request #65 from zhiweiyin318/fix-typo
442fc666f219b8a13da6cc582697f6d402924324 fix typo
f84f0f9bb5add20e3d8523191686d890d3f3d7b5 Merge pull request #64 from zhiweiyin318/upgrade-go
c7e178b7179924bd3cd57b9e3f07ad3103d63c43 promote go to 1.15
4326165af060d5c3e7988d0e0c7a5b40028edbb1 Merge pull request #63 from elgnay/update_comments
795575932ff1be22712cf670e33508cac30420a9 Update code comments
b3263720de38796047b5e12f6a7b1c372f89dc53 Merge pull request #62 from zhiweiyin318/add-gitignore
c45f77abe5600ba8e10a233e1e00475c30db40ae update gitignore
97f351e0f3a8b74c76e32d1ad85da3bf1e4f680f Merge pull request #61 from elgnay/issue_8944
4252656611319dc2259db92cfb5bbea24369b2b4 Replace resource mapper with dynamicRESTMapper
3bab9e71e1b67d06236f4f6056dc690a5caa3335 Merge pull request #60 from elgnay/issue_8136
1ae24f248f1b94f4240ce6cd4181152f4385d970 Correct typos
46b765914e41bebb8814e72212021f5e0430b9b4 Merge pull request #59 from elgnay/upgrade-library-go
6e884f2f065e0155381b02369cd876aa41738576 Upgrade library-go to 20201207213115
5c61a475339caeadeade2b5fc10ff52b9a3c0ee5 Merge pull request #56 from elgnay/upgrad_kube_lib_to_0.19.5
efa81f50b10e7ee2a1ac4d48e443a83f0915e0a2 Upgrade kube lib to 0.19.5
c935790bb4ee3b7f391515fff8ac70104a794f1c Merge pull request #55 from elgnay/issue_6841
4efd6bd5e5ef7af26ff81f68cccb2b4e01aeff34 Update comments of AppliedManifestWorkController
82409da4382730a010370fdb6ca9d53c7ea313c9 Merge pull request #54 from skeeey/contributing
d779278e7fddfccae6f3c5ef151bbb3768ead1ab update contributing guide
95a42a6175ed463d35c1ab262dcd609550192534 Merge pull request #52 from skeeey/updateapiserver
3d6d695af88430b7ad01148fce763c47b097ce1a temporary fix kubeapiserver issue
26bc54105d4e38d22316e1fc348b0527bf356c83 Merge pull request #51 from elgnay/separate-e2e-build
c39326ec48139d1609d16faf2b4f8b10575fae47 Build e2e binary separately
5adc962d29c0f027740f5e2463507a73c8663d03 Merge pull request #47 from elgnay/issue_5094
e4ae150248e91d12efa729921aa77fbf974965a8 Merge pull request #48 from zhiweiyin318/build-e2e
bfa5db9e20a7464733167283c6980e5990afd5f5 update build-e2e cmd
a6e71e8083fec97d09fe65322dc228df78249c01 Fix remediate static scan findings issues/5094
ca970cb7684ca4da49be305d30812e69215b06a7 Merge pull request #46 from qiujian16/metav1condition
c6430529fbc34c64cc98f254272fd4f35362ef2b Adopt metav1 condition
43d5d5189eaca4987546e9ff1f47ff6163f8913f Merge pull request #45 from skeeey/fastforward-test
7a5dd11bf4dd030a396c630073f78593e90679c7 fast-forward test
8c49db59870aa3032d62a9a7295d890280f9dc52 Merge pull request #44 from qiujian16/condition-merge
60a859d9f1d635ed18a3e74806cc0ef62415cf3a Resolve condition dangling
cf59c638930ce9c08b435b137724e7c739b1cd9b Merge pull request #43 from elgnay/issue-4565
7cede9fd2f3d3f7b5c053bc87924d7ca95decf25 Delete resources applied by controller only
ff23692076844eed5875c00a1f2157e969799dfc Merge pull request #39 from elgnay/available-status
08efde43095943c0df9297989c90fba4f68a7c97 Add controller to handle Available status
1d4eb680f1eac8e066966aa7ea8f6d54099de2cb Merge pull request #38 from qiujian16/webhook
440af3438aea8878f47b8cc53ef352e693d30345 Add manifestwork validating webhook
98abd3adc07a19d57364224440bedd67c89370e1 Merge pull request #37 from elgnay/e2e-update2
26e5edb7738f2a95b7210c11cac29dc2923c62e3 Create appliedmanifestwork crd with agent deployer in e2e testing
c92dd74c5f987cc93c6b4fd0aa100cbe4be88c24 Merge pull request #35 from elgnay/e2e-update
017b3aa42784884b429f03124ab83fd7fedbdf5e Update e2e test cases to work with registration-operator
adb51793e07b32e3896b020e7e524c9d9e79b6e8 Merge pull request #36 from qiujian16/pr28-followup
d4bd6c718eb3160ad5e468b2af707fba69a75e54 Follow up of pr28
3e84b9014f2c90b78f6f9fdc7b0d5eaf12458ba3 Merge pull request #33 from elgnay/upgrade-api
b72f2c2d519b8dff114162e805af10691680d2a2 Upgrade api to version 20200715201722
1fa05673bdbca451c8c99624ad9a91c33950018f Merge pull request #28 from qiujian16/implment-applied-work
5205603e30ef79aea9fe6fd21f78e6b4a5b54009 Merge pull request #32 from pmorie/jqiu-owners
dbccf4b1ebc47f4da6c28e8ad873d2de9f2eab5d Add jqiu to OWNERS
3b8eda718b7e3fdbf7859caa78e958f3f6dd63f5 Merge pull request #31 from elgnay/fix-build-images
e4fa6ba7e3ded07915725f05ad409877520761b5 Implement appliedmanifestwork
86413e55c1e836aea77a6640833c72f89647cdc5 Fix build images issue introduced by pr #30
2a5945181684c88b1ea8edd42f5ad49d1c89da69 Merge pull request #30 from elgnay/e2e-test
22c633a6e3d3541126211a958d822ee3047e606d Add e2e test cases
ed85268a5c20e5573d9aa7e520d160f61bdea52b Merge pull request #29 from elgnay/issue-3332
b269b91a24d2e4a86273da59865dbf3af655b30d Check if finalizer exists before applying manifests
6f1f7408cbb91f1d5177c203b4a47f6ca0be1298 Merge pull request #27 from elgnay/issue-3250
de41bc43e1564b1e2f633c265f4be6492a6d706d Handle unknown kind returned by GuessObjectGroupVersionKind()
b360885547fab24d98c69d9c8996523abfd90c4d Merge pull request #26 from elgnay/pr25-followup
25e2dbdab7692a2a42362c2c2a85cd7d2d351324 Address remaining comments on pr #25
f202c51ee8fa84b0d1b39dfaecc22faec5a86de0 Merge pull request #25 from elgnay/foregroud-deletion
e1ebbae886cabcb929b35e68f75499af535ea22c Support foreground deletion
0471c88397a600cdbabd486ee3c435029d4fae00 Merge pull request #24 from skeeey/update-base-image
d4e2d4cd6401ddbd390f376d10e274307646dda5 update base image
75ec3fc00a89a1bbe3f75c8d0655793936fd5348 Merge pull request #22 from elgnay/integ-case-applied-resources
7628104ef14187bf7880cd8def63b7f4d2cc8b35 Check applied resources in integration test cases
7e19f0e66b36066034ec4356c7929fe90b185f2a Merge pull request #21 from qiujian16/security
fc69931178243823e8072970d4fbf9ebb3057442 Merge pull request #20 from elgnay/delete-untracked-resources
e75664bd0316aa5e3543ae60e7865b1dad927ab3 Add StaleManifestDeletionController to delete untracked resources
e66ab9af973e750f32d70cf186eb26d992c0f091 Add security policy doc
0b640bf510a0c15a77371ee0d5e2ee8e8abdf333 Merge pull request #17 from elgnay/more-integration-cases
4608646d1a8831d798563b72be6d8290173bb596 Merge pull request #19 from deads2k/separate-controllers
4eb9c3b617a60734bad80656cc471a6524df9669 update go mod
bed0d6e7ba342c6ffcd047d5a1f106ae865ea7f7 separate manifest controllers
1d0803b91018767d7f48d316e251bfa4e1204d5a separate finalizer controller
43492dd79091ca09f4ab07c4d0c947a22e100257 separate test helpers
9734749023a44dd926dfe0e5fbfcb9d074b7a436 separate add finalizer controller
daa00a9da97b792d5b8fac424f0bb38a2c1e12d6 Merge pull request #18 from elgnay/guess-gvk
af80dfbc197adcdf3278707cd6d600a3deaaf443 Use same logic to guess gvk of resource object
188bd6fbadf8a179235b109a3dbec6755b19d4bd Add more integration test cases
0f4a815fdd89368d1deb822bf9d6ad71951e3ccf Enable status condition checking
315e8a683fc3ef1154d6ee211fc44c9f2212b9f2 Merge pull request #15 from elgnay/fix-gvk-not-found
99b8678fb2bc44b7c525513b7f190760f11ed941 Fix gvk not found issue
8bea1a167a6dcc311552f12f14d1c4d197207747 Merge pull request #9 from elgnay/merge-conditions
7ff87da266cb129161bb62ee379cf9be98fc1834 Refine manifest condition merge logic
484dafb5edfe23261959e654a5900b0318703551 Update manifest condition merge logic
d9ff096fc0db57c4f99d2daff6e2663cfeeb4ff8 Merge pull request #8 from elgnay/aggregate-applied
c1a07f89840d6be0f187f9a16b5f63f3e1c4833e Rename func isAllInCondition and test case
9b484af1e70f77f19d00e61dbaeef77d8c89cec9 Generate work status conditions from manifest conditions
e05f43a320577caa0ef9c2aefc0d3fbcc846ebb3 Merge pull request #12 from elgnay/integration-test
29380fe79e44747b0c522ea6885020a3d1346bc6 Merge pull request #13 from qiujian16/fix-work
f30e60b60d4e01cda1505251fe449d166032f781 Handle deployment apply error
90cf73cd3f1d45ce7bc5fcdc6ad163bd5dc657aa Add basic integration test cases
b10a920e5202df15b056a23b070051d70bffd267 Merge pull request #11 from elgnay/upgrade-api-20200512175145
8fd4a79322021c704881e5f31a1db88a20e58d19 Use latest work api to correct typo
ff8a27a004f35b512ff229cdab232a58e900892d Merge pull request #10 from elgnay/upgrade-work-api
4cd23a54fff073e2d49a9f4ee58b8ed8d53fb596 Upgrade work api & update work agent cmd flags
25feca979369b873fc32e5abbaf77288d0467baf Merge pull request #7 from qiujian16/update-unstruct
e9143d61585b6ea6e1944512891ce11f5611174f Update unstructured object
be6c44ca395b3bcad9e01f63988c105fc6235b30 Merge pull request #6 from qiujian16/dockerfile
7c6637b060a1b811690038698faf2a8093507e08 Merge pull request #5 from mdelder/mdelder-update-docs
9bde4119d52a899d20b16871571057dc70c2f398 Merge pull request #4 from qiujian16/agent
b57f946ca31b2f4c48f24fbf1702253c5c2956c7 Add Dockerfile
9aa8a8bb3dd7b8ecac876490ee3b2550e1e410c0 Add work reconcile loop
258f273c059614acaafcd2f5e724518cb100b56a Clarify expectations for contributions
c17a7df9c1abad1d456d4d8ace8fa46f75ded517 Merge pull request #1 from qiujian16/add-controller-base
5efec48c4853f46885f6355ee1ccd7b3c972d817 Merge pull request #3 from pmorie/owners
98066e32133174d6f094572db52046bd6167bee0 Add OWNERS
7ef58f61a51b576ff944f77249e1d2373c084226 Add controller base for work agent
f2f94f9e7e15337eed163caca674d9abb8e5c9b3 Initial commit
```

Status: Syncing successful
