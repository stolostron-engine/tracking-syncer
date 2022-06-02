## Fast foarding of stolostron/placement into stolostron-engine/placement.

## Status Summary:

backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
1e52cfdf4add52cbbdeacdf948aa99119be2dcc7 trigger build to fix cve (#19)
27e876570b7e48407c7a706284fa53618422a3fa Update golang builder in Dockerfile (#70)
18273829d8bc745d7d74805bceb6f043a4a1ae13 upgrade go modules (#69)
a77fad3f295438d118d376743b08c2beda4c9e2c add changelog for v0.4 (#68)
cd1afb4af1271752b794bdc0466601fbbd59ae47 add more UT for taints/tolerations (#66)
ab3d8b4441d0c595fce7ddcb6a5f28fdfdc8f794 Avoid building latest image in release branch (#67)
33be032d73e0df8c2144902724ba1d75abd25a91 requeue placement when toleration seconds expire  (#64)
aa32f623d7b6f468f9c76261f08f2a71f121b85a support legacy clusterset  (#65)
2152581aea98edca9e3e7f96edece40f6575e5ed Add filter plugin taint toleration (#63)
9898dbd56be5892c8832accf1eaf64369929ddaa update placement and placementdecision api to v1beta1 (#60)
3b92008154433f41c3c652a3a8cd11e2cc0c7b58 add changelog for v0.3 (#59)
137f8cab3fd586b6405f9b4c07626b187a2f20cc add resync controller  (#55)
61e8e4d8b73f36b966c109c53286fdcce95a3112 fix CVE-2021-43565 (#58)
872fafd2989aa4ed26a5a30e5383f762c2bffedc upgrade to golang 1.17 (#57)
d13d0dbe48a6b5757c3b7f6e320c73cfe531798c placement extensible scheduling (#51)
0780b9ddac021d62ab44c91a8988d94b1029a837 merge functions for performance (#49)
37993e413b6546017167d59f37ee6b0d42ddb194 Remind user to deploy placement controller before running some test cases (#47)
bf225de491193ff312f3fa33c728b68a71dd3540 add owner (#48)
0f74167126e0fb4e3df21626b407749703419f17 add doc for scalability test (#45)
7db4f6194a4945853b0212fffd18d0b00428d582 add scalability test for placement create/update (#44)
4d799ef0511748f01957d6ed44a457d68c154669 add length check for event (#43)
d08b95abe2f26e9bfa4d6570c32c1bb7651a6d84 add scalability test (#41)
a0e134ebee57e02ea10b6b65a5d3fa8bcba4a5f4 add changelog for v0.2 (#42)
00a0d597a3ae336bf053a5e6a8c12c3338216eab update placment when clusterset added (#39)
c6599116263687549625c2f8e8e3fc7303c97aa3 Merge pull request #38 from haoqing0110/br_prioritizor
d8bfca592f377b0c79d31a52ddcdd55fab312763 remove prioritizor ResourceRatioCPU and ResourceRatioMemory related code
b9eb5872ae1603d0b3d4a5d3e000b59be9849d8a Merge pull request #36 from elgnay/update-readme
e9e39d3728d0ab104993de77a0108e13217f39a9 update readme
67f5ef663a277633a8b175de34805d95b6472658 Merge pull request #35 from elgnay/upgrade-clusterset
9307989329c9dfa42a29cdee026097e63d30c5aa upgrade clusterset
4983cfa6c2a92e3ad20deb85455d6adf55d32b5d Merge pull request #34 from suigh/09141622
7bfe2e7ae44b371a9791a7c2afe347488b129362 clean env after e2e test
961e1584af341561c1a3507c5de9306ff507591d Merge pull request #33 from wangglbj/main_wangglbj
942115a126aa572e5468ae42d0c2c8b4e31d747a Modify the incorrect format of sentence in the README.md
86c46b9156fccf2361880ab0b9fde75a619dbf19 Merge pull request #32 from haoqing0110/br_resource-schedule
07e3bfbee68ae840680e8ad616c9e5016fde776b add resource based scheduling prioritizer
b07c8d354f23c3d36e4308443ce6e7e8fa25fb21 Merge pull request #31 from haoqing0110/br_placement_prioritizer
2d1f7c301a212e43b830c13748ad089a243be904 add prioritizer with weight
38d7baa6c5d99771cd04d870d5aef465c836ac76 Merge pull request #27 from vincent-pli/avoid-forbidden-log
7f1e971474eb20e5a05203e33e7d7709e2d2f062 Merge pull request #29 from suigh/08181828
2bd2cb135b3a94fa70b41ef85b21be5df8708282 update the sort logic
119a651bee6c23171887954658a3b775a4bd20e4 Merge pull request #28 from suigh/08091731
ce545455630f19d7fa8dbb516a301790a0518927 add output of status to the readme
50febab1c3736bfbfc638922f7a74e51affb6da1 avoid forbidden message in the log of controller
f3b0086f797a235344aa799b344f78c4192575ae Merge pull request #23 from kim-fitness/main
21ca3eb82682f36b5e9cd4d123a884e123afc420 1. Add a new step of cloning repo before building the docker image 2. Update the .gitignore file
7a6c1dc670c42433ed342c5adb89cd7fe16073a6 Merge pull request #17 from qiujian16/plugin
148623f8609cb3e4a297923c1f387fda66333134 Add debugger endpoint
ab17aad3d362243b3e5a96fa1f09c039d6108e3c Merge pull request #22 from xunpan/doc
10340f1620c731a38d37ebcffa560b19446273e6 add lost step in making images use here document to decrease user effort in first try
4004e354fa3f5dc447a81664496969f97cc9577b Use plugin to support steady/balance
f77087930fca06290d78626f64dbf9c1aa9b9901 Merge pull request #21 from elgnay/add-more-e2e-case
447e95629380a3a8fb2b032c705ad3bffb501b5f add one more e2e test case
dc4e489035d359ec12ef2865a74c520a45380f88 Merge pull request #20 from suigh/0726
e938b25d1af8d09e889acf050c2a9d2c1d7e8a40 remind user to remove proxy
f6dbed9b420be722b4e03296c28ab9e231d7745c Merge pull request #19 from suigh/0720
a633609cbff36196f6c39630925092069161579b correct the path
26fc7dd6a4ce23a63aea7deadaa5ce8e7c784214 Merge pull request #18 from zhiweiyin318/release-job
110a248c3c554b61bf0f117cbd0522ef0e0028b6 add release action job
eb89113408a3fe8f22500a23d541ba1a07b14f31 Merge pull request #16 from elgnay/update-readme
e708709643efde753f1eced8767c7e63edf33df6 update readme & makefile
b3323dab425f9beddd7b7674bd6e02e79a66232d Merge pull request #15 from qiujian16/update-deps
81dd4ec841658d853aa3cef4580e0abe925173f0 Update deps and actions
796a2664991fb67e63e0167cb25f68a5303374db Merge pull request #14 from elgnay/issue_13120
08b26501ccfa926bd2069aed4fbf90cb2bdf4059 add more condition reasons
e7dafdac127a177770e2dc156aa8e6abcc1a8c22 Merge pull request #13 from elgnay/multi-pds
577ee8339472013694fb7f385f495f3ea5a09e4c support multiple placementdecisions
598002e18f02d6df48c6f8fcd5089c9e88a0dded Add condition for No ManagedClusterSetBindings (#11)
d8305f08a72e579ad1706c06a9e73b45f57ef415 Merge pull request #9 from elgnay/add-event-sources
f5b9c319724389224aebafe60085a7b85779ab70 reschedule once cluster/clusterset/clustersetbinding changes
2a71ffaffeddd3ee75272632f16a94372ffaedc9 Merge pull request #10 from elgnay/enable-e2e
cf967a313fd0be98b7dff3faf4d68a54aa2da70a add e2e test cases
47127df16cce1387298c8c07815d32352ce84174 Merge pull request #7 from elgnay/scheduling-controller
3d64c80b752e316737514f8b4e0e3a9644cac8e2 add scheduling controller
bfcbbc5785980b6a589ef4fc1134a614657312e0 Merge pull request #8 from qiujian16/update-readme
73e552a0fe251bf4cf9e2fee2c15f8901ec404b6 Update readme
863078da04df44856286f4f1d8ca36fcb4fc49ae Merge pull request #6 from qiujian16/rm-task-tmpl
e9cfefd06219a0b5dc03aa73ae861078f3d3a600 Remove task template
ef56ab5e729a4dcb453c26db44e3bd8ed5da566b Merge pull request #4 from elgnay/creating-controller
745568e10736af4a093d6102dda51c06d9e62770 add placementdecision creating controller
583e76101d58de4e1a16b6627ac99c47d526829c Merge pull request #3 from elgnay/add-missing-files
45a1ebb053c6a0441d8fe731bada15ec8ed926db add missing files
3ecff20ee0291a064aeb8a1c9a89a21dc141caad Merge pull request #2 from elgnay/empty-controller
10ce79464eb5d54d50d1c710a56a76ee66ef3d84 add empty controller
aae227496eda2fec1f9606d662a9e82183638c6e Merge pull request #1 from elgnay/common-files
6f1686e7e3c8d5f43a971da5ffca1c684ea27638 add common files
1aa20662077a0b0d5d2c3df00dc26214fa05b5c6 Initial commit
```

Status: Fast-forwarded successfully.
