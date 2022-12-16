## Syncing stolostron/hypershift-addon-operator with stolostron-engine/hypershift-addon-operator

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 178 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
f8dd251f1bfc442bb2b171f281fe9450b0fdf471 Merge pull request #133 from rokej/metrics-1209
411b17ddf90fab211e6e83af7f2f739b9ecbb9e3 add more tests
3ea1b7d5ac948e5d3358c8fdaf53e131259cdb47 more test coverage
6963fa4855e81e58cb3e6140dc80b6969c0a296a more test and more metrics
1b23cb59dde7edf60e1aa14cefd786989de35204 fix test and add new metric
afec0891f14e59d88de917c3329acae62739565a fix doc and add a new metric
dd45cdc7688c50ca31d29c982fa655e65509eefa fix doc
0eddcd3449952e72b710494e6042bdc73082d195 add metrics doc
6ee7d0629dea2ba343be86a4ca9f94bf259cec84 add metrics doc
abe076d62b995c3123b9f9a1c841cafca32539c1 add metrics doc
e33f2349c936a4283b17c290dadcaf3443a050e6 add metrics doc
08eb732fe8d67bd2ffbfad73863f7042d3651564 Merge branch 'metrics-1209' of https://github.com/rokej/hypershift-addon-operator into metrics-1209
f532d8189880976ce14f9e90c1bb505996ff6b60 add metrics doc
7bd8ca7142fc97d829ef788bbe7bcb24d882c175 Merge branch 'main' into metrics-1209
bb57258b7b94f193811fc77cca5849043a37c37a more tests
87d0f60411444856a45519f8b1e691507a675a4d add more
689876282498ddaa2ac3fd4abe9cb05a246b451e more work on monitoring
03a0f8f35bf526d9ff4b9803d0438e251ebcc358 WIP
cc62adadd434477cb08e772df0432a6fbdebface metrics in progress
f9d98f78b2ba1932c3d70a404b0e98ee40cd7f9f External managed kubeconfig secret support for custom api server port (#128)
2e82fe52dd32fa3fed7bbb4fd59d833611d966b3 Merge pull request #127 from rokej/update_cli_paths_doc
1077af788ce039623d49fb3b1baa2c51ed4fbcba add missing env vars
2295cecf33592c5f7c414101e1f62470ff9bc2a4 update CLI download paths and doc
c0f20f8486692644473ebee0c52414a7ac8f803b Revert back to golang 1.18 (#126)
d1218dd73b855648fe4b257e53fbb98e8442b316 Update golang to 1.19 (#125)
79e553ea74ddc5ca99b6e50e48bac828bbece6cf Always copy and use MCE pull secret (#122)
ce6cb86e4ffefadf14936334df76b5fde30473ab Merge pull request #124 from rokej/hostedmode_doc
8b47643bde39921f72b68722a15b5ca5a949de89 add hosted mode addons doc
bf2e81ee43329fac7d61635cb01350746e15dcfd add cluster claims to indicate HC count above threshold or at zero (#123)
abd9736f3fe1ae3e3995ad1ecd09b8db70941e31 fix function names (#121)
4f10bf5acd5ecb9a9366679614b76679888fff85 Merge pull request #120 from rokej/cli_doc_update_1202
8b0b19637df600fb1b70c2447560eb705ca43160 update cli doc
dcb10e2dbdee78f1f3af0cff80933211d4fbf4aa enable hypershift CLI download (#119)
6b9bf70030d720c8d1f4ef1b60374a56de293d6c Create hypershift namespace for all platforms (#118)
24b89031b84756221f5db3e6ce2e002fab4ca0e7 Switch the default ManagedCluster name from InfraID to HostedCluster.Name (#110)
d7f9b2e3f122b1b16d04266973cdc94a1939d401 Add a doc to explain the hypershift addon status in details. (#117)
0e3dfd90c562b6d3e58378fbb2f5c1c61b60fd6f Merge pull request #116 from rokej/more-doc-1128
3c5499b2e1c0e2c396b0cc45a35efa896538e8b8 add more doc on AddOnPlacementScore
330ce22bc33f822e43904bd785d3bfa9e4490434 add more doc on AddOnPlacementScore
984cca22c98ed08d142a0f55e14adb1677aac398 Support node selector and tolerations (#113)
c5826a56519045c2bb89b32a6a9c3ccc310209bd AddOnPlacementScore condition and clusterClaim for max HC count (#115)
243fe2fb4653dbbd84a905325686e8dc2346e682 ACM-1754: enable hypershift-addon on local-cluster automatically (#111)
bea602fca0fc9efdbca685848376b9dc2513f9bd Placement score (#108)
b8a8906276f69bb80030b3e30829e741a98760da update doc with changes to deployment (#109)
310ec75e75e50cd82513db6eddcdd64eee34153c Use the addon image pull secret for the install job (#107)
dd4ba9120eadcc12f1960642524250324b3de528 Merge pull request #106 from rokej/update_doc_1114
44db7b8901548afb9a8782b76cc087baf1645fee Update the manifestwork HC doc
71dfc7f903ec637396a76b96913301741e4e4e1c ACM-2052 (#105)
baeb22881354c43be16f8f8da118ad71495288f5 Merge pull request #104 from rokej/ACM-2052
4e8624bbfb059cc228da0132464e7dbfb2272c7d ACM-2052: fix the external DNS doc
f13597984279feba70e3898598e9d89bbf6a3ae2 fix incorrect usage of controllerutil.CreateOrUpdate() (#103)
4cc637e91a78398f0b2999993c6004b38c29c15c Merge pull request #102 from rokej/fix_manifestwork_doc
2737c68656c62ba7ce52bda291950c914574637f fix manifestwork hostedcluster doc
876f6c535a72ea7379879027c04e3f628447d71f fix manifestwork hostedcluster doc
7cbb9900630e19f562c428248b1fa2d65095082f update doc (#100)
8c96eb120ae1714132b389723ab61059e9e095fa Update installing_hypershift_cli.md
d9cc26309fe4c4ade279180a55bd491eaf439669 Merge pull request #99 from rokej/fix_cli_links
80591eb14af48bb61a7619e2f1d47db3e99d6c79 fix cli links
71be8f9d4df258b5a13fc245c1f670a34db085b2 Merge pull request #98 from rokej/hypershift_cli
0e7d21212c7c1432b084298f9e3c43bcb1f4cdf0 add CLI binaries and doc
f04c3941ef9e7545a1d4394cf63e53fd5d1437a1 Merge pull request #97 from mikeshng/status-controller
adf3c9314ed381fbff582bb91f96882bd3328334 Add new addon status controller to check and set status based on  Hypershift deployments statuses
e3efacd678df4479b089bef141b26374ffbb9c8e Merge pull request #96 from rokej/ACM-1923
6c156f79d4b569220f0a392a0935de2ab80646dd fix a typo
a04d6ec810dc07878dc0d179e9720e4b2e781eea addressed code review comments
9bcc73ec4489bee5a9304e8fe24dfaed1b8392b4 fixed tests
a97f06d74bf086c8a82f1b43ff543b8a0bf85ec3 added secret change detection and tests
9e5749b85ae4c71ca103c610840548b8f0b1ffa9 fix ACM-1923 so that addon restart does not reinstall the hypershift operator unneccessarily
b0183710d1ea7bd15fc3539ac544da2081481206 Add support for the ManagedCluster-name annotation, (#95)
0dd7a5a030f2c3d2f1a352df0215ca8ae4e17577 ACM-1824 detect changes and re-install hypershift operator (#94)
2afbcb0e9031609e1c5d4d7a9002d0b0eac929c9 Revert golang back to 1.18 (#93)
00cc57d01ad10d882d08607e541feeb7028fa660 Trigger CICD build (#92)
b7b687f8fcc64980c06af74dc662b41ca3541c6b Update golang to 1.19 (#90)
e7ebf4c9ae8b1df4acb55f89011d3b9906866ff0 Plumb in `--external-dns-txt-owner-id` (#88)
17b2372291a2702e1c61de4b8a6480e997ee1b3c Add documentation and Scripts (#87)
47e349c864b6d4be515f20dde94b8d26a9c6bb73 Use job to install HyperShift operator (#80)
9cbd0ba79720bd4259ab5f41dd58b5ccf7fb27e0 Document how to create a hosted cluster on local-cluster without HypershiftDeployment (#79)
b82407c304219f83a9f4cdc4d0a03292d52f1967 update image override configmap name (#78)
c75e2433933eab0918b74e960a2de5da0434ddb3 Create secrets on the hub when the progress of the HC is completed (#70)
0df71d854d8c046b05d4a96d65746948f39299a2 Support upgrade of images for Hypershift operators (#73)
8572219628973f646f9ec7e08eccf484c7f4bdce fix configmap example (#74)
536c3eba23ef92d03831155ea3fa7262152b1dd9 Hypershift operator image upgrade doc (#72)
1d4355ec37170dc4b831d583f748ee878b4714b5 Do not delete HS operator when deleting HS addon if there are HCs (#71)
40287565ad33cce0a70419e6dc95c153803235b3 enable telemetry in hypershift operator installation (#68)
27e8825923f15db3c5f77435d23d0015ea40d940 pick up the latest hypershift 4.11 upstream (#67)
6d72f7844d9d753cec3e04e370547086bc478236 Add missing support for External DNS parameters and credentials (#66)
3cfda5211b1c6c2a44a8f3d0fe18e1afebac4a64 Merge pull request #65 from jnpacker/rebuild
a78ec1ebbe44a03dd695076c598ab38eca653e4f Trigger a rebuild
e9a2857775a0277c8586d0d73f27e51448de6b91 Add support for CUSTOM ManagedCluster names (#64)
e2ed48fb0d9770597045fb7c9593e4fd460ebc8d update hypershift 4.11 operator and go module (#61)
5419b1eb30dba0e9c522029d5c1e58567fbfebf5 disable readOnlyRootFilesystem (#60)
8ab86bf73d83934dcfb640639a2c19c5e5b9cafa Reduce pod privilege (#59)
b383709fbba7c11c089e29b3432aa8975d39b072 delete code for building hypershfit binary (#58)
a6002bd10e90ae131bcaff68ebda51134c2266ae support private link hosted cluster (#56)
de3bffac4c48ba266e4492143dae2d209605bff4 Update version to 2.1.0 (#55)
849e72232d2ad1a89b872a337b85836869f71ace ACM-1474 add support for private-link (#53)
16be15b90d68ce779ac58638e7faf881c0b098f0 Update hypershift version to match hypershift deployment controller (#52)
1f8a98b664a9a874e65d55d8b7422d171877f7ac Change name of kubeconfig and kubeadmin-password to use infraId (#51)
8cc67a753433c3fc69de3259ac1a078a36b46bb5 s3 bucket secret should be optional (#50)
3a8dce5b8ba89ab39f0ae2f9587c08579de5b2ce Bump go.mod version to fix hypershift-operator install problems (#49)
211ae1e14b05752dd9520e9a318cccbc69c1b9af New unit tests (#48)
308357a625fbd262c9f286c39031c9ef8ca3938b Bump hypershift-operator to commit c7c2b57c98ca (#47)
aff9cd4d04a0b42af4d70e29a87b456d0e1285ff Use hypershift library code to install hypershift operator (#46)
4170452029312cc25434edcb96e3f7254402b5fd bump hypershfit to latest release-4.11 (#45)
2132d26d890d33edf0b497ec5ffd29033e202926 Annotation check (#44)
c06a4bb4c2bb0edf9d2841b5516ee20462450d8a Bump golang to 1.18 (#42)
906fd38b194963542e51059ba55faee607c28937 fix typo remove the extra blank (#41)
3088d2c29e5d8d5e52308b35657c38ee816167f2 Add image pull secret for addon agent (#40)
b9a3653f560fb39d1631c371dbe6459d2ccdbe3b Noticed that we did no upgrade the hypershift-operator  (#39)
81e21b81ad92903fe68bf17307d94e29cec0294e Update pull_request_template.md
da558ec7614a15920d9e404bd5d870dc4d4d7198 Create pull_request_template.md
2dbb231dfe848adefbc40240048df7d98c3e4292 Update openshift/hypershift references to main (#38)
d4ddab44bcd0906ec1c549541fca87443bfb6a71 Exclude e2e tests for sonar (#37)
220c77ce9a5fe9910b47fe8929764b57d9c56077 Fix e2e issue (#35)
4032858a0aa3792f7ed6deb0c1a98fc8b42d6f29 Add e2e tests (#34)
c2e80eb7d9ded07400ce60cacbf225908455fe79 Update owners (#32)
20e1724e6241826dabdcd5cddf78c8f2b6d9cecd Use branch release-4.10 to build hypershift (#31)
4cb5788cc1ffc5ad93a75f89c11e84a28960b5e5 Add permissions for operator (#28)
c3d39c37bf7fc6e607a95b01986d1f372669975c Fix: using spokeClient in deploymentExist (#30)
9e864a9fa54b052a17f9dabfdd13ad137660b474 trigger CI (#29)
bac78c6aabb3550423956a1b89c2310cb9bd618f Add cluster claim for hypershift clusters (#27)
aa90da9dc54f130d2162e15d66a93b670d3eb2aa Filter hosted cluster by annotation (#26)
117d6b4558b72253f63fe02ed64bb07754ace142 no op change for rebuild (#25)
831bdc92b2ff567410dffa22d57833ec7d55d054 Bypass when image pull secret is not provided (#24)
2ae358ddd1c4db75e2345d57b878000121614096 add configmap sample (#23)
fe763b0944cc3697421f653ccdc3fd83e7ecbb9c noop (#22)
072c806c09b758d885d2629beb51a3617fdcd674 Merge pull request #20 from ianzhang366/ds-configmap
11756b3c37b9c547253375385886c2c5816262c4 make sure the configmap is consumed
b3c0dce661587f3c8c297814da6b61506b5d2929 Merge branch 'main' into ds-configmap
baf998b1ab4ca08f9e71689f388afa13f1411c97 fix delete flow (#21)
4b5478c291abb2fb3ee8d896f50beebfcde84bc2 make sure the downstream image of hypershift is used
56b1b0e4fdbe7282a629050d1c9d08a575086b0f Merge pull request #19 from ianzhang366/mark-on-deploy
fa58e760d2e8639b4f4ad82606a19d1dadd84b26 fix gosec:G601
20812314ec24ff354bc531e38ff92215caf7576e mark deployment directly instead of use the managedclusteraddon mount the multicluster pull secret to hypershift's serviceaccount for downstream images
0cee05dee8f15fd40cca46e181a896b0657e02d6 Merge pull request #18 from ianzhang366/split-build-target
3f3d70f9907495cd6c4217b81901036f63ad3bd9 split the make build for downstream
caf52d8bb702960b18ade1dcbe7d0e6f137075a6 Merge pull request #17 from ianzhang366/fix-docker-img
0ff7a17d4b65a48f0ab31cf7585e202fa89ae7d1 remove extra PATH setting
6dd9baaff2303173579ef8ca97c5e192a635db1a Use hypershift binary (#16)
18d1cf3b6a077e150981660a4d356da965aa936d Change hypershift deployment annotation name (#15)
54c941bddea7c266b72c63fe34193a52e5105489 Merge pull request #14 from ianzhang366/cleanup
0162b5bc527b87991994f1a3dfdbabba29a81cb4 fix vet error
e350ffc6c14f37fe62656310b0089815a23604f1 fix gosec issues
d25dde45e50c46f1fa598b7148eeb79cc53b4755 fix format
6032f03b7c1a31284a1fc92f3a8f5c3f324a376f Merge branch 'main' into cleanup
03d5cc436379d2aae7e67edfbd0d5773d3715692 compiled version
d8dadeee2dc8d07eef4f1e47ad480461d4151311 update hypershift to the latest version that compatible with library-go
23f6c38c2bd738ccdc8a11b98643c65ebdbe0cec Add target namespace info to the hub mirror secret name (#13)
68bb8f4abeea7047ef50c11c409c5ab1711bcf06 limit rbac for manager within the sample (#12)
9eae7b60883b9676961b8699c450aa143944c6fc Delete bucket namespace flag (#10)
659fe37fea0e74156c5e4e9dc69a8e247c28ca1e Disable install strategy all (#11)
acd2b808146b90d6327e00c2151c1f6b4d96eddf Make the hypershift operator image configurable (#9)
bf426f08d45441a389de8c3f611efe2f7e6a6d04 Merge pull request #8 from zhujian7/no-op-change
acb33e59b46c2d2dde466fc6aa354d1a8b13dfe9 No op change for rebuild
a32e6b629907b67a618ee5f36553e3a94ea237c6 Merge pull request #7 from zhujian7/non-root
57521fad2937306b4bcb08b1a3b1c81096002575 Merge pull request #6 from zhujian7/sonar
54445cd52137e322117382667ec09e11c1e3a69a Change user for the Dockerfile
4a89b05802b8b81c1648642fef745c7b2d22a09b Add sonar properties
b725dc1066630ab5c72f5460f70af749876db423 Merge pull request #5 from stolostron/watch-hostedcluster
b9e539f9ff8c08de9d932c449929905df0c2c835 watch hostedcluster owned by appliedmanifestwork and sync secret to hub
5fcfcbcba26ec65985c71c6960b7ac24b172db18 Merge pull request #4 from stolostron/secrets
add52a6378986e949c143813e21b0c25b4799be9 give agent permission to delete secret on hub
f39acc70de508f579103666180371559216de673 fix typos
669be3dc61e092b18f3d20d421a366bcf06cd627 add newline
cc228b49ae1378fd4a5843a4b627c870f8249145 secret clean up when hostedcluster is deleted
ad7fbd8bd0dffaa39a140da2b236620ef6f85d57 Merge pull request #3 from stolostron/fix-rbac-and-addon-namespace
bc196807096de5aab19de8f8fe01319c99d6deb1 make sure the hub client is set up correctly
eafffe755ba846c6e52c31eb5ed1667bf648ebf0 Merge pull request #2 from stolostron/use-controller-runtime
b219de62c8fa9b4d5a826cf6062ee5e06f20bd3a update deployment sample for addon manager
f16d311c974bc4f4c87100f4fdb2d769da013573 use controller-runtime to make sure the cache won't stuck
c9cca7165c02c2b7353755891855cf3c89468df8 use the hypershift library to install the hypershift deployment instead of running it in a job
2f8a895b86486a989d96961c58327d00afe86703 working when using hypershift lib directly
8c293f340bcd07ff18ea09dd01af41f4b187a87e fix go.mod after using hypershift install lib dirctloy
3edf4297b04dcfb17d80c6d09ae432f986da30e5 embed hypershfit binary to image
56fb42df33cb0764ad4b2bc2bcb46054a27840e4 fix some job teamplate issue
9bb3f5fe59d6e991c125d7512ff52dc714999ae4 only miss install script in the install job template
052a1868ebbc60c989469157dacd9227be224e35 sync hypershift generated secret from spoke to hub
527c515abb5d06182295bc4126a4c3866fa83fdf Initial commit
```

Status: Syncing successful
