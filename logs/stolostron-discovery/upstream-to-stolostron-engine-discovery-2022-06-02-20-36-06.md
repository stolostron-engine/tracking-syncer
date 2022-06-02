## Fast foarding of stolostron/discovery into stolostron-engine/discovery.

## Status Summary:

backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
27952abc604264eb9d391a622e8be5ea27d600b6 Update README.md (#129)
5bf12929112cdb5d94856a847583f84718c2033e Filter out deprovisioned clusters (#127)
a7de49ce12dc5283b16e9043b62110a5e9938301 update dependencies (#126)
604febe6b5b8022be3617992a382a6895e2d7b1d Revert "update dependencies"
8019b28e443cd66fddfc26b1a8d776217d5a96b8 update dependencies
49ba9cdb0599212a23393142015a75e0938163fc Add Description (#125)
2146116512bf12efda64cae1b78dac3f443bda4d Propogate deployment updates (#124)
98dfd0d822e52ccdb5b07a4f922f96c7c57798ec Update memory limit and add metrics port (#123)
cb10f4bf36f9e0a3331ab74a1e19740d20cb4cfc Refactor Metrics into Bundle (#122)
51b11c5c6aa79a86ae5d8cec0765127ba0a4cb63 Merge pull request #121 from cameronmwall/no-op-4
333840d4de75ec1a1fabcfb1b080f843f3f481f4 no-op 4
3d3c5401816f2b4d73e9f3a1e8c071e0b2c7e37e Merge pull request #120 from cameronmwall/no-op-3
b438ecc3b6256691869680bed9c5024f72819299 no-op 3
6c3753bae6b803873fec49717d7b5a0d482644fe Merge pull request #119 from cameronmwall/no-op-2
3b782b79f2a533393b748c1d86c85096a4bcb2bd no-op 2
74eb4d6f462945b0103c94cc9fc55ca8d04dca9a Merge pull request #118 from cameronmwall/no-op
4bab78a57dc961fe88da888d837531d6f48b159e no-op
6253407d9b9896dcd8477c1eb66799012aafd0d2 Add v1 APIs (#117)
ca8e2fda27ad44fecf75929bd58875be8f2097cc Update golang.org/x/crypto (CVE-2021-43565) (#114)
2d1c7114e13e6df3f5681fe49061bc2525afdda0 Rename open-cluster-management org refs to stolostron (#111)
cacaf9212b5c5f389fd7fb97b65f5575ca761813 Only cache metadata of managedclusters (#110)
74c6f43c409be12695cfb685e773d1c6274b56b1 Updates for release 2.5 (#108)
c51bd18d1836343a9b7430e7de7cb9ebc9a85cec Remove osdk alias from Makefile (#107)
49dfc9f974926da6b379afe0f2b57a858de3e753 Update osdk version in readme (#106)
b0f1212c14de9fd64510dc7eb8b0813c9e402180 Replace calls to deprecated ioutil package (#104)
8a4ac97653b60eae303c800ea584dd3f37a11159 Rerun osdk generators with latest version (#103)
8dc6462b069f59d54f85abe0dd0b9a451baf62a4 Update Go and dependencies (#102)
9f4115bf7b3f21dbc8a9f72648d430920574e4cb Refresh (#100)
946138011e4fe99d6d077973cafb918d1a527be2 Update for 2.4 (#98)
4c48e0505925e7b7638842ae425e951cdcf8de09 Remove duplicate annotate make target (#97)
3bd097f3ebfb0dad2abb5e60365f3a13e95235e1 Remove temporary token code (#96)
b8e6396b27aeac2dbc2987f562748f71c20cbb3e Log errors in scale test (#95)
f96129b48fb089215de3c4e23b411a9a6d481a69 Add scale test (#94)
e9eee625cb41e5c3ad75d1d3f790aab6539c894d Add custom metric (#93)
3dcff79cffacc306aa2c83d3c948fb765b0f8b97 prep for DCO signoff (#92)
e00b4bcb31df3e87ee219854400e3546bad3bd08 Run tests against PRs with Github Actions (#90)
79e1ebd2d0565007a867e442b2ba84c6791675db Use dynamic dates in mock server (#89)
80d38e9423dfc9588149ef09319267a8f7e5e395 adding type transformation of cluster type MOA to ROSA (#88)
8dec2656f7b84e05d3444789d02865a6e564a97e Adding type to discoveredclusters (#87)
37000844ff033659e5b03c3b2d6086880442d45b Copyright header check (#86)
a28b5e59e7e8c3bfd61882372e2b91504f4ede08 Simplify format of token secret (#85)
935e106b773d054217a0dd65fd10ddcee2721394 Organize Makefile and document running tests (#84)
263acd637c676c70a0c6bb3d3a932b4a446b2ab1 Add labels to testcases for issue triaging (#83)
82e3951535aa365c3efa2808daf6d5ff5f358471 Filter lastActive time to the nearest second (#82)
8dc514a9bade79adec8c2eb0a12946cb707dbaf9 Leave existing managedclusters alone during tests (#81)
195851e6fc75db60c9b2d81e0d80313a7c7dc14d Reduce directory permissions in generate.go (#80)
b4dd12ce934e55455697bc9b10aa51ea6a0e5e96 Replace periods with dashes in DisplayName (#79)
988a8b51ae39080b12a557f108e5ee4a96f8aad4 Add testserver dockerfile for Prow (#78)
1499d4720bc56275d6e066102409f18de21ce246 Testing improvements (#77)
62b5d1de6e136f1dc7d763d151fdab37f87341d3 Update DiscoveredClusterSpec comparison check (#76)
3ecb17e1064d28e3208825d7c203b6278c5a10fb Add apiUrl to DiscoveredClusterSpec (#75)
397aa0dd22c607401271aa28797912f19e936eba Version updates (#74)
3da1763b8ae5e393909cf0bf40ebe3eb9b904ff7 Update filtering logic (#73)
1dc7c6e8199efd88e224ac3b4fb4466238656308 Address sonar vulnerability warnings (#71)
7a62244e3677b3368f61b85134593ec656e6118f Add DisplayName (#72)
ed02cb211f7b23efd050484db538eebf58f957d7 Add credential field to discoveredCluster (#70)
42ded7eb908370f50f1bdd45129266fa7077e241 Default name of discoveryconfig to be discovery (#69)
85cc91e0978925931ec37be76b7aba716c4c8dc2 Multi-namespace support enhancements (#68)
1acf6efcc382b76d077b540d941c7835b73a6184 Fix bug in assignManagedStatus (#67)
76503c23e7dd98c79d00b2929ef7949b68ff4510 Add credential field to discoveryconfig (#66)
010f37d78b195c5ff2439cec1cfa1e42b50f6eec Add discovery-operator serviceaccount (#65)
7862a2fcf877dd66b49ad82ca57ed1dccd636852 10542-Scalability (#64)
ef8cc511f15f90d8180f9632d22efc3c01e74a70 Delete existing clusters after unrecoverable errors (#63)
211ada4260994da07b69e28d088fa4bd5fd1fd5a Update DiscoveredCluster spec and remove clusters_mgmt api (#60)
c07175ae800ec1201baa7b1fabb3b1fc8c10b312 Remove arch from Prow dockerfiles (#62)
3988afe96ede3928237c4780112b20203be99fda 11336-remove-cicd-owners (#61)
41db975b96c4b3c7d644457e62510d745dc42c35 Remove discoveredclusterrefresh from project (#59)
d50a3ca0736bbbbb67a79e952b7db4d8fc359629 Update go to v1.16. Cleanup dockerfiles. (#58)
1894511fbe6ae6c91f1c7053ea6eef537eb23588 Organize logic to support multiple provider connections (#57)
0c8f772715d601e5d5d0e30d57bc69991a0d273b Remove commented out code and delete AfterSuite, which is now handled by AfterEach (#56)
202fa46c7287b59b8e54a25656330b3a4b5568b8 Add Prow Dockerfile for building e2e test image (#55)
c3d09d8c067933fe36b9ca4e73e212f20b80ec15 Enable running tests in KinD (#54)
0493d3354e2dfa70bf656b80e9ec7d88b8ba553b Reconcile on any updates to discoveryconfig. Gracefully handle error due to config being deleted. (#52)
6a9ebcb5f5bb027fdc4bfeb2f3b0240eb281a09d Refactor managedcluster controller to move logic out of reconcile function and into separate functions. Replace functional tests with unit tests. (#53)
43a43cdab77a591938f4c9e1d03f5832253de9ff Update README.md (#51)
52a382fbb415df16b587ce4e5a70cbcfb10bec70 Update README.md (#50)
df3e38bb6b1755ecf17431d48cff9453d639496d Update README.md (#49)
cc05dee917c105e44f9cc5b7fc10b72e45cf4986 Remove travis entirely (#48)
3eeeb346a6ea5f49c8faf825a64b46f71f9c2cb0 Add OCM subscription api and filter archived clusters (#47)
1ff6dfedd937754fd0eff3aa83ceb256a2899197 Update README.md (#46)
8dda09de67f7c8bfd7362ca64a5e5ef569c180cf Update README.md (#45)
688f76fcfbeba77c3ef43e1bd0dcf423dc9093d6 Add Architecture Diagram and Roadmap (#44)
69461b908dae95a00f04c49280347a752402e97b Update Makefile (#42)
17b514b382a34d3f771ada84167844307dac9e68 Fit and finish open source (#41)
cf420530e3ae10abf652a4a514bb589e765087ff Add DCO and Contributing.md (#39)
d335b57035e4f4da7c427a24c18ced3cc25f8ec1 Remove publish branch from Travis entirely (#40)
9dd2fec2cc819772fefdb53f1c979ea24b6802b0 Update go version in readme (#37)
88b2f7c6c4d1c67287e259919d5a4dab51902a60 add eol to sonar-project.properties (#38)
7c266a4b518ad163441faeefd3cefc4db9b75ea0 Uncomment include in prow makefile (#36)
bc33e1e07464db7591e236ca95e6448a371604cb Remove sonar and publish stages from Travis. Keeping publish of test image (#35)
6c988ace535b56286ab1a325c7575f6eff01ac72 Sonar changes (#33)
6e6284a08143b0ba071b92b1b15aaaca31b45622 Sonarcloud onboarding (#32)
bf36dc0d6dd39932fbcdf2a4f26d136f4ab0d912 Add cicd members as approvers/reviewers (#31)
9a64d6680091e60aeb0f3a4ae6598b6084484304 Merge pull request #30 from open-cluster-management/unit-tests
99655ba1184394d97143470dbcfbbc1eb95664c4 Add way to run unit tests that don't rely on a mock server or envtest
299edb1f3af61b390642c0bea798c54016a875d7 Merge pull request #29 from open-cluster-management/add-prow-files
98eeee088d186ea05f4bf690e74597b6aa70e1ee Add Dockerfile and Makefile for Prow jobs
ca92c6ccc2611e258a2b6143b85ba7552c4549d0 Merge pull request #27 from open-cluster-management/post-main-branch-swap
02ed8a3a17ae03b6a42033f741171c1fcbd42463 remove nl from release main branch file
48ff32a22c12e3a1208eaebd1bb917c766f19726 Update README.md
fa3d1e6506d4f310fbc434e2de1855f02152912a Merge pull request #26 from open-cluster-management/prep-for-public
694b1d386989f43b9b85a051253027c9bd6f90b2 Merge pull request #25 from open-cluster-management/adding-copyright-header
7f0c37be30bffa182038c28614f85ef41f2e8265 don't add to mod file
7179c53ee3fe3febd77ad8c02ce1814d34b74d7e don't update sum
fc7f30df166db5b985c2a297fab193887a47d09e fixing newlines
87f440147378af3d15816f915b1b64a0679505b4 adding copyright header, need to test before merging
617a37433862d1ddc4d722d5c9cee8384b74f710 removing unused parts
0bfa4ccec2ebc363f23a6d290dd6bd700ed13638 renaming default branch
96138d57341621eb9ebee3451fa405f4bfc7c010 Merge branch 'master' of github.com:open-cluster-management/discovery into prep-for-public
750426911f7a8c0edb69f99548b1a7e2b7f4b93e add disclaimer in readme
bfc3f154f243291768f091ace75d979a3f74350a Merge pull request #24 from open-cluster-management/update-api
09ede0f4a369119db5e321ebcd9dfbd8cb755322 prepping for open source
b7e276a283a05887be374c922aaaa9596e20715a update description text to label field as nonfunctional
b5f8d6e8de4a60d109502b5863342e0037635de6 use activity_timestamp instead of creation_timestamp
504be34b81ae9025655897d57d49a39494862128 fix spelling error
19bcf962074727f795607ff3efdbfec8b8505afe update operator-sdk and regen
c27d662be2b9e1afeff03228075a80211718b421 update function test
60675c07103eda1f6c447a728c0bc80cf4bc6200 change age to lastActive, add openshift versions
4cbc30488f6e586b1a0da9eb4d979c8fd76c6351 Add managedcluster controller  (#21)
24546c406853367fabd2e6e52890e3ddb6825788 Generate v1 CRDs (#22)
2b23d95efa19a6d9c2f6c6be8701dfd73847d0a4 Update discovery.clusterserviceversion.yaml (#23)
a75bc832106c14199cdc90252475d1aced7a832f Override ocm url with annotation (#19)
61d32ab181199af2bf21cff5ed5468012c0a5f60 Update to use osdk v1.3.0. Fix tests (#18)
12d8a5e35f693010967904d0f258544dbdcb1adc Update fast-forward branch to release-2.3 (#17)
7bbd1dc5a6862780df4a5c2f9628371079afb102 Merge pull request #15 from open-cluster-management/link-config-to-providerconnection
4d7464a63a4905ceba0c2b2336c1dc5563421651 link discoveryconfig to providerconnection
21f86bd3f3dbf2fcc27221fa65c23b947eeefb79 Change discovery controller to discovery operator (#14)
65787bc063934af63689cbf86bf24d35d36b7348 Add controller references on newly created discoveredclusters (#13)
814083ff59facdd2a4666eb85d9e402af8ab9021 Update go version to 1.15 (#12)
8a2e151f4330cc822796a765b43e119076e6ee08 Add controller for discoveredclusterrefreshes (#11)
099a2c3d3e2263fe4504f9ff299989cd39932aa9 Update README.md
8022d408c49aeb43db4f16732e66ebaea97406b8 6584 staging (#9)
335852e7a58e959cc2690da89b0a3e5360dcee1e Add initial bundle material for merging into the composite ACM bundle (#6)
a9aebd16e72dd8a5d01af83655e208a939c32d4c Move OCM mock server into its own contained directory with a separate go mod. This lets us build the discovery image without including modules only used in the mock server and vice versa. The testserver's Makefile has also been updated so it should work whether it is called from the base directory or the testserver directory. (#4)
66174b5fb8936fbf77ec7c4fd5ee5aff53f4eb2b Add a field for provider connections and subscription information (#5)
058c07f8cd825186bde0cfed85da958ffb368379 info to spec
20314d678b1ba3c90691954b4c2523d9cb80edca Merge pull request #3 from open-cluster-management/cluster-spec
90d82e0a3e9a2f7edc47c1aa6c5edd92c21476ed Add spec field to discoveredCluster because operator-sdk expects it
53549f442fec50e3c12055c311e8fe18efbe61f1 Merge pull request #1 from open-cluster-management/add-testing-server
1babd5179864c1cfce74ee9fb4bd58df8d14e513 Use same pull secret to get mock server image
67b63d93d896ba084d7a8f53000390aa3d9bdc2d Merge branch 'master' into add-testing-server
23286814522252ef691242f452742686447485bb Merge pull request #2 from open-cluster-management/cicd-onboarding
dc504aa3b9ff18865fccba4e803e9d1ce4bd051b Up deployment memory limit
0891272d8665cbe4062c54226efe2b6601c2e97f Change image name from discovery to discovery-operator
0e063ffdf26cdd5d084146ec395bb986611fbe1b Remove copied files
92f5b7852df43cd24298fdce2608183a439743bd Add files for CICD integration
0910a2512c67f9f013e132ded0ac82c0b2561916 add Makefile.test
4c7f35298abf3c4bac240c90ae53976740403f39 Add Mock Server
eeef7005580d6b10b1c96dc31dedcee9e01f5da2 first commit
```

Status: Fast-forwarded successfully.
