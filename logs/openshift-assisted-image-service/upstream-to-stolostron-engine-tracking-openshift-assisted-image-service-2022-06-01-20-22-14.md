## Fast foarding of openshift/assisted-image-service into stolostron-engine/tracking-openshift-assisted-image-service.

## Status Summary:

release-ocm-2.6 -> backplane-2.1: First run, created backplane-2.1.  
release-ocm-2.5 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-ocm-2.6 -> backplane-2.1:

New commits (first branch sync):

```
2f689a1084b8b0cedc7b2c787ad7222624fde662 Bug 2078531: add an option expose all endpoints on plain HTTP port (#71) (#74)
95f275cd8f19d972c1a38518595bca17a64bd170 hack: use `go install` to install goimports and mockgen (#76)
d983e9eddb62231ff3a3bddb4c8456195ff619ca Revert "Bug 2078531: add an option expose all endpoints on plain HTTP port (#71)" (#73)
82eb5029ef5e64dffdbdfad5d1e0fadb059a6a15 Bug 2078531: add an option expose all endpoints on plain HTTP port (#71)
c8cef07941f80a2214228fe9dd53a569eb459a75 Set Last-Modified time for iso and initrd downloads (#72)
d67d761513d06f2d3ca95de35176e3c66c0ab00b Update openssl libs in Dockerfile (#69)
49899bb8384a40fcc080b93b25b3d829fa6d0f4d MGMT-9538: Only log.Fatal from main in the image service (#68)
1ebdfb91f2c5a05888adf160cba7dd74cd43fd52 Return a 503 from images and boot-artifacts before downloads finish (#66)
21fd9b967745e8fab4a4c5e9e1f14989fb608dcd MGMT-9019: Download ISO images in pararell but work with them to build the minimal ISO sequentially to reduce the storage required for the whole process. It increases a bit the execution time, but is worth it (#65)
054a1afa8d28f4bcfcbc742b1c16e7b39164c96d MGMT-9333 Add ipxe-initrd endpoint for customized initrd (#64)
40ad31d5abf75105bd746a0951e57fc61aeb313e MGMT-9332: Add endpoint for rootfs and kernel (#62)
10a987fbc26110c8e1b7f434e7bb76a04ba57382 Fix overlay reader for base readers that return EOF early (#63)
ea4c14e09ef34d85ee2fb766567104d7ee9790f8 Use fields from http.DefaultTransport in imagestore (#61)
97da3acc1a6ae3610a9b41b43553311f5ad42058 Update go-diskfs dependency (#60)
96cda90a73533a79f20c4c91ccdc157a27ff6fc1 MGMT-9187: Publish coverage report (#59)
a9f6dc6bd2cf99a2be89d4259d5b1a29587b5c84 NO-ISSUE: Update RHCOS pre-release x86_64 image URL (#58)
e61d9e7d26d4db591aadd69e37664f86d4598f02 Bug 2034686: Allow for disabling TLS verification for fetching ISOs (#53)
2fbf226ace539347375d3cc661645ff15e01cd2c isoeditor: support editing FCOS grub.cfg (#50)
0418b5553969dbde41bd60f17542ea5390d8c767 MGMT-8927: build image from scratch to handle possible cleanups (#56)
a13506f65332281556e5d601f3ef4399865cf3fc MGMT-8925: allow more size in requested PV to store all images (#55)
5a37cb590dceb2834c23db5ec0229c10c3776b9b Add os image entries for 4.10 to imagestore and template (#54)
e43b2410af234ed573ec2a2713873ba649fbb279 MGMT-8661: Added openshift_version to image path template (#52)
7912abe558e4dc13ae57b2854bdb157f2f5320cb Handle CORS headers properly (#51)
725ace298b84e71cfa4be6be364f7483692cc1e0 Set the Content-Disposition header (#49)
319229cc2680f4d8ef82567240e568abcfd63bb8 Add monitoring template for gathering metrics (#48)
c53b4ee0adb81a6c581af30071bda2093c31f794 Support OS_IMAGES as well as RHCOS_VERSIONS (#47)
557d6c1b005809ee783db3357146f13b210a7bb1 Pass the status code through when assisted service request fails (#46)
a6f4e9968f11ac730523a38fe17bac0661a885ed MGMT-8306: Use renameio in downloadURLToFile (#45)
1cc99ed1c6bc9187c069509a3b1764ce28aa678a Use edge-infrastructure image instead of ocpmetal (#44)
1552361c0458d9035f9f456867665e71680dfd54 Close the ISO file after serving a request (#43)
cdcb2b829ab21ae8ce813b6c0dead330f505901d Add the ability to customise PXE files (#42)
034967d32be6a616013717c2c01697233f6e4a44 MGMT-8216: Handle persistent storage for the data directory (#39)
df7c37591acd5b87a5bbaf2120fac236819d66f1 Add a template to deploy to console.redhat.com (#41)
24cda2dcc77cbf2dc0bcb601b41b8391d5cceccc MGMT-7897: Rework authentication handling to support image_token (#38)
3986a90c45eb663a2b8e1c344608c7ce3c0f0017 Update owners file (#37)
22107db3e9d2960b46ab6e2aee34ea3c7c821834 Bug 2012796: Add liveness endpoint (#36)
4010348b8e14117126a4e3ddd71ab922c11e0711 Make Ignition archiving code public (#35)
9137c9ff632369985811019b574148fd6b5d9795 Bug 2010276: Image service should fail if no RHCOS_IMAGES are provided (#32)
cf04daf26936587e561bec7fdadb390f02894569 Bug 2010819: Use the request context when making requests to assisted-service (#29)
6bc1574a5a295eb8befee8098f30cb1b0408aa53 MGMT-7734: Integration tests for the image-service  (#28)
416570d913d1344a54c56d71892d8636ed2897a2 Limit requests in flight for image downloads (#27)
990475c3bc76b8133ad6ba7b7b4821b34d685342 NO-ISSUE: Fix typo and formatting in readme (#26)
cbe44d6641408ce20dbe1176281b67383c5114b1 MGMT-7762: Switch to stream8 (#25)
5a574a41f4388b253f4c8b2e84fd58e0b24b84bc MGMT-7754: Support iso creation with EFI boot only (#21)
93e6b832d744fc5ac310f8564f6bf86889701cbb Align type values with those from assisted-service (#23)
2ad31f7bfa30ee4a7d7ed4d0ff94d8b55ee84091 MGMT-7762: Pin the UBI version to 8.4 (#22)
9c9aeeea0f399d169f109382932c510503793f66 Add support for multi-arch base images (#18)
e0f69c62a43e9c134cedb091d4dab678788a449c feat: support self-signed certificates on assisted-service (#19)
0afd62c70b06cb3fee29c0f991a69488adbef59f NO-ISSUE: Ignore Dockerfile when copying files to image (#20)
444604a3bea438bdd1a3cf92513a61625f814ef3 Use array format for versions and add image arch support (#17)
ade86965c3da51de2f253e3feee68eee0111a6e7 Query initrd content and embed into minimal isos (#15)
8675374a2fc26898ab5b29d110d1700e38656272 move to v2 api for discovery ignition (#16)
6418977e725a2894a40650845a334640ae8ab0be Use docker for build script instead of podman (#14)
1f34613c70379ffb5a7b3fe6828ae9d5a4bb3c9d build_deploy.sh chmod +x (#13)
d048ddd204e88625d58bf0459a53cb1e026167f5 Rename `Port` to `ListenPort` and document `ASSISTED_SERVICE_HOST` format for clarification (#12)
6a8831e995984718c682cd8a33dd56abb2fd7bb3 MGMT-7499 Take an auth token as a query parameter and pass it to assisted (#9)
6aa491c00377e2af70c1cb9bf9ac2be29851f5e7 Add pull request template (#10)
8b8c22e4f95d826d2506a4f70d44c5b7c94f3a00 Add build_deploy.sh script to create app-sre image (#11)
b910b5cd5617aa374acf2e91b59c82d9516304a8 MGMT-7256 Add ISO stream customization (#8)
a14dbde369a71fbae33a15c300ca4750a8d732ce Clean up test setup duplication (#7)
826093a143ea0330882d635e6fca8261962a6a6b Merge pull request #5 from carbonin/add_minimal_iso
6bbb0fb45b5f16ff520ea5b7a74c757818533821 Add type query parameter documentation in README
3720baec2bdeaf1590f87806a0eb28e0930ab442 Move isoeditor from /internal to /pkg
c336cdb2668c836b6d5aa7757798761179ae641e Get tests working after isoutil move
b17a4d5fd593cd64e14aadc98ad0e10c1a93cb2d Move isoutil into the isoeditor package
656d5abc88ebe7c7a2c12e657c2a687151195567 Create image store correctly in main
947eaecccdda181d6e067ba581cd80edc007a442 Pass the editor into the image store and test minimal iso creation
440f401f7b67c75304819e0bb25e641a2db7d1b5 s/carbonin/openshift/ in imports
ffbe2880cfd8b8af55e5e77fc598a5b62ebafab1 Use the new isoutil functions in isoeditor rather than a handler type
ed9c75ace0f8b642c991631146ec02f6c38be227 Simplify isoutil
c654828fb49e4634b70b4e4b9eab00a07751c358 Add "type" query parameter
e0c16d041fcb05f9a191b8faf2cea0679e00b231 Sync files in the iso workspace before recreating the iso
4cc11cdb8c1591cae5f266a54519a392e4333cfa Use the imagestore data dir in isoeditor
490d786d163ea92e3ca9f9ebcf381996ece85d8f Remove unnecessary log line
d433f6d18049bafe5d2b8dc6b9d4627e88ceb484 Create minimal isos in the image store
472e34ed52a6c8fe68ef00e43bbd8569f2b7715b Use the default log instance everywhere
6be0030c2b35a24bcc11b998be3a57d21c9a1dd2 Remove isoeditor factory, get tests passing
4db243f362f8d89af0977cbc4f7d67f5c2ed252b Remove iso customization from editor
a53b34ad4726292fd1f1641fab448cf76c447c54 MGMT-4942 Download rootfs from mirror.openshift.com (take 2) (#1697)
4d38ec308b8d8195de5b8c43c4a02fa58694be74 Revert "MGMT-4942 Download rootfs from mirror.openshift.com (#1669)" (#1686)
59edac26c0a3ab8df124878d83bdafc5efb74073 MGMT-4942 Download rootfs from mirror.openshift.com (#1669)
f855c405faad17d3618dcb38d1900aaa3be72e48 MGMT-4072: Remove coreos-installer dep (#1177)
0c53517c3fd76bf5fd57793361573a275f9d2435 MGMT-4693 Make minimal iso boot with UEFI (#1372)
f1635d503c3b5090b6ea42a592b130ea5ae81b9f MGMT-4366 compress custom ramdisk archive (#1260)
d21b5d9d049ff8a1d4ced336c17192e5d5ccf9dd MGMT-4365 validation for custom ramdisk size (#1251)
1129e92f4e49dd262a251b96bec1134cdc543d32 MGMT-3979: Embed ignition and ramdisk into cluster iso (#1151)
8013e367728c64a69f619f24eec39da3a23471d0 MGMT-4095 - update minimal iso flow to work with nmstate static network configuration (#1178)
b4ef07a30b92101c024e5f6a9907daaef69a8930 MGMT-3982 Store initrd metadata in system area (#1171)
cd18595867dce6315e4871f488361b6a537a5f56 MGMT-3976: Embed ramdisk placeholder in template (#1150)
c00062d05d69b5b6bea0a8c7bcd83bf2ed195ee3 MGMT-3970 Make the iso editor scratch space base dir configurable (#1063)
0323832e6b0c01cfec4c81591e741fc3f34e40dc MGMT-3999 minimal-iso proxy - capital env vars (#1090)
8b0440080f861215eacc9859839ebf027d43184d MGMT-3999 http proxy support for minimal-iso (#1075)
c87bce8fa6accb12b92893721c471d1d416bbd30 Upgrade golintci (#1077)
60f45dc3e2d4b24570c200a7dba203f4396727f4 MGMT-3844 Limit concurrent minimal iso generations (#1032)
f2685fcc495f57022aa010f0e07eb8b7841c4799 MGMT-3510 Set static IP during boot in minimal iso (#986)
0d2e7091eecf74c61c2a4f82c416ad86796a68f9 NO-ISSUE Fix format issues found by gosec, update format-check (#950)
e68d4d3a4d91dca58247c966b068dd9e10469004 MGMT-2977 Cluster specific minimal iso (#932)
f0909a3c25cc7c81d37090366af6421bcbd00ba5 NO-ISSUE Move commands to hostcommands package (#948)
bb25cb3bdd6c386fec0346fa7eebcee1f79fe74a MGMT-2977 Remove coreos.liveiso kernel param for the template minimal iso (#930)
9458b2d03c0c472691a9dc1628fe9f6e59afda5c MGMT-2976 create and upload minimal iso template (#911)
d1f8895fc572725251375adc36e51eb8635a7f05 MGMT-2977 Enhancements to isoutil (#901)
5cbc89388fa6bb71fa3a4be4a72004939a045443 MGMT-3514 Add extract and create methods to the iso handler (#803)
d4023cce826797a96322e43ade4255f6f30b91b4 MGMT-3353 RHCOS per version (#869)
82b0d6d824f0d4a727fd054de84b2f9304ff11da MGMT-3297 - support static ips when rebooting nodes woth RHCOS image (#872)
bdcab0069f6c71f5eadc8706bbe03c617f755bc7 NO-ISSUE - make format target shouldn't format anything the linter doesn't check (#876)
4794165211f1721eb7ae27e471a4c3b7b54256bf MGMT-3456 - Will not attempt to format bootable disks that look like installation media (#862)
b23e32ab3695fdd735e6297670aa35615c451089 MGMT-2245 Extract OCP version from OCP images (#856)
7fb7f6ed800581ecb632d52ec4463395ecafe8a9 MGMT-3100 Upload/download PXE artifacts (#755)
c1696a87bb6363eb821414983f7fd7d52bed27bc Add setup script to share logic with prow (#6)
d30452bcb1a7be440adcc47f0289723220720e65 Remove github actions configuration (#4)
56e0862a4f742c53c1f382c8f48da552203b94f3 Change package and module references from carbonin to openshift (#3)
f3a8fb8ebfc594c2a7495aac2c546f464c878676 Merge pull request #2 from djzager/owners
b19d5a6481f6d98b1d7156e9014991419f59ac4a chore: add OWNERS and OWNERS_ALIASES files
b6be0e3c2ce16125fcca148bca63a953f455a9e1 Create github action for image build and tests
6f134fba60baf06c7c4ff13656ba20cd31e17f66 Remove the build directory
829a5accf65b9d21c31790846e548ec63452766e Update README
e27676e5f5ddf130e721ec48730dfc3ac468ce09 Replace standard library logger with logrus for json logging
78a4a5e42dff4157f7af3f0694ec98b2be613538 Add https support
0c1093dad4e3c44ca439aee499783c06d197bd7b Make port configurable
b97a61f5acc54b920c3c8b5a7882d8d383011034 Add tests for images handler
6d6b30818cf4836654ca6f4fb3c8ef961f274ed0 Make ImageStore an interface and add a mock
a8ac043b4a1774f20bad9d8ee12c8797f2653435 Base image downloaded on version query param
363196cad21a9af342080be74e84770b8a6433d7 Add metrics for the image handler
3e5013554d772084fef5545d0767ac71fbadbf71 Add basic go metrics
32aeec63e053769398dd6d037b3084af0da24482 Rename handler files
7efa5028a80ee8f7131fe6e7c4f63fbf3ee9efd6 Fix image override bug in imagestore and add tests
2ae06b2747f6b2034c791b0a3bda9531bd6b265f Move image request handling out of main.go
d1dd8a486717ed769c73e35e98b70bd9eff0d93e Add a health endpoint and handler
f5a2eced17e504d64aad0212b9e4cb508c912f15 Use built-in NotFound function
3d15d751beddc83dd05d0a6190fa13940cb79853 Move default versions into imagestore package
36df091f2af07b63443d282fdacb16351ab92a15 Add skipper support for running lint and eventually tests
02fe4857601040115c6602ac96e7aa200fa3ac85 Initial Commit
87143a11e740270c2193c90a60fb762918632f98 Initial commit
```

Status: Fast-forwarded successfully.

### Branch release-ocm-2.5 -> backplane-2.0:

New commits (first branch sync):

```
32ef0fdd5f796b3f910d1b53be4b75cf77319204 Revert "Bug 2089195: [release-ocm-2.5] add an option expose all endpoints on plain HTTP port (#77)" (#78)
b719eb5189986373bc30eab9fa755d35717efe73 Bug 2089195: [release-ocm-2.5] add an option expose all endpoints on plain HTTP port (#77)
143162a1b03d47da6b020a49c45f6a534efe2c6c Update openssl libs in Dockerfile (#70)
21fd9b967745e8fab4a4c5e9e1f14989fb608dcd MGMT-9019: Download ISO images in pararell but work with them to build the minimal ISO sequentially to reduce the storage required for the whole process. It increases a bit the execution time, but is worth it (#65)
054a1afa8d28f4bcfcbc742b1c16e7b39164c96d MGMT-9333 Add ipxe-initrd endpoint for customized initrd (#64)
40ad31d5abf75105bd746a0951e57fc61aeb313e MGMT-9332: Add endpoint for rootfs and kernel (#62)
10a987fbc26110c8e1b7f434e7bb76a04ba57382 Fix overlay reader for base readers that return EOF early (#63)
ea4c14e09ef34d85ee2fb766567104d7ee9790f8 Use fields from http.DefaultTransport in imagestore (#61)
97da3acc1a6ae3610a9b41b43553311f5ad42058 Update go-diskfs dependency (#60)
96cda90a73533a79f20c4c91ccdc157a27ff6fc1 MGMT-9187: Publish coverage report (#59)
a9f6dc6bd2cf99a2be89d4259d5b1a29587b5c84 NO-ISSUE: Update RHCOS pre-release x86_64 image URL (#58)
e61d9e7d26d4db591aadd69e37664f86d4598f02 Bug 2034686: Allow for disabling TLS verification for fetching ISOs (#53)
2fbf226ace539347375d3cc661645ff15e01cd2c isoeditor: support editing FCOS grub.cfg (#50)
0418b5553969dbde41bd60f17542ea5390d8c767 MGMT-8927: build image from scratch to handle possible cleanups (#56)
a13506f65332281556e5d601f3ef4399865cf3fc MGMT-8925: allow more size in requested PV to store all images (#55)
5a37cb590dceb2834c23db5ec0229c10c3776b9b Add os image entries for 4.10 to imagestore and template (#54)
e43b2410af234ed573ec2a2713873ba649fbb279 MGMT-8661: Added openshift_version to image path template (#52)
7912abe558e4dc13ae57b2854bdb157f2f5320cb Handle CORS headers properly (#51)
725ace298b84e71cfa4be6be364f7483692cc1e0 Set the Content-Disposition header (#49)
319229cc2680f4d8ef82567240e568abcfd63bb8 Add monitoring template for gathering metrics (#48)
c53b4ee0adb81a6c581af30071bda2093c31f794 Support OS_IMAGES as well as RHCOS_VERSIONS (#47)
557d6c1b005809ee783db3357146f13b210a7bb1 Pass the status code through when assisted service request fails (#46)
a6f4e9968f11ac730523a38fe17bac0661a885ed MGMT-8306: Use renameio in downloadURLToFile (#45)
1cc99ed1c6bc9187c069509a3b1764ce28aa678a Use edge-infrastructure image instead of ocpmetal (#44)
1552361c0458d9035f9f456867665e71680dfd54 Close the ISO file after serving a request (#43)
cdcb2b829ab21ae8ce813b6c0dead330f505901d Add the ability to customise PXE files (#42)
034967d32be6a616013717c2c01697233f6e4a44 MGMT-8216: Handle persistent storage for the data directory (#39)
df7c37591acd5b87a5bbaf2120fac236819d66f1 Add a template to deploy to console.redhat.com (#41)
24cda2dcc77cbf2dc0bcb601b41b8391d5cceccc MGMT-7897: Rework authentication handling to support image_token (#38)
3986a90c45eb663a2b8e1c344608c7ce3c0f0017 Update owners file (#37)
22107db3e9d2960b46ab6e2aee34ea3c7c821834 Bug 2012796: Add liveness endpoint (#36)
4010348b8e14117126a4e3ddd71ab922c11e0711 Make Ignition archiving code public (#35)
9137c9ff632369985811019b574148fd6b5d9795 Bug 2010276: Image service should fail if no RHCOS_IMAGES are provided (#32)
cf04daf26936587e561bec7fdadb390f02894569 Bug 2010819: Use the request context when making requests to assisted-service (#29)
6bc1574a5a295eb8befee8098f30cb1b0408aa53 MGMT-7734: Integration tests for the image-service  (#28)
416570d913d1344a54c56d71892d8636ed2897a2 Limit requests in flight for image downloads (#27)
990475c3bc76b8133ad6ba7b7b4821b34d685342 NO-ISSUE: Fix typo and formatting in readme (#26)
cbe44d6641408ce20dbe1176281b67383c5114b1 MGMT-7762: Switch to stream8 (#25)
5a574a41f4388b253f4c8b2e84fd58e0b24b84bc MGMT-7754: Support iso creation with EFI boot only (#21)
93e6b832d744fc5ac310f8564f6bf86889701cbb Align type values with those from assisted-service (#23)
2ad31f7bfa30ee4a7d7ed4d0ff94d8b55ee84091 MGMT-7762: Pin the UBI version to 8.4 (#22)
9c9aeeea0f399d169f109382932c510503793f66 Add support for multi-arch base images (#18)
e0f69c62a43e9c134cedb091d4dab678788a449c feat: support self-signed certificates on assisted-service (#19)
0afd62c70b06cb3fee29c0f991a69488adbef59f NO-ISSUE: Ignore Dockerfile when copying files to image (#20)
444604a3bea438bdd1a3cf92513a61625f814ef3 Use array format for versions and add image arch support (#17)
ade86965c3da51de2f253e3feee68eee0111a6e7 Query initrd content and embed into minimal isos (#15)
8675374a2fc26898ab5b29d110d1700e38656272 move to v2 api for discovery ignition (#16)
6418977e725a2894a40650845a334640ae8ab0be Use docker for build script instead of podman (#14)
1f34613c70379ffb5a7b3fe6828ae9d5a4bb3c9d build_deploy.sh chmod +x (#13)
d048ddd204e88625d58bf0459a53cb1e026167f5 Rename `Port` to `ListenPort` and document `ASSISTED_SERVICE_HOST` format for clarification (#12)
6a8831e995984718c682cd8a33dd56abb2fd7bb3 MGMT-7499 Take an auth token as a query parameter and pass it to assisted (#9)
6aa491c00377e2af70c1cb9bf9ac2be29851f5e7 Add pull request template (#10)
8b8c22e4f95d826d2506a4f70d44c5b7c94f3a00 Add build_deploy.sh script to create app-sre image (#11)
b910b5cd5617aa374acf2e91b59c82d9516304a8 MGMT-7256 Add ISO stream customization (#8)
a14dbde369a71fbae33a15c300ca4750a8d732ce Clean up test setup duplication (#7)
826093a143ea0330882d635e6fca8261962a6a6b Merge pull request #5 from carbonin/add_minimal_iso
6bbb0fb45b5f16ff520ea5b7a74c757818533821 Add type query parameter documentation in README
3720baec2bdeaf1590f87806a0eb28e0930ab442 Move isoeditor from /internal to /pkg
c336cdb2668c836b6d5aa7757798761179ae641e Get tests working after isoutil move
b17a4d5fd593cd64e14aadc98ad0e10c1a93cb2d Move isoutil into the isoeditor package
656d5abc88ebe7c7a2c12e657c2a687151195567 Create image store correctly in main
947eaecccdda181d6e067ba581cd80edc007a442 Pass the editor into the image store and test minimal iso creation
440f401f7b67c75304819e0bb25e641a2db7d1b5 s/carbonin/openshift/ in imports
ffbe2880cfd8b8af55e5e77fc598a5b62ebafab1 Use the new isoutil functions in isoeditor rather than a handler type
ed9c75ace0f8b642c991631146ec02f6c38be227 Simplify isoutil
c654828fb49e4634b70b4e4b9eab00a07751c358 Add "type" query parameter
e0c16d041fcb05f9a191b8faf2cea0679e00b231 Sync files in the iso workspace before recreating the iso
4cc11cdb8c1591cae5f266a54519a392e4333cfa Use the imagestore data dir in isoeditor
490d786d163ea92e3ca9f9ebcf381996ece85d8f Remove unnecessary log line
d433f6d18049bafe5d2b8dc6b9d4627e88ceb484 Create minimal isos in the image store
472e34ed52a6c8fe68ef00e43bbd8569f2b7715b Use the default log instance everywhere
6be0030c2b35a24bcc11b998be3a57d21c9a1dd2 Remove isoeditor factory, get tests passing
4db243f362f8d89af0977cbc4f7d67f5c2ed252b Remove iso customization from editor
a53b34ad4726292fd1f1641fab448cf76c447c54 MGMT-4942 Download rootfs from mirror.openshift.com (take 2) (#1697)
4d38ec308b8d8195de5b8c43c4a02fa58694be74 Revert "MGMT-4942 Download rootfs from mirror.openshift.com (#1669)" (#1686)
59edac26c0a3ab8df124878d83bdafc5efb74073 MGMT-4942 Download rootfs from mirror.openshift.com (#1669)
f855c405faad17d3618dcb38d1900aaa3be72e48 MGMT-4072: Remove coreos-installer dep (#1177)
0c53517c3fd76bf5fd57793361573a275f9d2435 MGMT-4693 Make minimal iso boot with UEFI (#1372)
f1635d503c3b5090b6ea42a592b130ea5ae81b9f MGMT-4366 compress custom ramdisk archive (#1260)
d21b5d9d049ff8a1d4ced336c17192e5d5ccf9dd MGMT-4365 validation for custom ramdisk size (#1251)
1129e92f4e49dd262a251b96bec1134cdc543d32 MGMT-3979: Embed ignition and ramdisk into cluster iso (#1151)
8013e367728c64a69f619f24eec39da3a23471d0 MGMT-4095 - update minimal iso flow to work with nmstate static network configuration (#1178)
b4ef07a30b92101c024e5f6a9907daaef69a8930 MGMT-3982 Store initrd metadata in system area (#1171)
cd18595867dce6315e4871f488361b6a537a5f56 MGMT-3976: Embed ramdisk placeholder in template (#1150)
c00062d05d69b5b6bea0a8c7bcd83bf2ed195ee3 MGMT-3970 Make the iso editor scratch space base dir configurable (#1063)
0323832e6b0c01cfec4c81591e741fc3f34e40dc MGMT-3999 minimal-iso proxy - capital env vars (#1090)
8b0440080f861215eacc9859839ebf027d43184d MGMT-3999 http proxy support for minimal-iso (#1075)
c87bce8fa6accb12b92893721c471d1d416bbd30 Upgrade golintci (#1077)
60f45dc3e2d4b24570c200a7dba203f4396727f4 MGMT-3844 Limit concurrent minimal iso generations (#1032)
f2685fcc495f57022aa010f0e07eb8b7841c4799 MGMT-3510 Set static IP during boot in minimal iso (#986)
0d2e7091eecf74c61c2a4f82c416ad86796a68f9 NO-ISSUE Fix format issues found by gosec, update format-check (#950)
e68d4d3a4d91dca58247c966b068dd9e10469004 MGMT-2977 Cluster specific minimal iso (#932)
f0909a3c25cc7c81d37090366af6421bcbd00ba5 NO-ISSUE Move commands to hostcommands package (#948)
bb25cb3bdd6c386fec0346fa7eebcee1f79fe74a MGMT-2977 Remove coreos.liveiso kernel param for the template minimal iso (#930)
9458b2d03c0c472691a9dc1628fe9f6e59afda5c MGMT-2976 create and upload minimal iso template (#911)
d1f8895fc572725251375adc36e51eb8635a7f05 MGMT-2977 Enhancements to isoutil (#901)
5cbc89388fa6bb71fa3a4be4a72004939a045443 MGMT-3514 Add extract and create methods to the iso handler (#803)
d4023cce826797a96322e43ade4255f6f30b91b4 MGMT-3353 RHCOS per version (#869)
82b0d6d824f0d4a727fd054de84b2f9304ff11da MGMT-3297 - support static ips when rebooting nodes woth RHCOS image (#872)
bdcab0069f6c71f5eadc8706bbe03c617f755bc7 NO-ISSUE - make format target shouldn't format anything the linter doesn't check (#876)
4794165211f1721eb7ae27e471a4c3b7b54256bf MGMT-3456 - Will not attempt to format bootable disks that look like installation media (#862)
b23e32ab3695fdd735e6297670aa35615c451089 MGMT-2245 Extract OCP version from OCP images (#856)
7fb7f6ed800581ecb632d52ec4463395ecafe8a9 MGMT-3100 Upload/download PXE artifacts (#755)
c1696a87bb6363eb821414983f7fd7d52bed27bc Add setup script to share logic with prow (#6)
d30452bcb1a7be440adcc47f0289723220720e65 Remove github actions configuration (#4)
56e0862a4f742c53c1f382c8f48da552203b94f3 Change package and module references from carbonin to openshift (#3)
f3a8fb8ebfc594c2a7495aac2c546f464c878676 Merge pull request #2 from djzager/owners
b19d5a6481f6d98b1d7156e9014991419f59ac4a chore: add OWNERS and OWNERS_ALIASES files
b6be0e3c2ce16125fcca148bca63a953f455a9e1 Create github action for image build and tests
6f134fba60baf06c7c4ff13656ba20cd31e17f66 Remove the build directory
829a5accf65b9d21c31790846e548ec63452766e Update README
e27676e5f5ddf130e721ec48730dfc3ac468ce09 Replace standard library logger with logrus for json logging
78a4a5e42dff4157f7af3f0694ec98b2be613538 Add https support
0c1093dad4e3c44ca439aee499783c06d197bd7b Make port configurable
b97a61f5acc54b920c3c8b5a7882d8d383011034 Add tests for images handler
6d6b30818cf4836654ca6f4fb3c8ef961f274ed0 Make ImageStore an interface and add a mock
a8ac043b4a1774f20bad9d8ee12c8797f2653435 Base image downloaded on version query param
363196cad21a9af342080be74e84770b8a6433d7 Add metrics for the image handler
3e5013554d772084fef5545d0767ac71fbadbf71 Add basic go metrics
32aeec63e053769398dd6d037b3084af0da24482 Rename handler files
7efa5028a80ee8f7131fe6e7c4f63fbf3ee9efd6 Fix image override bug in imagestore and add tests
2ae06b2747f6b2034c791b0a3bda9531bd6b265f Move image request handling out of main.go
d1dd8a486717ed769c73e35e98b70bd9eff0d93e Add a health endpoint and handler
f5a2eced17e504d64aad0212b9e4cb508c912f15 Use built-in NotFound function
3d15d751beddc83dd05d0a6190fa13940cb79853 Move default versions into imagestore package
36df091f2af07b63443d282fdacb16351ab92a15 Add skipper support for running lint and eventually tests
02fe4857601040115c6602ac96e7aa200fa3ac85 Initial Commit
87143a11e740270c2193c90a60fb762918632f98 Initial commit
```

Status: Fast-forwarded successfully.
