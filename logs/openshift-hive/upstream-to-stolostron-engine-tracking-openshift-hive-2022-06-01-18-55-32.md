## Fast foarding of openshift/hive into stolostron-engine/tracking-openshift-hive.

## Status Summary:

ocm-2.5-mce-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch ocm-2.5-mce-2.0 -> backplane-2.0:

New commits (first branch sync):

```
4052426cb48924959e121d63068f9570ea0a9d22 Merge pull request #1753 from abutcher/backport-HIVE-1858
90c46ab57569f3600d9552f9d668f64c23fa74b7 Decode VSphereMachineProviderSpec via openshift/machine-api-operator's ProviderSpecFromRawExension.
275fd9bd46dc8e20045a024a605ab10245bc4dc1 go mod vendor
da113e5cdccfe5e11aecd6dba426438d05614b0b Add openshift/machine-api-operator to vendor.
8871bf4cdee39bde41a714c52c81f92bf7d40dce Merge pull request #1740 from 2uasimojo/backport-bundle-gen
9f80f2c447a9198b2775f93c365832d332915ab1 backport bundle-gen updates
6cb94c6de6932c785d8954299d61bf6c68860bbc Merge pull request #1739 from 2uasimojo/cve-dep-updates
ab2d233dbde5e4dc76d52df0ef361e46e06789df Update vendored deps: gogo/protobuf, x/crypto
f42617c99ca102bf3f262194b5ff14e6186dd996 Merge pull request #1736 from openshift-cherrypick-robot/cherry-pick-1733-to-ocm-2.5-mce-2.0
715197c03a523765843d906d86a7fd0b8704c86b Set ovirt cd platform label.
60649c01ab8dbf17df815360eb3098c025c83764 Merge pull request #1735 from openshift-cherrypick-robot/cherry-pick-1714-to-ocm-2.5-mce-2.0
47733359b2766f3e485522ad14590964e1d7e734 Merge pull request #1734 from 2uasimojo/HIVE-1791/ocm-2.5-mce-2.0
fafbf32dfd91591a72cec6c87bd840aead7b63a6 Add test for cluster metadata partially available from ClusterInstall
09890a4540209909785211f38bfdd6e094522a8a Ensure cluster metadata has an AdminPasswordSecretRef before copying.
1cae813f6668110f8fd653f12f1c2d9bfd9ffdd2 Skip "claimed CD" creation webhook for DR
b039dc499f49b9444ceb2626db61c8535964e198 Merge pull request #1730 from 2uasimojo/HIVE-1786-ocm-2.5-mce-2.0
096eab32870ef961cea2ba52f6e54af17477074a [hiveutil] Remove default machinepool generation skip for oVirt.
faf1354dfeff7f2f1ba83de07b3d6d2f5ec729d0 Remove preserveOvirtMachineSetNameSuffix.
99ce733c174a19b455ab01bd94e4049663753c7f Fix nil pointer dereference in oVirt MachineSet generation.
5cfdd440feb60686cce722f2ae62f8f635359fde Merge pull request #1727 from openshift-cherrypick-robot/cherry-pick-1724-to-ocm-2.5-mce-2.0
bd92285554ac44f83784480a6162ab12c09ab0ac Set RemoveTemplate=true for oVirt deprovision.
7a1238d8bdd43c95d778f56a9bb9a2ca39e93320 Merge pull request #1719 from 2uasimojo/HIVE-1781/NonePlatform-ocm-2.5-mce-2.0
5fc06f36806e7133d4329519a723c87bd1a1a09b CD.Spec.Platform.None => `none-platform`
6feded1618a1c09bbf47009257961838db5b7905 Merge pull request #1716 from openshift-cherrypick-robot/cherry-pick-1701-to-ocm-2.5-mce-2.0
128e265ae800ffbf1131b681969555f1e1326c22 Correct --creds-dir param for ovirt uninstall.
6dec9c34e8ac39e23a9ec90f01415615b56956e9 Merge pull request #1695 from 2uasimojo/bundle-gen-backport-ocm-2.5
47f410033e6dd5f03faaa00bb7bf3ca9b4556213 Backport bundle-gen
54077a8310b23ced44a9b949b0fb22451d090ba8 Merge pull request #1684 from 2uasimojo/bz/2050332/regex
665b268161d83a3ea9d0ab4788031528110ef4d0 Bug 2050332: explicit Pattern to validate Duration fields
c2317e6c13bdf3366eda9ecb724a7a61608ff9c0 Merge pull request #1683 from 2uasimojo/hiveutil-multiple-label-doc
1882bbd61945206ea92fc061a0336723a3545ebc hiveutil create-cluster: document multiple labels
9c572408b5299c520160e7a317c52e80b0415b9f Merge pull request #1682 from 2uasimojo/groupified-api-resources
070e413d8ce96054f5493faf8cd97e828570c3fe Groupify hiveconfig template
ad1892abdaabe201f011479d68201fb524e4d028 Merge pull request #1681 from 2uasimojo/appsre-build-confusion
f9b3e8ebd26943eac0174a4b20d52ad2086a77a4 Add output to de-confuse first appsre build
cddf7e5432a7e494ab3b36f20437a6af8eaad709 Merge pull request #1679 from 2uasimojo/HIVE-1753_and_HIVE-1723/codegen-GOPATH_and_go1.17
df3db863884a7b366f478eea47b29b8b434597ad Updates for codegen, go 1.17, etc.
787ae354f7b9e7f0dfdca1595630213c88677b83 Merge pull request #1680 from 2uasimojo/HIVE-1753/trigger-ci-to-update-to-go1.17
4546811d838537ab63ce308d5febd1e8f58cd546 Trigger CI to update to go1.17
5abaef4785e6a7ac70871573010d3b736aab4db6 Merge pull request #1674 from 2uasimojo/HIVE-1747/sort-running-by-name-second
2f232336262a00e4ee866f5b69bce353d30369fa Merge pull request #1675 from lnguyen1401/natGatewayFailed
27cf49462921abff45fcb6814aa19473891611dd Added NATGatewayFailed Error code
8dc97bc97ec826dbc84b1ae9c9bc872b323eb0fd Merge pull request #1671 from gregsheremeta/prefer-generic-terraform-code-install-log-regexp
25c9b6f93ad7b033c04ed1a6dbbce5eda8c0fe59 Merge pull request #1668 from 2uasimojo/HIVE-1746/cluster-operators-pool-timeout
e3144f86689574942d7b6defc52ba23d985bfdd0 ClusterPool: Secondary sort by ns/name for running
ebda04c1ae4fd1010a1ea1caa313b91b23e884ee prefer generic InconsistentTerraformResult install log regexp
b0fd36fab9eb460936f67936abbc083c755e0f41 Merge pull request #1669 from supreeth7/nlb-error
1575b9557e00ac39f13eaf3c15c1acd6bec6d756 Merge pull request #1670 from gregsheremeta/fix-bootstrap-failed-install-log-regexp
9f56d9d7257f17be9bff4de51b9e0731e4743e65 fix overly specific install log regexp for BootstrapFailed
6e65d3df651ee78d2dd452aab39aba231e61f31a Add regex for AWS NLB creation terraform provider failure
c9b285a82676119e39f4019029e5a92fccaa0563 Merge pull request #1667 from 2uasimojo/bundle-gen-github-user-env
884790dc274b81842c94bd340429939fd7e22430 ClusterPool.Spec.HibernationConfig.ResumeTimeout
46e0ce921a7ad71f02dd6f2db67cb03db6808868 bundle-gen: Recognize $GITHUB_USER
a607db055268e8dacd1b32e8428b3413ac19f8b5 Merge pull request #1666 from 2uasimojo/HIVE-1746/cluster-operators-toggle
f698e1a304f8cb9ca203486cfdb25b39a474df12 Label to disable ClusterOperators check during resume
fcac82e4f82ff7f0162eba7a26e0aefa1b5b5936 Merge pull request #1664 from joelddiaz/webhook-certs
cb92e67bedfe97a7596e66b9d97c42ea41996b66 inject CA data into webhooks
b212e8a45e956e8e59a5f8fcb108f298b3708442 Merge pull request #1652 from 2uasimojo/HIVE-1679/claim-running-clusters
d31e272ac02447d1db1ec0c355e03d25f37970ad Merge pull request #1660 from 2uasimojo/HIVE-1736/leader-election-1
7ec5c25fab0d734f9702666b1244cdd737eacee9 Leader election migration 1: ConfigMap & Lease
bb19a6a03364aee2deae2a59ca18f16c06665e6b Merge pull request #1662 from bmeng/install_regex
e4fb02fe2850db08bf1436df3397cdbc674fc2f8 tighten up regexes and messages
9aec08e07074c8b8252f5c62e8033f2919ec5717 add regex for known installation issues
a0671aa97ef391a4dbb6a84d3866294d5372f346 Merge pull request #1658 from blrm/add_failure_regex
33da792d3239f4e0084dde65f6c0cfd8192f3073 Refactor: consolidate leader election
d8975c5f5f3b98f86320c5f33c48361fe7588498 De-lint pkg/operator/hive
b2933dd1e5c681d432cb65bfd3f157ee13feaed5 Merge pull request #1656 from abutcher/vendor-installer-ad535d3
3cfd5abc99881c1023444e94433fd6a59124e262 OSD-9688: Add regex for VPC missing install failure
af4db56fd9b133d1aa30d48efbae54c44245d1be ClusterPool: Claim running clusters
539fb8389c05b445aeae71960f53a80fbcbcaf98 ClusterPool: Use CD.Status.PowerState to detect Running
b2a4421c157a906d428230eb81fe8a7bd79b7e0c Static analysis cleanup
7f08e65c3c1a85175862ed17c35780ba084d6a54 Cleanup: Consistent ClusterDeployment consts
012bdd5d0b52ac15bd9a17bbfcc81fe6b6dce3ed Merge pull request #1572 from bdematte/fix-syncset-uwm
66d78fddec2fa0c0e86c985fec92ab6b585b36bb Merge pull request #1653 from akhil-rane/fix_install_pod_failure_midway_installation
d4722280bd716ead21a30d29e62429d720da762a Vendor machine-api-provider-gcp for unmarshal GCPMachineProviderSpec util.
3e017a9db3cad0c2767e8922567a3b085da30ed6 adding test and integrating review feedback
7363fb7c4c6f23b431d59234eab1a7d6a47ebc96 Add error message if install pods get killed or evicted
636ab70a3dcf2b385fc7ca5bdd30c812a78a49c3 Add the name of previous provision to cluster provision
ebf5aaa1a60a103996568244792af0ff6a1f7d95 Update imports for installer vendor update.
5043d3921169916fbfab3bd558442e56e876695b Update installer vendor to ad535d3.
588f139c6122c62fd5232e7b47125bad103680fe Merge pull request #1649 from 2uasimojo/bundle-gen-docker
71fcc7901b1da041692318b4dc2351b9f597ae5e Update bundle-gen.py to support docker
6ba92bb3a76860feca36f62c0c4dfeb1f04e443a Merge pull request #1651 from 2uasimojo/HIVE-1734/claim-running-condition
43c79c144c2bda6af9029904e9eda3a3252680bb Use cd.Status.PowerState for ClusterClaim Running condition
7d022be6d5147e6455c6e44799e935645868fa6d Merge pull request #1650 from joelddiaz/update-x-crypto
14e583c21f9435ddbbadc1512877c71a390bbcd8 update vendoring of x/crypto
71c1839b3ebb6453eb50e140a42fd0306709446f OSD-8194 : modifying order of operation for syncset update to avoid deleting new resource version
e50103a3e833bda1b7cfd53ae7d04c61a103b401 Merge pull request #1646 from 2uasimojo/HIVE-1729/claim-del-wait-for-cd
4c8578ec03b107af8d4fd649eb8cbc27e9491f81 Merge pull request #1643 from 2uasimojo/no-container-0
202e653ab68705233c688517083424c7e62bbaa3 Merge pull request #1642 from 2uasimojo/inspection
dd74b28871f9de9d8346d677ab1e2c5229a4fec4 Fix some bugs identified by code inspection
ce16a5d6792a92e21c761374206cb15be0848eee Merge pull request #1645 from abutcher/HIVE-1465
8b81f2d08e0fb3b8d3910d251eefd2fe7d15724e ClusterClaim deletion waits for CD, Role[Binding]
aff8a503c5a0a1ddffe7ec1f41f17617beb3177d Merge pull request #1644 from joelddiaz/doc-additional-certs
25098480c566e9984df755ac1d67ac2fcd59ccc5 Stop assuming containers[0]
443f9262bb3a3f6567a25020f4c15254cb818365 Set auth condition when auth validation fails.
7c4809dfb4655909e38ed2d2e71958ec0d055680 hiveconfig additionalCertificateAuthoritiesSecretRef doc
32a93e12e1298ffbaca34444540bd1c5cb221e6a Merge pull request #1641 from mrbarge/proxy-errors-2
654d57ae6fe02812edfc564c9bfda8976f29c513 Add additional proxy installation failure regex
00f7a93bcc693452b0c1be6a722e758ce63050a4 Merge pull request #1616 from 2uasimojo/refactor-configmaps
642042ebd3914aad31d2d8c9fea71221da516d9e Merge pull request #1604 from suhanime/hive_1601
efae6a12ade3019f830efe8fd58ca3ed4dc83309 Refactor: DRY operator configmap/volume management
49d19b865b48f5af4c7de36e848401c58fc0bbf8 e2epool changes
ed764520405b1793f95fa3466364987e7c0722ef Add new reasons + code refactor
da6aa084015c6d4c4f7c651402790f030d163828 Add more reasons for hibernating/ready conditions
f73ed3ee0ff8bb4840661ab202ff486bd4ee0ec2 Check clusteroperators
022ab9e893702fcbfad967eca40abad01de57e7c Add cd.status.powerState
c0c34366183fea87eb7846a14972bdb6b8999a32 Merge pull request #1640 from gregsheremeta/install-log-regexps-inconsistent-result
b489b2d21e885326435cddc9327153e577e29f24 add install log regexps for terraform inconsistent apply (a known installer bug)
f3eea67ff7b899544bb4680290d9937ef71680bc Merge pull request #1638 from gregsheremeta/install-log-regexps-route53
e8c1604264b705ba19ce7bff48521b58bdb71122 add install log regexp for route53 timeout
19b5910931fa7148b295a8d796085b4a7ce7bf7e Merge pull request #1639 from gregsheremeta/install-log-regexps-bootstrap-failed
29a33582101fbbac6d382851f57036e14cbf8ae0 add install log regexp for bootstrap failed
bea2befd082c5ef9c944a9d7ae37f2d7cf797dd9 Merge pull request #1637 from csheremeta/quota_regex
4511b09e59d24e34ad7be7d17b59601906679201 Update installlogmonitor_test.go
c0ccc79d64500b97234fb35cf4011cb0e7151ce1 Merge branch 'master' into quota_regex
d3afb525bd9b607b0397018e6dd28fae9f78d5cc Merge pull request #1634 from 2uasimojo/HIVE-1722/cloud-NoWorkerNodes
fc9b4025550bc27189e010b8ec56e3e4f27adfd0 Add install error regex for AWSEC2QuotaExceeded
79d06c1498e02c9e324c9ff154c5c682b6847b71 Install logs: NoWorkerNodes => (AWS|GCP)NoWorkerNodes
a9ff46299b41edcf069f6529204d44c66b0a935b Merge pull request #1636 from 2uasimojo/HIVE-1367/fup
25c6571439914a1f79897e9df492feae6187c873 Merge pull request #1614 from 2uasimojo/HIVE-1692/FailedProvisionConfigMap
058960894e9effdf489fca6bc382d7d5c476ca69 ClusterPool Inventory RFE followup
55f636380a95c92758f95b5033f624e4f1059948 Merge pull request #1635 from 2uasimojo/HIVE-1697/consolidate-docs
735ceb4f8b261d79440c3c7df9862cab0f4d15ed Consolidate S3 upload docs
779599494aca1c72391c0a4a3b9453f78310cf50 Merge pull request #1633 from 2uasimojo/installlogmonitor_test-dedup
1566d49af21982b916eaafa166460f3f5ca29764 Merge pull request #1625 from 2uasimojo/HIVE-1697/document-log-upload
0c90e03bf559a582977a46eab983487ce141987c installlogmonitor_test: Default to using the real configmap
8a171ea5c4cc665fa3e416a6ca89284c1247a4cd Collapse duplicated regexes in installlogmonitor_test
9f4c6a8734530c1f7e50fbe0e7d4f5661cfe5c63 Document failed provision log upload
b3535fa5f52b7f27198fece87d1ed6f68efff91c Merge pull request #1620 from openshift/fix_azure_e2e
e7f4b1feee0e498a2780a13ce81b0ae86aa80d23 Use a ConfigMap for FailedProvisionConfig
8f6fd212c6aabd01fabe9accd40d5a51240a2f11 Set managedDNS=false for azure e2e
989dcd87b34283819af96cfe78d1aac94cdc8820 Fix azure e2e
7d1044bd87aa1e0afd42978fc081f4d908deee2c Merge pull request #1607 from openshift/rfe_cluster_inventory
da269c76225075019b30f9a9937b2d3abceeb955 Enhancement for clusterpool to work on on-prem clouds
98b5cd0cef3932237c30fcc78a81017801bfd0df Merge pull request #1624 from 2uasimojo/hiveutil-ssh-private-key
a6d5db8f5d4176fe9c19f9d0885e4edebd50a8b3 Merge pull request #1628 from mrbarge/osd-9064
f3e702dd7ad6e0aaa04c5d260387f481c4131ba8 OSD-9064 add install log handlers for proxy install failures
1f0f3eb646c3efedf882147b0d39f8d961729d2b Merge pull request #1623 from 2uasimojo/e2e-logs
c49404b90ef86c008c71d22b2c08b105ff4e85fa Fix hiveutil create-cluster --ssh-private-key-file
6a6a262ed3065910a122de0dbbbf3fc828278ac4 e2e: Fix disappearing logs
21cc8d004e334cba0566648b65c3c2232f413d60 Merge pull request #1622 from 2uasimojo/testify-imageset
d7d231b641f917197af1c6c64021233b942e85f5 Tech Debt: Use testify for pkg/imageset tests
f59c26b3c4ba02e52c7bb4baac9b7a96f3e1b91b Merge pull request #1619 from 2uasimojo/HIVE-1698/InstallerImageOverride
26039daa92b6dca632870b0974df08d232347c5f Merge pull request #1621 from 2uasimojo/e2e-node-timeout
0ac6df976de19c78bb4b5a4e4696f91134b92bc3 e2e: Increase node wait timeout
925c01abe44907f28acc4d8495cd2c9cb0f1101a Merge pull request #1618 from abutcher/hiveutil-cloudname
aacc8555fac61b380d3b42502570f2737b29ad94 [hiveutil] Add --azure-cloud-name parameter.
2406a774ca270362ae432b0d4de8f52c79e14c3d Merge pull request #1617 from abutcher/OCPBUGSM-37645
716c354e4df093e25350ea025fdc1fb095927738 CD.Spec.Provisioning.InstallerImageOverride
c29f62849bc7bf2ce8e22e5ec932da3ec3e378f9 Respect azure cloudName set for clusterpool.
bee4a4605d7921f5900bed2242bdc688a51a4313 Merge pull request #1615 from abutcher/rev-installer
0d3221e5506c4edc6560229d0171708ef63e80f2 Various fixes for updated installer vendoring.
eba32d856fd9614be5c1a87731e32f917d8d96a0 Generated updates from installer revendoring.
b8d56cdd6f6362b1dd69eeaf757744049991b154 Rev installer vendor to release-4.11@11bfe563c288
8f0773c53b8463b73fa3171cebcfe6abf4a48107 Merge pull request #1613 from 2uasimojo/managed-dns-configmap-name
9cd299ebdf364f26e683686ce990ab5e345685b7 Static name for managed DNS ConfigMap
75b487e158f853df60ee48534a767e9b8670b7fa operator: DRY computing hashes
088d10ee8ead6357ba33754a2024abd8b6907eef Merge pull request #1612 from joelddiaz/provision-stopped-comment
5fbedbf63fdc8aa201701b2e898f7c84ebd034e1 clarify when the ProvisionStopped condition would be set
f704abe069fcf9c69dc0c62841b21fd662032082 Merge pull request #1611 from gregsheremeta/tweak-lb-slr-regexp
e75ef9e4608c081b7e4de5f0d008a408f8e98cd2 move the install log regex for loadbalancer creation failure to its own condition
cd6a19d6d80e90c63a79df32176c2a1e08133f93 Merge pull request #1610 from mrbarge/add_lb_install_error_regex
c145b0d24533bee908fb5865555865ae7165ab0d Add install log regex for loadbalancer creation failure
aef31121ec47c248615b0324d5aceba4568cea3a Merge pull request #1609 from 2uasimojo/HIVE-1662/RetryFailedProvision
e3ba9bf0a77fe8d1a16bd9bf88501a92dbee369b HiveConfig.Spec.FailedProvisionConfig.RetryReasons
387d32ead2d398925f618c8c885608d19a912da9 Merge pull request #1608 from 2uasimojo/clusterprovision-test-helper
a46c8dbb511b09bac75b3db5ce9d97f0f6240855 Make clusterprovision Builder test helper
3392e4ebfd16fd4e91bb69b6a9485631be8925c9 Merge pull request #1601 from 2uasimojo/HIVE-1656/edit-targetNamespace
e46485b1e35b052836c3688b133e63bb26b707d2 e2e: Save useful info on failure
891d3c0adc038f3adf88bbe52619909a16c0897d Document targetNamespace quirk
a67835c6e185ab50947e7cdc5b235f540396f8f9 e2e: test editing targetNamespace
e9868fdd19cd34672e86a82808a1347da5dc1039 operator: scrub old target namespaces
9b0a3fabaea6f46481bbd8f2c7eb8c4263cf60e9 operator: Label targetNamespace
6f0e5e6765c9aa5d7ba9a8c364d1aa3dffa62d6f operator: cleanup: Remove unused event recorder
078ca1b039d7122c9c5f0a57b3807ff8e48fda2b operator: Allow secret watch to switch namespaces
948182aad7803cf4372bb43c1439719143efb905 hive-operator: Remove controller-runtime Client
d66896015d990af5d33503f6f7539bc28a7a2c17 Merge pull request #1606 from maorfr/pl-perm
fff2204c29fc2fe38ba1a9b0998b6c2f99800b88 add ec2:DescribeNetworkInterfaces permission to PrivateLink permissions
2e9224a00a1c7d9efc75040a4a49071f44af1f06 Merge pull request #1605 from joelddiaz/dnszone-docs2
c62158e791ccc6b576bde4e93dd06e815fd36c60 fix DNSZone docs permissions
e360a7970f301bf403aabac404c021b4c3573d1f Merge pull request #1603 from abutcher/revert-1290
67db08a38d1e72cd847c1bd31cffbcf2d0fee1e6 Revert "Merge pull request #1290 from abutcher/hive-1351"
2bbebf5983eecf3e539241cecd2c46a1681b472e Merge pull request #1602 from 2uasimojo/update-golangci-lint
903b27f7a3825232dfd3122a638f5cdef33bf852 Update golangci-lint (and indirect deps)
16c6e0ff6fa1a64be4fac92eab0b0f7408f8c671 Merge pull request #1597 from suhanime/e2e_pool_fake
465c7e09324aa91db010346980aa5b24e1145fb4 Test hibernation of fake cluster e2e
5d176d0966d0afc219e07c0136b4c3f4fbf79ba0 Merge pull request #1596 from abutcher/machinepool-controller
a02d5b19d07550a99c6086f5d3b1efaf42d65da8 Merge pull request #1598 from joelddiaz/managed-dns-aws-perms
94ac1cd4814d61104cfa0b5abf1405637accb88b Rename RemoteMachineSet Controller to MachinePool Controller.
e0c0031817c35a143c065a7dd065480907a3be4c list out permissions needed for managed DNS on AWS
0870ebf8af4a2f55b3c3697df5b788bd9f652e8b Merge pull request #1591 from abutcher/fake-clustersync
a9ad3685ac3bb2929f743a470a6273867118edea Merge pull request #1594 from 2uasimojo/hibernation-clustersync-backoff
ebcf83977bbb28b183bbbb54ae9407c4c026a3ed hibernation: Backoff delay checking clustersync
35b62cd3e7ce148d89f2057cdad9b3cd551f0c63 Merge pull request #1593 from abutcher/HIVE-1669
3e18fb2123521ef3a0cded651293bcc6fe64ea0c Merge pull request #1595 from 2uasimojo/HIVE-1684/no-break-at-capacity
ee951335475f673e7f92386190f0c20f0dda3afb ClusterPool: Delete broken CDs at MaxSize
5257024436987604d39a3af68efbc62291926ea9 Add UT: Create DNSZone with/without Azure CloudName
7a11e6b4e9422ce0fb75f495323cfaf4274dc3c9 Set dnsZone.Spec.Azure.CloudName when creating dnsZone.
a8a51e64fe64e54a59887ce1555b39b1a03b2890 Remove no clustersync assumptions for fake clusters from hibernation controller.
a2fa6c0492f2e95f1e3c86625a46dbe7ca34b3f3 Create clustersyncs for fake clusters.
93104b601dd341d0982c0cb3dab8fc9e3710963c Merge pull request #1580 from suhanime/refactor_hibernation
bc1417a33246d57e3420226b3f676bcfe37e610e Merge pull request #1587 from joelddiaz/minimal-Dockerfile
5d4b25c86a79af0678b6e004c31665b21fe39b1f Allow fake clusters to proceed without clustersync
772d7ef2299ee556a76c268f2aa5a0eddc58b09b Refactor Hibernation Controller
726d444bd90eb27eb41174498398d61527231501 Merge pull request #1590 from abutcher/gitignore-pycache
68828e61aafd84016dd5462c36fbd894aa94919f Add **/__pycache__ to gitignore.
9d8df6a5a0f3737599fa870c694d00810b35a267 Merge pull request #1588 from abutcher/HIVE-1669
50a82c40219797063799a394a46f4b59ce5e03f4 Merge pull request #1586 from 2uasimojo/HIVE-1677/clusterpool-metrics
53123054a50d3a655e33bc685474af7374875848 HIVE-1669: Create Azure Client for Azure CloudName
24049eb69ee1aaeb958b6a5419c9c2895d68931c Add useful metrics for ClusterPools
a5fccf4528f8ba5a0fc1d2a03a550eae1bc971d5 openshift-install baremetal RPM dependencies
44544aca46ddc7f626ba0e223155eb89120e7fc6 move to UBI-minimal
1dfd9e22a1c2f936ca0ef50d87f025b40bd4eadc Merge pull request #1585 from joelddiaz/centos-stream
7cd669c517646b74f2e73f0d0133a60d637b3147 move to centos:stream base container
f0cc1ba6954b5012c274e0c3bcb4aac0b97303a7 Merge pull request #1577 from 2uasimojo/HIVE-1655/unexport-metrics
c54c31c3826b42aa568cf4b2aaf24c42abb4f0ca Merge pull request #1578 from joelddiaz/hive-ubi
c475591843492534e6b7fbafbb66413577651276 Merge pull request #1584 from 2uasimojo/podman-auth-file
4dfeaf09f7a54a97de57b3a12686e9eb782721ba Fix podman auth file path
1f5d4c70c300f334e6ec3fb94ece9834007414d2 Merge pull request #1583 from 2uasimojo/docker-podman-login
8152247ef7fa3994d1d79c11045d3d51917f96ea docker/podman login for appsre
329d066b005784ae4959df182534e566ea04c215 provide a UBI-based Dockerfile
5ea84b9215bf5176fbce801960a49b9ab7f7bcdf Merge pull request #1582 from 2uasimojo/podman-push
45c5aa597fa59cc79736976ff4120dfa91c3fda6 s/skopeo/docker|podman/ push, stop producing :latest
15f912f39474eb14e3c14fb9e53069f570486e40 Merge pull request #1581 from 2uasimojo/podman-detection
09a4dfc44ffb4f3197f131dabf26e61f6ccc85ca Support podman build for AppSRE pipeline
168bd5d530ee6f68031514e28c733af20b16b966 Unexport metrics
6804034f628595300ff28d602da5c9f422693d16 Merge pull request #1576 from openshift/remove_agent_install_feature_gate
9fe8c486aaa4739356b40be02f2458f968cfd82a Merge pull request #1579 from abutcher/controller-runtime-v0.10.2
e252965a78379a64ddc879b4319b80dfb787a178 Bump controller-runtime to v0.10.2
bd434e4b6c3bb5342cc3d46a22188bd0f89340f3 Merge pull request #1575 from 2uasimojo/HIVE-1643/metric-claim-time
f1a668201b697a39fe87214cf7fa787f1ab54ca1 Remove AlphaAgentInstallStrategy feature gate
34f65a6dc7d53a733326c05af03b9d0ea78ab46f ClusterClaim delay histogram metric
a691d6f21d9ea55d94e97913ab2e4bc46a9ad7fd Merge pull request #1574 from 2uasimojo/HIVE-1667/clusterpool-installAttemptsLimit
3706bbe92d7016a14295cee7db47f02aeeb2cb34 ClusterPool.Spec.InstallAttemptsLimit
1b0e7cdce7368fb8f2745c1079ce81a5c63c0c7c Merge pull request #1573 from 2uasimojo/HIVE-1664/clusterpool-cd-rbac
f0c27baa5452e3a714a02214de298248e3b8e92e Refactor: Verify CDs after ClusterPool
255a57d2d1a11501a2b6f79a446be76268adfbb2 Expand RBAC for ClusterPool CD namespaces
16ef5a35537d678669522fec07f8f7a49bb76d44 Merge pull request #1570 from tnierman/TooManyRoute53Zones
88bd6b21276be5cfb0734e5d9685fc4f7b46866a Added 'TooManyRoute53Zones' install error
a27a4f7abc4eec5fa1037d8db7f31e7c158d4f74 Merge pull request #1568 from suhanime/provision_metric_1660
79c100afdb1cc3139bd19ef61a483791828e02c3 Merge pull request #1560 from 2uasimojo/HIVE-1504/by-digest
b7a5ebc4b7cc8cdb8444dc352835566e5bef8fd6 Merge pull request #1566 from 2uasimojo/HIVE-1657/clear-syncsetsnotapplied
e3dfe3aec913342981085b892d7d6af3586ac059 ProvisionDelay metric shouldn't log unknown conds
3abab03eafc501ba5b272007186f6c95c0c68bf2 Clear SyncSetsNotApplied Hibernating Reason
291cb115f814bf8e03cbe6408a824bdcc8583fd4 Merge pull request #1567 from 2uasimojo/HIVE-1651/excessCount
64392349478de3108ba23d38c319af7788ec5f9d Merge pull request #1565 from 2uasimojo/HIVE-1596/adopt
45664c2a41f014e7756fffab2842d8461e8ed5db ClusterPool: running clusters for excess claims
c770a0a1c6e3ff14821cedcf9ecf8675d8a8f02a Merge pull request #1559 from 2uasimojo/HIVE-1654/nix-integration
92325c63c08f4f077d2547febf6884aabe4f0d9f Merge pull request #1564 from joelddiaz/update-owners
143a0c631bb80aa132c598d693ece89820412e96 Fix Provisioned condition for adopted clusters
25d51259b20f1cbd9e5c4d1c65771c9084c5b332 Merge pull request #1506 from suhanime/fix_claims
0cd2355ba403f50d7f623c9d9a8f0c01d1ba03c9 update OWNERS to reflect current reality
28ed8ad37188ba0e5e4eb0522383e81110ffacdc Merge pull request #1561 from abutcher/bundle-chdir
787490c8eb1b44931e1e6fd89a5b01a4f3299369 Merge pull request #1562 from joelddiaz/error-on-failed-push
a44c69af7178fc2661b17dc41f35471d99b377e1 fail on error to push container image
db6ad8065cead1ae690c833b8af3c60f7f8cf1c6 bundle_gen: Ensure working in hive clone when generating bundle.
512b7f461ca18ba5bd6a2ff464d02832a48b5b3c Merge pull request #1546 from 2uasimojo/HIVE-1596/deprovisioning
675412fd14f27d37dfae060b8dd292bcce954059 OSD: Pull operator/controller images by digest
a4040790e9560df3f59cf6d6afd38b0ffce245ec ClusterDeployment Provisioned condition
a1a382b237ae78dfc53ca47fe94b42c44c62fe11 Deduplicate ClusterDeployment condition updates
a22d1ae40ce5feb93753ec6cd69402e90225c78e Merge pull request #1558 from 2uasimojo/e2e-pool/broken-cd-flake
994cf6ce98a5a810caaa2dd7344a826a5dfcff44 Remove integration test suite
9d6bea016c58990178301fab171821d88d3aeadb e2e-pool: Broken cluster flake
8671ed2067e47e5ed0b6e718e7163a6741ed7b39 Merge pull request #1557 from 2uasimojo/HIVE-1604/another-v
ec7854ce1212f0eb7458238e2f6e35996c361096 Merge pull request #1556 from 2uasimojo/HIVE-1604/branch-discovery
5e4bfed5baee96550a56326c93598e4d18a330e9 bundle-gen: Another missing 'v'
cb2e06ff64877117dd70b397965749cfdf165c46 Merge pull request #1547 from gregsheremeta/more-install-log-regexps
6c8a520f3b7f4f445aab38c8739e3b9c3601998c Merge pull request #1554 from abutcher/bundle-gen-tag
2ce9cd09198d3fb849a59eabbe461360cd7b9200 Merge pull request #1552 from abutcher/HIVE-1638
a20b1d1222e403fd17463b44da6b91eb228c4315 Merge pull request #1555 from 2uasimojo/HIVE-1604/cleanup
4b40839575bd852f29fae31eb8a8eec83e08b134 bundle-gen: Discover ocm-* branches, fix alpha
0f970d9116eeb2d19f2cdb5b3936ac7ec39259eb Clean up old operatorhub script
e099a264f1a7164031b381ac59147e0c6c85014b add regexps for common public and private subnet misconfiguations
23832ae9123aebc9cdeca7486a2409189ce73159 add instance stopped regexps to install-log-regexes-configmap.yaml
0cb8d3dd69a2207114750849e6a094f75cd1d81f add VcpuLimitExceeded to install log regexps
c2d193c6b7d3b19ed0be4159c23eda808d4c5b57 reorganize install-log-regexes-configmap.yaml
929316878e24f1a0830dae31b6d7384029f03688 bundle-gen: Add 'v' to image tag.
5a9f38f0188a8e126cf795c692b54aa52a7c2b82 Merge pull request #1553 from 2uasimojo/HIVE-1604
c3ffcb302dce6fb12850317653acea87137aaf44 Merge pull request #1551 from abhinavdahiya/fix_adopt
0d4916863fa8d092ad7daf3dd32f6fe06f7ddc6d Remove AzureStackCloud for now.
e1182a0fff31bee654ede3d27e42dfc4ff3f07ed Merge pull request #1548 from abutcher/read-regex-cm-tests
37f1f1ac3bd6b4ded7807449215c6787084d5e67 bundle-gen: format
08f2a6a025385ee88034c6aa7496f004671ef604 bundle-gen: smart branch/channel detection
3ae8f094aa10793b1c61c1e8d6fcefe77d84e86e bundle-gen: Fix version 'v'
97fad752147c1841c2478eb907e87ff0300c5813 Merge pull request #1550 from abutcher/HIVE-1604
4d813057d712b43ebefaaae1622fbddf0d89adad HIVE-1638: Add cd.Spec.Platform.Azure.CloudName and plumb into deprovision.
1daef7d3dc7b3dc7ab98f74549c59f454634cb26 Add github module, skip image rebuild, fix push
d70876b18768b10ea3b83a38d0583e5646b0d048 clusterresource/builder: add type metadata for adopted kubeconfig & password secret
f8fae7dd912959cfeeac0b907ee75522859ee437 HIVE-1604: Amalgamate build and operatorhub push scripts.
1411793e782121c0df003d9bce467ac93fe31122 Merge pull request #1539 from yithian/add_install_failure_errors
0b9229b91e6f8a3c2bf095efbdf017226e69d026 Merge pull request #1544 from abhinavdahiya/vpshere_creds_missing
ba62f070eb2dbd4e791fdeaafde49b91cbd67162 Update pkg/controller/clusterprovision/installlogmonitor_test.go
63c533c0e62c629dba661ead70ef1c0588435166 Update pkg/operator/assets/bindata.go
85eae76318d5472ac9f02811c23a3f14510fddf0 Update config/configmaps/install-log-regexes-configmap.yaml
ba37c6cdbf2d9b4450ca7593949287d49ea01910 make update
660f48b811618cd3b349a87281114dbed640916a Update config/configmaps/install-log-regexes-configmap.yaml
8790f09be267ca0afdac081cc04e67a24ef35e1d consolidate AWS error blocks
2b604d7473fb7873f2b844708e00050c9ff27eb0 add install log regex for insufficient permissions in AWS
bd69f1e27339d01c8679bb141703ae05bc46dd62 add install log regex for when the subnet doesn't exist
2f226988e209d0435eea74585d733cdcd3d4a3bc Merge pull request #1533 from 2uasimojo/HIVE-1615/e2e
4e11974b19330300ff2eea5b4ed36cf4e9d29952 Merge pull request #1545 from yithian/cant_delete_IAM_role_failure
b67dcd1ffbeccea6b70c094ecd33ff996b1d5330 Read default regexes from configmap for test.
f3fb2afd340bb6e84a41be326e701bc10e1a179c Update pkg/operator/assets/bindata.go
d62947c1b7f69d434b41299a396c29e6ab03e9c4 Update pkg/controller/clusterprovision/installlogmonitor_test.go
e4aa69d167650ebb195d0dc80cac654e287401a6 Update config/configmaps/install-log-regexes-configmap.yaml
4210cb29d3306dfe14c7abc1ca687cdde6c6f220 use AWS role name pattern
6dc55296f160c6a0ff64c9086f1b3249bfeeee23 stuff from make update
48f20e45111570f3d06ec8ed5806b4254d4592c0 detect install failures when IAM roles can't be deleted
c0e9a5bfbb68a790101c2f56e1fc40372f4bf102 Merge pull request #1540 from abhinavdahiya/dnsoptin
34c28060eaba71ae973d591324428db1a7c1c587 Merge pull request #1535 from 2uasimojo/e2e/dnszone-actuator-hack
8bd974e18917e31a6064ad353b0070264fdd31fb Merge pull request #1528 from 2uasimojo/HIVE-1576.code
25dd7ecb2563e1d3e864e37f4e1a65d545652c89 validate username/password set for vsphere installconfig
da7c6cbb17f8e60d0c93b2a1ed8c2e0bf13992cc Merge pull request #1543 from 2uasimojo/HIVE-1576.rfe
dd037dfd2000df062603c5731d9b87bd961224f8 Update hot spares RFE
d10122b36a6e9b20a064e84e1400a125e1ae7c9e e2e-pool: Test broken pool CD replacement
4f6ad43549167caa362caaaacd249e9ea6b58804 Merge pull request #1538 from 2uasimojo/e2e-pool/ready-pool-flake
6c0828d59e69d3e98ced7d30feceb6b06dadb2b2 Merge pull request #1542 from abutcher/CVE-2019-19794
52de6793a2bc05ef04690e4aa35292cd7b585403 ClusterPool RunningCount
398bb08f0fcdc4bfc29a74a930667ec0182e2f7b ClusterPool: Register new clusters
cc061de1c654524a72daf3048483229a50fa8c5b Update github.com/miekg/dns CVE-2019-19794.
22c6da190a7a1a4585ad8e9de9d0bbb9781eb026 Merge pull request #1541 from 2uasimojo/clustersync-float-flake
ec0ea846524d4c8cfcc206aed9a5494d60388e34 Work around clustersync float compare test flake
b3ee879bb097c64da55eda242226f557d225da9a e2e-pool: Move AllClustersCurrent check into wait_for_pool_to_be_ready
fd486a1b0a17d3c4e6fa941aa2fc2c435021682f controller/dnszone: add condition to track dns api opt-in required failures
18827f64c00ea6400411366452293adf9fbecb72 Merge pull request #1537 from 2uasimojo/HIVE-1058/register-the-durn-metric
820ee2d8a2fb2df31f1d3b48c56f3ba6282afeb1 Merge pull request #1434 from 2uasimojo/HIVE-1576
87a861ce1745caae9a933d1490fc7ba8feb5d25c Merge pull request #1536 from 2uasimojo/HIVE-1646/clusterpool-example-namespace
cfa4da0c85697fc7698432621e568b1fc28886d7 Merge pull request #1525 from abhinavdahiya/hive-metrics
a22a451a375a5a383d2746b6dbcfdbb5902527db Register hive_clusterpool_stale_clusterdeployments_deleted metric
138c8e0045d06891aace020d43ce7160da9513ba hive-operator: support exporting metrics to cluster
5d4754dc12523c323ddda5438533b3917ab853ac e2e: Force DNSZone resync on ActuatorNotInitialized flake
75b5c6fa4422491980302d248641c0cf6618dd98 Better namespace in clusterpool doc examples
0756b70e6db4f5a92d7eebbff7be45b4e79aa033 Merge pull request #1534 from 2uasimojo/e2e-pool/improve-pool-readiness-check
e6a2ba3ff91f19c937e69b6b3271220af3580d1f Merge pull request #1526 from abutcher/HIVE-1637
9eb7e10f3e3495e91bb1ac20814286001beebc4b RFE: ClusterPool.Spec.RunningCount: hot spares
b94f21c51d1332edbe0fb7ee309bbb48db662936 e2e-pool: Smarter wait_for_pool_to_be_ready
facc9585d6af13172b0484dd919e86067a5a8ca9 Add preserveOvirtMachineSetNameSuffix func to preserve -0 machineset name suffix.
b902c1555e52d9798dbf65b8c908de7083e02b9e Merge pull request #1532 from 2uasimojo/HIVE-1635/nodeSelector-tolerations-from-operator
b9fdf06954d49160aaecad5e59b071a3da8684c5 Copy NodeSelector/Tolerations from operator to controllers
9440dbf8abf1fa11a101d8d24c3d8947fd55f229 Merge pull request #1531 from abutcher/HIVE-1636
1a2c83e64ec5d824ffea1252061db19bcf103e54 HIVE-1636: Make ClusterDeployment metal platform agentSelector field mutable
b64b0e9240bbe9d9843ecc5f56d34bc88a58ec9c Fix expected ovirt machineset name.
49a896d05e4536b76b710094c9cc4817b932c285 HIVE-1637: Update installer vendor.
aaaeeffa04b291a0bd3b863afd9412a24e4658f8 Merge pull request #1520 from 2uasimojo/e2e-managed-dns-retry
162432afcb877cb7a6f1901dbd42a327d51693b4 Merge pull request #1524 from 2uasimojo/HIVE-1615
5806b7d6c6b087cbc84810bc2ada0b2478c359cf Merge pull request #1523 from 2uasimojo/more-e2e-pool
f5a92de39b7a712ee84831806eb7bed55ebae68c ClusterPool: Delete broken (ProvisionStopped) clusters
369293ccfb8d317569fc0ffdcdfd980ed9b0da6e Metric for terminal provision failure
ab478175bcf93b20027de44b55db3ac3db967728 Refactor: consolidate setting ProvisionStopped=True
b905af51d8c8f2e29ecb327a1edd7da2031ced7f e2e-pool: test stale cluster replacement
f056b0209f6d06a919e50d4a1423e40a258b3505 Refactor e2e-pool-test.sh
b5a401d8790246394247845c208a50f536f939eb Merge pull request #1522 from suhanime/provision_metrics_polarity_check
2543fb6268d254c8b340766986bf7d332defadb2 Add polarity check for Provision Underway metric
694e5a8a79e1a132e0bc32c21c225c25ccec8d62 Merge pull request #1512 from 2uasimojo/HIVE-1058/cycle-stale-clusters
f3e437e4a55962c898abcca7aa06c8f654306028 Counter metric for deletion of stale pool CDs
c5815e711e5ca7aec93bdfb07a51bc14eb39413c Slowly delete stale pool clusters
8b4f8db4acc4929200b1df14ed4681c2552fa682 Merge pull request #1518 from dgoodwin/csr-approve-fix
29c6245088d811da8e2818445c4c2ee292014ff1 e2e: Add retry for managed DNS
2998bc1b971b6f2a99e07de5b0391a2178e1f28a Fix issue with CSR approval and status being mandatory.
3e64a9db811e3a98bdcd12877ad5e1a568eeb400 Merge pull request #1517 from 2uasimojo/v2/powerState
1728d6d1d71e82e26af72c1b7fd3b24cb61ac4bb v2: CD powerState sub-struct
27b7f5b1a9cf2b04d03e3449fbbdf14b602d6bd8 Merge pull request #1516 from abhinavdahiya/rate_limit_updates
0f4cca5141e939a77257cbba437dc3ab66f9cf78 pkg/controller/remotemachineset: rate limit MachinePool error update events
199deccf39a02a236baf145e06379f123c799b48 pkg/controller: rate limit clusterdeployment error update event
167fbab643437eb3297f07f9654b7e003c19d203 RFE: Detect and replace broken clusters
5d3295dba3c5a4615fcabe07e63bb03a649682bf Merge pull request #1513 from gregsheremeta/add-bad-tag-install-log-regexp
17e754e1407fe3b9f3194ef1f8cebef781973e60 Merge pull request #1515 from abutcher/privatelink-encoded-message
b70da64b49847ba336e877d5cbcd1d4294ef8dbb [^,]
6adb511ae8fa9e6b91d57988d7939f4caee3a7db Remove encoded error message in VPCEndpointServiceReconcileFailed condition.
6f060f04b8ab4fb505b20486b09bba54c631974e Merge pull request #1500 from showeimer/mp-readme
c922942dac5ea989a6b348db1fe0cbd21758d02f Merge pull request #1514 from gregsheremeta/fix-gcp-cpu-quota-install-log-regexp
dee1382c0b21ddbe8185a3c29b2d3140877e7c06 add install log regexp for invalid AWS tags
a873e5d304f8598d3897d63149fa183c8ff02b91 fix GCP CPU quota install log regexp
bceea12511739f1f16d2101c32afab6193ccab13 Merge pull request #1511 from 2uasimojo/HIVE-1589/cleanup
2c00ecf3b14d92d9c8f23f1ef3d0d7da7efdd8f8 Clean up App-SRE OLMisms
6cfe9768993779579a4346458f2133ea9d5e53d9 Merge pull request #1507 from abutcher/privatelink-hotloop
221234d8fa19107fb167a185862e90272decf466 Merge pull request #1494 from 2uasimojo/admission-v1
bd1b7f8f2237a993ef5ff927ffd7a574c2fa2a55 Merge pull request #1508 from 2uasimojo/remove-unused
e77732de27c5d5e8e0eace1764c737234700e35c Remove unused ReadMutatingWebhookConfigurationV1Beta1OrDie
c0b297c50e9274d361046a6b85d40523e027b52e Remove spaces from expected.
7f3cf67bbf51d4c1d0a1b5cd30704a88c9c31703 Update pkg/controller/utils/errorscrub.go
703415cccd0ecf97dbe0f2d389cff346ecbc14c7 More updates for k8s 1.22
6b9840dd82240f660e4cb4f86b9e2e350023e303 Replace identifiers in not authorized message.
2fdd1f4d0954c419dfc35ae0922caa236ee6a1a9 Merge pull request #1504 from 2uasimojo/HIVE-1588/patch-hive-ns
7bc080db26b85524ff06669df7b3536101d4fb04 Update pkg/controller/utils/errorscrub.go
f8452f980adb68c99c7648739c3c7e91e565ef8e Scrub AWS not authorized message which includes AWS resource ARNs.
5b0267e547c460134aa6f9c8b3e1f3c574f4e26d Unhack: Use a patch to set CRB subject ns for direct deploy
bc71ecc5e9bff421cef8e0b9aac88d710ca0869c Merge pull request #1503 from 2uasimojo/HIVE-1588/restore-dedicated-admin-aggregation
ca28d1a70f1ae82ee180d5cf2cafa05b2763b1f9 Merge pull request #1502 from 2uasimojo/issues/ocm-backlog/15331
f632659142bed56596e19dab42c6cc926a41f7dc dedicated-admin ClusterRole aggregation for direct deploy
1c794f8591c5e814d82cb604720fdcd3ae1a2068 .gitignore: exclude *.out only in repo root
efd31ef240ef13bf9ba0fb496d2eac027508f2af Merge pull request #1501 from 2uasimojo/delete-ss-clarification
c5015e12ab3ae90fed68dfac67ab8529231d407c Clarify resourceApplyMode: Sync when deleting SyncSets
37988ea6d561c4a148170186d7d2e52ef987e2e5 Merge pull request #1497 from dgoodwin/reqs-met-metric
3b7f9c6320a41a05096e722e3cd4d23ce0883152 Merge pull request #1491 from 2uasimojo/bmg-imagebuilder
71087dd102b7d6dab9c57a76a7ee988e53de20ab Merge pull request #1498 from 2uasimojo/HIVE-1588/rolebinding-namespace
745052a2e9b39cf83e1f8bf3b9ed20d977cd6437 Merge pull request #1484 from 2uasimojo/HIVE-1058
5810d0dce62e228b8ee8811148467a915264285c feedback updates
063ded5e0d8582f2f8e4ba5bb652e929d11a9bca review updates
709f97643f288d832e989c95efb1440cac6ab962 Add RequirementsMet condition to provision delay metric.
3dc3c3c7ca4bc5737836252f4ae0b7b0fadb1e99 ClusterPool:ClusterDeployment version & condition
75d0f587695b0fb5abab3bdca9af485e489b200f tweak
c8367c535713d24be2b7bef8274b9af85ca70583 save
f5eca7d718395c5edaa4225d13ff162792fe61d3 Hack: Hardcode crb subject namespace for app-sre
aba0584f3844d600d28cc3c0b5f83ee5ea7cdaa9 Merge pull request #1495 from gregsheremeta/add-worker-node-install-log-regexp
2f3f7703aafb3cf2c15a2cb99e8e0df44a67d551 add NoWorkerNodes to install-log-regexes-configmap
855a64060f0bb2cb8866bf7dd0619462f1e14c5a Merge pull request #1496 from abutcher/HIVE-1625
e9a970e13dfac0616eb1c602079acf8c887baab6 Include CertData, KeyData in TLSClientConfig for ArgoCD cluster.
ed4d2b35e5b69bf7824938620327c365332db35e Merge pull request #1474 from 2uasimojo/consolidate-claiming
4e2e663cf7abecaf0f593b6473327fcf90715006 Merge pull request #1446 from 2uasimojo/SafeDelete
c8a5714353bbc6b13230eab2b8b543a1d7c57d6e Merge pull request #1489 from 2uasimojo/pool-controller-claim-conditions
b6494f74987e8b05559eee2642dcb1c5c6bf5c41 Merge pull request #1486 from 2uasimojo/HIVE-1588/direct-deploy
aad9706a13e0eb163231fe10a79dc239246a16a6 Merge pull request #1493 from dgoodwin/dns-preserveondelete-3
06dabb555ac816ad4c8057b39ae96e7d09e9cfef Fix transfer of PreserveOnDelete to DNSZone when deleted.
cfcd32cb8ae7a077ff8cd4244b3f0a4bc7dce4ab Update bmg, remove imagebuilder workaround
f40614fae9eb4b14a09210709e649e3274d7006a Merge pull request #1490 from dgoodwin/err-scrub-cert-warnings
511422f0c941f9e122c1a3dfd81e51fcaf0e18d6 Scrub errors for clusters unreachable due to cert dates.
8ffc028cdbd9b180f986d2910427ea367e805cce Merge pull request #1487 from suhanime/hide_internal_crs
d8180cbf2d77f4f7c46f6f092d9f2f01f36b992a Consolidate claim assignment into clusterpool_controller
f5d877b31826cca106883c5e985a35592073fd1f clusterpool_controller: Verify ClusterClaim Pending condition
3de9e02ea6c5c8b468ae4558e170c3936e45098a Merge pull request #1488 from 2uasimojo/nix-clusterdeleted
2011220a51e0be719e3d3d5a1481c9e66dba048f Remove obsolete ClusterClaimClusterDeletedCondition
93e02ef3c0ba91ba7a5db43dc6f33ac6a7f6b777 Add templates, scripts, targets for OLM-less deploy
b54dc95b7a81c59866c9d6b027e4f6af714d3e04 Update the docs
44790b5dd098c6d1a6f114932c8ae636b5352dd5 Hide internal CRs from OLM UI
5990617a5f027cc834f1b14d6a0ece0c7dc35696 Merge pull request #1483 from dgoodwin/dns-preserveondelete-installed
2f60df7bd82d64261649058fe45e3ec83fcf065b Merge pull request #1485 from abutcher/hibernation-controller-hotloop
1240ed436e84dff3a213c723d8576a6892a27dae ErrorScrub message in setHibernatingCondition to remove AWS request_id.
e555b91e6ffa43104481582745b834628c013cd4 Move full DNS zone checking earlier in clusterdeployment controller.
57147b24cb33b05de91c8070b459b66c24556e06 Merge pull request #1482 from 2uasimojo/HIVE-1605
40c30ab549edc8d2e68614259fb7f6ff0e5de1a9 Merge pull request #1476 from abhinavdahiya/private_link
4667797f009be631081e34c25ef4de6cb9498d04 Introduce e2e-pool test
4cefabc23bcd8e8ff79a12982cc30c7eff340c6f Fix transfer of PreserveOnDelete to DNSZone for installed clusters.
d6f5956a8f59994cc6e80c8acacf83b93fff80bc Apply suggestions from code review; mostly doc fixes
34d8b527b80acfb55701034adfff9caf978e3326 Merge pull request #1481 from 2uasimojo/bz/1989129
1edb014dd3828ff716dee30f74576f7046d736de docs: include a dev guide for setting up private link network
4d8d83dcd46406bc4ff1d6c7708eb7e07dc23727 Actually start hibernated machines
e4ff496d0c095384325c8d26c8dbbceca485d73b Merge pull request #1478 from 2uasimojo/sort-crds
afaff39ed2fba9acc9cf556ec11c634cbdf6cba0 Make owned CRD order deterministic in CSV
28f67bab3dac5fb9dec405e0536d64187faf964d Merge pull request #1477 from suhanime/hibernation_bug
28b65917986be39288621298992155dde796ee2b Hibernation bug with fake clusters
a9b5cf05279e0c81d3e97f187e11319c9cb6f783 hiveconfig: allow choosing dns record type for private link
63c215a175c95bf9c77da74d4dca30ba0c2ead15 Merge pull request #1447 from 2uasimojo/claim-ClusterDeleted-condition
8df60ac1564005c882fc40ec69bd799e88ea9768 Claim: Add ClusterRunning=>ClusterDeleting condition
83b25ab6d89e07f9e5aa3f08d5bd6c20dc1a9b88 Merge pull request #1471 from abhinavdahiya/aws_public_subnets
ce6423aad8f36ac3c52feb5a1eaa96a940c45114 Merge pull request #1472 from 2uasimojo/fix-clusterclaim-tests
625164b626c058be6278463ad6a2201bbc76c2a7 Merge pull request #1475 from gregsheremeta/fix-appsre-build-hash-grab
c28d2ec49f5bd40ed8e4c8e7a1f765851a0eba69 fix app-sre build script current hash grab
029ebd266f176150ae823aee40f64b37c075dc74 Merge pull request #1473 from suhanime/remove_office_hours
d42601f41bf8317bea10ef440e1e1f532748e446 Remove Office Hours
9298d51f61e77d879ccdde05a263bd5168190e2b Merge pull request #1453 from abhinavdahiya/hibernation
fd6d5aba2fce5af7d7df29df4ddf0d216af7e1a9 Tighten TestReconcileClusterClaim
0736fc38c28c9a2719a48f793275053ab3331c32 hibernation: support hibernating spot instance for AWS clusters
5422b69102dd0a57fe4144012ce041b5cf88ec37 remotemachineset: aws: fallback to using kubernetes.io/role/elb tag for public subnets when route tables are not enough
5bd11185afbfa5dcaed394d0b91ebcf67688609d Merge pull request #1460 from 2uasimojo/HIVE-1592
bc16f9a8affe9fa259974ea9372b136f6a36b1ae Merge pull request #1470 from yithian/GCP_service-account-count_quota
7f572d71bbba0e6df071bb60dddd8207ea78f91d catch failures for iam.googleapis.com/quota/service-account-count quota
00114dc339bab505df8efcffbb66c2c34d163753 Merge pull request #1468 from 2uasimojo/crdv1-fix-apiextensions
ac4b08cd8ebb175a8ac57231c33ce9b9d3d51b24 apiextensions s/v1beta1/v1/
e233d1e3baa7bb007483c338a1430ec991a3b435 Merge pull request #1465 from dgoodwin/dnszone-preserveondelete
122be6314106e74c5f287e0253c4da14efe2ec5f Add PreserveOnDelete to DNSZones.
7a06eeaa5fdb9c19baefdac4f63ed80853e2e0da Merge pull request #1466 from yithian/patch-1
03bc3a602fe982016926ae56a1a7b00a4baefbbf add a match for GCP CPU quota
bdc09013888d4adfb50ae974a432ef4d8b392e77 Merge pull request #1461 from 2uasimojo/bmg-deps
a398d4930513adec13c48c3d84b9ff33c97c8bb8 Merge pull request #1464 from 2uasimojo/index-cds-in-pools
9f4d579dd1bdb5ba0f091be69a12d0dd9d81a4f1 Index ClusterDeployments by Pool in clusterpool_controller
42d924f79de81495350fb9622fc0fd286579efb8 Merge pull request #1462 from 2uasimojo/typos
5d1b6c157c9813a65c849fb068ec8651e8ec2c69 Fix build-machinery-go dependencies
2162b3f29692e9419c1f4b3be45a9c174ae54bfc Fix some typos I noticed
a747efe7bb77765a9a0fce3c6aaf72f70ec47d56 claim: Consolidate ClusterDeleted into ClusterRunning
667abfc4ca5094c2efcf62d1cefc720544284a76 Merge pull request #1452 from dgoodwin/aws-disk-enc
1a56e6d1ccaff39104f73d78472827f0fbf1bca7 Merge pull request #1456 from suhanime/hibernation_clustersync_bug
136d1a15d38abcbd57e6561232a73a183cbb6827 Merge pull request #1457 from 2uasimojo/duration-format
700f63827fc9573a3e2f9e559caecfb898e28f82 Merge pull request #1458 from dgoodwin/optional-admin-pw
8f1dac326ece5a6312aa5419cf0657b99b2ba9a4 Enforce format of Duration fields
b053401805e3eeb28481c6cd9e9d8eec5aef6760 Safely delete ClusterDeployments
ed31af3549240a99b1cadc9b4c728e607d7fd344 Make metadata admin password secret optional.
3cdbf3097afee27ed20feb822c60ee72d71c91d4 Merge pull request #1451 from 2uasimojo/controller-runtime-latest
dc6fd60c3f710bd9334c21b05de6b8eec2931450 Merge pull request #1455 from 2uasimojo/duration-docs
e078674d98e2e2ebc6f153b5bd9ddeab044d2fc0 Merge pull request #1454 from suhanime/azure_dns_error_scrub
7d67ceb10a76f58b76bd41ee203b3ed51c0a3a39 Scrub frequent Azure cloud dns errors
15fa1565fe144c962947bde8194cde1c8ea03917 Allow clusters without clustersync to hibernate
5246a66d9347a3c04ca142976d04d293ed5d1c4e Test updates for new controller-runtime
c936fa1916d3d971edc3a104cf7f270f6fb99c3a Document Duration types better
54262c1c9f9857d829bb6beba5bae33fd2c2f63f Update controller-runtime to (unreleased) master
2ab83dd83936cda759d74c4641f39d1a75fd5da0 Add support for custom KMS key AWS disk encryption.
023f095eaf99afeb730b103f6881ef081c7ac88e Merge pull request #1449 from dgoodwin/argocd-deepcp
8cc95d025276c7f646f90b5f297744693cb6154d Fix missed ArgoCD config deepcopy.
8886f3b8e2961dc4365b92fa7cb36abf70ae4351 Merge pull request #1450 from 2uasimojo/go.sum-for-1.16
b9be4426a2160bbee3c30a36fbb908d591715f21 go.sum updates for go 1.16
616301492b6f2ff2e9eeadc156d4b780ce0f04de Merge pull request #1441 from 2uasimojo/HIVE-1579
9d13c73567de53bd11dac7d83ba3bbc7b40c200e Merge pull request #1448 from mrbarge/add-backplane-option
c50900b750bc2fc154245cb9ac2215ca26c6645a Add optional backplane escalation for logextractor.sh
c680d719e76745afd2cb0a749f543b1379719f9b Merge pull request #1445 from dgoodwin/cleanup-provision-failed
99c8620347b372f7f14df9259d807b0720132147 Merge pull request #1444 from dgoodwin/doc-cluster-adopt
49b5837aa081461f61ca9b3930ae95d2cfab47ec Merge pull request #1439 from abhinavdahiya/hibernation
97aac4854053524391eebbbcda0dfae88d706733 Merge pull request #1443 from suhanime/hibernation_fake_clusters
cd06ee7cccace552211b47065c3168ef15326628 Merge pull request #1442 from 2uasimojo/update-bmg
1943d31aabae6272be3c986cc41f50db64d401f8 Remove next provision details from ProvisionFailed condition.
969000264f6f59b80eef1d671b750b4eaaf1d919 Fix adopted cluster crash assuming unreachable condition present.
89117b4e9aa7f337f7e666147c6b19a8c45229e2 Document cluster adoption.
4614181b653322e9e97d0fef3c69df3aa695b278 Merge pull request #1436 from matt-simons/patch-1
45aa0f1bb0d3bb7cfc16355109fdb4217ea7730c Update build-machinery-go
8b6c3a54424255f3e0207000f8e66e344cef3d5a Simulate hibernation for fake clusters
4bfc3c43d9af3d5280d61ffe8d63cf7f67cdaab7 Build against go 1.16
3e7ab198a8cb01ca65f9ed63c4693cd85b2951e0 fix panic when metadata is nil
bf40780e4046c623096411568b9473ab117981b8 hibernation: update in starting/stopping progress conditions message
db4ec31bcb20e3e4f33b4948399046a33316b9d1 hibernation: include machines in undesired state when hibernating/resuming
0c2ddbd8f81de9979e123e3bbb027c0775aa5433 Merge pull request #1438 from suhanime/dns_panic
2e31d22a974814509e215542d1c270ff516b9dcc Fix panic in dnszone controller
888dae55d3d8259b7b6dee6b0eb4f6c0e64e3149 Merge pull request #1437 from joelddiaz/dns-conditions-on-error
b7a8ccdabed370563df1b33a63cadca86aef6355 go.sum changes after 'make' (go 1.16)
96a47a0e86a99d305fab5f47135bcd12054bcc22 handle the possibility that an error isn't an awsError
54d82744ac5253ff262a8de6061438ef421573d6 Merge pull request #1432 from suhanime/dns_cloud_errors
54c38447b6fa817c8fac190778e5667ddca07062 Include cloud errors in dnszone condition
697460baf215c1231db81329d57311d137fad456 Merge pull request #1427 from abutcher/HIVE-1540
33a351370375f500e82816e8f4ca90205b9627a9 Optional default ArgoCD namespace.
1e3f8aa4c6cdf96eb237737bd123160c6e0fb674 Merge pull request #1431 from 2uasimojo/update-e2e
6ca8b33ca44fd8ce45154ae9779c1058f2c884ec Update e2e-test.sh for ClusterPools (step 1)
f70e809370f99dab281c7d4355bb95919f2784d5 Merge pull request #1430 from dgoodwin/cd-conditions
96b5f0304f0f2113e34e84a73f78c94a6145e7dc Remove ClusterImageSetMissing condition.
aa52a29be046830ef27b59b586ab1fd08885348a Comments and use ArgoCDEnvVar for enabling via hiveconfig.
6d1a2778655a682e3a68a226e4b737ebbe5ed1ea Merge pull request #1422 from 2uasimojo/no-more-IMAGE_FORMAT
490532eb9b781b370c333a22f20ffc7f01308675 Merge pull request #1421 from 2uasimojo/coverage
46b9ddf645cbadbfe464bd8c883988c63fa5d8e9 Add argocdregister controller.
9f0da30641a041d1872e2ab459253feda06c4c4e Merge pull request #1419 from 2uasimojo/hivev2-kill-velero
45d686c8fdb488d0bb46f8f3750660a91e35644b Merge pull request #1425 from 2uasimojo/nix-ci-ext
f9be99131a5fdeafb2be34bed971fc9152cdb105 Merge pull request #1424 from 2uasimojo/kill-hivebase
15f64510297471a9035225fc64815a2fe971cfac Remove hack/app_sre_pr_check.sh
f7b6ee632e14cd0361ef57aef4de96faa481973a Remove unused Dockerfile.hivebase
3c6d4925528579438a3ba5a4ab4a3cfc5b651425 Hivev2: Get rid of VeleroBackup
d37960ac3986cd6ca04b5703d6b59cbc711fd50a Merge pull request #1423 from openshift/markmc-privatelink-doc
b3b7af6c9fc17e1e95a432dfe2af4436aed0b3a9 Fix AWS docs link in privatelink doc
bdf3bd99ead286f306813e56f4fce5a5760e9c88 Merge pull request #1418 from 2uasimojo/hivev2-doc
b08fa46a17a4fc8a8737ba7b1578136682a5e4b0 Merge pull request #1408 from suhanime/initialize_clusterpool_conditions
ff120e6c1fc854d94541f5e6e520b8b9d5c8db2e Merge pull request #1403 from dgoodwin/region-checking
49701db3a59d31516d7104303edbd7d874357bab e2e-test: Stop using `IMAGE_FORMAT`
6abb8fd78233de86d1b24cdde6c1dd9f19af65c5 Merge pull request #1420 from dgoodwin/fix-gen-operator-bundle
c92648366cfc9b49b259ffd2ebc657ae43c94350 Add code coverage script & make target
e045b0815274aa3c9f2d60a6fcd55022fc706f3b Fix operator bundle scripts for v1 CRD schemas.
f7bf5b1e733e49e772bc30dc706396fb19a8c02e Merge pull request #1395 from dgoodwin/v1-crds
ee3d38422e425bc4c18a8ff2ff5d3f550297766c Validate region in InstallConfig matches ClusterDeployment.
695585a3f1e40621e6ca3d2feef1b47a938f1323 Improve handling of RawExtension as embedded resource.
6f84c3c7bc57aa44b6610bd97748c9591c557031 Stop removing resources from CRD definition.
966b40e5687d82a2d70bf24703ddca8e87d864cb Preserve unknown fields to fix SyncSet Resources on v1 CRDS.
6aa42924bb8baa0f48ab91181cadf18c0cbcb841 Move to v1 CRD definitions.
7586eab5df73c8045f6621db222bca22d7262995 Skeleton enhancement doc for Hive v2
1da8686c66d6d97e0498b4596ad4b9040ae8073d Merge pull request #1417 from suhanime/initialize_machinepool_conditions
f00e376800ff53a6030a65570f4bdfadaeb63221 Initialize MachinePool conditions
e2c2ee450585f7a652d5614f2865ffeaf1a4f5d2 Merge pull request #1412 from akhil-rane/update_preserve_on_delete_docs
21015af705ee297f9d84e94e391bc9d8f67626d9 Merge pull request #1415 from 2uasimojo/velero-mostly-equals
d6e4f1685349096bc8e844f978401bbbd6cd9d75 Abandon deprovision for any cluster when preserveOnDelete=true
d5c3190ca4a54128202bb71716326c1c88d86c87 Fix velerobackup tests for DeepEquals
8f5cb7f276345253125b3604d5b361ac8cd5569c Revert `999` workaround for velero tests
0cb678de857459fbb9267c33ec19af56dfaa71e4 Merge pull request #1414 from abutcher/default-release-img
ba15b21b7f850aa999450fa71717c59bc7f094af Merge pull request #1410 from 2uasimojo/mostly-equals
9af7bbf17ad4ca9bef51a969774bb4d4d0bb6256 Update default release image URL.
48b81ce9c350521fed4a2872f215284d90af44bd Initialize ClusterClaim conditions
3c57723f538887a124852bffd9b7dd0d9070c852 Initialize ClusterPool conditions
a2c383ad7881106555c990fbe9a27ecdf97d8560 Merge pull request #1409 from gregsheremeta/azure-managed-dns-docs
759548bac58257153c0597bc2983f8e23332ee82 Fix clusterdeployment tests for DeepEquals
b81803163647a7ee69961f7652e2e188d0377180 Merge pull request #1407 from dgoodwin/controller-runtime-0.8.3
1d90a7598fd5e9111de32c10ff9ac5a1565c2197 add Azure examples to using-hive doc managed dns section
e79a4da8c43ae6e68694714a6b4bab1e86ba4393 Merge pull request #1313 from 2uasimojo/HIVE-1456
c7d60527612c141f58d748b8bf2e25d72f9499d5 Test fixes.
51493dab6715f428da61f3c83f55fb20fa519e1b Update to controller-runtime-0.8.3.
9e338a97ab83b5dc16a2c076df70ca82f248e1b9 HIVE-1456: ClusterSync: Status & Message printer columns
0ce908454afb2023f9669681b2e9dc8942390f57 Merge pull request #1406 from abhinavdahiya/machine_pool_status
933d88e968bab074bda14f02ef1eb4ed366f1887 Merge pull request #1400 from abhinavdahiya/rate_limit_updates
5bdbce0da273e6826ff43919ecc03e062ab5ce99 controller/remotemachineset: summarize failures from machines
579e6ab6094396d601b97ec487feeb22e128aed1 Merge pull request #1404 from abhinavdahiya/rate_limit_updates_cd
508bd356f7dd919c225cf5f5342187477aa92454 Merge pull request #1405 from dgoodwin/back-to-envtest-1.19
26eacb4ca3badbc3eeed99d8935b824d8a45593a Revert "Move to kube 1.20.2 for integration tests."
4376099acc9c78577b1609347655c98bc98def28 Merge pull request #1402 from dgoodwin/envtest-1.20.2
e666b4cd278174d743e7a6b78b4e2fee9d48d959 controller/clusterdeployment: rate limit updates to clusterdeployment because of error
06a81c0ea89b2d289943a8b0d4d918c60db58470 Merge pull request #1399 from akhil-rane/hive_operator_panic
6f1176c5c09fee19559e91869a36e51604e2e502 Merge pull request #1401 from 2uasimojo/add-efried
82f98f2425c871ea945b253d078adbba48fcdd04 Move to kube 1.20.2 for integration tests.
0432a8e34f7085f0de6f88b484613ceb38f7d72d Add 2uasimojo (efried) to OWNERS.approvers
c6db6f1aa0ae6fa73f25b57d4294f6c70d6724a8 Merge pull request #1398 from suhanime/sort_cdconditions
9513ee62000871ebe8dfedea1396ff9d0e9b1e6e controller/dnszone: rate limit update events from cd cause by dns error
70444e62cfcd5ba493dd0e0e9a8fdf77ff1f0492 Sort clusterdeployment conditions
1d570a5db1c86b885ac2ae4cdbfd13dde63f5495 Fix panic when hive admission serving cert secret is missing
1f33d9f2ba783dbe1647019fa707b7762fdd2359 Merge pull request #1397 from dgoodwin/envtest-update
50940e29fb2ec887b6ae4df168bfd423ab8b383f Upgrade ancient kubebuilder envtest tools for CRD v1 support.
c6ca3dd7d0e4edf7760f346435ea97a2ceeb6a86 Merge pull request #1393 from abhinavdahiya/rate_limit_updates
cd936a732faf7f9920053749402646867897cfce Merge pull request #1394 from suhanime/metrics_change
0cb0df7b1f029bb80ce0a721e568cb9862380731 Merge pull request #1396 from joelddiaz/fix-openstack-autoscaling
0ccd08169a794c57fac7746358d39d9df8a15e46 Merge pull request #1392 from dgoodwin/lower-lease-dur
dbd85ac2bcf37ed4d37014982a443a3ee073a2ab fix support of OpenStack autoscalling.minRep=0
0dd2728d5ed21c18787966a39df250066bd3c730 Metrics change to accomodate conditions cleanup
2c8455e048190800771cfec8e56b9f5c5969d319 Merge pull request #1381 from suhanime/initialize_conditions
fffedb481b9d3a46ebcbdae1cbdd5f7fffc1f787 Revert "do not include error message in status condition"
9cdddc351143564ccb435a1b1b04a9ea53e711ea controller/dnszone: rate limit UPDATE events that are in error state
2d314cc8af6a07efbf1d2bbaf6d61d2c2665385f controller/utils: add event handler wrapper that force rate limits update event
51649bfa6a31c51849a637651466e88a7b018c1e Initialize all ClusterDeployment conditions
356f6bf08f83e01c91eb80743abea9ed7ab761c0 Merge pull request #1390 from abhinavdahiya/restrict_release_images
e7b029e563c80a0400e8db4fd47dfbf1a189d0f6 Lower leader election lease durations.
521155fa756c3a55ffe28cf09a1fa05bcae458b2 Apply suggestions from code review
5cce7e2bf9d89170d520e6b93330b346b8d4688e verify release images used for cluster deployments
3493135392131af08b835c6e6cd62b35251ab8d4 Merge pull request #1389 from dgoodwin/dns-govcloud
3f862b166c24080329c3aa7c64b09fd6056196bd Update to aws-sdk-go 1.38.41.
62b91f0a61bc15de101d6c99e3e757f7bb05b295 Merge pull request #1387 from abhinavdahiya/image_verifier
e032492355a64bf2396d9a6b389587d58055a68e Merge pull request #1388 from joelddiaz/dnszone-status-error
3cdb681ed462a65141ec573440ec117bf674281b do not include error message in status condition
fb7117f720fb3a38641a36c57310a7087a21c9d8 Merge pull request #1386 from dgoodwin/plink-early-delete-bug
bbda8aa4cb54cf6b7bd622e79f08aebe6e5958b8 remotemachineset: periodically reconcile MachinePools for update
6cd6972471d01f01b20aaa5cf0ccfad34279d0ac Merge pull request #1385 from akhil-rane/expose_hiveconfig_conditions_as_metrics
c398a92ef39260796f1efd37d54f9e78ebfe0d73 Fix stuck privatelink clusters deleted prior to install.
acc5150929c7981377aab220faa86c652c9a015e Add metrics controller for hive-operator
28ac7071318a7f904242b3d544bd519ec9fec76c Merge pull request #1383 from mikeshng/doc-fix-install
c0bde6bf6e53d786a108cf9bd6e49b288c3c0f5f Merge pull request #1384 from joelddiaz/zero-replica-with-zones
c0d7289db0113cc5ba66f5da68ab7ba55ffb7088 allow to set zero replicas also when zones are set
19a8e6b451dfd68e9a8d1cb41401917d3980a1df doc fix for install.md - format HiveConfig yaml sample
1f7e5466cd2b834a96e73a51995fb42687fc8546 Merge pull request #1377 from akhil-rane/add_hive_ready_condition
b9fa5a80b7000e8f85ed945485cd75b5865f197b Merge pull request #1379 from dgoodwin/clusterinstall-ownership
936cfc14f87fa78c13c6ac6a53809edeb3e3af99 Add condition to display status of deployment on HiveConfig
1fdcd8781d1fa0d8343c8d638e474cebbecae9f5 Merge pull request #1380 from dgoodwin/plink-err-hotloop
cffb9ff0d4d28ffd55fe20e01a69ecbdbf58f8f4 Rename setProgressCondition func to setReadyCondition.
86ac6d003ed87ed3ceeff1a8f4ef42827bfd54c3 Fix hotloop in awsprivatelink controller in some situations
ee3226e09ab955523f633f3e028cc74bb6dc747e Merge pull request #1372 from suhanime/utils_change
c7dbe2e081c644fa490bc5705796f3cea346df83 Set ClusterDeploymentCondition for all status
6b04e34eae97ec63d6c306dcf22c5279c1938830 Add owner ref on FakeClusterInstall.
52c939136a0e5a34781888356e119e21df4a87e1 Merge pull request #1378 from akhil-rane/hive_operator_metrics
17de86b02b2ba29ac1758eeb9110d7a6c4a92850 Add prometheus target for hive-operator metrics
5c038fb051906a7c2d733e7b017690044c66c124 Merge pull request #1376 from akhil-rane/fix_cluster_claim_on_fake_clusterpool
1d9c87a6ff2bddc8c77fb72954b97868fa73d83f Merge pull request #1375 from abhinavdahiya/image_verifier
f128e51d8c60b00d9f49d11b402c19bdd82e1821 Merge pull request #1373 from openshift/cluster-installs
8f211caf7024e9e540817c64b48973913b28fa89 Merge pull request #1370 from dgoodwin/remove-clusterprovision-podspec
6ea7e05773450c7b201ad3c26eefb8be18f1b67f Merge pull request #1356 from dgoodwin/install-strat-enhnacement
aa2e1ec149123072a3f36942cb2c8e9232f48bf9 Fix cluster claim for fake clusterpool
15bcfebbc46911a52e226aafa9ac67d200eeb9c7 remotemachineset: requeue when we not steady state
6a14af7315590a483eed76f8e7300087991b64e5 remotemachinesets: sync ready replicas and errors to machinepool
9804488df8aa7fea27463a7aed411698c0e04c7f Merge pull request #1360 from dgoodwin/clusterinstall-apis
2e18329d9d4279640c12f265df735868bf51fa87 Merge pull request #1351 from abhinavdahiya/aws-private-link-controller-doc
d8cc0c8351038c0c2138e1bb2db2d3ee012b8e67 Merge pull request #1355 from abhinavdahiya/aws-private-link-controller-cleanup
a45f39b8a88ffa2e14103e76e03d9621bad50b36 Merge pull request #1354 from abhinavdahiya/aws-private-link-controller
206ba8b48b05956040091c0872b9cbc991e88e38 Merge pull request #1364 from suhanime/conditions_cleanup
ad6aff41df0fb349682a9c5ae2049892f2c541a0 Merge pull request #1371 from abhinavdahiya/pl_name_tag
9e8f83bfc418f50861d1e7a743000f4a0c40945d Add missed role for operator.
49a8d9f868550a1d46eca820b7c5098b91cf843d Drop unnecessary logic in admission hook.
723c0303d8f0321f3a2137c3a731be464a33db4c Initialize Hibernating condition
ffc59a4272b4e42f0b039718e0236a790ef7eb97 Remove unused function in fakeclusterinstall_controller.
1b78f293e85183be221aefe2342e3f9649d66ca4 Remove unnecessary ClusterInstallRef check.
fafc1b51b9d2051da257e7a6e69db6fea83d5538 Move FakeClusterInstall to internal v1alpha1 apigroup.
4e238962d49c66497a7636b38df20ecf5fbb8047 Merge pull request #1369 from abhinavdahiya/cd_watch_duck
1b6bfa0c028857c71e1a01dc2a06a73f7dba1146 awsprivatelink: add Name tag to endpoint and endpoint service
6ad1ad135dbea8c9e3a9673df09137de3c7ee610 Hide massive PodSpec definition in ClusterProvision CRD yaml.
bc86f04dfebe514b2afefd1d1ad9dc6fc52b1369 operator: support already known contracts
ed6a7675eb563cd90c2ebd72a2b38b4ff76d3579 Merge pull request #1368 from abutcher/HIVE-1498
d5b066d39c7d00acb05769c4935c0f8ea3554210 Merge pull request #1367 from abutcher/HIVE-1490
10ea1317c7198b64476faa12db34b02af1b0a6d5 Subnet install log regex made more specific. Added generic install config issue regex.
3462786f55cbab6140c0bd968199087352afaff5 HIVE-1498: Add InvalidSubnetCIDRConfig install log regex.
8c3dbf7dc221d00b25efe575709dd656031eab42 Document required vsphere params && fix incorrect error msg.
92c7b441126b960d1afa2b10a90caf9971382a2b Add note on how deprovision should work.
f7268df647dd2ab03297feef77ca16e41451e8bb Remove comment that AgentClusterInstall will live within Hive.
4818f0b604c6f546ca5fa90e72327f96ec552ada extensions.hive.openshift.io for RBAC
40b1d9239ea4a5e3b1e791d6c319d67111358c05 Fix a bug in the fake clusterinstall controller.
9fd648e713ed9b2fbe405d1f102052c107fa59e4 Add patch to label FakeClusterInstall a valid ClusterInstall implementation.
2251b86753b8716fc8dab75b83978042a8301f34 Add RBAC for everything in extensions.hive.openshift.io.
e603852bd3199c3e8da5cdbf1132656662ee8c09 Drop the AgentClusterInstall, moved to assisted-service repo.
9bb78d22f0e7a5ca60ddce464b809ce1a0585501 Improve transition of Completed/Stopped/Failed conditions.
f564ca76c77abca992bf11b7be567c28035578f0 Move more AgentClusterInstall structs to Agent sub-package.
33f9a2541789213e495be5f4c36f1866c473a346 Move APIVIP and Ingress VIP from platform to AgentClusterInstall.
76a1bec7ede3a5303dd513630e2d2a5f4f68d1a5 Move some Agent structs back to the agent package when possible.
bd43c227e71cd4f159987765c05762e0042434ed squash
61bdb97329e43cb630dc4120fb6c7dd584d8a9a9 Remove InstallStrategy and move status to AgentClusterInstall.
aa169c7172d831d0c5e57bd9df00feace45c0f29 Controller updates.
2e554bea263485e1c68564a330046687bfb9c467 Drop hyperthreading default, not valid until we can move to CRD v1.
48b7c09dc9033d3037a1017f658f4d28fdc6de3e Add hyperthreading for AgentClusterInstall.
b6174386ff6ec155cbae88328418ec2575b56c6e fix controller tests for condition dedupe
45852d297e8b02c85cc29fead982a5cb6c391e68 Deduplicate definition of ClusterInstallConditions.
4cbd1390d884aeb387b3a465b4920f39f1613df5 Add AgentClusterInstall.Spec.ManifestsConfigMap.
af4433c0562b5cf1fd6b098b6df11c2cb5616b7d Add draft of FakeClusterInstall controller.
83de1b132782ed166773661fea23ed0463f54f72 Add AgentClusterInstall and FakeClusterInstall APIs.
b4fe2f329d575cd342ac5fe471a763115c7c86f3 Merge remote-tracking branch 'up/master' into HEAD
e906999ec6ed954a682c0719125d426b352cb0b1 Merge pull request #1363 from abhinavdahiya/cd_watch_duck
0db1295bd26a02ccacf1114a533069ca2ceefee6 Merge pull request #1366 from abhinavdahiya/hive_op_watch_secrets
c546f5c5a4da0d8a365c6837ccc091fa3e55c9a0 operator: use the correct cache to fetch secrets in hive ns
3673a4c6a50be140b6e3ec4332b5d02a288a364c Merge pull request #1365 from jharrington22/clusterprovision-image-pull-policy
ab82585b87937813237bba16cbade5d8dd1fa783 Change ClusterProvision image pull policy
8beb29d4b2d662445c67b3c6efe46bf6ec68b253 Merge pull request #1361 from abhinavdahiya/diff_on_change
2a82f244118bedc218a142258b2936247b64b900 Merge pull request #1362 from akhil-rane/improve_syncsets_paused_status
99e9fb2955fdbeb6f1e16b2043ebd220ce9eafd0 crds: allow defining merge patchs for generated CRDs
958c8f01717dee0aae393b5fe21e59ec6fd10ffc Improve status reporting when syncsets are paused
b96c4e8d3e3efbacd3a5ca3e27d84177b9690bd4 Clarify that deleting ClusterInstall will destroy your cluster.
777353bd30b840ebe5133f42e61aeddd41b0c562 validating-webhooks: include diff when immutable fields are changed
dc7638c11719872d129236cd60c1c76caed467f1 Merge pull request #1358 from abhinavdahiya/cd_watch_duck
6ff4ba44b77a99dd51e61ffc7f01c3b1139f96ca operator: list CRDs in cluster to compute supported hive contracts
364c59619cb2cd49758436544daa5dd29459b6f9 validating-webhooks: validate that the cluster install ref is using supported implementation
5cc07623c7164ca3f67db317ec118bebe7d09475 clusterdeployment: support cluster install ref
9d21132664e1be35ebe87b9343ebaa5b9aeebd6a add clusterinstall contract
86bc4a4078b171470ef540812641228038024e87 Merge pull request #1359 from akhil-rane/regex_for_failed_kube_api
1b3c3973179a8dd54f677b88ce334ab667422212 Update required conditions after discussion.
d3a24a734e2f7390236562a4cf88154dd8aedda9 Add some required status fields.
53c884bad3b220d29e7999717f7fac3d05096377 Remove manifestsConfigMapRef from required contract.
aa77169b5a6530920ecbe82314417d9b530bcae6 Drop the ClusterInstall.Spec.Stage in favor of just conditions.
7ef1d9ccc48e03f2c342f60620ca0ee5b199cbfd Add note on aggregated ClusterRoles for external ClusterInstall APIs.
b8214b703bc571b3788be1060c49c990510b5d68 Add regex to detect install failed waiting for kube api
fb28165b0689adcf471e297ce7d77e8c17e5af2a Merge pull request #1347 from joelddiaz/zero-autoscale
b7e7b31a83e8f9f48406c4c66c821a9d90bcd602 Merge pull request #1346 from abhinavdahiya/expose_provision_log
644144e1f394068507960a2d58e04af07f64047f Merge pull request #1357 from akhil-rane/fake_annotation_on_clusterpool
a7e03048a75bd1842ed699e3f38af220f437b88a Add ideas around cluster deprovisoning.
bc04878c3b640fe574b021febd38d841dce8c852 Add option in clusterpool to set annotations on created clusterdeployments
84480b4216a2ffa9d459b0c19a29d7b7f103cd33 Skip hibernation when ClusterDeployment has fake cluster annotation
fe4c4b10b6632a7ecd2c83d65e0a0252835adb72 Add future considerations section including ClusterPool support.
9e488013f956f5724a357fec1a150c452490f932 Rename InstallStrategy to ClusterInstall.
7fd5d3fd352f11336cba35726fc2d296af180ff3 Merge pull request #1352 from dastergon/fix-mk-target
8d91c18043d40994f72b103d52a0b221ab9532eb Add proposal for breaking out install strategy to separate CRDs.
213b839b66e34cf3e9d7d40485e32a5aa300c744 Merge pull request #1350 from abhinavdahiya/hiveconfig_track_secrets
5d5607b455df10f936124bc29c8754637ce2dbe7 hive-operator: resync on changes to secrets in HiveConfig
3943b084ee92018ceec19f8d2035d30df0284233 Merge pull request #1353 from abutcher/additional-regex-data
2921f1c297eef5942d387308a2ab4f58a4b248d4 awsprivatelink: hosted zone cleanup reuse the status
8a424548d36a18f05d548b8abe9aca5cfa8138aa fix docker-dev-push target
0b29f129918fac6e9ba9b13b1cf2887fc0f9c814 docs/awsprivatelink.md: update required permissions for awsPrivateLink.credentialsSecretRef
0953660449f34d40388df9ecc43fffac987a85d5 awsprivatelink: filter our reuest id from error messages
9faf0f672dddd97aea2d34e33ac2cccb1678cd71 Remove configmap metadata.namespace and add eip regex for testing.
440f6e9705643b3a0b17b9a9355e854faa766ec5 Merge pull request #1348 from suhanime/makefile_buildah
ea6f0a2dd76c2aa48acb6d42689b6a712c38b52d Merge pull request #1349 from abhinavdahiya/aws-private-link-controller
c4c79e97ebed4248c1ad2e575fd5cc3b1785d7bf docs/awsprivatelink.md: include info on security group for endpoints
6c739726b3826c67b7df8157b424e00aa2ebc69c awsprivatelink: fix filtering inventory to correct subnets
6551ad675b904578c7292ef8c33c712e37b536d5 Merge pull request #1340 from dgoodwin/awsclient-mock-update
876bc19b957d034bbe96e28ed1f3b3272739f754 Merge pull request #1336 from dgoodwin/proxy-env-vars
a8dd174927b4265394e48859a3f39cabceb0a212 Merge pull request #1331 from abhinavdahiya/job_timeout
bddafad6173d6ef423f46431250de08683838b6e Merge pull request #1345 from suhanime/metrics_bug
499e5305ae3c986b3c5fd343dca06b1e48ebb135 Merge pull request #1343 from abhinavdahiya/aws-private-link-controller
0dba654f91cdc2c6e8b7ea6a0af1b99ee8ee72de Re-add buildah build target for dev
4b383f7878148ae76421003d404ae7d2bcc2b32c allow setting zero minReplicas for autoscaling
f211cd28bd2b4ee433b6c886514b46b03c777f19 include the installLog from failed provision in clusterdeployment condition
c1da8550590a9b018dc84e3a1265d597ce28b2ba Merge pull request #1344 from joelddiaz/eip-limit-regex
607f8dfca0e848ae838003decdd05e87d78934f9 Underway metric must report first true condition
813ef5a81089cc01ea2ce3403d67175d1b2fbb25 add regex to catch EIP Address limit exceeded
a12f5d687971331afc9539aa527ffb68d152d885 Improve testability of the proxy env var transfer.
875f780c8f5b399757c49c3b7c901336002fd7ae awsprivatelink: fix should sync to track time from last Ready update
3d85110bbc8400bcd07a96acc3d1acbcc68b3635 awsprivatelink: resync quicker when done once for installing clusters
3a8b5ee043f1c93872fa8cd36e21e944ceabdf27 Merge pull request #1341 from abhinavdahiya/aws-private-link-controller
f35934889863b22dbb01615f9a606c244e8d317a install: add active deadline seconds on provision/deprovision jobs
c5d3d24b6843f6c229e45e1e90b7a4dbddad40ca awsprivatelink: skip deleting privatelink when no cleanup required
aad5c50d5203eee14b7013eca5ec2ce8a325f625 Update AWS client mocks for recently removed functions.
eb2a798a625c156ef0f28810b70694c42293817f Merge pull request #1339 from suhanime/regex_s3_buckets
65a1f500fca20e6318c0550a158e855db52e52f7 Merge pull request #1338 from maorfr/policy-fix
6a4a87793801d50368b89fb5661a181680639d96 Merge pull request #1337 from cblecker/cis-mutable
0c6f706ecb4f096dee8ef7b87eb7f991e4648321 Merge pull request #1335 from abhinavdahiya/aws-private-link-controller
d2d79b2d63be4bd670fcdae606ccc388b17aed46 Merge pull request #1333 from abutcher/hive-1477
8818a9942e90fe54ae42b09d79871a3417181862 Check for no applyMode set (defaults to Upsert) when clearing resourcesToDelete.
397256ccd8a40fbc9e5e86b99187996b48dad0f3 Add S3 Buckets Limit exceeded to install log regex
1f665fe97c7479478b00fdee8e62a60f14dea73b Transfer proxy env vars from hive-operator pod to all hive/provision pods.
be5861d95950870e2abe83f7bc72f61e9ac65542 change aws permissions policy from dot to colon
aae3d58273fd8f104a59b0f5d4ec97677c6d133f Merge pull request #1317 from clcollins/fix_logextractor_creds
2a887e6fb7679323e9801be752380cd30912789d Allow updates to ClusterImageSet.Spec
affb485a0bfdf2ca19ec45370ad687be0be99600 awsclient: initialize elbv2 client
f0512c6621c0e5f217e19adf14a2df739d048ab4 Merge pull request #1334 from dgoodwin/required-aws-perms
8b03a05b14d1f6be92ea3c4f1620a31d42f37e36 Remove unused awsclient calls.
d6ff743fc72955e76f7b6ae8e6376f6d9de1a200 Merge pull request #1332 from dgoodwin/skip-clustersync-uninstalled
0237bac6754a1433475c6337ceb380fc4ae1a16e Bug 1947220: Skip uninstalled clusters in clustersync controller.
a535d29c4d2dc4f7f9bf3f30098c69d9334bee2e Merge pull request #1327 from dgoodwin/container-build-improvements
f62fb13aa5cbe8c16745a2080159f818697f58e9 Merge pull request #1328 from maorfr/og-api
98e608fa5b2206dd1e52d058292368fa73ad3ef5 Cleanup, formalize and document container development process.
b28419adbeb32e9270172ab86c6c5296c9527226 Merge pull request #1330 from abhinavdahiya/validating_sideeffect_none
73585aafdf3e43be77dc3eac29c3f27bede2a153 Merge pull request #1312 from abutcher/hive-1412
968160d2b4b7a257ac1eb3ab48a63383b679b891 Merge pull request #1329 from maorfr/hiveconfig
84607fa8b95ec201a165ba0acadc596d4b986566 config/hiveadmission: set sideEffects for validating webhooks to None
d458872845951cce5175c432abc2b722add9ad40 Updates from comments.
aab4f5212844a098e8b2ea3709d06b07090cf71d Restrict list to secret namespace.
7b3bcdf9089769deb689b9ab2d48c7710220b68f Use FieldIndexer and get cds with matching secrets from cache.
5d916010c1fd01e172b95505a345b203bf8a668c Sync changes to managed secrets in cd namespace to target namespace.
4842957ab764e7dbd5321fbd393ac78e41f156f6 remove HiveConfig from template
bd62efc60d68534b091eb2bd9c5a3b8a06a65488 update OperatorGroup apiVersion
7a0d63904c3f13a5cc4859e6309b621d92ff05dd Merge pull request #1318 from dgoodwin/controller-runtime-0.7.3
78df2dd46e634cd150afb411a2f4ba9037d8271a More missed filed from merge.
7453827b442e309c3b050ae0573dee9517f2e37b Merge remote-tracking branch 'up/master' into controller-runtime-0.7.3
7ce8ff441ae4cbd76caa88cb282eb80482cb9386 Merge pull request #1325 from abhinavdahiya/aws-private-link-controller
dcb7da1b9d5b27a8be4f9e1cd949c3239dec108e Merge pull request #1326 from abhinavdahiya/aws_installer_pod_creds
0f017ae1b808cd3fe73099925a415d11c34b00d2 Merge pull request #1324 from dgoodwin/remove-apis-cr-dep
6a1560e0eab6e2215a2295831fa3ff1253a4c381 Merge pull request #1323 from akhil-rane/add_invalid_credentials_regex
3d5599c6148a8b2012a1632cae7847393ad46121 docs/awsassumerolecreds.md: fix hiveconfig instructions
3d70063209d2ed58c0eea371f3abc74e6f1330d3 awsprivatelink: support assume role for user aws client
93c25da46ff56aabac27c64006d20041e3311308 Merge pull request #1321 from dgoodwin/drop-apivipdnsname
e5030791c863f93ef3c76a4238eb3b49ef5dbc45 Remove api dependency on controller-runtime.
865c5431f3c7033d017a1bd83996e3acdc7831e2 Add install log regex for invalid aws credentials
2ec4bed169da235967a988f375c6c67caa3217ca Merge pull request #1322 from akhil-rane/fix_install_logs_upload_to_s3
cd8c0e1ce181fcab26962e58e0bbb0c09f76f94e Fix issue with the upload when logs are collected using oc adm must-gather
f2eb68bca72944b777a1fea565a4bb607bfe203a Drop agent platform apivipdnsname.
360d9a8d072804e78611c5c1e417e82726129661 Init struct with field names.
df0ad9131ad540dc8a60a2f9b2d67857ce0fc676 Switch from wait.Until to wait.UntilWithContext.
e2aa2c0494f455e1d2326e36574382d038dc9c1b Apply suggestions from code review
0ef7fba7596329cb6d9d19c9d2707f0d8f2843b5 Merge pull request #1319 from abhinavdahiya/aws_installer_pod_creds
9e5539ae8bcd30f852bf5d570ef3abd956774449 awsclient: fix createing client from env when no config provided
5d6952c82c4e8837ea53055b70c78fe353221c6c Fix e2e suite.
f8bb4e2a6389e638d81b96a4d0a8d6b1042de6ab Cleanup for dns controllers and tests.
4e9e5975f5ca7e93a6a27779dce08608d4fe4427 Migrate new awsprivatelink controller.
19f6331a399a558fcde850da9d1271169b68803a Fix remaining dns tests.
43ab4d3146ddeb75c00fbb999753eab8a68130f7 Fix dnsendpoint controller tests with customized comparison.
9d625f5def50ef1af761b702ac00e718a010e31e Unit tests compiling but there are dns problems.
35ebb86515f4c1d8f0270ce51f86e06cddc85d80 Migrate installmanager, hive now building.
f9b0df03dd1d4fa2c823b6a1a141287efc617c20 Migrate operator hive controller.
dfcd411e9cf4649267d60b97dfa42131999747e3 High risk dns endpoint fixes.
aa719933ffc345e460d1a6da77c9a17ea7331070 Fix clusterdeploymentexpectations.
cb0dfd2544f27ccca303300dd2482b6c3bba65fb Fix most of remaining controller MapFuncs.
b8d6f77fbab5ac7b807c225aa081bbec1667d2d7 Fix remaining controller Reconcile funcs to take context.
136433a94e12b09473f920f8eba5db5dcce478a7 remotemachineset controller working.
f20706c81c89103472ae4d144460b54138a82a69 velerobackup controller working.
de4e1648d4078c9637ff309e1f3ff935ed23a249 Hopefully fix stopCh use in metrics controller.
1bb52de79bf889e40593723ce409569c3d954492 Fix utils use of ObjectList.
f8fcba42bd92e09c4736e4f33e9f039ba7a05108 Fix loggingeventhandler meta.
77a6d30db17fd7aadccb473ece924f1b0ed3db23 Fix dnszone utils mapfunc.
12b4983cdd01e66c7da0075eb44711c9d18a6243 Fix creation of metrics DelegatingClient.
5f11a9378945fba0cfe8fdf12c531f991517d47c Upgrade hive to patched controller-runtime v0.7.0. (not compiling yet)
d8ae8b678f3c32e53ae3de835b96577363bb95a0 Upgrade apis to patched controller-runtime v0.7.0.
fef4eee9f990177fded2253e3699561c7d13e141 Merge pull request #1306 from abhinavdahiya/aws_installer_pod_creds
5affa6b30644d7fd933d2929fd4c2fc64bde86b5 Exports AWS credentials in logextractor to fix auth bug
47b237f97a7225660933ef74a80d7bd39310ffc2 Merge pull request #1316 from dgoodwin/f33-docker-dev
79552338552d0ccd9fdbc5c769f9a7d643d97aa8 docs: add docs for using assume role for aws clusters
b153de36f202e27f303cb584371f6605de3f3ad4 support AssumeRole credentials for AWS clusters
049764638928c7eff5c13caec4550cda28bdd87f awstagdeprovision: support AWS config while keeping refresh function
a82758798e41279a519fe873477774954a9dc158 awsclient: use AWS CLI config when possible to configure session
1b951aea3b777ddf063fafe9b1753afd2ddc39fb installpods: allow using AWS config in install/uninstall
0e8725fb6978066c2fa9f0b7f32414cb4bc79614 Merge pull request #1315 from dgoodwin/sts-doc-fix
ee535cc51dff7dd4fa2f682eb0296b6dbe999dd0 Merge pull request #1287 from abhinavdahiya/aws-private-link-design
8adfa4bae87a0c50af9247f2a60549b923191da8 Merge pull request #1309 from rdoxenham/rdo-ingress-fip
38180ee3ac761885beb3533fe110b11bb0dc2c7e Remove ref to dgoodwin quay repo and error if IMG is unset.
092489c4e8b79d0e5cc6ed08204f2090e8010a18 Add a temporary Fedora 33 dev docker build/push setup.
97716a2e4f3c2cf9371998eb31a462e4253e63ce Fix incorrect property name in AWS STS docs.
1a372a5322151176f4fbcac579abc772c0fefec8 Merge pull request #1314 from 2uasimojo/typos
20072b235fab40162d1154c8512ce1f42d77c784 hiveutil create-cluster: Usage statement cleanup
391a0f02748c52719be5e15dd4548aa6f059b429 Merge pull request #1311 from 2uasimojo/patch-1
ae5d0caaa4352c6be4cc5b0bead02afe9f83a658 Tweak formatting in install.md
1070b5010c8afcb20329f13c9d01baff0a82432b Merge pull request #1310 from dgoodwin/resume-stuck-fix
e5dc3035330257c86651a1852621798bbb52080f Fix clusters stuck resuming due to stopped instance.
131179d8b0c015f6c3e6943275b981c2e9947c9d Merge pull request #1295 from abhinavdahiya/aws-private-link-controller
11c83003dde2c09b3cc08db7c710cf64ca2e1758 docs/awsprivatelink.md: add permissions required for various credentials
309025671627c03c910b25e52b844954447d8976 create-cluster: allow enabling aws privatelink
b154963a0d5c8f313921073127d437de36f4b650 add awsprivatelink controller
4622d3995174cac4ea7785f14fd48018bce25bc1 create-cluster: supporting creating Internal clusters
4bba97d4a8b4b78066263516c007549b3b28202b vendor: bump
fba304c99a8a984efe82e8003ee9590919c77ede Added option for specifying floating IP for ingress services for OpenStack clusters
fcd45d99f0d8f4cbc2af566f1ab314c03ae9748f Merge pull request #1308 from dgoodwin/sts-installs
1767abad57faacfd5118709e1d47087fa171592e Remove remaining refs to bound SA signing keys being AWS specific.
71bf751ce020751f39c4457c0531f0cc1fd42944 Docs cleanup.
8f1ce029a2927eabda8c3dd6dc3c718d2591e19c Fix proper API files, rename to BoundServiceAccountSigningKeySecretRef, move to Spec.
96333fbb6f82ce18343bc920abdd0536985a4f71 Review updates.
ef09e76b68a52c2f4fe33a24e28e4322e60aab95 Move serviceAccountIssuerKeySecretRef to not be AWS specific.
694f643789bd65048cbc3eab74cfd9d51eec5fdb Docs touchups.
94bbc330e352cd3927d9855bc7e6bb66126921d4 Add docs on provisioning STS clusters with Hive.
1a812b62c7347610f15b123c7df4f1fe3e23e103 Drop explicit roles.
5cf064b1ea7e1ecc18d0ce364b244accc10eb40a Add create-cluster support for STS.
7fee440b4d8c840e673ea579aca0c40b1d091e0a Provide STS service account signing key to installer.
0d08916e8ba760ba04c3edd9a879ae47417d14ab Merge pull request #1307 from dgoodwin/install-docs-update
e45e0d5cecffc1f07623c1fd313d730c63da9d74 Update install instructions to point to community operatorhub releases.
743e04722e53a15295cc881fb7ea2fb0921d5671 Merge pull request #1301 from dgoodwin/agent-api-updates
93da7767b9d4275ce527c86168651c0a211dc23a Fix generated deepcopy code.
813667d047802490c4e0dea6b5543510d8bdc43f Restrict worker agents to 0 or 2+.
12f703e53091663a991bee83b190861067a9ce15 Make Agent APIVIP and IngressVIP optional.
28fe8a1345b4d67d48840f842fc63fc339cfb64f Drop Agent VIPDHCPMode feature, not yet production ready.
29b843bad10c0168d529b9f759e0d066f1c379aa Move agent label selector from install strategy to platform.
b40b83dc59b4219080b042203a1b9966e388c42f Merge pull request #1304 from abhinavdahiya/fix_deepcopy_gen
4f2dcd624252d02af4dfbb4f5c264fd7da28d037 hack/update-codegen.sh: make sure deepcopy functions are updated in apis
cacb68599e974a4e72d1bc8f1323ae16d370c102 Merge pull request #1302 from gurnben/add-clusterclaim-age
3f6124cf2ff063f03b81e37f985480dbe01d7c87 Add an Age printer column to clusterclaims
3fbe20bdb3943ab3267b7a1e1aca0a5d7fd88a6a Merge pull request #1299 from dgoodwin/abhinav-owner
afbdc34e2f49c4101f5d89db0bc2bcfbdc53fa45 Merge pull request #1290 from abutcher/hive-1351
90f72398dfa23fd8fa18f05fb43fe61f5b6a6337 Merge pull request #1300 from suhanime/controller_runtime_fork
413794721e9693be4084eee19b26bd4ca91c9587 Add validation for cd.Spec.MachineManagement.TargetNamespace & cleanup from comments.
8e58ee0ce259e154df9bae7904ed15cc4b40ba9e Point sigs.k8s.io/controller-runtime to a fork
e34535e069f69b1ab43ee50f10d872e128d1f2e1 Merge pull request #1297 from nimrodshn/add_support_for_providing_compute_and_control_subnets
36370c62391b446c198dd1b030dfe5a9519bda16 OWNERS update.
c681c54696570e17897e1d06e4442958cd2670ac Add support for specifying ComputeSubnet, ControlePlaneSubnet and Network for GCP MachinePools
b4da073f127acf167e363724e5c2b8b303cc4cb5 Replace ownerRef with finalizer && cleanup.
7026427c0ae52f82840dc9a76ce5a568ff0497e5 Merge pull request #1298 from abutcher/HIVE-1394
9663a028089ae8a7dfc321d35cca045581d1fe96 Add generic install failing reason ResourceLimitExceeded.
4ace5412813f2f3afc7052928d5edc913f5e966f Check if secrets exist in targetNamespace before creating.
f92fdca2774d82d308306934ca59e88d9f02c891 Fix imports.
ffe40c687781dd84e7fb1d81a7c29054b6470d05 Move machine management to separate controller.
30801da10866a762357117272ace862d4410fe78 Some updates from comments.
8f8db654bb20d67491536c55cbdc9264de516278 WIP: CMM POC
cb7a0679e4cb40cd122f0660ecc42c5ca676968a Merge pull request #1292 from abhinavdahiya/apis_go_mod
92f29a07c4108c2ed4415406310bffcec845ac9d Merge pull request #1296 from twiest/dnsnotrdy
1690112c9dd22c0b6853b202af0d797a98cd8b83 Fix typo DNSZoneResoucreConflict -> DNSZoneResourceConflict
28b29b09bf1b211af49e9f3dbc74e39c0213a5c6 Merge pull request #1236 from twiest/hivecop
d598969b9bcae32831926a205ffec8f58426fd57 Merge pull request #1293 from dgoodwin/act-on-agent-clusters
c595fe32f24e26cf283725cc555f790438dd766f developing.md: Include steps for working with apis submodule
2b0f7aff53c8141b7d6a42d5645143807f3a4273 Makefile: update targets to support go submodules
9eef4cae259c2eb871e965125bae804b634d0236 Add regex definitions for this week's alerts
91ad2fda29a3c4707b7a3d42fa05ad7f2f0d04b5 update generated objects
3d01091643768479f15d751329a3c2c7873e6edd update build tools for apis submodule
9dcb1a4d8acc309d69e708e57f94a98f93f59f52 migrate pkg/apis to apis submodule
1a41ce2b8d03b93c29ca7360b4a35a645222ea92 add a new module github.com/openshift/hive/apis
498132b1b172cf3e56bc6138ad02199244154f6c move validating-webhooks outside of apis
70949de3bb1edb91ac7b2444d4d6660c4c8a8fdf Merge pull request #1286 from dgoodwin/relocate-docs
9ad9b166df6a77323c3a211c6343ed399d3125b3 Add some documentation around ClusterRelocate.
238530de1e53c5af8c9e968781c8bbfe6052ac73 Merge pull request #1294 from abutcher/HIVE-1387
e256fa8f2498dadb98f03e2e22ae3440e1a39e5f HIVE-1387: Add regex for VpcLimitExceeded
6ae9c9337af420fcc19817f8f41ad33591b1f19b Merge pull request #1291 from twiest/dnsnotrdy
a2f8b152fe317b33931c3236a128d8c6ef8d22be Separate out DNSNotReady condition reasons
8f0095d2a37711146afd7d01dd32d4194f9730f2 aws-private-link.md: add the overall arch diagram
21c0bb715acff8820b473b78a63775929d467b8c update the design for better DNS handling and managed VPC allocation
9b300f30d9e4e87309a2be38c4ce52b46b5ceb63 updates from review by devan
3f1ae77c3a0ce3289a606c8ade5344a885b27cb9 enhancements: creating private AWS clustes using PrivateLink
a6d2bae3a129b39cdfbf9acc6e81f3808c8545ec Re-enable most of clusterdeployment controller for agent based clusters.
295f0606d40eef09db39ecbf0213b4fb03ea313b Set platform annotation properly for agent bare metal clusters.
e64dc507b71440beb9829de735835cef590e579e Merge pull request #1288 from twiest/docs
8f1a5a974c5d9221b4d9a994e980aa8e2cc58824 document scaling clustersync controller
652eefc764f9d71862200200584bf91334380a77 Merge pull request #1285 from dgoodwin/agent-validation
fe1f079973b71e05aadcf4d93f42e108f10176cb Merge pull request #1289 from gregsheremeta/clustersync-3-replicas
2c0f7273d70a9c47aba7595224f0579cba366984 Validate agent install strategy and platform.
da6006a51586db53ef4493ea1812b00e0cbd39e9 add controllersConfig section to template hiveconfig
199323e24b868e680f66db73daa4b146d27b4c9f Merge pull request #1283 from abhinavdahiya/remotemachineset_openstack
9e031ac4575aba242ac35cd2333b54077c6d0451 remotemachineset/openstackactuator.go: re enable using clientOpts
fce8b0f8b48483028bcf1d6346682ae7bf0525b1 resource/apply.go: fix for 0.20.0 k8s client-go
032dee72fc0cae68d567e98cffa31719d0c7de24 vendor: bump installer to master
50cba933cb4b558dc7b6f3714b05af04611fc0d8 Merge pull request #1281 from suhanime/go_slug_1356
56b56caf5e5d00396849900469fe376cc5c1e89c Merge pull request #1282 from dgoodwin/gcp-encrypt-keys
6a885360a3f73ba18bfb9ec7b1594310843dca3b Merge pull request #1278 from abhinavdahiya/cd_release_image_version
fc83de37fc2472c28bb704c0e3872b0cb55f29d0 Merge pull request #1277 from dgoodwin/machine-cidr-optional
c73166019eee7842c5490b65a10c8ab203106523 Merge pull request #1275 from abhinavdahiya/add_install_restarts_metric
9702f887d80b25c37ae3ceb14ff8c4ce2f45ffb0 Add MachinePool support for GCP disk encryption.
b7cdf9e1482b2e62491a427980950e7d1ad621f0 report release image version in clusterdeployment status
f0a2887b304337d9d0fdb309cbb91e6a1a87d92f Tag hashicorp/go-slug to v0.5.0
dd28eafe8b984fb8c221ca3addc7aa7def05ce5b controller/metrics/metrics.go: report metrics for only at least 1 hour elapsed time and 1 install restarts
bc6636f3099ca6e01a1ceaaf57b7d3783ac78009 provision_underway_collector.go: allow setting min duration for provision time, add metric for install restarts
a9b1b500dbf6c99806d895bba3829b91d1ec2d40 Merge pull request #1276 from abutcher/regex-configmap-template
b7f5273e17a3ee47b88b8858c8744e25914d62bc Make agent install strat MachineNetwork optional.
975f684452c3a17b2c445ffd3dc57123ed2f64dc Add blank configmap regex template.
51f4cd584475e5fe735da84d0302ae47de0605aa Merge pull request #1247 from dgoodwin/add-agent-platform
505f72b4b50a63d747e5fe324e7b2ad91aa8bd12 Merge pull request #1272 from abhinavdahiya/installer-bump-latest
88bd3619403b1803f1c032d56dc71cb9443834c0 Add enum for VIPDHCPAllocation.
b847fa9aa065edc358677d2e55063f48857ffeb8 Merge pull request #1273 from twiest/fakecluster
dc89529b778ecb56d6bfb9913844d13115822c6c pkg,test: update import for machinev1beta1
c2d05d1219d37e305f5624d93ffefa04e7ee3294 vendor: bump installer to latest
22c6e0265bacb6218a5685327f557110d379e9f0 Add fake-cluster- prefix to fake cluster uid
5e014bb3ab480d616cf99d90c48f6345c8e68e2e Make machine network required for agent installs.
bcfaf726de8d8e786df7d1a13ba5d5ad8184f8fd Drop imperative status for machine CIDRs and agents that map to them.
1ea79d59e8f30a45a874fd0ad38168c3854dd074 Merge pull request #1270 from twiest/fakecluster
f4b983cf3e9d03d4d9c7d31e0174769ddbff4e23 Change fake-cluster-id to a real uuid
bfc7fe7736c0f38bdef981013e6194a4868492b2 Merge pull request #1269 from abhinavdahiya/create_pool_add_namespace
2e6d264fd9ec2ec84c6e1a4494ebc91b669c09ef Merge pull request #1253 from abutcher/CO-1301
7f6c2e8e9c2beb54c4c8fc9139b7b799668c4de5 Make APIVIPDNSName optional.
7e3bae88dbb28a9b3b65b153e45cbd17df563958 Refine agent install strategy and platform.
1a90811a2a475f05771af12e638d68d9506f6b40 create clusterpool: make sure clusterpool has namespace set when using -n
a1e442db3c81cc1131567eecd022af0798144fe4 Merge pull request #1264 from twiest/logextractor
ffe404d8ba72c0cce1f76eb5ded8aa9fc089c950 Remove role changes.
f5c65e9dbce1456847285ac43762ae063ed670ef Move additional regexes to separate, optional configmap.
873b694d3f7370ba9db8540073b11c5e0357fff6 bindata
ab46aae6f8b03672c7bc60b322552c82878ace87 Update hive reader role with install-log-regexes write.
04f9068419c64fa77c65e9c30a2fb263ef117844 Update test for additional and ensure regexes take precedence.
4c8fe4c3545e9abb4334da48bb2b2330fce19d01 Read additionalRegexes from install log regex configmap.
043c50d6bf19c99a53535300e7e5f0b923ed519c Move InstallStrategy under Provisioning.
abdf14c3fc19a265472df803fc438c936fc5f8e8 InstallConfigSecretRef optional for agent installs
11de048520e68aad6eb0b96054f5d83a56760018 Short circuit clusterdeployment controller for agent based installs managed by external controllers.
7c85d1cfada073125ec64d622159cf7231445e23 Block use of Agent install strategy unless alpha feature gate is enabled.
fb42e53957fdbc48de8f1d1ca98185145946acce Define alpha Agent install strategy and bare metal platform.
74bcacb8b7fdf226ceac6912c23d738656825c8a Merge pull request #1262 from mbarnes/syncset-paused-metric
2dce6a3c588a24db71a147cffc68a02b170444bf Default hive ns to "hive" in logextractor.sh
44ecd3f8dc08849950981f9401181edde7a4c4a0 metrics: Add MetricClusterDeploymentSyncsetPaused
b8b3af3b3f8a5d976e1c735fc4b3b4c8ec025882 Merge pull request #1263 from abhinavdahiya/controller_runtime_use_logrus
611cbb87683fa89e70392b4df025fa9d77ce11d5 ensure controller runtime uses logrus for logging
c1943a22f3d572de87d60cc29b61c20c8f9202b6 Merge pull request #1258 from jnpacker/installattemptslimit-for-webhook
0d34f41db198d591963a0f168b394f31289219bf Merge pull request #1259 from abhinavdahiya/hiveconfig-feature-gates
7ff43a4f137004163b99607399e64c4d094f41fa Merge pull request #1260 from twiest/clustersync
3b6da85f4747da725912d4500917644bff30b50f Delete clustersync sts when spec is changed
e9f095ca61482b51307ed3c850b3ecc7c01f222d Merge pull request #1257 from dgoodwin/claim-display-columns
cdc27793771b3f86b5cafb7316e09671effed41b Enable installAttemptsLimit for modification. (make mutable for webhook)
dcd84ce1b301c757ec677e860d6eea5d960783a3 hive operator: sync featuregate config map and hive admission to use it
270ce01192718049cefd8cdb2df2972f65890e57 hivev1 validating-webhooks: allow adding checks for fields in clusterdeployment based on feature gates
82573635979c019b94b630fbf33cff2dd2712a6e hivev1: add feature gate selection to hiveconfig
17352abc29565dd85f291281baf8bac96ad1bbb6 Merge pull request #1256 from joelddiaz/clusterpool-docs
2b96fb1f7a4888c9bbc92e19195b4ca9872c683b Add some display columns for ClusterClaim.
ec5e793b4087b1609442f55869b0c5e63c47c143 clarify ClusterPool docs when using installConfigTemplate
057b4bc746db2f0a05a139e3925fdf9cd53084e5 Merge pull request #1254 from gregsheremeta/add-logo
e54af5423ab801eb31c3471f721130f5c4ae3eab Merge pull request #1240 from abhinavdahiya/cp_lifetime
c29403e63141e6855a1ba2a06acd8c0b200eb375 clusterpool: allow setting lifetime for claims
2a6cc85bb482cdabd9b6170f116cf37163500220 add logo png
26653ed477f345d359b0f4846ca70ed2fad37a21 add Hive logo to CSV template
266c7b4ad1482c9e1cec39a0233710413f4ac450 Merge pull request #1234 from suhanime/public_machine_pool
55ec88a708ab094d3ce8538709fd1d3ab1cf5a7d Merge pull request #1251 from abhinavdahiya/ostk_rms_ca
d7f89614d8d07203294389757e11e09f781e98b3 remotemachineset: update the trust from CertificatesSecretRef for generating machinesets
ad7ec60dae72ffbe5b3658c3ec30d6bea484bdff remotemachineset: ensure reconcile logs error before returning
85cd755c7612ae23dc3e804babe636916e5bd89d vendor: bump to latest gophercloud with custom trust support
c2c25f16f7785a1f811d3214cbb151d2a50038b2 Merge pull request #1250 from abutcher/official-centos
e25c3b5e7c215f3c437867bb0815f721a6e9cd2d Merge pull request #1244 from dgoodwin/gcp-ssd-quota-regex
1534d35ea354c85ff25202637bd868e6c93aee85 Add install log regex for GCPQuotaSSDTotalGBExceeded.
cc0b2f3f34e352c0bc124c248b172a341fc6509b Move to official centos image in quay.io
93e5a9fee058fd4cd308594be890c05415cb41ed Merge pull request #1248 from abhinavdahiya/ostk_rms_ca
0f6f325a05c7ce6c8c57f6fc8f4b6db762fb2b36 remotemachineset: log when machinesets generator prevents proceeding
09b8d2a5b501141f04a6ad037339b74ef8dbcdcd remotemachineset/openstackactuator.go: handle error when createing yamlOpts
e6007b7745b12727c79acaa1db4bda68085cfe86 Merge pull request #1245 from suhanime/add_images_not_resolved
ce76ea58af644896428a4129ff9207699373246c Merge pull request #1241 from akhil-rane/update_install_regex_23_dec_2020
bf8324073f3df46fe49bb8f97df1050c70367a07 Merge pull request #1238 from joelddiaz/vsphere-creds-certs
eabc67e7c77270905b666653507b99757ddcff9d Add InstallImagesNotResolved condition
7eec0032a2e8cca029b7cbc9ff1ad30424bcc14a Merge pull request #1243 from abhinavdahiya/openstack-certs
df47e712dd1dfea6c6de2ce210a4f233df4bdfc7 install/generate.go: fix openstack deprovision command when certificates are in use
f38273105497aaf45a3db836fbfec3ed51e2f275 Merge pull request #1242 from dgoodwin/new-ci-registry
d76003a1ee213e67c216427b70a728a56558cf32 Move pullspecs to new openshift CI registry.
5c42511aae014279f6fd53878965893aac8f8576 Merge pull request #1237 from abhinavdahiya/cd_image_resolved_condition
d6f1f04ea9008e423f5da2bf4706df87821bca97 Merge pull request #1239 from akhil-rane/corrections_clusterpool_doc
ce73565e67ccf9b011cdf97630ff939515de6d92 Merge pull request #1222 from dgoodwin/better-scale-sim
88f1f0f97b211b4be2f24181c91c0cde2e910fec clusterdeployment: include InstallImagesNotResolved condition when job fails
e001706f08e905e58afb70f64eec6b26eac28f8b Update install log regex definitions to detect GCP precondition failed error
b86e088c68d4401fa556c916c5730bca21b549d2 use ClusterDeployment's CA data when validating vsphere credentials
a27ef2e81e3cb02777432aaf95cab0717fe87ad5 Allow public subnets in AWS MachinePool
453814a31965252459e2de5b1db2d55872e5094e Fix errors in clusterpool documentation
d06ba266a5c84374644c4244ed7b3a83d16a4d77 Merge pull request #1229 from abhinavdahiya/cluster_pool_limits
4073e2ba6b9be6a5f2212d0a262cd9609f737a83 fix the remove annotation to be true value based like others
ef9f7f28d0ea4370095429cdf94ce621e672da33 clusterpool: include deleting claimed clusters for max concurrent
1efbc4857535052762176eb908a99baf25b0c203 Extract common remoteclient scheme installation.
8a8889dc46f54759d1e73801fee91ae8098e9b63 Use IsFakeCluster util where it was missed.
604bb091bec71084839d7de9d504ae217278dabb Use fake clients for fake cluster communication in most controllers.
8bbed1a7b64af53bedc087d1768a59f45405bb5e Drop two unused remote client funcs.
2010dacaee2973accc69b5371e3309dfb1f8080b Composition instead of conditionals for fake cluster install pods.
64bf658a57375f4f423f6f39d57f148c9ff12973 Merge pull request #1231 from abutcher/CO-1198
ed8750b600e5df882ecd59d66645e8ea0001ab43 Update scaletest README for latest changes.
15a9f2b1e459de1411c57e9dbb1ec309945db99f Allow fully fake clusters with no real backing admin kubeconfig.
95d90e11af647b474bd42e38ea70e3ee1e66bc29 Merge pull request #1233 from akhil-rane/time_based_scaling_clusterpool
4381783eb1b7a8d444002083846a731a649993ca Add documentation for time-based scaling of clusterpool
2d14ac89d6088bc4512d5c28fa755cc99350aef3 Merge pull request #1232 from twiest/hive_metrics
e0fbe5a69a4de3d52c327e59223b74fb7cbef9e7 Merge pull request #1230 from akhil-rane/fix_clusterpool_installConfigSecretTemplateRef_field
071211df3c04ac41860022c7fe61ca667108327a Change hive-clustersync sts labels to match others
e7aa1ab73bbc81ebd477c50407b4705f872d2e4b [DOC] Replace SyncsetInstance with ClusterSync in troubleshooting
40f38802d88bc3ee8e5d681b4486ef871f009a6b Omit clusterpool's installConfigSecretTemplateRef field when empty
f9755735433630639905e006a0ea45114b81cc11 Merge pull request #1214 from hassenius/clusterpool-ictemplate
867382c17093c18bd733321ea493058d1760020e Merge pull request #885 from staebler/cluster_move_proposal
f5e393e19acdf8aa18c81847549b6e9dd4120b42 expose skipMachinePools
f67784f1e49e0cd6c33dfbcdcd38aeba49755c3b refactor installconfigtemplate unittests
6738c296ba8d8030842857127b2fecfd104fd76a remove comment
000e6d0677a159aa50b844d2af3379859cbbe358 clean up unused test code
783f88a201a030c9d67dc453acd2df682f959906 Merge branch 'master' into clusterpool-ictemplate
c6ac2da1d971e06642952ccfab9da4bbdc068fbb add info for installConfigSecretTemplateRef
05507b4e1e9d3109467bdd55bc4a11ab080ff25b add unit test for installconfigtemplate handling
2be2273303874e187d1be389810a23a56916ca23 Merge pull request #1225 from abhinavdahiya/openstack-certs
6fab7450ad852f3e94edb430c87e20f4594548b4 Merge pull request #1226 from suhanime/office_hours
ac482f0648a767c7717cbda69fe387410f5a459e add test for builder merge installconfigtemplate
13fed8b796163ad72f06474fb3e800b0d01c5fdf Add note for Office Hours
f23859b3deb144f915ba069a007c013003a16037 Fix installmanager test.
bee2d155082d608738c0043c1e3594dabea82ccc Invert fake cluster logic in install manager for readability.
a66f9bbdeb4e458920823c6908ade59a3b4b04a4 Create a fake resource helper implementation.
afb02bce5a7fa17cc163b6a43c9e1bcf0c386323 Fake out resource delete as well.
d99a3be740f540676d0d4bccbef4d8de2c8725b3 Remove global hiveconfig annotation for faking all applies.
e584f96c6ed7c9c54fe3678ec5723785d2abcf05 Add annotation on ClusterDeployment that will fake install/apply.
fee98afebb20c94a78081331e517f63207dbc8a2 Fix spacing problems in scale test readme.
ea53e6c7d6fca89d8f29cd0b318f714128f67a68 Add create-cluster support for -a annotations.
8f4c04c02768b5798b3d07be2b426f0f66e622af Merge pull request #1189 from twiest/install_log_s3
f73fd4d60b63123d9cfc5c6283b6be1d7e34cb36 Merge pull request #1224 from abutcher/CO-1205
9bb3e6e07d1af6c5f19ad574d34355422c058e0c OpenStackClusterDeprovision: fix optional certficate field marshalling
dc7431fb730ac5ae670bc4363f88ef0bfd21c2bc Merge pull request #1223 from abhinavdahiya/cluster_pool_limits
e376e771bf20598f40238bedce424d7b1234f1c0 clusterpool: allow setting max size and max concurrent actions
14103589f1a43cb972dc0f9618f3d85bf1b2a938 Merge pull request #1221 from twiest/install_log_s3_config
d8b4795eac16f6da4318178240ab10c015799048 rename InstallConfigSecretRef to InstallConfigSecretTemplateRef
d70f6dbcbb1467a4ac4e8d5e867d54b2b7404d3a Revert "rename InstallConfigSecretRef to InstallConfigSecretTemplateRef"
5a12a068e19bc514d92cd448153ff590b4797db4 initial test test
24f52bbc593623f2723a8fb52bc6ae9e2a42cd88 Document and update logextractor.sh to work with s3.
076e900d4dde14808a577fa9ecdf1ef76f6e748d specify secret key
3acee9292a6d4ab9c4014a6ab89e09ea63964988 additional installconfigsecrettemplateref description
3c6a2682e24a763084010711ef0efb83be1068d6 rename InstallConfigSecretRef to InstallConfigSecretTemplateRef
3477c608c01ef15d492d6ce4047428cf09f0a94f fix typo
da73849f3beecd4d0cbfb5f8fdac65382c8a117e initial support for installconfigtemplate in clusterpool
cb5142fd2211e73994b640a3f05a810ba53c7953 Store install logs in s3 compatible storage
1c8e84814653d8a81d95d74981684e4d878b4733 Add ClusterPool.Spec.HibernateAfter.
1ff5a0560ca1e6336d4e5dd55f2b2611929e77ac Merge pull request #1186 from joelddiaz/vsphere-creds-check
2f59e7cc1b7ac750f20d302b5a3237a019aaab95 Merge pull request #1219 from abhinavdahiya/cluster_pool_admin
c55c4ba3e6771133cc7aa933d256731e993909ca Merge pull request #1210 from twiest/syncset_statefulset
0e43ae0fbf500c365123763953c50aa5b1b7c1e3 Add FAILED_PROVISION_CONFIG param to hivconfig template.
fd0e4c53b7ce5b6d4aaf6208d2a51776ac6b1881 Implement horizontal scaling of clustersync
9b650c3874b0f27b693c0b5fc4d0a2d27d7fd503 Add condition to provision_underway_collector.go
c743702b5ec13a34f1077fc412479152bb9f4171 Return error when credentials fail validation.
f6b92abdb9e19f0c55ebd99cd6d2093ac24f1c3e Merge pull request #1217 from dgoodwin/fill-claim-on-resume
b61ee6b6475625a4dd3c8246691560113e9d76b8 doc/clusterpools.md: document how to define cluster pool adminswq
43ff061b860d561863fe82a22ee51463db7dbf54 config/rbac: add hive-cluster-pool-admin clusterrole
c3c0f276139b4b5d4d9f9dab6f93a3f9dfdf6c09 clusterpool: ensure clusterdeployments namespace has same rbac as cluster-pool-admin
58fe555836cb5c2ff618dbd1d18a8404ab6393b4 vsphere creds checking
042e16ae59af35355a7fae3d767f0eedefe8d854 Merge pull request #1191 from dgoodwin/prom-cfg-multipod
e7fdd5d3f9920620ed62e8d815f493d4ac89a179 Merge pull request #1215 from dgoodwin/minor-scaletest-readme
207d975db47703af9b1e549359b105461558d5ac Add a ClusterClaim ClusterRunning condition.
f6032bedd8a625d24c9f65debf33ba37dee6a5c3 Merge pull request #1220 from dgoodwin/fix-failedtostart
7a4ece8ca2d02cd619da7fdaa357ddfcb5bd8784 Merge pull request #1218 from akhil-rane/CO-1217
978d75ef7c8cff45f0d49df066b3dda5d5acb980 Add annotation to group first applied metrics for cp-cert and ingress syncsets
a473f243ebfd468b1c21a78496ee6d806c603098 Support opt-in Non-Selector SyncSet first applied metrics
26c5fd8d9441f1088e468b2654b5c25005ed49aa Merge pull request #1216 from dgoodwin/fix-regexes
2f0e9cbb3256f02ed6fcd849b91f40500f45ccb4 Add cluster platform and imageset to provisioning underway metric.
952f2aceed95518c2a2a94ecd7e08bcb468f712b Fix unparsable install log regex configmap.
91d813dc1d2db376ddd6fbd673c7f563017e9d8f Fix resuming clusters stuck in FailedToStart.
cb4179562da8a59f7f20f0c4a1c570cda91dec55 Merge pull request #1141 from joelddiaz/openstack-machinesets
2f43a0c8da3a7dddb72811c35d1a3cc675984962 Merge pull request #1213 from akhil-rane/CO-1265
838b04e58e073ea9f0f06b35950bc0678617d436 Merge pull request #1205 from abutcher/CO-1107
65c5a50ecf39a2a5baf3154ec0829a0666362412 Update scaletest readme with notes on HiveConfig and fake applies.
04fa624812422066347753908996c8389b384e78 Add support for editing Labels and Taints on MachinePools
a8a5cba443f43423f820dbc3f22829a43ed9f46d CO-1107: Return error when syncsets not applied < 10 mins or clustersync not found
4b98f786a75686db89953003e6e783443f70d8cb Merge pull request #1212 from dgoodwin/gcp-invalid-regexes
2a9477484ab3e4907d6ef2f57a3025a408a1ae64 CO-1107: Add test for syncsets successfully applied and one for no syncsets for clustersync.
ab81873e49cc7c06a6a6c0072aa348a7272e9e3a CO-1107: Wait to Hibernate ClusterPool Clusters until SyncSets Applied
36b60b246724f42c9371cd4d8c077e24a6bae244 Merge pull request #1211 from dgoodwin/dnsnotfound-unknown
3aa607e953190cb31a94164e7da334d6883e6257 Add two new GCP specific install failure search strings.
3026783289289ddb19fd84a9b7ffa48520f0915d Fix DNSNotReady+Unknown in provisioning delay alert.
b58f0638feac5ae3bba7ba25e660feca6a097587 Merge pull request #1209 from dgoodwin/clusterpool-doc-platforms
4cd5aa390b08ca7c4d269cd33729565174b2eac8 Add note on what platforms are supported for ClusterPool.
744e7f91780dbec2f771b51114d7ecf1ce151b9e Merge pull request #1192 from akhil-rane/configure_dns_skip_install
0d339227e0f8338f04122018961e0c33622eb016 Merge pull request #1203 from dgoodwin/fix-new-cluster-cp-cert-patching
0c7065ae14cf2b8443b8d02f25327502bb8e31aa Merge pull request #1208 from dgoodwin/dns-not-ready-metric
f758b3d318bdb33a39387ae0a01be043b689636d Merge pull request #1207 from suhanime/fix_e2e
ff9adaddecb4e347707dbe9469a58477c22d44b5 Report DNSNotReady in the cluster provisioning underway metric.
09360ab9817e94ed4a2927303f84c0002d336c00 Fix e2e to adapt to multi-steps
50d76a6d0bac433c33282c465f21a4e3bd00ddb1 Fix control plane cert patching for new clusters.
39bf33ce3b230179692f32eb1acce622ae67a0b3 send a non-nil list of Zones for OpenStack
e295799398fddbe27cfb5c4d165a0742ff269d29 provide our own OpenStack config loading functions
b8e8e2ba9b471445b9c76dc0798a456a4fa1d146 Merge pull request #1190 from dgoodwin/simulate-apply
280c914964ff90282ba1d03ad2e2f0354c19c2a2 Merge pull request #1198 from dgoodwin/clusterpool-docs
70412fe02149f5baeea74a468cb29ce33a71bda6 Merge pull request #1196 from abhinavdahiya/openstack-certs
7e79c452faa533fbc79927e91942c9563e5f4410 Add hiveutil doc examples for creating a ClusterPool and ClusterClaim.
afbf9834f056d73e6ce540527909854053c83735 Add TOC for using-hive.md.
e5c87b6e1bccdc32bc1d9175adad0de473998b87 Add some ClusterPool documentation.
2ec253a4124cc32bc28499cfbc628aab4329d0df Re-use OpenAPISchema on the resource helper.
cff2d10b97dc508cb4056ac7f25de75304904af3 Add CancelRequest to our roundtripper.
312e8da18bf8580750d427bc561d0c53b18bd4e3 Use time.Sleep for simulating apply scale tests.
6730918647782937c0ff4518e6cac9e2159cf414 Add example commands to demonstrate hibernating/running a cluster.
958e833c35f0c03528c91d8f9c1af97c573c452e Configure DNS before halting installation
aed14fedd9c1bc0ad298a11a57b841fa0318b9da apis/hive/v1: allow provinding a secret containing trust bundle for openstack APIs
bbef2a4af27f5585e21030f09acd5a74cc83461c Merge pull request #1193 from dgoodwin/cpcerts-patch
8fc1c2e8ba4720cf7ee018aa1f4daba0e864e237 Merge pull request #1195 from suhanime/vendor_installer
32a29360ded846705e7a30a5943990af1bf5810a Patch APIServer config for certs instead of assuming full control.
9c2c61ef37af38dc2258fe42d15425dcb009af75 Point to current installer master
bfca32fe89d89efe3782960b95d40f8a4c2406a3 Add dev prometheus config for scraping multiple pods.
530e4aeea7ff9430d39480b0af58a38ce5443b4b WIP: fake apply
56a4d0946e2d3a2e3c8af09b0dd56bc8092383a7 Merge pull request #1187 from dgoodwin/log-slow-req-millis
2637566fed2073f54d54c03b1dfb818e91d4e815 Merge pull request #1167 from abutcher/CO-1188
b2ce51d587fded44f601da4c64058886e4520e30 Merge pull request #1165 from akhil-rane/limit_install_attempts
2212207c7eb70d75b526d4354e91f19a50f694b7 CO-1188: Changing resourceApplyMode on SSS doesn't update ClusterSync.
f9c5952dd664b394bbef1d0d6ab8a8ac77552915 Merge pull request #1172 from joelddiaz/hibernation-supported
ff249e1cc4ea42634fc0778ec8bfd5a5cdf6b24f Include elapsedMillis when logging slow kube client requests.
c128c714d0e706ada17278bf18a8d9537dfe9a7c Merge pull request #1181 from suhanime/provision_metrics
185ffb9a89f8ddbad4ff9729767399db6ba8ea57 handle switch from unsupported to supported hibernation capability
7964faec0d67714fa80b4ad1e7d7856a99203ea1 Add install failure details to provision metrics
ac33b0edab1ac900eb21e7c741be596eceb18bba Merge pull request #1180 from joelddiaz/podman-kind
28d66defed42a447de7de0c1bb249b066675663f kind with podman docs and Makefile
74e1c58c7801d9b404532d6df7084d165a9f3a7f Drop InstallFailingCondition
44cfe65482a0b080533ab5d36afb7f6df3145af6 Merge pull request #1183 from dgoodwin/clustersync-insights
6c98ddbf0bcabdac7ff5fa7abe532fb2901bd8ea Add option to limit install attempts
6bc79bdf751b9f30b85ed07e7e158cd83cad56bc Use durations instead of millis for elapsed reconcile GT buckets.
851e3f2b7968efea11f7e412b9851039f31c4db4 Standardize loggers and use observer in all controllers.
6727da9d3c6927627a663aea83a0d009c0c6f111 Merge pull request #1174 from joelddiaz/revert-1154
ca9a173c94e7ac48a0734dc7a4237ec78e1b754d Log kube requests slower than 5 seconds.
f2328d49ec00d854787d0ba387449a01ff90875b Improved millis buckets
e58257c9e34d86db8259d7d7c339c3e9441ae3c2 Add elapsedMillisGT to categorize requests into searchable strings.
9f6631bd18dffcf268fa512ac9aae720af5b3f8f Log elapsedMillis instead of a duration string with varying units for kibana querying.
cfff7c1826afe78cce5fe3e7d7eea8a93ca07775 Centralize reconcile elapsed logging and metrics, add outcome label/field.
332baf201c1d33a9dbb2e3c40a9c9c2fcdf3fb51 Add a reconcileID to clustersync controller logger unique for each Reconcile.
6513969715ec6be29592f89a5a982d12250e53ba Stop using default buckets for kube client request histogram.
c747d555cded654bdfa52e8b4129b35c9fb40ed5 Revert "Merge pull request #1154 from joelddiaz/azure-resource-groups"
37b75a14788b85b742a0fdde8861338c479f3d03 Merge pull request #1175 from gregsheremeta/scaling-hive-doc-link
0f22503fbde11b3541f29efc5d73e0df5a996063 Merge pull request #1177 from gregsheremeta/remove-dockerhub-from-pipeline_2
2bf0567bc32629a7a06da301e1d64938223088c7 change osd build to not use dockerhub part 2
febdb89a829dfc1e20e6a959990d6b6bf15578bc Merge pull request #1171 from gregsheremeta/remove-dockerhub-from-pipeline_1
a88fcc8178155fc0ab8da21df5d142d5ed3d9829 Merge pull request #1161 from twiest/install_log_s3_impl
f2ff16039134dd8ad5e2cfdaee66b7325ce7a1c3 add link to scaling doc
38c3290896c0f13f9f447065d513c05c19d3d9a0 Merge pull request #1150 from twiest/install_log_s3
e460cdbc12d43c4b82141d785439ae081d94c3cf Merge pull request #1136 from gregsheremeta/scaling-hive-doc
86bfd2b03753955bc15d132153f4434dd522db2f Document OpenShift Install Logs in S3 Enhancement.
340cfa38c173e35bd7975253bd914a910222b7bd Add s3 install logs config to hiveconfig
1468d156fc7d90d1817a4f5e0daa0cc66a1d2f75 Merge pull request #1173 from joelddiaz/skip-leader-election
0d02a0d576c39855e4ad1e53509a3cf9407d1186 allow skipping leader election
6c669650011c3707fc3829f9717bd9fc2c7f5030 address code review comments. Add new section about thread starvation.
147547075924504e3875a115ce5df7f909d18124 change osd pipeline build to use quay
abecef56d4aab34d1f6e621c5a835a8a95da90d7 Merge pull request #1169 from rayashworth/master
aa8993b8118dbbce39fd284a1c0c744f06db0f27 Update using-hive.md
8811ed6fd984850d9b7ae7ab02a716924e7e3c29 aws cred update
f81fd52f49257826bbad2ee8b369dce2bb7bbd70 Merge pull request #1166 from staebler/new-is-old-again-machine-secret
45cabd4f984d8fdc3114ae68e7176e7c7fa36985 controller: revert back to using the old user data secret name
ee801b15645b1d0aa1ff08fe538b7b2c608dc3d2 Merge pull request #1163 from dgoodwin/latest-installer-vendor
e67018efd898830d4a4cf6256282c59737c8eb90 Merge pull request #1159 from akhil-rane/fix_leader_election
d9bf966b4409a4a3a09d473b0f9ceb79fc0aab90 Merge pull request #1162 from staebler/disable_inflight_metrics
0d3dc88f07b6d472ee4676416af9cd99683d126c Vendor latest installer for GCP SA cleanup fix.
bfda04d1bdeaec08e2a5f44018ea504eb08004fc Merge pull request #1145 from suhanime/clusterpool_cli
c7580bfaaef1bcd3be94aeef87f06efcf66eed04 vendor: replace k8s.io/apiserver with fork that fixes hiveadmission delay
3195d5a3f2cb0e1da1e5916199929ff4ca954146 Add hiveutil commands to create clusterpool and clusterclaim
34d28c1d6e001687fae2d0fc3ac722fe173f0c8c Merge pull request #1154 from joelddiaz/azure-resource-groups
54442c3959748609d63aeacdba010b86a97e7a5e Merge pull request #1160 from dgoodwin/impr-ss-tta-metric
c2311c50701622dc874047bb22929b09ba348cca Fix stalled leader election after Deployment updates
933fc5c64b6a7b768250325afba775116b325b9b Stop reporting SelectorSyncSet metrics after initial sync success.
4bd6d19e745bcdea3a59bdf85756a17f6c53ac89 Set clusterSync.Status.FirstSyncSetsSuccessTime and add metric (#1153)
84072d4457c71c4a67fa2ecb2f227047aa4262d6 Merge pull request #1157 from dgoodwin/cd-output-cleanup
6a54a39b4bfd991002a0b0e0d0d70543e495d668 Merge pull request #1155 from dgoodwin/pool-cluster-labels
9b63ef444725c138bf0edb9542f491947be26695 Merge pull request #1135 from staebler/drop_cluster_version_from_status
a7b5556c6f195f1fb43750b0fd835ba28f54fd54 Add support for ClusterPool.Spec.Labels to apply to new ClusterDeployments.
79a4a3244d10a627952ddf8ed5f7730ce7568e51 Refine ClusterDeployment printcolumns.
28dae1a2f0d64e5d5a42db4ebd17ce08ba55c6b6 update hibernation to handle user-specified azure resource groups
3cddb7f48550ba28cc5d104d2f34554f0720b109 allow specifying resource group name for Azure clusters
fcf4fe51f19638cf5a81581673d1aeadb74f4982 allow specifying Azure resource group name for deprovision
4c65c6a1b69b9921afcf53fba654150ecef89c72 Merge pull request #1158 from staebler/3_11_generation
0dab5e86903adfde64af3fcaa4dec71fbb147603 remove clusterVersionStatus field from clusterdeployment
91ab2259d18b2a0be53d86105c9f4cdd7f5a0ac6 types: add status sub-resource to syncsets
3d1253c4e4ce26502664d30b864f2a4b777e15be Merge pull request #1156 from staebler/revert_controller_gen
636342de082b247d5b4e7e00eece38bb0da87ec5 Merge pull request #1146 from akhil-rane/openstack_docs
973c70c086026b32a233401fcd38b93c2a59861e makefile: use earlier version of controller-gen
f08b3fc2426cfe8ae69cde537aca09c91cdb0a80 Revert "config: update crds"
bca59df7d788ac54f4d10250b30c9f9347c78d1f Add docs for OpenStack
f45b75759b859ef298ed7de3589f904e8f1d9ec4 Merge pull request #1151 from dgoodwin/mutate-hibernate-after
c2a5d6128e0c03d761a989d12a237b8ef048b894 Allow mutating ClusterDeployment.Spec.HibernateAfter.
d26cf17f3f1f7faf5c47bec45654d4176ec012bc Merge pull request #1149 from suhanime/tag_librarygo
af8cfcb3fbe28fd9b6d6605b53f14cf60608bbad Tag librarygo version
c432c82b439afaa876eb5b9115f78b487d6c839f Merge pull request #1139 from staebler/syncidentityprovider_unittest
569d6c730e37a5469ea230263a2bbd6eec98089a Merge pull request #1142 from dgoodwin/log-sss-first-success-times
05641a1fde255f70f16c1bd16e334acab77072f3 Merge pull request #1122 from dgoodwin/hibernate-after
b4b0c0a0d7f0c7a5567eb326cf76a30631a36af9 Merge pull request #1147 from abutcher/CO-1187
f541c19b753afee000b39e6f9578380da7377dd6 Merge pull request #1140 from staebler/reconcile_on_clustersync_add
32c57da2842265aecd8945b72f028718f13a02e5 Merge pull request #1144 from staebler/replace_goautoneg
5b76d571e52d2134f0f452fc377b1fe2257d7e32 config: update crds
94d79a8d1f253cc77a51f04f4507c19bc3c1a359 docs: go 1.15
24397d7bcd04566c032674d76f480080748e43c7 vendor: update library-go
7775364fc58047eb1ffc0ecb374aca7d29b88f14 Merge pull request #1143 from staebler/build_with_go_1.15
f924f80d76646232f70d7cf0c73531747d136d14 CO-1187: Latest hive doesn't honor syncset-pause annotation
6974d7ebc1d5a3c447687c4ff72309d4e2c3c0fd dockerfiles: use go 1.15
8b6a6850f0995e93d76453db91a050c51f38c418 Log first success times when we report the metrics.
e3dabb7d37c466b9c45a6b6de8a18bda10dcb8ea Merge pull request #1138 from staebler/spot_instance_condition
9433e24306192c06e0712bbc26e66864907271e1 machinepool condition for unsupported spot instances
b40252ea8020c5ec13ab2235e63c78be45444fdc Merge pull request #1091 from akhil-rane/improve_leader_election
28bf14b3887cdb1c10090452f190846482c3d807 requeue cd after creating clustersync
c19e20d74cac08ac129f0e9a37ee2ae52c23bee4 sort patches for identityproviders
e161615d5d2a874709135c70366868e8b4909ccf Merge pull request #1137 from staebler/deprovision_cred_check_symlinks
30757d56cbde59e083e693de1cb3759530b5c989 Merge pull request #1109 from twiest/check_aws_creds_uninstall
ca369a66c1ec1b3eb6fd55bfb50d269f306fd978 Improve Hive's leader election
a6c12742d9259ad68f468da00cc3fb57b8bcacd0 Implement HibernateAfter to auto-powerdown.
30a75fa5ef6d86b292ba62a2b601a9af7ef54223 Update development guidelines to run hive controllers from source
b8b706456238383247ef84250aed842192556a10 Add condition when deprovision fails cloud auth
76f39cf2d4a59f81e1bce026f80b2120f3d6e1a8 Merge pull request #1134 from staebler/claim_delete_after
cbde96fe8bd4ffbd97b605c64827fe1f8bbede60 deprovision: skip symlinks in creds file watch
77ca427f6415da9d73837b69cd6b44383489b260 Merge pull request #1089 from csrwng/azure_hibernation
e29ad85c1ee70af137b21bad1d212603a9ec4c09 add lifetime field to clusterclaim
d2848cb1c7de75d780eeb6b4699be9892035de74 Merge pull request #1083 from akhil-rane/configure_controllers_through_hiveconfig
ec54a1d26c083387f22823dbfd641d491f5806ed docs: add scaling documentation
6025264255a42eb574b3ad6068f69a694975b37d Merge pull request #1132 from staebler/deprovision_cred_check
65d3aeb37e91992666bb642aea6dd058c9d71f93 Merge pull request #1127 from joelddiaz/vsphere-docs
58a5e4bfc753385647c4d3dacf4311cb72553b29 Merge pull request #1133 from bvwells/azure-dns-cleanup
d9a1167e4c8379cb31c42ebc0311ea80ac8f19ac add docs for vSphere
fab5b72dbe76e46dcf3220d5a4cf4304e0b5fbe9 Merge pull request #1126 from joelddiaz/ovirt-docs
acf5786dfdf65fccba6a0d40bf74a5c5213ecb97 document installing a cluster with hive onto oVirt
f950949e1363a70d5bd684fbc4bb7cba7ebc883f deprovision: kill deprovision when creds change
9fb2b35fa083fd9675dec0591a00d7893b2790eb Check error creating azure client in DNS cleanup
0e29757417e8dae3d05ceb0546b2487012a58103 Merge pull request #1131 from staebler/azure_install_cleanup
3dc8bbaf6ba93aed0bc25f61cfd55805454f4460 Add hibernation Azure actuator
91d35e9ae400a8c81903ed7ccb355cf9030c8cba Vendor additional Azure SDK package
5d6282976dcea2d3fb7aaa3badbff660fa63b39e Enable configuring controllers through HiveConfig
78c0461e5f917e1946c8a185b479e6d80b1eab81 install: fix azure failed provision cleanup
4dca74d267dd6928fdb78b5136e07bd18249157d Merge pull request #1128 from joelddiaz/vsphere-remote
c167614cd80d01e3f8cb82fde327ada39c65a7f5 fetch vSphere image in vSphere actuator
5c241facc6fed27619da7d6b211d2cece77af8a3 Merge pull request #1099 from dgoodwin/restart-uninstall-cred-changes
15265619811ca8dee497e5bc47cd197b3257faca Merge pull request #1118 from staebler/more_ssi_cleanup_fixes
83d238267b074024ebd53be1c51aece12708151b Merge pull request #1115 from joelddiaz/azure-dns-cleanup
66b1f528fcb20b0b4f7ec8bac7c2f58dfd220538 Restart deprovision pods if AWS credentials secret changes.
ed5f9cc5b65cb0ea59d336f6ccad50421803c5a4 remove ModifyStatus from DNS actuator
2cf1ceae4a409a841df38cd3c025e6b95ad59a82 azure dns cleanup after install failure
d0454b294196ab4bc36e50809bf719c2a37d3fe9 Merge pull request #1125 from staebler/generated_client_changes
2e446e061e9fa35391bf510b8496cfe6d59922fc Merge pull request #1124 from staebler/azure_deprovision
5a0944c857c55f0bf7b329a2b7f070fc18ca65ba Merge pull request #1112 from joelddiaz/gcp-dns-cleanup
f6267e2db274040c3eca40901d8dcad4a55ce72c perform DNS cleanup after failed install for GCP
d41e5f18688b11dc3a5203489be6c10e2e518c0d client: update generated code
df024bd7957fc800e363d7f24561ab862b5839cc fix azure deprovision by implicitly setting resource group
0f9c2b414760cdf5268f1eea9e16681057916ec2 Merge pull request #1121 from staebler/images_for_machinesets
d0da9cb7df6f6b927db2a56ae13c26e5646b1d6c use image from master machine for new machinesets
1de2281d9931d22c8b7816b6c8c2f07f82432b7d code changes needed for new versions of dependencies
cbba83bcdec460352fc90abdfa7226adbdf72b1e vendor: update installer
c0aae622a8b5a5a4376bf3628f76c17c490a97e9 vendor: update machine providers
2d24bd3b569494995f1701d0b2f1bcf0cc051c02 Merge pull request #1116 from staebler/CO-1114
1c7f86d93b0f7caa137f739bd58b536715c376dd Merge pull request #1120 from gregsheremeta/lock_registry_container
ea202cda32caff960a7a1aabf7d5852ddafebc6c pipeline: lock registry container to 4.5
7c649a1b37abb231cabd8967ce9f26961533f308 Merge pull request #1020 from staebler/remove_v1alpah1
333ea957f7a1f86c0f9777603d062fbd4f8628db vendor: add github.com/blang/semver/v4
4b98f3ae342f4600cc1225f2a891cbf8e78e8abb CO-1114. Handle different worker-user-data secret name for 4.6.
cef31b481c1f1c10cef4b34f5e39a149143ca0b5 Merge pull request #1119 from staebler/fix_delay_on_first_syncset_apply
779162359d2e696edabcd2ae5be1e1d2227e7e66 accept gone SyncSetInstance during cleanup
4503e6bf5cd7bbab1a45998f0e6b331ea9edad93 controller: requeue cd when csync is created
f0b188b7750f8f37a29a20b0f49820b31386db33 Merge pull request #1110 from staebler/cleanup_syncsetinstances
d180d7f4c474df6eb4420cb01495fc66a4904eba Merge pull request #1084 from csrwng/gcp_hibernation
c80c65f3df5ab7ae08dfae584c5e8737425296eb Merge pull request #1117 from gregsheremeta/fix_velero_template_in_pipeline
d65a59c9a300f0320ebf7d52104a4e3a22793f73 fix velero template in pipeline template
47c4c06fa9d076580113e1644e957f3df0c509b6 Merge pull request #1113 from dustman9000/add-velero-config
7e7427ce5d25e090710bb9f18ac2904cc147b604 Change bool value to string
c9a5ffe8b9846e44182e2dfcc589f63787ccef9f Merge pull request #1114 from gregsheremeta/pipeline-yq-fix
16456d664f64aa1c7b95d4186fdd547938ab73aa deploy: change production SHA retrieval to use new location
ae981314b297a0e9698e612c987053722b3f78e7 Add Namespace
f18d1a2cc3523d7575b4d6c58b46c93e7e4831e1 remove code for v1alpha1 aggregated api server
275a46a4fa2b79a51942addf89056b96e68f3d7e remove residual v1alpha1 migration scripts
a6d8da0e33f2aa151f26cbd7fa0998d0c979fa8d Add velero backup to olm template
f6e38b9ffa118f457ad9b328f5c896adea039df9 remove the hiveAPIEnabled field from HiveConfig
40a1e3a4db889803255c5ea321e6a50f4c1d88a6 Merge pull request #1107 from joelddiaz/aws-dns-cleanup-second
91a97ffb3248ab21e317fcc6cc1647c84febeb54 Implement hibernation for GCP
162b8f4a5372afaa3ce271a4325f0e5f72ca9f07 Merge pull request #1111 from staebler/create_clustersync_separately
0c17526e1ffc6f562c3b83d6d6e57588f0b245e6 controller: create clustersync as separate reconcile
2a198fd0a88ae865a4c7b0eb0ee274eadf8b04b1 operator: fix cleanup of syncsetinstances
5efa43a584dcb5718485667941ad638b43be1bca Merge pull request #1093 from staebler/clustersync
f36408860556c0f5abb58b1cd9942551fac6206a more code review feedback
de7dd1d6a81e0c48360aa4e52bb29c64d1d9f8a0 pick one DNS cleanup codepath and use it everywhere
cb7e14782d5d85d7a9890ecd2e5f01067c07cc22 Give operator permission to delete CRDs
ccfbdf9be82d52d8d0f29f39e82ab0b87cbcdb96 code review feedback
5367ee2b7e7decd5383fcabd614e56803b99698d config: add clustersync to rbac
02dbef76928e25b90e23af9883a70db3763c2f5b operator: clean up legacy syncsetinstance
5fc61c69235cf729f68c3107dfea576dea3d92cf apis: remove syncsetinstance type
3d7fb4001ba75a084cc2e784bd88781327a4ae55 e2e: use clustersync for e2e tests
ace8500105217272f1b9f58b68fe60648c4337c5 controller: use clustersync for metrics
6a5d249699fcc06515883297378a4686c2c3d40b controller: add clustersync controller
aaad2270dc42b60f1b6e3e5593bb51af4fa86a19 vendor: update gomock
5cf68946ca7b91909b0ab5803632f79bb2e8324f resource: mocks for resource helper
3c039c3fb8a4c1b699bd30ad0204619082777372 controller: stop creating syncsetinstances
e497b73b91e0de673aa4b28753e73363ac9c1429 controller: remove syncsetinstance controller
4e7e3be35b1cb5678ce066940304cae051bf8e06 apis: add clustersync type
c53da67c2788655c9a1d057d1fa1dbe71a373a39 Merge pull request #1106 from csrwng/hibernation_node_delay
bf5a6906091671136d580c3ea08f9c223a2394c7 Merge pull request #1105 from dgoodwin/unreach-ssi-hotloop
fb7371b2d66aa2bc08fe0bfdbc53d8bbb03ca5cb Merge pull request #1103 from klaphi/additionalTrustBundle
7e584d731947848074ff744ded1dfb1e8de2f897 Hibernation: increase delay to check for node readiness
7c0a7c54cadcbba92ac107dab968fbdecb345651 update-gofmt
e26b481c596ebe60cfe07796ad29cafd73e0e17c Fix failure to detect unreachable in ssi controller.
1e2a869615b05c23416e16b67f8acd5bf46cfdd6 Don't repeatedly try to delete the install logs PVC.
58135f869e9578d707e92b04b753eceab5a104a1 additional-trust-bundle support added to kubeutil
86cd1c9a5f145ccc4d823d8fb58b651e66a6e99a Merge pull request #1101 from gregsheremeta/revert-dns-cleanup
130c59ff83d0d6d1748155e22f7157232605126e Revert "pick one DNS cleanup codepath and use it everywhere"
c3e748587bf93b2a1e196b3a9bb5e206990bc866 Merge pull request #1098 from joelddiaz/unify-cleanup
65fb4af148ca96acae23681bb6865b2724cca417 pick one DNS cleanup codepath and use it everywhere
a365cabcb8e2844eb3f0c8c8b9ec4282576dd338 Merge pull request #1097 from dgoodwin/fix-metrics-crash
f0f68db36d2bb655fccfa8deac42ae318f640fa0 Fix metrics crash on new InstallLaunchError condition.
6cf778143c3d684e44ee5746be0163479999a298 Merge pull request #1094 from alrs/fix-destroycluster-tests
2111ecc81af7a747fa3c38c43d31536bd86acc43 Merge pull request #1095 from gregsheremeta/revert-api-server-template
f69d65eea4d642ba50b199e4b02378b7f35607dd Revert "expose hiveAPIEnabled in hiveconfig template"
1ba4ee2709523324788f4ca7a3188f36b0325f17 Merge pull request #1088 from gregsheremeta/hive-disable-v1alpha1-expose-config
bd66d1bb20472c5b073819c35407efc1c9625d78 Merge pull request #1063 from akhil-rane/condition_on_install_pod_failure
8b7044b12ee5de1cc9c54c46a91b9b946aefa854 Detect install pod stuck in pending phase
79a5a27a5465eaec9d9e3a484661abf00470da8d test/e2e/destroycluster: fix dropped errors
ea8022fbc99eebd00f63f597c886a2b172b5deb3 Merge pull request #1085 from csrwng/build-config
bf483f1702947f87b4d50178237230444109420e Merge pull request #1086 from twiest/velero_ns_option
d28940547f92da3316d7cce7fa664a3e19cd9b17 Add velero namespace config variable
53c19cc2702ff7276517ec1047abec3937bb5cd8 expose hiveAPIEnabled in hiveconfig template
1966962fb7b250ad5d297fd3fdbb690e30f68349 Merge pull request #1087 from alrs/test-integration-resource-tests
7a9524c767ffdf9f9215a56151ad6a9959f4b809 test/integration/resource: fix dropped test errors
6c9f319b2b6246ac44bd93c0817c39357d9d2807 Merge pull request #1082 from csrwng/hibernation_conditions
bb374bbdd18c3a5b03d42b28a3c27a1ccc3a8701 Add buildconfig manifests and instructions
85aaa85e8a80d6220e4323c83607e19ee363f359 Merge pull request #1079 from staebler/clearing_clusterimagesetnotfound
29904928ea9cf1b2c3b6dda2f0477ab1e1e0d445 Merge pull request #1078 from staebler/base_domain_validation
9fd1e9b748d29d6e279083084ed3c0f24ccbf5c9 Hibernation: set condition when failing to stop/start
7d0187f3baa25dc7afff638f9bd3926c9d974cb5 Merge pull request #1046 from kahootali/add-spot-machinepool
f11cd011588e1bc9402e94de8f9b104a4d5d74fc Merge pull request #1080 from staebler/release_image_pull_if_not_present
888f9e60e253cda49d0f96a952795c9e4710e735 Add spotMarketOptions to MachinePool
740ff884a317289d70d39bb63f718a21cf8ee413 use image pull policy IfNotPresent for OpenShift images
86331222db022aacc7643252b5744729ed0d2c51 Merge pull request #1069 from staebler/clusterpool_hibernation
aa2835b255742e03437333713264a641504d4229 clear ClusterImageSetNotFound condition when imageset exists
71e3110a3cec03614e63dec19b1443e81c41e338 validation: base domain that is a managed domain
a100d6a0e86a8adc1ff6c6f87bbdb832ee69e091 hibernate clusters created for ClusterPool
aec3a23b78b9f6b6b77c8ac25cb3bfdb9dc9b57b Merge pull request #1068 from staebler/claim_rbac
1807586082bd64ab558e7acdb71f96eae8576ea7 Merge pull request #1070 from dgoodwin/scale-testing-improvements
69dbde556c5dae316116e57483a079fa883652b2 Add milliseconds to log timestamps.
e1e15613764485200249e90ea8d359f58f150f9f Use stringData for install config secret for easier manual edits.
699ef4270c106232068cd933f9c2847b29407462 Add documentation and expose port for pprof profiling.
ed188514821289f2a47c0a7f8b92c540b86f474f Fix missing service protocol ports.
090e37ea4db4571ac8bcaeff6cb70056768902c4 Fix port reference in podman kind script.
81bb1526d42affaa202e18a1428ad3e1c437c5b8 Updated scale testing instructions and results.
45b32aa2572ac0012ec76ab98e2be49920218803 Add new builder options for adding cluster labels and skipping machine pools.
57a074c2e99f187bffb4bb07f50f5e3963381951 Merge pull request #1072 from twiest/prov_pod_req
75f78440bef02fb560246db51354bd05e894cdd4 Merge pull request #1077 from staebler/hiveutil_region_error
24e6f8de6d727bf420dea36f51ac29334a7b966f Merge pull request #1075 from gregsheremeta/enable-hive-delete-protection-olm-template
1d6fa4f4851458e175c0126ea40cea3dd6de15a9 Merge pull request #1062 from akhil-rane/fix_dns_missing_permissions_status
67efe4ad3cbd5f74b32affdedee3feb50a26ad9c create RBAC for accessing claimed cluster
96c45dd1bf9f7b969ad18ea4c95eea096f2944d8 add deleteProtection parameter to hiveconfig in olm template
790a5c4b73811a2eccf28943cb19cdf0f3c9a880 Merge pull request #1065 from staebler/clusterclaim
70043ef609fdad09d56f2a9e51173ef55852d200 hiveutil: print validation error for create-cluster
e566f5152b5eec0bfb7905fe2f6b473c9536ad77 code review feedback
c82303a638c3215fe59fbf455f7d86dad597f9ca Merge pull request #1074 from gregsheremeta/fix-operatorhub-script
883b2cd6f456895a945134797a93265aa7e4e44b consider pending clusters when determining how many clusters to create for clusterpool
8c7c4dd009498968e6d07636f2b72b25f0ea7214 assign clusters to clusterclaims
d162f1904ad4e7c34255c68ac3496c831ed3079f add clusterclaim type
4272c49ea9a36265872ea9bbcb51c14469d24149 Add memory request to provisioning pod.
34e4c1401e2e410b428105c723a99c6395165240 Merge pull request #1064 from staebler/gcp_machinenames_4_4_7
5a07e605021717431e689da153bdf52ffb999baf fix bug in hack/generate-operator-bundle-operatorhub.py
eb4528a368017ce4382622c8d904e2d884ba1b8a Fix insufficient credentials condition on ClusterDeployment
bb68a3046b812a718aaf9cd5fe4380f80fb2bcd9 Merge pull request #1047 from csrwng/hibernation
a213b4dcb3deea7852ba3742c3d137ce4a1d1eb5 Enable cluster hibernation
c6391dd134d5fdb4543e2030ce148556f965d329 Merge pull request #1043 from twiest/ovirt_machinepool
672ab67c782bafaebcdff5a92bbc94dcac6a8ae8 Add OVirt remotemachineset actuator
5521a4dc127772a411521b9158582723ae78bd59 Vendor ovirt installer machinesets
7f8583fd9966d9634b90cdb9f26cc396e2cea3f5 Vendor fake kube client
b050ef309196fae0561bd15a10660dcfc36c6d35 Merge pull request #1060 from staebler/clusterpool
eabdfeb3c896fcb16077189369644ed800f56e35 Merge pull request #1056 from staebler/fix_cluster_version_labels_update
ebf0be497a148235e4bdca291f95e9077edde6b8 Merge pull request #1055 from twiest/dnszone_conditions
4fe2df99f7a5d1fecf65564a46d0a3a026a77e12 Merge pull request #1066 from staebler/force_delete_zone
e21359ca0ceb05f4c1cdfcc20b8d5f3a60d07a51 delete recordsets in cloud zones when deleting DNSZone
922d043be2a1c9aedb6685ec68805df7ffa8e471 use full GCP machineset names in OpenShift 4.4.7
4bad9c26328f1f73f2c2396c342fbdf52e66c8a3 Merge pull request #1049 from dgoodwin/ssi-metrics-2
56bf3d28bc746feed5bbff10b1af8b2548bfaa36 Merge pull request #1061 from staebler/apply_no_file
f532fa6f3f6f02df2e55c8ad1188ce3a9c42b75e Merge pull request #1053 from 2uasimojo/syncset-reconcile-timer
53999c3731f1b17992e8332df889989a1503e360 Add AuthenticationFailure condition to dnszone controller - [x] Add AuthenticationFailure condition to dnszone controller - [x] Add unit tests - [x] Manually test
2ea1e2e0b1111fc2bbdaedaad896e57840623a05 do not use temp file for resource apply
91df0c9f7d2b41ea4f7de654211c781cd7e61974 add expectations to clusterpool controller
3ec637bc2c402f714cecf42bfca092f1ee825332 reap namespaces created for ClusterPool after clusters deleted
df5e55b3f48704ed7bac23d973591b2152ba00f2 additional printer columns on clusterpool
b7064771d68356caf28490712c181b272a81c580 respect the region specified in the clusterpool
57f2fe73b7cd41e6b80d09dec871805dda82816f add clusterpool condition for missing dependencies
9caf293f1ddc02c941d1d64d8ab0571930cfac25 add imageSetRef to clusterpool
351e7ed7149e1574f53f5178f291c07e6e8e1e09 add scale subresource to clusterpool
53642f92117c27c622ba61308d8d5319b012fcd3 code review and other changes
a72342da2f6f732ebd0053e01beffec0f1fc6deb Add ClusterPool API and controller.
3261cec3ba098e1ca4019db3d1b91a2db86f95c9 Merge pull request #1059 from staebler/double_machine_pools
91d328e5032fa5f98752b2890caa3b74d1328fbf stop adding MachinePool twice
d2ef9a80f6808eb3f6e2548577d9382ecf49af67 Merge pull request #1038 from staebler/gcp_full_pool_names
c4f19f357d9044a7ed48512af0bd5b7a326a413a Merge pull request #1058 from gregsheremeta/fix-deploy-saas-sha-parsing
179e06e53e860a5184f2b0e24deae2860fdc28a3 adopt new saas file name
632a612d90cbf81560c9268e6dd8ab43497dc970 Merge pull request #1024 from abutcher/ovirt-provision
26b3bcdef4a818e3aea21693f63c0684bae39508 Merge pull request #1035 from csrwng/hibernating_clusters
58e281c45f0ff74f9d6a4de3e254680736824b94 fix update to set cluster version labels
53f92b2817337f26ee0f2868ec82a6530face55d controller: add logging to gcp maachine name lease decision
59d5a4be922b715fdfdb4a2a3a7014e430af5c3e add support for full gcp machine pool names
fa644bee9b32c48b76aedc37bbea5607dc899e90 syncset controller: Restore reconcile duration metric
6f007197ccacaf2a095c0857306475477d70e2d0 Rebased bindata.
60e4896851cb343697182d88a77631ac7960fafd Add oVirt machinepool platform && updates from comments.
3398738df633673ba42f539002e808abd03816a7 Fill out oVirt create example.
be37bf4bb98f777ff4d37ea30303a46def4387e2 Add oVirt cd.platform validation.
82390636c3aabfbc373a9aad4acc39fe303ea810 Address comments and naming.
70003400662c601d1cf10b9ed13b966814eb2a03 Add separate oVirt certificate secret.
5149ef14ed8e055bdec32dd1801b29ad9e7ed779 Fill out ovirt structs.
740442094ddb368ad774e6eb7c309f9bd882104a Re-add SkipMachinePoolGeneration.
63d3854850230a21bcf31bf5e758ab7d41ea894a Vendor.
b68293beb7d383d699a6918eea47b8f95d655609 Initial oVirt provisioning support.
1089770699e1ba45b1bd40793fc6be4a844e13ff Merge pull request #1050 from staebler/update_go_mod
e9039a4eea4493f37bc13c3d02bebf09b197daa4 Merge pull request #1048 from gregsheremeta/adjust_approvers
0be6f1f86588adec4df12e7683ab4e2c9a04c3b7 add semver to go.mod
288be50f096753fda786efaf1d8ab1554518c959 Add new metrics to evaluate syncsetinstance performance.
8c811623b2e74b8bbaf75fd111827497c823f7c9 Design for hibeernating clusters with Hive
84bcab2ebeb2a3ce69f5b3d5444eb720bcd402d2 update OWNERS
b95e3901218743b27663916fef79a88c80991f98 Merge pull request #1045 from akhil-rane/skip_deleting_resources_when_unknown_is_set
5cdc58cc07846bdf385e9e5f90001d6e9c418bc6 Skip syncset resource deletion when UnknownObject condition is set
68fa75297dbfe1a3911bb3e880a9ae0a746d8c75 Merge pull request #1034 from dgoodwin/olm-crd-ownership
49c076130b935b1a04ba8aa97c5afc734694ba87 Stop applying CRDs in hive-operator.
f0f66ff5cdf345e88e26ad7a78d96aee7d8cd30e Add all CRDs to the owned list in OLM CSV.
37cb830b1b881ceeaa5f94df48e09b382d38f255 Merge pull request #1042 from dgoodwin/disable-leader-elec
025b40ce0692262ec710632150e87eaa9cb894ac Merge pull request #1041 from staebler/version_labels
edae560f5434e752c3a2dfa9bc39e34884ce1c58 Merge pull request #1040 from staebler/e2e_aws_expiration
2ef00a9aa1239ef51e7a1e04ff4e8176e8a9203e Merge pull request #1039 from staebler/wait_for_dnszone_gone
d27153fcffa163ddbe9cefdbe09a7fed1ee743a8 Merge pull request #1022 from akhil-rane/fix_error_creating_crd_and_cr_in_same_syncset
862323f90bea1e3499adb8ec1b88aa7898f5d399 Add env var for devs to disable leader election.
25b9f23097f7d1eafb4a53223c92608c107902c3 add version labels to clusterdeployments
194b39c50a4afbe608b567336625baab6b89de5c test: add expiration tags to e2e aws resources
cb1a99f672ac70c733cb6bbb28579ce2e526d7be wait for dnszone to finish delete before clearing cd finalizer
1379e1b8bd99779d67b28bf928795ab2f2d5f032 Fix unable to install CRD and CR in same syncset
d70488aabf907363960834809bf7bd970f853d4e Merge pull request #1036 from suhanime/sloBasedAlerts
2f806e59d5fcbc47046c4ce8f39efeeb5cbde4af Add syncset time to apply metrics
1470476a157c9b945421ba99b35a63b3fd0b64f3 Merge pull request #1032 from akhil-rane/dns_missing_permissions_status
f648e819b6e4cdec29be4e3068e2b453afb033d4 Set ClusterDeployment status when DNS Zone cannot be created due to missing permissions
8e189175d0e15feb22eb73d91b1327029115ef6c Merge pull request #1031 from gregsheremeta/add_uninstall_pod_label
d3c42f739de5ed66297cd69c5e7765fe1d8a88fe add uninstall job labels to the uninstall pod as well
747bf1e27b623ff6425dbe82215a7adbb096dc27 Merge pull request #1027 from dgoodwin/label-synced
07f5be11438946142add8541af35efa0618febdf Merge pull request #1030 from abutcher/aws-flake-regex
93aa24d02e352cee9c7b659f49c744122d30f994 Merge pull request #1029 from jewzaam/disabledControllers-template
b473daad53c76c34ae7583b4298cb3b631288211 Add install log regex for unable to find matching route table.
c620219ad9bca899b9356d99914f86579b0ab8ec Change hive.openshift.io/managed from annotation to label.
70d2ab7f6eedd5f049c29ee469a86e8db4dce399 Merge pull request #1028 from staebler/deepcopy_for_platforms
ab7c0c6fa45582b97cca5bb4a56c993a976b536f Add disabledControllers to hack template
6d7b1d76c3a59be51320b282aa001516931a02ec hack: generate deepcopy functions for platform-specific types
64c44612a3e71cc88dbb0167ade66a8ca98d483a Merge pull request #1011 from staebler/rework_cluster_relocate
bba3d0f7b85f5c9143ef749691066234a6f76485 Merge pull request #1026 from joelddiaz/disabled-controllers
33810615f55356e8b21b579ba1e20fb3baf3488a Merge pull request #1021 from suhanime/cdOwnedConfig
dc6f5db8578afb21dd6eaff4601b6aed000160ca move cluster to another hive instance
161da1b8fb38e48e4996115adca33f2dd2e26a89 Merge pull request #1025 from joelddiaz/dnszone-info
316df1f473520c942e1f236d3e11ad63d076a3cf Merge pull request #1019 from dgoodwin/annotate-synced-resources
6fe3780e4c82f03998fea400b70793f9d7c55e56 Add cluster deployment as owner for admin secrets
b8180462640e299015372ac8e383ad6e4aa68ec6 Reconcile non-controlled owner references
f3ef0a42c357299c7f97940b1c524644b86f4cd0 allow disabling controllers via HiveConfig
382c7127442c0c6f1121ef70bde8bf4b02072a3a use standardized log level printing
c9e07c43652e4690baa630057f732b596452e20f Merge pull request #1023 from staebler/gcp_disks
64503fe8a592c64b86a43ee4638e422c6e53b6e2 set OSDisk fields in GCP machinesets
6773308713ad9d367b3f7a284b2f1e4c03fea5a2 Add hive.openshift.io/managed annotation to resources synced to cluster.
5ef54a2bcdb7503d59c810e3a25bed2f2b0b8841 Merge pull request #1018 from joelddiaz/redisable-velero
1ed0385dbd3873d90869a9b85322c3d02f270ef0 Merge pull request #1012 from csrwng/apply_large_resources
37d3703a4a38b742a083806406121dcdac6588db Merge pull request #985 from twiest/vmware_machinepool
7e154514eb6227a57b3ce90633643fff3572fd4e Vendored latest installer
c82eb8a1d0a91249537c6745326ea0f554d84d2b Add vSphere remotemachineset actuator
ee6c138810d4252e57b671faeefde3e5326e9028 restore behavior that disables velero by default
dbd934dc8406c7b1183ec97db0a7955ad7816475 Merge pull request #1013 from twiest/update_vendor_docs
6f531c3741503d2c3604ae2bf9e1b073860a5f32 Merge pull request #1016 from gregsheremeta/use-app-interface-for-bundle-pruning
b16b42a55fa1bb85f32ae4832b3277db1f0b78e4 deploy: change production SHA retrieval to use new location
d5edd7a72bfd3ec28be249aa4a5ab173750f715b Add docs on how to vendor the installer.
84d8d4a9f68b1c642bf2441ee319650779ecc61c Merge pull request #975 from abutcher/vmware-provision
ff32b6b5d21d05712e109a437d942c963f6b6e86 Corrections and multiple certificate copy.
5bd73e95fd9749d71a696d4369186b4969637216 Fix enum consts, add kubebuilder annotation
8204901dde70dc1ffbfbbd6d3d981f157c0329da Merge pull request #1015 from akhil-rane/fix_connection_refused_not_setting_unreachable
9490fe5ad97cc0af7a0587001eb26d547496f3b7 Merge pull request #1014 from akhil-rane/fix_adding_machinepol_in_existing_vpc
02a9360024b2263ef797e35fd6e438d60999f2bd Merge pull request #994 from waseem-h/add-azure-dns
bdf46131f87e55bed0a5f8060ca96e8020fdae74 Fix connection refused error not setting unreachable condition
9b867c9a484a597caf0b542a257710b4ea3b05ef Update manifests and bindata
48d691c356f05c107e1293c9d53fa21306afe1d9 Add apply behavior field, implement createorupdate, createonly
ecd7fd21e0d9f6ecc072a1fe2a78c4a5dc6cc371 Update bindata
d3faa3202d0048591010b560a1dad09ea7fc72ed run make manifests
6b5839806adb7575b457c6055f4b37efb2a4d413 Add missing error check
ba9fdafec1f895b35aad67c2ec8d24af958def03 Add boolean to omit apply annotation in Syncset
47182a1264231dc3c4a8c844dad8174f000838c2 Make CreateOrUpdate a separate method on resource helper
5de9254827342a9b99cf424003a2ac4d7cf4d209 Fix panic while adding machinepool in existing vpc
a27a3ae210239c5c6475f09dac65ba22b4fd0106 Merge pull request #958 from akhil-rane/delete_install_pods
4c5b125f183bfa57291d7c5fe84584b33e2439b2 Refactor test helpers
85d6e7bc12ff44a26a9d00c04fce29311b0c1010 Add test cases for azure in dnszone controller
b8db91586bb7a270b7b7f48ae0db1d6b5742d9be Add azure actuator test cases
3623da25fe3d13c5933387bbe69fba3668ff7d54 Add live tests for azure dns
d9fc109ede351ae5240b1a111711447faa341a25 Add unit tests for azure dns
095defc085c37e42734a418ece19eba80246b5ec Fix generated client names
29d842605601cfd0409507f0b529ffa132d0d9e9 Enable managed azure dns for dns zones
e24e70bc3619a494545ccbafdc04465ecc96a964 Enable azure dns in dnsendpoint controller
70dfcd9a37d45def53951db8a5d3c379a496169f Populate dns zone for azure
a5b3c25f274ec7f214b19f56458ac8ab6ff39b12 Implement azure actuator for dns zones
799294f0cd9ea6be7cf97ac549d5b90732f6142e Implement dns nameserver query for azure
2b291958b0e9716051f5954e971f25e8f46c12a9 Handle applying resources too large to include in an annotation
e5ff7136220ea47899c6b9763824558719b06321 Refactor azure API client and add required methods
6bc387e00de1d05e1478cc9e07ac8bf9b92da41d Enable managed DNS for Azure
3bd7001e8cd306137719ea24dbe143cbe03d1623 Regenerate CRDS, bindata and deepcopy
80e32e855316dd4355fa20ee5a20ed1e641ee590 Add schema for Azure
8c46cfe8f9ed4b31d1781711a2d0b6ae869434ac Use utils method to fetch azure credentials
3c68c0e20a704660c99445cdb40c2a9898632e60 Generate Azure creqdentials secret
2375f0788fbf86940bf871aef5ca9cffc55d587c Merge pull request #1004 from dgoodwin/provision-result-metric
5d1878dd6e7a698db7bea7294ef7e74fe0a91460 Merge pull request #995 from akhil-rane/machine_pool_support_for_existing_vpc
b3cb9286922724e5b8e1600effcb82c17180ef81 Initial VSphere provisioning.
82e3c68de56d404b6fbb3e6ed15e58017ce5181a Vendor.
753a14a5a6f2c070aba3eb0a65aa63a063adb211 Merge pull request #1010 from staebler/protected_delete
dfcacd6985f25de559bdb384a0a6fab112216b04 Add MachinePool support for bring your own VPC
c1adcf9c010a0318965d1cdffcadf0a90a907765 Merge pull request #1009 from csrwng/e2e_delete_cluster
a1bab20da2fab54f9d4ae498c8b1653011cce971 Merge pull request #1008 from dgoodwin/syncset-secret-security
e5002af8dd5d73e1a1dbf289fcf5e6cd3a2869a0 Add test to destroy cluster deployment
6d4eae14dc2a0afbf1d78279a8418e4fd6c6564a Merge pull request #989 from joelddiaz/azure-doc
b65d534c462f1e432b71fb5f206097eac32ca0f1 Merge pull request #999 from joelddiaz/enable-controllers
76de7ec5b8a408f8447dc5d51faf6358fcdeaa17 allow enabling/disabling controllers via CLI params
37078702f42d322ab12c14b9c110dd66769d5f21 Delete successful install pods and old failed provisions
91467d9b5663820c85233e0f493b6081dbb1252f Add counter metric for completed cluster provisions.
5ddadf7e94faf158e44fa77c01b3e7b181c80edf Block SyncSets with secret ref in another namespace.
dfe71ff27e53120f6cf9bc81fa5e3b61d166a39a validation: accept all cd deletes on kube 1.11
eacdf239801952edfae01794ff1b8e01952f436a controller: do not deprovision when protected delete on
f3d32cedc76cb524287fecc9f1a181fcfba6b4d9 protect against accidental deletes of installed clusters
dc0c552868b78242880b8f29d9663e37513f198d Merge pull request #1007 from staebler/revert_cluster_relocate
e8633a07c2a7c5b8364811988a27fc2317701887 Revert "move cluster to another hive instance"
1d34ca929d9c015c9b6e682877f9e8af62ebac99 Revert "controller: add metrics for cluster relocations"
b140ae9ca5b5d7684e26fdf1dffdd6cef539fe97 Merge pull request #1006 from staebler/disabled_recolate_for_managed_dns
895573189472188fdf662132a251f5c626489643 disabled cluster relocation when using managed DNS
d605db04b3421a0a0dc97d768cf53d043f1b8c34 Merge pull request #1005 from dgoodwin/dnszone-cleanup-fix2
a36e8a2c12ed30317ef2ccb1f5abbce5b6a0d13b Another attempt at clearing stuck DNSZones.
4b3029e24203752d99e81ae4c1ef53f54f4c904e Merge pull request #1003 from dgoodwin/disable-dnszone-relocation
b9c0b4832f3c334018980ac0bd6dfbc7281d1d64 Disable DNSZone relocation temporarily.
ad6464f0962c9b2ab5b5a4363f61b576158b12e1 Merge pull request #1002 from dgoodwin/dnszone-logging
e26b302fff5112300be83972aa51dddcbf70722c Temporary logging bump to figure out why DNSZone deletion is stalled.
b2476828301a66eb21cdc5f1bac7d80eeea85ede Merge pull request #1001 from gregsheremeta/revert-998-take2
74febd65ff6b9f612ea8b8e7ff842c38ba4b05ab Revert "protect against accidental deletes of installed clusters"
48c16601768839b68e4ba1e1ca5ac993732769ad Revert "controller: do not deprovision when protected delete on"
7fc3ebf7012d92d7acf56094321f1548792df155 Merge pull request #1000 from gregsheremeta/revert-998
1f8995179909aad5ba41ed152a798c3850a7c1a7 Revert "validation: decode correct object on clusterdeployment delete"
6e1029b90bc1298919e78380fe58f96073b9ec35 Merge pull request #998 from staebler/protected_delete
c7bd4f82be829456846e875909eac9ceda0685b5 validation: decode correct object on clusterdeployment delete
d158f09f32b8a503151174917af20f48e8ad5a4b controller: do not deprovision when protected delete on
a7df339c82afee5e89194127a1a13100c6fad535 protect against accidental deletes of installed clusters
39d1b4f0d41b8d9807092db04f49b20e821e3a25 Merge pull request #978 from dgoodwin/kind-0.8.1
caf770f0bc74f08389b79ff74ff6f91a6edd9c4f Merge pull request #982 from dgoodwin/kind-podman
7c5494b32a4f9abff70ac16b02a25b1cf600793d Docs updates for kind 0.8.1.
bb98c77c21f3b6952c6a907e04596fcbf3f95549 Merge pull request #971 from staebler/cluster_move
587fb838184d504b454b8a749dda38e0a722b8eb Fix fork/exec error running under kind with podman.
d43e166bfd2631b29f4ce6f094452115ba205067 Experimental kind podman support for hive development.
35d221845bcc52f43347b69abaa8e727cf7714cf document azure creds format
2af28b568717ae65ad9f20f3c891615091ced1c3 controller: add metrics for cluster relocations
3192c38f5a4e3a4ba82385bf07a90c3d599c7c3c move cluster to another hive instance
de85f8d29ab7bea9b025e4ae33ff416d3f7318b3 test: expand test builders for building resource objects
f1fdda82f056c008a88f12a46e24af97e6a660bd client: add generated client for ClusterRelocate
c809fffcbb20de4d974fef6cbcae3a03a2fe81f9 types: add ClusterRelocate type
fd7d83ec127b047df6148a8722fa0d314b31dea7 Merge pull request #997 from dgoodwin/revert-delete-protection
b6f83d23ebf5384c03d9d5ba9ceea8d779041015 Revert "protect against accidental deletes of installed clusters"
d2effc78c82d4a9f2279a3ae0a0ec98b05239558 Revert "controller: do not deprovision when protected delete on"
c623f6f9467c008a0fb599d064fde277f2a77158 Merge pull request #996 from staebler/protected_delete
2efcb743135b614d0d94532f5eba966ea810fe28 Merge pull request #986 from joelddiaz/gcp-deprov
31268f1ebd31a18e5a9cf83a13fbb5e1527c7e32 controller: do not deprovision when protected delete on
88e47c1b4e8fe30d82471bf11c0609864be39d96 protect against accidental deletes of installed clusters
aaa932dc19dab9be51998a9f2f512910df8c516f Merge pull request #992 from staebler/nil_availableUpdates
bf45456579638425f20f78c6080b990b26f24fd2 Merge pull request #993 from staebler/restore_reader_caching
6c0c3fec2becc6ad105f92170ab37e533736b2e5 restore caching for local reads
bc13dd4a1e5d60deafb67c8776e8ed919d5c3dad controller: force .status.clusterVersionStatus.availableUpdates to empty array
affe87eade270825502cb5a2e5bda5ca521c8120 Merge pull request #991 from dgoodwin/fix-bindata
5eb1e50d0dc36ba0027e82fc1b07b14f2f8fedf9 Update bindata for previous merge.
677de55fca3ffb8d874c74824973e4bd2f79c745 Merge pull request #990 from staebler/remove_type_object_from_crds
5fecbe55718bde6441ee4dd5b7af4485595797ec crd: remove type field from validation
77b88cbf7469c6d0dbf46aede2b2d33828e2e5ed Merge pull request #988 from staebler/remove_yaml_break_in_crds
7bbd5ffc393edc8091eaf83abcaab216729b9b29 crd: strip leading yaml breaks
dcfafdeaa6ae96c816646ce77b8b2cd07fd1d32e Merge pull request #984 from staebler/older_crd_version
875569700a7b5a3e4f914da3c5831b7a3275b9e9 standardize on GCP creds flags/env vars
468303e42db88a5b4de6fc7baec86933e95b8a43 apis: explicitly set scope of types for CRDs
2560f52940f6e6185acb89e486cdde8681ac8a0d make CRDs compatible with OpenShift 3.11
9d80861b307f19813f74b81bbc6d8bb3fade7716 Fix operator hotloop on kube 1.18.
ab054cdd6d4010916b117ac95a16bdf015514cfc Update for developing on kind 0.8.1.
91c9e669e9b1b5e43b4c8d6d9639d0af51da812c Merge pull request #980 from jmelis/managedns
02bda080227914fb86854443a3ad837e636a0d35 Merge pull request #977 from staebler/docker-dev-build
57ac2a74054f4633ef151e43db7cd4302e649ec5 update bindata
c5818a8148f33f5cb9ae9c789505bf7b216bc15b replace references to managedDNS with manageDNS
61114f2cb7cf497f4dc037566a0966bc9fb7104b makefile: add docker-dev-build target
cfe72586f378e15a17b888b578a53e205f09bfa3 Merge pull request #974 from akhil-rane/customizable_additional_wait_for_cluster_provision
619dd97f178ad2828f304aca61b5679558f17d59 Merge pull request #973 from gregsheremeta/adapt-olm-registry-deploy
03d62f59df8e6a4059c557972eaba5a270c4e6d8 Add annotation based option to set additional waits to complete cluster provision
1f6405f630533c1595f104683d1e6bffb5ad1554 Merge pull request #972 from gregsheremeta/generate-operator-bundle-improvements
a41c437412a2ded9eb0d2efddafd3b201eafc389 adapt olm-registry-deploy.sh to new generate-operator-bundle-operatorhub script
4d1154d68590a34a910149636548156f7a7f64f4 generate-operator-bundle-operatorhub enhancements
564e001f639c0740a366e9729b8db1f7daefcc5c Merge pull request #968 from gregsheremeta/delete-bundle
48cdc7969a7594accac9177f7ad7b578d0491df2 Merge pull request #947 from dgoodwin/openstack-mps
64c91f343d6a7a1aa2135dbdbecc855e46830805 Add OpenStack MachinePool support.
ed64595d0ba88db5b2f725ce62c0483e91c69224 Vendor additional code for OpenStack MachineSet generation.
d9348de8ae632eb236aec1b24bcd078d903e7867 Merge pull request #964 from gregsheremeta/add-generate-operator-bundle-operatorhub
ac8f72898ad49d93c6b9dcddc341bc0c175470c1 Merge pull request #961 from dgoodwin/cert-rotation-fix
b8f5c4d8f49b61adc94ddf8be3ee2939f13bf7d2 Merge pull request #967 from gregsheremeta/typo-fix-in-version-log
a02b0cdeb640653b591e5fbcc4d8806be0e6b72f Merge pull request #966 from staebler/update_to_kube_1.18
2bd88698eedeb911617f28b6be07b938a5d5fc6f remove operator bundle and version.txt
b2e92ad09adc0eaceb6b38fba3cc42b410d39101 fix typo in version log (openshfit -> openshift)
7ce5e3f7ba81385ba568aca23d0313c165a6cde6 generate-operator-bundle-operatorhub.py: use git hash length 7
858d5ac84da1ca1e4b2267a6c935f2fdfc7766a2 client: update to kube 1.18.2
965547e128034686a32ab080ffae98f7447c623c config: update for kube 1.18.2
c721e570d7f6ddc3dde0cea2ad95b961a631ab96 vendor: upgrade to kube 1.18.2
63eb8888775d4ce3239d577c0e9745ed5891fce2 upgrade to kube 1.18.2
bf54f723b3473fef30317f801da0443a4ace4359 Merge pull request #962 from dgoodwin/ssi-metrics-clearing
ec70c836b43aa623a03bf67445cc28e3a273ad5b Detect serving cert changes in operator instead of hiveadmission.
01d12f07379dbafdf94c9d6f4e4d68d50e598f46 Fix syncset unapplied metrics not clearing.
78f7b3ff04b0d549340ca25385021b632dcf138d Merge pull request #963 from dgoodwin/yum-update
2a66a047093a63c68be32a522e1d0e237b6c72c7 add new operator bundle generate script for operatorhub deploys
00511062db2442e9e716044f4bc94c6b03d49ca4 Run a yum update during container builds.
62b92cc963e230999786ac6f88f7e695d8fe9b51 Merge pull request #937 from staebler/common_makefile
b2a2fa9e28cae7b26798d8e5612175c816ef71ee update version generation for ldflags used by common makefile
61aa917a2d6ea081de829cdbca4198a3e7455821 crd: make more fields optional
f87cdefe33d0f29d50de88d1bf855eacab71cf92 make: temporarily remove golangci-lint from verify target
4e6e077633201a787d951571d6b04dc0d3b187b8 docs: reflect changes in Makefile
602f2582dc666eefcc866b135e0d518f653b48a3 vendor: update dependencies
885b748d660c1bf50fe3c3536947665070aee3d4 use standard makefile
2bcc601e897555008f6f0e70df804da51462af3f Merge pull request #959 from gregsheremeta/operator-bundle-1.0.3
6129e11ea6b4d5f6b8a6fa16cbe3662465e5407a Merge pull request #948 from gregsheremeta/update-csv
3e7b71d87d1a252e3cb657f76d3b6711db876dc0 Merge pull request #956 from lwan-wanglin/master
3fef9a5959502ad232cebea9f84866a58d6de241 Merge pull request #952 from dgoodwin/hiveconfig-delete
27c387f9921e763c50d68e92505b1a23bdeeda94 operator bundle 1.0.3
641d25e6a9adce2552f4a5ce22a0ac0479430534 Add e2e test for syncsets
1ef5c33131355339bf2eb34a294f0cc3a236b9e2 Fix operator error deploying openshift specific types with GC.
60b90d82f62e559e555950313a435d7e6d7fa7fa Vendor OpenShift authorization API.
73d17d21af54f36ce3a82da35b79c74158582457 Implement Hive uninstallation via deleting HiveConfig 'hive'.
5f17ab3a5fc96db6c670f81c105724213fcae4a1 Merge pull request #954 from twiest/fix_label_ownership_apiversion_bug
9c11d2c66740d3bfb634cddad6790d36df64f762 Fix label ownership apiversion bug
e752e86f1767b027871688b6d27846d1a916a84d Merge pull request #949 from gregsheremeta/operator-bundle-1.0.2
e9168980fbd93cb3afe01d2509dc76253ac9fcb9 enhance the CSV template for operatorhub.io deployment
7162d129c6595417d5297612ce6502ffc1259cd2 operator bundle 1.0.2
a5c260d3ff8dc9485669fe564b4393098ff0b593 Merge pull request #907 from abutcher/syncset-errors
62fad9663335fab364b8d7d40c1020aaafd2ad3e Merge pull request #935 from staebler/upgrade_kube
043dde05ce4306e635dfb7e14f3a7197a1154254 Merge pull request #946 from staebler/fix_gcp_deprovision_help
861ca579667683af4c4ee659d3c9fe08bcda4fd1 vendor: remove go-healthcheck
730d52ac1bf87369cf8ea3db60d76712fb52f5fe use liveness probe feature from controller-manager
acfbccf382d7aa033534e9b4a1bc9c16aff6d3e8 give hiveadmission permission to list/watch configmaps
925f9d3f8dc0056fbdf070e76fc3260f472581db fix tests to work with newer kube and openshift api
bca66be4758c6e6e48476e566c4c4358ff5cc435 vendor: vendor dependencies
9114722e661b56ba12bed6e9f9b1edbce4795e41 update to kube 1.17.1
8d1e432490cbfb4b033dd5599a6c564bfac27f31 use k8s.io/kubectl instead of k8s.io/kubernetes/pkg/kubectl
32a0a83a99e613798e15c820074ee3414ac66c50 copy AddLabels from k8s.io/kubernetes
69c44f2ba8388967365b6e3697b38ac22ab36daf move apiserver code into sub-module
cea13e869c22b2e635dd59eccefe414c26109d2b remove the hiveutil v1migration command
ab3fa5ee4eb2f967509deba6e8d16902df9cd997 remove the hiveutil label-objects command
a50e44dbe66eb057af85544c5d3e95307905cda6 Merge pull request #942 from twiest/reconcile_references
b3ccf0e206018607cc2f5d93763098e12831b81f Merge pull request #944 from staebler/upgrade_installer
2f5ade585e139c0befc727545f67230942feca0b hiveutil: remove --gcp-project-id from deprovision help
350a99661c76c1e548d7e60723f7c12f6035ac2f Merge pull request #945 from akhil-rane/add_throttling_to_install_failure_reasons
2c6af290537082d1b5641820891a31954186789d Merge pull request #939 from staebler/go_vet_vendor
059871c7be57b8108df3392591f6f9f092a17d76 Merge pull request #943 from dgoodwin/e2e-namespace-fixes
7a5941b33e59ae85042c2fab82090edc64a331fd Fix now incorrect release image and gather more info in e2e.
f4ea476b90e6a57fdcf013cb43417a2bcd1af7e1 Merge pull request #938 from gregsheremeta/operator-bundle-1.0.1
2fad97cc983c199864ae84f3c291e4c21ac0567f Add throttling to install failure reasons
18c78464618723e9e47124b16ba43c08478913b3 vendor: upgrade to latest installer
4c679450e44e47ecb4d741e29f40e230ac36a6a9 Stop treating syncset applyErrs as controller errors.
a5571fafadea795cb75eb14da0607db9974ebef7 Merge pull request #941 from akhil-rane/update_kind_version_in_docs
364c64048111eda4c721e109d471ab1fc9115fc6 Fix bug in label ownership reconciliation
cfc4b522241ed16e706133950f071c2e1b4e2ba7 Update docs to specify supported version of kind
ecb060fff501542465d84a01f9bfdbb12c6a2cd5 Revert "Revert "Add ownership reconciliation based on labels""
7d0288e22eb3a76deb6e080adf1e18c55cb55b03 Merge pull request #940 from twiest/reconcile_references
3fbd9593d3727b02455ce1f8c83aa1ad2a3c1e9a Revert "Add ownership reconciliation based on labels"
7f123aa7b4f9c18d158c0033c3b95d536047dd55 Merge pull request #910 from twiest/reconcile_references
20f01bddfd7c34e8dd6b2e67de3769ea7c2101fc use vendor dir for go vet
5c2a49a033b9ecda259e4d8d9c0fd5682fb47cde Add ownership reconciliation based on labels
ceb9c380e1ba54a255eaf8f81ab1fc6dabbad7a0 operator bundle 1.0.1
d80f25ace2566e6724b3825726bd82820c6b2588 Merge pull request #936 from jewzaam/applied-printer-ssi
5eaaeb97f5d7119072feb2f705e816afc8a22c32 ran make generate to update bindata
4185b02ff23a57a6e1c677ca1052b0ea604ee486 Merge pull request #934 from dgoodwin/downward-hive-ns
8de86ccdcb0122b897780671213bc68258f94906 Create 'Applied' print column for SSI
bd4ddc1812968dd21fc1bc4c250fbd88a1f859df Merge pull request #929 from staebler/syncset_jitter
3918ff6d6f5875619cc759367142ccf9f74bf622 Use downward API for hive-controllers namespace instead of passing explicitly.
6e5b27e17d444764f1a823a35ce03c74e472b489 Merge pull request #920 from dgoodwin/configurable-ns
ace2059bb9fe195afef51964b9550e9f2bceb667 Merge pull request #902 from joelddiaz/openstack
ae320ad5ba1771604288f386d05a8c4f366088bc Merge pull request #933 from ahmedwaleedmalik/patch-1
a3594226c0372920ce4b83c5008ccbfd0772daa9 Merge pull request #927 from dgoodwin/ami-override
0710d43a6915689eaded992c016922284aabdf6d Support hive-operator and hive in arbitrary namespaces.
8c3770e2655aa14630bb1860d712363f5dc4267c add initial support for deploying onto OpenStack
07914ebb7896dc7ea4c53069ad6fd760ae4f6022 Merge pull request #912 from ahmedwaleedmalik/fix-olm-registry-deploy
4c2f16a92ac170a78ab57538cf801e2b3b3bf128 Fix ocp image tag
efa1e4570a593d888c0287473aebdd6344a7ee3e Merge pull request #930 from staebler/go1.13_requirement
de913a121691acc45c734b4dab27d1c4b2271a90 controller: add jitter to syncset re-apply
a2e8bf6f0009cac10fcc0d63c11dd249e3f63a52 docs: update install.md to reflect go1.13 requirement
acc3339aa33b5274b2cac8e77462de40457911d3 update vendor installer vendor
7536e51b20346f5990486a81af60e28aeda9138d Add an unofficial MachinePool AMI override annotation.
383c3c2ff471c793ae73cf495e1d785a6104a865 Merge pull request #922 from dhellmann/docker-use-make
859b372fa0e5693dc3b78815268186299f196b92 update dockerfile to use make to build binaries
2813734340d782cb36bd6db786814438b86ee449 Merge pull request #921 from staebler/use_vendor_for_generate
fad0e1f4b2ae5e77f695e48678a58cda9cb50c01 use vendored dependencies during generate
165e7ee4e9427f5e54c12f183f8947abe2c18b3f Merge pull request #917 from staebler/use_modules
9f60ddf35ad594262c231e97a76e3f36ea8bd9ad docs: update developing.md for go modules
35bffca5100e609a0b32e0fa27d78eef5769e4ba vendor: update for extra-build tools
04705ec5a152522655a143a38ec46e18896acf9b use vendor directory for code builds and tests
f5352eef07c12576d4a65ff5733a13d4c5d25980 do not use vendor directory for code generation
10af7e7e3c605dccb88e23cff6db68d4b7eca50e vendor: rebuild the vendor directory from go modules
8924c7c147839416ee04dd53c72034a8c97e96be vendor: include controller-tools as part of top-level vendor
ba22a0106eb72835387e41c29e0631cceab22326 vendor: switch to using go modules to manage dependencies
f0cf32526fe737f3cf0e5dd6c2e1075ca9ae74d0 Merge pull request #918 from staebler/go1_13
ed858dd35fd6fdedd2c57d9f7a6fabcaac46dc36 use go1.13
bbc18e4d847b247c02ee99ac8623d741d9cfa2db Merge pull request #909 from staebler/unreachable_backoff
7f50af08bcdf5c031940df37fd62559d90bade37 Merge pull request #915 from dgoodwin/vendor-no-hosted-zone-fix
387d26a84d1144dd4439aa58be599fd2e0b06c5c Merge pull request #914 from dhellmann/unit-test-cleanup
2c31cdd8f90686037ab6fbfc6a1f7ba6e320534e Merge pull request #906 from abutcher/secret-mapping-docs
1c4d8a519d4366e654044ab576573f8429a34bd5 controller: use requeue as backoff for unreachable controller
f0828a800fa9bcd59d56608aa4ecae41fce702de Merge pull request #913 from dhellmann/log-version
b26d7d17b7349304e606233f009ae3cae716ce74 Update machine pool generation to match installer change.
e004593748254b7e470cb508803e781b75cff1c4 Vendor latest installer for NoSuchHostedZone AWS deprovision fix.
fd703de7ec83b7d3c331310570ac87222b35a3e7 make log redaction tests more robust
ff1a68b198b3710d38bcdb2834ff889d00b6a8c2 add version information to log output
13563c4e549fdd0d07bfa9f89575851f7b14941f Fix CSV_FILE name substitution in hack/olm-registry-deploy.sh
05bdc62ac891cd18a71570ccf12c04e81db6a5e3 Update other missed secretReferences -> secretMappings.
e503130882dce2c6945762439283e9a62d0467f8 Merge pull request #905 from gregsheremeta/rename-bundle-package-filename
57f7516d1cd4cd76e340a6d570c5b7a52a219c43 Merge pull request #896 from staebler/discover_images
3ecf9646c95ff0647f7f03a499825a91d552d326 Update to secretMappings in syncset doc.
63c0bb9ac44941f12b632f175391a10eda49f959 Merge pull request #904 from cblecker/remoteingress-mode
183e828aa9dae6869108b96e55ff24fdff3f8826 rename bundle package filename per operatorhub team request
86cc061f3b1fe35c1dc9468b058c128202e45b1f Merge pull request #903 from lwan-wanglin/master
118db6916d94eec87cb343ecc1446ec942b1e7d8 Update some API comments
8918544dec72ede9a764b51f99dc1afce75af102 Update ResourceApplyMode for remoteingress
628f5e08149df53342606ed032a6f7bb450c5643 Modified the Deployment version in e2e test postinstall file
a1577fcd88d62654ea9c54811f5512bb9287ee7d Merge pull request #894 from abutcher/applymode-validation
cc8b8f79b1f1beae559b7931c1230b05fbe28c23 Merge pull request #900 from dgoodwin/apply-all-crds
d5292a5e78844a750bee4ac1eb9be1d436eb2b5c Dynamically apply all hive CRDs from the operator.
5bffbe6c787305754d0e9e3b7abd00bc7f4af8ef Merge pull request #901 from staebler/admission_json_unmarshal
3282812f1452b6c48ac3c7da80f6a87a0dd99302 admission: use kube decoder instead of go json unmarshal
b30a64113b55e008fd7f93941a57342307ba6fdc Merge pull request #899 from gregsheremeta/operator-bundle-1.0.0-1
78bd78e95b337a557702bfed71700ff399e4ecbe operator bundle 1.0.0
a0a0af5eac7b5fe3209950d6d7e994eaabf77832 Merge pull request #898 from dgoodwin/fix-baremetal-platform-case
ebdfe309fe0367c06087ef679e956cbaa20868c1 Fix case on bare metal platform to match openshift-install.
b8afd7a13712c24baebda4c858e0c9e8634526bd imageset: do not use oc adm to get installer and cli images
5c09d390ee2f9ada4718df37a1485d58afd54e57 Merge pull request #880 from dgoodwin/create-cluster-package
68910dfd34fd4da1b6a32ecb318e7346415771b0 vendor: add github.com/openshift/api/image
8b7c3ef12d89a1905b871dbf871d602491127c91 Merge pull request #895 from dgoodwin/clear-metrics-better
7e05a08575526c269db67d2e135f45774c2481e4 Refactor hiveutil create-cluster into a pkg library.
68b96d9e0456a99a851fa09ca73bf8b7d3b57f32 Improved clearing of provision/deprovision underway metrics.
a24a1f3b71d2ecf8ffbe163d87ab4232433b3a2e Validate syncset ResourceApplyMode has a supported value of "", "Sync" or "Upsert".
2154ceae736c99e3956e7084d1547a008439e023 Merge pull request #892 from dhellmann/override-cli-image
d159c329057062997a9c878d5edd3f817891d1b8 add config setting for cli image
584da850d20727863b3b7655ff5637bb9baa03d9 Merge pull request #893 from dgoodwin/vendor-installer
0c1ea8babb4e7132b4a15f30d3c10e45158eb8ef Merge pull request #891 from joelddiaz/crd-watch
006bd95a0b0f1a584660d273c834208c81312daa Vendor latest installer master for deprovision code.
84ace315d8e77fcd037764d50b4da6397b614430 Merge pull request #890 from gregsheremeta/hiveconfig-template-empty-array
6154813e50056a753c287e09d371c0c6c70801cc modify openshift detection logic
0e2c2af9d29b6512e6b3625e42fa21cdd5899fe0 OLM artifacts: use empty array for MANAGED_DOMAINS default
37b03fdc3d598705e18c02314dfb3a49d586daa9 Merge pull request #887 from gregsheremeta/update-hive-managed-dns
2be9968efcf9ea36d285d4a5b2b260f0fee68f3f OLM artifacts: switch managed dns config to an array
571a9efe4fbe8f0bf5546292025a503558dfa139 Merge pull request #888 from staebler/apiserver_machinenetwork
0bd484df2c4758106876dd47ad0c9610d8d67116 apiserver: omit empty serviceNetwork and machineNetwork from installconfig
725b685dbb69bf4fae805db7d28f7ca3236228e3 Merge pull request #883 from dgoodwin/gcp-ms-out-of-chars
65e76863372625348cf428cf0c8b97bceb2ab65b Merge pull request #882 from dhellmann/log-console-output-line-by-line
6c86bf09b26935222a627082b17b61d934cdadda add log regexps for common libvirt failures
a7c846fbd1d6b274945925dfb63c674fb014d8ce update cleanupLogOutput to handle malformed data from libvirt and ssh
961d5ca65ef923dd5ba81372b5449118ce76dbda docs: proposal for inter-cluster moves
23915ca5e5e5554851934c0451128be52086bedc Fix crash when using more than 35 GCP MachinePools.
9d6391083c5416ace2cc5c7032f3c2efa9dedc23 Merge pull request #866 from dofinn/add_cd_region_label
da18667fb289444d7767b07780a773de31cad66d Merge pull request #879 from staebler/migration_targeted_restore
037610c4dd3234d7b0bf33b30817f712f6c6871f apiserver: sort machinepools created during clusterdeployment create
dfd79973b39b8cbc5c87390b6801f33eecdd734e migration: delete installconfig after clusterdeployment
1ac9b3c7c27080b56ecda4e9f0bdd301b2f4b305 migration: fix mis-spellings of specify
0284a5ce77dd49981de01bfaf1526f4f5c2d1867 migration: make it easier to use a custom list of resources for saving owner refs
ffc146641e12fa6ee67851dcb3e0058e43ef1031 migraiton: add post-restore validation script
fc72a20358b1cdd6cd357b0829a97f0d829ea8f4 migration: process for fixing bad restores mid-migration
ab8379278d42ae36ae73dc3d001e30c339925500 Merge pull request #876 from staebler/migration_batch_deletes
55cffc79d7ed14fd2c2bbd9e9e1a808889777501 Resolved typo
63bc2e684fa2c9b261221cd8ec2204e8b14d71c5 Merge pull request #870 from abutcher/debug-logs-ssh-keygen
539fe70647d59beeb3970e4c9b4384c78b27a569 Merge pull request #877 from dgoodwin/deprovision-approvals
be5b1cba7a96b3bf77dbc0c9cdc8dc38affce71e Add HiveConfig.Spec.DeprovisionsDisabled.
b91b0c4fc6108bfe79ab24aad5a077736816cfcb migration: remove initial fetch from delete process
6cbebcb8d6465a7fabb065468ba6280a5d9c24e7 Merge pull request #782 from dgoodwin/gcp-ms-leases
21b52714388cb8f5cdca49731b0923bc89866224 Additional test assertion
d5d2d9f0268f3e4467bab3c2a76effe54d8bf2a8 Merge pull request #874 from staebler/machinepool_size_iops
2641319311be896a2e74e7f18d8c35955eaf64e9 validation: allow 0 for aws machinepool iops and size
96f6642138779343eebad8a75fda52b07cf41186 Merge pull request #871 from dgoodwin/baremetal-debug-annotations
d877dbecfc6471afa501b335c566a5a64a7efbb5 Add install failure debugging annotations.
efaf67860f5e0ba94256f05fa01fecc6935038ac Fix bug in GCP machine pool name leases.
20ac602bad25ff36ec31416ebec029889d43b8a3 Implement support for multiple MachinePools on GCP.
93722ed9cefada2fe80db518e729a64eb9b6c5b3 Merge pull request #843 from joelddiaz/apiserver-url
a2d69d732b46b9eeffb4754a552e517e37183a31 Merge pull request #872 from staebler/owner_ref_from_certificaterequests
b781a7824e3c85c8eca78e208dca359df3a7040a Merge pull request #873 from joelddiaz/fix-lint
f38e9141e8a90d6f57dacf45956ce049a86aa5a5 don't run the env var, just evaluate it
b29b3d3c5b14233d5ff02390d49ae60776b5e8c8 Merge pull request #867 from twiest/fix_v1_migration
9b4a429924ee17ad72549e0c60096d414ea334bb migration: add certificaterequests to owner refs to save
ba0980e463724037f015eaaf8aa8cbbcbe9a21eb Add note about ssh key format to docs.
478634095229bec9b4629c1bac1bd7304b394fa2 Merge pull request #869 from dgoodwin/block-bm-machinepools
c812ecee2225fcb60dade5e69bf28f091b249c69 Remove support for BareMetal MachinePools.
9500d226a8f0f063726b135114cd2a262fd27720 Amended changes as per comments
cbd54becf7d3ac2d63152f8940530d1baefe9618 Fix for v1 migration.
0d907d64e5c2e09d89262086c100f8fb6f22f415 Merge pull request #863 from staebler/migration_speed
3a5f13e04d8f0064b4650e2633210bc90e03b500 Merge pull request #861 from staebler/azure_machine_pools
fb2ac5110f542c2be5df2d6ccc7c79e890f28943 Set region label on Clustdeployment CR
ca65e9bf1725e21c03ff3905026d3b4aa1277c23 migration: limit the number of resources fetched in a single batch
e890b54329c55bb38cdf8d33528545eec14f138a migration: improve the speed of recreating objects
ef523170f85b610a6a3285e64467918a41fe828d migration: improve speed of delete
a77fad3c5a68f5d13eeb48229c841d09f58c4c6f migration: improve speed of restoring owner refs
642977d727ba38d5f7ac3dd24fab0ae314320bf9 migration: improve speed of saving owner refs
867d7fb189bfb577556912217c22fd8e8368ad59 Merge pull request #865 from abutcher/remove-installmanager-debugging
6c003e277a525ccc40ce53e16d1ed6aef7777b7b add support for machinepools on azure
9e4682d137d0534a20395255c4a41b516a701d25 Remove installmanager debugging.
80e19f4c0ff54656a6c8c38fe060c21e2d2c5a69 ensure hive puts a domain/hostname into the apiserver object
d64db99c39a6872cdd62777ec9c552820931c4e4 Merge pull request #848 from staebler/docs_install_job
54648a2dfa058815bb92c093037dad068e08c7f5 vendor: add packages to support MachinePools on Azure
33ccafa73c5670b3c3047b74eaafac0e69c8a489 Merge pull request #860 from ahadas/docs
67d95abd92d42cf8177a6c12da96081b40ebf349 Merge pull request #858 from dgoodwin/maintain-kubeconfig-certs
9de5c48920e573c871b25e191650ca93c5916d53 Merge pull request #854 from staebler/aws_cn
f65983070826d3ab4e9db210068bc3cf25784606 fix a broken link
fa12980e932cd8c639211f59edf389442a1465da Merge pull request #859 from dgoodwin/hiveapi-memory-bump
85a71b4816ba675c55adbdc3c0aa17c8a8934518 Bump hiveapi memory limits.
7b8568cccfdd7d507febffc0c70e482951105777 Add additional CAs to admin kubeconfig even when status URLs set.
99c0220cb317404b7c0368c1a5ac63882b53dd0f Merge pull request #851 from staebler/using_hive_v1_changes
9c42e13b74e39ac235b62e55d81f5bae2f705108 Merge pull request #857 from dgoodwin/deprov-3
1d7bdad28b5124a89c8f0c3a8673d259533878e3 Also add v1alpha1 clusterdeprovisionrequest to operator and other roles.
ba4158aa9322f94c3b7f83ebe9af199198c09eda Merge pull request #856 from dgoodwin/add-old-deprov-frontend-rbac
217b85c88e35b46e014dc1bcc71a52e5d8cdec80 Readd v1alpha1 ClusterDeprovisionRequest to rbac for hive-frontend.
866fb84351bb88d6ed22c884e9f0693c4de479c0 Merge pull request #855 from dgoodwin/olm-template-refs
571d4127acbef3e72bcf3588dbebc270897187bb Fix incorrect hiveconfig v1 field names in olm template.
8cad7e4ee4c5a209c5416feb47444585bb3dc242 support aws china for managed dns
df4f1fcfdbac681a552cac9d82ea2661c9bc4be0 Merge pull request #853 from staebler/machine_pool_validator
626e7f77cff97663d7c69a0f8a37dce5bb39abbb Merge pull request #852 from staebler/migration_dnsendpoint_owner_refs
a047a261b2162c1effe3f343b67c172c4b645be0 validation: reject changes to MachinePool platform fields
0492cb5267fbc7d818d7d6b3805e127b0f04e259 docs: update some more places for v1 changes
072d87fa91f1cbe8e20d8e4c47538ac52515ce13 migration: fix dnsendpoints not being skipped during owner ref restore
37d41b19324ef9969651ea8620ab458dcdb7d053 Merge pull request #849 from joelddiaz/additional-cas
c985417c1a26a7890b994270f1d6e88d6580c5c6 Merge pull request #846 from dgoodwin/globalpullsecretref
a4bb0186ddf21854184ae2479477cccf5ee5658f Merge pull request #781 from joelddiaz/relaunch-controllers-on-managed-domains
5ad60160424bcc5aa9351ac704896dee514c046f Merge pull request #844 from staebler/migration_updates
1af9c73840744aff864874fa84993af769ab85e5 set the correct field name when adding additional CAs
43c300396054b28addc7ebed01f2a57ced82f50c Update install pod labels in using-hive.md
ad0bc1950b7bbdab6cce2ddcbfbc728f8c1a6348 Fix globalPullSecretRef mistake from v1 refactor in docs.
3fd866b5a7ac05d2c6d70e2443d7d0a76682ecd6 migration: changes to support hive-int
d74b16cb9579980961208f4ea27acee419b7f493 Merge pull request #829 from staebler/olm_hiveapi_roles
529c14acab05b54e51a58ba9ea7c5c82bd573dd6 handle changing managed domains in hiveConfig
4b67a4f987f5a24833c816d3802daeff15763a9c update vendor of kubectl
076f0a64bdecced0f28affdbadfa39f5e9125da5 Merge pull request #837 from staebler/get-kubeconfig
2e16aa244f57f3a5326f6a3e98f11e74dda10f7a Merge pull request #809 from twiest/label_migration
fb5fae3e9a475855917c1a9a113702423bc795a5 Merge pull request #839 from dgoodwin/bm-docs
5205edb061f381dcb03ebcdadb8916b7e4490f7f Migrate hive objects to have expected v1 labels
0942ee7eb8b6bf7f6701bd4b0a94a54746d07038 Add documentation on bare metal provisioning with Hive.
dee9b936325432d2206f553b16a435612d6607b9 Merge pull request #823 from gregsheremeta/update-docs-v1-2
f95446d21ae47da6689f8de91c9b1463955223b7 Merge pull request #840 from staebler/etc_passwd
ccb04b3087a7af3539abcb18236c55e402b42e49 installmanager: remove manual adding to /etc/passwd
dc9fa1a66ccaf8f3bc9b8850a8b3f82b6de68941 Merge pull request #838 from dgoodwin/fix-missing-imageset-condition
a2e298425f691b201a7173f56be1a08392b7e9ba Fix missing ClusterImageSet condition.
fc03af290e1b9c5b72c5c88c0c9c2404b6181ba6 hack: script for extracting the kubeconfig for a clusterdeployment
0729352a493d5fc3289d0490eacb8420c5722fe5 docs: update using-hive.md for v1, add hiveutil doc
e789e98e9671ba4cb2ee8e24bc658d4578f72001 Merge pull request #830 from staebler/restart_pods_on_cert_rotation
72d9e43734348b5684168bdf5e33438888d8f501 restart pods with injected certs when the certs rotate
7ebe666a764b7b0d4f40fdba992b276c720523fc vendor: add github.com/openshift/library-go/pkg/controller/fileobserver
ed7dfcb60d719846815e1f7be88a8060cc76949c Merge pull request #826 from dgoodwin/drop-remoteingress-toleration
6474b80ec27b558177c42515316e7cbdf690baf1 apiserver: fix rbac for olm deploy
10ef28784ce236aec1d7de6d0f572fc270d96596 Merge pull request #798 from abutcher/vendor-installer-peering
e4b92d0ae0cd3f033b07b3ed3c713de07f98895c Remove now obsolete toleration edit in remoteingress controller.
8f9aa4d7e2fa05273adbf96dce375ceb9bc84689 Merge pull request #825 from staebler/apiserver_service
503395dbe3ed7d611c34b9431a6e126f1325a64b Merge pull request #824 from dgoodwin/v1-merge
d213a362fd5b9ec9556587873f0ae09e04b833bf apiserver: fix rbac and port used
908a8f4ac17aff1e67e46d6008e7a116c2b94eaf Merge pull request #820 from dgoodwin/from-centos
cca7a311ee8f298a6077e2f1876bb9c7aa9217f0 Merge remote-tracking branch 'up/v1' into v1-merge
4d078ea584cc465c8d519956ba32f2b583376527 Merge pull request #799 from staebler/syncsetinstance_restconfig
a8e7a33c6906a49390c6a3a421ba7c8d86e2f9f9 Merge pull request #819 from dgoodwin/bm-libvirt-ssh-key
88a94a1359e24699f12dd0548d763c625fe5b2f0 Merge pull request #822 from staebler/oc_3_11
81bd9995c3ee04fa3b37d7e2f960395d3a249b14 Add vendor/github.com/vmware/govmomi/vim25/debug
f7c5efb98260934b9b361be7566b1ccccc20df09 Updates from installer changes re: MachineCIDR and AWS Machinesets.
b952da534e9e723db67aafe330ce8060e9f2bbb2 Update installer.
ed063bb7d388a8bc20937a070cee94e0d57a56ba Separate cluster ssh key from libvirt connection ssh key.
c5c453821654a02feba9505c6f9b2c2440a1a9c5 migration: support oc 3.11
0b63cf8e420eb0dba1a34095db326e3618f184ed Switch to FROM centos:7 and restore libvirt dependencies.
17687ff6cfd8d01625a98021b02531145cf63212 Merge pull request #818 from dgoodwin/bindata-fix
b01fdb6c6016e01cc46f4363cde9664972b088df Fix bad RoleBinding definition.
967182617403023e0621bb919521ff2e0a9af8b3 Fix missing bindata in rushed merges yesterday.
2e69f0473a45cd8c840ebdd0f654c4be06d89fe0 Merge pull request #816 from dgoodwin/master-hiveapi-rbac
dd34ae8150022d00a05a204cae17a802d4f2cfab Fix RBAC for hiveapi.
97cdb87be521d55697f79e41e8ed515ca76988d0 Move hiveapi to port 10433.
8b1c393442db7f14c3b7d9ec79619aa409d1159b Merge pull request #815 from dgoodwin/hiveapi-fixes
a0126f6d4e34ce30c021197751f4abb0a5ddc761 Fix RBAC for hiveapi.
0f4aa2dc43b31d36d4b22815db002aba7408f3ee Move hiveapi to port 10433.
1f12b6e4d1187769c1773a0b10378253c78dc1ea Merge pull request #813 from staebler/migration_delete_dry_run
7648f4d4c48c5901b0405a011c1a78f863363b4e Merge pull request #814 from staebler/olm_template
2f80fdfb9962308e082411ff73ef4bacd4399cdf update olm template for v1
552280c4b3ef785229ad38418e776a13c8727cc4 Merge pull request #805 from staebler/merge_in_v1
f0a6afb8e08968b410bd6a1fde367fe794a83153 migration: do not mutate object when doing a dry run delete
5e39753bba3c3b8cbb566afdf43f81def484dec0 Merge pull request #811 from dgoodwin/backout-libvirt-rpms
5d10df9370261e5821f028d351324ee88ca7c6c5 Merge pull request #812 from staebler/ensure_pipeline_disabled
ec6e9fd5b67a10c1df69fb7b6c44b7bd64756e40 controllers: add doc.go
c95128313ec771470c478584cb676c93b003f5f2 Remove install of libvirt deps temporarily.
6d92db9f68fc74d9d2a734198d4f6d8224fd2eff Remove install of libvirt deps temporarily.
03163b388f5c1211cb7fe6fd639fb278f07ee8de merge: fix bad merge of Makefile from v1
abbfa5e4b9ed0aa841d25a77e98881a1f9c1c06c Merge branch 'v1' into merge_in_v1
2a1e9c94c3e9b45b8726ad6277d3874c8d4db908 Merge pull request #806 from staebler/build_image_mockgen
214f70196b13370613816e0b54f89b276cbdc724 build: include mockgen in build image
300286756b5b5b7ad11bb3493824e7285712b4e4 Merge pull request #803 from staebler/migration_restore_status
5441b7da2cfb7cd713b207ddf72eae813d8d468a Merge branch 'v1' into merge_in_v1
f62f768b73f8561748968975f1625b28cb0ab11d Merge pull request #802 from joelddiaz/create-cluster-types
5d956c32c2db5080db8012eeb357caaf676df28f migration: restore status on re-create
e8af026943191a598e6aa34fe663b16295b56282 add type info for syncsets and selectorsyncsets
d6803ca2993138b2e9e18f7a6c47a5a9d13eb6ef Merge pull request #797 from staebler/apiserver_resource_version
0c9b363c9feee0bafa37746e86ef4b5b4e7862f0 apiserver: clusterdeployment resource version amalgamation
5d26c05f298a71ebb4e415adba7233a1bc1d5d31 Merge pull request #800 from staebler/remoteingress_spelling
7c2944c373da4d5a71eb17bc244b81741df24df5 controllers: remoteingress spelling error
9117102fd023792553cbdd6c8413669da63a7a78 controllers: return when syncsetinstance controller cannot build rest config
353167cf8b7bfe313663d8b54a8a912b27b79313 Merge pull request #796 from staebler/apiserver_certs
2dab406332e83cf684e4a98451d8ee7c2dc211ec Merge pull request #795 from dgoodwin/ssh-known-hosts
5ae631f5043e7307b8db9baad220b6c6b22fae56 apiserver: update migration README with certs step
176eefa2185ffdd4fdd883b5501b635733e50c58 Formalize addition of ssh known hosts in install manager.
c1dbfba0fdb6a4bfa8345ea672849d4a89e0900d Merge pull request #794 from twiest/velero_owner_reference_labels
69425f9f98d92d1c993bc3c3cd964c4a91f04b90 Add labels for syncsetinstance
520ae4cbf17d9542f28be66209cf2642525f9c4d Merge pull request #790 from staebler/apiserver_watch
7edc0d7d842214714c79b9f90a6ce7221de43694 apiserver: watch support
a876a2be0a9a3f067986e35f489af3c816f05304 Merge pull request #791 from staebler/hiveconfig_restore
964cc92ddf961a0f9f323d0c7a37d1d923142211 tooling for restoring hive config as a separate migration action
b75bdabbeb49c66850c743621414e3f996d13625 Merge pull request #785 from joelddiaz/api-server-config
cec972885d083636d62068d1a553e8cab742391f Merge pull request #792 from dgoodwin/log-regex-aws-nat-gateway-limit
db1a368508c8543b83f0e4d3b2fff24144ab6bda Merge pull request #779 from twiest/velero_owner_reference_labels
36fc72f0963524cab1e74832a69c52a0ad8affcb allow hive operator to deploy/tear down the v1alpha1 aggregated api
5e86610a418b908a1940a8e0cf5be50a0166ac96 Add an install log scan regex for AWS NAT gateway limit exceeded errors.
942cb9400786ecbe74f31023660b492a387e7966 Merge pull request #789 from staebler/apiserver_status_updates
fc9418c91204e69e83b7f108fc58646d3f24f0a7 Add labels used for ownership reconciliation
15d16a49b6380b3a8e214a4ef03194593121a7fb Merge pull request #776 from staebler/migration
99c7cccc769326bf85f98c8e56d779e21acd07ca Merge pull request #755 from staebler/cleanup_iamgeset_jobs
3e80b06b5142c14c566cc8bc786b32670e2da1b9 apiserver: send status updates to v1 API
b4f6b7dc8d3f71886d0f10ca80cad9df36e29186 apiserver: handle machinepool conversions
d80ca91bacf6c8b0ec6e8c16d92244d7867bd71b vendor: clean up vendor and add github.com/openshift/library-go/controller
8bb04c5c955a9275974a2f3fb161aef152c35883 Merge pull request #783 from csrwng/reftypes
4554f99c53d841f5c4137f6bbab693d44c80db3d handle re-create of HiveConfig and DNSEndpoint
f6136cf401387ba6db36cf9b0a074e9f7447b062 update to v1 migration tooling
5b7bbd244e3a25880776cff714d3719cab2b73d4 Add phase1 and phase2 v1 migration scripts.
0c15a968881ee48f02fb113b99ed30f91f70aeb5 Merge pull request #788 from dgoodwin/maint-mode
6d3e7a1f96ccd0b8a5f1be406c25c11d2eda59a6 Add maintenanceMode support in HiveConfig.
4ed85412fd05922cf11f508f5dc966a3af882c6c Merge pull request #787 from abutcher/cd-name-samples-syncset
8e8ce9ecadaa2b14d9d28fc16e5393c5e8c75135 Add cd name to sample syncsets.
e8e6159455219fb12e19ba6b1a6c0010f280a797 Merge pull request #784 from abutcher/create-sample-syncsets
644a5faabeee435f03dd4528eb08ff71bc2b64a8 Add --create-sample-syncsets to hiveutil create-cluster
a8e2ac9824eac0f1a0d97a05a3ac418f417b4bb1 Remove use of ObjectReference type in Hive v1 API
846c8ad71dadb6df45d97844d44d7fc15daff25d Merge pull request #777 from dgoodwin/adopted-status-urls
02738988dd83815ce8d91775e91e71745a565338 Extract URLs from kubeconfig for adopted clusters without a provision.
1ae1429ffbc31124f95682b1ea9ded265074e5af Merge pull request #767 from abutcher/configurable-reapply-interval
5d8650f58c02f41cc79c2bbbb5ef7a91c2b7e734 Merge pull request #778 from abutcher/resource-apply-mode-doc
4b149b5355c957c6e86fa4ab5b704c2de2aca2e4 Update Sync resourceApplyMode description.
2932bc340cbc6991d3aab57cfd46a4ebbf4330ac Remove ApplyOnce from SyncSet doc.
5a784d384e765822bb2f0117b88a957fde685e16 Add configurable syncset reapply interval.
face6e6b55259e7de038d950a1cbece13142741e Merge pull request #773 from staebler/hiveconfig_update
37fc8a907d29e8c912fbff9730b15280d9177f6b apiserver: block v1alpha1 hiveconfig updates when multiple managed domains
3c2f6a36cb532eac6b3e4b1792e572cb95641b8c Merge pull request #750 from staebler/no_master_machinepool
eceacc3c60fa5bf2dab672115a0ef2318cc22af8 Merge pull request #769 from staebler/apiserver_updates
9be42d99537f6676e5d507c31688d5c530da915b apiserver: updating existing object when converting
d5ae0a02012400f7188f5e908e6fa67698957359 Merge pull request #766 from staebler/apiserver
3e3fb8fc85769a9831a3293eb28b2046d992ae87 set up apiserver deploy procedure
ba82b0065ee1c5a48c1a508f6825b2e274dc7511 create v1alpha1 aggregated api server
c4f0d7946ab438165d132b0512d885a96e9ef9ca move controller-tools from vendor to tools/vendor
65643f2a90f54ee8db540a1766bb045dbabc2ca2 update vendor to include packages needed for aggregated api server
94d45449ba862a295aac70045153cd57253d13dd Merge pull request #764 from staebler/selectors_in_client
f3b994562c84e5cea94284bc8285e002d389be17 Merge pull request #751 from staebler/dnszone_actuator_logging
20e382280909f6071189ef0b7c57555a70019d31 Merge pull request #749 from staebler/remove_default_machine_config
1e15fe1919068798f0012a6e1b6c8ca1fd1c914a add selector types to generated client
f12a23ba3ee502ed8e71761e1d1af3c080e3adad Merge pull request #758 from joelddiaz/multi-cloud-dns
f999e6c8e80f2e2b4639537dc235008c96c263ea Merge pull request #762 from achuzhoy/kubeadmin_pass
9f6576ea941e4092d62f966560fa88a0dca54603 New command to retrieve kubeadmin's password
8e8d0d33ee843dd3256e1f2c49468c0c9d8ce40d Merge pull request #761 from staebler/client-gen
51f2b9c79c6db8dae0ee303143cdf82000f6c512 generate clientset
99c3874a86a6ebc6cd97be04b799c524bc88ab4e allow managing dns for multiple cloud providers simultaneously
2c10c9a77ca25369a9a4a3585a1592fc95cd34d7 vendor updated testify
9d7bf5350ca3a3006139b3993cd4f5361010d4db vendor: k8s.io/code-generator/cmd/client-gen
a27fb102f6f279dd0d94006c646ab8485dc27918 Merge pull request #760 from abutcher/controller-operator-health
44c15c314eca193c3ff40499d89d6ca10e82ce17 Info log starting up messages.
ebc27fa2abd6f3a6b6b9e12e309977999a9e8f83 dep ensure && add go-healthcheck
683803ba4c29ec0d4bb0ffbef975fa913ca882e0 Add controller and operator health check.
c087557794a869151ae3fed2c2272dc0bb537e83 Merge pull request #759 from cben/build-docs
76a4c014bd12da2f07d5e82791ce11a7feb4ee52 Tweaks to docs from trying on a fresh checkout
d1db6158b4c86e51d02675dc6af5f318eaeee5e1 Merge pull request #752 from dgoodwin/bm-libvirt-ssh-user
5520264bfcc88f7f70f411c2fc17a1d18ddf8d34 Merge pull request #756 from staebler/pull_secret
269921d81b4c884651e218f34de8891dd307c1c3 Merge pull request #757 from staebler/dnszone_notempty_delete
17da5f2d80558e948dd1916087818c576e2f1d81 types: remove DefaultMachinePlatform
5306849525526422e0c2e6969a0fd5470bd4796d Merge pull request #745 from staebler/no_gcp_project_id
124aa5475c81ca8aa611dbc7c31fc842785914a4 dnszone: info level for log when deleting non-empty hosted zone
235a7b6e4ba2df3a0fef7a9683b4261c846bae12 install: use merged pull secret in install-config
8e179e472b3a83cc243903551e422a16f8e646dd Merge pull request #754 from staebler/api_url_override
0fa575fb6c2c2f435c7842eace4d955092ac4995 api url override
8ffc99ac2a344bf0aeedeec6f9f3bd357c70ed5a Merge pull request #746 from staebler/env_var_passthrough
e9607589e95e6dc000c16d3add4ba235456f7aa3 delete imageset job when completed
b89e786feef4724a61430ff2a64f1371c0498c04 extra installer environment variables
9233709916e36ac69f2e9379be09e67e052b09f8 Merge pull request #742 from staebler/no_installer_image
d031d0f24968b7d9bceb68f1b06e4c9ec184b88c Merge pull request #748 from staebler/user_agent
817692fb462f0044d1e9b10f60045c984203f96f Merge pull request #738 from staebler/move_provisioning_images
b0100844e143c57c1e4cf3bc458e144b573165ac Merge pull request #744 from staebler/machinepool_scale
c71e0228ffa62840bc1bdaa1f511eb3caab64286 Fix baremetal provisioning when run on OpenShift.
d2c990dd05c1229853e2fda3b3c8b682fd9d1cb4 make logger field names consistent in dnszone aws actuator
2f83292d77d58a7a7be2f58e97de9c8ac8c2795c validation: reject machinepool with pool name of master
8e6d434e311c1c92abafeb7fdc34977214ea1f45 remove support for overriding installer image
d55aaaacefe1ae37c903dfc485bb81cee7213584 Merge pull request #747 from staebler/log_level
4bf7b257969bb5b6b15bf1d9a441d3144f963d72 add user-agent to aws and gcp requests
ded88637af8954860205777fe47ff1549be83697 remove gcp project_id from clusterdeployment
fad07059e337ba0bb99869dfe8c8bd032d3d06a8 add field to HiveConfig for setting log level
6e12830583deaf3481a44bd7dbd55067fcc7d650 types: add /scale subresource for MachinePools
d51bc782a3a599e65d0e80efc3dba602ab0403d9 Merge pull request #743 from abutcher/fix-env-cache-dir-regex
d173f24e46a17ec43a17558ddc3ba80613a916bd Remove variable cache dir from applyTempFileMatcher.
9d2de7000523bef91020269ecc64e30340630ea2 Merge pull request #739 from dgoodwin/v1-bm-deprov
086a2070e88808f838fee2d673a6cbf4eb47da86 types: move provision images
725c4e28167550155331c9ee12f23215a881cfd8 Disable deprovision for baremetal clusters.
a84e993ee6b346633626a6e2b998a76e6098e36e Merge pull request #723 from dgoodwin/baremetal-validation
bd9e01abaee50f9dd21f24ac03c453cc9ad9d7fb Merge pull request #741 from abutcher/restore-apply-err-condition
9f34189d174c5a2bb6478fc05cbc4dc544278a9e Use regex for filterApplyError and cleanup test/comments.
d910e50ef84a24d605ba40a09a9ff75d2ad238ea Remove temp file from kubectl apply error and restore adding error to syncsetinstance status condition.
307b581809617f05b737a2765178cd7a1af4bb4b Merge pull request #736 from staebler/no_mockgen_install
5c366e437faf5ef0569ea965d03ebd234efe6dcf Merge pull request #720 from dgoodwin/syncset-metrics
90a27b09f879ff47e21075f88d7cdc7c13c81f5e makefile: do not install mockgen automatically
3f1286028a4535e64be2ee12c69eaa550e7a0c2a Merge pull request #737 from staebler/include_mockgen_in_build_image
677775d84ae8be437a8a91d5633d2544c62e949f Add SyncSet metrics.
dab26c6d5e40b07b1b42166b2f7f8b1d56090af7 build: include mockgen in build image
e74bee2e4a65d9c5b3b8d8e1b0728c820a4fa556 Merge pull request #735 from staebler/machine_autoscaling
8906c0c703563520185e4bc50420ab02a7459a8d Merge pull request #733 from staebler/fix_installer_logs
be36a4abf3347f6507319c0ccd866ab8a48c77a5 Always initialize SSH agent in installmanager if possible.
f2f280075341565b5ea376b6fced90fead339635 Merge pull request #706 from staebler/remove_dnsendpoint_resource
8d5fdb1668e7ac4578b8b5793c54d671131e8c22 Merge pull request #734 from staebler/merge_from_master
30db34d2940a11e1e9a173a570fc5a09e31a1ccb allow machine pools to be auto-scaled
8f2121f525d6f68aa8129c4ea291f3e242269932 vendor: add autoscaling types
eb1e314f2d0daa455d24de78e36f1f9804345912 Merge pull request #726 from matt-simons/v1
54d29e16406b80bc404f89c133760ddb70e1408b Add documentation for secretReferences
6835ba726dfcb7516d887ae9135703ffcac7cae8 merge master into v1
bd0d95cfb495ff820a146e4df78c422d325c67de Merge pull request #727 from staebler/gcp_machinesets
c708359354e65f9a228e6f571837355de587b9f7 types: remove dnsendpoint resource
b278c4b1fd6d19cfff30546ffaf6d5ac8a132080 installmanager: fix interactions with installer logs
98aa00d62bc2a521060ec9c4df17275652a371b3 add machinepool scale up/down test for gcp
e5cfd46e37256f2417c1cef0726cf4ae8e791ffa Merge pull request #558 from abutcher/CO-499-rm-apply-mode
abd242e2d4c050ebda55ad680ebbb113f47723fa move gcp machineset functionality to remotemachinesets controller
b792185a6c288bf084ad52cf538bf3f4cbf3bd23 Merge pull request #728 from staebler/skipping_machinepool_validation
cedd32401b2d919aa055fa12ad5b7caccfeca4fa Merge pull request #681 from abutcher/ssi-requeue
52f4af9541b2062ed1eed422fb19be3d5017d164 Merge pull request #729 from staebler/provision_cd_column
d4bead4e48ca12a65dc50b94329f2e6e41bf1a78 Merge pull request #730 from abutcher/fix-secretRef-validation-kind
efac892848af140987487e75ea192d4a7e024dff Fix secretReference kind validation.
d1089914c2daa8703bf52f65977146cb5ac2540b fix ClusterDeployment column in cluster provision
99da6863a889c68a0ae8bb7dd9dd1e0016efd469 fix machinepool validator so that validation is not skipped
0a6bd66423360c79d9cce815c2e08bebe81de2d0 Fix incorrect json tag in API.
4578c57eefee500cd78ad564dab6cb071bbd727b Add support for a CD annotation hack for ssh known hosts.
e130394868bf989346a2da563d90a5d7c5dad496 Merge pull request #724 from twiest/doc_manageddomains
0d015dd8d1356639ef6fd88cebefbe9cd3a96767 Merge pull request #722 from dgoodwin/scale-test
93abcc1d9b73d2721f90f32c65d2dfdc9e3a3dfa Add docs for managedDomains behavior.
1f0cdd7b48597061cb13a11217ff204e6d849f4b Allow bare metal validation to pass and begin execution.
33abab5d85217e8db61f85a9dd286e03edb21e06 Merge pull request #721 from dgoodwin/v1-baremetal-initial
9a0f2d4ebc9efa6e339f1aa3514e6f58670d1655 Add scripting and notes from first scale test.
c6cac59f90f0892e5451947cd46b417982aac778 Add basic support for bare metal cluster provisioning.
dbba4e8a98ad315f9f6863ca7df493b5480bfbc5 Merge pull request #718 from staebler/remove_machinepool_finalizer_on_cd_delete
7f564b41fa2e8ff5f1b4e7da5844415f7482348c Merge pull request #719 from maorfr/fix-hive-frontend
07ba355e49cf3af0e97e69096db2cb2fb8d21c20 remove from bindata
9844c60ca125059fa76346b3e7293ceb5bf02221 fix hive-frontend ClusterRoleBinding
646c4ab998eece49a69026e4e70f91bea2b17a9b Merge pull request #717 from staebler/merge_from_master
f2a2cc9dae39b7c783141b621d51e6304fa09953 clear finalizer on machinepool when clusterdeployment deleted
46093b43d4999e534900d0ba6a303e760f7a81f4 merge master into v1
e0ae973cfb10e1f7661901087887926ceadc4bc9 Merge pull request #716 from maorfr/fix-fe-group
b1af9a21d0cff18b6499d008b30a347b2f8e3aed hive-frontend ClusterRoleBinding fix
92d10cedf8d7cd3d801c05ffe56a42cc61148ec2 Merge pull request #715 from maorfr/hive-frontend-group
258dc86be397b7968664f200adfb132931cb4f6e add hive-frontend Group to ClusterRoleBinding
f3f77df97bb2191726c93e552ef430a907f77e50 Merge pull request #712 from staebler/e2e_tests_on_kind
eff13e794c398023d5a5f8a0d92b045f5614e0ae Add separate ssiReApplyDuration test.
28dfd5a5bf5027983fd5040fe90d96b28ed8031d Merge pull request #710 from staebler/enable_managed_dns_for_gcp
334a324eb78886de06727a23b1435be9ba0c23fd fix gcp resourcerecordset contents
b5f1ba673d7a8f90ce021e3b05c27d1a036c1cc0 Merge pull request #713 from dgoodwin/v1-aws-dns-secretref
b1fad16dc9b7d3faae040533dc8e382649359e4a docs: update using-hive.md for managed dns on gcp
947d6283b9c99e7af8be4f4c16b0d1636e72bbf2 e2e: use managed dns for gcp e2e tests
7ef880d18ba64dbb779534b6e0cf56ff2d7f132f enable managedDNS for GCP
bcccc796ca74f06d40cbadc3a12d3e52555229f4 e2e: use namespace instead of project
e0915c9649e52f990a93f69fb1410c057aec5b25 Remove ApplyOnce PatchApplyMode.
bd4b4a260c8231a7d108af3dcc167381de735e40 Rename GCP DNS credentials for consistency.
48f6a37469c65aa06a64a0804464c965410d8f71 Remove region from AWS DNSZone.
1d8e97296a2afb2b07940f3864513721b4879b98 Rename AWSDNSZone credentials secret ref for consistency.
bc0a1eb2f923a69c06e2a141046c5f90ec8ccc66 Merge pull request #711 from staebler/git_ignore_certs
1e05e459c7289178002b40d3ef54edca8c8480a9 add hiveadmission certs to git ignore
945f696872849b123373f314dc3fa71f9768beff Merge pull request #694 from joelddiaz/gcpmachines
5ba53e5b68d17e3ecef3c79e960a88d22aca80ac Merge pull request #709 from dgoodwin/temp-prometheus
9eb733feb41249c14e4a5e28df7e9cde23cd2ac4 Document deploying a temp prometheus to view hive metrics.
357b906e4594e10bd39e96126ffb96295e07d87c Merge pull request #708 from joelddiaz/onegcpmachinepool
5c2a7cfe6c69ce740c7604cc67bfc604879ad9fa clean up field path names
37688f7b05d055db130b3a434d96db796ef85410 Requeue successful ssi for resync.
6d7c773320ff5fd4f78b7cf0d828286c9b7b7fe3 make sure GCP compute pool has one named 'worker'
e8ad5b3e8ea6156b5207436b806881dd07538089 do not allow more than one compute machine pool on GCP
0ada6fcb45f2b8d5edb107855080d35c1250bebe add machineset syncing for GCP (using syncsets)
c312c02e7b7d39dca24186f13d9d0593127a2649 vendor GCP bits to enable syncing machinesets
e3a0112632c921f70527b2e5573c6ca6a6c52f4a Merge pull request #698 from twiest/dnszone_gcp_actuator
fb4624584792da40980ecac9a8b7c45436461aaa Merge pull request #705 from songleo/patch-1
6fae374d8ac60453194c2062ed4514d9bbe4cd1d docs: modify CRD to CR
bff3d25dd68a6aff496b3a79f0ff98143acaeaa4 Merge pull request #704 from staebler/merge_from_master
cff28c729d94bd4ec734fc67c663f9bd4786a3e3 add gcp actuator tests
651b5911f9bc78ff457065e9a8553dbfcd0b0970 Rename mocks to specify aws.
c2cfc3a08abdaee10f698d125130adfdcfa11f6a Add a gcp actuator to the dnszone controller
8aa089a6b968d304a404b213f6fe2f55ece5de4d merge master into v1
6231266bee9ea721f2b0caff6c12c16820dede48 Merge pull request #701 from staebler/dnsendpoint_scrape_first
b1ecbb5e5dea0bf8c17cbc5445414ab4d5961658 Merge pull request #703 from staebler/v1_default_deploy_image
d4db42978e1ac2a86fbdafc8e976debe16ff2c07 use the latest from the v1 branch as the default deploy image to use
7ad6648e36d0b4eb1a7b73d49232d9596794720d Merge pull request #702 from staebler/merge_from_master
4631a75557b53dd9958442a75e8fbdb5cfd966d5 merge master into v1
949243a9914ea48aa6108b43b618e4c3e926a9bb Merge pull request #691 from staebler/machine_pool
a315f3251680b71771fce69838f86c4b91a2bf9b dnsendpoint: do not reconcile until initial scrape of root domain
e4c83ba89ffafc16bc35081b0b93096f6e220eab validating webhook for machinepool
8eb94b2626a3dbfbd8aa465a1b61fe658a704254 move machine pool to separate crd
a057c9fcff2fd64fc2c7555b522b3109263f4a12 Merge pull request #700 from staebler/fix_dotting_for_gcp_endpoints
a533c55222393449de85b24a759bab3a2355281b dnsendpoint: fix dotting for gcp
11b64878fd8bcd846e80de49bbef12f341f2f29d Merge pull request #699 from abutcher/sss-matchlabel-docs
82e7fa6620eb67a7f9b96c99c99e17f473d5d65f Merge pull request #695 from dgoodwin/v1-safety-checks
a6f2ddd177ec7c16d4791a464a2a990f2d601542 Merge pull request #696 from gyliu513/mf
e200f95dd29f0a2fb05abf6831ff93e25daaf6b7 Prevent running a ClusterDeprovision job if owning cluster is not deleted.
8d26a65a8a66641b034f5d5181b1172650475d79 Merge pull request #697 from dgoodwin/v1-cli-adopt
33c573c30162f8b36cf104a995809bc742f8370d Add hiveutil create-cluster support for adopting clusters.
079b0ece25d3cace2f12c9674d78ddf894425a07 Update SelectorSyncSet label selector doc.
5837b7e913a63d05aa73bc4a5c91c26abfdc0717 Updated makefile by adding .PHONY for make target.
f003d73422d367817599f66ede534f41c95834e7 Merge pull request #692 from staebler/merge_from_master
f4ea418f4982d7145ea210930cd1e2251ad88099 merge master into v1
fc36144c03b94a04b0cf8998a30f6603705398a9 Merge pull request #688 from dgoodwin/v1-azure-ic-fix
3c8947d73ca529a6d3e2b5c2f6c6b434d2f9c12f Merge pull request #687 from dgoodwin/v1-rename-deprovisionrequest
64ff3eaa49362e1ba1d3e310cfad03e2b33c951c Merge pull request #690 from joelddiaz/skip-nil-secret
105cae8c337ded4158e858a6d92cec0dc7324bb5 Merge pull request #659 from staebler/gcp_endpoint
6389320e27833d9ef8af3135341b568f431c5350 don't add a nil secret to list of objects to generate
488b0896072b263edcc143e988880a00cbec4195 Fix missing details in Azure install-config and CD.Spec.
7100962a1f059a36cc65f9f431e6ecd12bc281c3 Merge pull request #686 from joelddiaz/ignore-empty-private-ssh
b2ef054c97869de94b33e8b1d6ef80ea16cfb0ea Refactor ClusterDeprovisionRequest to ClusterDeprovision.
d579f4b2b14f9187ccf46430ffd0694e7320aaf0 don't create empty secret for ssh-private-key
dcd886a31ef9aa26608eb5bc4986d172873a6181 Merge pull request #684 from gyliu513/e2e
6db69a44b2d84734802cf1a117200f1eccd5ce94 Merge pull request #683 from staebler/fix_e2e_tests_for_v1
814718aaae2dba796a41525fd6aafe6d8fbc2954 Merge pull request #661 from mvazquezc/mycluster-ssh-key
447ae7db1d37549586078264b47c83fe8f26aa23 docs: updated e2e test steps.
ea859e339c820d8647804f4c0033df5d1d7d3d0f update e2e tests for v1 API changes
f5faf34a858170631e90515d543fabeaffcf2d90 Merge pull request #682 from gregsheremeta/provisioning-and-installconfig-required
12df18172da2e7acb47f11eebc35cd94bfa72603 make Provisioning and InstallConfigSecretRef.Name required
bd2877bcb10a04ac330630f3b59c4eecd6ad3b94 Merge pull request #680 from LalatenduMohanty/change_file_name_to_v1
b7b4eeb131e962a7216f891aa0922c8fbce1d44f Merge pull request #679 from dgoodwin/v1-infraid-display
53d2e1bf70454505467164b13a9172b42b58402e Change the file name to v1
2ecb92277c17f16c7fcf3ec35f3869497f0cc170 Fix kubectl display of InfraID for new location.
c53bc2d411046e376b3468e18317fc6fe974140f Merge pull request #677 from staebler/remove_federation_fields
146712cf05e1e48fe6b36250055d2599fa3800f7 Merge pull request #678 from twiest/v1
cc1d32de4d15d7ab571f8fee97da3884d94a85ae Rebuild bindata with Ref name changes.
51eadbfd3a115dc8ea9fc1546aad74f19fd33471 types: remove fields related to federation
792d81cdd77b636868905a6e1283dcff03077795 Merge pull request #676 from staebler/ref_in_validation_text
a2b348a0aabb960e644787ab722d572264de16d8 Merge pull request #675 from gregsheremeta/update-status-conditions-on-spec-2
6e0cb40bce38915d1e0c10bd855ae14699723841 add Ref to responses in validation failures
ad7aaf42b55cf89c8c5451ad3afcf0eabb2c65c4 save infra ID in Spec instead of Status
01990d9537d4b96714f1ced8178705991550ef9a Revert "update status conditions on Spec instead of Status"
73398ac1266c54ef025f08b2ce3384dd30aa8c8a Merge pull request #674 from staebler/add_Ref_to_ref_names
ff71bc8f02a5c1a0df9a18adf47d29d58c8ed6f7 Merge pull request #673 from gregsheremeta/update-status-conditions-on-spec
d039c293ae9e4f043021b8b2f883c4bf847a5514 Add "Ref" to the name of every reference field
47dc180276316ea74b15973a18c46dd126834a46 Merge pull request #669 from staebler/rename_secret_refs
8ce28f850af073d02c497c28cdc53b19ccfedc22 update status conditions on Spec instead of Status
2bcf808b2062de3b0b2ba5358409c485286eca8e Merge pull request #663 from joelddiaz/require-instancetypes
16a3e033f6b7577d842e7dd4a6d5e271d8b551b5 Merge pull request #672 from dgoodwin/v1-clustermetadata-nil-check
95f2e7f6d287d795bf04b8aa92e2241f7640155f Add missing nil check for ClusterMetadata.
e58e4ffea645900585d669ad33cda0a586b75bca Merge pull request #670 from joelddiaz/big-aws
b1a4ba4dc18a4d5fced6952c9830b32a935d19d7 types: change names of references to include the resource type
d29041b80b945efef409b4b474276aad91927d50 Merge pull request #671 from staebler/fix_v1_integration_tests
88163ae663f37f0b49a886df382e491aa4af2292 fix integration test still using removed fields in clusterdpeloyment
8daf9452e9a299fd60d82b08abcaa438cdee1de0 bump default instance size (match v1 branch)
f51c3ed37de9cd6d473cce8cb268fb4628f900e5 Merge pull request #664 from staebler/custom_manifests
65d87a96aeab0cb346f330b5e6f44fb002c26b40 use manifests configmap to simulate bootstrap failure
e016fe1ab4e754ec16e62f410ffa96a4410900a9 allow user to add manifests to be installed
493d3f883844d8ea941d889ae2ec5991bbc1648b Merge pull request #648 from twiest/refactor_dnszone_ctrlr
a53fd817039de8bdb2877182deaafc63f06436c7 Merge pull request #662 from staebler/cluster_metadata_in_cd_spec
951d9062f116c098d2b94d9bab88d51c23534b70 move cluster metadata from status to spec in clusterdeployment
af4472b785569dfabf09ae59e512e2ddaf258b51 Merge pull request #660 from dgoodwin/v1-install-config
a120b02f0aaf33b066dd92a6d940afb2f85717bb Add InstallConfigSecret for v1 API.
2f240d21a38b4114922c1f12503f6f5767e8c4d2 Merge pull request #667 from gyliu513/kind
83c0ae3228c8a42f731cefd5102a673a140a1def Merge pull request #665 from LalatenduMohanty/fix_duplicate_script_failed_provision
97ff785b8adfc50fb8d7c3b06410be4a0e1ad0e0 docs: hiveadmission-dev-cert.sh request cfssl and cfssljson.
4a61acbeb38fd96913126ad6293451ef1148f1bb Previous cluster ID and infra ID must not be set for pre-installed cluster
59751360619e6e42082e70a497f1b17dcd5bfa8d Refactor dnszone controller into the actuator pattern
8d28a1b7a12389054f3e8a4cd8f38776e5d286df support for gcp dnsendpoints
4278a66b169d9d237eadec0e97afa0097899867e Revert "vendor: update dependencies to remove github.com/miekg/dns"
11a2e62156f45d07639ddb4a6241ef5ea3b7c8df Merge pull request #618 from staebler/set_spec_installed_last
03b69219d38e6df9cb927215cd2b1ce134da4626 Merge pull request #642 from dgoodwin/kind-fixes
8c1c7d8a8d5ae3397484466ed2188388d2a6c010 address PR feedback
1d0013e49fef4e1160826b930d4d3cf27a001275 add webhook validation for GCP to ensure the instance types are provided
2e81992a56c597e620d152bb89344e175cfe907e Fixed k8s typo
e061d3f01c539d0c09f4d942330ed0ac6e9f6018 Added Devan suggestions
9bbec12118bbb678c0ed323173ac6794edd7f712 Added ssh-public-key secret creation
fa0ecccac85bf980488de1d020383ec14030dd7b Merge pull request #652 from dgoodwin/v1
c33286fa4bb2c6e06133254405f903406428685a Merge pull request #650 from gyliu513/delete-aws-cred
9f203b43fbe6e6fffb19187b8d111c7be6879de9 Merge pull request #655 from staebler/no-external-dns
e773d9acae45a13b9fbb12d53cb9b920a1ac02aa Fix additional refs to v1alpha1 in config, templates, scripts, etc.
b75ae6df4dd66c90ac9ca830a6e3589fce112e06 create external dns in hive controller
6af13008483139cc691e5962993b8bea88a2a11f vendor: add github.com/stretchr/testify/suite
10329f22fa1d56dcfb910c17bb7f5df195401bfb vendor: update dependencies to remove github.com/miekg/dns
2f554f8a481887def167e6257d920d2b466b82dc Merge pull request #651 from gyliu513/faq
bdd4ccd5a215df9a2473b84520d78a6496eb7c8e Move API from v1alpha1 to v1.
ba8a72bc54b7927560566ea14edd2b49bf214ea4 docs: Added syncset and seletorsyncset to FAQ.
0a30faad05c1c6c79a62b06ff3fdf857a87e538f docs: added a note for the creation of secret for AWS
29dd346e821c1f7f8c20cdaa3c00990ac68fcd8b Break create kind cluster scripts into two steps.
b2c325eb8d828d6b5cc1c5cdd6b493740983fd38 Merge pull request #643 from gyliu513/dev
14f5c62dea602ce3db5d495ec7bd7d5c28227104 Merge pull request #645 from mjudeikis/fix.resync
c24f034e41cb00d7db457c083efbbb79b04e06fb Merge pull request #647 from staebler/fix_cluster_version
b7bb4a7a158d0bd854ea1ad80af377a1c6400bc4 controllers: ensure valid cd status for imageset jobs
4a6f0f3a1d1e54f38907b181c3e883bbddc37cb5 Add script and docs for vanilla kube (kind) deployment.
c1c0b8c58f926997784b02504d19647503b7fe14 fix resync
fef9867bb8655ee736706019c34a79eb5ecad437 docs: Corrected aws environment var.
e9a1bcd5ec8d40764b2d965843d0403ea3ad00ba Merge pull request #641 from staebler/remove_kubeconfig
ef0e86a08c00d537e8394fcf205b79ce67da5b49 Merge pull request #639 from dgoodwin/fix-operator-watch-errors
8e539d230147eab364f1dac61653f403fdce19f1 Merge pull request #606 from abutcher/CO-587-syncset-resource-sync-cleanup
e3379427c0b88da10f7198e7e04596e7986de928 Merge pull request #640 from staebler/docs_more_hive_image_refs
258e56beb6a5c94536f5071ed5b3b0f9d7bc953a controllers: set .spec.installed last
e87939f107304e9ee0a5ec0a9c192febabbef97d Merge pull request #620 from staebler/clusterversion_validate
e374669661a8046f0cab7f3a8d77e22efde56cdb remove stray kubeconfig from testing
db5d9bc2675cab1a3adef7b1a3e2a80e79a1c48f docs: remove more references to using a custom Hive image
50ac2561c0c9f9885e459c857134840ab09045ee Fix error in operator logs watching DeploymentConfigs.
1c37153bc9a1aae16dc1a40a90328a2e2a13d1ab Merge pull request #613 from dgoodwin/manage-dns-e2e
32fd3c12799a0afecc55864c776c1954fd920572 Merge pull request #632 from clyang82/br_hive_imageset
ff9e3aadb3191dce9daeebdf89c03d7087782d4a Merge pull request #629 from staebler/syncsetinstance_getcommonspec
9782d04511e017cd909b9f95623b9c1111b39042 Add ClusterImageSet example
4d54f29a90e161f34a0559262b26f22581ce1c9b controllers: ensure all status update of clusterdeployment have valid clusterversion
acbbe97e68242fd057f38753d4bd2c45bbbad8dd Merge pull request #637 from LalatenduMohanty/add-staebler-to-owners
3d07dd7c088df0c57013656b6de704f2a29d614f Merge pull request #636 from LalatenduMohanty/add-loginfo-setting-platform
9d2a15327fdba5aabb7e67fec6ec9333705848dc Merge pull request #633 from staebler/hive_image_in_docs
414912546a332f0a359a841b5dc38b2f9b0a2613 Adding staebler to the Owners file
a370dacf9c59c3850000a3cd33fe9c0f07a12141 Adding a log when we change the platform label
08181a9c5e6981d9d80100fdc1f76bd03ac82298 Merge pull request #630 from staebler/syncset_spec_errors
77fc1657a37a883ba8643a4dd0b1b03a0c22c9f2 Merge pull request #627 from gyliu513/hive-platform
c964c2a2221cbf8a57a658ea56744ab0755096dd Merge pull request #625 from dgoodwin/create-clusters
b8bd838b69834c37acd876004a7e925d209eb15b Merge pull request #619 from staebler/delete_not_found_error
aab8fb5494721ca7c5a67c3c1a6f231e5e413655 Merge pull request #617 from staebler/remove_spec_installed_transition
2687036a9920d5f2e9e2865fb2764e8fd809182d controllers: remove dead code in syncsetinstance controller
fb6ec430ddb4a13224c949a23aacc7be91296a0e Merge pull request #634 from twiest/vendor_gcp_client
5ca7cda525b9d73b9d934d8867e2d84c6db90dde Vendor gcp clients
360b946bc32a16575a4ff3a425589bee0ff7f0de docs: remove reference to hive image for clusterdeployment
f8aa80269f96c4af7758c9b5e971c981d42cdebf controllers: reduce level of some warnings in syncsetinstance controller
ec73da1da372c9f0ee9cbeb36f43d2cd03050021 Add manageDNS coverage to e2e tests.
90ccea94937afba139dc0c2eee6f83050173e8c0 controllers: log NotFound errors at info level
3326fb3cd37dcecb7cdd9b212add75fa81244ff5 controllers: remove code to set spec installed when legacy status installed set
440f3535379f7fdc969ba7de458759ff7debc6d6 docs: Delete support clouds section
08ae9d507dadd94c06026bb334400de3b3c3a736 Merge pull request #616 from staebler/remove_delete_legacy_install_job
800c80aad0edc1feb7d44e1f2a5c43b6939f0870 Merge pull request #621 from cblecker/platform-label
4f2c8f34a620cf7f6ba5926cca7271e4209ebd65 Merge pull request #611 from gyliu513/using-hive
77fa709ee9acf6aa56c86cbac40977e138fb4e7f Merge pull request #624 from dgoodwin/gather-bootstrap
f81e5537baac331fa8d4d1f6909139f8ce1375d1 Merge pull request #597 from staebler/controlplanecerts_cond_changed
121ee287dde0923178580f2ae76bb1ca8ae04807 Add variant of kubefed's create-clusters.sh script.
019c192b86b878debb3a00b48ed48ad9a48c92ee Merge pull request #615 from staebler/merged_pull_secret_hash
f96061493a0c2d8d8968b6ff59c66603fb4db7b4 Fix bootstrap log gathering on 4.2 by using openshift-install gather bootstrap.
541c365fda9d12d863f40e9442cd765186e1c0e4 Merge pull request #614 from staebler/updatePullSecretInfoCall
cb2551f1cd89301031745f517c9e0205974cb8b6 Merge pull request #610 from clyang82/br_hive_pv
f2908155d307288894982c836756282080401d8b Add notes
a1175c2a5e58bd7d9dc7c9e1cf698d6107c36809 Merge pull request #604 from staebler/dummy_provision_with_installed_timestamp
6209698afac7a43e32649465a5efa4b7fbdf8e35 Merge pull request #583 from staebler/dup_create_error_logs
17af5b572915cd69869aac39e6ad51926c724a4d Add cluster platform label to ClusterDeployment
8832f60566c672d85acedb536816b1086840baca Merge pull request #612 from dgoodwin/kube-rbac
6db9f5bc46490a97914e775031759833abb193bc Merge pull request #600 from gyliu513/syncset
925cbe386590257cb8f453b8b11de24f68cfc6df controllers: remove code for deleting legacy install jobs
d8b8a9c09cb61a58a49a107736f50c63b6a204c9 controllers: do not compare hashes for merged pull secret
7726ee6a53bf1259aacffd50c676ae75664decb6 controller: no error message on creation when already exists
acb000d4f685d65fd120933ce7f8f8da60f0e419 controllers: improve variables and comments around updatePullSecretInfo
e14e3954da005ac3b512b780c00b39aa468374db Merge pull request #607 from twiest/remove_sd_release.md
09c9dbf87335af0e03f6e1351c8dd7be895287b0 Skip minor OpenShift specific assets when running on vanilla Kube.
6b9ebef7be5df30f8390b9aa309a2c63810459a1 Merge pull request #608 from inderpaltiwana/hive-install-readme-update
688f42657ae9dd3894e552f53ef86c564d842f11 docs: consolidate using hive
2af245fac21f29c05caca6c42f90ccd64cb89bf0 docs: updated some commands in syncset
3d307b5c4d092b63003ad8a7d5ff49e6c35c27a1 Merge pull request #603 from LalatenduMohanty/update_install-log-regexes-configmap
fe9974974ec3681317fa4dd2bcffa2ec68d020bc Add PersistentVolume in using hive section
2ad98911667f56a8c4cc36b6fc5402cb271fddb3 Merge pull request #602 from gyliu513/hive-arch-cr
966b6dd0c4859ed36842faadd06dfe41781ddf89 Merge pull request #594 from staebler/update_conflicts
404396006eb89d561bb7762eaa6a1065eee49751 go lang in pre-reqs
8aa1fa287e7f13877c7743432da567a9c9f48322 Remove sd_release.md
e07524873b54f632b894759490a1a6425ffb709f Cleanup syncset secretreference secrets when ResourceApplyMode==Sync
85a14e440c25d78d3e23c52b3b20c8dc97bdc912 controllers: dummy provision for clusterdeployment with installed timestamp
095d76facafd48c0a52babab5f3a4f5e16e8508e use info level for update conflicts
56933924cf41d88133f27b53061603632262da3b vendor latest logrus
aae24e54db2baecf700dbbe4582056dd809ec364 Merge pull request #598 from staebler/unreachable_cond_update
e0277d8216c162d1a6d07ead139d650dad59eb37 Updating install-log-regexes-configmap with MonitoringOperatorError
f8188fb174f2fd0ef3bcc4692543aa5b490b5c5f docs: operator is managing CRs but not CRDs.
0d9bf6fea6d98782dc5b2efc00c388451e11431e Merge pull request #582 from staebler/clusterprovision_admission
9699c66b29dfdd93d4045fc5a9305eda9efa847b controllers: consolidate condition updating in unreachable controller
618ad7a416d07328d230984f76b2fb641c246f10 controllers: simplify conds changed check in controlplanecerts
058d5f5446ca6a3e9f1a83765676d83a5f9c7984 admission: add webhook for clusterprovision validator
924ebcc1738b6349d09478635b17c09aa8ac9ec9 Merge pull request #593 from LalatenduMohanty/remove_old_webhook_paths_CO-595
62d487d46baa595b38dc080176b984b92954d184 Removing outdated ValidatingWebhookConfigurations
e9c7c46acc96518ee4f057273b9305822068e1b1 Merge pull request #591 from staebler/missing_clusterimageset
1d43f4b78df8c72347011a8e9f586bca3bb5f29b Merge pull request #590 from LalatenduMohanty/add_gcp_azure_to_readme
73bbc79fee20b1f5454a89c4581d0bf36bfdb85e controller: stop cd reconcile on missing clusterimageset
0883abe31415b13ccfe7d5c88408dd82b7ec34f7 Merge pull request #571 from LalatenduMohanty/fix_plural_name_issue
fa2ed47fc9d53b75cc0c9b55d4d0aaa929565f4b Modifying admission validator names to make the plural names of CRDs work
a352c2917612e4674f29384a1bb9f6bec8506574 Adding azure and gcp to the supported cloud platforms in readme
5907aaca1232fcf22926aad94bef418698abb029 Merge pull request #588 from staebler/secret_for_certbundle_error
61efe975386eaae8b26c21b18afe46e3816a742c Merge pull request #586 from staebler/validate_cert_bundles
676ebed5779801d681fd87b615c3739b10a6e87b Merge pull request #587 from staebler/remove_dnszone_delete_warning
ef97d58e9e6ca2bd4d0e883d6699f5006970237b controller: reduce severity of log for missing cert bundle secret
1c822f76c3feb7f810b38f25de587db6012e0dc7 remove unnecessary warning about dnszone not getting deleted
3384d52e4b078107b279401d3b28d601ac9f9d91 Revert "remove unnecessary warning about dnszone not getting deleted"
a885667e6e547314d3dd55d13c8fcdc3aff6676b add validation for cert bundles in clusterdeployment
d23560d2f7ab72895a48e76cbecbbe0b5d192ce7 Merge pull request #581 from staebler/collect_e2e_must_gather
a562cbe96990c23afa8232fd6a5bfe51490906c0 store e2e must-gather logs
908f2de22bb4ede4872afde344f134e7d93a66ae Merge pull request #580 from staebler/fix_bootstrap_complete_check
28002238a609a91293a1d3366057f550933b97eb installmanager: fix check for whether bootstrap is complete
f7bf3388352fef43ef952c814d579df1bcbd5bb7 Merge pull request #579 from staebler/deprovision_request_dup
81b3d587e729c8be4c83be800a399ca4b3a44bcf Merge pull request #578 from staebler/dnszone_deletion_warning
72d49e46f6b115cdd8c792e41ec69b5b6abd7e6f Merge pull request #576 from staebler/gather_logs_success_when_no_private_ssh
9e5b55ec2be77dcb1edb773759f4feada919821c Merge pull request #577 from staebler/wait_longer_for_install
9ad718b932ed6d84f1b057de6c2623899cb7a3ab remove unnecessary warning about dnszone not getting deleted
f0d748e6db68069b873165125a6d3eca0eefe5c1 installmanager: additional wait-for install-complete after failed install
1935f24882396ae468f806d6e79a3c72560d3357 Merge pull request #573 from dgoodwin/route53-record-cleanup
d7d727d608f0f6244de286afeff79dd3a9615522 Add support for install retry cleanup of A records in managed DNSZones.
8ec56c103aba24ed216b432fa3d3e592d677d4e2 Merge pull request #568 from wanghaoran1988/pause_syncset
080429930e4299b12e2cd93a49027b8804bbf672 do not emit error on failure creating duplicate deprovision request
7b21d5e0d7bf27ecc8ac8be02280c2168a1cd716 installmanager: fix bug where gather logs is reporting success with empty private ssh key file
6ceafaa407067ed8dd476742bfce2cb9fe9e3b25 Merge pull request #575 from staebler/installconfig_password_leak
dc43217dac98ec677826306a049bf5e37db7f48b Merge pull request #574 from staebler/logextract_namespace
31c45cf5b2cb9dd5fd518a0ab4269ce31dd0bda3 Merge pull request #567 from staebler/e2e_other_platforms
26e707003f9ee060b2f199e8af5a5674f57ba2a2 remove logging of install-config.yaml
be29cabea05aca522ccf6c853361adc1a3ba8b07 Merge pull request #572 from dgoodwin/manage-dns-docs
990437cf1e11e6725356c275d20241ad0ad3162e e2e tests for azure and gcp
120ce0ffdb5725284cc4b9d0dc5473d7945b1ad7 Update docs on using manageDNS with missing steps.
2047b4aa765aed2f25de253e331d099f77fbdbf7 accept a namespace to logextractor
682b121e44bbff0e02f0c43f5aa37e1f6dfb1320 Merge pull request #566 from twiest/hive_dr_backup_backoff
b7e4c4a537ed88ad2a06a940e7454ae6d472cb3e Add rate limiting to Velero backup controller
f19c9ea4d1d67d400e3e3e67f2be563b7be533c0 Add ability to stop sync to target clusters
30a1011410d191c011ebba314c60c1b2ede677b7 Merge pull request #570 from staebler/remove_obsolete_todo
9926c534c39ae28902d23da945bf161aff347d5e remove TODO comment made obsolete by re-renabling golangci-lint
ea29418bf35bb4903759a067516047f7c4d938e3 Merge pull request #569 from dgoodwin/bump-dns-logging
beb334bf3342ec32b7a36f5844a7c8ef33511811 Merge pull request #565 from LalatenduMohanty/golangci-lint_cache_permission_issue
d1277988377e7e06b6ba0b8df1b3351557ac9451 Bump to Info loglevel for DNS resolve checks.
798db4e81ea296135832f631d367243ceb85b9bb Setting a GOCACHE path explictly for golangci-lint to work in CI systems
542aa1bc2650672a3eba59d10114b18402b75272 Merge pull request #561 from staebler/mpp_crash
e4fe2c7f4528ee200a38e661d478e3c7e095bb3c Merge pull request #564 from dgoodwin/create-cluster-cloud-docs
63d31d7176c4267d2c7c1310d3ae103ffb48d43f Add hiveutil create-cluster docs for Azure and GCP.
e499c6ddfa1343b2965e762a5c8e4d79a8271c93 Merge pull request #545 from LalatenduMohanty/CO-436-Add-statusCondition-for-syncset
740a05db1505c872854de3cdcac94c29d380d2aa Adding SyncSetFailureCondition to cluster deployment
528e9947ae4f157472665031c9d914f76b567e9f Merge pull request #563 from staebler/unsupported_platform_error_message
959f8dcae5e23570d945de658456a03d66f0e043 Merge pull request #562 from staebler/machinepool_convert_config_other_platforms
4c5846e564e042bfac3791dca1d1aaebc50849a4 Merge pull request #554 from wanghaoran1988/update_syncset
a3a0caeba1e66709ede5930c4812a23c23d147ee Merge pull request #557 from dgoodwin/additional-e2e-artifacts
17dcebb986b0dd5a71d36cf5133ee0fb5b507657 add missing conversion for non-aws machine pool platforms
4a9292ee0bc16e0410a7b1c7e1d5aca3b4979e7a fix error message for deprovisioning unsupported platform
78ef58cce56e3703c388983cbae1ed269ac899e6 Merge pull request #556 from staebler/gcp
a26916b7b644b504160d64b7df849b7ba1d999fc handle nil worker machine platform in remotemachineset controller
81c4379446346b5f1b5a0c320fcbafcd2f6aab71 Merge pull request #559 from LalatenduMohanty/shortname_syncsetinstance
5fb6b5789df40fec8c4f9d8f37b92bdd5a053182 gcp prov/deprov
3d1f748d2a7241914887a353f73351e2437eb7a1 vendor for gcp destroy
44a10ecc46ff7376b7de70ba5f4fe6a35a82400e Adding shortname for syncsetinstance
1cfc88b6694727c3506be53112fee35d100fa0c1 Merge pull request #546 from dgoodwin/azure-2
ab9361e1d8de3cea34f0e5005052e38713d0746c Grab some additional yaml artifacts after e2e tests.
528cf68af5aab7b4103343471e6eb407c31d2b7e Merge pull request #555 from dgoodwin/disable-golint
b1dc8f0f6f142636bb546cbc7281b186e43a0cc1 Temporarily disable the golangci-lint target due to CI issues.
fc277d8c44bf94fa6f0e26ea1f5fb2a2622a9b11 Support Azure install failure retries.
f037aa47bbede2cfdc631df90d80408ca6059ecd Skip remote machineset reconciliation for Azure for now.
962a5ad568f4a76a05334742664a7f10c76dfe26 Add tests for Azure cluster deployment validation.
f992a53e6dd36dc00ab89cbc3e86c56d96356387 Implement Azure deprovisioning.
4510de33004509a1368c84044957488e9b55d624 remove secret from clusteringress syncset
09d14f313b90a1501e4e42417a33e60f915cb13c Merge pull request #553 from wanghaoran1988/ignore_owner
8e5c0b1dac0b7eece0bdca05bae07c410507b767 ignore ownerreference when using secretReferences in syncset
6b733a93692b3d89d9aa96cda4fa5ff18e34cd81 Merge pull request #550 from wanghaoran1988/secret_to_secretreference
1b689ee94b44238c5806bf092f7c925f29724ac3 Merge pull request #551 from LalatenduMohanty/add_unreachable_controller_check
d4c916a4f69868608116f74618e248af26f3c383 Adding check for unreachable condition
919be0510ac1b1d5e46b9a23ae8b0104d714121d update syncset to use secretRefence
17307155c7a7eab25bc7fbfcbc888c5be1784208 Comment cleanup.
e63bdc631b3211ae4727608baf186d37522e98d1 Refactor some cloud provider create-cluster options.
530e12a2d051a017f3cf135cb9d5c79e3cebe576 Finish plumbing of install for azure
5b93d2b0062018204b53ba1046b69119ca4e68cc Begin adding support for creating Azure clusters with create-cluster.
ce4957f8c3d66924d986186cb0f21fe22d017325 Add Azure and GCP APIs.
d45fd7ab2dd2d2a09b71587c9c7d7fffc0f2e150 Merge pull request #548 from dgoodwin/ssh-priv-key-chmod
f92148518cf81dc9d6f9450f89e4f8398ee2eda6 Merge pull request #549 from abutcher/double-lease-options
f576d40d5a062d1c637e46fe31d9db1134ae497d Installmanager ssh private key permissions fix.
af444538eaf01c57a6fbc2b4e5c8dd9c8fb3e75d Lower lease duration, renew deadline and retry period to double the default value.
8c695295b8ca75aeb79909c6c7b2fd66884804a3 Merge pull request #547 from abutcher/lease-durations
a234b5568b9c4a56f6ff267237e0c6a8eea78f01 Merge pull request #542 from LalatenduMohanty/adding-info-in-dnszone-controller
8a2c57af38a8b7b1a9356eef09b21567cbd5306b Merge pull request #544 from LalatenduMohanty/update-docs-diagnosing-syncset-problems
37678d4577835d63e7215bdddbe183e89cdc0214 Extend default lease duration, renew deadline and retry period for operator and controllers.
9b8cc787b49787d74ae77e4aaa429b9766b3fb71 Merge pull request #535 from staebler/dummy_prov_hot_loop
676da7da582e51f528ec0640ff1f59fb36187242 Updating diagnosing-syncset-problems and adding an exampple of syncset
a13d23aefb1fc933f2b5c7c3a0d3c23aa24bf90d Modifying some debug messages to info in dnszone controller
22b882585142ef562e285b8d429f97c2bf221508 Merge pull request #539 from twiest/hive_dr_hash_ns_object
1e1e60664a2756a2d552c36c90b8c3d9c255003e Change Hive DR to use checkpoint object
29dd13f0ac8ea7d07661ef24260e2f8dc4fbec88 Merge pull request #540 from abutcher/syncset-resource-validation
a1dbceb6e706369db1cf500d55f4cf17186f22d5 Reject authorization.openshift.io SyncSet resources with upstream equivalents.
7776e82850f8803419ecd92d13c7e09c6cc2cc41 Merge pull request #538 from staebler/prov_web_hook_lint
9b8d0cc261ac5ef11a4c3401633b2b66033537ad create dummy clusterprovision for legacy clusterdeployment
7e8117645d68a157eefb09bedc3322f81741a7fb Merge pull request #541 from dgoodwin/dev-notes-update
a3bedb61ef55573b7ca3b36958386c325b499342 Add note on minishift admissions-webhook.
e0bf4ee8781e6af6c52c23d0117b60dc31c63c28 Merge pull request #534 from dgoodwin/revert-dummy-clusterprovisions
b24a8bc34f21ed44c96e4fb4905bffdf347c4a84 fix lint warning in clusterprovision validating web hook
cdcec1258972590124680372c6e550a9453710c4 Merge pull request #536 from wking/installer-bump
446d27c6b11387b46262da8acf36f8b8b6545055 vendor: Bump installer to destroy untagged subnets
10c5df67a1902a218e774d289d1bb2b8489725de Revert "create dummy clusterprovision for legacy clusterdeployment"
3ca12a1c57f83089395845d92d5e2e9aa55799d2 Merge pull request #532 from staebler/set_installed_in_cd_status
0bb3c43f30cfc7d5af20b97ebcbf14ff3e3e8ed4 Set installed field in cd status when cluster installed
b20645de77092a68005ef2779187df173be1d9a2 Merge pull request #533 from staebler/ensure_provision_for_legacy_cd
31f03c7f2a70706f5c8a9df25a918ba31a6bd824 Merge pull request #527 from staebler/provision_job_race
437c7ac9de11a4b47c05ab3660360070bb60f8d9 Merge pull request #491 from abutcher/secret-reference-controller
9bebf85494f901a6b5181510f7820c95548d65f3 create dummy clusterprovision for legacy clusterdeployment
7f7cf48a0abba8f386400ceb89be8041898f2483 Merge pull request #531 from staebler/unowned_dns_zone
55226d21b97a8286290f358cf83c5cb6320d0566 Merge pull request #512 from dgoodwin/manual-rbac
5bfce5ee94a747bec0724881198222dfe89ad412 Merge pull request #526 from staebler/duplicate_cd
4c8e72d579de049065b62bb972cdfbcf415209a8 Merge pull request #528 from LalatenduMohanty/co-539-makefile-change
8873dc74fb0ef941268f268989d4450e0d16a79f Merge pull request #529 from staebler/e2e_install_logs
f76dc1b124fec04cf67a67288272f929daf2b445 Merge pull request #530 from gregsheremeta/selector-sync-idp-docs-typo
e24b470b6aa71b9cf829a03752a4a9306b699e75 Sync (Selector)SyncSet SecretReference secrets.
0dd453fb386f073ee359f52b14ca2b50db962d7d Do not use DNS zone if not owned by clusterdeployment
54b3936e88245db7cb0b853c8404c3a1f98f15d7 docs: fix typo in SelectorSyncIdentityProvider definition
d630a0754175f073d3df2b004c6b323a835fdc9f fix gathering of install logs on e2e teardown
3d0be5f0388cdf7be4310179161b347163f4920d script for duplicating cds for testing
a40cd1fbe929fd915e0ea1e31253174f32b38d8f allow for restoring clusterdeployment and clusterprovision
b70fde1cd50d1d1ebcefc3fa4d8c24f446f4c223 Removing downloading of golangci-lint in Makefile
0f312c99cfb3694b88d3d3251a87167a72e32726 Merge pull request #514 from LalatenduMohanty/co-539
8556a3db4a6f1bea584cb68af76c1cc8aff666b9 Merge pull request #524 from dgoodwin/aws-refactor
fc5bf4220e97cdc7b832089111a90887ab2e995f Merge remote-tracking branch 'up/master' into manual-rbac
6b11d68f6ba236f5929c0b2eb93b860302c61cf2 Adding steps to download golangci-lint in build Dockerfile
a7c3d8700831bfd8aacb5b5ac1e1bd7c7e6ef97e Merge pull request #525 from dgoodwin/providerspec-nil
d1e8b3539c20b181da10338572dba221464bce46 Fix crash on nil remote MachineSet ProviderSpec.
4e2d125072926cbb2bc8252e5bbd75e70778eab6 Use expectations to ensure that clusterProvision controller does not create multiple overlapping install jobs.
a37756ecde782931c8ff95e081be436140e2fa54 Refactor AWS APIs to separate package, remove OpenStack and Libvirt.
711e9d6aebf0df76ab2612ac0aab01d7c72a83db Merge pull request #520 from staebler/remove_syncset_status_from_cd
3ba3b3d2ecbb331f4ba55a136cd95ec1307a2be3 Merge pull request #522 from csrwng/local_e2e
5d99a4bbd07790dd2b8c8b98a750bd75be6f195d Merge pull request #521 from staebler/remove_legacy_deamonset_delete
c119525c8f4a862623b85696b8cd2b3c6f2dac19 Merge pull request #523 from abutcher/using-hive-cp
f9688fa980bb9747aa9d0b5603f9db65325ac7b3 Merge pull request #515 from LalatenduMohanty/better_wording_around_config_mgmt
c1172de84bea7f2d90a242ed518fb4e0d482d701 Update using hive examples for grabbing secrets.
fc9342931f74a160349ab6a3912435885e80b232 Remove SyncSetStatus and SelectorSyncSetStatus from clusterdeployment
3693b4d4a2549971e58ca8868c3652ba1ae6e5ff Improve wording around Hive's config management in docs
6e16087d7a1da931bbe5d7c5ff9fddf40ef5a4cf Merge pull request #519 from staebler/remove_wildcard_ingress_migration
00066c5b7fc998b9200eb353c37b12fe26d33a3c Local e2e example and instructions
a17183ddbdce5bafac2a4d37a14b3eea14e58ef8 remove deletion of legacy hiveadmission daemonset
339584af68296920bee3ab8e4c1a03f99816e34f Merge pull request #518 from staebler/expectations
8006eaa134a620fbd2f11c50f4dd8797858a1099 remove migration of wildcard ingress domains
c759bfa2d208cba05501fc9aa9394ad8301979ec Use expectations to ensure that clusterDeployment controller does not create multiple overlapping clusterprovisions.
31f6f6f2c1d2299b8a40e89d24307d81dd1ec9e7 Merge pull request #516 from dgoodwin/add-ssh-agent
3d39e4ff6b4ef03a7bcad31f412f4efc48ddf09e Add ssh-agent to hive container for log gathering.
10f8b6427807f07a52030b76cf5ead238128b54f Merge pull request #517 from joelddiaz/revendor-installer
610895b08ff4ec0840fbb66510ca67171f53390d vendor updated installer
0c571b0f4eeeb1fe653bc0ec3401b01b2fde0130 Merge pull request #513 from twiest/hive_dr_dnszone
c83ef8878503ce0db9b9365af36a751047113bc2 Merge pull request #482 from staebler/clusterprovision
b7b62176fcdf8ed8d5bf024d2d49e3326e53ff4b Create Velero backup object on dnszone change
c3c8a9024ac56955153012b736621fe692bd9530 fix golangci-lint errors
2689c94252b4272dc7d87a1dde25c14b9492f92b Add initializing stage for clusterprovisions
9745944e1ffe1b97ce8f486bdd71c7f68fc54ba8 fix e2e tests to handle new install job name
fdcf35648a92b18fa303c78c4c4e6e354fdd96d4 add unit tests for clusterprovision controller
7e8493d9c1dd145ee92eaf899df7711bc47df123 make SSHKey field of clusterdeployment required
61219b280478a92f29fd43cfb6d330873628a817 Parse install logs from clusterprovision controller
6488415c0e631cb68fe9259fe11c9f1f8786c719 update clusterdeployment controller to create provisions
f252ef23947286800718e0a52cd0ebfc97148286 use the same hive image for everything
a6fe3ad40c643d468c168e48cc1789cb3eccb2a4 add controller for clusterprovision
9002d7cfe33613de6ef6560054f7aa4856ffedeb add validation for clusterprovision
b608722a7080892c0195e3f15f4e8807e0382659 create clusterprovision type
1580a9ab65d58b5b8eb39e5680a5e720c22dd7a9 Fix Makefile merge error.
e988de248072b07545cb3a441dccddc6b9f078ec Merge remote-tracking branch 'up/master' into manual-rbac
b9bc27f8425ec9b88bb4ad8ebddeb63014092fd8 Merge pull request #510 from LalatenduMohanty/update_golangciyml_Makefile
3d96881bf04dbf3420feacca9b6a0ff76b670a35 Fixing govet issues e.g. impossible condition, tautological condition
c55b20fd5399b9ca4c6b6c809d7eee02cdd763c9 Fixing ineffectual assignment to `err`
e51bc28790c6cc7431ce6a3444892efb9fe75ebf Removing some unused code
e6a4037fb5aaaa43fee3052fd95d8aa1c2d8fa95 Update makefile to run golangci lint bydefault
212eb36631bbe26d22c39d068e99c27803ce1a1c Merge pull request #489 from twiest/hive_dr_syncset
f1343cf28c40ca82cfc49566b71a2d3107a3ee6a Manually manage controller RBAC.
6a2821a4d1d3fcc6ce739773ccdfa23f308649e5 Create Velero backup object on syncset change
b21b7ccdedb0b658462084ecd45ba257ab7d25d6 Merge pull request #511 from LalatenduMohanty/TestMergePullSecrets_enhancement
5dff0aabf433a4029c9077f961104a28dd86a4b4 unit test improvments for TestMergePullSecrets
54a7584ed26dedbca19df3e08e4f833ef49c8341 Merge pull request #490 from LalatenduMohanty/load-secret-data-global-pull-secret
cf7d97cdc684b6d58304fe9e17dc6a8b00f93ed7 Modifying code to use constants.HiveNamespace
036fb9d8c402a1477e9100e8c5fbb3a3e92f7134 Global pull secret should get updated when it is changed in hive config
d34ae54f9e92454cc05a5b19ea4d622ea110f9d5 Merge pull request #504 from csrwng/cluster_operator_status
4303c9d14852b15cf0d79444db438de95c9b742b Report target clusteroperator status
b3cd763dbd2e4cd2d49cc412b2f2616d112dfe53 Merge pull request #496 from LalatenduMohanty/make_docs_easier_for_onboarding
7c4f73236f0bb70ec2dabbce505e484bae926df6 Merge pull request #509 from staebler/logging_event_handler
27909bd9d3b233a2750471965cdd95147ab8c9fb Adding quick start documentation
82bebefcdf80aa22952079307dd9ca18f8e42404 wrapping around event handler that adds logging
ce8e5cdafe18c1144f4a87c9a5cc3421275f12d1 Merge pull request #508 from staebler/bad_info_formatting
bac30a0eac37323b93576492056706916005df00 Use Infof instead of Info when formatting needed
10915d60aad9e26128b942f8bcae9bca06450795 Merge pull request #507 from staebler/syncset_admission_operator_role
52bec168490c31febd0f8619a085e2faa26be9e2 Fix typo in operator role for syncset admission controller
f3b91891e20eb49509dc6a3406aeaeaddaa45521 Merge pull request #506 from maorfr/hive-frontend-events-create
8fe461d7d727b88758e6dcd77006aa0ef97a9b7a add change to bindata
17f9f12026b3e01821f18bf31796d61be398e91c hive-frontend add events to role
1f82af0b7f37305a7b82c4ac21be169f3031f2a4 Merge pull request #505 from csrwng/fix_cert_location
e3dfe2a4d010ee555b8fc661c37a36c1aba26601 cert util: change copied cert from cert.pem to fullchain.pem
aa4247acf827a778a2e3dbf21d9d4d67f36ce846 Merge pull request #503 from csrwng/api_cert_reload
d9ad823bc47507a4d1f1cd5ad9484197f6fee1fb Force reloading of APIServer on certs change
f7a269279621b8fda64185ad2adfbad2c5b05362 Merge pull request #501 from csrwng/cert_util
4d092519a6a5e21ab0ef4eb7f5180a2d82b96739 Certificate utility for Hive clusters
1b9198c5fdb26abc3738832cd370fb449fc34973 Add serving cert option to create-cluster command
2c87056591fa79aff930b1d174f3ab121720ad70 Merge pull request #502 from jmelis/fix-numeric-prerelease
60891934118e82d15f05ef6ad6b2b2a041626619 semver complains if the PATCH first char is a 0
f8949e88f62aa78167fbd03b59d4a98404fee2f5 Merge pull request #497 from LalatenduMohanty/golangci-lint-misspell
9a9cf96430609c2badc02d3f2939918c39ed6c60 Merge pull request #499 from dgoodwin/logextractor
7a0b677d8292ad2d4e1450389da8916802a79975 Add script to extract cluster logs from PVC after failures.
e4c4e0c30e0e034ba70554e6299aca49d57babed Merge pull request #500 from LalatenduMohanty/run_generate_bydefault
4fff1695cb209df6fb95ce38cf7f6bcb0e27a433 Run generate bydefult before verify
734a039fce74192d10fb436d9581fd9f95dca7d4 Fixing spelling mistakes as part for golangci lint fixes
b5fee1617ff7573bfd4cf5db93ea60c4ea7d1cf8 Merge pull request #498 from LalatenduMohanty/golangci-lint-varcheck
9e09fc5332cbad4a33cd062ebc56b4a7b72d89b2 Fixing deadcode as per golangci lint issues
2eb2bdc12e4a0fa282689d1ae2d1439fc743b489 Merge pull request #494 from LalatenduMohanty/fix_hiveutil_for_globalpullsecret
1bba1380f13e41fa5e83a5a4c1bb396ece366e56 Making pull secret file and environment variable optional for hiveutil
01522952fc85baa055991a94fbea8889cf84c862 Merge pull request #495 from joelddiaz/set-invoker
60311264f45edbd06afebc4d2c447cc2a439e5ad set OPENSHIFT_INSTALL_INVOKER when launching install
7bb975b14faac4325871c977244933752679e99a Merge pull request #493 from dgoodwin/temp-cli-image-fix
b87d2f0c0493cbd63ca3264443fe373fc3c256f3 Use latest hive image for processing image resolution job.
8b95429d0ce65f7cc9a339f3a8faf7c00b3e8ebc Merge pull request #492 from abutcher/syncsetinstance-hotloop
ecfcf189d0c54e388dd962d96bbe20f9b4a028ad Temporary syncsetinstance hot loop fix.
3f238dcf2321f6670aed13ace466b3cd2061af3e Merge pull request #479 from dgoodwin/logs-pvc
705db11ff2d9d20594f737ff281b76e0e36c39eb Review cleanup.
8fe059e5ea49869f7e7100800fda99bf372dad66 Merge pull request #488 from dgoodwin/fix-time-to-install
67fdbfb10923dad7ac976731e89539d9d9ebadca Fix long delays to install after generating global pull secret.
86f42acd2c77986c76fd5e2b70d2e4af952819a6 Test fixes.
6b6918e7726942154a68b32fa4e66f5b9f3fba12 Track installed time for PVC cleanup instead of job completion.
0642f70dab85f43d4a6a676d5457df5ac4a3cc71 Separate creation of PVC from creation of install job.
1c4e46adb40fa038e3ce81e4abb888b70b83c0df Switch to gathering logs by default.
c3a63d227b4e1c5b1a4132a1b9b980346e847aa3 Run oc adm must gather if bootstrap gather fails.
bb3214bfeeb181695110b1a29a59ecf1b5983fec Resolve and mount CLI image to copy oc binary into hive container.
329c9ffb1e1fefe28cd502859d7705f88fb39a28 Gather logs from failed cluster bootstrapping.
eb66fa8568b3feb9e9745eb85b37dd73fb7cf0ac Merge pull request #487 from LalatenduMohanty/remote_ingress_logging
744c83fd46de953e4ec9c090959b886e23515700 Merge pull request #484 from twiest/add_hive_config_option
ee53f5b384be5dc669ad27da9f76d9f2eb5017a5 Changing retry log to warning for ingress certficate bundle
43ad997f5dce2c712f358a30e1bc7a31487981f5 Add velero backup option to HiveConfig
7a0184c498dbbaf8063382b9a5b7a1dfae05131c Merge pull request #485 from jmelis/global-pull-secrets-template
86730cbb94fbb6879f149b2a2247d12c1b912dae always define globalPullSecret, but defaults to empty
8ce45336fa764f36dc6be065c0a27051a94e1e0e Add templated globalPullSecrets
8a6f0ba3351d03d85ed30bf27aa286adb487efd6 Merge pull request #486 from dgoodwin/empty-global-pull
973fc1752efae62f827ace884d0ef4b6913ed4f1 Support empty global pull secret instead of absent.
17eb27cdf72509b62179151a5f8938557daa5c55 Merge pull request #480 from twiest/add_backup_on_cd_change
045d38e4cacdc5cdb11cc5fa3d02f650ddb63c30 Add Velero Backup When ClusterDeployment Changes
7efbbc89e0b6d9bf2e6b6730c9ee66f91e5ca2be Merge pull request #483 from LalatenduMohanty/global_pull_secret_docs
3140f0d49aeb6baabf86c67992dc093657d6d07c Adding documentation for global pull secret
ca3100ecafb880a8d3fd8daafbc90b038b5c545e Merge pull request #467 from LalatenduMohanty/global_pull_secret
2b5c9d0df535908f315b756526f112a15c5e1f05 Adding GlobalPullSecret to Hive config
7fe3b1f889ca5384fb476dd30624ff81326143bf Merge pull request #473 from abutcher/syncset-secrets-sync
f20c40f9ef7586b99571c03ecb5b8917f5cdfdf4 Add SecretReferences to (Selector)SyncSet CRD.
ab760d01ff552163c1feab6ce3c2570399a15710 Merge pull request #481 from LalatenduMohanty/doc-updates-1
fb998b192deeea6260d75e3e1a09bb66147a69b0 Added steps to enable debug and more small enhancements
f9210f5fe8c2b2084f1f92bfd4d29677f47aaf76 Merge pull request #478 from staebler/deprovision_service_account
d04fbcadd0d22ea093c25e920c557177998aeb09 controller: do not create service account for deprovision
9514c58afcfc4ca992e1e81c201d1461e4a133cf Merge pull request #476 from dgoodwin/deprov-install-finalizer
5a0ebb4c259e4c02c53477abcfabced7f517f846 Log waiting for install job deletion and remove unnecessary nil check.
642daace03fb5a0c3253476562a5661798b19116 Merge pull request #475 from dgoodwin/wait-timeout-log-parse
cc2fbefb618b5e9772e213c4a1b312597532b751 Add an installlog entry for the standard API timeout.
3d7aa6ecedab74cdbb987a11be66bbe175fe6240 Merge pull request #474 from dgoodwin/leader-election
5889b7c0fd26dcf7c374385dcbfdad6d1d71a945 Add leader election for both operator and controllers.
54a0048bce721dc1a094ba7d318f86038d03e80d Merge pull request #472 from dgoodwin/ssi-metrics
1d5144382d26ec8b5dbad5d3be543a0145a304a2 Add missing metrics for syncsetinstance controller.
bc0bbc2f7a4fdc782d2d95e3d4061f4367414dcf Merge pull request #470 from csrwng/vendor_installer
d1baf7b937928be18c28fc7f3e743f5f17e5fa3f Vendor latest installer
f208825987c17a8ac89b3b133f6b20c698697ccc Merge pull request #471 from csrwng/move_to_golang_12
40eab92225b38433948f6739229a3c32e77a1c55 Switch to golang 1.12
9163d9155b0ff1822c2ed2e63977aec695870c17 Merge pull request #465 from dgoodwin/regen-deprovision-jobs
5c161da2d0dc959922c98e4aa491b7954b42fccf Regenerate deprovision jobs when spec changes.
4a24a9de7186af502ed9424381fd1c2b0fef07a6 Merge pull request #469 from LalatenduMohanty/improve-code-readability-1
b11b3d9a6c38d63caa96398083b7aa7851623609 Simplifying a conditional loop in cluster deployment controller
559edac066f8a1f64135db6cbe892243e2004adf Merge pull request #461 from dgoodwin/docs
47619cade4785806f3a1d1c194c861fc2a669e58 Documentation update.
1a97507b29dc3c9ca6efae91af8cfd0822c73127 Merge pull request #460 from LalatenduMohanty/ineffassign_linting_errors
05eae9d62594a573688f36fee97434b1ba92eedb Merge pull request #455 from LalatenduMohanty/golangci-lint
7a2f0867b3457a868c74ce1a08c096b9edebb787 Merge pull request #463 from abutcher/install-failures
cdcb5a5c5e5c448d7c28cbcca8c507d622b33945 Merge pull request #466 from jewzaam/hive-admin-selectorsyncidentityproviders
d75fd7481f69b15fc82348e0813af601a8a16747 ClusterRole hive-admin can edit selectorsyncidentityproviders CRs
c60bf61e93f8548c3c145fc63061bcd4787e0248 Merge pull request #464 from twiest/vendor_velero
349cb12ee8c79fa5adb428e297fc8ace9aa71f71 Merge pull request #462 from dgoodwin/remove-legacy-install-config-gen
4cdd76a5c59c18837f949410f016f2cddfd7a139 Fixing ineffectual assignment to errors
640eeb505263d2b64223b52da399b7a60ef91aa6 Vendor Heptio Velero
fcbbbd1c4c769121069957be396c17cce6fbced0 Add regex for no matching route53 zone found.
9fa424a4b87e35f1cf1770fd078b563ac7ad531e Remove legacy controller gen of install config.
dcbe1ea75af33e3cbd84b97ac18d0d538039bd2c Merge pull request #457 from csrwng/e2e_create_cluster
7d27e40f40facb14d460533ffc56056d77c00944 add debug output
497fb8a8b35e59d86caef453ec054952f8b33b6f Merge pull request #459 from csrwng/remove_timeout
00da62c657e71930f6b396ec001b8c60f9ab2890 Adding golangci-lint to Makefile
066ea48740464e978b3116ad84fb6b15f0243533 Merge pull request #458 from csrwng/fix_make_deploy
edd0453fd44cf0daf18997c5c7de58dca2daf3d4 Use hiveutil create-cluster in e2e test
106555010b35a1847384cf9473d1da54cbe550af Merge pull request #456 from LalatenduMohanty/lint-fixes
cf3b359c5de65dab6e084590c88ff1792704483f Remove e2e test timeout
df65494b41d9537fcd0973599c6c3baf036967d9 Use kubedeploy edit to set image in make deploy
d291096f0862c54ed299522c10f328eba2a6fd0c Removing deadcode from controllers
cf0074db6760503e24183dc9d31e99326b08f24c Merge pull request #454 from csrwng/e2e_postinstall
91a2f88e9b86076ea340ba45b5d1b21df697780c Merge pull request #452 from csrwng/admission_debug_permissions
1e830b557f8129d13cc3fcd66cb3e376236cd5e9 Merge pull request #453 from csrwng/fix_machine_pool_validation
9dae6a5ebc0863daa67075fa1e3acf3c02e9d301 End to end Hive post-install tests
dfdecf386f1e086f7757b9f5a45d3bffbd50b84a Add permissions to allow debug of admission
8fa0ab677413d38cd2ebd92757287c06f7f2a036 Fix validation check on machine pool mutation
0a350e47ec5af913a9d7e2aadeff299be24a7010 Merge pull request #451 from LalatenduMohanty/CO-458
abe52136c1805f7f7b19078f7abba69888c62e8b Merge pull request #445 from dgoodwin/remote-client-metrics
6281faea66a8de3c99e29d367cd0c23dd80a1c7a Preserve RestConfig WrapTransport if already set.
6c3f75c1e9b04ee70e67831a6d1cb203c6f84c64 Merge pull request #450 from LalatenduMohanty/make_logging_cd_consistent
0646257aea6af5d9989d462f26a86beddf6d00d9 CO-458 Stop Deploying openshift-v4.0-latest in Hive operator
3ec5472f503224dd371330e38701adfd1c1b8ee5 Make logging from CD consistent with other controllers
22783915bd2c79e1b33c2169c1921b55444a9117 Merge pull request #449 from LalatenduMohanty/intro-hive-readme
224fd5494d9960916f9caaaa6bc865e1520eb27d Expanding the introduction and adding a FAQ doc
5646f702f8328b9d259660215e457ba53bf7fc6a Include status in kube client metrics.
7c3812ec114b947de4c94902d2c28114d4d000b4 Track metrics in the resource apply clients.
276945eb7b27b96f121e5de5c8eb38f67998b45f Add kube client metrics for remote requests.
d01c18edcbdccfa730f3d869cfe3d62d54724a5b Merge pull request #437 from csrwng/syncset_instance_2
ab3d2ce266977fcad20ae70e549e93ffe27fcf16 Merge pull request #448 from LalatenduMohanty/making-code-readable
fd54a3ad909f327b59bda87e6da9b63a726cba94 Trivial changes to make code more readable
70c7ae2e6e52ef493d6b6a487ca1d8c1aac6f927 SyncSetInstance API and controller
cd6547ca9b4e150e0996893a42b26cc4da5b156b Merge pull request #447 from dgoodwin/remove-logging
a675ea15dd4d9a083cf483c6a005ea02febecae2 Drop hiveadmission logging even lower to avoid one line per request.
b010f67541c9d755c0573f87a42ebc58ee17eec5 Merge pull request #446 from dgoodwin/reconcile-time-metrics
628a1f8f6eb782c22925be6820ccde1babe09a2f Reduce metrics and resource apply logging.
7ad3042f035a4fa9f73d22d109405aeba0ee506b Add controller reconcile time metrics for all controllers.
000d858552b3da0fe4406fb316f51656bc0da3ae Merge pull request #444 from csrwng/syncset_remove_dups
0f6489056fca27cf5875ff797f014b02f044fe8b Merge pull request #442 from LalatenduMohanty/co-455
352e876cd47d89250e853f93b4e2717f63279f0f Remove duplicate syncset status entries
8600bf0fe451758676da466ae144508f8ef7d8d3 Merge pull request #443 from LalatenduMohanty/owners
5ff9afa05a823454278bc3c03f48ec1f206a8ab1 CO-455 Send install job duration metric only for the first time install
cbd70aa1b336038f23b24aa2ffb47fd00517e6dc Adding LalatenduMohanty to owners
17f1c04535e836273a19b5bd55c7909d3c088fbd Merge pull request #435 from abutcher/delete-forbidden
7d5c1776c15dd5fa9d61d4337c23acea7c4bdb4c Add test for selectorsyncset.
32e144f5cd8bbe72baa0705a2569277b74ca9412 Update SelectorSyncSetStatus for SelectorSyncSets.
047895a0268ba33a974cdf376de8bbcd40726edd Merge pull request #436 from joelddiaz/dns-condition
4cd65924d378f7ecd7394ea1049e298d1ae4d23f Merge pull request #434 from dgoodwin/hive-frontend-mgmt
2779f5d76ba332e3211ea9ef37a8f259c3ad9bf6 Merge pull request #441 from csrwng/revert_dnszonedelete
a1b0d7ca1c0a35f775e09891ca12d6c01c546c70 Merge pull request #432 from abutcher/copyright-update
b129bbe30216d40d9cac35353cb7ddefbf5a4f71 Merge pull request #439 from csrwng/revert_fixup
59c539a9411b6313e56fe1df8f2d3fe5156b6c0b Allow cluster deprovision to proceed even if dnszone has not gone away
aee489928ecbc8917da58401e402004bde943aff Revert ClusterDeployment fixup on clusterdeployment controller
7a4e9b3306610489b926a20a11244bb210342646 Take control of hive-frontend role and service account.
943856344df6ef6a2f09a1443afc4f7f8c8d75df add metric to track how long dns takes to become ready
dd56955208676cc79a41846578ac05f406bf0fb1 set condition when waiting on dns resolution
5039173a588462805a06ecd072e821a2ef77a0b1 Merge pull request #438 from dgoodwin/skip-unreachables
4183272f3deefdeb9289ce9528edfc5b8a38e224 Skip reconciles for unreachable clusters.
84b5b61deb80750912f8688007274e093d01768e Merge pull request #433 from dgoodwin/less-logging
1b48df22051aa7bd23f75effe65d8a206e4bceb0 Ignore resource deletion forbidden when cleaning up syncset resources.
523703a43793ed412ee6c3457f634ffe49510eb4 Merge pull request #427 from csrwng/handle_deleted
7bc3f59b308a2bc586691a908f6f4f2f32d3cf16 Merge pull request #422 from csrwng/cleanup_dnsrecords
2bee85a34820ad378b4be6b1a3277be9199f4750 Merge pull request #430 from dgoodwin/client-metrics
ee9c9ff4f4ff8bb33ec7602ce604f51e362d2abf Drop hive log level to info until we resolve hotloop.
f0885df65e9ba1d4ca8236383dc501571c03b44f Cleanup log levels in cluster deployment controller.
ec4d1479e5dd9ce316ef7e0f0fd7f848c39f45a6 Wrap controller clients with metrics tracking.
cd8cccf260a149bb08ebe7cd01ed0b89d8ac8876 Drop operator log level to info.
a84c4bce722b489e08a22f1ceafe45c51ebaa105 Drop hiveadmission loglevel to 3.
e79ccc71be1b28df54a7c2ea17536e99ad01f08f Merge pull request #431 from dgoodwin/skip-configmap-reconcile
c087cadf11804ca62989d42d5da65da1b238e853 Update LICENSE and remove copyright headers from existing files.
94587315b47a48b38e215d7a0bf04e032e23740a Merge pull request #428 from dgoodwin/hiveutil-delete-after
12b959ce4a986f93407d00398500333383db5643 Reduce configmap reconcile rate and logging.
cb8474845e51531d7c837020f58045237caf3e43 Merge pull request #429 from joelddiaz/ssh-image
13ff64e3e0276bcb9f693f60952bf96fb0fadc90 add new custom base image
5c2a115f13849e1572792c44ad7d4119f2fa50a6 Add hiveutil create-cluster --delete-after.
b0276c7d7f374c767a68ff465545998f659a3731 Update clusterdeployment controller to handle deleted resources
eb30980511fee953ade14bb889979edee5c11f3d Merge pull request #423 from joelddiaz/remove-install-cli-param
8e113e236c5e0e6407b72c2af9187ce5227cc870 Merge pull request #425 from dgoodwin/stale-metrics
2258b9f60420cb5d9a7112ee5e91976f47bf427b remove recent command line params for passing private ssh info
7ed638e4f10a8224b3af2524db59d1a426976f50 Attempt at fixing stale deprovision underway metrics.
245a1b26a9eb78ea48b86525794ed245329b421f Merge pull request #420 from LalatenduMohanty/move-installmanager
274de0e0396ca2bc3a8be55d5de6d46a3cec0eae Merge pull request #424 from LalatenduMohanty/unreachable-hotloop
5449df3c40949152e5ac7061229b41e79ae55597 Don't update cd when unreachable cond is absent in reachable cluster
1634202cae560955743c4aa121ad5c8296512d0c CO-447 Move contrib/pkg/installmanager/ to pkg/installmanager
96009f831787220c55a71c374d6e7df5fb0e229e Merge pull request #421 from dgoodwin/install-manager-logging
0c837c021550146eb1ad1fa00fc746a23258a5ed Merge pull request #418 from abutcher/syncset-cleanup-sync
885e77a3c058276bfc27eb550bbe000089b6cd61 Small log fixes.
7dbcb7f4d87fccc2fa42cd7083e5ae5202cc6442 Cleanup NS records created for managed domains
b9777eab9f3b0d66489833fdf4470c21dac49a17 Cleanup deleted syncset resources
433c5f072a05255c7a13228bb5d9e8b1d38bace8 Copy installer binary to a temp file and rename.
2cb7de6dce8d927454c802d0df3bd1da1902080d Mockgen changes again due to someone with outdated binary.
30331d84d1bbbcced9b0295aed191c3d0d2785f4 Additional logging in the install manager.
6627ec3d82826a5e6031448a1ec79d1741cfdfa5 Merge pull request #419 from LalatenduMohanty/fix-without-Loader-warning
2cae61e7771d814b226aa1b5d1aab0ba1c3fa7b3 Fix the YAMLLoadWarning in generate-operator-bundle.py
102cff180ea836e30ecd919455a3884eab092bdb Merge pull request #414 from csrwng/e2e_postdeploy
9984745a1e1f9c6b716250283d7c447b79d11c8f Merge pull request #417 from joelddiaz/hash-jobs
0952493d95c2681b0d358e8a5fc0cccc0782ca55 address PR feedback
fd989e5eeab60da260c4bfadc54225b37a916d15 Post-Deploy e2e tests
dfa4a9563432402aeb0e7432793aa1ad65138a4c WIP: save job spec hashes for install jobs
72b1ee5606b7270d5ae6e5ed1fcf7bc8b8078b56 Merge pull request #416 from dgoodwin/installlogmonitor-2
4cb9a70f3b002aa51bf9eb7e9e492418a4258ec6 Merge pull request #415 from dgoodwin/ssh-opt-fix
f89111afd625675d41b1c8e31de209c567d1ebe0 Write sleep seconds file when we fail to generate assets.
d16d059529c71f3d177daa07a18f67a45730d988 Fix broken installs with older ClusterImageSets.
68d0c3607c542090b78478139aa39308d646b16a Merge pull request #410 from joelddiaz/tarball-save
b18b25b6bf03b88482181dade2d91f0c27e1289b initial pieces for gather log on failure
93e6d0041fc3d0648275e4643754d3e3de099f8f allow defining optional private key
444e8403ee69ef38b77eda31638adf9ad7303970 Merge pull request #413 from csrwng/name_length
5957da60141c56a8ea15be43399351b34df7f669 Validate cluster deployment name
6956047fcf642b710c46a3fa416f0738c3aefb05 Merge pull request #412 from dgoodwin/error-reporting
4ac42736888f65ed8205d1dd9d178a0804f6f87c Remove incorrect copyright headers.
1b9a23d12565b574018245faf7fc1006112376b8 Merge pull request #411 from dgoodwin/makefile-oc
9319edf9c4f5baea7edc562626828b7e9ed37e32 Use owner ref to better resolve cluster name.
f67814af3683bc7822367f1f9032459fcfc880bf Use oc instead of kubectl.
8e0a22d5527880916fc217a0a15c398ed61e1d16 Monitor install logs for errors.
1d85899ceceff61004efab367e6142edcc6cfabb Merge pull request #394 from LalatenduMohanty/unreachable-controller
ad0d79f2ed4488abb90a065d6f8205942c5da249 Merge pull request #409 from dgoodwin/cdrc-reconcile-time
cb228d3d2c02f707a7a5b7beecf859728da8db6a Adding unreachable controller
2e41f621c0e5aa9f11f9399d9eaa36398e9ac15f Add logging for reconcile time in the cluster deprovisioning request controller.
8a788f2ae40b854ef7aa453225215bc2c677c83b Merge pull request #408 from dgoodwin/log-new-install-jobs
f05190e5cc0591b696870a095632fb7379ed58d2 Add logging when we delete an install job due to generation change.
0d58f1f401d804c7bd6820c68b226abc343b0b4a Merge pull request #407 from csrwng/generated_names
c614b7fa6ba4ec2bb5cc87759a3faf0d9e52cc6e Merge pull request #402 from csrwng/release_image_precedence
8d85bc97d6a66b5745e9fa5e591802e5ee3b07b7 Use release image from clusterdeployment when present
70551c731a16b48ea6fc2fa5c820e0773f695dfd Merge pull request #390 from twiest/master_team_ctrl_tools
3dd5afcde924103cd2208a01390da72da532e226 Handle long clusterdeployment names
d3226281484b35a6e3526307ce581f5f7b4bfed1 Merge pull request #406 from jmelis/migrate-to-ci-int
364fac06785305cd9256f1f951bfd4472f87048c migrate saas-hive to ci-int instance
893a6c9765399ebe21992142b670bfed297e9643 Merge pull request #403 from joelddiaz/ingress-validation
917056d5f918c050758c59e6736f078e0eb10cfb more validation
bf9ca58fe434dd3ec5b159554918f21e146ac8f4 Merge pull request #404 from dgoodwin/cleanup-dns-bug
e0301a7a1aa835df1e0f275f9e54cb3b7307d83f Fix leaking resources on install retries.
76a964f7575e70d70ac5ce87163ef334185cd2b6 Merge pull request #401 from dgoodwin/dnszone-deletion
eddd8d8f3285f3a3103de09a61dcfa66be739515 wildcard ingress migration and webhook validation
8f888e169c1d5d4ef4f56d3e49b58e45b8d36fc4 Fix up Hive to work with Kubernetes 1.13.4.
0873cde8883904b2466f36154689dc923a235e13 Change controller-tools from twiest fork to OpenShift Master team's fork.
511d0179428ae9bae75c103cb05e15386a2fe24f Merge pull request #396 from csrwng/generated_kubeconfig
d6bef9e223f8732bbf4674fdd18c29296daafae7 Ensure managed DNSZones are deleted.
69d29cb46d4e45368d79f202867d29c1a89f1c4c Merge pull request #400 from csrwng/update_createcluster_defaults
eadc5486a66d1f9e9c153be667d6380b1fc2282c Update README and hiveutil create-cluster defaults
a6f79d8b4e8ac8708e9590f7bb41c13eefbf45ab Generate kubeconfig secret with additional CAs
429c0540809c4fbf0754d9fd3a365374ffcd949d Merge pull request #398 from dgoodwin/dnszone-hotloop
19e28401e47a67319ddd21dcde317b42cffc2d99 Merge pull request #399 from jmelis/fix-parameter-cert
2bcccaf535fef4c162e9979165d5e9738fdd94c0 Merge pull request #392 from dgoodwin/retry-sleep
9306007a494e1a1dac985f27cb05d270a9cf1058 missing parameter added to template
66c321bbdf88651f0a63d9b9ad779af5265d1c4e Merge pull request #397 from dgoodwin/readme-create-cluster
27bf8fbb8bf63feaecf85f294bb55f8bc552142c Cleanup stuck DNSZones in terminated namespaces.
943fd249438499c5d056b3febed0dd811f26a6f5 Fix DNSZone controller hotloop when waiting for availability.
1cc985be99c353234d0bd48ea64276ca424753a8 Change README to use create-cluster instead of template.
fdf2768cf297fd93ceb8e20d388f666d98acc8e0 Merge pull request #395 from mwoodson/master
4c56a9eed7ba7feb6c902eb6bab699ec83478a81 added the additionalCertificateAuth to the hive-config to be deployed
9831c5a6106b64ff7ea6ab96d4e017dfabd01081 Delay install retries with sleep.
272f6c4fa347704fb7fe6229f64747df3fd83286 Merge pull request #388 from csrwng/master_cert_fix
eaa4f75a4bc467931d4a28b8e869e178619591ea Merge pull request #393 from csrwng/additional_ca
4745ad095a23765fa6dc060c1081690a36aaa170 Allow configuring additional certificate authorities for a Hive instance
70f04bcb40d611f8ed94c0f19f71023d3608bed0 Merge pull request #391 from dgoodwin/drop-rc.0
785c1cb85208fd3441e70c3803530c2b25c57512 Drop outdated and broken ClusterImageSets.
7e0dbf98f78dcb29bfe4751861169a71f3e12219 Merge pull request #389 from csrwng/ingress_cert_fix
855a8edc1b0ddd20d98ea2549d0578eea7ab600c Remote ingress - include toleration to ensure ingresscontroller reload
6bb6735547ffe8dc988dd31c0e1d99e21e5170bd Control plane certs - use additionalCertificates field
01ef7e20f396537a6eb670defadff2768251f47f Merge pull request #387 from dgoodwin/reports-2
2342f033ce2b8f695ac3997856f938a03005dec8 Merge pull request #386 from jmelis/add-hiveconfig
07d084afb85b009d02c421f2e1c11e7ae27bb622 Merge pull request #385 from dgoodwin/operator-apply-crds
8d01f3ff9fd252c244a3dd63c8a067ad781b006c Add provisioning/deprovisioning report commands.
da72b8b394c74b42423d9b2e85800c5c1128b8ec parametrize rest of values
b81110f14870c154068d56b3b548e3a15533ac8d Adds HiveConfig to saasherder template
07661fc82e59dce6cf291beee853b4b63a3859c5 Deploy CRDs in the hive-operator.
ba50e367dc5e933eaae697f04137780f8137c172 Merge pull request #384 from csrwng/optional_nameserver
681886eff65c6e31084d89f2b1a73d6c37ebad9f Merge pull request #383 from csrwng/release_image_src
dafe3ce8afdb7e8d0d2a13c760abb051cdcc5aed Optional DNS server for DNSZone checks
0fbbb931118b8c0991f289390a0c1569045e98d5 Add release image source to create-cluster
2ee97e3dd6b9de1f22b0ea4322eb56ed7f228557 Merge pull request #380 from csrwng/remove_state_field
811927c8af2fe79fa8caabee18af625fd2288994 Merge pull request #381 from csrwng/fix_create_cluster
2cd528c460d80c5de0a8213bb3f78fd23b5c1473 Merge pull request #378 from dgoodwin/metrics-work
9399b4cdf49fa4cb216fc668af4b99fdd2db60cc Fix cluster secrets in create-cluster command
5753882c16b34a6678863f70487dc8691bcfbbdf Remove spec.state field in clusterdeployment
777af551de8b787443bd23687136f4b72ca6e62e Fix missed delete cluster metrics.
a5d26569cd32b3cd3b2556f8555b5dfa2e041070 Merge pull request #376 from dgoodwin/deprov-fixes
ba3e6cf803cb2d970e70d2acf07583bb61d442c8 Detect namespaces deleted before uninstall job completes and give up.
a87d88db1d1b90d68743272156e5cbe1bd1ce2c4 Merge pull request #377 from LalatenduMohanty/add_timeouterror_for_unreachable_cluster
49046e3c55bf72d5218d6609d3f6d5725addce22 Adding error to log for unreachable cluster in machineset controller
efdc04ed13ad00b98371dc592e053aeab1feaff1 Merge pull request #375 from csrwng/deprovision_phase2
5ef1a1ad22d337c1e4de07d8af81e1adc2c10b89 Cluster deprovision request - phase 2
7dcd15f65f3d78850fc5c716d853e187d25ea196 Merge pull request #373 from dgoodwin/cluster-counters
20260ff21ff7a3bd1502ab2fda605c8588f319d9 Test fix.
262900286f08e70e1d288a2b191caf227021eb84 Add cluster type to more relevant metrics.
7fa9b0d2081d2f650a871311498c9f6c1cbaa977 Add counter metrics for cluster create/delete events.
34a8cce2c3df3e8a6de36e73a577342bc02d43cb Merge pull request #371 from dgoodwin/report
a9101479123eb46de19248a551c23cf840473879 Merge pull request #374 from dgoodwin/underway-metrics
2fb72cbb4e809ea2e0fc399769b60bc884848c28 Add provisioning underway seconds metrics.
c6a31d5f821de177aa0bbadb9595183b16c75f43 Merge pull request #372 from LalatenduMohanty/ci-git-issue
d28a43ee53c90545e02bea9e7d1a3bd9dd5e28ff Workaround for fixing jenkins git issue https://github.com/jenkinsci/docker/issues/519
3216c0676f35926d2286d78467945cc6ba1f505c Add a hiveutil report command for gather info on failed installs.
785ab700299ab33aa6796be403e37f447ab8858d Merge pull request #367 from dgoodwin/jobsort-fix
65408e23b5cc5287beb3bc3abe6a2360b14f5a49 Merge pull request #370 from csrwng/migrate_patch_type
d108bb4b1a4a104cac8e3fb7adf7448609ad2856 Merge pull request #368 from csrwng/syncset_validation
e5aac2d59be3b3a3fedec74a00f8de88764ac618 Merge pull request #369 from csrwng/deprovision_request_fixes
5803d9ac6a6dc76cbd91443c6dddb8973a8f55f8 Add test for syncsets with no patches
f961d163eb3c99cc869afe5564817a88eb90ff4e Migrate patch type for SyncSets with patches
b4c85ec9bfb6a8b593c4cfc33c4f3ac823b70a23 Fix manager role for clusterdeprovisionrequests and create service account on demand
68dccd21348cfe02bcff7139a8f7ad3f562be354 Validate SyncSet PatchType
7d4e2bd0ef9ac8c130583b7ab24a172d06902be1 Fix failed jobs showing as running in metrics.
d574e8cbaed4db3501a1f259c6799a459484734d Merge pull request #366 from abutcher/patch-string
152d9b686142e87d7bd86711da6a9f368857c139 Update patch types in integration tests.
7ac31f3039812c5c4d1ca120d9c816e80209ddb6 Test if patch string is valid.
47083c5aa804349ca8ee82fbcfa00b7a92bf28b0 Merge pull request #365 from dgoodwin/terminating-bug
aa29ae500ae1ab45dde685baccab2dc56797dff3 Use short patch strings in syncset patch definition.
5ac28455f1b3e1105d0cf8bb064b17ce94eda34f Fix PreserveOnDelete clusters rapidly deleted after creation.
6cf6092927ee0c46f7be48e3536a116b66b1ac5c Merge pull request #364 from csrwng/deprovision_request
ecdc07514d363bf50f9f6799f92ce49a531d0e03 Review fixes
4e6cb9e9986631a4c005e2580ce614fcf74af4ee Add ClusterDeprovisionRequest CRD and controller
7dd0e038ca026d3069d06556de1cf636b97c1c64 Merge pull request #363 from jmelis/hive-admin-selectorsyncsets
0419f54d4a0257d2bf2a66e4a72d22cfdd909c03 hive-admin role can CRUD SelectorSyncSets
43810ad27b748b03a3967232d2800bb8aaa977ac Merge pull request #362 from dgoodwin/imageset-hotloop
949470164456a499c5c504ca019caa501d0ac7b0 Fix imageset job hotloop.
d761067055fd7ce1d33bd797b221cf6103256f9c Merge pull request #358 from dgoodwin/more-metrics
63c16fba37f572b40ae5571992815c83edadfc23 Merge pull request #360 from LalatenduMohanty/CO-380
883e0eca4d353b97ec2794b160a2c47e0425acf4 Merge pull request #359 from LalatenduMohanty/steps_to_access_webconsole
b93391418fa75751d3548ad2a232becd435551e8 Adding steps to watch deployment and retrieve webconsole password
0d0adaa17eb8f78966ad3bd84340c8608653ae68 Merge pull request #356 from joelddiaz/protect-labels-and-taints
56a7e4935623034bb3f1f17ccbd2eb953bee0898 Issue CO-380: Add hive-reader role Breakdown hive-admin role into an additional hive-reader role
413d8f3db862d9f294ff6489b5778c3dc2dd712f don't allow updates to existing machinepool labels and taints
65078b047c1c1b27998ad343a5950a8a940a92ac Merge pull request #357 from joelddiaz/mutable-certificates
0bbe823c362f8832a9031800db6d2ab9991905e7 Additional metrics and cleanup.
44a3b84ba176bca9c17d8ae837813cccdfe6d00d allow modifying certificateBundles and controlPlaneConfig.servingCertificates
7badd2771dd50063d11f8c90a648168162e50bf7 Merge pull request #355 from jmelis/add-patch-admin-role
163a7a7aa8711554449c7ff219133374522df3d9 make generate
2bf8de2fcec718c03b9cf62f68417dca7c6775cf Merge pull request #353 from abutcher/docs-link
9d4b2a7637c1465aa3d71d3b86a1ad4eedb62702 Fix typo and link to syncset docs in README.
f5a0f110c1460f10f586a1989e965b02943107ce Adds patch verb for cis and hiveconfigs
074b723e77ece0d981dbb109f8d79f058accecaa Merge pull request #354 from dgoodwin/deletion-skips
82317f389c7d7616b90b9cc27ab1e5647137ec73 Merge pull request #352 from dgoodwin/image-res-metrics
d80bb357f8d0b1d59c4191085c3ba5b6f3ff0251 Skip reconciles if cluster is deleted.
2595a619dde2de1880aef3e95d282e3b458a0c05 Merge pull request #351 from joelddiaz/remote-labels
82767afce6716e3abb0bf0e367ff065ff1678ec6 Remove metric for installer image resolution job duration.
dbe4d12e72bae7aa794dddae523b4037382d6ef1 Merge pull request #350 from LalatenduMohanty/use-mock-through-dep
603f4da856bc0134ba79d4fd517fbdd007f5654e Merge pull request #347 from jhernand/add_genclient_comment_to_hive_config_type
2eeb45d0067fc2b94806a9f89f0c5fce17924bb4 Using dep for gomock and mockgen
a0c80548dc588847e6eb02df59beb14b5c9daf82 Merge pull request #342 from LalatenduMohanty/update-readme-delete-steps
8ef6af2787e846f5fc78c9c87928a9d406713800 Updating the deprovisioning steps
986e4054a1b4ee5b7e2316c4e3f3aae7e38ac91c Merge pull request #349 from dgoodwin/5-concurrent
10c3fe8107d50eee8303f9a89f388134baed2c3a avoid needlessly making a non-nil map
621f3a4191f5050836734b421be2ecd88299baf0 imageset job metrics
4e3e75fa1ac647156446c2f721ba0f1a0d42d2ae Merge pull request #348 from dgoodwin/add-named-port
c0d0fd4382d9958b53a9f78867748a4ba4c87631 Drop from 100 to 5 for concurrent goroutines.
2e488e246a84e9f7cad81afab98b07615f7b10ba Update bindata for named service port.
0ed020fb51d0e3c76262519e3d56e08cb27142f0 add name to the port definition
6149d07664b58aafd30f8d1b77bd0ccd286067e8 add named port
ea75d8e24ac5d4baf59be18123b1e3b302966a69 Merge pull request #331 from LalatenduMohanty/issue-formatting-fix
bab7cbda7688fb2cd39930787c4cebfe4502c652 Use `+genclient` for the configuration object
8f65720ac1e90cf7f253b9941e79907353583cf3 Merge pull request #344 from dgoodwin/fix-gomock-1.10
e8a23ceaf8508b87f82eb49698d2caf449ee8ba0 Formatting changes from "make fmt" on go version 1.11.6
3b2b2d76a5a5076be89e31edeb7b94009e06fa1a Bump Dockerfiles to go 1.11.
2e3ea1635aaf8938ac3739819bc000b79df537a3 Remove generation from container build process.
d0140186ab522fefe3ee934829fc5d75f47ace1b Merge pull request #343 from dgoodwin/syncset-hotloop
d9bdbd97638e23da5504bad33676becce5a1ed54 Fix SyncSet controller hotloop.
def19c611db6db1815359f4b5b6f4fa6874ff282 Merge pull request #339 from abutcher/syncset-docs
75ba8f5c5122abb2a1da908443c6c9b5e9129479 Merge pull request #341 from LalatenduMohanty/update-readme
b655fcb34f89933aeab8b5ff183a90fc74f7a9ea Document syncset.
a37c9a9c7d985107b1d3b6f6a46d44a5d9fca136 Merge pull request #336 from twiest/more_logging
62d643f2293d5e6e08a43856fedeefd7bfaffa1a Updating the Readme, removing the hack/minishift-deploy.sh
458a7d5cbc7ed9f1793bcfc10367c8d38f6f345b Merge pull request #340 from dgoodwin/parallel-reconciles
0214d2e14951e9bad5f802449e3d1427346333f7 Move possible 30s remote timeout into a guarded block.
ee935e535d329aa1b8b07d2c4734e1c72b876fb3 Remove mem/cpu limits for controllers and operator.
4c458893cfb2b81e645aec3b8b400f19287fab44 Allow 100 concurrent reconciles for most controllers.
d16237f4dddffc49c0a89e24a5cd14d7908c6bcd Merge pull request #332 from LalatenduMohanty/issue-adding-make-clean
535080fcef88f0894ad04803fa20978e2e150dbb Merge pull request #330 from LalatenduMohanty/issue-make-test-failure
4733e1443c4556b440417cad4ffce7be08941d86 Merge pull request #337 from dgoodwin/hive-admin-rbac-fix
71aaee733ae7bdeed67e747537ed361f2cc7c4f4 Merge pull request #335 from ShivamChamoli/prom-install-job-kickstart-duration
388984fbbe0a2581efcdca2f87e4131638389f03 Merge pull request #338 from abutcher/rm-object-logging
1de838bbd926da14c547454a43c8084868268b4a install job kickstart duration metrics
d987a417c4bb94883d9396829c6a7d0379f7f751 Merge pull request #321 from ShivamChamoli/prometheus-provision-job-duration
466f847dcdd91b8149e8668c3728367bbc109b90 Merge pull request #334 from dgoodwin/beta4
7b565c7e6c1c976bde61826221d1ac122ba34c64 Remove object info logging.
9518cde9d5b2efa8ce5c8a07065197b20431706e Add logging for when reconciliation loops start and finish.
a06946e0f7285bd30c4120f397f1eb293fafb1f2 Fix plural rbac for operator for hive CRDs.
f4ffa1d3335972c614473243a57c792e031f0502 Add beta4 ClusterImageSet.
475e6bd90689b673da7e71f553a9a1141cb33bb5 Merge pull request #333 from dgoodwin/time-to-install
9de3f2685257abadf5904259c70d5099e0371047 Log elapsed time for cluster deployment reconcile.
34825af2e1e47e9613bf263bea219b21330661e0 Adding "make clean" target to remove built artifacts
d8fb63ffac1975f21c200c5c5dcc7e83fe31e33f Fixing "make test"
efac3571027646b8755b0feb43fffbfaf1aa7672 Merge pull request #329 from joelddiaz/requeue-after-status-fix
12d994502e28d5664ab29144c3c8a3cfa1fb90f6 force requeue after fixing status fields and adding finalizer
ebe3f8e2b39c9edbf22d81389352404f70bad750 Merge pull request #327 from dgoodwin/bump-memory
1f93570c7573709a6e3fd04ef5158ee6a8e6247d Bump memory due to crashes in stage.
91362d1482fdb7193f2fccd1900688b9336e218c Merge pull request #325 from dgoodwin/cluster-type
124a4a7f38e6c508ead989d1022d44e4602b90c5 provision duration metric
25827a29d83c996369d768570d75de0140d49bb8 Guard use of cluster deployment labels.
6a70e07b861cd062f1f3ad147a3b49ea411c2fcd Merge pull request #326 from joelddiaz/no-password-in-installer-output
74cda47782580d4b739e105d372bc2592b6a6b1e Partition job count metrics by cluster type.
ab0d35a228bb2bb3ed08d3b9ce7a1929de576bb4 clean up output to stdout before printing
ee5560ae1769af5b0e68a75c68354306b5af819a Merge pull request #324 from joelddiaz/no-passwords-in-installer-log
e19c988963396a7c5adfeb732fc1149c4d00f8a1 Add metrics filtered for clusters in last 48h.
2887b4701729c1750832c4e163d01d423b475e8a remove sensitive lines from saved log
4aa3f896f6412eb3998f8897521428c053959791 Refactor cluster deployment metric totals to be more dynamic and consistent.
05dc03cfcbedbe30d175652e02a0eca2afe2d69e Merge pull request #323 from dgoodwin/plural-syncset-rbac
86a8844e77823c4453ae2d98eb2f9854320f8650 Add optional cluster type.
cd287961dfd408e41e82c41abe03fb5702a69fba Fix hive-admin RBAC not working due to singular types.
02f0fcf7f87f546a4a2f59733bbde786d70da23f Merge pull request #320 from twiest/vendor_latest_openshift_api
942082c9f76791f5b2f20eda93457a72fd107043 Merge pull request #322 from csrwng/createcluster
29a560daf8138a7e80ae817e34711bab89dff5e7 Hiveutil create-cluster command to create a clusterdeployment
edbad41be3242d010f297c36039f11a9df655233 Merge pull request #319 from joelddiaz/saveoutput
c4a19cabb6c458cb8aec3ead0667c9157e0ccc2c use exponential backoff when saving configmap/secrets
ae5a23e8a8db9ccbbc28aa352c2cff8ddda2361d Vendor latest github.com/openshift/api
d4670d1c4b905281c58606bdedf87a01ed8c3b76 Merge pull request #304 from ShivamChamoli/prom-metrics-job-duration
80dcf05e766490d79e20e185acfd26341079bc4d save installer output to configmap
dd4e460ef9c7eb38268a24d57201a4d054735411 deprovision job duration metrics
ec14bf410cd6afe8c9a2a6d2f30f002ada93ee5e Merge pull request #318 from abutcher/syncset-patch-string
e049d744c1907cb307c6a778576c9fde186eae5f Merge pull request #316 from dgoodwin/fix-operator-role-rbac
c086e44f9e8cf0fa21bce11ce6dc3701944fdb75 Merge pull request #317 from csrwng/disable_federation
1c5c08874c94733a9d273bb4cf713f816b57b7e7 Fix condition update loop.
7a6c6dc910c1afe57a66635c2e36bda4f3f3aeac Change syncset patch from []byte to string.
42ac5eef92ee86010a7dda7c53e4853da4325f6c Disable federation controller
03d973287e833833cd607ecd8569a2ce17cdd94b Merge pull request #315 from dgoodwin/aws-client-metric
426ac646f7368bc56fa417a676b73283bbfb41c9 Fix multiple RBAC problems with operator deploying hive-admin role.
747fcba690024de0c4fa6d77be98edd26699d1ef Merge pull request #313 from csrwng/resource_improvements
4fabfdc1dc34bcdb3786806f40f9dc424f032de7 Merge pull request #314 from dgoodwin/refine-restart-metric
a4bd8bb7ea5b02166297be7c2b0984691afa400f Merge pull request #312 from dgoodwin/condition-metrics
485afcc97e3df46d9b2a4aba16add0b32f04fed4 Add metrics for AWS API client calls.
8bd337276bf7ac5a6466a40eb3b10ee60d18c17e ResourceHelper improvements
9ddd83147e24057e110c9142a83dc917bd81cb35 Do not report restarts metric for install jobs with 0.
f5299846264a528007a39861bd9b589372feea85 Add metrics for total clusters with conditions.
19eeb4cf53285ec44932647b6a82b775581b668a Merge pull request #311 from dgoodwin/condition-metrics
9eec78b0d1f849cfe442783af190f2e8eb6aa321 Merge pull request #309 from dgoodwin/readd-service
22610daaadc712e1d2975000c1e78ae51ab4e646 Merge pull request #303 from joelddiaz/ingress-certs2
06c3c1485f6cd3b31d3670fbcbcf6f8d5d7ee0f3 Merge pull request #307 from dgoodwin/restart-status
147b3bcb4378284b892a187fc4f1776931d32577 Track uninstalled clusters in various buckets of severity.
3a47f096f0654fb51a8ef2a581d7d84b3257a45a bring your own certificates for ingress
b1f91608e8bc202ed1cb35f43d3bce4c18e5a9d5 Merge pull request #310 from csrwng/master_certs
81c9d0760cc60b28766694dcb6b799aafc5da5bc Re-add service for controller metric scraping.
4ccd736642d8d25a39b5fb1462ae3e7a1c9c6770 Correct merge issues.
475438a1d97da51109be41df50ffa3273fb39838 Add missing rbac for pod watch for metrics.
9e6739532913b7e08d010cbbc9394f7cbf144bf2 Remove flaky integration tests for now.
95ab16a6395b9945736becdb6ce4b0c6ae065fb5 Store install pod restart count in cluster deployment status.
17aa4553c0fd2e0c5226d87854b5fafd003ba38c rebase mistakes corrected
12aeca539df666e0fc02cb015003b426a5ef6a53 changes for ListOptions
201c0e7dbe4c23b9d42465efca769082fb631644 final changes for metric
1f8e40d3a4d360f09b0c32790bfae084a3a0e7c9 changes for installer pod restart metrics
1dd9b530f635a6fc7da63ae918949f8e772dad8e installer pods restart metric
8f5e56ff18e4432bb242eeec2b7c83217c4f410a Log how long the metrics loop took.
aed94b524e7280b3206930644e88d84f9d1a0ea8 Prepend cluster deployment name to secret names
36520f9e9d4bc902bcaf60c75da097fceb3eeb00 Fix logic errors in controller
eb6387f3bbd7b33218efa23e1da6ab06fe89652e Fix running jobs metrics including completed, add failed jobs.
83dce70b4f761ff0acc935d01fb0ae025c8f1350 Merge pull request #305 from dgoodwin/hive-admin-role
3c426c2be46cff7116a23185ecb577f561cbde73 Add control plane certificates controller
5f8a16a3f975d9137e864e8fde9d1c6b30f62773 Merge pull request #308 from dgoodwin/cvs-interval
ecb269af6e2657fc8ab88f5d0ae7836882a6caa6 Merge pull request #306 from dgoodwin/add-cd-printer-cols
3e870a0e02b5f5c347ec1cb4d0363b76e3bb8781 Remove cluster status resync interval.
c971bcd8b0b81d53b153716995bff84e5f8bde89 Add infra ID and cluster name printer columns.
68a5c368c507ad017ed334a83153f15a1b12089b Merge pull request #302 from dgoodwin/remove-beta2
6b83d1324379db480e551d2177310179b266f2a0 Deliver a hive-admin role via the operator.
e9cfcb4bd0b04ed1001df3a5cfa15871afbc5940 Merge pull request #300 from csrwng/dns_controller_changes
215e529768622196e1255aeda1c67f4fba69f294 Remove and cleanup beta2 ClusterImageSet.
2caf4ac573e79a0944475a75a1e159d738dd0343 Managed DNS support
deb933372ec600b8dad51020a1be4375a0a3cd1c Merge pull request #299 from dgoodwin/install-mgr-install-config
0f870d1ee1f045db25d42787a690d04f758df7ab Generate install-config in hiveutil install wrapper.
6b1eae28f11db8257861be1963df54bd4a23e910 Merge pull request #301 from dgoodwin/hiveconfig-frontend-rbac
d74a5c53515ff2ad9e36b3c15d2964f14293eb55 Add frontend role RBAC for HiveConfig to view top level DNS zones.
f0ac08ef1ec39dc32506e3509cf1944e29c2006d Merge pull request #298 from csrwng/synccontroller_syncmode
9cbf0f01edf7c9625723d13b24a2f3129f9bfe5d Implement SyncSet sync mode
7667718c9cc0a77cf3c2953d123ff7a95d7c4e7f Merge pull request #295 from abutcher/syncset-patch
38c308f11083119a71b30cfbc22ccbc0e29223d0 Merge pull request #297 from dgoodwin/ami-lookup
82d5123b0ff318f4cf8bb358bcc5afa433dfba47 Apply syncset patches.
38b72f059609a234d47399ae71760d57a9f00a96 Use remote machinesets for AMI lookup.
5183431d23a0f2209c9cdd2b63d999943212165c Merge pull request #296 from csrwng/beta3-imageset
75ca6a25ed667f338416bc678f367b20d878c085 Add beta-3 ImageSet
89e7c908c3457bc03992e4042da7cd1a78ee5fb9 Merge pull request #291 from dgoodwin/machineset-creds
ba6435982692916c98a2c3ce1112b1a31de7ae89 Fix hostSubnetLength in e2e template.
b4a1e06892dc3528719a594a6a625dd87fb35e32 Merge pull request #294 from csrwng/external_dns_integration
3e08d9cd3981cac622f0769ccbae25918a3ae149 Deploy external-dns with hive
1af4d6ffc16b2c04ced525ca1379daf028fb7787 Merge pull request #293 from csrwng/syncset-tests
c2ac6a75b1480bfee5019c2fcdada7beb8848418 Syncset tests
05c1a41c48471e0e865ce4331ae8875aeacb857d Fix missing cloud infra for machine sets.
bcf314774abc2ffaf80e80a69cdacd3a4137c4c4 Merge pull request #287 from ShivamChamoli/prometheus-metrics
d53a7f5f7c66fac718c5dab345278cef063cb613 install/uninstall metrics
6cad865f99526f0fa369f8a1ee49db9249c0ebf7 Fix cluster network host prefix for new installer restrictions.
5b0b5cf0f7753e33c0ae6534138d5901f473f64e Update installer code for machine creds secret ref.
184ff1e9da33738a5b3948330c08bf65bc44dab0 Merge pull request #286 from abutcher/syncset-controller
5edc28019bd061b3b0fef6c0719d8e6728d24a26 Merge pull request #290 from dgoodwin/chatty-logs
9a8fecc04d24525f996aab197f7acef04c0140a0 Initial syncset controller.
cdbe3bb94293aab6273f9386e2ed776c2bf7291f Remove logging of full machineset in remotemachineset controller.
c6fd57fd3d772dda5f17bafa460094198a0f078a Merge pull request #289 from csrwng/dns_zone_controller_enhancements
f3fc2c6719dd6de6913020b0962c7267c605976f DNSZone enhancements
accf34edc4564f3a548e43eb6960a4fb9257da00 Merge pull request #288 from dgoodwin/dockerconfigjson
aa6544fe75ddb5e45966be20782639ddc6228115 Add pre-beta3 openshift-4.0.0-0.8 ClusterImageSet.
99b1bcf37f6b9a04695f6a8f291305a7147e630b Fix integration and e2e tests.
da97adb5ae4e1d5cd1fb2a10fa2dcb86099741ed Remove unnecessary use of pull secret in remotemachineset controller.
99c1c2f4b664f4f32a1e2a5a35908a9356d78fe7 Skip some clusterdeployment install job code if already installed.
1e9c1c8314838150eaebd45b08d79d18d828336f Switch to dockerconfigjson for pull secrets.
84ea1d824336aeef4a8cd0501e31e0af3f3b3cd8 Merge pull request #285 from wking/hive-job-prefix
d50680e53eb1e57995ef6cef2c30a73d23532ff0 Merge pull request #269 from csrwng/admission_tls_restart
ac6d9cb465c173413b65abf9e943be1ff1f14cda hack/e2e-test: Add "hive-" prefix to cluster name
98a7a3fd1661331fb6b03cd1b7cf33d459a5e903 Merge pull request #284 from joelddiaz/add-remoteingress-type-info
a709e020cf3d11445d27c6b5c7408e850aa672e6 add Type info for the IngressController objects
f697ac15523c03c266725cf36b2c2e4726dc6bdd Merge pull request #276 from twiest/selector_idp
c121a6b6f33fb668316a833bf16b35108118c84f Restart Hive Admission when certs expire
693e5980b8834930bfeb81d941e925d4b4747d41 Merge pull request #281 from dgoodwin/hiveadm-fixes
6fda2e9b3d1c75a4bd98545dc5529bb948d33733 Merge pull request #283 from dgoodwin/cleanup-legacy-clusterid
bb5026217b28d82083c87c84188dfddd59b1e804 Merge pull request #282 from dgoodwin/metrics
c2362cac373452c2962792815da1e0257d15d28f Fix IAM user leak on deprovision.
ecbedef03c0738e501159301d1dcf52c1d90c703 Begin exposing controller-runtime + Hive specific metrics.
fc1e9f7a6eba322257b827b94b7a4c592110a684 Add syncidentityprovider controller. - [x] Add syncidentityprovider controller. - [x] Add unit tests for syncidentityprovider controller
74b6c99896a91439fa4b4cb3d7664d043f135151 Simplify obtaining service CA and remove need for global client.
d1174998425efdc4a6654c53648c5f74420c4319 Apply kube and service CA onto relevant objects.
3e7b8d3446317afbba7cf0a7abecb54493f39759 Merge pull request #278 from dgoodwin/operator-imagesets
07203900f8821660cb1e1f65b062843a7feee9d1 Fix hiveadmission for cluster deployments.
cf4acdcd6e4d58831cd35bbc53240286406185bb Add a custom imageset cluster deployment template.
938c260e883bea09e54183c6117bb2359d155ff0 Merge pull request #280 from jhernand/place_genclient_nonnamespaced_directive_correctly
9157a01051075c1a06678dae45be0a1546d0df51 Deploy a default set of ClusterImageSets via the operator.
5e4508f7eb75aec301c03de731585759fad21838 Place `genclient:nonNamespaced` before `genclient`
5c42746c4edbf6c1fe7a08354566401f3085a53a Merge pull request #279 from ShivamChamoli/replace-hiveadmission-daemonset
bd35077fb05b28a94e0f1c81694ba056e184336f Replacing hiveadmission daemonset to deployment
c6dbd8e7006d7cb1e0f372ad912f518dbf3e4338 Merge pull request #277 from jmelis/do-not-rebuild-image-operator
c77790299da7f3185ae43a40e9cef69e9e915a64 do not assume yq is available
64760d5f41f59e2fc4f76a66fce674cb0e0f4dfe do not rebuild image catalog if version exists
048367a537fb178fef1d18c5f7576828f8908a1e Merge pull request #274 from csrwng/verify_generated
071453fee378452d6f7028f9ec811c641595066b Merge pull request #275 from jmelis/push-prod-image-catalog
8297d159dc541e1087287aa900f2dc07373b411c Add test to verify generated files
2d3768ce564a1c92dcd93c874643d5504c36e77c typo
8a870a0b3147dbf1e12caf4de45b8b70eceac766 typo
7504bdf1418efd797a0ae789905e598fadba2505 push prod image catalog
485932e93130a259a2bf59f6ea9f4ab436fad1ce Merge pull request #260 from csrwng/certs_api
ba6ee5efd982a559a8a32a59f16375d5ccfb177d Merge pull request #273 from csrwng/install-job-timeout
67422cbe9df18b5c1066d72934f2630a20853bd9 Increase timeout for CI install job
8ed5b528ed5a4bcf0a706fa04c894bb809b3a876 Merge pull request #271 from csrwng/check_in_generated
c2aa9d86f30e3db8056b1581549a012762ed943c Merge pull request #272 from csrwng/fix_release_override
d9df5cd64ebd0d09d798a918f87313f61661dc7a Specify serving certificates in ClusterDeployment
3eed901b00557f196e0ed3c39026ab5830c22ff3 Merge pull request #270 from csrwng/fix_olm_template
37d5384aae19c03c78a12324423c662f966b2cdf Ensure release image from ClusteImageSet is set for install job
e8b0ed626e1273319af0eaf95b142ca83e324e12 Check in generated files so we can be vendored
a5abc37d845a1a3afc490a686ca89c20eff153d0 Fix defaults for olm template
ac635b031c20df8b51d4c9c5acc45f1c977c7baf Merge pull request #268 from ShivamChamoli/cleanup-legacyResources
c398fce387a714b7a7127b24f2a8024fe8eedbb6 Remove cleanup of DeploymentConfig and legacy Services in operator
626b9e7b9870781ae9ebc0361b2d460d57e776a9 Merge pull request #267 from dgoodwin/frontend-pod-logs
973f63c9efc1bc0cccfa24473dd42946808b956f Add pods/log permission to hive-frontend role.
4163fc2406475ad2d70f62b2748d13cafdf333c6 Merge pull request #265 from dgoodwin/frontend-role
cc95376e36352ff407bc1d095333831dc920e968 Merge pull request #248 from joelddiaz/remoteingress
efbce36e982b18cb69a7f0ff5b50ea47275478da Merge pull request #262 from dgoodwin/admin-rbac
976d46ad795bd39aa57c569f73af709ab4daac45 Add hive-frontend role.
991629b4241d9d0afd6a2c08fa3e513c21da5880 Remove committed OLM bundle.
bb730f1257a2f36001954d54c5464a92d86ca68a Use shared apply helper in both hive/hiveadmission operator code.
6a9c7fdf088b5d0c20131785caa9aae4c5ab9b4c Merge pull request #1 from csrwng/fix_auth
b3f96938a043f996ab70c3acb6f2271692ae2e0d Explicitly read token when using WrapTransport
12c88f148e805ba577a3d1b38268bef8b69135e5 Merge pull request #264 from jmelis/fix-build-deploy-typo
6eb597e39534654b46e910d833b89712ba56bdcb Fix a typo and relocate the AppSRE CI/CD scripts
89aaf350b320f514fc4702a0e51f3b3d489ec3c9 Merge pull request #263 from jmelis/add-image-tag
aece2ea24a2e662a41b8a07a7d3428a0c90337b7 tag the hive image correctly
9693c6d4b64473f81869034a309bae02fc464815 Adds IMAGE_TAG
970b3e609409ab3964d40bce6be1bba0fe5d41b6 Merge pull request #261 from dgoodwin/hideadm-compute-nodes
191b2fb86ce0c630465e5ea33c20cfb314a25ecc remoteingress controller
79f2d3a96e4d21165546bab99c87c5341ae1061c Use resource apply in the hive operator.
a9fff6fa2bbedd62b1018ca88062def9618a4003 Remove hiveadmission daemonset node selector.
5d3c2e7e3dbb4f0fe5b5c5d9626d8df86bdbf0d2 Merge pull request #256 from joelddiaz/openshift-api-update
8c61fe5abc428b6d2f24d89f82d0f3e3fed91984 Merge pull request #258 from jmelis/fix-build-deploy
d5f403d3638035d40bd3c44999013309e74b0d52 fix bug in message formatting
8fc1877096919c5d903336082413116990527b9e Merge pull request #254 from abutcher/syncset-api-changes
e8c06c031e828464b68a74644e8004c05c30144b Merge pull request #257 from jmelis/create-hive-operator-catalog
4c31287262d3bac458c682a0d245641c1749122c import updated openshift/api
74be230443ead92f463c8d363e1a1f65cee37662 Create operator registry container in AppSRE CI/CD
06279c74a7d4ca4114136d10b84740d7a1459519 automated bundle and push to saas repo
6f798b0c2830579f6f370f2fc393743c367c4258 Merge pull request #255 from csrwng/infos_api
df7a47e004aa6843bfbe9ed1534ae3712be30432 Update SyncSet API for gvk and update cd status as lists of SyncSets or SelectorSyncSets with status.
ed963ec5da48a3e57167cb763482ae58497b7a13 resources: add separate Info function
20c528c092b4db302cce88cbeac2855234c16f79 Merge pull request #252 from dgoodwin/remove-package-gen
681c1e0023f7ef4f07a64e66852a887267f12a62 Remove generation of package bundle from OLM script.
14cff038cae0ac2b7f2b339357ef0811a82976cf Merge pull request #251 from csrwng/hive_integration
12c066e87b2635c886f461afa0d7727d5e78f256 Add integration tests for apply/patch
ad32c1f2968c795e4da23f6ad1351048a6ee4154 Merge pull request #250 from dgoodwin/new-olm-bundles
65268603fe4da94a38d0fd3a9e157691761b40b4 Generate new OLM bundles and document testing.
77bea4ac532ea62c07495a5f773a13b93b4f6184 Merge pull request #249 from csrwng/kube_patch
a6b018d9f37ecf8fb6c9be312f4988b343ebea07 Add patch resource helper function
6475c9eae3c306580c906bf05719462e0a6ce030 Merge pull request #238 from dgoodwin/operator-csv
4c65148a0134dd4d6945d7c6db6099797528730e Merge pull request #239 from ShivamChamoli/testing-aws-leakage-bug
3f73a592e78971501f64a068c7eaa413185fba1e Restore "make install" and remove CRDs list from kustomize.
ccfd0f3c125e727daea690ab9a4f50976fcf1ca6 Fix service account problems for hive controllers.
67aec3b70b20b92e7a026b574b55d095b982037c Merge pull request #247 from csrwng/kube_apply
b8f46e1576ae15e91d313038b26c30998a5bec38 Move namespace from openshift-hive to hive.
41ee29afc900a450ef1459a7ccf272f1640303ee Add missing rbac in make install.
814cca92feac3b49b05d29c8dd5c3032d39e3c78 Function to apply arbitrary resource to target cluster
6299ddb5d3e27b07ebd7bbd32c36021ef598274a Override PreserveOnDelete if cd is not installed
830c2ff587829dc7e890b3bab7ad4b0ef09ec91f Merge remote-tracking branch 'up/master' into operator-csv
e79a246145dac5768376db0271058d6dc5a6455d Merge pull request #243 from dgoodwin/hiveconfig-init
98ab98c301df1130ef35010f9669cb0f7f4c8634 Fix ordering of manifest generation for go-bindata.
91b047f1bc317c23bf8d094062759f555c55ecd6 Merge remote-tracking branch 'up/master' into operator-csv
d097626c6ee3cb8676fd3076df67e1082d1088aa Update date in CSVs.
9b6de13f28077236e1c3cd8bd09ed92717f20e7f Drop OperatorStatus/Spec until we're ready to use them.
8ec1ea435c6d9b6ca52fa79c478ff792365a13e1 Remove HiveConfig image and use operator deployment image instead.
9c04ae64ae77de6d24f3664f1294f22ba575770e Vendor kubernetes kubectl commands
ce33b3aa900935918e704bc96d33ed24f9f3b49c Merge pull request #246 from csrwng/use_image_set
f264a246125a81d8474d5e43c68ecd09986cb81e Use ClusterImageSets in clusterdeployment template and in e2e
0a8296b1183a385d97d1b4e5c2817c9788aef602 Add script to generate OLM operator bundle and ClusterServiceVersion.
9b554552dacf89cb58e733a5dc8ee1b734eee39c Merge pull request #241 from csrwng/cluster_image_set
d2f4f2305a5bf8b3c44eafedeab130ab08470852 Add ClusterImageSet CRD and InstallerImage update in ClusterDeployment controller
4f36a636e1e4f1f1a097253c3cf463a9ce10c9db Merge pull request #242 from jmelis/app-sre-ci-cd
ff5ec5f74ade430f0c8963fb1b8dd0a1baf42ff9 Merge pull request #218 from ShivamChamoli/update-jobs-automatically
1e49c900b258816e6f6dc485d065279e8f396178 Merge pull request #245 from wking/network-interface-deletion
587842479ef5e7120befa4a68101b4c6e0cb1641 vendor: Update the installer to get additional AWS deletion
e850dc600cad1288bbf14e0d9f286e563dc5026f automatically-updating-install-job
c1db986d7588afbff2f044e739ebcd9492552ead Remove HiveConfig image and use operator deployment image instead.
8f20a7fff46c056b4f496af89c4fcbe96e8b0e9f Rename hive-controller -> hive and test build
b61557fd276454c9b15fbeeba3efa682aeaa0561 Merge pull request #244 from twiest/selector_idp_crds
2d7ecea52b3ab2cc617d0b85531af1388eb7d846 Add SyncIdentityProvider and SelectorSyncIdentityProvider CRDs.
b226f80d2eec7dec18759275400c2b01e5d3fbd6 build_deploy.sh and pr_check.sh for AppSRE CI/CD
8f8ce6ee5a9f621523c0597da8de7015be4a778a Merge pull request #240 from jmelis/remove-make-generate-target-dep
016012e347ff004dd444d2a650dd6d21698b463d remove generate as a dependency of docker-build
8695b78dac773dc06e6f2f5fe16201ecb5ebb86c Merge pull request #236 from abutcher/syncset-types
ae426f8cf1b6cbbffda4349f2555a5ac09f399e0 Add syncset types.
158603d78733bdf21f65cea69cbcc353320e2e1d Merge pull request #208 from abutcher/ic-non-worker-pool
e10d7a48e089a88e986226a14f37aeaf2c7971b3 Merge pull request #233 from csrwng/debug_uninstall
5f9fac4072b7b1dd90a8dd04565bf5d47c6bb867 Merge pull request #235 from csrwng/move_api_tests
9df6d8acbcffc013a361cb998f5a08b79f875895 Account for uninstall job being deleted
8423026ff40b6f43447a974d93910d0c3ebd767e Merge pull request #227 from dgoodwin/operator
16208cd9d1f8c96fa13f574f0db70e7bc571087c Merge pull request #237 from csrwng/bump_installer_022819
a94f46bec1eb2936a3873c67bb8b503f5464eb95 Fix remotemachineset controller tests
aa6e95250ca718d9a73fae3173bda9a5603f922f bump github.com/openshift/installer 02-28-2019
71f7c86af83410c936c2a2810ea9eea4fdb0d4fb Improve debug logging for e2e uninstall
56dd65f3749accd483a7f7a69312a83f9c7dcf6f Remove faulty leftover err check.
9c9d0363a8db613ccd253b1525543ec58e2eb5ba Move tests that run test kube to integration
8dcab7d39ac8ed531d4f664fe89bb28d8019ca46 Merge pull request #232 from csrwng/fix_dockerfile
d22c82bcbe7950529e47e84d5f659197710a3206 Fix multi-stage Dockerfile for CI
6bde0cb5973ba64b880e177de32c272fe7b33908 Add hive-operator in CI Dockerfile.
688b17a00fe22cfec1e85bd29ed5947768416ae2 Merge pull request #207 from abutcher/machinepool-labels-taints
a0cbd50a3f5a224d5ae0300bb9e40b6a51636f72 Add some CI debugging info.
fc3dbfd0bd94381bab95b9fb370d69cbe124017b Apply Hive CRDs with the operator payload itself.
64bd8f987102ba40916618b93207ad5a9ef71293 Add missing ConfigMap rbac for hiveadmission.
51be784e61bf130c74fc7e998edad5311abbf700 Add missed hiveadmission rbac to manifests dir.
63fd6fb6dc2529c492ee06051a246f34a347961b Skip metadata for go bindata.
7bfc954be01e31c654280e36eef2bc2ac55a4900 Remove non-worker pool when generating install config for installer.
517be59c3c9ce8cf5b4bb08d98be65a3a66dd13e Merge remote-tracking branch 'up/master' into operator
1177718716052e2f6c3883f5752f94e332cfd879 Add MachinePool labels and taints.
3b9f2779f4cfba486069dae364a0fd95dc74f6fb Merge pull request #217 from dgoodwin/image-pinning
e79c21ca3655415eadffb15317e9508060bd5de0 Limit cache to openshift-hive namespace in operator.
feb1fde75b42f61ed446153604e397b11f2bc824 Fix event namespace warning.
9891707bce564d2cfbdb32f10edd9df5769285b3 Merge remote-tracking branch 'up/master' into operator
4ccfdd0b710c9f1fc7688407f75724c36fd3d933 Use version of go-bindata with MustAsset.
a2073ca8d6e997cb01b6200554061b09d22180c9 Merge remote-tracking branch 'up/master' into image-pinning
a134041dbe1c0e934aee8839736c4164c80b6953 Cleanup use of mismatched images and clarify docs.
982152df57fa188237f9087176b4beedca6dc6c2 Merge pull request #230 from fabianofranz/clusterdeployment-crd-names
7b378a3fb1fbdc32e4422a37b2b994969c082c80 Remove unused services.
d9b731a305ad1b6760f88f1cfe2d982f801a60da Cluster scope for HiveConfig, add missing OperatorSpec fields.
7412f5e39e79fcccea781cf92326e414dedfa4e7 Fix some Makefile dependencies.
4b72a617bf3ca8678a71be5d0daa4b2aa5158a14 Fix bug when deployments do not already exist.
6cf9edca34404b9a6a190b8fecf5467ab0a56496 Do not rely on HiveConfig outside the operator.
3a8833642e6e15da4d408ac61a1529d4fc6f627e Embed OperatorSpec and OperatorStatus, unused for now.
e7059aede3e8784fc2a3fa42b49eaa601b516fd9 Short name and custom printer columns for the ClusterDeployment CRD
a357d7fcd669a9fd288c844ed6630a225bbe06a5 Merge pull request #224 from csrwng/clusterversion_controller
6d1e3c6f483e4d5011dd2cf29e2ce117ddac3e49 Add controller to update clusterversion status
c141270ba74b7bc0f0a2d3ed55a81ee098c37e14 Merge pull request #225 from csrwng/support_legacy_fedclusterref
bc99566164f9e2f096babeceeaf99d5a239b1322 Merge pull request #228 from csrwng/bump_installer
df4a5ffc8c938889fec6d79d99a365a99d9f1b03 Merge pull request #1 from dgoodwin/infraid
77d34e0899e7030cb9be5c66051e063213a7626d Support installer InfraID.
701b81d4c44d0681404d013b4104d7d2ed1eb7e8 Update to latest installer (again) - and fix clusterID
2c2b18554594d30a9e1933f9b31502717aa57aa2 Move resource apply functions to util package.
9483e36a54cb60531926ed2673f6b0f11cae269a Merge pull request #229 from dgoodwin/openshift-sdn
91c8febfb6ce00363910de552a6e6a083778e05d Use test hive image in clusterdeployment
08af8d3e748748c55bc402c02fcac4034ed08d6e Code fixes after bump
3eda6d129c179e14dfb5b0eed8eea7d261c0241a Bump to installer master
f397608aed2c96f456ae893d712484c3953ec8ba Fix HiveConfig RBAC and support Kustomize 2.0.
6d6cddf8575d520376cbec3bde89f6b43c05fcbd Verify fixes.
d87d1156c178c6be3d67d081d2da3ee558ded37b Merge remote-tracking branch 'up/master' into operator
e3bfb15d718bad6b59eb5c11a756c43967a70138 Test fixes.
335c9aadfa5ec01bb449b7f5cd3b9a26c0aed882 Merge pull request #223 from twiest/make_e2e_more_resilient
9a498668fccbb891c33233b93bbd7bb6b323489b Match OpenshiftSDN -> OpenShiftSDN network type change.
3df80597ff0603c25d327aa131daa5141140904c Add retry logic to e2e-test.sh
a9ffb5af700bdc46dab2a880ec8414cd9e99242e Merge pull request #222 from wking/install-config-v1beta2
4b1894140c9b5cdb7dd04f862a28b2f3b9769607 Use HiveConfig image for provision/deprovision jobs.
ffaddb80f36fec245d02bba270a55c6fe897ada5 Support changing image in Deployment/DaemonSet.
fe8c892d6b15999a01444b2ec13231ec459ee0db hack/e2e-test: Set the executable bit
fce374166519da9202725e3551ea2c9232984fb3 hack/e2e-test: Use uuidgen to create the cluster name
4fb71abf3d7385aacb5de3e13ff08a732981711f vendor: Bump installer to v0.12.0
ab7ee975eb4bad26bd4adc489866986f083c83f7 *: Bump to install-config v0.12.0
40ba4f4387c005ad886685741e970a2fe05ace98 Update opshive deployment instructions.
bf7bdc647ccd1a22d5f2804f6413fca457117abd Update README.
1287b6549529159ce425c75d16604a1ea0e7d915 Merge to just one HiveConfig object and controller.
1f81907e18b1e6a1b7c307b61a7149ccc61c487c Watch for namespaced resources we manage.
7d16548b6cede4d3bac5cc9217a030d445147ce7 Only allow one HiveConfig and HiveAdmissionConfig per cluster.
1b92a8c58345ad14852b630a032d1915c1f6cbc8 Support legacy federated cluster names
6976e3679c3d5a2b8e3e1db62082667354df6a67 Allow configuring the Hive image to deploy.
58d82adbfb9c32d25518fc2cb04ff6e9c9afb0cf Rename operator CRDs to indicate they are app configs.
c08594ab7f9c1d90e8462c0cc76496a2729f7171 Rename hive-controller-manager to hive-controllers.
21961804d3e4307173292888ae981f00b8070456 Add missing webhooks to operator.
d8eee4b4bc27fc4112f175c524097231d34e1069 Merge pull request #219 from twiest/kubebuilder_optional_comment_tag
2b7b6ed2b9f087fd5f8421af2756c7b8bd99940f Change kubebuilder dep to one that respects +optional comment tags.
7fb42d3b64d8eaaadef626f57de9110798d39289 Merge pull request #212 from csrwng/federation_tags
c5c2bc400261b70a6c67f2a7326f2ab704ca59a1 Fix issues in Hive deployment.
c9e4423a7f59e1b07bf1ecf79cc9c2e63263263c Merge remote-tracking branch 'up/master' into operator
1ed4e67acb5b6e4dffeb10113f4d8302adcaf5da Merge pull request #215 from twiest/fix_for_kustomize
b651f9f266d13c21e22dda60b019eac5743b95be Isolate and manually maintain operator RBAC.
ec9c5b5c8881083bb4fffda5fee02b4f91336325 Deploy operator with make deploy.
7a474d4c20469e71b4c30384d4792821ffd0620b Deploy hive with operator.
ce10a227ae9d1040afcffdd249224c67bfe9153b Deploy hiveadmission with operator.
1900f449f59667c4bacc8335625ed3e76f40a75f Vendor go-bindata.
050695a4ff6a9573c01b871e12a2ba9c10acf5ae go-bindata wip
da29a6c8c5669c5e848401147947fbe5b016ae7e Review fixes
870cf563c1c7ab16e5c6d27913a1fd1cb7acce9a Make manifests to generate artifacts for OLM operator installation.
89385d73eb010599015a030e9d545e5d94a0dbfa Start of a Hive operator and HiveAdmission CRD to operator on.
97ab2d2c0e9a99d6574f7a634ebb65825ee83daf Fix layout for kustomize 2.0.0
4783bdbe4aae52a9c53fa5d0bd96b24324d5d46c Federation controller: handle label sync
2fbb0c7de6be6cb7acfde154085d55fe90908408 Merge pull request #204 from csrwng/e2e_test_update
e8e0dfd1cd1b2007a8d94663612fc5104774a209 Merge pull request #205 from csrwng/update_dependencies
b40dbddeb52be1253b992ca2c8e1ad5880cc79a6 Merge pull request #206 from csrwng/update_kubebuilder_version
3239b0550aa4a709f437daef6e7f79687ef6c512 Update kubebuilder to 1.0.8 in builder image
a7fc922752468b391133d6f8182f23a656ae2ff5 Update vendored dependencies to Kube 1.12
95ae59c697a798b212e461b8cbb5d7c76258b780 e2e_improvements
2239699589cbb2e24b1c00d99601695f7d8de19c Merge pull request #202 from ShivamChamoli/additional-checks-cluster-preserve
899b9451ca53fe5292767860fdc848336d9a742d additional safeguard for PreserveOnDelete
85287d3497fa0a8e98923b9ee3e127110b62e5c3 Merge pull request #180 from abutcher/multiple-machinesets
2d00743f75ae8e5d79f47a711c9f94ed0b49758b Merge pull request #191 from csrwng/e2e_test
13bc1aeec6697c08c339bee5daf44f717ecd42d4 Merge pull request #200 from twiest/vendor_api
102dc4258abce80ab569b00cc4413527ede1c57f Add test for additional machineset deletion and fix deletion.
97ec2f6b15fadfd63fa64b9c9ac9a78b4c16868a Merge pull request #201 from twiest/fix_makefile_sudo
8bcee7edb0afa74db011c91534820197f9cd980f Add e2e test that installs hive and creates a cluster
6b97e2fd460a8c90389429395fff290dc5a66a15 Fix setting Makefile DISTRO variable.
c0956dcb53043adef3a06572a988567bfc872122 Fixup previous revert.
9ca73645b0fcaf0001ea40023b424cbfeae29989 Make use of first machinepool's AWS resources initially.
dde0e9cd9a95d5437b89607dc742ce23af794d6b Revert "Vendor github.com/openshift/origin/pkg/cmd/server/apis/config"
61d605d360ff4f3ee6b9c16c0dd677119e505f3a Merge pull request #199 from ShivamChamoli/correct-web-console-url
362a17d09322a1d5fc328928dd7ba6e9c41c8cbb adding https prefix to web console url
4ac4c41162b9f436bbe6306c291b9105768ebccb Merge pull request #198 from twiest/vendor_oathconfig
0f88164f6fb9f5b5204e3c4b755c65f5dcb26079 Merge pull request #197 from dgoodwin/opshive-fixes-2
b89cb2aaf9049d3ff9266981f6d00b704804d55a Vendor github.com/openshift/origin/pkg/cmd/server/apis/config
6f3ae005392d2208a057e7dcafa9f508e5fdd5d7 Fix cluster version status on older cluster deployments.
c793b76b7667ad35bc625bc580b02e5c8142e2e1 Merge pull request #196 from twiest/dns_warning
739c1b6f9b3bdb80f6a24ca9ab4d3b744b092229 Add warning to README.MD for DNS base domain.
dc37f2ea1de3263decb4ca745a8112d340865997 Fix crash when cluster deployments have no annotations.
2db95bf11678c3031f26c25b0e294a6b7b611b9b Update SD image links to latest release.
005a0bacc8a92039774077fdabc4a6ef083eff24 Merge pull request #194 from csrwng/try_once
35cf1eacc4dc7cae71a7d61eb1998c7c10591d13 Add annotation to try install only one time
1accaf8591a33bbf94e4b493c1e1bd5859b313cc Merge pull request #192 from dgoodwin/web-console-url
2a39c29ce7c1724ced20fd2f058c95cf88a93f5a Merge pull request #193 from dgoodwin/edit-preserve-on-delete
34ca51807a2dd565f3c7767f95c7ab54a05a5a91 Allow editing PreserveOnDelete.
699ad873eabf619a00252a7680a447f37e75de80 Merge pull request #188 from twiest/admission_logging
cf0ffa494e8b5d258c3067c428620a54752ac457 Merge pull request #190 from csrwng/parameterize_deploy
5e53ba1ab633317418a05ddadafea9fbf9ee466a Fix gofmt.
435824c569ddda1231ca67376725c798abb78f7b Allow specifying a Hive image when deploying
5d8a7bbe91185ba7d90d9ff3e00caa4a741c446a Consider multiple machinepools within clusterdeployment.
79fade7e5c463c7d892a9cc8b1cdb004c2369f2b web-console url bug
85d3c96539dbe1aef53091419796c2d84df5f151 Merge pull request #189 from dgoodwin/deprov-update
d9f1aa0360fc4d553b2594241c5fbf78c13da819 Merge pull request #187 from dgoodwin/fix-another-spec-modification
9a4a29768b480d1e905cb3b9a379d8533919b9fc Update deprovision vendored code for dhcp-options fix.
04f397f600bdb7dd68bfcf730523ffe9fb781968 Add the fieldname that is being changed when denying admission for ClusterDeployment.Spec.
2daca6dc2ca402c4c0fecae5d535d7a5ce4ebfae Fix another spec modification.
d4902295a02bfe3cb726c58617b967e3172c5afb Merge pull request #186 from dgoodwin/remove-ami-from-api
459ba8424ccf3645844974da428ca1004c7a2633 Remove AMIs from API.
0a5c615100d51f766fa1ec27bfed9dd007d35ee1 Merge pull request #176 from twiest/crd_validation
8cc519a17b49de711b81418179f4aa76e279c702 Add toleration for NoSchedule to hiveadmission.
8900ffa9730b6587ff93644cf33e55de606427d5 Merge pull request #184 from dgoodwin/update-installer-deprov
bc3fd119d57be6100be0bf8018a0c264d3710333 Merge remote-tracking branch 'up/master' into update-installer-deprov
a12dc78aa574837ba12eb1568a99cbd1bc0950ff Updates to fix vendor compile errors.
ea23cf7dfadcadb8682addf4495d573d6ab4ac1f Merge pull request #183 from twiest/makefile_fix
122991feab0df74f9bc66689d84ff2134e00be15 Make ClusterDeployment.spec mostly immutable
e4d2ad9f828d04df4790fdf1eda2f5b2e6462322 Change Makefile to run buildah as a user if on Fedora.
20e4519a58c8fc4b695de696cfa346edeb24ba49 Merge pull request #181 from csrwng/federation_controller_improvements
7843d6a0c11d728769351161f6434e62aa253dcd Use a finalizer to cleanup federation artifacts
17c62092f96b1782d4d4a76c633b39d352fb3d4e Fix cluster-api deps for installer.
7d3cd103c6f22175d6178ccb7993e972b218e419 Remove mistakenly vendored federation code.
b8871189bd58d607d469a29a83a83b2cc064acce Update installer vendored code for paged deprovision.
f08b3885506663148f2da3d747c5210299891944 Call federation Join with idempotent flag
35531704f38431a2e968a9d5ec59240e7181dba8 Vendor federation with idempotent join
c7d424889289a0d4364ddce7959761f5d75ae870 Merge pull request #179 from csrwng/fixup_clusterversionstatus
ea61b9e25d14599a8997ff227762b3ae1e7b8bc7 Set History to non-nil on ClusterVersionStatus
266dc4cfed3be1af5c25d49167a502f0f01855bd Merge pull request #178 from dgoodwin/fix-networking
58fb04bdd3b384092ee9752dadfbdd2700ef9bf8 Merge pull request #177 from dgoodwin/optional-preserve-on-delete
a297706d3e0a0a8d7931b01fc54292005f56e8fe Fix networking in cluster deployment template.
3d05e4942637de7841f9736bba1d44243b4e11c6 Make PreserveOnDelete optional.
d4b9f418d7df452bc5fab09c9ada48443f8c56e0 Merge pull request #175 from csrwng/update_openshift_api
55ee2565dc1a833d92b1ee3b9300b36159c87cf8 Bump github.com/openshift/api
af1e5ae7675cceb769bb9045436000a26a5edcb3 Merge pull request #173 from dgoodwin/preserve-on-delete
05bfb18d8399eef65d61f0d696f621df64cb8017 Merge pull request #174 from csrwng/federation_example
e5576725d6dca7e22bb6feae416e7272c5ef06ac Add operator federation example
3a4718940417f1f9329df131a1c5a4db6a7d1253 Merge pull request #171 from csrwng/federation_controller_part2
9111b9f0389e0300b85697824123d2bc7d6151d8 Merge pull request #172 from dgoodwin/release-image-override-fix
14930263afc8917cfe25a6f366e4d2292a9cca22 Fix gofmt.
1e207498bc873838da31b203c419e66bc5a49c3d Fix installer release image override var name.
bf1a693a272ee5228fcf97b95f25cc9c78f13c4e Merge branch 'master' into preserve-on-delete
5452c99ec008120a0f0857e3a40cd6d28b326f6c Federation controller - Next version
1013ba35eb6689e16afb135fdbacce3cb364918d Merge pull request #170 from csrwng/fix_rbac_for_federation
3edb4489a624874328109e6767056c0a3664ba08 Fix RBAC rules for federation controller
2c2363ebade245d9e5c45f8e153138a3abf46b8e PR for PreserveOnDelete functionality
55777d37b4779e754a519b8143ff1c5f01762dbf Merge pull request #169 from twiest/sd-release-20190116
47a353ffee3d0a3aa76ad36736a39de2b5049b7d Merge pull request #168 from joelddiaz/clusterdeploymentname
9c8c4fb4f09afbcf83da911680eb047ad4417ef8 don't assume clusterdeploymentname == clustername
c7147d813d91f7becc49a2a4c91b208a2dfda360 Fix sd_release.md docs to be more correct.
16e73a5c8c677674cbb4fe00310cf61c043b5c65 Update SD image links to latest release.
2f826c2faeb65b6f1aed13440ed558dce8e302da Merge pull request #167 from dgoodwin/uuid-upload
4182ed4aff5ab5b3c41bc18d4335476cf8e67457 Upload UUID before provisioning any cloud resources.
b71943123aff8670ab02bce08a525814f2ad68ae Merge pull request #166 from dgoodwin/region-deprovision
05fdd5ba7bd3ba21767bc25b34ca2c65f3e12b1b Merge pull request #164 from abutcher/pool-config
3fc31d7a52dc6234b7e28b1ae770bfa827e4523d Separate ClusterDeployment.Machines into ControlPlane and Compute.
1a643016d269b9b3ddfb6da48ee976c5aeaff6dc Merge pull request #165 from csrwng/federation-controller
c61dad521d657cbb72f61a330bc6430ce55f8a3b Review fixes
bad11cf863bc279bd15f592eaa2b9a50f73402a4 Fix deprovision only working on us-east-1.
7fb96f9379d6ddb6f93869431f0243a90fabb919 Federation controller
d950cabeb147288ddba321942a00af3b2cfae83b Merge pull request #163 from dgoodwin/api-cleanup
f6119f920c70aae70b333b1073fe85be681f3547 Remove Spec.Config layer and rename ClusterID to ClusterName.
98f7269d0ae761e53d2420ae97b87d1c62e69ab7 Merge pull request #156 from csrwng/install-federation
1a6aae056c75d16c6bcd37ccdd36a06b13c726c4 Merge pull request #162 from twiest/sd-release-20190114
a732d5de98faec60163342fe86cf55a4c89e4c7e Update SD image links to latest release.
f993b777ef86ae900108bc77161dc0c68fd50374 Merge pull request #161 from dgoodwin/drop-clusteruuid
4cfda6444341037e57d00111d9b007f5838256d6 Fix cluster UUID not updating if nothing else changed.
856b0fc5b90449f8bdee49e450c507d760fafbaa Handle installer removal of cluster UUID.
31300aec0f1a6bafb525b0745ccd3e9f48b03470 Merge pull request #160 from dgoodwin/install-config-version
0732b2a69ce5af8f316f8cf252a6da2b4627757c Merge pull request #159 from dgoodwin/cleanup-kubeconfig-errs
dcefd986de53b4047fda15784b55aecc572dba2b Cleanup errors when admin kubeconfig doesn't yet exist.
17eb403b3a65a0bedeed5ff15658c7b4e6471a93 Add install config version.
38df5734cd4a7cf502e30d2bfe35c842eea1d3fa Merge pull request #157 from dgoodwin/fix-default-image
147a252182af7f8778d871c02a459299460ace17 Fix the default hive image in code.
d31384cc3f82d67922824bcbbdb87d13dbf58989 Script to install federation
70cf20aec9a7a06e17987157c034cc9aaea04dd9 Merge pull request #155 from dgoodwin/uuid-back-to-status
5a317e31e5bb5e2997c367e47c165106de49bd30 Match MachineCIDR and ClusterNetworks config from installer.
682fb2673cfc1b2f13941cf0226bcbdf94fbb1bf Re-add cluster ID to deployment status.
1b67e15719b8f06bdda75acf32143081074c3536 Vendor latest installer for changes to install config.
5134d94b8ef3971c54d98fd80e62523b9904d899 Merge pull request #154 from dgoodwin/fix-bad-scheme
529d0ecfa0bcbc15e8448e825eb8836c7bb1e5a1 Fix missing config.openshift.io type in scheme.
b3fb6eaa26168264a7a3156b0eaa9eb083a97380 Merge pull request #153 from dgoodwin/deploy-improvements
9fb838b76a8acde45a41549cedb3f574b11d6719 Drop now removed admin username and password from examples.
e16d9e5cde06479e5c8ef8be0da3d9d175adad19 Improve process and docs for deploying in cluster.
628597ed1e74b292e148d30067c40ca9c57cadb4 Merge pull request #147 from staebler/use_install_config_yaml
ef2d6cc1bce3c5e694708cb468788ca5c3121e68 Merge pull request #145 from dgoodwin/vpc-crd-updates
f29af672a1f59811f3a01c99864ed03c75e8ac96 use install-config.yaml
2faffac2c229474e250fedbb0066de2a76f2c963 Update CRD for changes to VPC API fields.
464c1c1a94dd3ab62ac0c6f5d46f26b700d10a02 Merge pull request #144 from wking/vendor-aws-destroy-logic
f046c358840d18cc204c2cb4533819490955efb2 pkg/apis/hive/v1alpha1: Make VPCCIDRBlock an *IPNet
99124d71ca7f8b1726069b73a74e6d06acfafd5c pkg/apis/hive/v1alpha1: Drop VPCID
e1fb618c17473af3459097ea564ca2ad6c829562 vendor: Bump openshift/installer to a7468d16b81d5fee95de4dc632fabe7b88d17f05
89a3af7cedf1cd8630c3ed5aef0e8cdbef94c454 contrib/pkg/awstagdeprovision: Replace with installer/pkg/destroy/aws
ad6f8d5b8ada076792b5fb64d313f0e5d5a0e1b3 Merge pull request #143 from abutcher/capischeme
70f3bad269d3ac0517a6eaa3d931fcef50979081 Set cluster api scheme in cluster api client builder.
5476306eb2a270f8caee2a1e9482a9ab4d37aacf Merge pull request #141 from dgoodwin/opshive-fixes
a54f43d2df1eccff06d6dd146fea32dd6f95eff3 Merge pull request #142 from csrwng/multistage_dockerfile
8c88e0941045d5aaf2cbac8e3123fc19c0aeac12 Add multistage Dockerfile
44b97dfe99c17ee6f8bb4d96e2926611f80587c3 Fix renamed release override env var in installer.
a95fd18530b01098c5b88f7a9f296001678f7805 Merge pull request #140 from twiest/add_validation_webhooks
13e2fb45bba5b5443e802c2ec0327a6a5d368e49 Fixed path for hiveadmission in dockerfile.
802db5420da6a88f034fc2501081e2ab12e8463e Merge pull request #138 from dgoodwin/opshive-fixes
ee8657577b0b66fd51331f2802af79d3313715c7 Support deletion of older clusters prior to openshiftClusterID.
f078753eaae60cc12091d9608150421e730e21a5 Tolerate deployments without an SSH key.
5bdfeffd0023b12d4a3dd454238b277f324381d1 Bump memory for Hive controller.
0817a1b0225218bc7632d9b3a73dfc8d1048db6e Merge pull request #137 from twiest/add_validation_webhooks
c0fd8297d7fde056812c539ac3e632775b291660 Minor fix ups
67901d396ec46474cd8b6bb25ae4d27e0bf7d501 Merge pull request #136 from dgoodwin/sd-release-20181212
0602df678e42d05ab2e33b1d14d0923cfe8d6e32 Update SD image links to latest release.
35441ac627200726ab9dae96386dcc4f94e60614 Merge pull request #134 from dgoodwin/release-image
5ecd1b6165722d33f161b602eaa93bd6eb19d952 Merge pull request #135 from joelddiaz/more_fix_clusterversionstatus
c9a9d2fc2a8a13cb4036060a98e63b0746e4ed21 More use of omitempty for optional fields.
9dd3a8606819315c8bc51720528dfc135144f06f fix clusterversion.Status is more places
587a511dc7181380dfd806954b196c9f6ee0aa6d Log errors removing the deprovision finalizer.
252f9a980212fbc325d68693bfbb50a6e35dbc70 Add support for specifying release image.
759234aef443f3308ee62d99f31ae94fbfe480c7 Merge pull request #130 from dgoodwin/upload-kubeadmin-password
b814da6154d12bb4b2cad822483b6d42d3549724 Merge pull request #132 from twiest/add_validation_webhooks
a524df8600174da7bf3369d51d5867cca0865aa0 Add hiveadmission to Dockerfile.
fa0a2fc6f09083f5b75486ff5068de54cf59aecc Merge pull request #128 from twiest/add_validation_webhooks
bfe5e85765d926ca80ff6c0b5455384bc408f97a Add validation webhooks for hive CRDs.
20f2c7323b639f805e950b4058045a3fc7fe43e4 Upload kubeadmin password after cluster creation.
c1d65458cfd134819f02a507b9425d4b0a97e580 Merge pull request #120 from joelddiaz/clusterversionstatus
5348f6517b74fffc52b99828258db8a4e71b36df Merge pull request #131 from joelddiaz/update-kubebuilder
bf4c3696c65b4e5a954af18a82251f4aadca593b update kubebuilder version
6b498e0402aa7cf70003c8ac8eaef6dc30a52b9c WIP: store cluster version status into clusterdeployment status
81909a2401b81b00ee11d115502c3e05cd979b57 Merge pull request #129 from dgoodwin/no-more-terraform
604438168304fe7748f06b8882337c83dcf2581d Stop copying terraform binary out of installer image.
a870fff8cb86dc100c3d05e5212b3c9afad631da Merge pull request #126 from staebler/replace_tectonicClusterID
4452543cfe965907181c0b98ef798b08d75ae169 Merge pull request #127 from joelddiaz/gomock
e733614251e534d653b0603eb1a4a9db0ab8975e updates for new installer
af50e6839406a2add3ec482a9a608538aa3dc6aa update gomock
6a78fa1b1ac64e5d66d2f5799945867510420e85 replace tectonicClusterID tag with openshiftClusterID
e68f4dc80162bd028e86fc45b93ec6d3791d7103 Merge pull request #122 from joelddiaz/delete-vpc-endpoints
08d272963bf7eb24555af8f09d1cbbd2667c61d1 Merge pull request #124 from dgoodwin/rms-generate-name-fix
1e6a65b079f40329dba8df39b9043ed4018f68fc Fix a bug with uninstall after the AWS cred secret property rename.
adec9f81dc220be9cd067b70900b4839ef04322d Fix remotemachineset controller when cluster deployment used with generateName.
b7d715187ba967b42d8abd36c9914fd011d8698e remove VPC endpoints
eb3cdc79bbaa90c388e0ab1a2f8b7f5be707a983 Merge pull request #118 from dgoodwin/aws-secret-keys
6b31677c041380d632b67d7bef7ddfde8cf34b68 Merge pull request #116 from twiest/vendor_generic_admission_server
a1f20aefb4f6f2cff71dc589fa34a713ed5ab5ce Vendor github.com/openshift/generic-admission-server
fe65629f2a655a66a1c6ba48a8a205a19b42123e Merge pull request #119 from twiest/fix_go_cache
b5fbec4a8b1748fc7079c25c7ba5957f7ad39ebb Fix go cache error during build 'go: disabling cache ...'
91188817b81f75a041f452ccf742de7b48226164 Merge pull request #94 from abutcher/sync-machineset
744c5ef9a34f40266e3496f4ae68280b5e90396b Sync AWS credential secret keys with installer.
b4f11003335c60b6c7fd0f08668681a8a0f1074b Update dependendies.
928dee011f601da762abee7ef9a4171937b8b98d Add RemoteMachineSet controller which syncs MachineSets generated from a ClusterDeployment.
8e1708f82b102c2290ef4fdbe5648d3a361de5fe Merge pull request #117 from csrwng/support_glog_level
64152d2a1d4747845967e8f5b9fd4b89db7aa1b0 Support setting glog level on command line
7034556e738edfcf337ed21c8a3f46ed25975512 Merge pull request #102 from dgoodwin/buildah
909197fd6466d13bc81ffdd49f71445090927873 Merge pull request #98 from dgoodwin/generatename-bugs
2349f175d3e4fc6542dec79add881a59f2d7b1b8 Merge pull request #113 from wking/aws-tag-deprovision-ignore-all-errors
f945dbb3fac69cac16ffe773ee71141dc2112efc awstagdeprovision: Ignore more errors
91c0ceee12a6f60090d08cab494f01e512c80951 Merge pull request #97 from dgoodwin/opshive-logging
ddefa0c2c6d11d027c8bbbcf9ac14e84b8c9832c Merge pull request #101 from dgoodwin/log-rhcos-errors
fd92d98091acb208351657132998b1b1a7d58640 Merge pull request #105 from dgoodwin/install-job-protect
550a8d4e15d1fc6db94c5ec6ae2e764a97297eb0 Fix cluster destruction when install job deleted.
54021425ba626acc45fce92b5b43a848c0e46ac7 Merge pull request #103 from yaacov/fix-cdlog-errorf-typos
6b8b833c7703fa73bc5c59dcd0a5727c02776be5 Fix bugs resulting from use of generate name.
6b1d82b939db1af1e05701d08a786d6ccdff0cab Fix cdLog typos
244dc395cae37a35d8c78ced825a524e5798750f Add a buildah-build target.
622f4171acb07a81155e8bdfe02c1e7e511e8b53 Log errors during RHCOS AMI lookup.
5a359d10a189b6e1fb906360bdab49af064b51fc Merge pull request #100 from yaacov/add-dnszone-to-readme
3ae602f76fb3b197d4a6b90a134edcc699c1403f Add dnszone crd creation to readme
2821ce865ab3d75e5d3e67ab30172a3b6c1597c8 Fix lack of debug logging in sd-dev cluster.
345682ad49f0655dbff4ce30cefcb4508a486ee7 Merge pull request #84 from twiest/document-sd-release
ac262f95aec77f84ad05b9c77da9d6d2a49d3afc Merge pull request #92 from joelddiaz/more-cleanup
c7fe72d7a0a4e85e55af3a0e2fcec627323fdd77 cleanup configmap and secrets before install
f14975f177e8129ca427ab5b5526f40730e2824c Merge pull request #93 from csrwng/flag_msg
db6bcc0c011569ab46fe010eec81a467d95a6115 Remove extra log message warning
f5d8b68b74cb26c9f01f2d51f0e900768f09bf03 Merge pull request #86 from dgoodwin/sd-release-20181119
5745e39715e24ca7beff917584bb884ddc017c12 Update SD image links to latest release.
e77ab9c1946d32307b49588c089bd0a1549948f7 Add doc describing how to do a service delivery release.
0d050003b67bd63962197b53a07a6837080841b3 Merge pull request #83 from joelddiaz/flannel-to-openshiftsdn
916e0112867d3938e20174ba41e87c4159a81017 move from flannel to openshiftsdn
dee094f6681df6ec6acb695705c1299c2d6e0222 Merge pull request #81 from csrwng/rbac_status
ef5107abd49c540a575841fc18fb36738dd426ab Add clusterdeployments/status to controller RBAC
9b121f98cec849639782a3fdaa293370c16664d7 Merge pull request #78 from dgoodwin/status-links
460eb7e4091f8af5f8a0c39372a333f8932a4b26 Add kubeconfig secret and API/console URLs to cluster deployment status.
9c2ec4c9003e18354063865b9d28e8a16ec577b1 Merge pull request #76 from jhernand/add_codegen_requirements_to_api
3f80de11911ebb728c2e36926205edaaece7be58 Add code generation requirements to API types
3ea2acd55733df39b13f3a753e801fb891fdc0d5 Merge pull request #75 from dgoodwin/ami-lookup
d2f43f6c3d237b0e99bad45b336d364d61aede93 Update CRDs for new AMI/Zones machine pool params.
3f09c21acf40957406b15f631f4bdea01b78a778 Merge pull request #74 from dgoodwin/ami-lookup
d2160d32f90c24cfc3ad4725fdecbc78bfaef476 Lookup default AMIs.
9bb090933b02cf8b39e545324742e8fbe07a7901 Merge pull request #70 from twiest/update_opshive
f2685009ec0a4c2ff74141657791835376a8489f Update sd-dev image links to the latest images.
fe1b28a9185506e0af7705352303971ac5d15c33 Merge pull request #69 from dgoodwin/joel-test
9507f9a78b4e2f8076ce7f3622fdc228bc7ba196 Temporary fix for installmanager tests.
a284ce0aaafdd708c8bd58000908eefc3e62aea4 cleanup before install
573ebea5ed75acae88fa8e7e8bcda98654a16f3f Merge pull request #63 from dgoodwin/deprovision-hacks
f2843591458e6f3173af79634852f3c8183d4d97 Add notes on troubleshooting uninstall.
fbeaebff58fce3af6371bae3a7bd6bbc8af79166 Merge pull request #61 from dgoodwin/installer-updates
85bcd78b9ee807115f1dea4bf17cb00a7fd81ee5 Move ClusterUUID from Status to Spec.
aeeb572514d68e5db476ad0c6d7b0fa474fa3f6a Minor code cleanup.
db6d497de269658096790667f1c300fb7288fde7 Add a test for install job cleanup on deprovision.
6b860d1caec1fe4344428bc8090bcc59eeeeb6d3 Fix for install manager tests.
f5927403e54467a28da0a969df18d8ffe78031a9 UUID test fixes.
bb53c13b307c1c518a9cb387c966652dcc23a82d Use hiveutil to deprovision without metadata file mounting.
d7b4a2e0609ff46dee4dd92bd504682906e47e44 Cleanup running install job on cluster deletion.
24905d7d3b91df48427516c57f27ac437b2b2443 Generate our own cluster UUIDs and provide to installer.
fadddb5eaa6c77cd8e6c4b5cba6462bbe6ccab38 Vendor latest installer master.
adf2edf820dfb8bb38658e4850bd3725e0ffb21b Fixes to begin installing from install config map.
8c7844d9b61c35f53bab561f5ce4d879fef86ec6 Merge pull request #62 from abhinavdahiya/elbv2
004e9e45c2affde0176c3362ac8ffd6c9f348dd0 awstagdeprovision: add support for deleting V2 LBs and LB Target groups
24817cc636930cbfc2becad7119dca4207c9158e Merge pull request #60 from dgoodwin/mockgen-readme
0850b878226ea988a7bed0448017a9dcdf262229 Add instructions to install mockgen to README.
ef6beb7b14eddb889a97cffc9d1a1d997da47ca7 Merge pull request #59 from twiest/add_remote_image
9edd2625ea3b5cb81451df553e0c1e0867a2dd7d Merge pull request #58 from joelddiaz/catch-pending-instances
a3e5816f6eead3ebab13b9e7016200adb1c5c7bc Add remote image support to OpenShift Template
2144b13ba32c1c453b618ff4d850ead99da8e0ea catch pending instances
c7fe8886596ef540dc4b820db30ab3e15c142a0f Merge pull request #57 from dgoodwin/deprov-logging
6e2c9decd6fce81b706667d367f6ba99640028ff Fix pointer logging in delete load balancers.
e7db09323ebf9b5d746a02ced945bd05525cf4e8 Merge pull request #43 from dgoodwin/install-config
560109bc15725b4443f9bae66718fd701e0260e9 Merge pull request #54 from joelddiaz/pvc-deletion
eaea2f1f735fac95be57ce94354bcf0971ac0c4a Convert ClusterDeployment to InstallConfig.
e629984f23a0a6bb1c09c45ee7771fd8f5329b79 Vendor openshift/installer for InstallConfig type we can serialize.
ac25d4918bf2b135bc3af590016cd05cdc85c728 Generate install config map again.
27bcd29ef8e0425ae3a29545eab94324459072cd Merge pull request #52 from wking/instance-pagination
2ffeaf5818139f4ede51c11133a4a2ee5bfa35e5 delete PVs
0089a8d1b661e1dae325a279412f9ad1f4507fee Merge pull request #47 from wking/or-tag-deletion
131112b928553bea6ba6530aea18ff1a199e4f86 Merge pull request #53 from dgoodwin/image-overrides
b3cb9302256a2c4219489dced68b9325c763c280 Add support for overriding the Hive/Installer image.
1cde39a21ef16eff8d39dc644720cfa1cb6449ee Merge pull request #51 from Miciah/awstagdeprovision-fix-bucket-name-in-debug-output
b1cad9871d6fb39c1f4a41cef710f5545e0edd0f contrib/pkg/awstagdeprovision: Allow for OR filters
d4b97563bae67a2e211ed41f2f0e71b5bd638e62 contrib/pkg/awstagdeprovision: Switch to DescribeInstancesPages
1d4988176bdd278c73ad9757bcfdc94b02cf0d3f awstagdeprovision: Fix bucket name in debug output
35b79981201c722ff95fceac41ef7d0d7b2b8271 Merge pull request #50 from twiest/add-remote-deploy
145286600a38dd3f152e88aef4583ce155be98ee Add `make deploy-sd-dev`
8e047f8c75eebf0ef411db0aba38d698c423f54e Merge pull request #42 from abutcher/requeue-after
4ddf95c6494b8c51e94ed9ea9884523b60f7ae53 Merge pull request #49 from dgoodwin/deploy-fixes
93af76b4fbd3dff24f6d2ae82f53f9fc2ea2ec2b Fix dev deploy.
5f1970a099d1426dc80ae3631c1997aa4e0c688f Merge pull request #48 from dgoodwin/install-mgr-tests
b4c91556d05277f10052f0dcf60aad22ac5b2f96 Patch to run from my temporary quay image.
5739a2d12e758ae301c19a7fa550d7fe2318f1db Deploy to openshift-hive namespace.
7c831db448d2a22e57f21670ccf810a08f7f45eb Use DeploymentConfig instead of StatefulSet.
97024afc46f7751fb0d71e2db8afae237f7cb6b8 Add happy path test for install manager.
a72a8866b6a06f8e8b87ac163d892393d3301281 Merge pull request #46 from wking/hiveutil-aws-deprovision-docs
2aa33ed09f89ef82e72645ebaac37f74c1209e13 Merge pull request #45 from wking/remove-move-command-from-deprovision-library
f20b81fa06ac17bc22096571d199cbfc8774fe5e Merge pull request #44 from wking/public-aws-filter
6e7bacc045eda07562b870e18f3809d8694c6c01 contrib/cmd/hiveutil/awstagdeprovision: Add long description
8de157dde0df018c4b24c33e50e91d0b48a02b1e contrib/pkg/awstagdeprovision: Move cobra code into the hiveutil command
553c02aeb6744a3e575e66bd840fc643cbb34915 contrib/pkg/awstagdeprovision: Make awsFilter a public AWSFilter
e852b08741e835f7233614687be07fc1f565f83f Requeue clusterdeployment with delete-after annotation.
26b3d5e640e0a756d27f788866c9f6c80e05fd38 Merge pull request #41 from dgoodwin/kube-1.11
25a591e4e83ff04211f288d0e736265985259e8d Drop kustomization patches no longer required with kube 1.11.
0da92f5dfb05c6f3229150a77e1d875b8a717a98 Vendor Kube 1.11 projects across the board.
4a6fd61ebc49fff490ae13120b24861549e20185 Merge pull request #40 from dgoodwin/deploy-in-cluster
f192fd685098f00a97e1b6d285ac449407dec230 Fixes for running controllers in-cluster.
afa5a5fd24702d7a1d087600e2f6206e6a7c8ae8 Merge pull request #37 from dgoodwin/artifact-ownerref
890a5b4f7150d9effe8d893070beccff3d2fc266 Merge pull request #38 from dgoodwin/8h-cleanup
4505ad450789e52a4621d53532afd15559c3bfb0 Merge pull request #39 from dgoodwin/golint-path
69b4f6998d42abe3ebbe85f5f7a4f9945c053f20 Fix golint gopath error that popped up today.
cf2e2b68a7ecf07f6ca7cd1f7ec6d84e37c6fa98 Automatically cleanup our test template clusters after 8h.
3e387f33659c81555a4a431ab5f8ccca232e8ae0 Hiveutil make target depends on generate.
1f84daf0884688ec0edeccf231c4ab6faf2a0893 Cleanup admin kubeconfig and metadata on cluster delete.
962bc373369d6401b8281bfd32ada5a0a82ae44a Fix bad admin password var name in template.
ee00d4f4d5d4d2eeae8ba0253f0a9b10cc8bf055 Add note on how to easily extract and use the admin kubeconfig.
90b357ee049bb866fffc6fa50ebed4ca7868df96 Merge pull request #36 from joelddiaz/lb-by-vpc
b17543739854b5a6efe7ad6ad75eb4c9c968f96e delete load balancers by VPC association
e9a26e0351b7016768cbe004c267ccc617ec93e1 Merge pull request #23 from joelddiaz/dnszone
e970d023fc28b46118735e10d0ecb8f346acb5ad Merge pull request #35 from abutcher/delete-after
c6d270944e3f0160d1b0909df7dd143aa1a5f5ba Port support for cluster delete-after annotation.
f7f992ab302850464da22a0abc15e1c5801351bc port dnszone controller
476ad1f52f5e45637582b0177b0a0fba3942267e Merge pull request #34 from csrwng/fix_permissions
8d4b5c369033800774a07f44706c7c0b33463aec Fix permissions for clusterdeployment controller
27c7e7ccc75d0aa32c528792050f48f7de759964 Merge pull request #33 from csrwng/controller_ut
2cc58ad42fc1c16e474af8c71f0d13a0d47a8d39 Add unit tests for clusterdeployment controller
7623d2ccebe3656f83dbfc91fbf9f6e0e253dd7a Merge pull request #32 from dgoodwin/install-sidecar
cd7113b8a71575e5afcaa9f2deb6bab6dc73fcd8 Upload cluster metadata after install.
2e49e132346fc42dc40135708039e8a69ace1b08 Merge pull request #31 from csrwng/uninstall
31d029dbc51186efda459c4069d809c508c66515 Generate uninstall job on clusterdeployment deletion
7b650f6de8f2185fa21aca9237c68a9aa8d86d61 Merge pull request #30 from csrwng/api_secrets
90a75a4e404fec966fdef2e4ba9b5ce48b0562a8 InstallConfig: use secret references instead of strings for ssh,adminpw,pull secret
6d6c4e9f6b00a970251c63ed821a0eb2aba873a7 Merge pull request #29 from csrwng/make_deploy
5db42f292a55638f818bc74393166c1dbf346594 Fix deploy target in Makefile
b0a8dbfc6ba65176d7f162242b03077ced50af4c Merge pull request #27 from csrwng/install_once
a050d77562a1ae37fc2358e047edef10623fc6f7 Merge pull request #28 from wking/tag-20-load-balancers-per-request
e49201c5832884a0c8d821ae1857d4764644cc2b awstagdeprovision: Tag 20 load balancers (max) per request
41846e89fea35612b47d89e1ff892615f6e7fc81 Merge pull request #26 from ironcladlou/empty-lb-fix
6314a2b0feb0214ed1d6275114219355307acc2e Fix load balancer deletion hang
615be24cb32fdc5c84d124c7e535011210e59615 Avoid installing a clusterdeployment more than once
6009b37520cd34b2c3e84b43a13a7de24589b013 Merge pull request #25 from csrwng/cd-install
9a0fa8ac13f6168d7289c4831d36685454f81acb Use new installer to run cluster install job
48aad420e14b94ef5c814c02e0891f870924df6e Merge pull request #24 from twiest/fix-make-fmt
af60d1cfa17fa55210a5c2e81fb6d356ffdb9898 Change 'make fmt' to be inline with 'make verify-format'
b4dea3b90af94bb295fc861446e29ede62fb744e Merge pull request #22 from joelddiaz/newline-docs
2789b85192821c8f2191f6b1f7863e301b99d96e don't let newlines sneak into the secret
51f9ceb4bdf66946492c0180b55cd0523e421710 Merge pull request #21 from csrwng/controller_cd
17305020cea3f2b917419cc82beb23a5e8bfe24c Modify clusterdeployment copy in controller reconcile
21ccbb916b60509563909178d6b089cffd01e323 Merge pull request #20 from twiest/fix-make-verify
7e7f82b1cf476110e7e7fd4ef5bb4cac1814f058 Move make verify dependencies down to targets
faa7917ab22c96e62f0ca1cb3ba90926d0ec08a0 Merge pull request #19 from twiest/fix-make-verify
9a32dfed3ebd3508e40cb14c4540a354ce5f3571 Fix make verify for CI.
58806efcc138811b7297fd4e0938cb406b9e11bb Merge pull request #18 from dgoodwin/testing
e58fa3bb189b87a62cad895595ef812e6cfac331 Fix test that was failing.
844b6889dff898848baea912c65982ea34c57866 Merge pull request #17 from dgoodwin/deprovision
4bf0b51637f7f6643ab39f80dfddb45e28cd415a Add comment on exported const.
6028d65e92ba668abef06efa21a37aab3f0236c0 Clarify development workflow.
714204145d7149392f5a6f686333635c997318d1 Add log level CLI param to the manager binary.
914829967829562025ef42b4b13c1c9f57a82062 Add deprovision finalizer and a mock uninstall job.
2905ed2549529bb890b6d397e7df9869ff5f7806 Merge pull request #15 from joelddiaz/kustomize
3adb68d465449e1142d3a1320b09ce20cc54a64c Merge pull request #13 from twiest/ci-changes
ae569e39af47bbd47b72d2c0b7c27094c0d05fc1 Add make verify target
296cb990171c6da62e134f3590c120bd16ef4d43 Merge pull request #11 from sallyom/delete-iam-no-instance
64c7b0011432767e660819953e1fbb5e4b8ec045 Delete IAM resources if associated instance is not running
b5faeca35686e68ed41f3185b47475b6cfb0b89a Merge pull request #14 from abhinavdahiya/master
6da6af1ae21cbf7e14514717692ce41727e5908f kustomize isn't liking the wildcards
32cde50fd32ec040fbd18fc671f6309dd3574f48 aws_tag_deprovision: continue on s3tag fetch
9fa92023d09f1800822b6f972e55f598b60b7faa Merge pull request #9 from joelddiaz/hiveutil-verify-imports
3149f2357c8d97809dee2dea3947f57d7b6535df bring import verification naming validation into hiveutil
82e3f1779ca55866cf53998d58b58814b35b7836 Merge pull request #12 from dgoodwin/installed-status
17e778e58fb13da5665a4fd00fdcbdc2898147a4 Merge pull request #10 from twiest/ci-changes
888539014700f019d972b28e7a8630fd23457255 Change Hive repo to be compatible w/ OpenShift CI.
590c671f0c305015cefb1409be23d2bbc8595920 Get a basic unit test operational.
9b130f17ec7dddb95c758d94ab0070a36ee8eacc Set installed status when job completes.
cf38689aa19d1e1e2598249cb1cc121e15f025e2 Merge pull request #8 from joelddiaz/hiveutil
ca98a4fd079b124bf2d14dc262c09a6ba1afb2f8 add initial hiveutil
efc39c681595e00edef758f4295dc265b115d4d2 Merge pull request #7 from joelddiaz/aws-sdk-go-import
e586ead5ebc8d18b36e4b31b178be5adc80ed000 import aws-sdk-go (for upcoming hiveutil)
b9a735809cd7ba218bcc6d4172695675e8ff5445 Merge pull request #6 from twiest/ci-changes
20e7414e997e1a4fd144a7d94a958cf6620639df Change Hive repo to work with ci.
eaed394bad108e31193bf06890b921898c7e5154 Merge pull request #4 from dgoodwin/creds-secret
b8e83d73c3942a237836e61d352465724b479a8a Merge pull request #5 from dgoodwin/yaml-json-tags
615c00dccff485e9dfd15c879d2d814bee09cac7 Use a yaml library that respects json tags.
c68743eccd65240fc49020c1f200ce4839c7a5a6 Add secret for AWS credentials.
8a08c4323cb2776c23ce3bda1cf1a48093cf9446 Merge pull request #3 from dgoodwin/write-install-config
e37b7d5b7a9f21abdc072386e564ceaad9db9bbb Generate a ConfigMap with an installer InstallConfig and mount in.
767042e4cfefb6a27dbea5e69b1329a63987883e Merge pull request #1 from csrwng/add_owners
a1ad22091816a2600da1859fff9cf7553eb56c45 Merge pull request #2 from dgoodwin/dummy-job
d9f69491ed3df31865cf221ee6f775846900257a Spawn a dummy job for ClusterDeployments.
fd42ba1fa86fae12a8c6ddde3158fd700edaaeda Add note on creating the ClusterDeployment CRD.
88ebffb7b6968d200d78fa0d00f4ab31858e7692 Copy in InstallConfig types.
934f6842dfb90fb60adb5489bfa5c736daad7ffb Add template to create ClusterDeployment.
c5f79497296a9e7284d62155dc342e29e0ff737a Add initial ClusterDeployment based on InstallConfig.
0aad542ca89e23933eaf62c4fd656669fd83e392 Add OWNERS
3d040c154a204edd34b0f6e264cb5c46842b5d3d Use logrus for logging.
ae457a1a011118c7517ce85ba3b3e1c0d10e1ffa Fix dep updates by pinning to k8s 1.10.1.
93ac39c9c1815fa71750775d3fed4cdea3ecd3dd Initial repository generation with Kubebuilder
9c56c62c6d0180c27e1cc9cf195f4bbfd7a617dd Initial commit
```

Status: Fast-forwarded successfully.
