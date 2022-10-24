## Syncing stolostron/release with stolostron-engine/release

## Status Summary:

backplane-2.1 -> backplane-2.1: Picked up 2 new commits.  
backplane-2.0 -> backplane-2.0: Already in sync.  
master -> master: First run, created master.  

### Branch backplane-2.1 -> backplane-2.1:

New commits:

```
bf2be2a6c71b441136597ab0c980b3eb444c115c Add snapshot 2022-10-24-07-47-11 to backplane-2.1 2.1.2 [skip ci]
c435980ed32413509407ef27117a15893f595d87 Add snapshot 2022-10-24-07-47-11 for release 2.1.2 from backplane-pipeline quay-retag branch
```

Status: Syncing successful

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch master -> master:

New commits (first branch sync):

```
b85079b3cf1f841e28bb671a2770c2b10bbd6007 Removed 3 governance projects [skip ci]
2c4afa7238ecffc22d3572512e50863ea029880c Fix missing input bundle directory error when building community-op images (#409)
4c133326e12435177c06376ff6b5365d9b6d5ca6 Handle implications of having community operators with release numbers that differ from their related RH-released ones (#407)
e2ceab7b22698742e0816cf23e53706a733c9bf7 Add acm-multicluster-globalhub [skip ci]
751d65d67afd95386285e0a9a52609d1c4fcd281 [skip ci] Create version map
8ba2b8120971b8fe9b4736d5edd9d4232a457c13 Add acm-governance-policy-framework-addon [skip ci]
a2a6e6a9b691f8f3c864f53ddd850d9f6e4db154 Correct link to MCE install documentation (#398)
992bd7ad4f789aa633876dfb464c070ea4f30730 Removing SV2OB [skip ci]
c0ac31fc6e24522b9aa57994e1612ef80edc94b5 Add acm-search-v2-operator-bundle [skip ci]
52daa966d2c6af9e69a6152f6c216149686aa573 Remove hypershift-deployment-controller [skip ci]
19b4bae1e75a63e0bc552bc1d36d555abf404f3c Remove 4 search projects [skip ci]
2e7cff7c77184c41b47531967c9a15c543133ac9 Restore search-v2 projects to ACM 2.7 [skip ci]
c8d4fdca984d75962625b8427528c7ad38e55672 acm: Update CSV text to fix ref to MCE in a couple of places (#396)
e6730afc5049e9e37034a939058e5ea8a387c321 acm: Add instructions on disconnected install to ACM tile verbiage (#395)
89ced2a972646fb7a2804f87f90a99706d8bc342 Update doc links for ACM 2.7 and MCE 2.2 releases (#394)
ab6376a2bc658f3e47ffa317295c37b6f6f04e5d 2.6.0 => 2.7.0 [skip ci] (#393)
048f76fcd52a811f9635869f9f6878fc9b3e3f7e Add cherry-picking scripts (#390)
0435bc9b4d3cd001934652731e6832fcc507664d mce: Fix typo in subscription for MCE 2.1 (#389)
7a3450fcbd5c35b7639f63f5fbce3069e9e5133f Add ability to generate dummy entries in downstream image manifest (#388)
75e5785de233ae41369ae70c033737616de2ebbb Search V2 no longer Tech Preview or better in ACM 2.6 (#387)
82543f71c2577a5198dd262dbb91b66a2a6dafb2 acm: Remove cluster-proxy and -addon, now in MCE (#386)
98fceb673d05f4e10fe353544c08a498a6076143 Limit Release Processing workflow to release branches (#385)
94aad87f7ce845ac50b050fea3b8ec0e3aa6186a mce: Fix doc link for MCE 2.1 (#384)
2019bae5af968f3a1480d9bb4f647067ae07ebde mce: Add cluster-proxy-addon to donwstream image manifest (#382)
a88364ee78319cb6f186acb25aa8c283328106c3 Restore two projects [skip ci]
f1a1058332bcfd2490ba9a7e4386b33dc40d55b2 Add external image ref for postgresql_13 (#379)
652035e2aad15c0cc2a5142af9d60c0ffb893448 Adding cluster_proxy_addon [skip ci]
58909466f5d5157b97c5672abd5180b2698cef8c Restore search_v2_operator
2e85e4d8037b7e8ff4409f83c847b844ccf057e1 fix: Update donwstream to use config file when creating bound manifests (#376)
99ac33fac642b86f9cf62acc441b0397d7d47e92 Add OPERATOR_PACKAGE env var to operator deployments (#374)
dbf28e5152926f031e6aacf97a1ffadde6aa1ef8 fix: Fix incorrect relative-path reference to mce bundle config (#373)
065ad94a33218ffd18b7b9be389260feea3ff453 Offboard klusterlet-addon-operator [skip ci]
2e81af9cbd35992d756baa494926a89968a2baeb Update downstream config files for ACM 2.6/MCE2.1 (#372)
c019b67c96c4fb26f41e9992fadf293e9ba2ff11 More prep for stolostron/stolostron-engine community operators (#371)
359b060349215a23f84b1c163ff0f51315f534d2 Remove some obsolete bundle-image gen scripts (#370)
28ddd4fb268c5c6713d2dee15d68851b9e5ba8a7 Add -U option to use existing manifests (for debuggingmostly) (#369)
40c23ce5e0b4ab13b332a05dc903615367d129dc acm: Starting with ACM 2.6, get AppSub bundle from dev repo (#368)
cf24152dfc32c7dc57d5ed441823ccee54ebfd64 Do some tooling prep for our community operators effort (#367)
e2a2585cdb7434529650a7e8ab4da4a65aca1fa3 Some more cleanup of unnecessary ocm-hub bundle stuff (#365)
245f3956d969af1451ae0e6b690cdee8c2177574 Remove some unnecessary top-level build scripts (#364)
e0471daecf0eadc664a8c8da059a3de7bce668eb mce 2.6: Update doc links (#363)
e9dd18d2fbf2f3c87321ad21619b66d529108fa2 Update MCE links to documentation (#361)
462c10a1d784f10729843560af7e61193d36335a mce: Fix incorrect inclusion of namespace in init-resource annotation (#362)
1dbe1fa45e9303d6ff23be3276d668478d857afe 2.5.0 => 2.6.0 [skip ci]
2feca5a4269fbd78aafc58afe426fdebf6ff74ba Update bundle logic [skip ci] (#358)
c78afe9fcbb9cd46e0e4af7e32c80dff393b5746 acm: Update doc links for ACM 2.6 (#357)
e33b8b1b12ee7216ec62419e434b43e44f49144c acm 2.6: Temporarily use AppSub release-2.5 channel (#356)
087a6d29e808872f8583c523b1ab185d8fd73f6c Update postgresql_12 to tag rhel-8.6.0-container-released (#354)
7046e7ae8d3b5ac682c2d964333cac2d3812dc87 Remove three projects [skip ci]
7c6d51c9469b06a3ec0fb5b4f339e5fb6c806e12 Fix opm error detection broken by PR 349 (#353)
bbdef33acac9ad7352e96b2106c795668292bdbc gen-custom-registry: Suppress emsgs during image cleanup (#350)
2990385add49f4e1d135855ae7f1956b440f265e Add option to generate file-based catalogs, update OPM (#349)
13638175248123f8a031e32b10d9429ac41aa44d Update valid-subscription labels for mce
250f881e64e187aa199b0e2d8197fc2ce359f795 Upgradee version of OPM we're using to v1.20.0 (from 1.13.0) (#347)
ea841808ee2fbc7d6fc4e6bd30e9c557586ea87f make two oauth references available (#345)
e1206b71fa1fb95f208982a704cf38fb771cdcc9 Add ability to inject OPERATOR_VERSION env var into deployments in bound bundle (#343)
edf9639ff83bdeb0bfc22242e6813717b1d9049b acm: Finalize valid-subscription name (#341)
99475dfa026221031b954e135191a9fbad67a95b acm: Add valid-subscription annotation (#338)
d0979ef8f2e85b7a7cd1b0b71f21af57940aad0e mce: Add valid-subscription annotation (#337)
7ba2d0022057476fca8599c07c2ab64ae8357b4c Remove 4 UI projects [skip ci] (#336)
7132adc5b173dedb6c30804b75deeec325e9841b mce: Rename image key: hypershift -> hypershift_operator (#335)
f420f1d0f7667bfac2e3e582b428fcf400693e4e Renamed hypershift => hypershift-operator (#333)
29e4e1f61e06c8f39afe932538e63f95b19cfe9e Remove volsync [skip ci] (#328)
25b314fbd23699b1b949886d48ff87ee3e96b64b Update mce-manifest-gen-config.json (#325)
08d6f744f35ed86bcee4838526f93c1cd570e6df Remove acm_ prefix for eight onboarded projects (#323)
124be9b56d6d1357fedc6cf532589cad956888bf Adding APISERVER_NETWORK_PROXY (#332)
88c2c482849db1d43c521064120a615c3bbfafc2 acm: Add image-ref env vars to AppSub hub-subscription deployment (#331)
b78efc60091236a775c55a041b635b2db70424f8 Add 7 hypershift projects [skip ci] (#330)
c69ad06d0fe1e75f6f9bb6e71a84f7f898b9a630 mce: Fix typo in image-key name for console_mce image (#326)
08d33c31c9bc825b2516e5f1a0cf0102a5e30c63 update external image references for ACM and MCE
fa320606904e0ca9206fd01d0a94eb7b49291488 mce: Add hypershift deployment controller image (#320)
5e5f2c8f5e5a7c9c5c5ba6f49642d017ae85338c acm: Remove external image entry for PostgreSQL (#319)
3ee3344ff310162054f820e648b4dcbf8da2ebcb mce: Add AI and Console-MCE to MCE 2.0 (#318)
e9cf00c0ad8870700aedc64ea936b053f50f6797 Added 3 projects, removed 1 [skip ci] (#316)
6813a2d70b5b5b96a474def791ebc80f58260ff6 mce: Update API version in CSVs MCE init resource (#315)
021ea08525a5537377bbe5e0f23b058809fc99c6 acm: Remove image-key-mapping for discovery operator (#314)
2cbe501bf5946de421c59065a4a64643fd47bd71 acm: Remove discovery controller and CLC images from ACM (now in MCE) (#313)
712a6b945780b74427885ac094d0451a7eabbee0 mce: Add managed_serviceaccount image to MCE 2.0 (#312)
9b9871bd049e28f59c49f80286e3d9b233a03822 Add Discovery and CLC images to MCE downstream image manifest (#311)
3b05bd8b64fcaf399d75279c30d77de0a4a612ac Add five projects
09e4f91d3ea487b051b9b558f165598a35da5fc5 ACM-to-MCE Cleanup: Remove from ACM stuff now in MCE since MCE 1.0 (#309)
60094e445d103399ac92706fbaa92df67dac60a1 add arm catalog publishes for acm and mce (#308)
c0f99d9c18c4680981dec5fac1591512015887d7 Bump published OCP catalog versions (#307)
87f00b121455064e7f8318b1030c2ca764907664 Remove placementrule and deployable from ACM 2.5 (backward compatible approach) (#306)
ccf9b4ceaa47a1a7ac35798d7381f72b7c9a810c Removed deployable, placementrule [skip ci]
5e53f22409c347dc22f911fa56cdd37eb987ac65 Removed search-ui [skip ci]
8efbe39ad6d4972b9870a8c4a62b3c2c39a5a996 Removed deployable, placementrule, subscription-release [skip ci]
d41594186b866f56886bb58af69ae2c55c18417c Remove temporary ACM release-9.9 branch stuff (#305)
3992b1df5ea47253bbc554abce111e01f64e3e32 2.4.2 => 2.5.0  [skip ci]
1d9cc7d25926b42ea357555080979c4f4a6acea7 Update build harness location for github org rename [skip ci] (#303)
5e44b40321fe3a6ea5e002d051dce7a1488e479d Update action for stolostron org rename [skip ci] (#302)
aed2643c9e185530554e027cf1d444e894ab78a0 Rename o-c-m to stolostron for current ACM and MCE releases (#299)
5728a45755394e3dc1b7021ac8dad2bb0ae03cc7 fix: Avoid KeyError when imagePullPolicy not present for a container (#298)
dae12435c9cfd679223f14ee4dad820c9917821a Remove imagePullPolicy from all containers in CSV (#297)
c7b20fe895fc931dc655261443528e76fecdac9b Update mce-csv-template.yaml (#294)
372d667c49613369d5f690eb7d34ebe9792412ec Add default icon for slack messages (#287)
d06f162d17b511716bcf4d09bb59c3d82256c66c Ensure we only clone the single branch [skip ci]
dec7bf8cc42b18756cb0d42db6f44ecaf044868a Better slack messaging [skip ci]
52e7c7a2533346b27949068479a2c9ccd0f5554c ACM-2.5: Turn off prev-channel override for AppSub (#293)
e6628b82f402db39b6d88ed809fc5deda123295d acm: Set release number in doc links to 2.5 (#292)
998fc2a47e72af4400bed88ba7ae8ac2a22e37d0 acm: Fix doc link for 2.4 (#291)
fdaeee5bf2fb60fc1f2eaea7f343c5d9b710ee45 ACM: Fixes to PR 285 (#286)
e8c931bf28810cd52290ea7f758708ebfd1f4759 ACM 2.5: Drop out parts that are now in MCE (when building release-9.9) (#285)
edb549d3d83f3967027798b032acf09f529a70ba Add PPC64LE and S390X as supported platforms for MCE 1.1 (#284)
62d4088214fbd95339360ca5f243ba671c397d60 Align activation of s390x support with correct (2.4, not 2.3) release (#283)
1557ce496e2f63e1e6427fc61ce6dddb452318e4 starting with ACM 2.4, we should also be shipping to s390x (#282)
528f5f2356cb72f383d41e9f91af9ad2c8d39ebb Fix missing-previous-bundle errors when building upstream catalogs for ACM 2.4.1, MCE 1.0.1 (#280)
0dc198f1c4007c860106105272df2fbfa3f3445d fix ocp version file variable (#278)
d866d31147e80f9fe08048a4acb6a8e78d5fd946 Add github action that will only trigger on not-master branches (#276)
78e2ec39c4478407e292dbc02ca2e473afedc810 backplane: Update doc link in CSV description (#275)
6431bac1f17fd936fe1d554f181f3bc3d1b9a5ff Backplane: Add CSV badges and doc link (#274)
bf1e86c28cafc6a43b3b7b324bac071e3da1e459 Add fips-mode 'badge' to ACM tile in OPeratorHub UI (#252)
e446aa5dfd6ffed1c74eae28dda5fc033e327871 Update MCE Image Reference (#273)
51a534ce202097f156483a525b132c1b2e28b5e1 Update MultiClusterEngine image ref containers (#272)
c157de0a63d99d3db69f4141010bea0132ae4d80 backplane: Change image namespace from rhacm2 to multicluster-engine (#271)
c770593e5dd541f6280ae05902e48bb583754feb Undo temp bypass  made by PR 269 and cause abort on unlisted CRDs error (#270)
21d6737b06b45eb1d83e7c616833b2d1b0663411 Temporarily disable bundle-merge unlisted-crd check (#269)
6e64f6358302784bc0c784818f622e9e7b53b566 Update cluster backup image key name (#268)
b802d87a0ecb4c4871ff5aaf6ddd8041232e0f32 backplane: Use lowercase for Multicluster Engine (#267)
715e10fa824b4cc9214b47cda2fd2bd3f843cee1 Add experimental (disabled by default) handling for CSV webhook defs (#266)
0cb64fc47951ccb55da8863c260e3e0fb34834d8 upgrade-orchestratoin: fix: Don't ignore -n option (#265)
57f5d492c4c197691f2a0d869dd33e6120408240 acm: Add key-mapping for multicloud-integrations image (#264)
381072ebe18c5092aba9a582ca61f509546553c1 custom-registry-gen: Backoff upgrade to OPM version 1.17.5 (#263)
673aca068d679fe7992dac270a0dd35d07ad1a90 bacjokabe: Fix display name (add for Kubernetes to it) (#262)
b2d337c5506a1db0be6b1991613d738ca4666db5 backplane: Spruce up pkg description in CSV (#261)
05b9a20352ce314f14b89defe06fb51d53b88e55 backplane: Change to use MCE in manifest/bundle/catalog script names (#260)
7d7d250136e4bf4423f145ded528ef87aa694b2d custom-registry-gen:  Update to use OPM version 1.17.5 (#259)
e5abd90455f5816f4a22e441b585f1f5b23c5e5e Update common render-templates to use config in this repo  (#258)
329d10f45247d3e26030628b60556219ab67d49a backplane: Move config for downstream processing here (#257)
0cc1d273c651f027e80fea7ec393afb4afa975df Correct managedcluster_import_controller name
29563cace2b50c3103d9e9bc990dc5532057b9b9 Added VOLSYNC components
a2b51fd845bc813dba6873b5baaf9d0fe019ecdd backplane: Add import controller to downstream image manifest (#256)
804f9a423ddc6e2e7e6711aa0cfa2272236a9996 rename to multicluster-engine (#255)
c298d8cdab9c5a328e8c5030c603f2913fb15711 backplane: Rename package to multicluster-engine (#254)
b6d3c0a8e403e591eb563c5fb27ad7babed36411 Moved CLUSTERCLAIMS_CONTROLLER
a2cb245876b205e49b28deba402c3ed80372f444 Added CLUSTER_BACKUP_OPERATOR
9c43befabaa2ff6e066d3b1100c975786b846cf6 Add VOLSYNC
100ce0e678a7ed5cf7df2813d48e54adfe482e70 Added MULTICLOUD_INTEGRATIONS
2ab9a61465bdc5acb2be23caaed60e3cb555f5b6 Adding CLUSTERCLAIMS_CONTROLLER
aabdfda4ad69643b8f885f1a646c983a33bca9c4 backplane 1.0: Remove hive and registration from bundle (#253)
95e17e5d7152b46e9089d840aa2d744dab8320d0 Add prometheus
4784731b4be179e5fd1623d69a8dcaf758b8dede Add node-exporter
8c0635444a49185f22deea9344664b790916a7d3 Add proxy-aware 'badge' to ACM tile in OperatorHub UI (#251)
7d64cc4912aeaf0186820725e935e18609aba6dd Ray is a first-class CICD citizen (#249)
c21e9377f54a7af3c4c03e4a4150929f212eba48 Extend bundle-finding optimization to trigger on full semver rather than  just x.y.z (#250)
62c7ed02a44547465ac01041a539af4d946ab7e9 Added KUBE_STATE_METRICS
a376ff4d7372076b075a27cea17cb65ff3d9991d Merge pull request #247 from KevinFCormier/patch-1
f3ee6eb4227248f0d69acad918d754ca474ac424 Update manifest-gen-config.json
0c758c805a73254541eee7e8e5533d9bfd38501e Added ASSISTED_IMAGE_SERVICE
8a36b0689c0408db9a5f3b7c2fbc45e0515cc548 Add CLUSTER_PROXY_ADDON
588c6ce2fc80e0fcb2a7b76a749726621bd6e37f Update to release-2.4
a1527b5cb4164d5d043c8dfa133a1df6da2700e1 Move common render_templates logic into shareable upstream script (#246)
3f836676b2947ba9138cbeff29f3246775d712ea Removed 2 endpoints and 1 rcm
052427a3bcf9f26d255b8075e022cdcfed77c1be Add work image to downstream image mnifest gen config (#245)
fc8ad0a0543a76472139eabd126f704d2e03a0cb Generalize image-manifest gen script, add config for backplane (#244)
c34be0203f08cf5b29929dba6ab81fbf922083fe Fix type on version number and bug in curl error detection (#243)
6eba267e25ee02f226c03e1fb5c804cdd1db5e64 Revert to using opm v1.13.3 again (#242)
6991959636d0b87cc6ed665074be253e53496738 Oops, OPM v1.17.6 is broken, use v1.17.5 instead (#241)
4b2331c55c574f2f231eb31e0077f3990178ab85 Upgrade to use OPM v1.17.6 for building custom registries (#240)
1a5943cf03ee6cc76cb78e00dcf2c14658a9ed9f Remove most CMB 1.0 temp scaffolding (#239)
9d9a7e0061a382294d2d856a1346ac9e72483e08 Add script for finding image refs for ACM's add-in operators (eg. Hive) (#238)
0a886678b4281144cebf2e3bfd56d2fe82416f92 cleanup: Remove left-over dev debugging msgs (#237)
f8afc5901fe84fab6795417a968ae8e88740df23 acm: Cleanup temp directory when done (#236)
0ed1c6570723943d963529fdad95eabe7a7d9356 Refactor and optimize bundle CSV finding functions (#235)
f23e3d35d8d0047b18e6e3fcf419e4f3e67485a4 ACM 2.4: Turn off use-prev-channel override for AppSub/Hive (#234)
559562fd528c8277e41d6d2c9fd72970b8da3ed4 Merge pull request #224 from open-cluster-management/remove-kui
5aec3a35923faed8d90973085ee3d8def2e3be46 Report error/abort if a specified image-ref container was not found (#233)
9bcf4373b0b0e21e27f00648fdcbd5b90bbde025 acm: Update hub operator bundle location (#232)
b6694cbe894b73440d30b9d1acc02c45cf761e9c backplane: Track hive ocm-2.4 channel until we get a backplane-1.0 one (#231)
a9031a594b50dda2e47dfa4b7bd1abaf76135041 Tidy up interface specification (#229)
517a9dadd68bf48594cb671d69a8f94cf0b3a415 CMB 1.0: Scaffolding for an initial bundle build (#228)
84b9bda66f110eea1cc7de54333b4d30bde118bb Fix previous-release calc typo/bug in prase_release function (#227)
a86dcb64633131104845ebb034c421223d946bd7 Change location of upstream community-operators repo (#225)
91b5406e5365738a320fa56e3d76a62b49901bb2 Remove kui/vwt as of 2.4 Related issue: https://github.com/open-cluster-management/backlog/issues/14399
bbafc0ae531f732881b7860128e05d131975df41 Fix bug in channel-override logica and temp enable overrides for ACM 2.4 (#222)
940723d9c9a9e309aa059a7a13bf9ee836c96007 Update to use new observability bundle location for ACM 2.4+ (#219)
b19cd90cb6e3bc8ee4e7ba805397d18397577819 Update name of observability-operator repo to current name (#218)
de68a15116c024aa5cf8e4f8c8bf4dcfaa8afe0f Initial/scaffolded tooling to generate Backplane bundle image and catalog (#217)
b5ae101b5543d8fe4508916e1b4ca161bab2fc40 Allow ServiceAccounts to be defined in bundle file (vs. CSV) (#216)
de918ed627af57c001c83f77b6c471be0d0f09a5 cleanup: Remove dummy image manifest files from master branch (#215)
703228a7081ed8ca2452bb524818bf74af6df2d4 refactor: Make bundle-image-gen code more common (#214)
2a656788e157dee2197950fa1e85185ee4e0fbc3 refactor: Remove cover scripts that are no longer needed (#213)
755e9825e5e653fe3cca2f8f7c2c1dad13934933 refactor: Move common manifest-gen code to Bash function instead of source'd snippet (#212)
d512cd3c9f2bace437e3a8b3c5b361106805a304 refactor: move bundle-common to parent directory to enable wider use (#211)
4b42133e598cdd66845109a8d16890ae26ca5014 ACM 2.3: Update rel number in doc links in CSV (#209)
92075b0cb0cee15e9b3470c70d6a514b7f2f8838 Elevate severity of finding SAs in bundle from warning to error (#208)
f8951cdfc486d1c4686864027044c5eb233a4634 Remove console-header for issue https://github.com/open-cluster-management/backlog/issues/13561
95dd98089c049019607e953b53793b9195467049 Removed klusterlet-addon-lease-controller
13b89d4433bd520b0f09af10212d37f38ba7c895 Merge pull request #207 from open-cluster-management/postgres-patch
f2eae8cdc873224321d2c7c6e2484935cc9e5c35 Slim down postgres image [skip ci]
51a0cfc35213b637bde61f5a999f21d4a677054c upgrde-orchestration: Add option to install operator on infra nodes (#206)
9ccc731cee8d1f470d9690de8ceb7135593964bd assisted-service is agent-service downstream
3e9fda9c10ded89b2c0c6122de87df45c368c786 Add cechking of bundle size against the OLM limit (#205)
14f9683d431d10095a68db4ab77471ed5e9546ec fix indentation error
0bcc036e98a7e54c5f6fff0481739461137bb2cf Fix how floating tags are determined (#204)
be6b5fab7fa2daf3a36ff15685a0b746f7c19888 Add Assisted-installer components
2988b5a930936eefa892c2c2cbb40d4a00bd2388 remove configmap-watcher too
6d3ea85b4b81f787d6dacf965dae1a7ff7d908ae Onboard insights-metrics
5045907b6b5aad830452b34d8c2bacd02192707b remove cert-manager from bundle scripts
77ccf49d42940746a368bfde355d25db429dd126 Onboard placement
37d4ff92a988990c9f5bf8279ccb99d759fae2f7 Use new hub-operator repo name (#203)
0f85481988199041051c40e13c420f116fe4d45f Use stashed Hive 1.0.5 bundle for ACM 2.0 builds (#201)
66d29f501f73d9cfda93b743c07386b0d752ad45 Stash a copy of the Hive 1.0.5 bundle for use in release 2.0 builds (#200)
b47d02de2c46a8587099443c50823b089b0221aa Remove Discovery from ACM 2.3 bundle (#199)
674a88043105101be3c17e3f6e1491800b162611 Fail with resonable error msg when no CSV found in bundle (#198)
a85ab49862602d50a124db9dc2be198192a39233 Merge pull request #197 from open-cluster-management/manifest-gen-update
01b9b233ed763d73df84d36a1590bf4803299c94 update manifest gen config
35414979d692b7ca90776cd3e0f813cbdca402c6 Add CSV labels needed for multi-arch support, plus some refactoring (#196)
3e7f20d6f302bf4a69344ddc944e4213e2e58c6d Refactor App Sub and Hive bundle merging to use new common code (#195)
1e0b92edfea04f5780fa284ab63f3d16f3724c3f Prepare for merging in AI bundle, but don't activate yet (#194)
afa5c63387fe777aabe1e6cd7ed80cb382e7e1cc Fix service-account check bug (looking in wrong part of deployment) (#193)
cdad4f825c77283efad8c5b3d5ebffbd71725ae7 Onboard provider-credential-controller
ba39c6a1e41c74f32452fa7eccdfc36148cc7e22 Add deeper checks for default service-account usage (#191)
d1ccdf5780a2e0d9d1b84329f75dab7712ace1ca Create CURRENT_RELEASE
af3a475fd12600d5ce471bbecbf5cd8cf5112984 Onboarded prometheus-alertmanager
b70b854a4a3eef621cfbf482bf4cb970c0459efc bundle-manifests: Don't always stop on first error and other fixes (#190)
7b16e846de9133ac2c0642cb3c8cfbb7f58ebd7e Chnage location of monitoring op manifests starting in OCM 2.3 (#189)
62c92b14c798d1ac8f8c7b326308ad2baf7df74a Update manifest-gen-config.json
7174fb57be2a49163d2365d4d8331b6bcc1eeb8b Update manifest-gen-config.json
b0adf7c3a28d66e01744d7122fa1b2540ed11d80 Fix syntax error caused by last PR (#188)
7e70d5101261a4447aaabedc4081f369e8258f98 Turn off use-previous-release-channel overrides for ACM 2.3  builds (#187)
4c5614b8bc8432b5dab9cf54439025cdee94ffb5 Update manifest-gen-config.json
cfc8e577375d513c7a2437826911645fa9ba18d2 Add more explanation to top-of-repo README.md (#186)
03086b58e26b49aedd12fa94c05e5fcc806f0580 Remove some old stuff from custom registry and top-level build tooling (#185)
fe0f09716669b5b0fa20ec158793280469f52aba Remove some old stuff from bundle-image-gen scripts (#184)
c61bf3540ea0566a2b20983a2d33b21b1f8074d3 Fix: Add OPERAND_IMAGE env vars even for images used in CSV (#183)
7fcccb032046614da8495627cc603a0137da6cf3 Clean up generate_manifest.py's handling of tags (#182)
7f3ff14bdc864c7fa9e8e5f517616022a3ad04d4 Add some bundle-gen overrides that might help community contributors  (#181)
7b3b5b1978d670e738d8b9a9a585674a63144af3 Add initial OWNERS file (#180)
19623c17f7513d2794d5aa1b2107d8ffe1acfdc4 Refactor bound-bundle scripts to eliminate duplication (#179)
404a8bb1b1d0e31347ba6797b2cd40a3a09d8086 Use OPERAND_IMAGE rather than RELATED_IMAGE as env var prefix (#178)
1bbf34d5448eaff7247d771a03cbc7ff2d293e7b Add ability to inject RELATED_IMAGE env vars into operator containers (#177)
d2ba93d84171f1f8acdb13d8310f00990d3c094b Remove some verstigal app-registry-format code (#176)
a12e26e0bcc1d6e30ddb31290a51fe582d56ef47 Prune out some long-dead release 1.0 stuff (#175)
35c63966898cf1c6c9c4c55f87031ebd18471fd6 Stop using package.yaml to find unbound bundle directory (#174)
bcd2e931774d7c7e7bbdb4480cdd8d022b0947e9 Add release scoping around enabling of prev-release-channel temp fix (#173)
351d6c84ebe4c9fe91d6824a4b4a0e73c2ddbe2f Allow skipping of z-stream releases starting with ACM 2.2 (#172)
98220eeadabc75fe6f2e8512aa00e7e8441f3129 Update manifest-gen-config.json
81b52d7fdf1251452ffd4afbeff7ae12c3f9b9f3 Add error msg to report JSON parse errors for some CSV JSON annotations (#171)
0ef8360a30ce49d41dfcd6e0a8ca0617de631920 ACM 2.3: Temporarily use ACM 2.2's channel for App Sub/Hive (#170)
5ca350f4e15b776e0e95aa15b6e406d5e07a88d1 Enable use of V1 CRDs (#169)
df8dd73700f6b331fb29acfa6eaa77575ad18d66 Fix OCM Hub custom registry gen issues caused by PR 164 (#168)
329408c5a78d27d6a19127495d51728eda140aea Update manifest-gen-config.json
ec01fa98fa635d5094b4c16e5363dd874c3e7864 Fix upstream catalog creation issues caused by PR 164 changes (#167)
91fe32e627a62b37450bb7eec80a0ed214e640b2 Add support for internal-objects annotation (#166)
3b38e093fd812d2f559b361245f4c803e6df2f72 Disable support for V1 CRDs until OCP 4.6 is the oldest OCP supported by ACM (#165)
63cdcb515970ba41f4cfd95dcc5d2c0b6c8125ed Add abiliyt to specify skips in CSV and do so for 2.1.2 specifically (#164)
754eb7ac5982615a48395e1cfe8b1f3d0992b72c Add support for CRD/V1 manifests within a bundle (#163)
b3c5c30ae0347ffebd24e561a27fe18c4eb3596e Update manifest-gen-config.json
883659cc29d0993f1cf8c921cbc38e036ee6aef8 Idenitfy bad CRD manifest files when they can't be parsed (#162)
42bfd36a4c18639e783c55e2182dd5c6000c2f19 Update manifest-gen-config.json
8f24574b481ad88d79bb9299b8166af254574da6 Defer Discovery to ACM 2.3 (#161)
aab4bbdcec87f3d0c41b99a9aa5225e2512794e9 Put discovery stuff back in effect to align with change made in release branch (#160)
929812f659398273c7243fc366e1ec88e202b144 Actually remove all of discovery parts (#159)
e808cdbca14531cbe81c0ab4e11f2455c9ef8c41 remove discovery for now since it is likely bumped from 2.2
82d45ad96827891f98738f1d5e8fc8be3015c3f4 Restore search-ui
f8a6a354a719397685b7eef875c4e61e953b37e7 Remove search-ui
b5723b19e81ac20584924df6aae880de7867ae25 Restore search-ui
43b42a511ee941632dccc93ee4de97be8068def3 Remove search-ui
5eba1fd105cdc8e77d4bc704530a7ab2384df97c Update manifest-gen-config.json
d5b92c6448a15ecfc8c6ec037331a329d9310248 Update manifest-gen-config.json
79b6f35029b7c34f2aa2faa192b181217301c62e Update manifest-gen-config.json
29db38d7682b87c876b02ee68ef52a21ebc64723 Update manifest-gen-config.json
eba03dafb3add2b57104c692b394a5bf3839aa56 Update manifest-gen-config.json
ebb0cede63232b0f93ac010d2a39fea350efc091 Update manifest-gen-config.json
900b76db79b4cf8f0a7b89e4fab0d8dbc31c4c85 Add discovery operator for ACM 2.2 (#156)
7fc0622d018dff64d5b30c88c9830ded226344bd Refactor bound-bundle scripts to eliminate code duplication (#157)
9b14e7ab906b485f16230565000268480df5cf8d Add submariner-addon to OCM Hub/ACM bundles for ACM 2.2 (#155)
48e23f0564013e786e9b6340334151a35a9ef0f9 Cleanup I failed to commit with PR 153 (#154)
37e550265083597564f68ec270640a004006c376 Rework handling of release-specific stuff in bundling scripts (#153)
cbb467290bc5658f25033f1711ed1abceb925389 Upstream default channel should continue to match the build's release (#151)
687211f2ec69c4a4ac3829d1b8e1a25de1390191 Specify default channel explicitlyl for upstream ACM bundle builds (#150)
3d2ada1282aa427a42f0285405b29e8a5670cc28 Add previous-release-channel override logic but don't enable it. (#147)
4d084472c9985ca3cdfa084ba841a8f7458b6905 Allow default channel to be specified explicitly rather than computed (#146)
574b61fdcb348b6241e8010353588da5dfb20fec Only specify default channel on x.y.0 releases (#145)
25ca5c4b1e53cce657c34f196b5cd85a54600ee2 Tolerate multiple yaml files in top-of-package directory (#144)
3dbbac0b357cb128b8be15d9a618b58e00a7a38c Hack to disregard "ci.yaml" (#143)
b22af7503c23334de77993294662dd0f3d63c398 Add note about need for AUTH_FILE env var if using podman (#142)
962b2b2b54db2c3381ea1f7c350402396fffaf7b Add initialization-resource annotation with MCH example in it (#141)
852c0de39b07b76c9be601acd9f46d95be2e7cad Undo change to CSV display name (#140)
df04880891d494ac9dd835de962f1bf02cbcd7b5 Change ACM CSV to add Red Hat to front of display name (#139)
c1963814c05120794e39ceb45ad4046daf0d2475 Update doc links in ACM CSV to poin tto release 2.1 stuff (#138)
2d2771266bfae5e18418163b789467d27a0baf50 Sync manifest-gen-config in master with release-2.1 (#137)
94edeaa1c29e0559cec7ec827bd44afba1e88dc7 support name should be Red Hat (#134)
89a94bbc5eda78d733d8ce17bc419544c7914c46 Add incremental bundle images via $COMPUTED_UPGRADE_BUNDLES [skip ci] (#133)
1c062dc4a10df8fa847566ae440f8ef7e70a311e Remove multi-registry check/error from catalog-building script (#132)
c4e832d624f6a5c6842d14f37ad37334d4b7c0e6 Update manifest-gen-config.json
b4494ad1d7b7ed26d69c22d30e036e12edf736f3 Fix: Add image-to-key mappings for onservability operator (#131)
3bf88398bb31b4e0c0741a51462736ab5ecb1338 Enable including Monitoring bundle in 2.1.0+ builds (#130)
62f001c6d6551e544af23af45a65dbd97245ec56 Filter out unlisted CRDs for release 2.0 builds (#129)
22db8c5c38dda1191cd2cff9639ac3b74c5c6ac9 Add grafana to external dependencies (in master branch) (#128)
fd8e413aa3f703ff44955b8e6e966ef62e51d6fe Get Hive bundle source from ocm-2.0 channel for ACM 2.0.z (#126)
441a9474d4a22066a48bb1c5dabaa495ec54e455 Get ready to pull Monitoring operator into ACM bundle (#125)
c9aa83bce06223cc3b63bf934260463836c1d136 Use release-x.y branch as bundle source for Hub and Cluster Mgr (#124)
b1abf5aaadd2dad9253a9d41d4938ee87d73edb6 Put PR 121 changes back in effeect (#123)
ca000f65b45ebb560518d9b7907eecb3dc0f077d Temporarily roll back PR 121 for quick-turnaround-2.0.2 (#122)
ae02c6930f54793e8b797ad4f1de22d694b72690 Indicate in OperatorHub UI that ACM supports disconnected (#121)
71b34c91db926ab8be7e5e85eb6c0178edde8d01 Extend (not yet ysed) find-operator-image script to handle multiple operator images (#120)
4ce2b84c5921a4e700c474409add0647746c235b Fix: No skipRange for x.0.z releases (#119)
d02b587f2b6968b957b8fd58e988d2ed2daad959 Keep Hive pinned to V1.0.3 for ACM 2.0.z (#118)
63865f0bfdd2955667982a5c8159d3022b026741 Need skipRange on all 2.1.z releases, not just 2.1.0 (#117)
021dc225f82e46cb904c9a8e69fcb266dc5f7788 upgrade-orchestration: Handle Upgrade-Available status (#116)
38fba9144f43e3c13b215ab07b1c3f37a75475fe Update ACM CSV to indicate Seamless Upgrade capability (#115)
142950adf2e451a4b29eb42222055da2221aac9b Add observatorium to manifest-gen-config.json
2393227f7e90b419c56aec2e3a33f19260a826ee Tidy up handling of acm_must_gather (#114)
e679772d65cd6ae12e542f45e871eb0f53ae5e76 Add acm_must_gather to manifest-gen config (#113)
4747af019928d9ca92afa664eadcd8fdcd74e838 Pcik up Hive bundle based on ocm-x.y channel (#112)
64f0c7a951c078faec2aab886f766ff6bdd48347 Fix custom catalog build failure due to podman/docker incompatibility (#111)
44209e079102a62a9ee8d1669418659ec1b4dd27 Add reworked downstream image manifest gen script (#110)
8e7a9928d209e83bae480eb084e0c7a4205f41f8 Add ability to build a multi-bundle custom registry (#109)
6d72c55fe51a6c463e244d3f95b75b31da183f51 Add support for skipRange and computing replaces/skipRange based on semver (#108)
e763d2217528ad80e5f354f8b7a8afe11964e517 React to rename of community-operators directory for Hive bundles (#107)
b0694a2acfddf2619a531b67f8f86adb879391eb Fix formatting and doc link in CSV for ACM 2.0 (#106)
7e034e8f02b4993bfafb2428fba8af12aa01f694 Freshen master-branch-only test image manifests (#105)
3cff06a3c23f0def3398248ebe2961599a18a972 Content review/changes on ACM CSV description (#104)
efb167ac49c3d052697a9f9e3ea19f1fbdbb71c8 Switch back to using release-x.y channel for App Sub in OCM/ACM 2.1.0 (#102)
7d8fd693425a573880a104d8406b22b3f99041e6 Temporarily use App Sub release-2.0 channel for OCM/ACM 2.1.0 (#101)
70e65ed54a3c3797a769e37b76edebe4b16010eb Add find-acm script (#100)
914f9b89f7fff3a30d78fdfb37fe08eac809e0b9 Update ACM CSV to indicate maturity-level stable rather than beta (#99)
7347776c0a719f7d19a242d72cb201f99517a6e5 Add ability to install operator at latest version (#98)
1f1f4a3cfa1bac523904829673d20a646fd37556 Switch to finding App Sub bundle from channel x.y for ACm merged bundle (#97)
164d7e2aa84e2260864d94266ce4b5e846c1db00 Extend upgrade orchestration scripts to be more flexible (#96)
916cb107dc9c0a6cbd7d18271b39d26a0876f386 Add writeup on manual upgrade orchestration  (#95)
d0c76559d07a730be5f5c604f016f6128e1a6b16 Add some simple scripts to orchestrate operator install and upgrade (#94)
69d426e75b1717a35b37787fb13b5db91dbf7e38 Cut over to using new release 2.x Hub operator bundle generation (#93)
ce9c4a4826b81b6dd5223e922dab7cb27e9559ec Permissive mode no longer required, didn't really work anyway (#91)
cde91d63c3e73933adbffbb952af7ce3b9fa42c5 Fall back to registry builder v12.1.4 after continued problems with .5 (#90)
d66d413e089de4e057def6f2ec375e07566b7a50 Move to using the latest builder (1.12.5) (#89)
ca792fdab3f8eaeb288856c185d2cf6f2b1da50e Avoid upstream breakage, pin registry builder used to v1.12.0 (#88)
31baa1e0507c534583ad2e5a84a732efe1340549 Build app-rgy-based catalog using permissive mode (#87)
822d64c8e09c804f7baf78ac7df08759029bee61 Fix missing Dockerfile in app-rgy custom catalog building (#86)
b82945cc6f35cad8aebad22a11b53331b45b8b28 A little more cleanup (#85)
5b6e8b713ec70bd742a0a0f42aace2b23b4e598a Cleanup hacking scripts some (#84)
7773ef35b725585941e305befdc46d40b96c7b81 Add dummy image manifest entry for nucleus operator image (#83)
dfe6c22a8a30f0edb748b83363996a96e4da47f5 Changes to merge nulcues operator bundle into hub bundle (not live yet) (#82)
51a48e0da64da18bc5a5db2dceadfde30feac650 Clean up image manifest samples in master branch (#81)
5dcd2808b3e831944c610452567cd8d259345944 Rename merging script to reflect its more general use in 2.0 (#80)
6a9f95b6c3694707a09c65fcd5f1814b494e9b87 More refactoring of manifest stuff in prep for diverging in 2.0 (#78)
c88cddc2c5d3c095085c66779d5a61ec5dd6a80a Rename bound bundle scripts in prep for adding cover scripts
1a2b1a2dfb6dc35396cae74ecb17096b3fb32c17 Add cover scripts for version-related redirection (#76)
359408ba2c96e9da40a6fdbf6fa5340304ddf3a7 Refactor bundle manifest stuff in prep for diverging in 2.0
a1441ed59d8137caa7e4a9038f28d67dd4ca5e5e Fix failure to propagate rgy-and-ns override option (#74)
031b25c3d653d3bfec6a07968ac43af83a6dd0b6 Change e-mail addr in ACM CSV (re: Backlog 2425) (#72)
8681684081d3545b30de2f3b2b0b7a049076f5b5 Un-check finger (#71)
b64d54b87be0e290f4b79c01bb011ff792b567cb Provide distinct option for setting bundke/catalog image tags (#68)
fb7bedbacf8cb3a6105efc255c68d823521279d9 Fix docker image prune confirmation prompting (#65)
f6d4aac16edf2d09bff54f0c08664711497dbdf8 Remove artifacts from back when we built out of master
5115cbfdc0d51e36834a66eb7c4178ef5a1661d4 FIx channel name for OCM Hub bundles (#62)
0590df92ba294096083d7f0b98460a09e58e379c Add new image and catalog building scripts (#60)
35b8f919cbbf331882662039af5125cf47f86182 Fix incompat introduced in last tooling PR (#59)
213a0993753ec9754d6813799c1b193f7f92ed12 Update bundle manifest/image scripts to enable release 1.0.1 (#57)
d180a52db99abadf9fed80ebec28e4ea15208211 Don't build out of master branch, ever [skip ci]
707dff1064e97604c8787e016110d9e5ec23829e Add snapshot 2020-05-21-15-38-39 for release 2.0
e142b99ad12648d792169be9c56586159f60b215 Add snapshot 2020-05-21-15-25-20 for release 2.0
a57e9c73e761edc133f22825aa3f4d670313684d Add snapshot 2020-05-21-15-24-10 for release 2.0
7a97ef8e2197c5c21f5a783b9ae221e05a28469d Add snapshot 2020-05-21-15-24-10 for release 2.0
3cda970dfad58bab73b81168ad8e2268de81fa86 Add snapshot 2020-05-21-14-51-03 for release 2.0
9d273e7b1f4205b7c5fc6fa9fafe44b74da62e8a Add snapshot 2020-05-21-14-50-37 for release 2.0
cb6a6e4c11964c2fb7f81e85979e6933395081d4 Add snapshot 2020-05-21-14-00-21 for release 2.0
7807819020801e3ef96816feed3b26cfa556721b Add snapshot 2020-05-21-13-59-11 for release 2.0
89b1b2dc6cd3c01c714709ae4f457918b9a48372 Add snapshot 2020-05-21-13-44-21 for release 2.0
9ef6871ab88c7971b04687c6dfbf7c5f2f5b0add Add snapshot 2020-05-21-13-37-38 for release 2.0
69863bcb0e0e502f3812b088b8b9d649544b9901 Add snapshot 2020-05-21-13-21-00 for release 2.0
3377d926d264da227200c65afe5f4de8fa71041b Add snapshot 2020-05-21-02-48-31 for release 1.0.0
ca4c4d33bd55345649f25b3f9a51665e83ba146e Add snapshot 2020-05-21-02-45-33 for release 1.0.0
16e677e13dc2dfb1104032c53f7e4c73b0b6a350 Add snapshot 2020-05-21-01-49-42 for release 2.0
e681b5f7f7a4132872eb7556d236a71af160262a Add snapshot 2020-05-20-21-22-22 for release 2.0
2c1720034557cf59f318109d923ae9092848b412 Add snapshot 2020-05-20-21-09-05 for release 2.0
4ac83052632c71647118adae3bb8ca3bb4ab6a57 Add snapshot 2020-05-20-18-55-55 for release 2.0
215cae0b4e69295408b13bc0691cb53523b6b1d1 Add snapshot 2020-05-20-18-53-36 for release 1.0.0
0f0504ba2bd2e6e6dff4d902303604d49692fdc6 Add snapshot 2020-05-20-18-52-48 for release 2.0
ed72297bb6dcf1be39f7ddd15b4b9bf63517af0e Add snapshot 2020-05-20-18-51-58 for release 2.0
84efda34765eb2998d13f1b22546ea63ca30e78f Add snapshot 2020-05-20-18-51-21 for release 2.0
6a1681a80658eb1c1003a1432fa74781ac7f3f62 Add snapshot 2020-05-20-18-26-58 for release 2.0
1a55e78f5fee656b7f609b2fd6a3a3a2f6d4a102 Add snapshot 2020-05-20-17-57-06 for release 2.0
5985d7104e9b4b2a63f887d1ce7e099765fb82bd Add snapshot 2020-05-20-17-45-45 for release 2.0
90b93379e74ae36b5b805955629aae8875049707 Add snapshot 2020-05-20-15-42-01 for release 2.0
4179a65b63da88998029a3b2aac7ec5a5359e67f Add snapshot 2020-05-20-15-42-01 for release 2.0
bc5027d11812805ff49247dfb5efeae45ccca9f6 Add snapshot 2020-05-20-15-10-19 for release 2.0
f146ab3300ba2a4a4aa57f2d9f16c5557787965a Add snapshot 2020-05-20-14-35-33 for release 2.0
ebfa7756228696e22bd3d897824656d48f975a12 Add snapshot 2020-05-20-14-31-21 for release 2.0
fb97c2ef7d70401fb81ef07b6858609036162b70 Add snapshot 2020-05-20-13-48-12 for release 2.0
4ea4437345edfd24fd3b44fe8939afa1f9592b41 Add snapshot 2020-05-20-13-01-26 for release 2.0
4144be8a7026f70bc095abcda256420a7e42db7d Add snapshot 2020-05-20-03-28-17 for release 2.0
2ab0c6b3441d7d136fcca49fc0b469c0e4bfa2b6 Add snapshot 2020-05-20-01-40-34 for release 2.0
487b1fc8c3fee4dcf33f5dadf7d299d449f7b4aa Add snapshot 2020-05-19-18-11-53 for release 2.0
57c6126c977922cb960a2d7b4eec97a550d08f07 Add snapshot 2020-05-19-18-10-44 for release 2.0
a553ce23d61f5f54163db78b16ff270e9e1a9491 Refactor bundle-image building scripts a bit (#54)
b1e5936b7cb016c1689bb220133724e2d6276f31 Add snapshot 2020-05-19-14-01-25 for release 2.0
3c336c86a25f9bcf004c24673633518dd49011f7 Add snapshot 2020-05-19-13-58-23 for release 2.0
3ae0208b59413ae6e31188a23a22c0816ff3696e Add snapshot 2020-05-19-13-22-05 for release 2.0
8112c9a90fdecc66481eb9de8ec4ee01eac7547b cleanup: No more need to commit bundle manifests in tooling branches (#53)
3e6730dedd495a27892febf9a39c9e57d3b3ef2e Update bundle tools to parameterize version better and produce either bundle format (#52)
50bfd5af5331dd181a8c1ade63066188ca1d8a65 Add snapshot 2020-05-18-20-54-54 for release 2.0
36ed8d1104aa429b7c1774130b10d77c4cc9c294 Add snapshot 2020-05-18-20-54-54 for release 2.0
6511ddd2d5c87868a7440cee1c26dc195e586227 Add snapshot 2020-05-18-19-08-49 for release 2.0
eddbff3496cf87be9859aa9775cfeb92b2d063e5 Add snapshot 2020-05-18-19-00-07 for release 2.0
f6c5a1d88fa940c523890845fe75186b7afdf4ab Add snapshot 2020-05-18-18-47-30 for release 2.0
4cf48ae39cafc1615973fe6a98f9415c588077d0 Add snapshot 2020-05-18-18-47-30 for release 2.0
ab03af84680b8bb14c0c7d7615f0cae526404e9a Add snapshot 2020-05-18-18-47-30 for release 2.0
51f11c47491444d042c9cb9b40a235d46a4706a1 Add snapshot 2020-05-18-18-47-30 for release 2.0
24f8c7594061b537338a233c82a22107558662c9 Add snapshot 2020-05-18-18-35-56 for release 2.0
f25a2469bdbb2a91c6e21fd6e9f67bbfecc55a4d Add snapshot 2020-05-18-17-50-32 for release 2.0
7893d8be125e5ccb78ca41f620af9875742ac8df Add snapshot 2020-05-18-17-50-08 for release 2.0
8196f109f1d3a1d975ccda191b4edd5080c94895 Add snapshot 2020-05-18-17-51-05 for release 2.0
2fdadf334ddb675dbfbd5f30f1cf426dabd83c9c Add snapshot 2020-05-18-17-46-09 for release 2.0
d222a2b25d23f65e8d419ec6455880f879a6c909 Add snapshot 2020-05-18-17-45-17 for release 2.0
bc4a760dd6851aa9f1e5236057203d1fca8be53a Add snapshot 2020-05-18-17-28-39 for release 2.0
2cf8366613045187ab0a015ee30daa921d622417 Add snapshot 2020-05-18-17-28-39 for release 2.0
48197b3a9f0e5913f516c7f197d1742bc565bbce Add snapshot 2020-05-18-17-18-19 for release 2.0
42bf6ddfc5e94e17fa976801dbc7fd5abf12e686 Add snapshot 2020-05-18-17-13-19 for release 2.0
a3369d92ce5d1d780cb41cb3756fc6bf5914c913 Add snapshot 2020-05-18-16-29-57 for release 2.0
833b1cae45ece14655c67d3c70c498502f3459ec Add snapshot 2020-05-18-15-25-17 for release 2.0
d0053e7aaba5780eb66e3a3c312291de787a7e50 Add snapshot 2020-05-18-14-19-27 for release 2.0
891bad16bd84eee49799d3724b1aae3fb73cfc42 Add snapshot 2020-05-18-14-19-38 for release 2.0
e2ed447167ec994591eb64fa3a4414ad7592fdf1 Add snapshot 2020-05-18-13-37-05 for release 2.0
fb45b21af218714dd17ebd5c1e4a9f4590015cb3 Add snapshot 2020-05-18-13-37-05 for release 2.0
343ac4d32770b28e9d8a8829634b3e315c9d97b5 Add snapshot 2020-05-17-20-10-35 for release 2.0
16d361061c1ed03e72b9acc623f019377ed7443e Add snapshot 2020-05-17-14-18-34 for release 2.0
bfaeb7f8eef07f900b916ca00d7952747938191a Add snapshot 2020-05-17-14-18-09 for release 2.0
d5f16be972cf74080a0d0702592913df21f8b871 Add snapshot 2020-05-16-14-17-36 for release 2.0
626c868bfde29ef259a8cee812b6e7287c2405f3 Add snapshot 2020-05-16-14-15-33 for release 2.0
42bd3315c4e406d8fa4cbaaf4eee6c4a9514d345 Add snapshot 2020-05-16-14-15-20 for release 2.0
81d1df379608ce8b392ccb27f3db2e988f0f74d2 Add snapshot 2020-05-15-19-04-14 for release 2.0
b2ae27518af5c0167073e7f92b5f93a5fca1df20 Add snapshot 2020-05-15-19-04-14 for release 2.0
56a701f5274812073d116511f410c063de27de22 Add snapshot 2020-05-15-14-17-58 for release 2.0
9cd3e9584d9766bb9a4f90020fabd585b54a8fa0 Add snapshot 2020-05-15-14-15-37 for release 2.0
4c7e4c82764e4bdd063a92d25f3a5138e42cd3f4 Add pushing of custom registry image (#51)
0c89b42c2e1b29aa3af269a23b0cb60e5140d34c Add nsswitch.conf from upstream-registry-builder (#50)
fa718bc6f144e12e9cf8521dfa2b6315388f3f38 Update hack bundle-builder script in prep for tonight's RC3 event (#49)
d894b21d6bdaab708ad5056b1cdfdcdbe3db6be6 Add snapshot 2020-05-14-21-01-31 for release 2.0
bba5b0d1207bf723a2f68d68335344a3cfe796f3 Add snapshot 2020-05-14-20-50-44 for release 2.0
e8498594f5ec3de9c1b23d4b83f08dd15a33fadc Add snapshot 2020-05-14-20-23-56 for release 2.0
18ae299d6aee1e500e24f8cbe08f26f1b78b0272 Add snapshot 2020-05-14-20-23-56 for release 2.0
acfe454f2cb74376c8a43d58a366d3ca07d4c1b0 Add snapshot 2020-05-14-19-59-55 for release 2.0
8aa317c241fe8829678cd45ae5c1ea45dc0a068f Add snapshot 2020-05-14-19-02-33 for release 2.0
b038c8219d8b5c37b276513bdd59be5e36492a40 Add snapshot 2020-05-14-19-02-33 for release 2.0
53bd242e8a821131cb1c5c2f85dc20b2612bca58 Add snapshot 2020-05-14-18-53-51 for release 2.0
0e56ab0e5b8cc78460e718d6134fc76cbe48ef16 Add snapshot 2020-05-14-18-53-51 for release 2.0
b7875034d93a1caa7c3be48a470b4daa4fad1375 Add snapshot 2020-05-14-17-48-17 for release 2.0
70c42884bc7bb1d1f7757abd6ad14b980cc33899 Add snapshot 2020-05-14-16-28-23 for release 2.0
2c92aa59022edb6bf3eb375d303291addb9e0e2e Add snapshot 2020-05-14-15-58-18 for release 2.0
1b69e2c692102f3a83c258aca024c40f89a0fc3b Add snapshot 2020-05-14-15-34-24 for release 2.0
4f2050dd1aedf822a73fd870549ac02dc362d389 Add snapshot 2020-05-14-15-12-43 for release 2.0
aa8646082aee5d2672cb0b0e82976396910be921 Add snapshot 2020-05-14-14-45-21 for release 2.0
7bc9830de37e178d56cd6aad77a281d42ee08d6c Add snapshot 2020-05-14-14-43-20 for release 2.0
817eeb231eebcef4f8ba53dbefd3f79bc58d4ca1 Add snapshot 2020-05-14-14-36-41 for release 2.0
cec0dce1e11c6df25cde0b492bdb0750c660157b Add snapshot 2020-05-14-14-15-04 for release 2.0
fef4804a072d715c1e33ab8168eb0ab4023c66c5 Add snapshot 2020-05-14-14-01-39 for release 2.0
b9c4d1fdc9c2cb5c5656472c20d5c76a13d98295 Add snapshot 2020-05-14-13-49-20 for release 2.0
fc29a811cf6a1dffbf0bbed2c303a379882dbab9 Add snapshot 2020-05-14-13-30-13 for release 2.0
1bc5020936cc6ba9956985e31ba0ceab450b0626 Add snapshot 2020-05-14-13-30-13 for release 2.0
5589727f56d33e57ec6d2245764b13db40cff393 Add snapshot 2020-05-13-23-23-25 for release 2.0
d6b0c172756ac55539f30592e4d38741ffa7aea8 Add snapshot 2020-05-13-22-01-34 for release 2.0
adafe7061937ba4387c10c5ff0509f048e003588 Add snapshot 2020-05-13-21-40-58 for release 2.0
ccc8c8af45285e12fe7862c11ee317328d426263 Add snapshot 2020-05-13-21-26-21 for release 2.0
3fa5c761db53a383357bd60716073ae82f6bc81e Add snapshot 2020-05-13-21-14-58 for release 2.0
12b60f6ce464a622a3e76161e44bd2039811949a Add snapshot 2020-05-13-21-14-20 for release 2.0
46512b028477f31b367a4164cf74d7ee28592701 Add snapshot 2020-05-13-19-48-28 for release 2.0
e5d74857eecf4c7135ba37d20597ecf6b2116f43 Add snapshot 2020-05-13-18-32-23 for release 2.0
1d7420aa452a618775fbea896dbc575dbf9f8510 Add snapshot 2020-05-13-18-08-45 for release 2.0
17418eddd11adacd061562c3bf1e3573252ce63e Add snapshot 2020-05-13-17-26-24 for release 2.0
cb34012728175fcea158eddb99b4fca2e3099d4d Add snapshot 2020-05-13-16-40-44 for release 2.0
d2a67dadf10546487c495c9cfb27cf751658e195 Hacking tools updates (none used downstream) (#48)
faa19617dd066cf87a47f9ab3c4db4e644561af5 Add snapshot 2020-05-13-15-33-41 for release 2.0
d26c5e8a422ad399bc1fbd82846c52d125df8236 Add snapshot 2020-05-13-14-47-51 for release 2.0
e750de2b2a69cc43476da27583148af22cbd0851 Add snapshot 2020-05-13-14-17-06 for release 2.0
070a0983a9a0dae49f712e819770fa48e69b559a Add snapshot 2020-05-13-14-14-19 for release 2.0
49eba889df77939af8948c9498fe3a5a674b8aac Add snapshot 2020-05-13-14-13-38 for release 2.0
1ee59fb5ce614f49fcdcf200d705460d7274bd3c Add snapshot 2020-05-13-14-12-36 for release 2.0
3c664452976bda6b8b3bb3c3cd8e719eeafeab58 Add snapshot 2020-05-13-14-11-26 for release 2.0
c273ae8940ae409356305b39d8498575086a32c1 Add snapshot 2020-05-13-13-14-46 for release 2.0
fb582812c23a98c2850ac04267d986ac0f7d01de More bundle tools (#47)
202edbdc1d4161fa16f33aa42afad2cbbd75bca3 Add snapshot 2020-05-13-00-04-53 for release 2.0
c78c4c3867dcde19e6438c512d2915af5ba8e7d4 Add snapshot 2020-05-12-23-58-57 for release 1.0.0
7d1ab9ec2c5f42bad1cdaaa7ddf52270118e1ce4 Add snapshot 2020-05-12-23-47-53 for release 1.0.0
67b2366ddd1c45ccac4344693ec75a7fb20bdace Add snapshot 2020-05-12-23-27-24 for release 1.0.0
9ea10683d97dfc6261bc18dabf5c7ff1a481fc4f Add snapshot 2020-05-12-22-53-14 for release 2.0
5876837e6556f23527997f0c212d7b346ed697e9 Add snapshot 2020-05-12-22-41-14 for release 2.0
cdf6c4676a2fe8bdf0d4865a11f4c23f4819503d Add snapshot 2020-05-12-22-38-29 for release 1.0.0
845319c90ef491686676435c5223c4bd77a6459c Add snapshot 2020-05-12-22-02-18 for release 1.0.0
7c32c571b013a51b332eb362e2b06acebaf8f38f Add snapshot 2020-05-12-21-17-19 for release 1.0.0
f42263023e9552f934f66efac77a64943850af2a Add snapshot 2020-05-12-20-26-53 for release 1.0.0
b481d4ab7c1781e6486fe875eada57dbfca548e2 Add snapshot 2020-05-12-20-12-10 for release 1.0.0
31463542ac46c9952b5c81a1218f35d83a93730d Add snapshot 2020-05-12-20-03-01 for release 1.0.0
b25c1d0b08107170384a3d33665a14a8a6e18c4c Add snapshot 2020-05-12-20-02-40 for release 1.0.0
96b48fd6fdbec41935acdf3581d696dc591b8c92 Add snapshot 2020-05-12-20-03-38 for release 2.0
7e413abce284ea7deb2213f294f946bcb38f5761 Add snapshot 2020-05-12-19-55-29 for release 1.0.0
8d8f45eb0c2f8df07c055ac578d7c29ff9bdccb3 Add snapshot 2020-05-12-19-35-45 for release 1.0.0
6ae5c9ebe1413fdf1ff234b312b25fe6bd1743d2 Add snapshot 2020-05-12-19-35-03 for release 1.0.0
e1837dd7615277e984e1ea9b1d76724bd08eeff4 Add snapshot 2020-05-12-19-27-37 for release 2.0
4fffe9259f6f52e50982802543b116cb81e26237 Add snapshot 2020-05-12-19-20-32 for release 1.0.0
2581b758f9497d3c1729bdfebbc521987140ec9d Add snapshot 2020-05-12-18-59-05 for release 2.0
57f0ace29bcedcd2c32db0e44c512f255c5096ab Add snapshot 2020-05-12-18-56-36 for release 2.0
734f9e4f483296b2f63f4d5379fa73361d80ed37 Add snapshot 2020-05-12-18-11-37 for release 1.0.0
2b8a871357f42b2f1d24a7e204a24e4817d92daf Add snapshot 2020-05-12-17-53-55 for release 2.0
a7e4903fd46e514b4788c9c649383d95fc5fdb65 Add snapshot 2020-05-12-17-42-53 for release 2.0
53c29840c78928de2e46252b8e4e125692586bbf Add snapshot 2020-05-12-17-19-44 for release 1.0.0
b6964910a356a55e76d8c091777fcf0d0dd72b8b Add snapshot 2020-05-12-17-17-41 for release 2.0
3444a1decd3467fc45bee8def420e73c0a4721ed Add snapshot 2020-05-12-17-14-35 for release 2.0
cdc1d41e10c3118a711980e6e26c41ee646ec353 Add snapshot 2020-05-12-16-06-58 for release 2.0
b3bcc768a693cd1441db765e18b4dd99c9db0ca6 Add snapshot 2020-05-12-15-58-14 for release 2.0
05ef460d373666ca91c79c0f8f31d05db02d67a0 Add snapshot 2020-05-12-14-24-06 for release 2.0
0fb3b77569d510408209d903d8f91ef10d2feb7c Add snapshot 2020-05-12-14-16-01 for release 2.0
84a5b6bf9421175eb900068f3717f9c4b5a041db Add snapshot 2020-05-12-14-13-02 for release 2.0
c5f4fe777a2dbf94d5af9f89ef8a98cac496f04b Add snapshot 2020-05-12-13-53-41 for release 2.0
942815acda9260823c7f5d6eb7e26bdeb43c79f6 Add snapshot 2020-05-12-13-47-05 for release 2.0
7e6856eb0d69868bad0e6a9ffa9efb475e99092a Add snapshot 2020-05-12-13-24-55 for release 1.0.0
b74ddfb1cad04cd98814b429c4c854cffcf31b31 Parameterize version number [skip ci]
a0971aa8b35e15cf0459aeee7e5b7ef50f950b5b Add snapshot 2020-05-12-13-22-36 for release 2.0
67e02ecd6d42d13fbf21dab2a11fa932d17bbc02 Rename snapshot [skip ci]
622e47a74f4c734dbd93c2c23d7f33b98732bcf5 Add tooling to tarball [skip ci]
fea2d38dd1443c652d06f1fa4b710f3469fb2240 Add snapshot 2020-05-12-06-12-26 for release 1.0.0
89adf4c7fcdecfbe00263aac8f89f5cde14365ab Correct git syntax [skip ci]
a0c60d4b39d5ecaf6c66cea08768d06f7d99dceb Add snapshot 2020-05-12-05-55-20 for release 1.0.0
958b9d31bff2fe717665c0cbb1cb07c1abb6d236 Update asset locations [skip ci]
c8f818cdbf0b528fd2c3d845c9156e0c8d6f3e26 Add snapshot 2020-05-12-05-41-17 for release 1.0.0
3d3de2486a989defa5f6fa02e2c8f41aa35d180e Commit changes back to appropriate branch [skip ci]
674727563a5ba0f2e4a789bf12851a800655d236 Add snapshot 2020-05-12-05-15-17 for release 1.0.0
9670ea1bf6d524aee866cf8ef08ae40b9b38ead5 Add snapshot 2020-05-12-02-24-11 for release 2.0
da6112445fd6dd05300626fd71ddd67ace61b8a9 Add snapshot 2020-05-12-01-24-20 for release 2.0
453c3c5229f61c0aa3b94135342a23141482fd21 Add snapshot 2020-05-12-00-05-24 for release 1.0.0
85236d2b572381e7030e11f558f14a3ed3ffcbb2 Add snapshot 2020-05-11-21-18-26 for release 2.0
b48f2333096a57dce5dcbb505bf58b3efe69b636 Add snapshot 2020-05-11-20-40-35 for release 2.0
247c69b4c18dc49f739fc0355157496a8c3e3ed2 Add snapshot 2020-05-11-20-32-58 for release 2.0
6e32718a5e39a010c6313258d0d33e43d265d07a Add snapshot 2020-05-11-19-28-57 for release 2.0
9b3f24eb6d9be634ada84ed2d327de12639857d6 Add snapshot 2020-05-11-17-24-10 for release 2.0
ed47e45c0040c5ad93723cde72321bac840a04aa fix comment pattern
dc4e03b5d09f658a1b36b00c7bc5139ba955555e Add snapshot 2020-05-11-16-40-28 for release 2.0
e2b0a7a2269e7aa5eb3d67b87ab9f91d03e72a74 Add snapshot 2020-05-11-16-20-59 for release 2.0
bb902b8dae5d27ac1d8b8a9086da8556e123c9ef Add snapshot 2020-05-11-15-48-43 for release 2.0
f1876ec99761f73b87dbe29d97c17a63fb78bfff Merge pull request #46 from open-cluster-management/down-hack
6114c1fb91abc9abf3ff9effc7058f5290dbd425 hack for proper downstream blacklisting
c4837cea9594a74678af691c13e85340ab787faa Add snapshot 2020-05-11-15-10-23 for release 2.0
9fce19d136282d11f67a40aad49264769944ed9f Add snapshot 2020-05-11-14-15-36 for release 2.0
a90ed6bb550fec51502f7466ab573f29c994e6f2 Add snapshot 2020-05-11-13-51-36 for release 2.0
34586d804e9b9755fcc9099c03dfb5414e79f5de Add RC2 manifest [skip ci]
5eeb98d2fa8703cb9021e79979af50a209675374 Add snapshot 2020-05-11-04-11-44 for release 2.0
7814060549ed3d26d21d26fc6563ccf8e9f52bd8 Add snapshot 2020-05-09-14-33-41 for release 1.0.0
dc296777628be8cbf78735c1b80eda65f6cc5d85 Add snapshot 2020-05-09-14-11-12 for release 2.0
41d4cc7125c136f68f469d9bc9ea2157dadee636 Add snapshot 2020-05-09-14-08-49 for release 2.0
cfa8c6f5e449f0c8a77ed71bcd29d19acee410fe Add snapshot 2020-05-09-12-35-59 for release 2.0
ebd59c9cae25d37190e1f36ef554c902699e6259 Add snapshot 2020-05-08-21-50-14 for release 2.0
a332f3049efa7c15e023b00c962b0a07b977c249 Add snapshot 2020-05-08-20-30-09 for release 1.0.0
bee89d9bf9e1b9222d1ec14d7441ab4ba8f835e5 Fix ACM description formatting (#45)
7147da178c45217d630e3d67503a7a9511cc759e Add snapshot 2020-05-08-19-15-38 for release 1.0.0
f2fd6ff41d788aa3cd0c75e1934f4e77818d23c2 Add snapshot 2020-05-08-18-57-11 for release 2.0
bd55369731d43dc771f475c63256390f2b455fe5 Add snapshot 2020-05-08-18-16-44 for release 2.0
26d86ba4aa499a425b359f8864641a625b6ddaa4 Add snapshot 2020-05-08-18-05-20 for release 2.0
2cbd0c5f5506c462413bc5ee18028c7ba5314574 Add snapshot 2020-05-08-17-58-12 for release 2.0
26cc5cc920c16f34bef24c50e6455a3668ac82b2 CSV description fixes (#44)
ae1ee7fc2eb913ba3f2506415d680df91cae6ce6 Add snapshot 2020-05-08-16-51-39 for release 2.0
027b9f7e35bcee6a75aba8bb828a5d4f93aaaf51 Fix Spelling and Grammar (#43)
3ec7b362f653dda282998f0b064f423f51d3acda Add snapshot 2020-05-08-16-06-39 for release 2.0
be4dc4d97b720a92b3263cff4d34739395e801f9 Add snapshot 2020-05-08-14-31-36 for release 2.0
6ea1f85ec4cf91a1d23fe3ff28c289d788a8cd1e Add snapshot 2020-05-08-14-10-19 for release 2.0
62aaf472ebb3ab8bd5041170700a1a29ea50c1d2 Add snapshot 2020-05-08-14-09-23 for release 2.0
e872af1cb7d261c6b152cc59b53ac989aef52f70 Add snapshot 2020-05-08-13-56-15 for release 2.0
4dde390d02a681f8f0017fb66cec3ad8d817df87 Add snapshot 2020-05-08-13-39-30 for release 2.0
9a5043fbee62411c22585d7d4cc7d97bbae6c2cf Add snapshot 2020-05-08-13-33-13 for release 2.0
70a82790066c9ba069fe4f7018baf366c12717ba Add snapshot 2020-05-08-13-15-50 for release 2.0
12dad5866c80cf68602b04a3e96f40e353aa2df3 ...and merge [skip ci]
2373e68aad52c90bc64840554ad7b6157ba9e5da Update manifests for 1.0.0-RC1 [skip ci]
aadc657f28c056a52e996656f56a5ffc77405146 Add snapshot 2020-05-08-06-18-15 for release 2.0
b326d4f599597b91f9ebe3f65173614e2a5213a6 Add snapshot 2020-05-08-00-49-50 for release 2.0
108a378ddabed02481448d6a7b6e2fb6bd177693 Minor tooling updates and some hack/not yet used scripts (#42)
3229f3e128ccc5fae381740cd32dc1c4ac2c4870 Add in Chri's Dawson's scription text (#41)
d5b2f2995778abca447f03649d8e362b5039cd0c Add snapshot 2020-05-08-00-26-50 for release 2.0
f09249c08687c5f4cdc1efd122981bac09424a0b Add snapshot 2020-05-07-21-35-12 for release 2.0
7ab99e04de88151a453f9c71810a803f333fa572 Add snapshot 2020-05-07-21-25-29 for release 2.0
128d90ed41c219b3330bd21c1b6fdc9439562e3f Add snapshot 2020-05-07-19-51-26 for release 1.0.0
664a42affc8d6c5b30f906e2ded5e22335af19ab Add snapshot 2020-05-07-19-29-19 for release 1.0.0
99a8e7f4ff9e6b4797be3a7e600dda0bd277ab50 Add snapshot 2020-05-06-21-21-16 for release 2.0
66faaeb0fc36a8ea0e6a071519a7e3d4d86c86e8 Add snapshot 2020-05-06-21-16-38 for release 2.0
c33c8302aef184b772e6758dbabae8aad10ab262 Add snapshot 2020-05-06-18-53-26 for release 2.0
cfc83bddea377a421868104de63c0ad77001e60e Commit latest manifests (#40)
9dac283a555e9ac555c8fb7251e30f0ec1772b50 Add downstream.sh (#39)
d06f40be7ecb5a5afd2020e0986bfde219d5fce1 Add snapshot 2020-05-06-15-36-49 for release 2.0
0d552e90182199ab0919f1bf8e7e4c6c0ca706fb Add snapshot 2020-05-06-15-32-48 for release 1.0.0
b6869b979a32850f29151807b307f8d3b973481b Add snapshot 2020-05-06-15-18-37 for release 2.0
53e42412b24abdc682a5eb4708a558eaac918aa9 Add snapshot 2020-05-06-14-19-10 for release 1.0.0
8f6a0efa452e13e3a0f79a0702360b9134650568 Add snapshot 2020-05-06-14-08-58 for release 2.0
65b6b6c0d03405e73dc80069c9dc50e25bfa72b5 Add snapshot 2020-05-05-21-51-23 for release 2.0
050240095e843402ed9abd74c12ab3bb252d447f Add snapshot 2020-05-05-21-31-28 for release 2.0
02d451d47077f6cc69484c7d39eeaa353716b9e7 Add snapshot 2020-05-05-21-09-27 for release 2.0
a55c9a04a19c4a42ef7093d4bc687cb15781492c Add snapshot 2020-05-05-21-09-09 for release 2.0
eaab1a647dd4ee6495b6c446a6529647ebf1ed38 Add snapshot 2020-05-05-20-27-29 for release 2.0
b59fa8e753f412bea453c7df7f019fa82359114d Add snapshot 2020-05-05-19-43-39 for release 2.0
98db5149077248e58cbd12fd7c810abd9750a9ce Allow rgy and namespace overrides when generating bound manifests (#38)
3b2015aed52a8682b03d33b1fd73eaeef07d8d37 Add snapshot 2020-05-05-17-45-50 for release 1.0.0
9c20ce2bf003b13b58e7d80c0ab5e35b49350b0b Add snapshot 2020-05-05-17-13-11 for release 1.0.0
d816155fa6989a0e390c942b3855d689da49103a Add snapshot 2020-05-05-16-22-13 for release 2.0
da06ec354956e6ea7f4ecdc22808dfefbb2f9a6e Fresen unbound bundle manifests (#37)
3f3697381bbfbc11eba93d98281527500590d497 Add snapshot 2020-05-05-15-39-13 for release 2.0
ce1d8a3c7fa652149a26df8bc649e05546a2f3db Add snapshot 2020-05-05-15-38-22 for release 2.0
172e8769e86b4f6502bc36b664acec3da2ea3b7d Add related images to bound ACM CSV/bundle (#36)
8fe62b8cdfa2d88f2b3af1eaafeca2b27d95766e Add snapshot 2020-05-05-14-49-20 for release 2.0
5198ac0d4f869523942fe1425af661391940c031 Add snapshot 2020-05-05-14-42-45 for release 1.0.0
4380263fbb6504de7d0d3444b492c25432302791 Add snapshot 2020-05-05-14-42-45 for release 1.0.0
c0974245d12f823ed7b02f8a719f8ff35d0bf84a Add snapshot 2020-05-05-14-22-49 for release 2.0
e3abeb665f1d67e25301e90d58c90264cb9e1137 Add snapshot 2020-05-05-14-14-43 for release 2.0
f48816ab8cfece6edba7dcd6f77bedae5d796e1f Add snapshot 2020-05-05-14-10-18 for release 2.0
f2039b89205fac2821bf3415d325d4b90fcd8c0e Add snapshot 2020-05-05-14-03-27 for release 2.0
c078bad55ac44a3a63f52f2c7ba2d1188c718ef2 Add snapshot 2020-05-05-13-51-14 for release 2.0
4da1dfa521ced4c24f02d9434dbebe46d9d65363 Don't merge categories, use value in CSV template (#35)
d4b83422581190ccc2962d7c583f563bc7ee56bd Add snapshot 2020-05-04-19-26-55 for release 2.0
df3399358ade673585689e863bc3560dfbfda7eb Add snapshot 2020-05-04-17-43-49 for release 1.0.0
9b81c506aeb64b22783d0b88dc4b64c4098da980 Die if image digest looks invalid (#34)
3731da6c1ef444fbedbf96e7f0dd3114cc04246f Add snapshot 2020-05-04-17-16-32 for release 1.0.0
dd5549c8f7242105233e32fd43dd93ff3e8b30b9 Add snapshot 2020-05-04-16-00-12 for release 1.0.0
6a2b880d682125e524ab7f3b8abda86d79c9d040 Add snapshot 2020-05-04-15-52-30 for release 1.0.0
f4559a2ae4d2fa68921a5ff88a388d2005bbfedb Conditionally push index image [skip ci]
579b7ed2cd45ff4e943162440d5d31d7012ad851 Add snapshot 2020-05-04-15-36-32 for release 1.0.0
8252e6690449787e2927be0fb2c2281377adda3a Merge [skip ci]
12d7de33386853b5dbc02c087e80b7306e1f3cd3 Assemble tag name [skip ci]
d7b3822c398ccf249d88e157851c4cba1819e232 Add snapshot 2020-05-04-15-30-07 for release 2.0
92bc20146cf0b4804e1afae188feb6bea043d113 Add snapshot 2020-05-04-15-21-48 for release 1.0.0
9c0f49d8836f01692fbf947db808c6bf4723ba9c Merge [skip ci]
f5aa3fcfa71ddab0adfd23ffd0ae1e9ec64663dc Split images out into their own stages [skip ci]
3d5665de9a3f0d3d4baa46658262713a07d5ddc5 Add snapshot 2020-05-04-15-09-50 for release 1.0.0
2bf5d6a89d57a75d7a39d3a6fb685edd8ffcfc74 Add snapshot 2020-05-04-14-58-27 for release 1.0.0
62f1ebfce34234478023e2bead55f5785eac34be Add index build [skip ci]
4aa978ef652ef48e4285d76f7b1e17716414e018 Update ACM CVS template and current unbound bundle manifests (#33)
8773ccec190e9a9dcba8a7b7384c2a7658bc2c53 Determine publish channel based on bundle version syntax (#32)
8c08df277985f3ccd77e92590c80800c935babd4 Add snapshot 2020-05-04-03-56-11 for release 1.0.0
a190aae7871f49e9319b17cb0dd96d6cdd44fcb0 Add snapshot 2020-05-04-02-17-59 for release 2.0
aaaf88ecf4abb2ed6f3092da61879ea14a7da380 Remove pull-secret refs when producing bound manifests (#31)
743c3c249cd3f6e23d81ded19c495b22b19d5459 Refactor: move manifest processing down into create-bound Python script (#30)
a5d45669e24c2c6ae808cf1fecea29032255aee3 Add snapshot 2020-05-03-14-51-14 for release 2.0
728a2c3fab8cf70bae4434df5516894729624753 Prepare to remove pull secrets from bound bundles (#29)
79e15ebfd6b6cfb0801c0f1c49393404940d88f4 Fix missing description in Hub CRDs (#28)
770bc106be11a305ffd3cefd80704d515df556b2 Add snapshot 2020-05-02-14-18-52 for release 2.0
772b9a172ebeaef85a1e4c7b3c27c5385090c7cd Add snapshot 2020-05-02-14-11-24 for release 2.0
b64c80514db1a6cc3eb1ed3a982c2ca61bc95632 Add snapshot 2020-05-02-14-09-38 for release 2.0
78183f3f921e83bd62e40f3a43667b9a857a7bb1 Refresh unbound manifests (#27)
35502a32fa7edb5e21f636d4195e1cf065d43804 Hack hive entry to corresponding to v1.0.3
9c8b217b8d5420eab5d5db42f3af859e7505f758 Bypass manifest issue: add manifest for SNAPSHOT-2020-04-30-22-40-54
2b259e9394d3cb72aefbdc30190e996448acce50 Update README.md
2a7e8c9907c3ff4168c2509ab7758df7b47ee8d0 Fix issues found in first ACM CSV test attempt (#25)
3c864d8e9cfd36e2be0c7572b45881e6a078cf79 Add snapshot 2020-05-01-21-53-41 for release 1.0.0
49e4eb71f993eef2cf39ae12c3bbb71c1d05c1be Add snapshot 2020-05-01-20-59-12 for release 4.5.6
378a45a6d72cd0315758a1d138d509c2312774d9 Add snapshot 2020-05-01-20-50-04 for release 4.5.6
23c5d2076757fc1a97054dc224081a148bc87aa6 Add snapshot 2020-05-01-20-43-26 for release 4.5.6
47f3263324ccf9e698f7fe8d34d5db0534ed2205 Add snapshot 2020-05-01-20-28-52 for release 4.5.6
96cd22ad2a033b3f68d78724d3c55caae7134517 Add snapshot 2020-05-01-19-33-12 for release 1.0.0
99661f72c72b731ca6230049f33686506ef16fa7 Add snapshot 2020-05-01-15-06-32 for release 4.5.6
12ce83fc8d3d7ec10d66d2a39faad75666201959 Add snapshot 2020-05-01-14-54-41 for release 1.0.0
d467e45a21206f20da244cb3843a8af47fcd9a36 Add snapshot 2020-05-01-14-49-13 for release 1.0.0
a2051f1237f65642d1fe519ccec395af2ec0ae7c Add snapshot 2020-05-01-14-38-26 for release 1.0.0
ec1c0f38b2ad602bbd610290059b54b3581a1c1f Add snapshot 2020-05-01-14-27-10 for release 1.0.0
d8eff90afe35fe85affa328a75940e86ceebbac4 Add snapshot 2020-05-01-13-55-39
8c72ed494c950f9bd95f4c63ed9b9302573b094a Use new OperatorHub icon (#24)
34c9c827b7a2c9269cbbf4afd5d2392819d8cf7d Prepare 2020-04-30-14-15-23 for building
e5ca8febd5f093ed4d1554f7ac52c635f16dc47d Refresh OCM Hub and ACM unbound bundle manifests (#23)
83b4376682b6264b45f99f663c5d935606cf29be Update invocation parameters
e5ae2318c09328ed6a007022cab85656ca0ad10c Tailor image name
aa2b98b2aec065ff7bd413478d668ba41a02eac1 Correct syntax for shell conditional
1774e08ad0a462d126cc03ba506390fddf87c438 Update invocation structure
d8251b251184043303e24f1e79fcf939ad4d1867 Add parms to bundle image gen script (#22)
acb00c625c970f0ffb991568ed398fbc0cc7579d Trigger build
d954b44ae243ee7ffcaef8c8bc3f219c6a97202e Travis won't allow use of --squash on docker builds (#20)
504b4e44aea25af5cad9e757fa7d8c80038e7bc5 Refactor to gen unbound Hub bundle using scripts in this repo, not Hub repo (#19)
68ee8f4ea0df0e902b2636f6b3c212e50018c2f7 Change image key for hive to openshift_hive (#18)
730dcd3c59a7f5317f111de7925a6441a6425bfd Trigger build
4c88c184542239a9764f48e9ad5e8b0542d98697 Add script for getting operator image ref from a package/bundle (#17)
215fbbd4aad8e946f621a9f903f1e5a61113571d Remove some dev scaffolding msgs (#16)
675b00880296a8626956daa9c14d8b6fb4326bc1 Change to using HTTPS with userid/token for git cloning (#15)
64d5c0214ed74e6c6c847669eabfe7a660700450 Fix some CSV format errors, bypass others (#14)
20cabfe64f00224a70d604f6af804de864f4e1fd Add v2 manifest
ce77011ac951c5e8368a37390c3d8a467c47da02 Add pyyaml to requrements.txt
7ed5162ab996bcc8b920a26652e301e0107e72d3 Bootstrap release travis build
6454cee4d0e390a00e60bd0a4022ebbe2c74a71b Get rid of unneded use of python2.7 (#13)
29597a05d75ebb5ad874afffa746ebb33206dd4a Remove accidentally commmitted test scaffolding (#12)
fb7f70e3642023a490848b86f3726d5fc23127d3 Update ACM CSVs with real doc link (#11)
d27fe1e47dbe94c2f5203737c69c4968be4eec29 Create image and push to remote registry (#10)
00866cbc1c781c025e3f27b78d178c21cfd74c81 Update ACM unbound bundle to pick up Hub operator changes (#9)
938388cb64afe9d11dd38444de1186884d36c013 Expect bundle manifest in repo-top/image-manifests (#8)
b0edabfc9bfb07decbdfa505f10ad7650f2ae8f7  Add some bundle image labels relevant to downstream handling  (#7)
27ce40725a3bd0a33a938d14e66ea527fd69a7e6 Refresh unbound ACM bundle manifests (#6)
ca97d3ad7a8c7e73f1344af33ff03dc5a6b308f3 First draft of ACM  bundle image gen (#5)
39e334524d07cacef394115f32dd04c71b294b1b Refactor bound bundle gen cover script (#3)
9d2b393961b420484aedf7d19ae8ed33aa4eaa48 Add an initial unbound ACM bundle (#2)
034c40a0ecb72eaf894d43e372e907f55d26f995 Tooling to generate merged ACM operator bundle manifests (#1)
ac2c8a458e09ad1862d97614c77ebf48968ba603 Initialize repo
```

Status: Syncing successful
