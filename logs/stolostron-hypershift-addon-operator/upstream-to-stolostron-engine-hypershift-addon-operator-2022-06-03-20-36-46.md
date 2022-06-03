## Syncing stolostron/hypershift-addon-operator with stolostron-engine/hypershift-addon-operator

## Status Summary:

backplane-2.1 -> backplane-2.1: Synced commits but not tags.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Synced commits but not tags.  

### Branch backplane-2.1 -> backplane-2.1:

New commits (first branch sync):

```
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

Status: Synced commits but not tags

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits (first branch sync):

```
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

Status: Synced commits but not tags
