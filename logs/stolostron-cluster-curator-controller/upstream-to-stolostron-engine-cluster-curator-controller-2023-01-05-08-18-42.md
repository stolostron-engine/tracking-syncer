## Syncing stolostron/cluster-curator-controller with stolostron-engine/cluster-curator-controller

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 137 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
99031ae51291255b5c82af5d007d99093d8ffad0 Merge pull request #146 from elgnay/fix-acm-2531
7f792311f38a352bc170ffd4780f1b201c05900f update the clusterdeployment failure logic
7ce469483c993629c5618309c2ce53ab49e9ea3d refactor installAttemptsLimit with pause annotation (#143)
da2350111baf8c6831d03f4409adcf970467a791 If the hook type is Workflow or the job_tags and skip_tags are omitted or empty then the generated AnsibleJob should omit the job_tags and skip_tags fields. (#142)
1556a39eb4903cf67f4538ea98a23a934818a38a save upgrade fields (#140)
1d827d1b6a2f95754124c45ae02deb76baa75503 Add AnsibleJob job tags and skip tags support. (#141)
967b8d08ab4951e9cff3d262411d2ed8c6b46923 upgrade hive to mce-2.2 branch (#138)
4aa578ea77f954b91e1b896e4d6f035464298216 add monitor timeout (#136)
3964e5e0d3ca6e768b40e4e6a82e5307cae6298b Add HookType to distinguish Job or Workflow. If the type is empty or Job then the controller will create AnsibleJob with Spec.job_template_name as the key. If the type is Workflow then the AnsibleJob will use Spec.workflow_template_name instead. (#137)
8f9612ecbd7e8cfcba4c1aced8b6108d48cc405c rollback golang to 1.18 (#135)
1c539b226882d62512329fc21eaf0ec89cb1cad7 upgrade to golang1.19 (#134)
c70296e77d79c82dc0d58a13a7d18aa62e71b1d4 trigger a new build (#132)
e8189bc0b490125289d6997f5acd92efcdcf0fb5 upgrade go libraries (#128)
d4a21c958ff6a6c72ff4bdb14e442e70a0a9f4af upgrade hive (#127)
4f6e82fd273fc7557d05b79fedc6b027e31fb889 upgrade hive (#126)
424d90861729be8b1eb5d9212bcceb4621356326 Remove ns deletion job (#115)
2214786fbdaedf82088fa7cd6854c76009fd6de5 refactor with clc api (#124)
13c323c1be609473982214225857fa54de73c679 Fix compat error (#123)
79fa6cbc5f53eb488122390306efc8ba93b2b389 add inventory to curator spec (#119)
d9a00e406078063f2bb028606f0e59d8e2e57a92 bump go to 1.18 (#121)
3577683c5beb6ebd216938580c697b051229e569 Improve coverage score (#120)
6977234e6a68c1994b367ced4655b0c9a7424089 add cluster info into extra-vars in upgrade job (#118)
d6e54d4cadafa83c0d1c567ae8cf760b0e9a0c68 trigger a new build (#113)
d128d1ddde1db04ec61b5a7fa43fb95891778a5e handle error in retry loop (#110)
cf5de683b9c07365ef3d408af269bcd57e92715b upgrade go libraries (#109)
3876ffb0eb892f8ef9a3e72fb46bef47cff4ab01 update dependency (#107)
f1bc9885cea7b54ad6832e04181cd9ee111e81ef upgrade hive (#106)
bd18d0532ef624caacbb716babc7f3d09a10af90 No-Op PR (#105)
bed372c3d4943bf84188814278c0e1ec4bdf2d58 set tidy compatible version (#104)
2b006a75a67bbdb5ac3e1095d37d546a89acfe52 enforce to use the latest ocm api (#102)
e4b8e5c35bac6a17e9ab970504d49665f6788534 fix missing dependency (#99)
b9c8fb48e071039a665f585538e8e19eced1d3bf org rename (#96)
3fdd42e04564fda9e11bfca2d385fc7528948b30 fix CVE-2021-43565 (#93)
a8cd4d08faa1db52c1917ef2403cdcfbefeb80be trigger a new build (#92)
ff9d46142a14b8ec56ef5f306ecbf4eb02918460 remove unused variables from Makefile (#91)
5f2edc37f19e00ae620937511415b7169f9dd833 trigger a new build (#90)
b9016d14dfbbfcbc5fb4224188604e2dca07f122 upgrade go version to 1.17 (#88)
9d7aec8e49eb29a2802740dc8415dce1b0541507 upgrade hive api (#84)
7d0e0d97b94370eeaa5b5620e0b54bf2ee672649 trigger a new build (#83)
8e2357627d18c01b112bfcb8de8f22cf043bb2de upgrade hive to 1.1.16 (#82)
8e7893aeb582c0893dfa8daa5baf24eaf4e8fa82 upgrade hive to 1.1.12 (#79)
4051a333a0b0475e4569bd76d40bae12dba09115 remove master reference (#80)
0896bf83a514611ed66d43583d4f54d4b62d5ac0 update component version (#78)
fd2083c37ea00bd8c565d0b54d5b474fb5f4fbed Bump go.mod to 1.16 (#75)
0e1bd745e9254b17bc97c663ad6b1c595347471d don't run pre post hook for channel/upstream upgrade (#74)
fe4acb82819d3bd7c8ea4fa1c0cbb27edfce5c5b add repo owner (#73)
128dd3944d169d97a071ad50233ab2bcf821dfb3 trigger build for imagescan (#72)
2ed65233860ff9512fbae72344f160cc5097c998 add desiredcuration for successful job (#71)
d98a3254d2cbe742b30d6b3bb642f6a56fc5ff32 update curatorjob status to add desiredcuration (#70)
a3597b87696e9e2a60d6ec0f2755a139c21890d0 Opt-out of sensitive keys (remove when found) (#69)
2c75f49c836962a45fd1fba2be83188d36a4a61d Bugzilla 1961123 CVE-2021-29482 (#68)
f17282fe0c6b0362c6ff47c0d3f62fbe7dd87daa Include install config (#67)
f27bdb74a189ca07ccdc6902de62df475b9afd87 Replace machinepool with install_config in extra_vars (#66)
98eba04e8cd75f7dcf6334e6224f2ba057770ddb Destroy curation (#65)
6405293a47404229f3affb7efae65ef1d5e3184f Change to new PROW multi-arch image builder (#64)
05907c7b6455078b7338c1e60e047d474cc2d7c3 Increase the timeout when looking for the hive provisioning job to 3min (#63)
2e885c8a1e4a919bbab59de1133986ca4d0f85c8 increase monitor upgrade timeout (#62)
eaf7647e004a40d2c9c70fd111752f4be7bf530b remove availableupdate check from channels (#61)
7edace98a0be19bd93a4cb4e7f2839a2f327527e Channel validation (#58)
270583b9f07b436755146d77662a7295dddb97aa Fix loss of jobChoice after activation, while monitoring (#59)
a36c49d10b9e1064e5981e3e10e72fea2fe5980d Ansiblejob status url (#60)
766b5fc2f895d85e96d46089c660c6be4012d345 add % in the monitor-upgrade status (#57)
3a4c5cd448fef8b7bfdc8b24941dd9470d1710a8 support only channel update (#56)
b96173f3548372c1235ce3841c40af3e65d9999c add label on manageclusterview (#55)
04da1cd8ffe78568e3a36b6936aa37b358d41ce1 trigger build (#54)
d4fd2902ddd0f1aa68152f1bbfcc51697e42dc01 add validation for channel and upstream (#52)
32c8af27686bffca6fb6ec8e737bd48de1d65b7d add kubejob to upgrade cluster (#49)
dfc7859966f398440e96b8e2663495724e422426 Add a clustercurator-job condition (#51)
092904c0d7963a76c10a5e21d51d9d6dfef39727 add towerAuthSecret to clustercurator (#50)
69d49c3c3fd77581115f97ddb315cbfd9ffec043 Add scale test in dormant (-short) mode (#48)
f3f26ddd299a5d04b5ea5c631f7312b40c470001 update crd with upgrade fields (#46)
d7716276bcf16b3eb577397d247faa29c7273e92 Extra vars: Include clusterDeployment.spec and machinePool.spec (#45)
0c79943e3969e3e6b7b5c645e448abe82f55d08d Triggerbuild (#44)
2907395a8de36e565f203c039c772a9302d340a3 Sonarcloud fixes (#43)
0b8846de27d7565e461fd5f7036353e55485d981 Cluster curator crd (#42)
231d5137282063f90c353b87ac912400520c9efd Fix leader election rules. (#41)
1249f627581fcb9af808fb016ee8d8e8cdf6829f Fix for downstream (#39)
1467c8d5b1f007060ba09a349d92a1466d44f44c Increased Sonarcloud unit test score (#40)
c44d1c9682e2db9f8b3339e5ed361363aeef1b31 Add container resources, stream line job reference, and remove unused param's. (#38)
a6207b9fade097604fefe5c6fe6b28442ade05d1 Remove template (#37)
32fa5723acd9b4d1bda0e6445069cd12410622f0 Check error sonarissue (#36)
9e133a0d47e3de32ee1a6a74314eb6e11b758f14 ManagedClusterInfos monitoring (#34)
9d6fd1c81e80502beced595d8b6c9b7ab157eec7 edit (#35)
94b5d6204596de3230cf50ed2cab68f010ef8dd6 Add the correct upstream image (#33)
825c678462536c01ee79411bab2662219b309c32 Adjustments for image-uri, no more tag and sonar-project (#32)
2fc556ca59b2437cbf563370e27728a477a444ab Add a line to sonar-project.properties. (#31)
30b3d4ae455bda2eb54186a19217ea2d3e60c7ed Update copyright (#30)
96e7a4ea7eeef1143cdea7abe5e36c8045c47071 Add a test for Monitoring Hive ClusterDeployments (#29)
4ebfc2bee98ce8b9cf06c34ad51572e81f352ad6 Add leader election (#28)
d9436edfaab01ee6785c9836f1919b8a63055ced Exclude controller_test.go (#27)
3bb3d647379e68e77d6d0417b920b2b166290d32 Helper utils tests (#26)
d66c74c04f540e0cd68b5c357db95d0c397f3b9c Add tests for helper utils (#25)
340c6b612be33e403cf5333adba66a8aae425ac5 Fix ansible test failure and missing make cmd (#24)
02102ac27f610f802d57106de527536e1faa71f5 Do not attempt the scale tests (#22)
710eed18d42ba817e0ca344d35ed4b397719a04e Scale & Rbac tests. Pod resource definitions (#21)
6893626d2da0521946f5f4da58aadf787d56c9a5 Ansible tests (#20)
e8b286f95e99ed5d96f8a97228149db7555777ca Import tests (#19)
a80ae6df6236ac82a93a8a73545689d0225c2434 Add tests for Hive Activate ClusterDeployment (#18)
14969e7e5a316bbc635c538251696ac9e2c347d0 Remote clusterDeployment create options. (#17)
d19895c96a9c9102e685fa1060079d99b3a465b0 Add secret unit tests. Adjust README.md (#16)
577a82d031ce313c7d89a96b0643c7c44fe7046e Fix the final sonarcloud warning and adjust AnsibleJob status monitoring (#15)
aa8b757d0ad0deb892b7abf14e0712d0612b978e Unit test cleanup and init (#12)
899f0fd3f14b6c274b1cfee98fcbc68a55a71484 Additional tests for controller/launcher (#11)
3d72ba6e04592e8992f61b6620b0224c3e8941e0 Controller job tests (#10)
eefc27ae2f36767b72a7045fc5314bba11d544f6 Sonar fixes (#9)
9736a3cb1365dbd77aa4f9b1a2a19b10b6279bc6 add eol to last line in sonar-project.properties (#8)
fd55ff36373be4b31a62e2eeff2f677f90301ffb Update to generic copyright (#7)
e4230050ffb8570196668fbe1ebed66d447498ee prefix the deployment with "cluster-" (#6)
1c3f9b301579bdcef0bd54ac20f4179d246ec9f9 Merge pull request #5 from jnpacker/arch-diagram
8efdc070c8a8ccb4d399fa9a645e4f5685c96202 Update controller name
91bf7ab58b962ca90b10c5d6fc6f902d93ea6fa4 Architecture diagram
e35de5b6f708cdfb199f4b9bf537725e120ab254 initial prow setup
1a76ec4c1e9b6a6bba53bd54f98aa25de5585eab Merge pull request #4 from open-cluster-management/add-creds
7f861b72d33f865421487a7604e09352e519388e Opensource requirements.
3385bf0ea94c3b8192bc5a4e9ab0f32f1c22ede1 new sha256
989e68c42372f6de2f0ec5db2aab0c1bed8854db Use @itdove suggestion for Launcher, as re-use kubeset a little more.
edd387bb5e8a923932a5175576d10d89f5aa7459 Move variables out of getBatchJob
1262f1d0112ff3aba246d149274ec7dac27ee653 Applied comments from Pull #4
cad9d81a5ab49501496012ad072b5917c27075e5 Applying Leena's suggestions
ae35379de7709fbdc9b87d3c4bc28c656d4aaadf Prepare for PROW
e5d418f3a39c00ac718cc9f432a27b294caeee15 Add support for mutiple jobs & extra var support. Jobs are executed serially.
d8229526cecaffdea2a0aefac21b7627cd3a5172 Add GCP & Azure credential secrets.
d31b90973d09bde0da5b94b418ab2f20a85bc1c0 Switch to klog, remove panics from the controller, fix the deployment.yaml template to be yaml
6eba899e31c09ae13009e600d51a26d16e5566d6 Fix PROVIDER_CREDENTIAL_PATH
bca6302a25c700e16db5e1d7f250d5e7717512f8 update readme
18c36426693db029570c3da6a654ebda0b178c93 Add PROVIDER_CREDENTIAL_PATH and update the README
abdcbd5c6cc48b935e6954d7c6ee8aad126b3bd7 Allow the environment variable for PROVIDER_CREDENTIAL_PATH
8bc339ef9f506ed9716f2b92e62c02d5cfa6e85c Some clean up of oc process template commands
18278ebb5c326378f81324af7b99609b693530cf Further prototyping
754f7b5e4134babedae45898d5f17de16ee8d51a Initial prototype commit
185bce3f4d8de2c048139a72da617f9e7f300da5 Prototype for CloudProviderSecret job (AWS)
06dc558980854fd17749503d804061fe21bbc844 Update api kind and crd (#3)
bfa64b947642baec897b60dc6164719f8f3d4a3a add api kind and travis setup (#1)
93b5b4cd18a66dabc44d72c3a0c2cbc83ee20716 Create README.md
f81dc95370595201d33b55781311f5d92caa9c05 update
2bd22230057ead38220d07a003c1b15af9e346db edit to type_go
192bffb680d5bac88c736e0ab1fece8091ca6c5f Initial commit
```

Status: Syncing successful
