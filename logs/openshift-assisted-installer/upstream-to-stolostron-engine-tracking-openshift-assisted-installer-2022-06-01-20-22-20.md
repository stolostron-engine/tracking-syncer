## Fast foarding of openshift/assisted-installer into stolostron-engine/tracking-openshift-assisted-installer.

## Status Summary:

release-ocm-2.6 -> backplane-2.1: First run, created backplane-2.1.  
release-ocm-2.5 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-ocm-2.6 -> backplane-2.1:

New commits (first branch sync):

```
c3186dd175c8d0049559f529082e0b52e8a71c2f Bug 2055978: host fail to boot from installation disk in case of multiple active "Red Hat Enterprise Linux" boot entries (#477)
4b2e5c9319c59d46ee2572a0d8fc70cfda8ee318 MGMT-9379: Fix arguments to make sure that HighAvailabilityMode is (#475)
e4476f6509db93b4b6df5c9c84f0c6c6fa913e7d NO-ISSUE: Bump k8s.io/client-go from 0.24.0 to 0.24.1 (#473)
fd15074870de3fa5349f9b61990ec089044c7300 NO-ISSUE: Bump k8s.io/apimachinery from 0.24.0 to 0.24.1 (#471)
8dc907cd487911bee190a57fb54b808e3655e3d9 NO-ISSUE: update bluemonday/runc packages (#470)
5f9d39ddad54b8f9ec25c9f65f5cbc8df1b09ecc MGMT-10003: save-partlabel and save-partindex coreos-installer args are not honored because the partition is formatted previously (#469)
11ebaa3b8bfdea7a7e30a60d7f4ba0ae8e2b4b36 MGMT-9379: Disregard HA mode for worker. (#451)
8611c1526eef4d3e683c10aee4f5bfc09119aab5 NO-ISSUE: Bump github.com/hashicorp/go-version from 1.4.0 to 1.5.0 (#467)
15a51a71d145cc669d4fb09e623db118ad027dfe NO-ISSUE: Bump sigs.k8s.io/controller-runtime from 0.12.0 to 0.12.1 (#468)
07a0da543cd2d228c3c3f78331fbffed3e658471 MGMT-10085: Cleanup disk which is part of a raid and have lvm on it (#460)
9607331c1442ad193eb15a42ec37b6eef7f0f3b8 NO-ISSUE: Bump github.com/coreos/ignition/v2 from 2.13.0 to 2.14.0 (#466)
1650642189d4a043250524d856c18ce41db3ed80 NO-ISSUE: Bump github.com/operator-framework/operator-lifecycle-manager (#464)
0e4614d83181238a9a30213a4ba52b5fe3a6f144 NO-ISSUE: Bump sigs.k8s.io/controller-runtime from 0.11.2 to 0.12.0 (#465)
6ee549c2479397632b3346a04fb21e54bede40ab NO-ISSUE: Reverting removal of dependabot image bumps (#459)
425d490f945b97fa4ee8d4aa06daf7e1f2478695 MGMT-10348: backofflimit in assisted controller is set in a wrong place and does nothing (#461)
3e648bd587d5211a79c1cb1bbb052abd0061ed4e NO-ISSUE: Bump github.com/operator-framework/operator-lifecycle-manager (#458)
adf3cde3e24586c0aee15b8bd50aa2f795b64c80 NO-ISSUE: remove dependabot bumps of docker images (#457)
e9b24b7baaa6bded8a01997c7cf6b756546de99f NO-ISSUE: Bump k8s.io/client-go from 0.23.6 to 0.24.0 (#454)
7d55e77f98fbef77fcd2d32409f5ae18033c6c7f NO-ISSUE: Bump github.com/go-openapi/runtime from 0.24.0 to 0.24.1 (#455)
d67d2843d0e757ef5643e6c873b49e61ef83a0ea NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.3 to 0.24.0 (#450)
7d147053bbb3ceb9529a2ee4f5ade7756a3d09a7 MGMT-9244: Prevent assisted-agent from rebooting the node when managed by IPA (#448)
ac3dab3fc0bb1ba5c43740ee2082344e313ab521 NO-ISSUE: Skip preparation of controller files in dry mode (#447)
912c3b26e4f1425bd362b416c90a69e1a9822089 MGMT-10077: Use logrus.FieldLogger instead of *logrus.Logger (#445)
65eb548395e9a93077b3fb46f246ba70cec6bac3 NO-ISSUE: Bump k8s.io/client-go from 0.23.5 to 0.23.6 (#443)
a1e0661fa5d6239e8d38c7980434b0215d763df8 MGMT-7340: add labels to the v2 api (#440)
e6f6a130f37e9e07f8f598ad4600571d50ca7dfd MGMT-10017: Cluster get to Error when OLM operator failed on applying post manifests (#441)
55b500bf804cb462249b0795167bfabaa10dad56 AGENT-105: Add Dockerfiles for OCP release (#436)
98994b0877fca88035531e9764f4c893c16b682c MGMT-9985: Eliminate use of global variables in assisted-installer (#439)
c9c39a06fdcd172a26cd61590cb96bffa031c5b1 MGMT-9971: removing timeout from waiting for 2 master. (#438)
42395f75f225f5d48679e1237f19b5cb230dc333 MGMT-9898: In assisted installer, add timeout and retry when worker is waiting for 2 ready masters (#435)
bf8bd3065dd10c5a321d721595f4c5b47ad5b15c NO-ISSUE: bump assisted-service version (#431)
b388edddd237c801594b3e72d6587106b0724bda NO-ISSUE: Bump sigs.k8s.io/controller-runtime from 0.11.1 to 0.11.2 (#430)
2332b103a294c5c4bd1efd4b88eca635db907e9a NO-ISSUE: Bump github.com/onsi/gomega from 1.18.1 to 1.19.0 (#428)
24f20629bd00c0f559b29cfd22dbf047cd9882ff NO-ISSUE: Bump github.com/operator-framework/api from 0.13.0 to 0.14.0 (#419)
89ae514be1699f8b6f5d2e6d6d1ed4ce4e14c2ef MGMT-9709: Modify assisted installer, to use more efficient queries when accessing the assisted service (#427)
e61ab030443ffd639fe4e085fdfb81adf47be406 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.2 to 0.23.3 (#426)
82572e77f6a0812092298497ec394d226ada107a NO-ISSUE: Bump k8s.io/client-go from 0.23.4 to 0.23.5 (#425)
11626f9a25c5ff7a7511840ae039adf3ae385e1d MGMT-9358: update assisted-service to master (#423)
e0139985a09745440cfb7d90e14f7154922de9f0 MGMT-8248: Hot fix for ODF/OCS (#384)
8ae99826e85ed2fa0548c08279781481f87813e6 MGMT-9358: update containers golang version to 1.17 (#422)
bdb26ccfa9c2e04f4a11a31e7901ae0697072200 NO-ISSUE: Bump github.com/thoas/go-funk from 0.9.1 to 0.9.2 (#421)
6a4afdd477b1cc64e5a298c308c81c42d7dd1f13 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.1 to 0.23.2 (#420)
35b38fc12d63740bfdf6893d252ca05c5e573df6 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.0 to 0.23.1 (#418)
7bd69e3a877ff250b0af6c5811f57a91c16c9f98 NO-ISSUE: remove Jenkins job files (#417)
7276fa7f308d60c312fcc9d118310a7803507fb7 NO-ISSUE: Bump github.com/go-openapi/swag from 0.19.15 to 0.21.1 (#410)
d7449ec39ea58309110d12d6de56f5167b1e7949 NO-ISSUE: Fix jenkins build (#416)
b3b57c6d1ab1e3962c902dc72c2908111371840b Fixing dry-mode issues / regressions (#415)
c0a868f9bc00644dee925381fcb2a143d7444764 NO-ISSUE: Jenkins should only build images (#414)
ff32f3b420a4acadd81f0fd600b4441ff3e6ba1e NO-ISSUE: Fix error log printing the wrong error variable (#413)
577473b443d40707110c353254d0ec2a8b38ac49 MGMT-9188: Publish coverage report (#412)
b8b71db6da9c3129630f77a7def548d0a1742192 NO-ISSUE: Bump openshift/origin-cli from 4.9.0 to 4.11.0 (#408)
ca4881f0e3c32ab0c135722c98be599e17a093c9 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.21.1 to 0.21.2 (#409)
5738c25f8a91ba356f25487d8f0f937b00402488 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.22.0 to 0.23.0 (#411)
870f95d9ade88a863e5f23daf844a5ba28c0d581 NO-ISSUE: Update go-openapi/runtime and fix url building (#407)
981b8144a38bfb13e8307f406e125700a09fa91f NO-ISSUE: Bump github.com/operator-framework/api from 0.8.0 to 0.13.0 (#405)
7d593502b6f2419c63667442c2590ba32ec76c7b NO-ISSUE: Bump baremetal-operator to the same version as assiste-service (#404)
dc92fc190f75f5dc80c2becc2f8d7c37621125ff NO-ISSUE: Bump github.com/onsi/gomega from 1.18.0 to 1.18.1 (#401)
42c6035fc9d378ae1b988853d742e65804b1ccb1 NO-ISSUE: Bump github.com/onsi/gomega from 1.17.0 to 1.18.0 (#399)
5e8d6dbe8ffc79f30f4b1625ab3c2acdb9200207 MGMT-8321: try to clean disk even if there is no VG on it (#385)
b91297b8b6a5cf10dbdc702deff015670bb32d28 NO-ISSUE: Bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5 (#389)
cf9d1d8ddb756b18bd390286a4530c4e3f49e8f6 NO-ISSUE: Bump github.com/PuerkitoBio/rehttp from 1.0.0 to 1.1.0 (#391)
b63f18a6a8f89c42934c04bf606f2c7444f65555 NO-ISSUE: Bump github.com/golang/mock from 1.5.0 to 1.6.0 (#397)
b53ccbb26cc9523fd78d9b8775354088ecbd1d11 NO-ISSUE: Bump github.com/coreos/ignition/v2 from 2.10.1 to 2.13.0 (#396)
1e7f12df5d0248f0ee3575a0e0f1b42b216587e7 NO-ISSUE: Bump github.com/hashicorp/go-version from 1.3.0 to 1.4.0 (#395)
8ff88eb4b57d7dcaf5eb788f23d9e6dfc6726444 NO-ISSUE: Bump github.com/ReneKroon/ttlcache/v2 from 2.9.0 to 2.11.0 (#390)
15182e2897a7994dae2753d09fa4b96394b53f4a NO-ISSUE: Bump github.com/thoas/go-funk from 0.8.0 to 0.9.1 (#393)
b1c557f7242850614ccdb108bac074a1381c506e NO-ISSUE: Bump github.com/onsi/gomega from 1.16.0 to 1.17.0 (#392)
57958134fb3659bda1dd7b5d204e58264f585df3 NO-ISSUE: update assisted-service package (#387)
09ce4b22204f67650e7178da790d8cb80c7e5388 MGMT-8064: Improve performance of installer/controller dry mode in multi-node clusters (#386)
e3e0586daac9b07b93f5ca2d220ac0c458f441b3 MGMT-8781: Fix controller updating configuring status with stale data (#383)
2b5e964a1a39debf53516ebfc6e5c7572d4f9987 NO-ISSUE: fix owners list (#382)
c81363a7fada8d23cfbac86ecc0f97835f1fa043 MGMT-8330: Minimize number of inventory client retries in assisted-controller (#381)
a9511521229f9b0e471f7af1d7db59359cc4dd51 MGMT-8293: Adapt assisted installer to latest swagger changes (#380)
5002bcbf8dbb3c5f82bd49292b0b8910abc7e3af MGMT-8064: Dry mode multi-node cluster support (#379)
c0c3f72975e6a3412c7a36cfacc262ad82d01f01 NO-ISSUE - add eliorerz and celebdor to owners (#378)
2cdb77683a090f01787688023186112b5712d45b Latest triage issues fixes (#377)
f9faeaf11ec91e502e60fb5b920a5a6fb988c9f1 MGMT-7912: getmonitors operator cache should not return value on any (#375)
833806892be6e86187041177129fa6e421ef6046 MGMT-8064: Introduce dry run mode to the installer (#371)
78994c76f194dfd796b2fc92eb3fe71ccf5d3eb3 MGMT-7912: Controller: Add cache to the operators status API (#373)
a7cfe1dd666dc06c0a94a00c4cb8906dc87a3fb9 NO-ISSUE: add backofflimit 100 and imagePullPolicy: IfNotPresent to assisted controller (#372)
149411cf81ec722e7d9ccaae4f3e4f430cd034cd NO-ISSUE: Remove user yuvigold (#370)
e6d6c7b12e0bf92716c679ea51d1bb6d5cc5d4b2 Bug 2010183: LogURL field of the AgentClusterInstall is not filled upon failure (#368)
aa6c55f384f9db22aba361e55f1cc2a6b4778855 NO-ISSUE: Add omertuc to code-approvers (#367)
a6debecfbbca16190db482dbc7201321a0a131c8 Bug 2004633: cluster deployment failed on connection error (#366)
08f2d4886744dea25e2cc24d1b778e15d4ec84e9 NO-ISSUE: Add `replaces` entry in go.mod for `irifrance/gini` which has moved in GitHub (#365)
a4fc5e8e45b58b5fa901c39b612c26c30bb8490c NO-ISSUE: Add commit-message prefix NO-ISSUE to dependanbot (#364)
f88da83680f3059a65253b7c1635fb6f4e9b362b MGMT-4078: Validate console operator in parallel to CVO (#362)
04b57c509591edbc8ec1a7a708daa39186aae3e3 Bug 1966621: Do not use run-level label for assisted-installer namespace (#291)
be3b5fd419778b79b02cf064170ef76eb2b15c64 NO-ISSUE: Add lranjbar to OWNERS_ALIASES (#356)
b2d7e1e2d9c572f3285ac5a99f3e038c6c72da07 MGMT-7760: Switch to stream8 (#360)
6f4c2222f36983578bbbb57502c8e09e12600ef6 MGMT-7504: move assisted-installer/controller to use V2 APIs for communicating with assisted-service (#358)
f4397ab54f417fffb1fad1b2adc9b0022ca2e31f MGMT-7315: Support IP-based matching of nodes during installation (#359)
4f877837986b0d4dfe5d9228bfb8e9f7fb77c888 NO-ISSUE: upload controller logs with operator status before must-gather (#357)
dbbd369ef45d1520b9bdd7f69d5c565a0841f872 NO-ISSUE: Use -v for efibootmgr to get detailed output (#354)
3673218609bec42b6cf64e2d81152e2cb25ced91 MGMT-7750: get efi file according to cpu architecture (#351)
f2d2adee1b74965def7e5733c22c619d71740dc8 MGMT-7713: Worker won't get updated to 'Waiting for ignition' when installing with IPv6 (#350)
cc8d5bb07c39e58b851f2cb27fc884511d077b95 OCPBUGSM-33782: Fix the manifest parsing (#347)
e346bc34fd2b3fb8d6c2cf6c0bb2125a565a198d MGMT-7292: Wait for the OLM to be initilized before CR apply (#333)
bbbebdaf4fa79ff31f61d978b5a17a35cb28f27d MGMT-7635 Fix logs gathering on SNO when failing to complete bootstrapping (#346)
f663d719f2ed68a82037eee1f742b011b52e7d3d MGMT-7597: Remove ronniel1, razregev, and asalkeld from OWNERS (#345)
52a722deac5af824684a148de6be1753ae1e844c MGMT-7178: Assisted-installer should not reboot worker till 2 masters join (#343)
3f66cb7ca27bfbca4d2425a8943c9745fd181aee OCPBUGSM-31802: hosts that were moved to ready state in k8s, didn't send (#342)
4c04303fd097f1de236d9fbeb046b005cb746de4 NO-ISSUE: remove obsolete installation-timeout parameter (#341)
f3800cfa3d64ce6dcd6f7b73f0578bb99bfdaf7a MGMT-7450: Removing pull secret token from failure logs (#340)
99a632124fb2babb1557cf0f97b4af908a20f845 MGMT-7417: Change installer and installer controller to support infra-env for the host (#336)
424639f00850b7f634f889e71e5e3188bae1cc78 OCPBUGSM-32117: Adding ipv6 support to dns busy address workaroung (#339)
2403dad3795406f2c5d923af0894e07bc8b0bdc4 MGMT-7452: Remove token from assisted-installer-controller log (#338)
8c2351a016d7e66f712ed77642c7cf9770c726d2 MGMT-3817: asssited-controller should always send logs (#337)
5273a2c3a8c84e5e41493b59493f392b1b3ae931 MGMT-4893: quote must-gather-image env variable in controller manifest (#335)
e285f301ffdc0296659346d66f9013b388632132 OCPBUGSM-27526: Cluster deployment freeze on Finalizing stage forever on Cluster Version Operator (#334)
57c4c942d12416ae3821d7df72b3558137640d57 Bug 1981465: Assisted installer wait for ready master nodes on bootstrap kube-apiserver though the kube-apiserver moved to one of the masters (#327)
a1057b1ef1c39c60285d4277435d32068230613c MGMT-4893: Add Must-Gather reports when olm controllers fail (#329)
90c1e8da2c5cb49bfb96a9f9c3c9d8d5b875cbc5 OCPBUGSM-31942: Return error on failed status operator update (#332)
1f26de355ad0b0a97680af4deec8d703a4c309c6 MGMT-7149: Merge wait for operators (#331)
e87d07c3dd341a337c7a36ef3e388598a5f32dd8 NO-ISSUE: Log message before uploading logs to service (#330)
ec000b28cc7500505680891509b9f918bee30e35 MGMT-7210: Upgrade Go version to 1.16 (#325)
706bbf2b41afdf76cc4d0200cc63241b8b89456b Bug 1979009: Change log message about EFI support (#326)
ebf29ac5f07e40603f447410979314f3bdbbe85d MGMT-7201: Wrap PostInstallConfigs logs and pass the entire failure message to the service (#324)
a9051890d8a89d859c22038115c50569e7bee10f Bug 1979009: Change log message about EFI support (#323)
df41ab506fca705f62197b508869f3d6e998a903 NO-ISSUE: Adding sagidayan as a code reviewer (#322)
56359ed5b6f109c898682a80dc22941b490673d1 MGMT-6663: Update progress of operators only when there's a new progress (#298)
809c74cfaf4431738be5ce18d67fd57361fd89f3 OCPBUGSM-30066: Retry wait for operator in case it failed (#319)
3de759809c810b83d82f9a6745915415b275f922 Bug 1973314: Update the uefi boot entry use shimx64 (#313)
d2b75685b95a7c38025469a10feb497342e72d36 NO-ISSUE: fix OWNERS files to match group members roles (#315)
34d09a8fe7a7f892bf0bc26fac5410913481a0eb Bug 1951812: Remove label from AI namespace after cluster installation (#301)
a597be74245b4437ede8c88d0d54a82bc5ccb08a NO-ISSUE: Extend gitignore (#307)
814a407bcbdc631410e34043f1001e3cc17d7a7c OCPBUGSM-30942: ACM/ZTP with Wan emulation, SNO cluster installs do not show as installed although they are (#306)
eb8cabf9b2b240c95a3b7b7d5f574b9b64cdf57a NO-ISSUE: Add check commit script (#294)
f01c5b021c94f46d7db16a8eadacada635c42d00 NO-ISSUE Add mkowalski to OWNERS/code-reviewers (#302)
c33dca244d518127cd041a6081561278e91a1e95 Fix Jenkins collection of junit files (#297)
cba20108695c46e710969cc4a5952a23c06663f2 Set Jenkinsfile with CI variable set to true (#296)
fbf3924bb0bea606c5466109f0b5f23354dbd29e Publish unit-test junit (#295)
9a1e31a87f1c122871334e88fe155d92c4a046fe NO-ISSUE: Improve logging of apply manifest (#293)
5234e2ae49c1db5e1141b9a4086f958fe0c2180c NO-ISSUE: Fix lint error (#292)
78acd450b4f6ff5dbcaea32006ff7f52cb0a7786 MGMT-4668: Add support to create manifest in assisted-installer (#271)
43bc204dfcc93a5306435505b8a81073f574aa24 Refactor finalizing condition to be clearer (#290)
2f5e9775435597873f808f2498dcfc03f929afda NO-ISSUE Reduced controller UT execution time by lowering the wait interval during the tests (#289)
5425f5c765943245dffc20ff081c6ca7140b45d3 MGMT-6584 Add host progress stages while waiting for control plane (#288)
bc513cf9e7188afac3fbbc4d55e8228542347ee4 OCPBUGSM-29397 decrease waiting time in case of cluster was not found or not autorized (#287)
4f5ad6a52b0fa1bcacb19be70aaeedb09870dda0 NO-ISSUE - removing assisted-installer-controller-ocp as it is not used (#283)
c76ba93cdd5b3e6f2734a0e7b35ab32213e1021a NO-ISSUE Add flaper87 to the code-reviewers (#286)
2fa0a040c1107796340f7576081fd758d88d8fda MGMT-6283 Remove EFI partition mount (#285)
ecb87ddc55520da440d6dc6540ec8c9b48fc57e0 MGMT-3145 Reset CVO timeout in case of a change (#281)
c5c58c594badd91811edb7cd00c0de1b9e3a7ca9 Bump github.com/onsi/gomega from 1.11.0 to 1.12.0 (#282)
6e5da3e76422db0e4782b848ee8725f513eae330 MGMT-4992 - stop controller after 10 errors of 401/404. (#279)
6ed31fa6d80b1fda8835b610b2c156fe615f12f9 Bump github.com/onsi/ginkgo from 1.16.1 to 1.16.2 (#280)
f93777fe9f2ed39bfc3dbfea458907659ee3f8ea OCPBUGSM-26978 Hack to release .10 DNS IP (#273)
255bf418332f8b86d9c79b3ac3114abdd31a486a Bump github.com/operator-framework/operator-lifecycle-manager (#276)
ca4a1afd7910c879d2fcc4ad68a5762e9eb5d0e7 NO-ISSUE fixed misleading log line in GetFileContentFromIgnition (#275)
1bdbb14b8c612b50f0aede32205db67c4eb40e6e Bump github.com/coreos/ignition/v2 from 2.9.0 to 2.10.1 (#274)
4ec55d970e177111b769cb5997b1668cd96d374c Bump openshift/origin-cli from 4.7 to 4.9.0 (#220)
3671c5da272ffe59fbd945255924b51d825d17d5 NO-ISSUE Avoid misleading error log when verifying bootkube completed successfully (#269)
95c358cda62d1982a9739d01b9438c0f802595e2 Bump k8s.io/apimachinery from 0.20.5 to 0.21.0 (#260)
57c3c3727774d513d437959702a23309a75a6fef Reduced UTs execution time by lowering the wait interval during the tests   (#266)
33f683129cf75e17a6d50c155cb1d8f6b299ee6a OCPBUGSM-27762 Automatic boot order setting is done incorrectly when using by-path style device names (#265)
6dcdd88ae216a1f03474e827597c2f679630521d Bump github.com/go-openapi/runtime from 0.19.27 to 0.19.28 (#264)
4fd74b88fd520b0716b10090a46cbb005b729eb0 MGMT-5188 Deprecate UpdateClusterInstallProgress API (#263)
6e32470e2f9038a23f9cf4293fefffa909b06565 OCPBUGSM-27526 Sync operator status with the service (#262)
32186b711d4cf992cfb03dfe73b0790c2a4e91a0 Remove dead code (#261)
bcfa1cc5cd298b3d7dd2560a8e6570b0fba62b60 Bump k8s.io/api from 0.20.5 to 0.21.0 (#258)
d6fac197d43fa5e50729e6f18a71052e43e614bb Bump github.com/operator-framework/api from 0.7.1 to 0.8.0 (#259)
b14dc972cf8c7518cc46f488b8955cbd264e675d OCPBUGSM-27324 Some hosts may never publish Writing image to disk: 100% event (#256)
6f5a0da63b9ea2184bd5474db3ccdf6c4f6d3313 Bump github.com/onsi/ginkgo from 1.16.0 to 1.16.1 (#257)
a53fbc785dec5586eeecd413d2c639afe27c1238 NO-ISSUE Allow @pkliczewski's team to lgtm PRs (#255)
d07817125318c4a72412777fab95191d5248eb9a OCPBUGSM-27183: Update pending OLM operators in case of timeout (#253)
8e77257e2460e081fb6bc4d1345e2cbf28b382b9 Bump github.com/hashicorp/go-version from 1.2.1 to 1.3.0 (#254)
58a0d2c1b6506efd891d2eb1f9f303343be819d9 Bump github.com/onsi/ginkgo from 1.15.2 to 1.16.0 (#252)
749f7737317f407c97d6ff347c569aac71d224db MGMT-4865 - Resolve installation disk symlink before running coreos-installer (#250)
9b8926a0660d3e342ddeb5b45860d52f9d2696b5 Bump github.com/go-openapi/strfmt from 0.20.0 to 0.20.1 (#251)
39271d500fdb664bc2468fe08eb42952dca8a189 Bump k8s.io/api from 0.20.4 to 0.20.5 (#243)
2c6d16c961893ef91dc366df60b0156a36f12694 Bump k8s.io/apimachinery from 0.20.4 to 0.20.5 (#240)
ed06d7561d123bf173e2292f5f26b82388a2df4b NO-ISSUE Enhance unknown host logs (#249)
f7e42c5ff7fae3d7ec671bbcefe7f1ac35cf184b MGMT-4839 Reduce spam logs from ops.ExecCommand (#248)
9d56673c34159d0a0c7797c0560ab116d30c7996 NO-ISSUE fix typo of the work available (#247)
2806f5cc7c6064180a4f2168a2b0104a9ea259db Bump github.com/operator-framework/api from 0.7.0 to 0.7.1 (#246)
9c5698f078e07fd4d00b1f982228c0e600279640 MGMT-4402 Use efibootmgr to set boot order to boot from disk (#229)
5baba44bdcce51612a48451f833aaa1d853afb77 MGMT-4206 Bugfix Call UpdateClusterOperator for every CVO change and not only failure (#245)
7e488a4ed5bcce1faeb4380fe4f2fd04a0e2b06e Bump github.com/operator-framework/api from 0.6.1 to 0.7.0 (#244)
097c8f25a1a817fffd2ec56d261c7bd59e6869e3 Bump github.com/go-openapi/runtime from 0.19.26 to 0.19.27 (#241)
65337a4797b92b1f3f6fe8045dd00526fde51579 Bump github.com/onsi/ginkgo from 1.15.1 to 1.15.2 (#242)
9b21fb43cca684ff4de4c8ef9682e1c0f36133c0 Bump github.com/operator-framework/api from 0.5.3 to 0.6.1 (#238)
c107911c4756e4473405e893ee80f4a6b079ac4f MGMT-4479 Specify must-gather image (#233)
5c054c1637c300b5d57212649d9a0df1b6b858b2 Bump github.com/sirupsen/logrus from 1.8.0 to 1.8.1 (#239)
f41920300a736bfd534b92cf6e50247c8cf33d6b Bump sigs.k8s.io/controller-runtime from 0.8.2 to 0.8.3 (#236)
2b18948532a6ef3b7a3ede344b88fd97fbf88a8b NO-ISSUE Log assisted controller configuration (#235)
27a24a3c4add54d880f62f407ab95342475af0c2 Remove login to registry.svc.ci.openshift.org registry from Jenkinsfile (#237)
5811c662d65c54427bde8552988ed4d5ef2efe19 Bump github.com/thoas/go-funk from 0.7.0 to 0.8.0 (#234)
0645568814701c122bed3ad9a25c9bcdf30215ef Bump github.com/onsi/ginkgo from 1.15.0 to 1.15.1 (#232)
6a7173b1ee85c49a4a16cc303f5b6fe69523095e MGMT-3662 Add OLM operators monitoring (#214)
a606a6f1b58f6018ce0b9bb97ddee5c48dca8be0 Bump github.com/onsi/gomega from 1.10.5 to 1.11.0 (#231)
f5a6942538208fb3e902784b90c00b7a995849ff MGMT-3854 log progress report (#228)
005c4d630fe9fad1831484c6a179acaf41756f47 MGMT-4185 Add other minor and pre versions to tests (#226)
7e1342ec81bb2e3d09e2b9c9378ea17cd22604e7 OWNERS: Add bugzilla component information (#225)
28ef7421ac58a22cf6469f3c235745e72ed19058 Bump github.com/sirupsen/logrus from 1.7.0 to 1.8.0 (#223)
da7ed27fcef94c0be5d259211d64ebdfa2aa9a79 Bump k8s.io/api from 0.20.2 to 0.20.4 (#224)
e43487afc7cb3cbf88f72e584fb0ac053f5c455d Bump github.com/golang/mock from 1.4.4 to 1.5.0 (#222)
f9a76f3ed2bd27a56a783dcf97033372640bef23 Bump k8s.io/apimachinery from 0.20.2 to 0.20.4 (#221)
b4974e7dc0d5d216fb96e58707fa9fbf9bb57890 MGMT-4179 Fix installer handling of ignitions to support multiple versions - sno mode (#218)
b38dc26154248fd50d882d39f293e8a7ca5abb83 MGMT-4179 Fix installer handling of ignitions to support multiple versions (#216)
37e48889a59192cfa465ff2b7a357f7334f8f7da NO-ISSUE Switch registry.svc.ci.openshift.org registry to public registry.ci.openshift.org (#215)
1e411eaf46c46b0ee49cf1f3de2c718ff0cd9183 MGMT-3860 Change use of certificates.k8s.io/v1beta1 to (#213)
b7272dfb8095eb3f9c9907f72a09b32518f5f310 MGMT-4078 Monitor console operator (#212)
b9d59c8c47997e1877d4727250a1aca47e417dcd Bump sigs.k8s.io/controller-runtime from 0.8.1 to 0.8.2 (#211)
8d1eda641591815333f5c9c149844167b1ac343b Bump github.com/onsi/gomega from 1.10.4 to 1.10.5 (#205)
d9d69ff4a299590bac47de6196d45ee751f6fe23 MGMT-3669 MGMT-3749 Update CVO status on change (#208)
2856aa4993f2ffc661ff8999f79dce921319e236 Update dependabot.yml (#209)
0f08980434743ff7c9cbb3378aafe27efd85dd25 Bump github.com/onsi/ginkgo from 1.14.2 to 1.15.0 (#204)
36e60242ec9b989da246acf7944f87ef1f3e77fb MGMT-3397 Do not apply 3->2->3 patch from Openshift 4.7 and later (#203)
f161d2a1b52f6c9e1e94944996c595905b6151e3 MGMT-3964 assisted-controller should wait for node to be ready in k8s before marking it as done (#206)
94f88585799ac3e4898157dca958f64f8184ce5e NOISSUE: Change Auth Token missing message (#207)
075b05e84dc694a56c3bb0023300f94b1082b2b4 Bump k8s.io/api from 0.19.4 to 0.20.2 (#182)
5724fd6c9033e7d2371a64886c27f55ea244b530 Igal/mgmt 3859 (#202)
29b0b435879a72a9ae41b24443a1e83875344e92 NO-ISSUE Add docker ignore (#201)
db9eb1f5d6bc26db21d2e77cda8d7b860d148c37 MGMT-3752 controller shall print cluster operators status before exiting and sending last logs (#200)
f0134628950c668ba8084aef109d01bc86e8a4a5 MGMT-3792 Move assisted-installer wait for joined master to look on hostname and not systemUUID (#197)
03564b1ffa8317fe478ef10de01eb05bfd99da67 NO-ISSUE: Work to get images built in prow  (#195)
5f4716bd86e1721fba97428609fb20cbe8c824ad NO-ISSUE Fixed error message (#199)
b847bd99ef75e0062c5ccfbc46f2d342363b7011 NO-ISSUE Use error.wrap instead of creating a new error (#198)
5ee4f162d4d4382234e977937050ac8718a316b7 NO-ISSUE Use error.wrap instead of creating a new error (#196)
69b670ce689596ccf9e5845838f3b42a9cfc25d4 MGMT-3573 Log assisted-controller events (#194)
ef13e7a544952cdc0b9ed0ecc90388b3b1b2e204 MGTM-3751 retry to send controller logs from installer and recheck controller state (#190)
faaf161772f54a39f52b031743b631e52e3d512b Add asalkeld to reviewers (#163)
a0642d55918bcecbd65d5523a61641a94d4aef50 Bump github.com/go-openapi/runtime from 0.19.24 to 0.19.26 (#193)
e93e11b72ad8ef9edab64d463f6b7091d55b2f3d Bump github.com/google/uuid from 1.1.5 to 1.2.0 (#191)
1f4b2ccb87ffbe853d5bbaa349bb1be305ef7746 Bump sigs.k8s.io/controller-runtime from 0.8.0 to 0.8.1 (#192)
5d21c2f4a686c039801d9cc6e417a907382f2142 MGMT-3491 - update service client due to swagger changes for additional OLM based services (#188)
ab5d12c8e63712f3cd8bdd144493cc0e2f1ae6c5 Revert "MGMT-3612 Assisted-insatller should start the patch.service in case of single node (#172)" (#187)
fee005ebfb6e56636902367870c9588da9957db9 MGMT-2485 Add hosts and status from service to log (#185)
b5eb270a6a3bb32fdc7bb26dfb1aba4e75bb5e06 MGMT-3692 Remove assisted-installer timeout while waiting for network type (#186)
6dd5ce197263d1bc476197a222506ac7c1d69e09 MGMT-2662 Handle the case when MetalProvisioning exists (#135)
486ff11d53db0af6ff3ca4c18e01bd9c27a4584a Revert Dockerfile changes for Prow  (#179)
5c66d0e672afb967615f6e9b9a8ad0450158cb01 Bump sigs.k8s.io/controller-runtime from 0.7.0 to 0.8.0 (#183)
a22e29667180e420eea3a11a3c3da7d69531996c Bump github.com/google/uuid from 1.1.4 to 1.1.5 (#184)
d88d8f08438cdd2eecb1fe21751c649292ff0f2f Bump github.com/go-openapi/strfmt from 0.19.11 to 0.20.0 (#181)
28a35c9b473dc315bdcad9196100b98e735a4117 Bump k8s.io/apimachinery from 0.20.1 to 0.20.2 (#180)
9ed5d7532fcbbc82baf5ebd800e9aee6b77e18cd Bugfix set controller deployment files on /assisted-installer-controller/deploy (#178)
c1c83b46a1ea21db7330321a7d3fb122ad0b1262 OCPBUGSM-22969 - fix panic due to a race between assisted-installer-controller and machineset controller (#174)
15b35460c26ba3f223bc4a5ea92769aebf10f6a2 NO-ISSUE Add openshift CI credentials to Jenkins (#177)
431431641810b8dded35e7085fb35c513a984564 NO-ISSUE: Work to get images built in prow (#169)
5fa8e960dac65e4d6aef986c2e523cede2527709 MGMT-3612 Assisted-insatller should start the patch.service in case of single node (#172)
87fec33f24b1a5294d7cb5dbe49f79b8a9382b43 MGMT-3431 pass CheckClusterVersion flag to controller (#168)
af07680badb3a6e4d1e42028b97cc3da02700c5a NO-ISSUE: Adding error to the logs message when waiting for network type. (#171)
8498e1c1eb229ac0cac0edb2802e56bb8ba4aeca Igal/mgmt 3580 (#170)
4e0f563356af7d608dd0359db3c4104c0265e568 NO-ISSUE: Updates to simplify openshift/release jobs (#167)
bcc0df2ba772f832bdd0185c8c70f846478d4d56 Bump github.com/coreos/ignition/v2 from 2.8.1 to 2.9.0 (#164)
09e277985ad6afef8a6173aa491218975da0641b Bump github.com/google/uuid from 1.1.1 to 1.1.4 (#165)
4b062b1691e92f0e2d6a72570d5b1c538cc3215e MGMT-2403 retry mechanism for oc must-gather logs (#162)
abcddbdefac17bce2887f758034833788ca1d78c MGMT-3519 Change control plane replicas patch to do the patch only when control plane replicas is 3 (#160)
1ba73c6e769561ef484ce4bcf632793954a9f58c Allow installing single node when hosts role is bootstrap (#161)
a9d24759db323c7f5845c35d2a7454e48493e18c MGMT-3297 - support static ips when rebooting nodes woth RHCOS image (#159)
9ff7bd99bba089f4b4b256dc4188b5cea0c9a4cd MGMT-3401 - collect oc log immediately on error (#157)
3193963c83bf98fe3f877058a97ee14643aa0a8e MGMT-3063 Add Env variable to enable/disable CVO wait  (#153)
060668f81b0c14eb89b3355d4f31d0f618de181d MGMT-2972 Update controller to support SNO (#158)
e4746613f8be5d6692c99e796a2e5127bcbb5dc3 MGMT-2971 Add single node installation flow to assisted-installer (#155)
89327c3df5eed10d5a9c25ae18491f349a54e481 MGMT-2970 Add high-availability-mode option to assisted installer (#154)
996ff36de45a6d3436acba096df864aa3e49c26b MGMT-3179 OVNKubernetes Patch for IPv6 (#133)
55924c9741e324aa13075abea5ac4fc11377faf2 MGMT-3062 Report cluster post-install progress (#144)
cd5f68a2fc91647a1d65c9d45b77e6722e854ef2 MGMT-3256 pvdisplay fails to run (#152)
90793522c0d18c34cf731789ff8001c9f08847b8 MGMT-2403 add rsync to agent's image (#151)
168090d9782ad602185f61245204140975c64a0d Bump k8s.io/apimachinery from 0.20.0 to 0.20.1 (#149)
ce9808c7404a4b0a6729711b5fda51ed1fbd87a3 MGMT-3298: enable MCD to use 'systemd start rpm-ostreed' while running as a container (#147)
c750c72a36730eb8758c0b7136ad0eda3d4aee16 Update README.md (#146)
c799e7db037bf52eba474fc92b777102e0f5f663 MGMT-2454 Only patch etcd for OpenShift < 4.7 (#115)
8a36dac584f7aeec89db4f4df68bd7c6d5c45308 MGMT-3262 Remove app-sre images (#143)
bd84577de049a6c2d431b279aadd88c573c915f0 Bump sigs.k8s.io/controller-runtime from 0.6.4 to 0.7.0 (#141)
b3140efe70689d521ec0575a3305ef12475a7359 Bump github.com/onsi/gomega from 1.10.3 to 1.10.4 (#138)
f3171a9901004cda1bd40aeb47d309648817612b Bump k8s.io/apimachinery from 0.19.4 to 0.20.0 (#139)
e3c999d9f16f8c8e9fa6d4105591da33ad84fc62 NO-ISSUE: Adding the error to logs when extracting ignition to disk. (#137)
a2904f9b3d4d3a13b02b4fed87b2fb4874eefd45 MGMT-1739 Remove MCO hardcoded hashmap (#136)
12bb20e3744860610ada6968a2ce59b6ba1f2a60 OCPBUGSM-21420 - fix race condition in day2 on ocp for controller check ignition pull (#134)
70e43bff1549bb2beebd492354367fd5452f88db Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#132)
4a7825c77c2393415a288f9528a607766e3b2a64 Bump sigs.k8s.io/controller-runtime from 0.6.2 to 0.6.4 (#131)
da60fec18ca5a0b881ee0f4a344750148a195de3 Bump github.com/coreos/ignition/v2 from 2.6.0 to 2.8.1 (#130)
e4a643f3f018652fda22d199b3761c10daf81327 Bump github.com/onsi/gomega from 1.10.2 to 1.10.3 (#129)
9dbc6508eb3e07c917e3c92ce14b5b9f7d2465ac Bump k8s.io/apimachinery from 0.19.2 to 0.19.4 (#106)
e165007b4890477ed217ece26e1d9ebec7d0366e Use quay.io/app-sre/golang for build container (#128)
b49b567137694fa7e8701eee5094ba1a209b45e9 Bump k8s.io/api from 0.19.2 to 0.19.4 (#103)
8ff67417a454747cb351065dd166c0b854f80b54 Bump github.com/onsi/ginkgo from 1.14.0 to 1.14.2 (#89)
2996498aeb9f0574a1b686dce02fddaaa383a580 MGMT-2403 search must-gather dir using utils (#127)
56b4760b61b64fb8b6e6512efc4f27909c12d290 MGMT-2403 Add must-gather logs (#117)
4a65179aed31f64cbca089ed8c7d5cd697849b77 MGMT-2779 Add --net=host to log sender command to enable it to communicate on top of IPv6 (#126)
6e72539b4cdbd8f11ee708c1d80ba95a06f8a793 MGMT-3088 push images to quay.io when we build from branch for installer & agent (#118)
d7086b4457e130c5503362df432de9d6f1c83cd0 MGMT-3112 Remove timeout on waiting for controller pod from assisted-… (#123)
40019622bedea289f0887d12ed7d419fe5af33c6 NO-ISSUE: Uploading logs before changing state to REBOOT. (#119)
9b543aac87b92550ace7caa2570ed08619d5bc02 Bump github.com/go-openapi/runtime from 0.19.20 to 0.19.24 (#124)
4031a6f25e48a8a800d193c32a08165aa2ef21e3 MGTM-3111 Increase waiting for controller pod timeout (#120)
a823d97146346db3a1f2659a6333f2edf5c2d44d MGMT-2411: fixed bad error format log (#116)
bd2cd1d044f26ec3a1421680fca909f23349377f MGMT-2403 Add must-gather logs - Part 1 (#108)
8a10924c77e86a3fdf281fc03b8e54999d1b2baa Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.11 (#113)
d14bbd458650a9588eec05dbecc11dc6dd6b1f61 MGMT-2465: added image_controller_ocp to all target (#112)
0ef1029522e1a9b1dfb0cc94cb1602dccd4d338d MGMT-2403 Add status flag to the post-reboot processes (#109)
31e4ddba131a57db53c9b056c71e78336f347d52 MGMT-2465: assisted-controller image for day2 (#96)
4eb057981c0ac4a2733b3a5a50059036eb70eb8c NO-ISSUE Add installer args to test cases (#100)
cfa6981d298fcfc934153eecc3c41c92753eb528 MGMT-2678: Adding bootstrap public SSH key to masters ignition. (#80)
1d3f470e514ab58948d46eb45f736cbf4914b55f NO-ISSUE: removed unused github workflows (#110)
c3f6b4d4d400070505a3cd787ca944968ce03089 MGMT-2573 Use the mco image passed from assisted-service (#99)
5444f0b9647da9999db1c72b936855cc5987e114 Update dependabot.yml (#107)
1edee71e6ae5baa250b52fc050b60d570a089c76 MGMT-2409: Added request id to each InventoryClient request (#102)
bf67ae8de3b37f83735fa26bb42bcb564cdf4748 MGMT-2272: set the consumerRef in the BMH object (#71)
0bd8e3bdc8e40147447b9578878be6681c8bc1be MGMT-2634 Remove host-name flag (#98)
5f21cd8ca7b332c6016e74cafe478318f9881eb0 MGMT-2694 Add additional args to coreos-installer command (#78)
68f1d891a2ec3d35864d718212d12f9bb8033b76 MGMT-2629 PullSecretToken marked secret (#94)
9e090803595b0040219a6f3d98a539252b199668 Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#88)
896afdba53590c8740f53bdeef7c85af2040d2ec Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.8 (#90)
c93a1be1504e75f39381e524502c785fb49dbdaa MGMT-2686 - add wipefs and pvremove -ff when preparing installation disk (#93)
327949f093e52cc92fa7d7129b936b5dab756d7c Very minor typo (#77)
903e9c19123d9525c0ebd955ee925cbe113e50fc Add label downstream-change-needed on Docker files (#84)
7c01a86e3adaf4a954657bc2c6f5529d3180154b Make errors from ExecCommand() less verbose by default (#79)
3022427c90e64f0db39b3d4c9fc4b081be74d785 NO-ISSUE add osherdp to OWNERS_ALIASES (#83)
583fbbc960171b2f4f9ce982b6ce75f8ab4f70ec NO-ISSUE update owners file (#82)
93495e81245278863102d155b15b4d0782641ff4 MGMT-2221 Replace master/worker ignition files with a separate one per host (#42)
afb52fcc1a82b37b8b8fa4e9cdc19459725c4bb9 MGMT-2767 Assisted-controller log of not found node is misleading (#81)
63431f832582b747f075a4936b3c29b6f73d4c5a MGMT-2661 Installation fails when hostnames contain capital letters (#76)
46535f1d0a6ab2913917d13c1078c762e5fa58a6 MGMT-2654 Disable wait for clusterversion operator availability (#75)
2b51e076ab0db989fa6253716a2e0606d9fd0b43 Don't assume docker in the makefile (#72)
1f34c80f256a32f26f1b9c663d3f551b302ce400 Bug 1890713 sending controller logs for the last 2 hours (#74)
3f652896725993d95ca3f0008ff78118d98061ab MGMT-2477 Send controller logs from installer before exit after contr… (#69)
220aa85dc6ae77c5d69d10b92a65fe1155028bac Create dependabot.yml (#67)
1290e31e3ed781169f33b7a110c1748471e5a5f9 MGMT-2456 Stop timing out installation, timeout logic should run only in the assisted-service (#68)
82db22b5641b7ee8d27a93fc899fdbf893c55109 MGMT-2461 Assisted-installer shoulld retry in case extracting ignition to FS failed due to rpm-ostree timeout (#66)
5fe984533152d28fb89789e6d1fb2ebc0f7bb711 OCPBUGSM-19280 Boot Strap Node fails to connect to API during proxy install (#65)
08a0ca837247d867a3fbb1953415e8f417754ed2 Igal/mgmt 2451 (#63)
eff1c86352abcaba1e202b7291c7fe87d6f19761 MGMT-2428: Onprem: configure controller with service ip etc/hosts (#61)
6f8dd246d5c83c2bd79aa8edc572f78628c7e40c MGMT-2417 waiting for controller pod to start running (#62)
08b39f023eff372ecc13e5638b14218e4965b426 Move proxy-func to utils (#44)
c0b2e67649fbaebcc2a3743a62c6981ea201956c MGMT-2385 continue to send logs till all routines finishes (#59)
5efd08414cb3785eb9186a026e886b0483cf3575 NO-JIRA add log for current cluster version status (#60)
798a12766882f67bc7596bdbeb44ba5a4fdb7232 OCPBUGSM-18103 waiting for cluster version to be available (#58)
a99a137329aa361ebad1a44920e771da578b44dc NO-JIRA return back approvers (#56)
39d85e1e8e611b45c9badbc58d2a895ebf0511e8 OCPBUGSM-18647 stop trying to update host status when all were updated already (#55)
bca2321f70402805bf7b85fc215bf22ca2fa5175 MGMT-1891 Configure CA certificate path for assisted installer controller (#46)
2447bc07095da892820010d0101d5d1ce8686edd MGMT-2349 Wrong retry request with invalid content length (#54)
1f4c9863f68c3d67cfa4a67c7da3e3e674ce8f00 Fix openshift_vresion.go spacing (#53)
2752ed5702260bfa1552e816e56f5147a25cf4c8 MGMT-1679 Call coreos-installer without image-url (#16)
cd473837303265b0bbec89c4852e29071abb6db5 MGMT-2291 Fix http res pointer dereference (#52)
8ab4c9b7130d8c3b3eb8860f0f4f6148bdfca1fe Use gotestsum tool for testing and publish junit on Jenkins (#51)
f7e76b4ce2aa9f60f88b7a2f26807777680cd519 Igal/controller logs (#50)
97e80c980d50754818d95e44dc748ec06c5c29b6 MGMT-2291 Retry invalid status codes (#49)
6eba2343329fdf983e1183987514f0f4aa0b22fd MGMT-2286 Continue on WaitAndUpdateNodesStatus error (#48)
b5f5a3eca8176ce29e996de1cd18ebb3d24ae88b Notify on abort (#41)
84035310be124f1014780516e257bfc30555d41b OCPBUGSM-17295 Implement Proxy function (#43)
dd267449bafe896c6c8432858e65ec6401a745d8 Rename SetEnvVars to SetProxyEnvVars (#39)
6e6230932797f60e24177773752a3059adae7b0c OCPBUGSM-17295 Set proxy env vars for controller (#38)
4d18213cb16e9ad2519acd3bfe8df70effe92215 OCPBUGSM-17431 update assisted-service client to support 503 and 401 403 for all apis (#37)
25aacd091e3a95cb15c49835cdee1466d3e1983a Update OWNERS file (#36)
546cf5001565e182435813bf23dc4b9eeb9a2b1c Accept proxy settings in install command (#35)
83d688d8220442eb8375b834375096100765ddc0 Fixed time.Duration lint failure (#34)
9f55020d9b713f2214d62e4c525dbeeeb0733dfe Fixed retry logging (#32)
57a288b482310846955c43011093b6ce99009fa8 MGMT-2116 Assisted-installer should retry assisted-service api calls in case of failure (#31)
726f8a0db1f118a17c1957be5062e08ea3ea69a7 Igal/MGMT-2145 Assisted-controller must not try to update already installed nodes or nodes in error (#30)
b9bd246847b4cc1142c301f39fb1eae94638fd46 MGMT-2112 Assisted-controller panics while waiting for it's routines to finish (#29)
95bc19200563acd59c28bee0b80924174ed17007 MGMT-1726 Assisted-controller namespace should be assisted-installer and not assisted-deployment (#28)
800610175080981aa67cb3a306bac0be667f8a89 MGMT-2140 Bootkube logs are not sent on successful installation (#27)
29308754372ece30c7dd2480ae0065a43bde1f92 typo (#25)
6d9bade681f879850764a1ad5a49227dfecb19ad MGMT-1626  -support v4.6 in assisted-installer (#12)
b5d602448c224ae6c86d19e09725a113e70c637f Removing hardcoded logssender image (#24)
8fe1050e3387361ffee74711d5d4fc774674f6eb Move installation timeout to be unsigned integer, Verify integer overflow (#21)
8311d156f36c1b292167018fec4ed118fc421cb7 Use IntVar for installation timeout (#19)
79faf4fdf818849d00f17b057e7dda26afcfde25 Add timeout to Jenkinsfile (#18)
07a9ccd577f92311045cd9f2d96d5fb5fd1c143c Update assisted-service go client to handle 401-403 (#17)
a57b8b2c9450e5721d1bc5b35e64fdec29edb52b Merge pull request #15 from openshift/osher/notification
87f71d2e43b3b5696a53019a68cfb08386b56b24 send slack notification
5b4d9174fd3ab6735e82553017276095d79bfb68 Merge pull request #14 from openshift/osher/jenkins_file_notification
fed28b2a47d949d9b869e6bc31670dfa17df740f chhange running agent to centos_worker
da97db8128de47aceb61271a1c38a007288e7fc5 add link to notification
ca7fd07d800a01555bf6c4dc645fbb0bd4455bab Igal/upload logs bootkube (#13)
35e9be297e2f75de92d4da1711ca6fc09829e07a MGMT-1881 Change journal tag in assisted-installer from assisted-installer to installer to match agent tags (#11)
ccbd55927d51dd9373efb0c411bc24b5926e6fb2 Add cacert to logs_sender run (#10)
c4e998f8be0e4b9e7f2d0b035d35c5787235c267 MGMT-1879 Add -insecure flag to logs_sender usage in assisted-installer (#9)
c72381dc79177558eb1eed7997bf368a77a51363 MGMT-1696 Fix propagation of HTTPS related configuration (#8)
313ae9fbf499c19898d4e1384d8c6d98403ae023 Lint fixes (#7)
60ef28fbc6fdcc7128f4c62538bedb783328a366 Igal/upload logs (#5)
8de7b457422eb09e48a92ce4c5de2f1a38ac7ec1 MGMT-1696 Support customizable HTTPS transport (#4)
52eda7a17e1fad442b342c94050a05b10ff1b93f Fix dependencies to point to new agent repo (#3)
0170928e4acff8e64972163a292b18df7e51690d MGMT-1714 Remove deprecated HOST and PORT parameters (#2)
b0eab81a8d061786fd63abc51021afc2053ca4e3 Renamed eranco74 to openshift
6b8b46ea95a1c50583a559f213d1a626f67e79dc Merge commit '785bf1c'
785bf1c396b8eee827311422a672844f252fd43d Merge pull request #1 from openshift/osher/git_action_replace
39653d771903bbbc12786f2789ebaad99fdd18fd PR fix
254a344f56bab4aab8da0c771289074decab6542 Added Jenkinsfile
8fc04746c5d0eff86e69c40997e69a520f79f390 Add OWNERS file (#95)
4791dac71030e8dd12a51bf06ec6dbf72cde02de MGMT-1433 Add Pull Secret token to Header on BM-Inventory API calls (#86)
9fb274534dce2b3d4113980218a3409fcfdd1d64 Fix build from fork (#93)
8099d13699cc5ca5706a22ba5d4bfd0c8d01e46e Fix build from fork (#93)
dc527ef83e2553a95b7f2fefa5f925f24ed0ef7c MGMT-1694 Fix unit test
c9832f90e82e273bd61641ed46570041afd791cc Fixed build git action avoid pushing PR images from a fork
7c97cf8e57a03d2a63c99d20831db074ac2b47ce MGMT-1694 Replace inventory host and port with URL (#91)
417b3f1041e42777bb8ef5c0c87e2ac05b6fec2e Avoid pushing PR images from a fork
b977a8079f489f9c6df216834d4b09869ed05c7d Added intalaltion timeout to config Updated UT
a35669b4b093f15d943dbacc41f9d2a7b5652e0d Updated docker version in the build container
b7657411b4552b46edd88c8c9fd47368bf7b3839 MGMT-1080 go mods
bb1ec0bdc30b7add37c22c2a4cf3d4d58e14de31 MGMT-1080 assisted-installer logs should go to journal
20f46fa4ba43297ba1528252818abaa8b628f6aa OCPBUGSM-11358 Cluster Events is missing the writing to disk progress logs Updated CoreosInstallerLogWriter regex to match the new coreos-installerr output coreos-installer version was updated from 0.1.2 to 0.2.0 [1861806] [Assisted-4.5]
6bd931176ac918fd4a47c7b942deba92ed9ea7fb Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane"
afb6b40271b9165592b69d88be75ed5167262a4e Revert "Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane""
a9c32acfa2af98d21b8c06021468c0dc21f1a122 Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane"
0f11212215a2bf5b469075a34140adc03e93e2af PR images should have 'PR_' prefix
24bbfc4b249e6258f1cccd7faa0d9b2158aeabee Added quay.expires-after label for PR images cleanup
765faa2abef9809b784043e6b51b3df760bd959f Publish image with hash tag for any build
ccc85243cf1b1d0f0127f7fc15256c097d37d07a MGMT-1455 - use only requested name to get the hostname of the inventory node (#82)
d0ffef742a26a46b16edf9a740dead140816663e MGMT-1481 autogenerated
abe12398dfbb11e138f0fd04e4a0884c3deabe81 MGMT-1481 test
ccf8fde0c6eb0587d169465d0c2434db0e69851f MGMT-1481 added waiting for console pod and running complete installation api
12d67716c31e932c36e878412d8f9d14394f6e4e MGMT-1483 Adding error message for write image to disk failure
f9596dfd86deb14e932d9e28c32f6dacd7524d21 Updated image to v4.5.1
782d6d3cbc257b27060731f4660d6a34df0cc8cf MGMT-1446 Assisted Installer Controller image set as config flag (#75)
ed8127bc4a11c6d535f9134703c881da5913e107 MGMT-1482 Writing image to disk might hangs although it's done Set the "waiting for control plane" stage only when the main thread actually wait for it. This change effect the hostInstallProgress order, now "waiting for contol plane" stage is set after "writing image to disk" is done Also removed HostStageFinishWaitingForControlPlane since it is no longer required
672e5eb0f534378f63b44d1a32b7db5e3b66868f MGMT-1394 autogenerated
2c89f7e2cc2ee16f8ebc3083eb69c4eed65553ea MGMT-1394 fixing tests
755ee4b99617ce47a9d420a0ca03ad44ec03b88b MGMT-1394 Change workers progress by adding wait-for-ignition status to assisted-installer and configuring to assisted controller
c9c293ed3b262e0c6c849f7f29ce4542dd53ff4a Making controller to start right after control plane is up
52ff1e6f28b703f6da73b85315e90777a50929e1 Changing default controller tag from stable to latest
09a2d9ccd99e272cc5f01ca987b22ae98d81d8be MGMT-1284 enhance install progress params (#66)
d1ca317d77a1a6d2166b801661bc9f5511b83960 Updated v4.5 image
0b359cd5235252b0abfb38a4e92a0ba4e3efcc19 Use models HostRole instead of hardcoded (#67)
5be92e69122b4344a955c948ac0c239a6627711f MGMT-1365 autogenerated
19ad60941d262eb415d6a4ebfd01b582d296573d MGMT-1365 fixing tests
502235ef8d9fac8afda9f0557cbfc1c3ee283786 MGMT-1365 adding set configuring state to assisted controller
dd944b41042672c6bfee2bc7ef4a0efb3ff0ddb0 Fixing circle depenpency issue by removing coreos_installer_log_writer from utils
3811de0d6691e597b312f81c803445237d380fc9 MGMT-1214 - use passed hostname to configure first ignition in installer, and pick a RequestedHostnme or inventory for node status monitoring in controller (#65)
162b693fc41398fec520999ead3b03d3cf328f80 Fix build image to work with new skipper version
19c7ccbf98b50d7d800416a4594e41914dd99e5e MGMT-1363 autogenerated
8a27615359bac72b2de5925fe469f105e19eecea MGMT-1363 Fix and add tests
9b2de2c364108336d80199c17854426308f38806 MGMT-1363 add configuring state
867414d64768c89d7aeb0148a8abd6cd75500aa7 MGMT-1330 autogenerated
c8f1f73b8bdc228db27fa3cf352ce1d7d044deec MGMT-1330 tests
ec96fc8c388808abedfdc1525938cbab1514a696 MGMT-1330 Add unpatch etcd after install is completed
4cf9c929d98625be03c259a4b9706693c750c23c MGMT-1274 index out of range panic fix in progressReporting
f847de9178ef6d3973045fb78c6c15459260b188 Updated UT
3931e7907189db3947b2af026ebb4e9eb5998049 Autogenerated
a1a9b60219fd4c5b7320d71a4e3d3798dd2c9619 MGMT-1102 Report host progress info for write image to disk. A new host status will be sent for every 5% increase in the write image to disk log output
e1a5778dc5f0284800d16c8632fa339f3a8926d4 MGMT-1213 - clear installation disk from PVs, VGs, LVMs (#61)
9afd7cdf8d1cfb32fe0385660097a4fb2ee6d391 MGMT-1167 check kubeboot status via file bootkube.done (#56)
f49c597a5c1e601fbc5424090b498111ee7c72d3 Remove unneeded file
743960db992f79691f1b0bd4c2604da533bc85b7 Added focus to makefile unit-test target
2836cec1e1e5779992d17a22313fb8beca654415 Fixed existing UT Added UT
22eebffdc7d59c14f48589d1640db35c4dafa027 Autogenerated mocks
3cd26ee90de51a733aa6aa81db0722975481c57b MGMT-1072 assisted-insaller logs looks bad ExecCommand now gets a Writer instead of verbose flag. The coreos installer function pass a writer that will buffer partial lines until it match the progress regex.
c663c60f7421b6ceee211a51693eb7da00e4cc5f Don't log 'Done writing image to disk' in case of failure
ed14ddb2341369ed3435777c4a87cc0f7290ca36 Added release.yaml to github workflow This workflow will build the repository container images upon git tag creation and publish it to ocpmetal registry with the matching tag
556205b8b62853609229b5aad47bdd7484c9f3d2 Push to master branch will build and push to with tag=latest
19bf629dbb6ef5750ba49999b77e478f28605acc MGMT-1141 - fix assisted-installer joined status reporting (#55)
2e3bfbea7631d2b8d4ddf5ed050fb6d29dcce947 MGMT-1135 - change assited-installer to correlate between bm-inventory uuid and kuberenetes uuid using hostname (#53)
0c76d88cd18ac9c87adbd9a8e4c3ffca96c73c1b MGMT-1089 autogenerated
b7bbd21a7df994a02e6041505b6403dddcf3ed6f MGMT-1089 Bootstrap should report masters joining progress
efd42ea028523ee96549980096161f10f6dbcfe3 Add Apache 2 License
63adf85c22c7a0dc7a3ec360c17fbc2825930c1c MGMT-1080 updated log file to /var/log/assisted-installer.log
e74723ea270d5aa6b08b47a3c26a1789f05cd09f MGMT-1081 autogenerated
d8899709ea6fe10544943eaf84fb18247ba5cd0c MGMT-1081 Can't download kubeconfig (no ingress ca was added) while cluster is installed but workers are not installed yet
3393d0b3bcfad7c39496a3486273363e5307769d MGMT-1004 Installation might fail while writing RHCoS to disk Added retry in case of failure
a29a376d013ba15ec346cf4417e5df0c139f3fa7 Adding unitest for ingress upload
59849fdbd02af28f424db988e62768e11d11b9f3 Autogenerated files
684f6fa4781a6a6bb055f8579acba43cf968a9c9 Updating controller role to be able to get configmaps
53f14afe45fb4d76ec1bd2bee9d6b0e07449baf9 MGMT-910 adding upload ingress ca to bm-inventory
70c67c2ca7709905c6c5f920f27b3df99d075a77 MGMT-904 Remove unclear assisted-installer logs Pass verbose option to ops.ExecPrivilegeCommand
3eaba33f4ddb48d34bcfd7669e40503da5ebc82c Adding sleep to WaitAndUpdateNodesStatus loop. No need to run every mili
89b43e14aaa8394f0478c87509c1956c42002d32 Result of make generate
ce4343c93624e85a14d269aa7162f6c182b4a015 Fixed version of tools installation in the build container
7e09ddada25fed1f203d46017783d947170c1db7 Updating role resources for assisted-controller
e82d7b63fabbb9db03cd403d5705ec1e80d0e0dd Write ops.ExecCommand real time output to log instead of stdout
2d2da357efa73bb2fdacd507ab7b862125cc036c Adding image_controller build to make all
3e5a5fbf60c4806fbef74f78902c869594c95907 Change image of assisted-installer-controller to quay.io/ocpmetal/assisted-installer-controller:stable
bdf4b927150c87e195b8491a0404ef95b8bf57bd Adding unitest for approve crs flow
188299127ad933eab81a434f9293bc876b634084 autogenerated mocks for csr approver
0aa72d2581965db7cb23ace4f44756d4f6e59679 Adding api rules to controller role yaml for reading and approving csrs
dcda5185dbe59f71579bf2bb68c89763a695118e MGMT-781 Adding CSR approver go routine to controller
81b4e564f8a2656e7e57c56b9de48620af9b2b82 Renamed readyNodes to readyMasterNodes
7d0daa4ae25508686c2fbfe62525a39b31a85e33 MGMT-902 Patching etcd before we have 2 ready masters results in etcd failure Wait for ready master nodes
8e3c628fc2d4da1ffd5bea4122897df7ba72e136 Use the k8sClient logger
3508a87f4a105586011bfbe18156944ef1373a1e Extended waitForMaster timeout to 2 hours
92acd29692ba41168e83df80e1050f232552f435 Deleting addPolicy from install function
021a02dd1f74db690fe33351f21b31dfc3106449 Fixing issue with RunOCctlcommand
5fb9841ddb8a00dcd2c80ba6ee8466c08dae8934 Don't run generate during make all generated files should be commited to source control
e562225e3393866745f21b482003930f9eed2c61 MGMT-839 Adding deploy files for assisted-installer-controller
f66ffbb7eb8ccdaef9069770dd30192af0c0a8ac Updating unitests and mock after adding assisted-controller
3a885053c656a86bed35f4967d4bc9a3f17fa41b MGMT-839 Provide progress reporting of the installed master after pivoting from bootstrap : 	Adding assisted-installer-controller and its deployment
57a46dedcf51e4640c225731d0d505bd87af9893 MGMT-862 Bootstrap node should use local coredns as default nameserver Simulate the netwrok configuration the bootstrap node would get if it will reboot by reloading systemd files and restart NetworkManager service it will trigger the execution of "/etc/NetworkManager/dispatcher.d/30-local-dns-prepender" that will add localhost nameserver to resolve.conf
710506de9de46fe3284284fbc68fcd6f3a249c75 Added github revision as a label to the image and push image with the revision to quay.io
0ded85230aeb087070e529481705efe93b5f2f4e MGMT-855 Write coreos-install progress log in realtime
9fc62b09fd74fbed206fc0a94b574d2b35ad78e6 Merge pull request #24 from eranco74/eran/MGMT-841
16292c546fa4082a00da88eec9c2799cf93503f3 MGMT-841 Assisted installer should use kubeconfig-loopback
a4d85203dec734621dfd5537d117408b9b8a85dd Updated inventory client due to API changes
f032cf273ed20c3785bad32e3034320fb5dabcd4 Revert "Updated inventory client due to API changes"
8b716d305474a0d84a50a0a068cbd37a650c7d3c Updated inventory client due to API changes
c17e6153c963f866dd37833a3c5be8b1a7821642 Added support for OCP 4.5 Use the lateest 4.5 nightly MCO and the latest RHCoS image in under 4.5 public miror TODO: update these once v4.5 is official
92df2c363c60d73e05370620d009606c059b8c85 MGMT-814 Add failure reason to the host failed status
e3a680b358e19560f5ec5294f43b4796bd16e340 Updated host progress status
7aa6ff3405105d5c1e7e48d1a97c8e0bdd8f9ffa MGMT-765 Adding support for openshift version: 	1. Use the right RHCoS image for the installation per openshift version 	2. Use right mco image per openshift version
4856bd495adecb1a8b0fff65a0a35afd2dc9fb1f Merge pull request #20 from eranco74/eran/status
465e665ac1695269257ea9db0925eceeb3da654c Updated done and failed status string
93232cab2692bd65e5fbef4d9c2b4f785908b921 Fixed UT
9b4b94a7d4ee40166531da5397bd2e757b977b47 Merge pull request #17 from eranco74/eran/bootstrap_goroutine
c0f4251706a465ee974985058c677ae933d9c042 Run the bootstrap flow in a goroutine so that the bootstrap node will start the master install flow (write rhcos image to disk) while bootstrap flow isn't done pass a context with cancel to the bootstrap goroutine Cancel the context when installNode returns
0393fdda885b4ffa80db6564b7985eaba92bdc96 Increased the timeout for the linter
24ef68c4d740a2186a08ff9f0e8aecf1e51ccfa1 Changed github action to use python 3
1e7879da1b353c1c568a325871d8a4bedd413096 Added PatchEtcd to k8s_client Added oc client
1b3265761badfa3c0c4098b7097b5824a400bd2c Added progress reporting
0691d2a71d7ee058e4bed6d76dcaccd21e546c22 updated makefile lint should run after generate
a9ac06fe0c929b77d4ba4aa8cd55575ea2d097d8 MGMT-704 Use MCO official release image for extracting ignition to disk
68bbd745c87907b28171ad33d0336b133a5a3496 Run make format at the end of the generate target
da645b35a7adc73cd43dc3745deeafad86418d90 Updated RHCoS image to rhcos-4.4.3
6e73b682cf68a2109d056a14067de9a6e89d403a Fixed etcd patch, we don't have until command on the livecd
879f4b2ce56c125de4c91f9939afbbe07135c336 Renamed master and bootstrap to HostRole{Master/Bootstrap}
8643c0637c8e90cc342410463fec3d1aab47c658 Use k8s-client instead of kubectl Fixed lint issues
be2519d4dc0dd5c5736e59fd0e8b4ca1c438c823 Update go version to 1.14
67c9187f4afa7fc0a91266fe5bc4f3c16dac0e43 Added ut target to the makefile
4e4168156860335bc63fb0472804a161d92aeb5f Fixed all goimports errors
d0cf93504b5f481fcaa4f5876ed5d9459639e556 Add INSTALLER env to skipper.yaml
4cb8daac87b0cb9921bc070e368d08f2ab282fa5 MGMT-721 Use the bm-inventory client for getting the files from the service
d427eedb45bccd22e0c94e193ae877e955aba720 Wait one minute bdefore reboot instead of 5
edb51a3a15094ed82831403ee61c1555eb58494b MGMT-706 Wait for the etc patch to succeed This is required since the patch will fail in case the kube API is down which might happen during the bootstrap
3e680ce3faad9e2995ff576d2513fa085fd410a1 Run the github workflow for pull requests
d5acc02b15c599434bea5f5da504c809e557e846 Added unit-test to make all target
5d5b04e4c960b60fc9f736947243b9f8c31faf7c Changed image-push workflow branch to master
866f97bb057318f60acde820be9d5f96aaaf4744 Adding UT Added mock using go:generate
4f5cdea1fd69022bd01763694c265a17b86b115f Added image-push workflow to trigger automatic build and publish image for commits pushed to master
c793ec230e6266086050ce11a684e85673d03f8a Publish image to ocpmetal namespace
a1f87fe9508dc9b8177d2654b4e92618bc3dd89b Added installer source code and updated makefile Updated dockerfile to use the new installer code Added go.mod
9ea865dab65c5396d4452e1ed97231ab940ed8fa Adde skipper
35a69db7194a08fae0c3aed225be90d6654e5223 Update README.md
9f1e983df8cd6f3ab08df688b01568b28142eab0 Updated readme
b3bffe8e5d20fb1494face76e9b4a6b1a42841f0 Use a machine-config-operator without any code changes
b66623102e15f70d0fe3b88ca7e6d9b31f750d4c Assisted installer first commit Added the install_node.sh script Added dockerfile Added makefile
```

Status: Fast-forwarded successfully.

### Branch release-ocm-2.5 -> backplane-2.0:

New commits (first branch sync):

```
80926726c6c26c6b8ea57a9f5493db435122da56 MGMT-9971: removing timeout from waiting for 2 master. Moving back to the logic where timeout is decision is taken only by service (#446)
eebab07e0cddc2244dedd002cb14ad86b777ccbf Bug 2073998: Modify assisted installer, to use more efficient queries when accessing the assisted service (#437)
8ab82f37c03d48e755a4da38c208479facaa86ca MGMT-9885: bump assisted-service version (#432)
11626f9a25c5ff7a7511840ae039adf3ae385e1d MGMT-9358: update assisted-service to master (#423)
e0139985a09745440cfb7d90e14f7154922de9f0 MGMT-8248: Hot fix for ODF/OCS (#384)
8ae99826e85ed2fa0548c08279781481f87813e6 MGMT-9358: update containers golang version to 1.17 (#422)
bdb26ccfa9c2e04f4a11a31e7901ae0697072200 NO-ISSUE: Bump github.com/thoas/go-funk from 0.9.1 to 0.9.2 (#421)
6a4afdd477b1cc64e5a298c308c81c42d7dd1f13 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.1 to 0.23.2 (#420)
35b38fc12d63740bfdf6893d252ca05c5e573df6 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.23.0 to 0.23.1 (#418)
7bd69e3a877ff250b0af6c5811f57a91c16c9f98 NO-ISSUE: remove Jenkins job files (#417)
7276fa7f308d60c312fcc9d118310a7803507fb7 NO-ISSUE: Bump github.com/go-openapi/swag from 0.19.15 to 0.21.1 (#410)
d7449ec39ea58309110d12d6de56f5167b1e7949 NO-ISSUE: Fix jenkins build (#416)
b3b57c6d1ab1e3962c902dc72c2908111371840b Fixing dry-mode issues / regressions (#415)
c0a868f9bc00644dee925381fcb2a143d7444764 NO-ISSUE: Jenkins should only build images (#414)
ff32f3b420a4acadd81f0fd600b4441ff3e6ba1e NO-ISSUE: Fix error log printing the wrong error variable (#413)
577473b443d40707110c353254d0ec2a8b38ac49 MGMT-9188: Publish coverage report (#412)
b8b71db6da9c3129630f77a7def548d0a1742192 NO-ISSUE: Bump openshift/origin-cli from 4.9.0 to 4.11.0 (#408)
ca4881f0e3c32ab0c135722c98be599e17a093c9 NO-ISSUE: Bump github.com/go-openapi/strfmt from 0.21.1 to 0.21.2 (#409)
5738c25f8a91ba356f25487d8f0f937b00402488 NO-ISSUE: Bump github.com/go-openapi/runtime from 0.22.0 to 0.23.0 (#411)
870f95d9ade88a863e5f23daf844a5ba28c0d581 NO-ISSUE: Update go-openapi/runtime and fix url building (#407)
981b8144a38bfb13e8307f406e125700a09fa91f NO-ISSUE: Bump github.com/operator-framework/api from 0.8.0 to 0.13.0 (#405)
7d593502b6f2419c63667442c2590ba32ec76c7b NO-ISSUE: Bump baremetal-operator to the same version as assiste-service (#404)
dc92fc190f75f5dc80c2becc2f8d7c37621125ff NO-ISSUE: Bump github.com/onsi/gomega from 1.18.0 to 1.18.1 (#401)
42c6035fc9d378ae1b988853d742e65804b1ccb1 NO-ISSUE: Bump github.com/onsi/gomega from 1.17.0 to 1.18.0 (#399)
5e8d6dbe8ffc79f30f4b1625ab3c2acdb9200207 MGMT-8321: try to clean disk even if there is no VG on it (#385)
b91297b8b6a5cf10dbdc702deff015670bb32d28 NO-ISSUE: Bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5 (#389)
cf9d1d8ddb756b18bd390286a4530c4e3f49e8f6 NO-ISSUE: Bump github.com/PuerkitoBio/rehttp from 1.0.0 to 1.1.0 (#391)
b63f18a6a8f89c42934c04bf606f2c7444f65555 NO-ISSUE: Bump github.com/golang/mock from 1.5.0 to 1.6.0 (#397)
b53ccbb26cc9523fd78d9b8775354088ecbd1d11 NO-ISSUE: Bump github.com/coreos/ignition/v2 from 2.10.1 to 2.13.0 (#396)
1e7f12df5d0248f0ee3575a0e0f1b42b216587e7 NO-ISSUE: Bump github.com/hashicorp/go-version from 1.3.0 to 1.4.0 (#395)
8ff88eb4b57d7dcaf5eb788f23d9e6dfc6726444 NO-ISSUE: Bump github.com/ReneKroon/ttlcache/v2 from 2.9.0 to 2.11.0 (#390)
15182e2897a7994dae2753d09fa4b96394b53f4a NO-ISSUE: Bump github.com/thoas/go-funk from 0.8.0 to 0.9.1 (#393)
b1c557f7242850614ccdb108bac074a1381c506e NO-ISSUE: Bump github.com/onsi/gomega from 1.16.0 to 1.17.0 (#392)
57958134fb3659bda1dd7b5d204e58264f585df3 NO-ISSUE: update assisted-service package (#387)
09ce4b22204f67650e7178da790d8cb80c7e5388 MGMT-8064: Improve performance of installer/controller dry mode in multi-node clusters (#386)
e3e0586daac9b07b93f5ca2d220ac0c458f441b3 MGMT-8781: Fix controller updating configuring status with stale data (#383)
2b5e964a1a39debf53516ebfc6e5c7572d4f9987 NO-ISSUE: fix owners list (#382)
c81363a7fada8d23cfbac86ecc0f97835f1fa043 MGMT-8330: Minimize number of inventory client retries in assisted-controller (#381)
a9511521229f9b0e471f7af1d7db59359cc4dd51 MGMT-8293: Adapt assisted installer to latest swagger changes (#380)
5002bcbf8dbb3c5f82bd49292b0b8910abc7e3af MGMT-8064: Dry mode multi-node cluster support (#379)
c0c3f72975e6a3412c7a36cfacc262ad82d01f01 NO-ISSUE - add eliorerz and celebdor to owners (#378)
2cdb77683a090f01787688023186112b5712d45b Latest triage issues fixes (#377)
f9faeaf11ec91e502e60fb5b920a5a6fb988c9f1 MGMT-7912: getmonitors operator cache should not return value on any (#375)
833806892be6e86187041177129fa6e421ef6046 MGMT-8064: Introduce dry run mode to the installer (#371)
78994c76f194dfd796b2fc92eb3fe71ccf5d3eb3 MGMT-7912: Controller: Add cache to the operators status API (#373)
a7cfe1dd666dc06c0a94a00c4cb8906dc87a3fb9 NO-ISSUE: add backofflimit 100 and imagePullPolicy: IfNotPresent to assisted controller (#372)
149411cf81ec722e7d9ccaae4f3e4f430cd034cd NO-ISSUE: Remove user yuvigold (#370)
e6d6c7b12e0bf92716c679ea51d1bb6d5cc5d4b2 Bug 2010183: LogURL field of the AgentClusterInstall is not filled upon failure (#368)
aa6c55f384f9db22aba361e55f1cc2a6b4778855 NO-ISSUE: Add omertuc to code-approvers (#367)
a6debecfbbca16190db482dbc7201321a0a131c8 Bug 2004633: cluster deployment failed on connection error (#366)
08f2d4886744dea25e2cc24d1b778e15d4ec84e9 NO-ISSUE: Add `replaces` entry in go.mod for `irifrance/gini` which has moved in GitHub (#365)
a4fc5e8e45b58b5fa901c39b612c26c30bb8490c NO-ISSUE: Add commit-message prefix NO-ISSUE to dependanbot (#364)
f88da83680f3059a65253b7c1635fb6f4e9b362b MGMT-4078: Validate console operator in parallel to CVO (#362)
04b57c509591edbc8ec1a7a708daa39186aae3e3 Bug 1966621: Do not use run-level label for assisted-installer namespace (#291)
be3b5fd419778b79b02cf064170ef76eb2b15c64 NO-ISSUE: Add lranjbar to OWNERS_ALIASES (#356)
b2d7e1e2d9c572f3285ac5a99f3e038c6c72da07 MGMT-7760: Switch to stream8 (#360)
6f4c2222f36983578bbbb57502c8e09e12600ef6 MGMT-7504: move assisted-installer/controller to use V2 APIs for communicating with assisted-service (#358)
f4397ab54f417fffb1fad1b2adc9b0022ca2e31f MGMT-7315: Support IP-based matching of nodes during installation (#359)
4f877837986b0d4dfe5d9228bfb8e9f7fb77c888 NO-ISSUE: upload controller logs with operator status before must-gather (#357)
dbbd369ef45d1520b9bdd7f69d5c565a0841f872 NO-ISSUE: Use -v for efibootmgr to get detailed output (#354)
3673218609bec42b6cf64e2d81152e2cb25ced91 MGMT-7750: get efi file according to cpu architecture (#351)
f2d2adee1b74965def7e5733c22c619d71740dc8 MGMT-7713: Worker won't get updated to 'Waiting for ignition' when installing with IPv6 (#350)
cc8d5bb07c39e58b851f2cb27fc884511d077b95 OCPBUGSM-33782: Fix the manifest parsing (#347)
e346bc34fd2b3fb8d6c2cf6c0bb2125a565a198d MGMT-7292: Wait for the OLM to be initilized before CR apply (#333)
bbbebdaf4fa79ff31f61d978b5a17a35cb28f27d MGMT-7635 Fix logs gathering on SNO when failing to complete bootstrapping (#346)
f663d719f2ed68a82037eee1f742b011b52e7d3d MGMT-7597: Remove ronniel1, razregev, and asalkeld from OWNERS (#345)
52a722deac5af824684a148de6be1753ae1e844c MGMT-7178: Assisted-installer should not reboot worker till 2 masters join (#343)
3f66cb7ca27bfbca4d2425a8943c9745fd181aee OCPBUGSM-31802: hosts that were moved to ready state in k8s, didn't send (#342)
4c04303fd097f1de236d9fbeb046b005cb746de4 NO-ISSUE: remove obsolete installation-timeout parameter (#341)
f3800cfa3d64ce6dcd6f7b73f0578bb99bfdaf7a MGMT-7450: Removing pull secret token from failure logs (#340)
99a632124fb2babb1557cf0f97b4af908a20f845 MGMT-7417: Change installer and installer controller to support infra-env for the host (#336)
424639f00850b7f634f889e71e5e3188bae1cc78 OCPBUGSM-32117: Adding ipv6 support to dns busy address workaroung (#339)
2403dad3795406f2c5d923af0894e07bc8b0bdc4 MGMT-7452: Remove token from assisted-installer-controller log (#338)
8c2351a016d7e66f712ed77642c7cf9770c726d2 MGMT-3817: asssited-controller should always send logs (#337)
5273a2c3a8c84e5e41493b59493f392b1b3ae931 MGMT-4893: quote must-gather-image env variable in controller manifest (#335)
e285f301ffdc0296659346d66f9013b388632132 OCPBUGSM-27526: Cluster deployment freeze on Finalizing stage forever on Cluster Version Operator (#334)
57c4c942d12416ae3821d7df72b3558137640d57 Bug 1981465: Assisted installer wait for ready master nodes on bootstrap kube-apiserver though the kube-apiserver moved to one of the masters (#327)
a1057b1ef1c39c60285d4277435d32068230613c MGMT-4893: Add Must-Gather reports when olm controllers fail (#329)
90c1e8da2c5cb49bfb96a9f9c3c9d8d5b875cbc5 OCPBUGSM-31942: Return error on failed status operator update (#332)
1f26de355ad0b0a97680af4deec8d703a4c309c6 MGMT-7149: Merge wait for operators (#331)
e87d07c3dd341a337c7a36ef3e388598a5f32dd8 NO-ISSUE: Log message before uploading logs to service (#330)
ec000b28cc7500505680891509b9f918bee30e35 MGMT-7210: Upgrade Go version to 1.16 (#325)
706bbf2b41afdf76cc4d0200cc63241b8b89456b Bug 1979009: Change log message about EFI support (#326)
ebf29ac5f07e40603f447410979314f3bdbbe85d MGMT-7201: Wrap PostInstallConfigs logs and pass the entire failure message to the service (#324)
a9051890d8a89d859c22038115c50569e7bee10f Bug 1979009: Change log message about EFI support (#323)
df41ab506fca705f62197b508869f3d6e998a903 NO-ISSUE: Adding sagidayan as a code reviewer (#322)
56359ed5b6f109c898682a80dc22941b490673d1 MGMT-6663: Update progress of operators only when there's a new progress (#298)
809c74cfaf4431738be5ce18d67fd57361fd89f3 OCPBUGSM-30066: Retry wait for operator in case it failed (#319)
3de759809c810b83d82f9a6745915415b275f922 Bug 1973314: Update the uefi boot entry use shimx64 (#313)
d2b75685b95a7c38025469a10feb497342e72d36 NO-ISSUE: fix OWNERS files to match group members roles (#315)
34d09a8fe7a7f892bf0bc26fac5410913481a0eb Bug 1951812: Remove label from AI namespace after cluster installation (#301)
a597be74245b4437ede8c88d0d54a82bc5ccb08a NO-ISSUE: Extend gitignore (#307)
814a407bcbdc631410e34043f1001e3cc17d7a7c OCPBUGSM-30942: ACM/ZTP with Wan emulation, SNO cluster installs do not show as installed although they are (#306)
eb8cabf9b2b240c95a3b7b7d5f574b9b64cdf57a NO-ISSUE: Add check commit script (#294)
f01c5b021c94f46d7db16a8eadacada635c42d00 NO-ISSUE Add mkowalski to OWNERS/code-reviewers (#302)
c33dca244d518127cd041a6081561278e91a1e95 Fix Jenkins collection of junit files (#297)
cba20108695c46e710969cc4a5952a23c06663f2 Set Jenkinsfile with CI variable set to true (#296)
fbf3924bb0bea606c5466109f0b5f23354dbd29e Publish unit-test junit (#295)
9a1e31a87f1c122871334e88fe155d92c4a046fe NO-ISSUE: Improve logging of apply manifest (#293)
5234e2ae49c1db5e1141b9a4086f958fe0c2180c NO-ISSUE: Fix lint error (#292)
78acd450b4f6ff5dbcaea32006ff7f52cb0a7786 MGMT-4668: Add support to create manifest in assisted-installer (#271)
43bc204dfcc93a5306435505b8a81073f574aa24 Refactor finalizing condition to be clearer (#290)
2f5e9775435597873f808f2498dcfc03f929afda NO-ISSUE Reduced controller UT execution time by lowering the wait interval during the tests (#289)
5425f5c765943245dffc20ff081c6ca7140b45d3 MGMT-6584 Add host progress stages while waiting for control plane (#288)
bc513cf9e7188afac3fbbc4d55e8228542347ee4 OCPBUGSM-29397 decrease waiting time in case of cluster was not found or not autorized (#287)
4f5ad6a52b0fa1bcacb19be70aaeedb09870dda0 NO-ISSUE - removing assisted-installer-controller-ocp as it is not used (#283)
c76ba93cdd5b3e6f2734a0e7b35ab32213e1021a NO-ISSUE Add flaper87 to the code-reviewers (#286)
2fa0a040c1107796340f7576081fd758d88d8fda MGMT-6283 Remove EFI partition mount (#285)
ecb87ddc55520da440d6dc6540ec8c9b48fc57e0 MGMT-3145 Reset CVO timeout in case of a change (#281)
c5c58c594badd91811edb7cd00c0de1b9e3a7ca9 Bump github.com/onsi/gomega from 1.11.0 to 1.12.0 (#282)
6e5da3e76422db0e4782b848ee8725f513eae330 MGMT-4992 - stop controller after 10 errors of 401/404. (#279)
6ed31fa6d80b1fda8835b610b2c156fe615f12f9 Bump github.com/onsi/ginkgo from 1.16.1 to 1.16.2 (#280)
f93777fe9f2ed39bfc3dbfea458907659ee3f8ea OCPBUGSM-26978 Hack to release .10 DNS IP (#273)
255bf418332f8b86d9c79b3ac3114abdd31a486a Bump github.com/operator-framework/operator-lifecycle-manager (#276)
ca4a1afd7910c879d2fcc4ad68a5762e9eb5d0e7 NO-ISSUE fixed misleading log line in GetFileContentFromIgnition (#275)
1bdbb14b8c612b50f0aede32205db67c4eb40e6e Bump github.com/coreos/ignition/v2 from 2.9.0 to 2.10.1 (#274)
4ec55d970e177111b769cb5997b1668cd96d374c Bump openshift/origin-cli from 4.7 to 4.9.0 (#220)
3671c5da272ffe59fbd945255924b51d825d17d5 NO-ISSUE Avoid misleading error log when verifying bootkube completed successfully (#269)
95c358cda62d1982a9739d01b9438c0f802595e2 Bump k8s.io/apimachinery from 0.20.5 to 0.21.0 (#260)
57c3c3727774d513d437959702a23309a75a6fef Reduced UTs execution time by lowering the wait interval during the tests   (#266)
33f683129cf75e17a6d50c155cb1d8f6b299ee6a OCPBUGSM-27762 Automatic boot order setting is done incorrectly when using by-path style device names (#265)
6dcdd88ae216a1f03474e827597c2f679630521d Bump github.com/go-openapi/runtime from 0.19.27 to 0.19.28 (#264)
4fd74b88fd520b0716b10090a46cbb005b729eb0 MGMT-5188 Deprecate UpdateClusterInstallProgress API (#263)
6e32470e2f9038a23f9cf4293fefffa909b06565 OCPBUGSM-27526 Sync operator status with the service (#262)
32186b711d4cf992cfb03dfe73b0790c2a4e91a0 Remove dead code (#261)
bcfa1cc5cd298b3d7dd2560a8e6570b0fba62b60 Bump k8s.io/api from 0.20.5 to 0.21.0 (#258)
d6fac197d43fa5e50729e6f18a71052e43e614bb Bump github.com/operator-framework/api from 0.7.1 to 0.8.0 (#259)
b14dc972cf8c7518cc46f488b8955cbd264e675d OCPBUGSM-27324 Some hosts may never publish Writing image to disk: 100% event (#256)
6f5a0da63b9ea2184bd5474db3ccdf6c4f6d3313 Bump github.com/onsi/ginkgo from 1.16.0 to 1.16.1 (#257)
a53fbc785dec5586eeecd413d2c639afe27c1238 NO-ISSUE Allow @pkliczewski's team to lgtm PRs (#255)
d07817125318c4a72412777fab95191d5248eb9a OCPBUGSM-27183: Update pending OLM operators in case of timeout (#253)
8e77257e2460e081fb6bc4d1345e2cbf28b382b9 Bump github.com/hashicorp/go-version from 1.2.1 to 1.3.0 (#254)
58a0d2c1b6506efd891d2eb1f9f303343be819d9 Bump github.com/onsi/ginkgo from 1.15.2 to 1.16.0 (#252)
749f7737317f407c97d6ff347c569aac71d224db MGMT-4865 - Resolve installation disk symlink before running coreos-installer (#250)
9b8926a0660d3e342ddeb5b45860d52f9d2696b5 Bump github.com/go-openapi/strfmt from 0.20.0 to 0.20.1 (#251)
39271d500fdb664bc2468fe08eb42952dca8a189 Bump k8s.io/api from 0.20.4 to 0.20.5 (#243)
2c6d16c961893ef91dc366df60b0156a36f12694 Bump k8s.io/apimachinery from 0.20.4 to 0.20.5 (#240)
ed06d7561d123bf173e2292f5f26b82388a2df4b NO-ISSUE Enhance unknown host logs (#249)
f7e42c5ff7fae3d7ec671bbcefe7f1ac35cf184b MGMT-4839 Reduce spam logs from ops.ExecCommand (#248)
9d56673c34159d0a0c7797c0560ab116d30c7996 NO-ISSUE fix typo of the work available (#247)
2806f5cc7c6064180a4f2168a2b0104a9ea259db Bump github.com/operator-framework/api from 0.7.0 to 0.7.1 (#246)
9c5698f078e07fd4d00b1f982228c0e600279640 MGMT-4402 Use efibootmgr to set boot order to boot from disk (#229)
5baba44bdcce51612a48451f833aaa1d853afb77 MGMT-4206 Bugfix Call UpdateClusterOperator for every CVO change and not only failure (#245)
7e488a4ed5bcce1faeb4380fe4f2fd04a0e2b06e Bump github.com/operator-framework/api from 0.6.1 to 0.7.0 (#244)
097c8f25a1a817fffd2ec56d261c7bd59e6869e3 Bump github.com/go-openapi/runtime from 0.19.26 to 0.19.27 (#241)
65337a4797b92b1f3f6fe8045dd00526fde51579 Bump github.com/onsi/ginkgo from 1.15.1 to 1.15.2 (#242)
9b21fb43cca684ff4de4c8ef9682e1c0f36133c0 Bump github.com/operator-framework/api from 0.5.3 to 0.6.1 (#238)
c107911c4756e4473405e893ee80f4a6b079ac4f MGMT-4479 Specify must-gather image (#233)
5c054c1637c300b5d57212649d9a0df1b6b858b2 Bump github.com/sirupsen/logrus from 1.8.0 to 1.8.1 (#239)
f41920300a736bfd534b92cf6e50247c8cf33d6b Bump sigs.k8s.io/controller-runtime from 0.8.2 to 0.8.3 (#236)
2b18948532a6ef3b7a3ede344b88fd97fbf88a8b NO-ISSUE Log assisted controller configuration (#235)
27a24a3c4add54d880f62f407ab95342475af0c2 Remove login to registry.svc.ci.openshift.org registry from Jenkinsfile (#237)
5811c662d65c54427bde8552988ed4d5ef2efe19 Bump github.com/thoas/go-funk from 0.7.0 to 0.8.0 (#234)
0645568814701c122bed3ad9a25c9bcdf30215ef Bump github.com/onsi/ginkgo from 1.15.0 to 1.15.1 (#232)
6a7173b1ee85c49a4a16cc303f5b6fe69523095e MGMT-3662 Add OLM operators monitoring (#214)
a606a6f1b58f6018ce0b9bb97ddee5c48dca8be0 Bump github.com/onsi/gomega from 1.10.5 to 1.11.0 (#231)
f5a6942538208fb3e902784b90c00b7a995849ff MGMT-3854 log progress report (#228)
005c4d630fe9fad1831484c6a179acaf41756f47 MGMT-4185 Add other minor and pre versions to tests (#226)
7e1342ec81bb2e3d09e2b9c9378ea17cd22604e7 OWNERS: Add bugzilla component information (#225)
28ef7421ac58a22cf6469f3c235745e72ed19058 Bump github.com/sirupsen/logrus from 1.7.0 to 1.8.0 (#223)
da7ed27fcef94c0be5d259211d64ebdfa2aa9a79 Bump k8s.io/api from 0.20.2 to 0.20.4 (#224)
e43487afc7cb3cbf88f72e584fb0ac053f5c455d Bump github.com/golang/mock from 1.4.4 to 1.5.0 (#222)
f9a76f3ed2bd27a56a783dcf97033372640bef23 Bump k8s.io/apimachinery from 0.20.2 to 0.20.4 (#221)
b4974e7dc0d5d216fb96e58707fa9fbf9bb57890 MGMT-4179 Fix installer handling of ignitions to support multiple versions - sno mode (#218)
b38dc26154248fd50d882d39f293e8a7ca5abb83 MGMT-4179 Fix installer handling of ignitions to support multiple versions (#216)
37e48889a59192cfa465ff2b7a357f7334f8f7da NO-ISSUE Switch registry.svc.ci.openshift.org registry to public registry.ci.openshift.org (#215)
1e411eaf46c46b0ee49cf1f3de2c718ff0cd9183 MGMT-3860 Change use of certificates.k8s.io/v1beta1 to (#213)
b7272dfb8095eb3f9c9907f72a09b32518f5f310 MGMT-4078 Monitor console operator (#212)
b9d59c8c47997e1877d4727250a1aca47e417dcd Bump sigs.k8s.io/controller-runtime from 0.8.1 to 0.8.2 (#211)
8d1eda641591815333f5c9c149844167b1ac343b Bump github.com/onsi/gomega from 1.10.4 to 1.10.5 (#205)
d9d69ff4a299590bac47de6196d45ee751f6fe23 MGMT-3669 MGMT-3749 Update CVO status on change (#208)
2856aa4993f2ffc661ff8999f79dce921319e236 Update dependabot.yml (#209)
0f08980434743ff7c9cbb3378aafe27efd85dd25 Bump github.com/onsi/ginkgo from 1.14.2 to 1.15.0 (#204)
36e60242ec9b989da246acf7944f87ef1f3e77fb MGMT-3397 Do not apply 3->2->3 patch from Openshift 4.7 and later (#203)
f161d2a1b52f6c9e1e94944996c595905b6151e3 MGMT-3964 assisted-controller should wait for node to be ready in k8s before marking it as done (#206)
94f88585799ac3e4898157dca958f64f8184ce5e NOISSUE: Change Auth Token missing message (#207)
075b05e84dc694a56c3bb0023300f94b1082b2b4 Bump k8s.io/api from 0.19.4 to 0.20.2 (#182)
5724fd6c9033e7d2371a64886c27f55ea244b530 Igal/mgmt 3859 (#202)
29b0b435879a72a9ae41b24443a1e83875344e92 NO-ISSUE Add docker ignore (#201)
db9eb1f5d6bc26db21d2e77cda8d7b860d148c37 MGMT-3752 controller shall print cluster operators status before exiting and sending last logs (#200)
f0134628950c668ba8084aef109d01bc86e8a4a5 MGMT-3792 Move assisted-installer wait for joined master to look on hostname and not systemUUID (#197)
03564b1ffa8317fe478ef10de01eb05bfd99da67 NO-ISSUE: Work to get images built in prow  (#195)
5f4716bd86e1721fba97428609fb20cbe8c824ad NO-ISSUE Fixed error message (#199)
b847bd99ef75e0062c5ccfbc46f2d342363b7011 NO-ISSUE Use error.wrap instead of creating a new error (#198)
5ee4f162d4d4382234e977937050ac8718a316b7 NO-ISSUE Use error.wrap instead of creating a new error (#196)
69b670ce689596ccf9e5845838f3b42a9cfc25d4 MGMT-3573 Log assisted-controller events (#194)
ef13e7a544952cdc0b9ed0ecc90388b3b1b2e204 MGTM-3751 retry to send controller logs from installer and recheck controller state (#190)
faaf161772f54a39f52b031743b631e52e3d512b Add asalkeld to reviewers (#163)
a0642d55918bcecbd65d5523a61641a94d4aef50 Bump github.com/go-openapi/runtime from 0.19.24 to 0.19.26 (#193)
e93e11b72ad8ef9edab64d463f6b7091d55b2f3d Bump github.com/google/uuid from 1.1.5 to 1.2.0 (#191)
1f4b2ccb87ffbe853d5bbaa349bb1be305ef7746 Bump sigs.k8s.io/controller-runtime from 0.8.0 to 0.8.1 (#192)
5d21c2f4a686c039801d9cc6e417a907382f2142 MGMT-3491 - update service client due to swagger changes for additional OLM based services (#188)
ab5d12c8e63712f3cd8bdd144493cc0e2f1ae6c5 Revert "MGMT-3612 Assisted-insatller should start the patch.service in case of single node (#172)" (#187)
fee005ebfb6e56636902367870c9588da9957db9 MGMT-2485 Add hosts and status from service to log (#185)
b5eb270a6a3bb32fdc7bb26dfb1aba4e75bb5e06 MGMT-3692 Remove assisted-installer timeout while waiting for network type (#186)
6dd5ce197263d1bc476197a222506ac7c1d69e09 MGMT-2662 Handle the case when MetalProvisioning exists (#135)
486ff11d53db0af6ff3ca4c18e01bd9c27a4584a Revert Dockerfile changes for Prow  (#179)
5c66d0e672afb967615f6e9b9a8ad0450158cb01 Bump sigs.k8s.io/controller-runtime from 0.7.0 to 0.8.0 (#183)
a22e29667180e420eea3a11a3c3da7d69531996c Bump github.com/google/uuid from 1.1.4 to 1.1.5 (#184)
d88d8f08438cdd2eecb1fe21751c649292ff0f2f Bump github.com/go-openapi/strfmt from 0.19.11 to 0.20.0 (#181)
28a35c9b473dc315bdcad9196100b98e735a4117 Bump k8s.io/apimachinery from 0.20.1 to 0.20.2 (#180)
9ed5d7532fcbbc82baf5ebd800e9aee6b77e18cd Bugfix set controller deployment files on /assisted-installer-controller/deploy (#178)
c1c83b46a1ea21db7330321a7d3fb122ad0b1262 OCPBUGSM-22969 - fix panic due to a race between assisted-installer-controller and machineset controller (#174)
15b35460c26ba3f223bc4a5ea92769aebf10f6a2 NO-ISSUE Add openshift CI credentials to Jenkins (#177)
431431641810b8dded35e7085fb35c513a984564 NO-ISSUE: Work to get images built in prow (#169)
5fa8e960dac65e4d6aef986c2e523cede2527709 MGMT-3612 Assisted-insatller should start the patch.service in case of single node (#172)
87fec33f24b1a5294d7cb5dbe49f79b8a9382b43 MGMT-3431 pass CheckClusterVersion flag to controller (#168)
af07680badb3a6e4d1e42028b97cc3da02700c5a NO-ISSUE: Adding error to the logs message when waiting for network type. (#171)
8498e1c1eb229ac0cac0edb2802e56bb8ba4aeca Igal/mgmt 3580 (#170)
4e0f563356af7d608dd0359db3c4104c0265e568 NO-ISSUE: Updates to simplify openshift/release jobs (#167)
bcc0df2ba772f832bdd0185c8c70f846478d4d56 Bump github.com/coreos/ignition/v2 from 2.8.1 to 2.9.0 (#164)
09e277985ad6afef8a6173aa491218975da0641b Bump github.com/google/uuid from 1.1.1 to 1.1.4 (#165)
4b062b1691e92f0e2d6a72570d5b1c538cc3215e MGMT-2403 retry mechanism for oc must-gather logs (#162)
abcddbdefac17bce2887f758034833788ca1d78c MGMT-3519 Change control plane replicas patch to do the patch only when control plane replicas is 3 (#160)
1ba73c6e769561ef484ce4bcf632793954a9f58c Allow installing single node when hosts role is bootstrap (#161)
a9d24759db323c7f5845c35d2a7454e48493e18c MGMT-3297 - support static ips when rebooting nodes woth RHCOS image (#159)
9ff7bd99bba089f4b4b256dc4188b5cea0c9a4cd MGMT-3401 - collect oc log immediately on error (#157)
3193963c83bf98fe3f877058a97ee14643aa0a8e MGMT-3063 Add Env variable to enable/disable CVO wait  (#153)
060668f81b0c14eb89b3355d4f31d0f618de181d MGMT-2972 Update controller to support SNO (#158)
e4746613f8be5d6692c99e796a2e5127bcbb5dc3 MGMT-2971 Add single node installation flow to assisted-installer (#155)
89327c3df5eed10d5a9c25ae18491f349a54e481 MGMT-2970 Add high-availability-mode option to assisted installer (#154)
996ff36de45a6d3436acba096df864aa3e49c26b MGMT-3179 OVNKubernetes Patch for IPv6 (#133)
55924c9741e324aa13075abea5ac4fc11377faf2 MGMT-3062 Report cluster post-install progress (#144)
cd5f68a2fc91647a1d65c9d45b77e6722e854ef2 MGMT-3256 pvdisplay fails to run (#152)
90793522c0d18c34cf731789ff8001c9f08847b8 MGMT-2403 add rsync to agent's image (#151)
168090d9782ad602185f61245204140975c64a0d Bump k8s.io/apimachinery from 0.20.0 to 0.20.1 (#149)
ce9808c7404a4b0a6729711b5fda51ed1fbd87a3 MGMT-3298: enable MCD to use 'systemd start rpm-ostreed' while running as a container (#147)
c750c72a36730eb8758c0b7136ad0eda3d4aee16 Update README.md (#146)
c799e7db037bf52eba474fc92b777102e0f5f663 MGMT-2454 Only patch etcd for OpenShift < 4.7 (#115)
8a36dac584f7aeec89db4f4df68bd7c6d5c45308 MGMT-3262 Remove app-sre images (#143)
bd84577de049a6c2d431b279aadd88c573c915f0 Bump sigs.k8s.io/controller-runtime from 0.6.4 to 0.7.0 (#141)
b3140efe70689d521ec0575a3305ef12475a7359 Bump github.com/onsi/gomega from 1.10.3 to 1.10.4 (#138)
f3171a9901004cda1bd40aeb47d309648817612b Bump k8s.io/apimachinery from 0.19.4 to 0.20.0 (#139)
e3c999d9f16f8c8e9fa6d4105591da33ad84fc62 NO-ISSUE: Adding the error to logs when extracting ignition to disk. (#137)
a2904f9b3d4d3a13b02b4fed87b2fb4874eefd45 MGMT-1739 Remove MCO hardcoded hashmap (#136)
12bb20e3744860610ada6968a2ce59b6ba1f2a60 OCPBUGSM-21420 - fix race condition in day2 on ocp for controller check ignition pull (#134)
70e43bff1549bb2beebd492354367fd5452f88db Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#132)
4a7825c77c2393415a288f9528a607766e3b2a64 Bump sigs.k8s.io/controller-runtime from 0.6.2 to 0.6.4 (#131)
da60fec18ca5a0b881ee0f4a344750148a195de3 Bump github.com/coreos/ignition/v2 from 2.6.0 to 2.8.1 (#130)
e4a643f3f018652fda22d199b3761c10daf81327 Bump github.com/onsi/gomega from 1.10.2 to 1.10.3 (#129)
9dbc6508eb3e07c917e3c92ce14b5b9f7d2465ac Bump k8s.io/apimachinery from 0.19.2 to 0.19.4 (#106)
e165007b4890477ed217ece26e1d9ebec7d0366e Use quay.io/app-sre/golang for build container (#128)
b49b567137694fa7e8701eee5094ba1a209b45e9 Bump k8s.io/api from 0.19.2 to 0.19.4 (#103)
8ff67417a454747cb351065dd166c0b854f80b54 Bump github.com/onsi/ginkgo from 1.14.0 to 1.14.2 (#89)
2996498aeb9f0574a1b686dce02fddaaa383a580 MGMT-2403 search must-gather dir using utils (#127)
56b4760b61b64fb8b6e6512efc4f27909c12d290 MGMT-2403 Add must-gather logs (#117)
4a65179aed31f64cbca089ed8c7d5cd697849b77 MGMT-2779 Add --net=host to log sender command to enable it to communicate on top of IPv6 (#126)
6e72539b4cdbd8f11ee708c1d80ba95a06f8a793 MGMT-3088 push images to quay.io when we build from branch for installer & agent (#118)
d7086b4457e130c5503362df432de9d6f1c83cd0 MGMT-3112 Remove timeout on waiting for controller pod from assisted-… (#123)
40019622bedea289f0887d12ed7d419fe5af33c6 NO-ISSUE: Uploading logs before changing state to REBOOT. (#119)
9b543aac87b92550ace7caa2570ed08619d5bc02 Bump github.com/go-openapi/runtime from 0.19.20 to 0.19.24 (#124)
4031a6f25e48a8a800d193c32a08165aa2ef21e3 MGTM-3111 Increase waiting for controller pod timeout (#120)
a823d97146346db3a1f2659a6333f2edf5c2d44d MGMT-2411: fixed bad error format log (#116)
bd2cd1d044f26ec3a1421680fca909f23349377f MGMT-2403 Add must-gather logs - Part 1 (#108)
8a10924c77e86a3fdf281fc03b8e54999d1b2baa Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.11 (#113)
d14bbd458650a9588eec05dbecc11dc6dd6b1f61 MGMT-2465: added image_controller_ocp to all target (#112)
0ef1029522e1a9b1dfb0cc94cb1602dccd4d338d MGMT-2403 Add status flag to the post-reboot processes (#109)
31e4ddba131a57db53c9b056c71e78336f347d52 MGMT-2465: assisted-controller image for day2 (#96)
4eb057981c0ac4a2733b3a5a50059036eb70eb8c NO-ISSUE Add installer args to test cases (#100)
cfa6981d298fcfc934153eecc3c41c92753eb528 MGMT-2678: Adding bootstrap public SSH key to masters ignition. (#80)
1d3f470e514ab58948d46eb45f736cbf4914b55f NO-ISSUE: removed unused github workflows (#110)
c3f6b4d4d400070505a3cd787ca944968ce03089 MGMT-2573 Use the mco image passed from assisted-service (#99)
5444f0b9647da9999db1c72b936855cc5987e114 Update dependabot.yml (#107)
1edee71e6ae5baa250b52fc050b60d570a089c76 MGMT-2409: Added request id to each InventoryClient request (#102)
bf67ae8de3b37f83735fa26bb42bcb564cdf4748 MGMT-2272: set the consumerRef in the BMH object (#71)
0bd8e3bdc8e40147447b9578878be6681c8bc1be MGMT-2634 Remove host-name flag (#98)
5f21cd8ca7b332c6016e74cafe478318f9881eb0 MGMT-2694 Add additional args to coreos-installer command (#78)
68f1d891a2ec3d35864d718212d12f9bb8033b76 MGMT-2629 PullSecretToken marked secret (#94)
9e090803595b0040219a6f3d98a539252b199668 Bump github.com/thoas/go-funk from 0.6.0 to 0.7.0 (#88)
896afdba53590c8740f53bdeef7c85af2040d2ec Bump github.com/go-openapi/strfmt from 0.19.5 to 0.19.8 (#90)
c93a1be1504e75f39381e524502c785fb49dbdaa MGMT-2686 - add wipefs and pvremove -ff when preparing installation disk (#93)
327949f093e52cc92fa7d7129b936b5dab756d7c Very minor typo (#77)
903e9c19123d9525c0ebd955ee925cbe113e50fc Add label downstream-change-needed on Docker files (#84)
7c01a86e3adaf4a954657bc2c6f5529d3180154b Make errors from ExecCommand() less verbose by default (#79)
3022427c90e64f0db39b3d4c9fc4b081be74d785 NO-ISSUE add osherdp to OWNERS_ALIASES (#83)
583fbbc960171b2f4f9ce982b6ce75f8ab4f70ec NO-ISSUE update owners file (#82)
93495e81245278863102d155b15b4d0782641ff4 MGMT-2221 Replace master/worker ignition files with a separate one per host (#42)
afb52fcc1a82b37b8b8fa4e9cdc19459725c4bb9 MGMT-2767 Assisted-controller log of not found node is misleading (#81)
63431f832582b747f075a4936b3c29b6f73d4c5a MGMT-2661 Installation fails when hostnames contain capital letters (#76)
46535f1d0a6ab2913917d13c1078c762e5fa58a6 MGMT-2654 Disable wait for clusterversion operator availability (#75)
2b51e076ab0db989fa6253716a2e0606d9fd0b43 Don't assume docker in the makefile (#72)
1f34c80f256a32f26f1b9c663d3f551b302ce400 Bug 1890713 sending controller logs for the last 2 hours (#74)
3f652896725993d95ca3f0008ff78118d98061ab MGMT-2477 Send controller logs from installer before exit after contr… (#69)
220aa85dc6ae77c5d69d10b92a65fe1155028bac Create dependabot.yml (#67)
1290e31e3ed781169f33b7a110c1748471e5a5f9 MGMT-2456 Stop timing out installation, timeout logic should run only in the assisted-service (#68)
82db22b5641b7ee8d27a93fc899fdbf893c55109 MGMT-2461 Assisted-installer shoulld retry in case extracting ignition to FS failed due to rpm-ostree timeout (#66)
5fe984533152d28fb89789e6d1fb2ebc0f7bb711 OCPBUGSM-19280 Boot Strap Node fails to connect to API during proxy install (#65)
08a0ca837247d867a3fbb1953415e8f417754ed2 Igal/mgmt 2451 (#63)
eff1c86352abcaba1e202b7291c7fe87d6f19761 MGMT-2428: Onprem: configure controller with service ip etc/hosts (#61)
6f8dd246d5c83c2bd79aa8edc572f78628c7e40c MGMT-2417 waiting for controller pod to start running (#62)
08b39f023eff372ecc13e5638b14218e4965b426 Move proxy-func to utils (#44)
c0b2e67649fbaebcc2a3743a62c6981ea201956c MGMT-2385 continue to send logs till all routines finishes (#59)
5efd08414cb3785eb9186a026e886b0483cf3575 NO-JIRA add log for current cluster version status (#60)
798a12766882f67bc7596bdbeb44ba5a4fdb7232 OCPBUGSM-18103 waiting for cluster version to be available (#58)
a99a137329aa361ebad1a44920e771da578b44dc NO-JIRA return back approvers (#56)
39d85e1e8e611b45c9badbc58d2a895ebf0511e8 OCPBUGSM-18647 stop trying to update host status when all were updated already (#55)
bca2321f70402805bf7b85fc215bf22ca2fa5175 MGMT-1891 Configure CA certificate path for assisted installer controller (#46)
2447bc07095da892820010d0101d5d1ce8686edd MGMT-2349 Wrong retry request with invalid content length (#54)
1f4c9863f68c3d67cfa4a67c7da3e3e674ce8f00 Fix openshift_vresion.go spacing (#53)
2752ed5702260bfa1552e816e56f5147a25cf4c8 MGMT-1679 Call coreos-installer without image-url (#16)
cd473837303265b0bbec89c4852e29071abb6db5 MGMT-2291 Fix http res pointer dereference (#52)
8ab4c9b7130d8c3b3eb8860f0f4f6148bdfca1fe Use gotestsum tool for testing and publish junit on Jenkins (#51)
f7e76b4ce2aa9f60f88b7a2f26807777680cd519 Igal/controller logs (#50)
97e80c980d50754818d95e44dc748ec06c5c29b6 MGMT-2291 Retry invalid status codes (#49)
6eba2343329fdf983e1183987514f0f4aa0b22fd MGMT-2286 Continue on WaitAndUpdateNodesStatus error (#48)
b5f5a3eca8176ce29e996de1cd18ebb3d24ae88b Notify on abort (#41)
84035310be124f1014780516e257bfc30555d41b OCPBUGSM-17295 Implement Proxy function (#43)
dd267449bafe896c6c8432858e65ec6401a745d8 Rename SetEnvVars to SetProxyEnvVars (#39)
6e6230932797f60e24177773752a3059adae7b0c OCPBUGSM-17295 Set proxy env vars for controller (#38)
4d18213cb16e9ad2519acd3bfe8df70effe92215 OCPBUGSM-17431 update assisted-service client to support 503 and 401 403 for all apis (#37)
25aacd091e3a95cb15c49835cdee1466d3e1983a Update OWNERS file (#36)
546cf5001565e182435813bf23dc4b9eeb9a2b1c Accept proxy settings in install command (#35)
83d688d8220442eb8375b834375096100765ddc0 Fixed time.Duration lint failure (#34)
9f55020d9b713f2214d62e4c525dbeeeb0733dfe Fixed retry logging (#32)
57a288b482310846955c43011093b6ce99009fa8 MGMT-2116 Assisted-installer should retry assisted-service api calls in case of failure (#31)
726f8a0db1f118a17c1957be5062e08ea3ea69a7 Igal/MGMT-2145 Assisted-controller must not try to update already installed nodes or nodes in error (#30)
b9bd246847b4cc1142c301f39fb1eae94638fd46 MGMT-2112 Assisted-controller panics while waiting for it's routines to finish (#29)
95bc19200563acd59c28bee0b80924174ed17007 MGMT-1726 Assisted-controller namespace should be assisted-installer and not assisted-deployment (#28)
800610175080981aa67cb3a306bac0be667f8a89 MGMT-2140 Bootkube logs are not sent on successful installation (#27)
29308754372ece30c7dd2480ae0065a43bde1f92 typo (#25)
6d9bade681f879850764a1ad5a49227dfecb19ad MGMT-1626  -support v4.6 in assisted-installer (#12)
b5d602448c224ae6c86d19e09725a113e70c637f Removing hardcoded logssender image (#24)
8fe1050e3387361ffee74711d5d4fc774674f6eb Move installation timeout to be unsigned integer, Verify integer overflow (#21)
8311d156f36c1b292167018fec4ed118fc421cb7 Use IntVar for installation timeout (#19)
79faf4fdf818849d00f17b057e7dda26afcfde25 Add timeout to Jenkinsfile (#18)
07a9ccd577f92311045cd9f2d96d5fb5fd1c143c Update assisted-service go client to handle 401-403 (#17)
a57b8b2c9450e5721d1bc5b35e64fdec29edb52b Merge pull request #15 from openshift/osher/notification
87f71d2e43b3b5696a53019a68cfb08386b56b24 send slack notification
5b4d9174fd3ab6735e82553017276095d79bfb68 Merge pull request #14 from openshift/osher/jenkins_file_notification
fed28b2a47d949d9b869e6bc31670dfa17df740f chhange running agent to centos_worker
da97db8128de47aceb61271a1c38a007288e7fc5 add link to notification
ca7fd07d800a01555bf6c4dc645fbb0bd4455bab Igal/upload logs bootkube (#13)
35e9be297e2f75de92d4da1711ca6fc09829e07a MGMT-1881 Change journal tag in assisted-installer from assisted-installer to installer to match agent tags (#11)
ccbd55927d51dd9373efb0c411bc24b5926e6fb2 Add cacert to logs_sender run (#10)
c4e998f8be0e4b9e7f2d0b035d35c5787235c267 MGMT-1879 Add -insecure flag to logs_sender usage in assisted-installer (#9)
c72381dc79177558eb1eed7997bf368a77a51363 MGMT-1696 Fix propagation of HTTPS related configuration (#8)
313ae9fbf499c19898d4e1384d8c6d98403ae023 Lint fixes (#7)
60ef28fbc6fdcc7128f4c62538bedb783328a366 Igal/upload logs (#5)
8de7b457422eb09e48a92ce4c5de2f1a38ac7ec1 MGMT-1696 Support customizable HTTPS transport (#4)
52eda7a17e1fad442b342c94050a05b10ff1b93f Fix dependencies to point to new agent repo (#3)
0170928e4acff8e64972163a292b18df7e51690d MGMT-1714 Remove deprecated HOST and PORT parameters (#2)
b0eab81a8d061786fd63abc51021afc2053ca4e3 Renamed eranco74 to openshift
6b8b46ea95a1c50583a559f213d1a626f67e79dc Merge commit '785bf1c'
785bf1c396b8eee827311422a672844f252fd43d Merge pull request #1 from openshift/osher/git_action_replace
39653d771903bbbc12786f2789ebaad99fdd18fd PR fix
254a344f56bab4aab8da0c771289074decab6542 Added Jenkinsfile
8fc04746c5d0eff86e69c40997e69a520f79f390 Add OWNERS file (#95)
4791dac71030e8dd12a51bf06ec6dbf72cde02de MGMT-1433 Add Pull Secret token to Header on BM-Inventory API calls (#86)
9fb274534dce2b3d4113980218a3409fcfdd1d64 Fix build from fork (#93)
8099d13699cc5ca5706a22ba5d4bfd0c8d01e46e Fix build from fork (#93)
dc527ef83e2553a95b7f2fefa5f925f24ed0ef7c MGMT-1694 Fix unit test
c9832f90e82e273bd61641ed46570041afd791cc Fixed build git action avoid pushing PR images from a fork
7c97cf8e57a03d2a63c99d20831db074ac2b47ce MGMT-1694 Replace inventory host and port with URL (#91)
417b3f1041e42777bb8ef5c0c87e2ac05b6fec2e Avoid pushing PR images from a fork
b977a8079f489f9c6df216834d4b09869ed05c7d Added intalaltion timeout to config Updated UT
a35669b4b093f15d943dbacc41f9d2a7b5652e0d Updated docker version in the build container
b7657411b4552b46edd88c8c9fd47368bf7b3839 MGMT-1080 go mods
bb1ec0bdc30b7add37c22c2a4cf3d4d58e14de31 MGMT-1080 assisted-installer logs should go to journal
20f46fa4ba43297ba1528252818abaa8b628f6aa OCPBUGSM-11358 Cluster Events is missing the writing to disk progress logs Updated CoreosInstallerLogWriter regex to match the new coreos-installerr output coreos-installer version was updated from 0.1.2 to 0.2.0 [1861806] [Assisted-4.5]
6bd931176ac918fd4a47c7b942deba92ed9ea7fb Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane"
afb6b40271b9165592b69d88be75ed5167262a4e Revert "Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane""
a9c32acfa2af98d21b8c06021468c0dc21f1a122 Updated bm-inventory client and use "HostStageWaitingForControlPlane" instead of "HostStageStartWaitingForControlPlane"
0f11212215a2bf5b469075a34140adc03e93e2af PR images should have 'PR_' prefix
24bbfc4b249e6258f1cccd7faa0d9b2158aeabee Added quay.expires-after label for PR images cleanup
765faa2abef9809b784043e6b51b3df760bd959f Publish image with hash tag for any build
ccc85243cf1b1d0f0127f7fc15256c097d37d07a MGMT-1455 - use only requested name to get the hostname of the inventory node (#82)
d0ffef742a26a46b16edf9a740dead140816663e MGMT-1481 autogenerated
abe12398dfbb11e138f0fd04e4a0884c3deabe81 MGMT-1481 test
ccf8fde0c6eb0587d169465d0c2434db0e69851f MGMT-1481 added waiting for console pod and running complete installation api
12d67716c31e932c36e878412d8f9d14394f6e4e MGMT-1483 Adding error message for write image to disk failure
f9596dfd86deb14e932d9e28c32f6dacd7524d21 Updated image to v4.5.1
782d6d3cbc257b27060731f4660d6a34df0cc8cf MGMT-1446 Assisted Installer Controller image set as config flag (#75)
ed8127bc4a11c6d535f9134703c881da5913e107 MGMT-1482 Writing image to disk might hangs although it's done Set the "waiting for control plane" stage only when the main thread actually wait for it. This change effect the hostInstallProgress order, now "waiting for contol plane" stage is set after "writing image to disk" is done Also removed HostStageFinishWaitingForControlPlane since it is no longer required
672e5eb0f534378f63b44d1a32b7db5e3b66868f MGMT-1394 autogenerated
2c89f7e2cc2ee16f8ebc3083eb69c4eed65553ea MGMT-1394 fixing tests
755ee4b99617ce47a9d420a0ca03ad44ec03b88b MGMT-1394 Change workers progress by adding wait-for-ignition status to assisted-installer and configuring to assisted controller
c9c293ed3b262e0c6c849f7f29ce4542dd53ff4a Making controller to start right after control plane is up
52ff1e6f28b703f6da73b85315e90777a50929e1 Changing default controller tag from stable to latest
09a2d9ccd99e272cc5f01ca987b22ae98d81d8be MGMT-1284 enhance install progress params (#66)
d1ca317d77a1a6d2166b801661bc9f5511b83960 Updated v4.5 image
0b359cd5235252b0abfb38a4e92a0ba4e3efcc19 Use models HostRole instead of hardcoded (#67)
5be92e69122b4344a955c948ac0c239a6627711f MGMT-1365 autogenerated
19ad60941d262eb415d6a4ebfd01b582d296573d MGMT-1365 fixing tests
502235ef8d9fac8afda9f0557cbfc1c3ee283786 MGMT-1365 adding set configuring state to assisted controller
dd944b41042672c6bfee2bc7ef4a0efb3ff0ddb0 Fixing circle depenpency issue by removing coreos_installer_log_writer from utils
3811de0d6691e597b312f81c803445237d380fc9 MGMT-1214 - use passed hostname to configure first ignition in installer, and pick a RequestedHostnme or inventory for node status monitoring in controller (#65)
162b693fc41398fec520999ead3b03d3cf328f80 Fix build image to work with new skipper version
19c7ccbf98b50d7d800416a4594e41914dd99e5e MGMT-1363 autogenerated
8a27615359bac72b2de5925fe469f105e19eecea MGMT-1363 Fix and add tests
9b2de2c364108336d80199c17854426308f38806 MGMT-1363 add configuring state
867414d64768c89d7aeb0148a8abd6cd75500aa7 MGMT-1330 autogenerated
c8f1f73b8bdc228db27fa3cf352ce1d7d044deec MGMT-1330 tests
ec96fc8c388808abedfdc1525938cbab1514a696 MGMT-1330 Add unpatch etcd after install is completed
4cf9c929d98625be03c259a4b9706693c750c23c MGMT-1274 index out of range panic fix in progressReporting
f847de9178ef6d3973045fb78c6c15459260b188 Updated UT
3931e7907189db3947b2af026ebb4e9eb5998049 Autogenerated
a1a9b60219fd4c5b7320d71a4e3d3798dd2c9619 MGMT-1102 Report host progress info for write image to disk. A new host status will be sent for every 5% increase in the write image to disk log output
e1a5778dc5f0284800d16c8632fa339f3a8926d4 MGMT-1213 - clear installation disk from PVs, VGs, LVMs (#61)
9afd7cdf8d1cfb32fe0385660097a4fb2ee6d391 MGMT-1167 check kubeboot status via file bootkube.done (#56)
f49c597a5c1e601fbc5424090b498111ee7c72d3 Remove unneeded file
743960db992f79691f1b0bd4c2604da533bc85b7 Added focus to makefile unit-test target
2836cec1e1e5779992d17a22313fb8beca654415 Fixed existing UT Added UT
22eebffdc7d59c14f48589d1640db35c4dafa027 Autogenerated mocks
3cd26ee90de51a733aa6aa81db0722975481c57b MGMT-1072 assisted-insaller logs looks bad ExecCommand now gets a Writer instead of verbose flag. The coreos installer function pass a writer that will buffer partial lines until it match the progress regex.
c663c60f7421b6ceee211a51693eb7da00e4cc5f Don't log 'Done writing image to disk' in case of failure
ed14ddb2341369ed3435777c4a87cc0f7290ca36 Added release.yaml to github workflow This workflow will build the repository container images upon git tag creation and publish it to ocpmetal registry with the matching tag
556205b8b62853609229b5aad47bdd7484c9f3d2 Push to master branch will build and push to with tag=latest
19bf629dbb6ef5750ba49999b77e478f28605acc MGMT-1141 - fix assisted-installer joined status reporting (#55)
2e3bfbea7631d2b8d4ddf5ed050fb6d29dcce947 MGMT-1135 - change assited-installer to correlate between bm-inventory uuid and kuberenetes uuid using hostname (#53)
0c76d88cd18ac9c87adbd9a8e4c3ffca96c73c1b MGMT-1089 autogenerated
b7bbd21a7df994a02e6041505b6403dddcf3ed6f MGMT-1089 Bootstrap should report masters joining progress
efd42ea028523ee96549980096161f10f6dbcfe3 Add Apache 2 License
63adf85c22c7a0dc7a3ec360c17fbc2825930c1c MGMT-1080 updated log file to /var/log/assisted-installer.log
e74723ea270d5aa6b08b47a3c26a1789f05cd09f MGMT-1081 autogenerated
d8899709ea6fe10544943eaf84fb18247ba5cd0c MGMT-1081 Can't download kubeconfig (no ingress ca was added) while cluster is installed but workers are not installed yet
3393d0b3bcfad7c39496a3486273363e5307769d MGMT-1004 Installation might fail while writing RHCoS to disk Added retry in case of failure
a29a376d013ba15ec346cf4417e5df0c139f3fa7 Adding unitest for ingress upload
59849fdbd02af28f424db988e62768e11d11b9f3 Autogenerated files
684f6fa4781a6a6bb055f8579acba43cf968a9c9 Updating controller role to be able to get configmaps
53f14afe45fb4d76ec1bd2bee9d6b0e07449baf9 MGMT-910 adding upload ingress ca to bm-inventory
70c67c2ca7709905c6c5f920f27b3df99d075a77 MGMT-904 Remove unclear assisted-installer logs Pass verbose option to ops.ExecPrivilegeCommand
3eaba33f4ddb48d34bcfd7669e40503da5ebc82c Adding sleep to WaitAndUpdateNodesStatus loop. No need to run every mili
89b43e14aaa8394f0478c87509c1956c42002d32 Result of make generate
ce4343c93624e85a14d269aa7162f6c182b4a015 Fixed version of tools installation in the build container
7e09ddada25fed1f203d46017783d947170c1db7 Updating role resources for assisted-controller
e82d7b63fabbb9db03cd403d5705ec1e80d0e0dd Write ops.ExecCommand real time output to log instead of stdout
2d2da357efa73bb2fdacd507ab7b862125cc036c Adding image_controller build to make all
3e5a5fbf60c4806fbef74f78902c869594c95907 Change image of assisted-installer-controller to quay.io/ocpmetal/assisted-installer-controller:stable
bdf4b927150c87e195b8491a0404ef95b8bf57bd Adding unitest for approve crs flow
188299127ad933eab81a434f9293bc876b634084 autogenerated mocks for csr approver
0aa72d2581965db7cb23ace4f44756d4f6e59679 Adding api rules to controller role yaml for reading and approving csrs
dcda5185dbe59f71579bf2bb68c89763a695118e MGMT-781 Adding CSR approver go routine to controller
81b4e564f8a2656e7e57c56b9de48620af9b2b82 Renamed readyNodes to readyMasterNodes
7d0daa4ae25508686c2fbfe62525a39b31a85e33 MGMT-902 Patching etcd before we have 2 ready masters results in etcd failure Wait for ready master nodes
8e3c628fc2d4da1ffd5bea4122897df7ba72e136 Use the k8sClient logger
3508a87f4a105586011bfbe18156944ef1373a1e Extended waitForMaster timeout to 2 hours
92acd29692ba41168e83df80e1050f232552f435 Deleting addPolicy from install function
021a02dd1f74db690fe33351f21b31dfc3106449 Fixing issue with RunOCctlcommand
5fb9841ddb8a00dcd2c80ba6ee8466c08dae8934 Don't run generate during make all generated files should be commited to source control
e562225e3393866745f21b482003930f9eed2c61 MGMT-839 Adding deploy files for assisted-installer-controller
f66ffbb7eb8ccdaef9069770dd30192af0c0a8ac Updating unitests and mock after adding assisted-controller
3a885053c656a86bed35f4967d4bc9a3f17fa41b MGMT-839 Provide progress reporting of the installed master after pivoting from bootstrap : 	Adding assisted-installer-controller and its deployment
57a46dedcf51e4640c225731d0d505bd87af9893 MGMT-862 Bootstrap node should use local coredns as default nameserver Simulate the netwrok configuration the bootstrap node would get if it will reboot by reloading systemd files and restart NetworkManager service it will trigger the execution of "/etc/NetworkManager/dispatcher.d/30-local-dns-prepender" that will add localhost nameserver to resolve.conf
710506de9de46fe3284284fbc68fcd6f3a249c75 Added github revision as a label to the image and push image with the revision to quay.io
0ded85230aeb087070e529481705efe93b5f2f4e MGMT-855 Write coreos-install progress log in realtime
9fc62b09fd74fbed206fc0a94b574d2b35ad78e6 Merge pull request #24 from eranco74/eran/MGMT-841
16292c546fa4082a00da88eec9c2799cf93503f3 MGMT-841 Assisted installer should use kubeconfig-loopback
a4d85203dec734621dfd5537d117408b9b8a85dd Updated inventory client due to API changes
f032cf273ed20c3785bad32e3034320fb5dabcd4 Revert "Updated inventory client due to API changes"
8b716d305474a0d84a50a0a068cbd37a650c7d3c Updated inventory client due to API changes
c17e6153c963f866dd37833a3c5be8b1a7821642 Added support for OCP 4.5 Use the lateest 4.5 nightly MCO and the latest RHCoS image in under 4.5 public miror TODO: update these once v4.5 is official
92df2c363c60d73e05370620d009606c059b8c85 MGMT-814 Add failure reason to the host failed status
e3a680b358e19560f5ec5294f43b4796bd16e340 Updated host progress status
7aa6ff3405105d5c1e7e48d1a97c8e0bdd8f9ffa MGMT-765 Adding support for openshift version: 	1. Use the right RHCoS image for the installation per openshift version 	2. Use right mco image per openshift version
4856bd495adecb1a8b0fff65a0a35afd2dc9fb1f Merge pull request #20 from eranco74/eran/status
465e665ac1695269257ea9db0925eceeb3da654c Updated done and failed status string
93232cab2692bd65e5fbef4d9c2b4f785908b921 Fixed UT
9b4b94a7d4ee40166531da5397bd2e757b977b47 Merge pull request #17 from eranco74/eran/bootstrap_goroutine
c0f4251706a465ee974985058c677ae933d9c042 Run the bootstrap flow in a goroutine so that the bootstrap node will start the master install flow (write rhcos image to disk) while bootstrap flow isn't done pass a context with cancel to the bootstrap goroutine Cancel the context when installNode returns
0393fdda885b4ffa80db6564b7985eaba92bdc96 Increased the timeout for the linter
24ef68c4d740a2186a08ff9f0e8aecf1e51ccfa1 Changed github action to use python 3
1e7879da1b353c1c568a325871d8a4bedd413096 Added PatchEtcd to k8s_client Added oc client
1b3265761badfa3c0c4098b7097b5824a400bd2c Added progress reporting
0691d2a71d7ee058e4bed6d76dcaccd21e546c22 updated makefile lint should run after generate
a9ac06fe0c929b77d4ba4aa8cd55575ea2d097d8 MGMT-704 Use MCO official release image for extracting ignition to disk
68bbd745c87907b28171ad33d0336b133a5a3496 Run make format at the end of the generate target
da645b35a7adc73cd43dc3745deeafad86418d90 Updated RHCoS image to rhcos-4.4.3
6e73b682cf68a2109d056a14067de9a6e89d403a Fixed etcd patch, we don't have until command on the livecd
879f4b2ce56c125de4c91f9939afbbe07135c336 Renamed master and bootstrap to HostRole{Master/Bootstrap}
8643c0637c8e90cc342410463fec3d1aab47c658 Use k8s-client instead of kubectl Fixed lint issues
be2519d4dc0dd5c5736e59fd0e8b4ca1c438c823 Update go version to 1.14
67c9187f4afa7fc0a91266fe5bc4f3c16dac0e43 Added ut target to the makefile
4e4168156860335bc63fb0472804a161d92aeb5f Fixed all goimports errors
d0cf93504b5f481fcaa4f5876ed5d9459639e556 Add INSTALLER env to skipper.yaml
4cb8daac87b0cb9921bc070e368d08f2ab282fa5 MGMT-721 Use the bm-inventory client for getting the files from the service
d427eedb45bccd22e0c94e193ae877e955aba720 Wait one minute bdefore reboot instead of 5
edb51a3a15094ed82831403ee61c1555eb58494b MGMT-706 Wait for the etc patch to succeed This is required since the patch will fail in case the kube API is down which might happen during the bootstrap
3e680ce3faad9e2995ff576d2513fa085fd410a1 Run the github workflow for pull requests
d5acc02b15c599434bea5f5da504c809e557e846 Added unit-test to make all target
5d5b04e4c960b60fc9f736947243b9f8c31faf7c Changed image-push workflow branch to master
866f97bb057318f60acde820be9d5f96aaaf4744 Adding UT Added mock using go:generate
4f5cdea1fd69022bd01763694c265a17b86b115f Added image-push workflow to trigger automatic build and publish image for commits pushed to master
c793ec230e6266086050ce11a684e85673d03f8a Publish image to ocpmetal namespace
a1f87fe9508dc9b8177d2654b4e92618bc3dd89b Added installer source code and updated makefile Updated dockerfile to use the new installer code Added go.mod
9ea865dab65c5396d4452e1ed97231ab940ed8fa Adde skipper
35a69db7194a08fae0c3aed225be90d6654e5223 Update README.md
9f1e983df8cd6f3ab08df688b01568b28142eab0 Updated readme
b3bffe8e5d20fb1494face76e9b4a6b1a42841f0 Use a machine-config-operator without any code changes
b66623102e15f70d0fe3b88ca7e6d9b31f750d4c Assisted installer first commit Added the install_node.sh script Added dockerfile Added makefile
```

Status: Fast-forwarded successfully.
