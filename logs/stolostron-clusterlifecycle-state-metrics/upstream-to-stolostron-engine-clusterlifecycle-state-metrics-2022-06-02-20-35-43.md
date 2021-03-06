## Fast foarding of stolostron/clusterlifecycle-state-metrics into stolostron-engine/clusterlifecycle-state-metrics.

## Status Summary:

backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
a89dceafab0215c5570c0eb9fd54a47608561057 trigger build (#82)
a8467fa89b644e92ae996035b43b4e86b2b55a53 remote socket and core check (#77)
9bb09b7e857f26ea461ff6462f99fb8e1bbf5965 upgrade go modules (#75)
eae4cc47a0cb0c47f21489518b27808fe6f5bd7c no-op PR (#74)
6b8a0e2bf8a6b849adc64e285307f7eabfa5828a No-Op PR (#73)
2eb80f40dd329c89161483a542b3a1fc5625787a rename to stolostron (#68)
4f6555333c04bca21f0d1828a2be6c43105eac5a replace dynamic informer and client (#67)
4ec19963d9ba365b649fbd6a2109f58854625385 upgrade to go 1.17 (#65)
75091b17ec7331b15b3d30c654eeffaba77f6048 using informer to replace managedcluster and managedclusterinfo listwatch func (#62)
a39075627558c8e95c279c69db415b07d7a83b06 trigger build to fix package vulnerability (#61)
62333090b6ab6a29d83660eca484e1a69f6c824e fix install kubebuilder error (#58)
c5722cd5b64f5a65b4eab33c0a60922481515ac7 remove sensitive word (#57)
d4a4ee13597f49dd98c57f463e3d97881f5f065a upgrade release version to 2.4 (#55)
0635781078576b7a7a185370c1a1b60793425140 add xuezhaojun in owner and reviewer (#52)
8b7d7040bda657f67c704a6d1a7169ddc085730b update owners (#51)
e4cd4166331a5601589664d8ad6f2aceca23b35b Use annotations instead of clusterdeployment (#50)
e678eea4536e6ab128d2ae965737a6a7cb31ceb1 Add createdViaDiscovery (#49)
664bb8acf95bec13481c2b6043864905f52a266b Check for OCP 3 (#44)
75480012c8d54bc52ec93a53fdfd03afba001c7d Add condition on worker (#43)
f1e6c848af61fc7d2d448743b22aca2999a9e5cd Add condition on socket_worker (#41)
511d16aa4a28461ecf9764f9e05055ad9db8c26a Check node list length (#40)
71aeeec184226a666c79419482312ad4ae72a598 core and socket worker (#39)
49d18584412924ae7d20a31e5ae0e4321d093c8d Upgrade to go 1.16 (#38)
f86dbadddc0465abb5b54aa7e720f8c56ced3072 update base docker image (#35)
07942c53ec1374d132d398772ca148ff1d9b99a0 Add vcpu (#34)
5bf25bc9a8c8a3e6b629086cb4b74d59cb85a734 Merge pull request #33 from itdove/update
f4d709615953d45dde7b26c6dc53f6d6fed4a5b1 Add code of conduct
3466ebfaab79bc272b8c0835870bb72f7f7e4091 Add component_name/version (#32)
1273330000168502670cab32113c7406afdd5145 Update check-copyright (#31)
930638ea48d8baa2570dd07bc86a8817b7948c3a Add functional test (#28)
264fe65c2e975da95d095ba84006b7702f251a39 fake_push (#27)
85af3bfd113ae5e5b380acc399d1b841e94dcf57 Cleaning (#26)
be60cbb68fceb72cb3e33b5ee634247934b8e1d8 Merge pull request #25 from open-cluster-management/prow-experiment
1d36d864a013b32be38797a566b6374194a9ee6c Merge branch 'prow-experiment' of github.com:open-cluster-management/clusterlifecycle-state-metrics into prow-experiment
96a3f37977063286da34e5f042d69be23c3b509f add new line
5d9be9e2b093926b38f587275d563d2bf8eed9b0 Add copyright
f28d035f5a0a108aff012d6f4965477c3733e6db Add makefile.prow
e189bbf20282230243356da7d157004735b3e2df Merge pull request #23 from open-cluster-management/prow-experiment
99e8bc9d9928ba6ce69257b927d467fb2bfa4e0e Add dependencies
a85c21c5da94138a3b2ac6afe24399044547a2f0 Check if travis for harness
100c5d1d382942992f644fe775eeed74bfd68148 Merge pull request #22 from open-cluster-management/prow-experiment
665b3f6ae72381d84231f444eac9ebffce7610e2 Add harness
a22a90d8e25197c4a76ef4279d5baf32a4d0ffee Add coverage image
ac729f197d48545406c88ebbcb46df7f5d33ae16 Fix docketfile.prow
02213d06b06e94fa32bc07074861b2f35d6ddded Remove build-harness install
01dce62881ccee293b27276d3943ec0810e1e4c9 fix test, copyrigth-check, dockerfile
d3a64ec14df87ca4528b053c7a256a7cba9be5e4 add Dockerfile.prow
11de77924a976f6c9f63da09d6669bac449b198c Merge pull request #16 from open-cluster-management/leader_selection
1a222be01953f36f218e17cdb2657683508e958b Put leaderConfigMapName as constant
5b62b5964a28dd0ac4b195cb5a5d50e3980afe46 Setup logf for operator-sdk
bcc4bde9683332c3b2288f0492b691c1bac0b4d4 Move leader selection after telemetry
29aab20b4e6a10eb7aca46730bcc0942896ceb9b Remove exit 1
8009c2a2a5e330300170b25af03bd9e21b07bfb2 Add leader selection
2351a61830c036ee8d73289be79e97d48230d2cd Merge pull request #15 from open-cluster-management/fix_remove_vbh
551e638f3f7ee7e16b7068da4d367b9f5b7a67f4 copy coverage-entrypoint-func.sh locally
8025db4769a9b90e68a964517a329ef4a4d3597a delete harness
ddfd333fb25b2cea90b4b77bf6c41150ad846b03 Merge pull request #14 from open-cluster-management/Add-RELEASE_MAIN_BRANCH
4498651bc0b543c50f8e827448784f5435789a78 Remove vbh
b533f4bf8a67096abab771c33ea4a0c78a620d7e Fix !/bin/bash
52aef72d50e770fa98110924a7982278c47f8476 Merge pull request #13 from open-cluster-management/goto_public
63195eff1f34386e611380564c21e60058eb9b17 Merge pull request #12 from open-cluster-management/schmidtd-patch-1
60a328785afe78aeb9c4c2ca9ffae09011aae0dd Add copyright
18cfe303a60fe58e77b1c2ef45586d577b106662 Add files for public
074c6f0ba773946b89764dd9c1a2fa3c7013b307 Update release fast forward to 2.3 [skip ci]
694b965f97e914cf534c07f0d1a567ca54aa14ee Merge pull request #11 from open-cluster-management/Rename-cluster_id-to-managed_cluster_id
9aa5a3dbcfdf8c16c0812f578cd0cc5360047c6a Rename cluster_id to managed_cluster_id
c760b308a3522e86d9e7fcc4562549a8fa06e7ce Merge pull request #10 from open-cluster-management/args
7f0bf275923c3fd7936948b40635d289badc022d Set param with "--"
c73aa0844b0fdc52ce9a96a75876592a4cbea6b8 Clean logs
0b18c2dc458daf247c66c96f82aa19968d1e1454 Fix args when main
50a92b86dc4dcdb22a33420f6a202e28c4bcca20 Cleaning
8b3a22a9b1298872a5a0fe77b300e3fb9d83354f Fix passing parameters when testing
a35e0570a09fd5dcab27f5538cb39a1a71078731 Cleaning
8202a5564eeb01d17ee18ba7544e7617085534a2 Test with parameters
5f241a23d13166f983e275c9d4a20dea23e61362 upgrade to Go 1.15
6f7d5338d6557f172d35fb37194a348302dc6474 Add sleep
9982a12ff9feca4c1749aea224451de345cbece0 Add sleep
54806dca9465b1d338f13c4b8185160c16bebe0b Fix POD_NAME
baa2bd647756c5a15dfaf79daedcff7c4b38dba6 previous log
996dd35bd37a159ff2f03c59eb9f0097d773f6c9 Fix POD_NAME
be611c2c55825643eba9b1b5dd875e6d2f2f4c03 get previous logs
46650b70c321b2cb3ef3882beaaf91d096595808 Always show coverage
c1c261f17c937c6c928890f18c37b19b42779906 Delete pod
17cd4583bd00735fca44b77c24ddc7a406747b3f Add SIGTERM
6d679bc07ebbfa5903780af2423e778e8dfd80fa Add signal
d341942151fa34bc3adcda0b0b71c8f4eaf18e4f Add sleep
f0e6987a2acf3b4a109a1563ee50e06fd01e8558 add -v
96cd48694f9fd792f14f6aefd0f7b37e67c78d94 debug
be5b14594c05dc163c440f4701071e8a400da375 More debug
e283aeb3906c7a64b7a17de54229bd75afb78efe debug
25725d47bb14ee8fb3cea3c03c574a96c2d6b0e3 Merge pull request #8 from open-cluster-management/Fix-copyright-check.sh
5e2b9caf1bc42a665e9c259cdb3f4c191c58644b Fix the copyright-check.sh
92a045f37f1f7a4f013b550f324ad885ccb7861f Merge pull request #5 from open-cluster-management/vendorize
a3c252e7fbbc3b9c39e149f34c7ed60edd5c438a Merge pull request #7 from open-cluster-management/mentric_name_underscore
03cfd3d88054c26b4a7ed96fab84adc5cbac7fc0 Fix Copyright and add "_" in name
34711aa7fd830ccebe4f9bf872cf43de77651dfb Merge pull request #6 from open-cluster-management/new_name
96303cc598f243ebc6afa1dd976a01daeaa0596b Change metric name
672f10aa75c298221d34ae2303becd264e3350b9 Include all vbh files
bfafea59cccd5536658f09f3190d4b15a4190d95 set harness true
b803eb6aa6ff9814e51d90f29daa41e8a140dd18 vendorize default
20b0998d5bb2bca07ebf0ff10815f591a4de3d2a vendorize
7728635a3a7d06886ff49990f8e6a08b45a0cd3b Merge pull request #4 from open-cluster-management/update-doc
2490fd95433d02162dfabc51047f9dadfb41230c Add copyright, update readme.
065b11d79b998638577dc4aba1c3ca9764f62991 add release branch and publish image (#3)
0aa84f4f3264ec4799a22b08db6c3bcbc5002628 Merge pull request #1 from open-cluster-management/setup-travis
1ef831157d01dba4115e17e588e72eb10f98038d Simplify version searches
502bc52aaf382f2222407e4b394893821d016a68 Put OCP version when OCP
8bed57adf44be3edd0d91895bd354eeb463d004d REPLACE_IMAGE
02593e72cfe6f6c15f59aff8deb197140f0521ff Fix port and functional test ingress
36daa61d8d0be0ce7f2d7865bad4d5b3b5fc5ab4 readd ingress
33faa3ed7a6b712838c524305f6ef3baba059fd5 Run http and https concurrently
2c0289df06cdbc295f97af5014f636746c1a3319 Allow HTTP and HTTPS
1b9ef180711144fee1f755c8843f84d3f86fc2ec add name in cluster_id
134221ef2db7adb003d357de4ada5ee60fc54d62 Improve unit-est
5e6260c22f6093f97455f062cece6bd0176bddad Remove cluster name
53f2924f0c6c7c0d78c44675f40209b64a1df385 Fix code smell
98e054b17768d1bd9e5f159689e199aa62a56354 Merge into 1 metric
ca51abde0f3e8472e3e774ad660c83e8c1f95a92 Update sonar token
f63e56c45cf90664f56f0b461735be043f62d969 Rename project
29ae6b5c15844da3b4c505576c0ec5a50d9168fa fix non-Openshift
d887ea344a0150c044be16e622aa4c77114525fa Fix functional test/add hub_cluster_id
4a80c6c56c22e161048c9565af1b6d7df6662b6d Set service-monitoring
45c5f915918ef43088b8e70f1f05afae759b7281 debug coverage
1b7ba172aa2a68438c1f15ebb83ef367e70b660b Debug coverage
65bb86e35ee7c5fe2f9ebd0463ee68d78b1e764c Run funct test
4ece50df14f0cebbe09b282ace3cd5f3ad376324 Add func test
090e0726c442d57a5bffcbecc5fbe9f1a1918be0 Functional test
c5e1e45576a2275ebb948f891fd8e40996a2f376 fix role and create coverage image
783c2e40a996b4c2deec589327fb95b92e6d761a Use ManagedClusterInfo instead of managedCluster
a34cc59c762ed436a48922ab144eff2a8e8e9fd4 update gitignore
f4d55f68fb659f412b4281366b879f7d27b8844c Merge branch 'setup-travis' of github.com:open-cluster-management/ocm-state-metrics into setup-travis
8c4d8504046f3800485e04ebb065c38029dba4be Remove html file from sonar
e3646308099d9c556c55e23d69b6f23dd3fa0730 Remove html file from sonar
ab59f54b58cd62fdabbaafbc4cc9c0faf1cfb8ca Add unit test
0e378955ff5bbc9f873a50e32a053fa0eb64df51 Add service/ingress
5152e0dd241bbc024dd86363ce68b67a583ca671 Add TLS
53765de920939ccfa2b8b8ed215e9b17c6b4f1c6 Remove vulnarabity
f771384685b08171c62e6d6a391db57f5a753ae3 Remove build coverage image
97b6c19841140bc5bdcce4440d8a9803fb77f9cd No resource to copy
f24f344fe48b1f032c36d5ba4bc26a815e71df51 non ignore cmdocm-state-metrics
efc5c8f0fdf44c1ae0fc7436626affbe6fa3e320 remove git config
1f7ae19e8cffbb7f191d21d8cf9e4f0a658bf37c Setup
806e8565e754e467a492e2094e293fa14e54972f add clusterID/Domain
f68d28432ab0e2efd295f29b9a0c4bf5cc02e6b6 Add metrics w/o clusterdeployment get
142d663efc057a2263eff6b60d93061a2c0283e5 add clusterdeployment
31de7fc7aaea2e58be27bd211691104725bc0705 Merge pull request #1 from itdove/managed_cluster
8977d83025a864054b885fa22a4d99960fa4f75e ignore ocm-state-metrics
74a072148fa936c049aaca02b2d1981848d0a498 Delete binary
6a20bddbe7e4a996975861e124f41079462a9cd1 Implement managed-cluster
50abd4660b2d61dd38255dbf458855c9781747f4 Add clusterdeploymen
07e907219de3b9dfe3aaf2daca1870165a195bf1 Fix panic
dfb9eabc46f18690f560ce32829092bd4d188c13 init
3adcdd94eb07c9f52e1711c2c8b89777261065ca Initial commit
```

Status: Fast-forwarded successfully.
