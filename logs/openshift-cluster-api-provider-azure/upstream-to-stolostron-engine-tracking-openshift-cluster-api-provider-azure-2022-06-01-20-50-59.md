## Fast foarding of openshift/cluster-api-provider-azure into stolostron-engine/tracking-openshift-cluster-api-provider-azure.

## Status Summary:

release-1.2 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-1.2 -> backplane-2.0:

New commits (first branch sync):

```
07fbd76dbd7945edb2ef8af968d4693d6dff35f2 Merge pull request #2133 from CecileRobertMichon/cleanup-go-install
7f605d5f9c307abd2df42b332fead8e555d073ab Merge pull request #2131 from jsturtevant/patch-1
8a619115b11d25681f1aab6daa279fd3202e4dfd Merge pull request #2093 from Jont828/ready-conditions
28fa9314c2f89055d54f324aa59072752fe293f4 Cleanup go install script
f3d40739b2113cb95aa0dbec65b0c5fa745c722e Use git to clone the repo
1278516765c1875025a48ab112320cb2d0bfdc62 Only show applicable conditions for AzureClusters and AzureMachines
6a9300696954b36e032c26356d85bbb7487f32b5 Merge pull request #2122 from CecileRobertMichon/errors-scope
c444fdb66713b580ebc65ea8ce4436715358bf78 Merge pull request #2115 from jackfrancis/rm-suffixes
ba4298ebad275a9559cfd7a37b0aa9d0f0e3bc5b Don't use error.Errorf in controllers to avoid showing stack traces in logs
613f40aa662a854a413ff78add894cdd9ac2ef6a Merge pull request #2087 from lzhecheng/ci-dump-pod-describe
dedfde30fa023074b83a4e1d8a2adb3ca0ebb1d0 Merge pull request #2117 from shysank/azureclustertemplate_bug_fixes
0d0a088295aa18647a4baea9b08e90f8ee370478 Merge pull request #2100 from jackfrancis/test-required-optional-experimental
5389eb7a38c9629230331194e9d8565468c4cdc0 dont return error if there are no validation errors
9cb75add632ea040c47b5d845e7f39e6ef7be269 fix kubebuilder annotation for azureclustertemplate
c5a07d2d96c036ea67f6f16131eca4c67ea80b41 use api server lb pointer for default
ada8e2b424353f69365d6429e4eec328bcedbbe9 Merge pull request #2109 from mboersma/bump-otel-returns
6765dbe0968bdce52a07d35ec25a127da65608d3 test cluster flavors: required, optional, experimental
fb031f0b7f8b251410cb3b0112349ff139d1652c Merge pull request #2111 from fiunchinho/roleassignment-machinetemplate
51b21173b60cd8c1f181be2c8648c52e7651c381 Don't default RoleAssignmentName on machine templates
0af59a957a98afdb6a0f0ce06c3e746082b482c1 Dump Pod events for CI
04012c51df9e47a74fef2dfc31fb9ec38a3daf70 remove redundant VMSS name substring suffix
083952e6df58777c5fd0bb2bddc18dbef447e011 Merge pull request #2113 from bridgetkromhout/version-support
e98c78207ff26bf6f91fcf1f6df62b9ae1aeadee Update opentelemetry-go to v1.4.0
935ab1d628a536a94b96c767bc61490cd62d76d3 Merge pull request #2072 from ykakarap/clusterclass-support
b37fc68c76c045993c5b30e00a1b2afe874e1b81 Merge pull request #2020 from michalno1/main
52903354697fd1ef75a202fb775c94d63830a50d Change version skew listing to a link to CAPI docs
c0416bcec595bb7b4d21b06ccf4d30f560341d1a passing custom headers to cluster and node pool create/update requests
4b70fae251a26a8ff1cc7cde82a56c52e3826aa7 Merge pull request #2061 from sonasingh46/system-assigned-identity-template
a4f54cc458d2a7d7d7ea6871e5e6cb71072f9757 Merge pull request #2099 from jackfrancis/aks-test-rm-timesync
0f80cb796b5ee640eb192783424cec61d03563ad Merge pull request #2108 from zmalik/zm/fix-e2e-exp
1f385682b9ef929a29ff0e56b94604e883d642cb use kubernetes 1.22 for e2e exp
4fa6e63ca9fc50fc8bc247cd650a6a2c9b49b8c3 Merge pull request #2008 from jayesh-srivastava/go-install
2d1e011f3bfbad325c7bfc20f89b9952267768a4 Merge pull request #2106 from jsturtevant/deprecate-dockershim-clusters
c5f88ede8e10556dee727db945b0d4e5cda267fe :warning: Windows Clusters & dockershim deprecated
99a589cef3e119ff7cbf890e9514da5309965dba Add AzureClusterTemplate
795082c26b296f22563621e6136537ec101f2281 Merge pull request #2098 from CecileRobertMichon/rm-master-taints
e5063d146e8801a33b33bb260e2cd7a5bd1f4964 Merge pull request #2085 from jackfrancis/ampm-delete-already-deleted
5d309d0a484f6702a5f538f27ebe638dc6efcbdc Bump CAPI version to v1.1.2
57f758e09ba4facd233af09020cb24e8edafd9b3 Add control-plane NoSchedule tolerations on calico deployments
47f13d90741c01e766bc3b7d01f082dedabc74cc Update make targets to grep control plane role
7f79c57b9f0695e02e5c5eb4b84b7eb0f16f8a1f Add node-role.kubernetes.io/control-plane tolerations and taints
23568a751aac1b25eb26b90bdede4c33974f6064 fix(templates): add identity ref patch to kustomize
658d43d699550e833e6121dcf9beebdbc60521f3 Merge pull request #2101 from jackfrancis/fix-image-pre-release
08fbaf6c98489f310e20f601043704a8b00896a9 Merge pull request #2097 from jackfrancis/rm-windows-vmss-dockershim-test
f7fd1995ddb5b40b62ce735468d59253e032e03d Merge pull request #2065 from alvaroaleman/set-internal-dns
189251e83ba77ee9ad2c286581536e7cfda5ea22 don’t check pre-release versions against known capi images
b97fbf54f0b919e42f3c21eba7f0f12897623883 Merge pull request #2075 from nawazkh/nhk/2073
f21b351d40d599206403a60dd90bfcdfaa7a5524 don’t validate AKS timesync during capz E2E
e68590fe6d815966b1b38153caf25a0f23cc7579 remove Windows dockershim MachinePool CI config
7b8db727ac4bc4b2b81696aea95e0cee98ce59b8 Merge pull request #1930 from zmalik/zm/add-aks-taints
fd485505c167beb2b07c8028a1b67967aacb328c AzureMachinePoolMachine: track concurrent deletes
fdb1d4375de9a1aaea58d3820ac1849c3fb36bba Merge pull request #2091 from jayesh-srivastava/kustomize-version
519369cbcd5c2ebff11acc2376c4952faf1de92a Merge pull request #2090 from CecileRobertMichon/fix-apiversion-upgrade
b2c000d2c11ae679dc2f60ddc598db3a902eca0b Merge pull request #2082 from CecileRobertMichon/release-action-tag
d8cf2825f7a92692fdaf97ac1c8a2be900e8dc7b Merge pull request #2060 from nawazkh/nhk/1789
3fab667c64b6268a935ceb9d6bb2a2160f6e03b4 Merge pull request #2050 from sayantani11/issue1973
ac9aeff16c7b4b248fd3e5037ac1e2a8de988574 improve formatted output of `make` or `make help`
94d929a2e47e740f5cd21e4aa1f4d522cb4f77f2 Merge pull request #2077 from sonasingh46/rbac_patch
5e848fb39b1627186883815c6fa30f03f881ce5f Merge pull request #2066 from alvaroaleman/inboundnatrules
55e72bd0db4ee23f870560160c91a4b2cf3a6e53 refactor annotation name constants from api/v1beta1/tags.go
136bab82543bc3bebb18542e2efde7d496f68a7a Update kustomize to v4.5.2
f011ea9c7d720ba07140365758dba15661fb1141 Bump CAPI init with binary version for v1alpha4 upgrade test
17be7481ed93084ec48594ae71941bb53488b827 add taints to AzureManagedMachinePool
4176bc865386dafc8d42715fc063504d44e7fe82 Handle terminal errors in AzureCluster controller
0a254d897968cea9a5031ff399261fc647efecc8 Merge pull request #2023 from alvaroaleman/external
4ab25455f0e7e646dda19db319bc05b17c32783c :sparkling: Set InternalDNS address on machines
740b60d21d23a4ae6c6c328453012b6dca8834a9 Merge pull request #2070 from viniciussaturnino/gocritic_linter
974d172fbdd6bba7bc4f2ffdeb0e89d9515f5e75 Update book release instructions for 1.x releases
a3c28efbf1598ef83f20b9bb1454dee334e5595a :bug: Skip InboundNatRule reconciliation if no LB is configured
0cfa523d5982541e5f0323c3f779567dd0fda8c7 Properly respect externally managed annotation
f6afaf78c739b78cfd34421105128cbd7f21d20c Merge pull request #2074 from thiagompc/fix-ammp-controller
47e99102c5562f9bae8b1fb0c663bed68b96ac91 refactor(golangci-lint): refactor ci errors
e9f6fa328eb72dbd0d064a18171ec07e823409d6 fix(rbac): add namespace list permission
38207150d20e534ff15899fb049304962b7ecccc Merge pull request #2044 from Matheusafonsouza/thelper_linter
2f4bb99afbfc5da9db71102d7cbd7c01d076c913 correct variable in SetupWithManager function in ammp controller
6e20db5c6efda470bc01c910ac76f78a9af95df8 Merge pull request #2012 from marosset/windows-csi-proxy
d9fc4b92c96593a31dc0b24102a808c2f7c2ed0d chore(golangci-lint): add gocritic linter
71f1710f119c9a74405a33e07d8eca8acde72fa2 Merge pull request #2064 from jsturtevant/calico-fix
7c2b6ab3688eea0cfed220a99a63399ed2c445c3 drop aws disable flag so pod goes ready
461953afa296c1e3e630f4ca36f1a80100a80b87 Merge pull request #1914 from Jont828/async-subnets
cedbd76c330ddb2fdf1add22634812d559e3c5fe chore(golangci-lint): add thelper linter
6861356c1a5c0900c5d17f0822a5980329f5fdc7 Merge pull request #2021 from CecileRobertMichon/calico-from-source
3ead4407ea7d48535a429d433d15093566f53df6 Merge pull request #1963 from Jont828/useragent
5522fe7a76c40eda32cb19d956edf9dc2991b5e7 Merge pull request #2056 from mboersma/cleanup-conversions
52f8f9d08fb5286f682393195391149d6dce28a2 Installing csi-proxy in some windows clusters Adding csi-proxy to windows-containerd dev template Moving csi-proxy addon to cluster-template-prow.yaml since that is what azure-disk/file tests use in CI
0dce5e5dbaf12d8429d18747ea8a379083ed7ccc Clean up resource conversion code
c3369a3f02ad557f0e39cc838ab540bf41dca370 Merge pull request #2055 from CecileRobertMichon/capi-v0.4.7
d8a4b622a029df94e7fe01315717f3aceba57192 Add version info to Tilt
d9768415981f6af7e26ac0b0bb218d7ad28c4bb4 Update CAPI upgrade test v1alpha4 version to v0.4.7
2cd76844f29cd942988e6ffefe8a329474ba8a30 Merge pull request #1988 from sonasingh46/predeclared_linter
e5ff73c3b62c5e7af2e73e0ca6c33a8bc6929416 Merge pull request #2032 from sonasingh46/verify-targets
87aee457735cdf6eb256cb2f5e55e78c38f758f9 Merge pull request #2053 from richardcase/tilt_debug_docs
bf284b9c5ab427702f09e275b65473784b7182bb Merge pull request #2049 from mboersma/bump-otel
a16ce1cb47d838991b07bede7bb3741ae179f59d Merge pull request #2043 from marosset/windows-logs-ci-entrypoint
d3788df51d505646d0a85c4c5c548d09adbfa456 Merge pull request #2034 from CecileRobertMichon/add-jsturtevant-reviewers
2a705e9e30dc2dfb040b6ca6b85018dc45b389bd Bump calico to v1.20.4
09793924ea25a915a61d212719ff26ac58f54c6e Generate calico templates from source
7e44c2970fe78ba83da0b6a1fe061c8faf88b28b Merge pull request #2018 from jackfrancis/template-cleanup
f4daf4bc717277687c8e4fa37d48bf5d4632b442 Make subnet reconcile/delete async
4db30b433d5b46c9ddc15b6371ef0fff382381be docs: debugging information added
10723030e57d15136ff9618dfce077279a4855a1 add apidiff and verify tilt make target
15704acddd7475628583ffc73c5f8525bbcecd81 Adding logic to get pod logs form windows nodes during ci-entrypoint.sh
889ea8c3961499043e915fa91e20907e312e2acf Merge pull request #1943 from shysank/azurecluster_refactor
1f47719a48f0999b4bf4338ad0c87540f3fefb98 Merge pull request #2042 from sonasingh46/verify-conversions
7271929ede365e753bf2d53bf40b6db004bf2cef chore(golangci-lint): add predeclared linter
c19ce90cca468a100c9576a3bdcbbbc8a095f8ac Name AzureIdentityController so it doesn't log as AzureCluster controller
309442d6ad894f78124f04b19c8a805b04bcbe8d Add jsturtevant to reviewers
9940f373b680141638477e22a9ae125cce4e3841 Merge pull request #2046 from alexander-demichev/gitignore
1e5a77990bcaa25daa9fd476e532cf39fa768ad1 Merge pull request #2035 from CecileRobertMichon/add-jackfranci-reviewers
760cd9a2a8d277463e9782d2ecbb16efdb725f06 Update opentelemetry-go to v1.3.0
d6850cd13bc24e7950ad6b3821f27fc66732afd0 Merge pull request #2048 from jackfrancis/disable-security-scan-job
f43070363aede6db81a28e7107764281fc56964c don't fail E2E on security scan failures
4c8a39603e4678ae76302d181e8caa78638896cf Don't ignore kubeconfig directory in git
76aab6a96002e4b5c9e601e559a7b387b0a76ea3 update v1alpha4 to v1beta1 conversion with embedded types
8ee1fdd969362f2929da46fb317a9eecde77dc5b update v1alpha3 to v1beta1 conversion with embedded types
d18fc7eadd2fff27ab4b13b157303faf20b67f77 update azure cluster refereces with embedded types
5d49003535618075e49679f6b76216488f6f9859 refactor azure cluster types to separate out fields shared by multiple azure clusters
b03cb7bd341114d46ad98b8b1b9fd10c8ce8ecf5 add verify-conversions target
04cba2231eb8cc472fc2f89e96fd2fb1912f0551 Wait for Windows nodes (if any) in ci-entrpoint.sh
1cc4c2d84feff6a7d2749125f87ade26f6a973e6 Merge pull request #1987 from sonasingh46/gci_linter
78f210446ee3a4df2acccb8e1db29a1b6fc86100 remove machinepool-specific test templates
bd23e2f9b924d8b145bd7daea571ea138e2ba1c4 chore(golangci-lint): add gci linter and lint fix make target
f6ac019929d04b465d969a2f69d59759d8122b57 Merge pull request #2014 from CecileRobertMichon/bump-capi
4eda00a749fe79c1103b0c9b882e781bb5e6550d Bump k8s upgrade to version to 1.23
0d590008ba9a1ef28b86bb39ecb082a1d9b7d825 Update KCP upgrade tests to use worker count 0
8979e696adfe000179e459a034beb7dbfb6bc473 Update CAPI to v1.1.0
e97e7b75eca63e1c8e6ebb2095afad4804c0e644 Merge pull request #1927 from zmalik/zm/add-aks-labels
ab85f9532e3b8157a27417c6d91938eaf4589af0 Merge pull request #2033 from alexeldeib/ace/paid
9897e1940acc0e1600f5d7b1bf7028791541202b Add jackfrancis to reviewers
6eed2d150e99924efa3c91ff874127f16b7b29f8 fix: docs for aks sku tier
7979a9705adabde2085801b04f87ad00e8888e1e Merge pull request #2016 from jsturtevant/revert-image-gallery
fc9a60fe76102db877491c4840c889fde8508c95 Merge pull request #2024 from CecileRobertMichon/fix-404-doc
a38d26a5446ace02b1cc6efbe7796c5b9c66b968 Merge pull request #1921 from CecileRobertMichon/async-vnet-2
5c96e824f739bc8627cab4017312e2054d329d63 Merge pull request #2025 from zmalik/zm/test-fix-tag-match
a4a800aa2ca542e4a3c4d12e8d7e1cd8248cbc5b use aks-managed-poolName also for vmss match
424e94f6083e557f79d1e882fc7274aa7e98534b Remove failure domains dead link in docs
dc0c3fad698c7c788ae5a14cfbb8c3c94180f97b Merge pull request #1995 from CecileRobertMichon/fix-latest-patch-e2e
cd672901fe06d036f183c612c0af713395d1d18f Merge pull request #2001 from Jont828/bastion-role
1535f203daf3a21c71f4a6dcb9483e47871eed39 Use updated images
e2abea2a0139ff9f8fd5e55dccc31a06208088e2 Merge pull request #2022 from alexeldeib/ace/docfix
a589f9dd2d9edf60e51aebeeb7a90a90f3ffae39 fix: remove sub id from azure managed cluster docs
021814e233fa3b83fabf87d8db7d13ec5fa1c2dc Add Getter interface for getting resources in other services
a03b9e2ed38833e70a0d1e42791a34d6198299ac Make vnets reconcile/delete async
e75d79fb7ddd20e0dd6d7bbe28cfb33bfc834253 Merge pull request #2006 from CecileRobertMichon/wait-for-service
6cc55e0cf3d476f9ecdb273920c863db87e0d911 Merge pull request #2015 from mboersma/update-nvidia-gpu-operator
8a502424bdc7d51204a942dd1934ebb6ea9152c9 Merge pull request #2010 from jsturtevant/kubelet-logs
47e3eb474492b790fc643b4eae86d1db501fde06 Add enum validation for subnet roles and a role for bastion subnets
ba163a2dfdcb2d6b52ebc3bbb7b5e6e2d13faabb add support for aks node labels
b5c7a99f435ff907fd9bab3e993dc0db439fe329 Merge pull request #1793 from mboersma/kubescape-e2e
be61a966f19b4cb6b7f8431ed6d748b0660b692c Update nvidia GPU operator to v1.9.1
d41727fe7786b4ff4ba8618b5a353780826bb124 Merge pull request #2011 from CecileRobertMichon/custom-vnet-template-rt
1bb3cfaffaec7b99a3c47e2291b9b3acba564fb5 Update docs on custom vnet creation
f2a9ed8c3a8fbcc7f21fbba154728b1639d176c7 Increase wait for service timeout
c6aef0bea3157a581a4fe164dc4a5de6aeb74725 Merge pull request #1976 from zmalik/zm/unify-agentpool-spec
c4064ec43e554d0979eee47bb256fac469257895 Fix the custom vnet test template to provide the route table and nsg names
6e63e7918442fa735cfefcee0a8e69e51840de6c Revert "Use a image gallery for faster updates"
364e0f0a9d4d4a50491e8be5e05287bdfd022165 Capture NSSM log output files
450e2d9de841a162ea44b5f6f714bf483f4e96ee e2e: Use the intersection of images available for windows and ubuntu to determine latest patch
a8555bbe56ce398efdd984906f059abef8e89d00 Merge pull request #1986 from sonasingh46/ifshort_linter
20b28c1aebe6c3dc7993578a719f05cb2069e31e Replaced `go get` with `go install`
9260653ffcd61e2407e56c9454e3a1c14785a359 aks agentpool spec through one method
53ede26b61da686b30f37639bbfda7e23968e38e chore(golangci-lint): add ifshort linter
bc44584aa2c2ff6bd1612e5671f4c2f6c4a8a3b0 Merge pull request #1999 from jackfrancis/cloud-provider-azure-versions
3f465753f23ad9f8a3242edc6ed8bf8e3a1ba15d Merge pull request #1950 from CecileRobertMichon/aad-pod-identity-1.8.6
d3fefd2e6ec4e3e81757ec032bf7e86d0009a9d2 Merge pull request #1985 from sonasingh46/unparam_linter
7e356ef434f70e47125af73af43b205a02a60241 Update AAD Pod Identity to v1.8.6
b6803209b50b6473c4e12c22644b8484fbf1944b Merge pull request #2003 from CecileRobertMichon/use-privatedns-api-version
fee74172efc0db07a244ceb870be759db56e0f83 Merge pull request #1951 from CecileRobertMichon/update-controller-runtime
6ed6b0593a30a72faee09d31522a72aa090092e5 Update private cluster cleanup to use the right API version for private DNS
06ada5b6c122af1b614f545c7db18fce900f0464 Merge pull request #1993 from jsturtevant/windows-ci-updates
171b34c671a21ef224e8525d89dacacae49163fe Merge pull request #1941 from Jont828/async-bastionhosts
de4ed4be04a1577c2e526740466f5566fba646c0 use latest k8s 1.22 (v1.1.5) cloud-provider-azure version
791672537afcf5c9c59c9da8771ce01c677b1c0b Make bastion hosts reconcile/delete async
1679861fce941d2444309b41337900e474b4df21 Merge pull request #1939 from Jont828/async-networkinterfaces
107468d8fa1bca64e94b9609e2b3393fbd807f3d Make network interface reconcile/delete async
1e16c703ef7d26b234984afbd57acf706b3e0473 Use a image gallery for faster updates
e7c37cc98b284e5b416895ce98543de70d676a64 Merge pull request #1992 from dlipovetsky/book-aks-patch-version-warning
4305550de3223b2434989f1bd74a9950a38b874d Merge pull request #1886 from Jont828/async-loadbalancers
d9630be8813260f539b4da7270592deee6e3eb9d book: Warn about AKS-specific Kubernetes version requirements
e958b3df62ce9517df1f07b593e9c39d0b41d218 Make load balancer reconcile/delete async
8f3d3bf4a36c00a9488ebbfafcced10a275623b3 Merge pull request #1996 from CecileRobertMichon/disable-stable
b2b3139d734f9ef84b622fea5a50cc18c7006051 Disable latest stable k8s version in e2e
0d6102adc3e32fcafcc5483718fb80aca724fae1 chore(golangci-lint): add unparam linter
893af0c91d95d121cd97e5dbc44380b5c06e2e2d Merge pull request #1984 from zmalik/zm/bump-kubebuilder-1.20
3b48466923f0ad027045ca5d81e760eaa6217c3f Add CAPZ v1.2 to metadata artifact
54fd54f1bd9920e72479c3c16cd176b058adefdd Deprecate KCPUpgradeSpec in favor of ClusterUpgradeConformanceSpec
f4a255b3b1680843ebd4e556f81feab363e19e43 Update go-logr/logr to v1
d2ba539b5fdd10a0e9020931d275678eeee64f8e bump kubebuilder-tools to 1.20.2
2bb771b1f965766182ce2dea19256468f7116fd2 Merge pull request #1978 from dmlb2000/fix-1977-make-controlplaneendpoint-settable
560bb19b5e9fc0b8eab335ac7b933beab9d575c3 Set Control Plane Endpoint Optionally
e123e78fcee9a9bb214999deb8c35fc6f1bffba4 Merge pull request #1916 from jackfrancis/aks-osdisktype
9f597df9dfb51027df62355bd52f0229e81a7fa1 add OSDiskType configuration for AKS node pools
7984078390c754239de792d5038a16d0230f3b9b Merge pull request #1971 from zmalik/zm/fix-test-managed-e2e
10ea3e929fb945721f8aa90bda72b1a1d228c8ca Update CAPI to v1.1.0-beta.1, controller-runtime to v0.11.0, k8s to v0.23.0
c26c92c1bae2b2f80a6c5db113569602e0db80b5 Merge pull request #1870 from Jont828/async-inboundnatrules
e6f168822214d2bc1524f0445083d13e2e4d626a fix managed clusters e2e tests
8bd2880375347c7abfe49f274ed23e7e83c74e40 Make inbound NAT rules reconcile/delete async
36c78d3cd955419a5a8cdbc83e5ae2e01346412a Merge pull request #1962 from mainred/fix-capz-docker-buildx-push-issue
ecb256236f2f0913e1a3a871eb24f3de3cc630a4 Merge pull request #1932 from jsturtevant/deflake-upstream
3b93b529515259f541fa45496005787a02876cf4 use dockder login as a workaround for capz acr
42cbf864a2de33b6cd1dcb51cf2ee39fa2cc7e95 Merge pull request #1686 from CecileRobertMichon/async-routetables
7c6da6122e503acfc5c50e435212c49c039c075f Run the kubescape security scanner in e2e tests
229f4257ec089032c960f28a957d5b0e99cee2f8 Use named returns in async clients
9a5c20a973ca3930dc47dbc9f9e2179c37a671a8 Make route tables reconcile/delete async
d29299c253e8d9ffbbd021690e54fd49ea45ae62 Merge pull request #1955 from jsturtevant/nightly-containerd
e109215d9304b516ba8a7dc9ff2bd663bb83bfcf Enable using custom Windows containerd in CI
cbe3bad2d79699ba6ce686c845a86e360cd0bb8f Add calico-ipam to exclusion
9847e977b7b73835878e46eecfa77b0881f97a36 Add pre-pull flag to e2e.test for windows
e271b8102444fd8e2a0112c30f3f67a980144fe4 Set Windows kubelet priority to above normal
b42e11e3e4b7f52e5f0785a7ed1644c7244d76b5 Add cni binary log
26008d9bc658b24955d643893924175ad6da5ef5 Update log verbosity and collection
01fd30a416d34dddbd54277ed8e9448274393a46 Enabled logging of Windows containerd
dc1c2de15e74999f3013231e96d31e241dbdccf8 Dump namespace logs on failure
8b84cd7aaa0e4a3150dd4c9e29dfe73a6aa0c0d2 Revert "Temp: fix auto update"
6362201603fb5e8645c5099a6bf667fca1b711a3 Update to use newer image
9afe3ada64f114c1281ca74911daf9f4a80ba4e4 Merge pull request #1940 from CecileRobertMichon/managedcluster-conditions
c55ae7b4eae2502e8c5eeec494c5df00920a61cb Upgrade Go version to 1.17
c507e7d47c04d296d8cf2cea8f9b2593eddf2b14 Merge pull request #1956 from CecileRobertMichon/update-generators
b622b7b05a3138c1becc5e22134d0184256f970d Update controller tools to v0.8.0 and conversion gen to v1.23.1
651a278931733facb9ce72e1886dff88fa0d6162 Merge pull request #1945 from zmalik/zm/fix-max-pods
fdae34a56188983f7dc6acdc01e213c1c18c5315 Merge pull request #1953 from jsturtevant/temp-move-gc-tests
de0d848ec6aea977c9c6b497f9ec27e6b60b23ba Move the GC tests to serial to temporarily
0fff41063a556648adcf6d24bf11f4409a1c3bb7 Merge pull request #1936 from CecileRobertMichon/kubectl-tilt
571f88a794cb197d3b07aad9a959a6a7d2fbe57b Merge pull request #1938 from mboersma/update-gpu-operator
1a43a68a3dd256f2a6468cf39d2b38bc9a8392b8 Merge pull request #1948 from dmlb2000/fix-1947-add-validation-docs
8ee0f669eb5d7be6ccfb3dd7813fed5e55d930c6 Add ManualServicePrincipal to validation string
641a1daefab5dc86b7066d0f2fa8b7f7a1cfe03b Add conditions to AzureManagedControlPlanes and AzureManagedMachinePools
a5b7ea87a85fc5e328d0d6f7d91e3ba0e3624df1 Merge pull request #1931 from CecileRobertMichon/fix-cache-error
76a8067bd4760c31e9309c28382fd3e038121000 Fetch latest Nvidia GPU operator chart with a script
365b5d050e190899259af8833e6ac6d24a2b0840 Return terminal error only when the SKU is not found when getting the SKU from cache
47ead2a504fc0165035e9e8c020b54d7422d9b87 Merge pull request #1933 from CecileRobertMichon/fix-extra-string
afaee522c313f129cce5a420f7fed09baa9bef47 fix max pods for the first nodepools
57d4c38d9beb316d7b1bea4bbef9b490d8922eca Merge pull request #1934 from CecileRobertMichon/transient-error-print
29a69e762c4705b2f20465c17d70bb1ec83e6d24 Merge pull request #1896 from zmalik/zm/control-plane-only
f049cc8ac53abdbbdd83ec6fe07d563b89c3707c Use hack/tools kubectl in Tiltfile
2eb34cf6a854623ee94a977b13a4a8d4e08f42b3 Print reconcile transient errors in logs
8c87782f64306aaa3c225a9f99f368eee146e701 Fix extra string in log statement in e2e test suite
631b1d97b2de2c39d7e5fbfd8d16cd8fda926ccc Merge pull request #1926 from CecileRobertMichon/yq-install
c39331be0d6f5b3a14d90c7f5e8bff9e4cb80994 Merge pull request #1928 from CecileRobertMichon/fix-metadata
58ac05e9075a1e5e4bca303e66d4b0db5593a00c Add release 1.1 to the metadata file
46975f636fae954f1a31ab6bb6796821f047ef8f Fix yq install in get-project-maintainers script
fff537114ca8348c65484cc5f5ef551f2851f2db Merge pull request #1922 from mboersma/fix-gpu-e2e
330ab44fea9d748a448395b209b5cb550cda649a Update NVIDIA GPU operator componentry
28fc0001bcca07033455d2080c6cb95398bba811 Merge pull request #1924 from Jont828/availabilityset-ready
58f7f829ca928dd67cbf92a0c78255c7399890ac Merge pull request #1923 from jackfrancis/update-ccm
d352e7c6ea47974d8ec7c858cb76dea7e9d3ecc3 Merge pull request #1865 from Jont828/async-natgateways
96015fd4bc529df817ccedb821d22aed49e828b1 Add availability set ready condition
154bf954db99a13e764701881e74a896be86520d Make NAT gateway reconcile/delete async
08c61a5eb3808cdf0c146a42b3794259bdb2c18d update external cloud-provider-azure versions
ff49c7a73034ec157340d0e0dbe19e7bca18d169 Merge pull request #1861 from Jont828/async-availabilitysets
020a2b654ba78a3cf5d1a4422a2cc22f8557e40b Make availability set reconcile/delete async
f49dc680b71ae4fb9ace6ed6acba2430b027d606 Merge pull request #1920 from jackfrancis/validate-max-pods-typed-error
7f45b09822fa0309026fd3d1f8f500b7458c5145 use api-machinery-typed Error for MaxPods validation
7a6f478d3cc9ec82b607df7080d1e28377f38bb8 Merge pull request #1881 from jsturtevant/add-windows-serial
ac7e9c1ad4d95a2b8cd60f30b4ab14df9d163209 separate AKS control-plane and agentpool versions
3e0a1a9d7f3c7c193851873f13c8e86a586bbb81 Temp: fix auto update
6c40a607aca6dc22eb5e2de48ca61adc6a14bfb2 Add HPAContainerMetrics feature flag
8b5fafd4fa47f5c5d96562fa0caf0c919804fae0 support running serial/slow jobs
92dcd55c2b9c19f3e37e04f7550a7a30ef986571 Merge pull request #1791 from sonasingh46/byo_dns
d0605831a48a551f1292b21c1c6a3a1bdbec8fc5 chore(private_dns): tag dns zone and delete only if owned
2b4a27e4d98cc2edfc4215c42804d6f1b3e6357d Merge pull request #1903 from jsturtevant/add-metrics-server-to-ci
67143919970f0cc0d17b3cc2c8741c6a8ddacaeb Merge pull request #1915 from jackfrancis/fix-maxpods-optional
19e7cb6389230096f57ed26073009577af1d4afb fix: MaxPods is an optional AzureManagedMachinePool configuration
e01076c1b8781fc8bafc6ae174859eafce2bfe14 Merge pull request #1912 from mboersma/bump-otel
a20197f88ed28205ada5e2018e0bdc789cf1b8ca Merge pull request #1910 from jackfrancis/aks-max-pods
36863580e6441e30c92ebfc602452dd3e8738aa4 add MaxPods configuration for AKS node pools
1b2d4f86ced53386a7529ae7b5e6cd6b42605001 Merge pull request #1906 from nilo19/chore/tag
0093c773718c6b7999b24893ebe2e4d83da4c104 Use insecure setting for metric server in e2e tests
7215edb4902eb229c26a42ef0893a34968ab6595 Add metric server as addon to k8s CI
26b3a43dcfd794c60bbe3736cddfd6ff09be7d70 Merge pull request #1911 from cpanato/update-capi
f2ff27ecab4c75fe3618c9a787cd0da45d9e9a9f Update opentelemetry-go to v1.2.0
32c5f477e0789425e1334f27570f90cc71623bf5 Merge pull request #1874 from Jont828/async-get
bd9607cef6e8f83ac0fba90483c084d1425f1465 CAPI: update to release v1.0.2
1a869cbe3a2762fded6d42e409a5ba4d26e4b5b1 Add async reconciler interface and refactor async service to get existing resources
ae17065420f1a985bc6c2d6ac857e835750fcfe8 chore: do not replace pre-created azure-json secret without the cluster name tag key
90653c12353f98817c9713429ae9faee1a84226e Merge pull request #1812 from devigned/mc-logs
bc6541623604a228919e8ea4d851d6d7330406d6 Merge pull request #1904 from CecileRobertMichon/kpromo-beta3
4ba16abd6f03e07371d58c5f9cee23465e4de2bc Update kpromo to v3.3.0-beta.3
1e975580ca29d23f974cc3ab272e0c015b882d5e make all logging consistent across the controllers
48e12d458d772c09f6768601927e5be52a2a3c21 Merge pull request #1877 from CecileRobertMichon/krel-promote-images
ed345c6b0552c53f2cb02f9c3bf5eb6f2e0cb64d Merge pull request #1898 from CecileRobertMichon/make-install-targets
69f34261d978324076604bf8cd36970c2031d0aa Merge pull request #1844 from Jont828/async-disks
7c14be515cd0cba0c0d6c98a23839ffed2d2ab70 Merge pull request #1897 from djdongjin/stop-using-capi-kubernetes-drain
420a1c5c80535da7454948c213db816d568aca9f Merge pull request #1890 from dlipovetsky/apiserver-host-private-dns-zone
99c9cb8ab6e829f1f889fecf414e53bdad070c54 remove usage of realpath in scripts
4c58842d397d005a5c6fa00d2753c9666b63a0b4 Make disk delete async
1a16f42bc104b6a8f5931dcb36f7c5ca184ff4e3 Merge pull request #1895 from djdongjin/enable-tilt-rebuild-template
632b1e1c9e9bbfb0adf323e573b1d6aa55c0d6e8 Update release-notes to v0.12.0
138472b63fa55ad843eb747df79bb3e0363fe07c Add image promotion make target
046d88144c64929bdc68d46c4e5ed8fa00e7c496 Merge pull request #1891 from Evalle/ISSUE-1866
f78f513b53b5743d183c377f1fa96d6c44f75d31 Update dev guide to include missing env variables.
0918e9cf71775032a9f95dcb689ed0c6514ea733 Derive API server LB DNS name from user-defined private DNS zone name
79e7c7cbec1d0f971ee0024c13bc0d5387f55939 stop using capi kubernetes-drain
7f70fb8506d63cabb0788d6caaaab9d9103dc595 Merge pull request #1894 from djdongjin/update-manual-testing-doc
21c403a11d5d5e5f71be6f12d9bd86c80efde04a Update dev guide to include missing env variables .
ed4af2c4704750219de1d020ad0ed636d42795fc Merge pull request #1892 from nader-ziada/codecov2
81e925bed9f9db7829cdff0128e82cd619f9bd91 update code cov action to v2
99faab8b31ce9d0d0ea449271f3be18771a04182 Merge pull request #1888 from kaitoii11/fix-typos
7d92a4bcb38facff57a27832dd800f2412553479 Replace all occurrences of ToNot(HaveOccurred())
066aa2b044bcee6d5c716eb52b01781ed7530f3e Merge pull request #1884 from CecileRobertMichon/kubectl-bump
9acef8b6be6a7c73a18440223aa100b487bf20de fix simple typo
721ada677ccaa97ce89dd265afb3888f43cb9e6f Merge pull request #1882 from CecileRobertMichon/fix-azurechina
e8b23bb89170f2a7e545844efe9f887cc558536b Fix AAD pod identity integration for sovereign clouds
885c6de3a9ac32d339b0ab804f069d1e8446f28b Merge pull request #1856 from CecileRobertMichon/shyam-owners
b344e7c502dd9a43974ee7c01f586fb9fe915641 Update kubectl hack/tools version to v1.22.4
7c4ceec47102a53da7a30332b0104746bf5ae6c2 Merge pull request #1564 from spectrocloud/aks-availabilityzones
3848ded6651623e8597c4fdb24881ec349577ccb availability zones support for managedclusters
ea26d56d7d070f518c064268641e63407afa43a8 Merge pull request #1815 from zmalik/zm/add-scaling
8d5cef520fa4a49732b02169fc1bae3eef41511f add support for autoscaling in azuremanagedmachinepools
953e88a6552ff7ac5fa6949b6f4d27a8c39f67ac Merge pull request #1879 from CecileRobertMichon/fix-conformance-latest
ad60559fd3f2274283f7f06becc3fbc1c1680192 e2e: Only check for valid image if version is a semver version
110a1c6da8a68b8f90d525ac337a557a2d6285a2 Merge pull request #1767 from CecileRobertMichon/cluster-upgrade-test
5cb44941f892c4953b3106ae7011e0341c0a5c70 Merge pull request #1810 from shysank/v1alpha4_v1beta1_upgrade_test
894e80e449c737695eebfc7f62c0daa5d6495985 Merge pull request #1855 from mboersma/sync-linters-returns
57e9bd6a563111ce382357521e2f1694ba725b31 Add several code linters
8be8e436664ef0dc86bea0fe1e4497243f9bc901 Merge pull request #1848 from mboersma/sync-linters
ee7a6ed67cb87d871a770045a4904a1eda93ad60 create separate context for clusterctl upgrade tests
04b2b78317540557156410932cbda69383055f95 Use stable k8s versions for tests
630a52ce3761544573f53a8d5c378889093128eb Add cluster upgrades spec
45519b18be2cb7a26034419df99d46c87b410285 Merge pull request #1863 from jsturtevant/fix-windows-e2e-log-collection
73c13e69ead4360d127aee7f64ac13472e6c31b5 add v1alpha4 -> v1beta1 upgrade test
91d283a6b6c91434ed4d6aaf5dedd8a6f8c66c0b don't ignore v1alpha4 test templates
b7bd53e8a121aaf694e1734f028e1fadc35590c9 update capi to v1.0.1
accfa04eb671137ff1ffdca293ff44f40e022178 Merge pull request #1854 from cpanato/remove
cd67a01b9241c3a713870c9c948adad6fa86fe43 Add ssh key for windows nodes to enable logging
5127e1dc9f1ab332741d6f4abe01af66eaf1329e chore: remove cpanato from reviewers list
e666293945be0ab1d73b34cae923bafd96465cc9 Replace and remove deprecated linters
feba723784818f210a7c4cb96e82d7b38d0b2334 Merge pull request #1850 from devigned/regional-vmss-client
613a2ab0042640161f2dd034691da6cd4cb03599 use a regional base uri for making VMSS requests
08a9e9c30268f8d663867c2cbe3b639869fec8aa Add shysank to maintainers
f347824186acfcde07be44c64fb3cb315ce32832 Merge pull request #1853 from cpanato/updateproject
87be5b143636edfb3623712cfc84ef74409ff892 chore: update project file
0ac1befc0262b22b35673fcf2473ffd69d8ec9cb Merge pull request #1800 from devigned/fix-managedcluster-diff
27add62c04f11f8203278f052021d490daf35ae3 Merge pull request #1845 from stmcginnis/golangci-lint
18f5065e53218a3ef9d1599f11d7b22c2dbf8a9c Merge pull request #1842 from mboersma/arm64-compat
6a9b3b9ea9d6c65bd05a51517ae1721cae136033 lock in aks tests in northcentralus
2d4c465f83ae4dbc08733a84bd4bd2a7ca9dace8 Merge pull request #1837 from CecileRobertMichon/vm-fixes
8478975be3f767bde5577d49e9f786e022843c32 Merge pull request #1846 from CecileRobertMichon/fix-build-provenance
b9751286d35efe77a7d28b793aebb08096d242db Bump golangci-lint to 1.43.0
eddf63698055dcacb255372206f422f67a9455ea Add PR number and pull sha in e2e resource tags
9eafec0ad517461ef36808b5e71d568a1b2ddc12 Merge pull request #1834 from jackfrancis/aks-versions
a7913b258fd4e08426bc8240ae74d117789bf3a0 test: always get a working AKS version
ed4521f178c95a4a8cda704d971b220477059a04 Merge pull request #1838 from Jont828/async-peerings
60025b09846019e9022aff86016bf4ee9a15620c Merge pull request #1841 from mboersma/bump-otel
acafac954c0cbd19ada81a865711ac71c6edff0f Merge pull request #1830 from nilo19/chore/mix
0579d7139f550b432f4912d60f91daaa0f4490c0 Make virtual network peerings reconcile/delete async
23d63ce7eaa63648a458d67a4b139e0f577fd4d0 Make CAPZ tooling work on arm64
f0f291ef99914aad82951dbd4b9497ae6d80cf00 Update opentelemetry-go to v1.1.0
618979623ec12a455926c899f8aa6f8955293a58 refactor amcp and ammp to use transient error with requeue
d282228868b92a209ac2b555ea6c50b4d5561249 fix tilt managed cluster default k8s version
c7bbbc6101bc5e44d8be1aa56fc2de6a842b46c8 move defaulting of amcp sku into defaulting webhook
f7090fb9b666619d5552fcb6b66610fe3861e5a6 fix managed cluster diff so aks added fields are omitted
fef4e34cbbbd5b85bc01e581a43a407dcc110dc0 Merge pull request #1839 from devigned/update-nmi
71088e8bdd6a3b0447643eee840284fc4ea2d091 update the nmi image version to the latest release
e038670db2173848bbf78660c7952e5210f2e232 chore: add mixed protocol feature gates
8a4b3575e90e2ddb353c289d9b72094067a467dc Check if a future is returned regardless of error for async create and delete
70fe32277f1bfe45f3ad32fa82d015266ca2dd60 Return existing VM as result if VM does not need to be updated
00fc487cc16b028cbf0b5f7ebd27e8cf89a0a91b Merge pull request #1835 from jackfrancis/rm-kind-other
16f7b405c0f77ca09b8d27dd8cd9fb649fae2ca4 ci: remove /kind other option from PR template
cbf651f192c774955f4380273527479716358b42 Merge pull request #1807 from enxebre/docs-externally-manage-infra
ebf1a1c91f7378a8b356fa1ee02d06e66e3fb0a2 Merge pull request #1697 from CecileRobertMichon/async-vms
70ea4017712a6778c0ba94d50bde98135c44ba1e Merge pull request #1823 from CecileRobertMichon/fix-test-docs
064c8625540e6e507898be93d219fa43a3bd2034 Merge pull request #1825 from Evalle/ISSUE-1820
33e315697a51e8569796dc4b4723575f8fb1b7fb Change branch from master to main in few files
c48e566d880dbda0d0b8bd758f9e53933b2c06dd Merge pull request #1821 from shivi28/mod_update
930c3ca0af91105a8e4ac801c8644ffc426cec6e don't print "failure" for transient errors
1a2aeeafcc5983ea5fd6cb7a25b93ec043a2322d make virtual machine reconcile async
d2b4e8ed2313adc270a0911d9d0c64e344f34cc4 Merge pull request #1822 from devigned/kind-reg
f813389a3094c9696b17634052669b3e100ca427 fix dead link in jobs.md
fdec79395272c9e8d067a7a748fc1cc8f2205425 Add externally managed infrastructure docs
1eb9e703ee88b4d1a588f001209efe7ae088f458 Merge pull request #1797 from CecileRobertMichon/next-version
2f6b222a6abac05f542d78887381446676db0dfd clean up kind with local registry and remove kind ingress
f6a99157f797eef19cd29669fe5361f5653b9c0c Remove indirect dependencies from go.mod
15edf5d0e13cdb1143aef76199a0cdeb5611b1fe Merge pull request #1819 from CecileRobertMichon/release-1.0-readme
b54b15671796fc3fadf627461fc472515f54c2fa Update README to add v1.0 version support
8b2481050f015b400a51a034f855a2f91eae34b1 Merge pull request #1811 from CecileRobertMichon/re-add-ssh-defaults
7ca2e2436fa697c568f5996e74f4e34473875378 Re-add defaulting for AzureMachineTemplate ssh key
29550242c70cc3b46764bf48d1fafa1bf0a773b0 Merge pull request #1805 from CecileRobertMichon/pre-release-notes
ec42b64a30a9f6b96fdc9995be1f871b0845ba76 Handle pre-releases in release-notes make target
df6c654b948852a46f93916c8f3109aa3ab6c6f2 Merge pull request #1771 from shysank/v1beta1_upgrade_tests
4482f7f5f8739820ca088cfa44fa01a8e20bd2f9 Merge pull request #1799 from devigned/ampm-convert
909f3a09620980335a4e7554049eab835a062bce Merge pull request #1795 from jsturtevant/fix-windows-dockershim
aefd581bf254fc3fc7e6789e99a3042b61aebc0d add test for default mismatch
4de6ecdc65283e3e10ff2dbbc06cc5cdd12d3d2e fix default mismatch during v1alpha3 -> v1beta1 upgrade
1a480030b41c6d505226acfa3f905c926e141922 add v1alpha3 -> v1beta1 upgrade test
a2a39e594bfa9adf454340ed0adad4ca08d8c09d Merge pull request #1792 from jsturtevant/fix-e2e
e56a316ae8bfb5b0c7b3282d1d4a56b0ce97afe4 Merge pull request #1774 from alexander-demichev/machineset-support-for-as
5b10d25bde20f49f62be2481c0875940728f5b7f Windows management clusters not supported for clusterctl init
3f5830607dab33f2420b5fa69ea18f796a4b2c23 fix env variables expected for prow
dee62c83b359f65c920c420f46ea9f9dea64162c Update availability set documentation
ea83f002dc5aaf92b38a7a4e6c7922aabef8ff2f Merge pull request #1781 from CecileRobertMichon/audit-api
d6dbfaf79d50d42cc358b823c3f4016c64891f2d Add hub and conversion for AzureMachinePoolMachine
b25ac49fab0cee6a22f0e34f8876830e30e86264 Merge pull request #1794 from nick5616/ws2022-flavor
1210adad5d7d49e0063aef65f767c93bd58bf0aa Merge pull request #1796 from mboersma/update-tilt-provider
c769575d165ed0253a25964c2a3e32561b8f9f1a Update clusterctl-settings next version
d445d98b24cbb70b82910df84d5a3837e1038a4a Added 2022 template
c9ac4f689ae10581ddc59b7cdd42ac857c1b7324 Add missing fields to tilt-provider.json
3ad17000ca0c88ea975e26ab5d43a3e49211cd0a Merge pull request #1721 from karuppiah7890/fix-1696
505ea5f48e640fdb1286a9da54317138c76de438 Merge pull request #1786 from CecileRobertMichon/ci-entrypoint-windows
5a89a0a6c3b6d8a354b5a145db9e0ad945ef81ec Add windows templates to ci-entrypoint.sh
11b01ea3e1a899f6ae1f586f1590b14cd7899a36 Audit API to follow CAPI conventions
ddda1124dc9f4ce6b89fc8e80dd27a9b603b08a4 Enable windows in tests
5bdf09cb3ba7f3512729292b22c0b8285cf568a8 Merge pull request #1777 from karuppiah7890/fix-1760
0d6e8431e51c7555e2664ce174b44d703de53a94 Merge pull request #1790 from jsturtevant/fix-failing-tests
4ffc9469a1778c1ae2fb15bd7357a7b11bacc477 fix TestAzureCluster_ValidateUpdate test
44396c35640fd56abe6ed808bd08b10d95bcbed9 remove duplicate test named 'azurecluster azureEnvironment is immutable'
0b105d570bae7ed8bb4928cd5d9c03b314a26cba capture test case range variable before running sub test in parallel
ec51e23be75260e432cb664ed691e3e8d900268f handle feature gates for versions running in CI
add934104f538e885a1a6c7d76355eb3cd6df61a Merge pull request #1788 from ameukam/use-k8s-infra-gcb-docker-gcloud
8508da989832c571b86d2a2fbe7a6e1ae59df327 Fix resource group not getting updated if tags are added
e670c7e780613be3fe2b060948fd5919468f84ec use k8s-staging-test-infra/gcb-docker-gcloud
9250e50ef766bc5a2fabddfc753f102dee32b0a1 Merge pull request #1672 from jsturtevant/windows-hostprocess
b7a8295b02f442ca7e706c066f22905cea9a5f62 Merge pull request #1787 from marosset/ci-entrypoint-to-jobs-md
bea20da85226c169875cf18c76959d4ffafc253f Adding pull-cluster-api-provider-azure-ci-entrypoint to book
faf03af1538ae889a9fa5b401e81c634f6853d49 Merge pull request #1783 from marosset/ci-entrypoint-fixes
1b86bca401d4f944ce25a4b2d47d63b0012655b6 Merge pull request #1785 from dtzar/doc-quickstart-update
31ba6f2eb63404d3c6fb336b4d4cef864220abb8 Signed-off-by: Mark Rossetti <marosset@microsoft.com>
140562861c9cc6dd11e9ebbeeff3d98a543a7250 Block wireserver for containers via calico
936a7a47e3b267f830c44b3adf97b96308d44b55 Add k8s CI verison support
a3139c2f77b408816a97d62fe32b20c664be71de Add Windows to Existing e2e tests
116abbf9e5e3accce46faa1eed4d689ff92ea088 Add Windows Containerd documentation
d2db53028cd3b292fc5583c6b7a93d2c1e4ee607 Add Defender exclusion for Calico
6a70f79f33fbfd691ebcdd38e56bf6f26e35ac55 Add base templates for Containerd
8e7df85183cae99227ed88020763230d9e3bdeff Update getting-started.md
469432ec6fcf64346e146be42088c0ca472acb73 Add supported versions link
9b09192fab049cb8605b1e27de49bae2fc172621 Merge pull request #1776 from jsturtevant/add-metadata-propagation-to-machine-templates
04efe15188b3d2f18cbaffe5c4f623c9c543bab8 Add machine set support for availability sets
3ef19e7d24f5d55649bda9ed129810ee0ed2fd23 Merge pull request #1754 from karuppiah7890/fix-1753
e2c05666ff5e56eb9fbfc5a4a9f567082fe0374a Align kubectl install and CI scripts to use local bin folder (#1683)
ab710536aaf9a54e7775272a717d3acce371cf32 Add metadata to machine object for propagation
bcfe2cd0e62dd1a18e248ef1b1d87a492b887eab fix tests in bastion_hosts_test.go file
4587bd2706f7c61ff09ec1ea671440ec6b53f002 Merge pull request #1772 from CecileRobertMichon/update-dependencies
42dbb8d7194e6c12e04ef909540b29bcef1dee29 Update hack/tools dependencies
c95250c37f7bdef685a7b14a6f792a5e7ca27772 Upgrade hashicorp/go-retryablehttp to v0.7.0
dcc9986cb4f43e13953ed66cdcb62cc0a4fca3d7 Upgrade opentelemetry dependencies
f3b18bca492b2dfd956485893a543285b8e0b6e4 Merge pull request #1694 from Jont828/vnet-peering
a6d045696f236099398e5f2f4e35e005cdd4d8a0 Upgrade ginkgo to v1.16.5
a6db588e5d289957dd87ee200260193a11822b49 Upgrade google/uuid to v1.3.0
a33028711377c76278fada3e74c1e0a7d6a3c2da Upgrade go-autorest to v0.11.21
e2986f6212c3c5ff2f95077bc3f5740e1587c75a Upgrade azure-sdk-for-go to v58.1.0
ac8d7a9f42da9ea7d5ab7869d1596e7a8283482a Upgrade aad-pod-identity to v1.8.5
ea347098bba0b3db63f39be88c9005181555c930 Create spec, service, tests, and docs for virtual network peering
5148baee4e686b18651d727793c3e83e2d4ed625 Merge pull request #1764 from CecileRobertMichon/leader-election-resourcelock
742cedf6fbadbd53c9d76592da64c02027f111eb Merge pull request #1768 from jsturtevant/lower-extension-timeout
93d9c3b40ca55367f8f024ee6efa376f736d28ff Merge pull request #1769 from CecileRobertMichon/capi-1.0-makefile
a8dfae7bd11a8d1d9f10c57b607a5842cc977be6 fix: install cluster-api v1.0.0 in makefile and tilt
82b11d037164ac8bd37634685f7ac3161fd7cd5b lower the extension timeout to notify earlier
2349883d1effe6344690459b40e5dc26138010df Merge pull request #1740 from shysank/v1beta1
1a66dcc7ffaab31b92045057b8186348060bcb99 update doc references to v1beta1
33c1d649573d3feb7613d45c1dcb3f9027a42235 generate mocks, manifests, cluster and e2e templates
2a14c739b2a0b25b3698894a205eb823c8c05f14 update e2e templates and test references to v1beta1
ad4df7342211d74a8a8eadd1e27958898b811d31 Merge pull request #1765 from jsturtevant/add-excluded-skip-windows-docker
6447a833ac5b65aaffcc0aade9eef97d635811ad Add [Excluded:WindowsDocker] tag to gingko skip
bf8fafe8e63d7f73b57a0653c45ad9eae312ca40 Default LeaderElectionResourceLock to leases
48f8160dee82a7897a2a1d1557f40fda05fe9ac9 update flavors to v1beta1
dc6ff6463d1d26c84c9a51228cda4dbc019f431f update common labels and metadata
c11fb6aba8ef995953e84b9724896ecfe4ec9401 update api references from v1alpha4 to v1beta1, and add v1beta1 to scheme
4f4f1f1bbf1c1f591204cb30c67a32f518e7e8f4 update v1alpha4 types to use v1beta1 as hub
a4e7ef22cd7ef889f4add8cb574def2facaadc7b update v1alpha3 type to use v1beta1 as hub
202fa4e4f1ad1b16740874fd43efe808c3ea150b add v1beta1 types
2bbd02bb1aed5817469236a9496121dde42b5b4a update capi to v1.0.0 for v1beta1 changes
ace988dec38dcdf27176a1d6f081cc64274fffb9 Merge pull request #1742 from richardchen331/optionally_specify_agent_pool_name_in_ammp
ed2c284a1444b7378dc11f63f2a5389b33d1921d Optionally specify agent pool name in AMMP
7f78c7bc945b8cabc35c476c09013fb1a9dab320 Merge pull request #1757 from CecileRobertMichon/gh-action-fix
6b9c361f8653e52a75ff90da49883c31a4a895f8 Fix release notes path in release workflow
4d1384efd736eab2b1c4eafbbf98b542da634819 Merge pull request #1752 from mboersma/bump-the-otel
df75af2eb24d913682c950a7b2534b09828bc204 Merge pull request #1640 from richardchen331/api_server_access_profile
354ddd1178c8867f41c73a0359b2c7a48190eab2 Merge pull request #1748 from jsturtevant/windows-dualstack
d1a200434cf910e30793c125f55d36f94aa21cd0 Updated otel to v1.0.0 and metrics to v0.23.0
2707d8d832a72c192e662f80b5d9f8247fe0c81e Support APIServerAccessProfile in AzureManagedControlPlane
055c4f1154a452b57874c2e68346669b8965aa3d DualStack went stable upstream so cannot disable
a09a1bac26f8502c271ddbcd2e281812744ce53d Merge pull request #1575 from arschles/corr-id-loggers
62a3b4f6685c2871bf59a410b8f0137631f58b65 Merge pull request #1730 from CecileRobertMichon/remove-kube-rbac-proxy
b825d8a6ecb110ff129d33be15c2c72adc43f345 Merge pull request #1744 from shysank/network_sdk_az_fix
6708c80ad4b44e2de164c008e388625f81d651e0 assign all azs to public ip for backwards compatibility
6fffebf7ab285927a3dd1c97f9a651d74e10894c adding correlation ID value to loggers
3ef27567085ca705c9aa1f294446b630c3006d6c Merge pull request #1741 from meixingdb/upstream-syspool
eb881cdfab9632d2e44fbaab1885a647221a9792 stop exposing the metric service outside of tilt deploy
15b5d9308dec8d0cdfea7793297055d2ee4888bd Remove kube-rbac-proxy
0e89625aa06bd5304f57f8e3876b0536f0f171a9 x
4fe1b243d2c694a70b8a154ca9ae13f7d68a5149 Merge pull request #1734 from marosset/add-windows-extension
e5327290e4fd5df3fae5779296b8e1d2c73c508e Merge pull request #1728 from CecileRobertMichon/capi-0.4.3
3818dc307cf9a20c43f5c03f7a0a756ccdf0cab2 Merge pull request #1737 from jsturtevant/fix-clousure
94acb9ea3f8f3dec3da34bb95949d9d77ce84129 Wiring up CAPZ bootstrapping extension for Windows
4cbce5eca9ddd058bcdced2a109b3074f6a96a7a fix for closure
80d909348a03f171708c15ee81d78183db36fdf6 Merge pull request #1733 from jsturtevant/fix-run-tests-existing
6d01dc774b3c78b264b727d644ee667b17c18289 Fix: running tests against existing clusters
76853c9a14e099ae7712a9902abe6dd3c77c289d Update cluster pause test with new log levels
45cea67a0dc908fbeee9e622fbcc17b56463f4a5 Update CAPI to v0.4.3
0ea1c6aa35532b51704f7acaba8eeb1bbdeb8fc8 Merge pull request #1691 from CecileRobertMichon/coalescing-reconcilers
de7cb8b67bee4219751baf7926dd836eee833325 Merge pull request #1703 from CecileRobertMichon/fix-release-notes
582090c26d4c2523294fd1ac374a5758997f3247 Merge pull request #1680 from richardchen331/load_balancer_profile
41b982d0cd025e1f7b01f20afaac3d0fe12c0bbb Merge pull request #1704 from shysank/unexport_ProcessOngoingOperation
eaf837e05dfa036627bfdc4faffb5ede771bbfb6 Merge pull request #1677 from whites11/vmss-termination-events
e0611d6ebc9918be9906fdcebe5d8bd0e4d2a690 Merge pull request #1652 from jackfrancis/nat-gateway-default
230737c5330949b899662362cfd0729b8d075b96 unexport ProcessOngoingOperation
0d374ba541065f18af492502702c218e6806eee6 Bump release notes version and minor improvements
3adb8b5067f3e7107ed474c26e6cef417dd5eae5 Add debouncing timer cmdLine arg
534821f81bc6c9f5967ac86578b9b1e6257f10c3 Enable coalescing reconciler for more controllers
2b5ca9c0fd20ee900f6286abd00e21d0f23fc898 Merge pull request #1699 from karuppiah7890/fix-1698
27da08af241d55ec5f9664407228cc4e5702fb9d remove unnecessary extra comma in tilt-settings.json causing JSON parse errors
2c7203980539027b74e41e92c2a439865ec1b721 Merge pull request #1693 from mboersma/fix-e2e-gpu-test-2
774313ed1a14808a56db499c7e95fa4a09532a2c Merge pull request #1695 from mboersma/fix-aks-test-expect
429ede2c35e78da37c6836d2d7ff469fd074d66a Merge pull request #1667 from CecileRobertMichon/async-groups
1963a3265fe30c654c6e09eead1da65bc3575e93 Allow user to specify LoadBalancerProfile in AzureManagedControlPlaneSpec
21141fd78de984757e04e647596b3b5c452ae9c1 Merge pull request #1676 from whites11/public-ip-single-nic
9f6ceda9fa84757cdf5b5ac8770f63d347367eba Fix an AKS e2e test expectation
6ae407cf72dc51053d5d72804d0f6f8be35ec4a0 Re-add NetworkInfrastructureReadyCondition
47caf96183f7d3bd1e4dda5944a06dae10318bc7 Make group reconcile/delete async
6fc7050a6ca2fac44e61b7afe632779a2230ce70 Test if GPU resources are available before scheduling e2e job
75ff0f4a397db50ed69d00367322ed8511720236 Merge pull request #1690 from mboersma/fix-e2e-gpu-test
be51d96ea085ff7d07803f78cba6fd18a451744e Remove test regions where GPU SKU isn't available
decf9ac679b63d8b6743f9f7168af58e329b5185 make NAT Gateway the default outbound SNAT solution
e656f30c756d44e205fbbbef673c70a59687fe02 Merge pull request #1679 from richardchen331/sku
f5a79aa1b3187507db7eafc15446a671594273f6 Allow user to specify SKU for AKS
946668db0cab11e201a23a816458f72d8b3886fa Merge pull request #1610 from CecileRobertMichon/async-machines
787dd19ee056c5c722d7c62c5a4e44ddfef1cd07 Add long running operation types, conditions, and helpers
309b1027f19b58c22a910b26d0e1cbdd2a368c36 Avoid duplicate NIC for AzureMachine if AllocatePublicIP is set to true.
14cf703797c86bf10df592ce5fa560ad7602e3ae Merge pull request #1678 from richardchen331/explicitly_set_enablerbac_to_true
38907d09177239a8c0078dfdad10a87c4fa65edf Merge pull request #1681 from devigned/fix-flavors-for-linux
8bfcf7a26bafda525126fb95b95f23182f9830e4 fix RANDOM var being omitted on Linux
2f9a30a4cba02e2c743a023c909fee6781995c88 Explicitly set EnableRBAC to true in AzureManagedControlPlaneSpec
3548d50588c8bd6f4a36fdead7487b065815b6b4 Wire `TerminateNotificationTimeout` to enable termination events notification on VMSSes.
d249c5bb8a6ede6568b108c66a52063cb2e3da9d Merge pull request #1675 from Jont828/azure-key
9045f0358b681277f1907f41a975c06c04850e2d Merge pull request #1668 from Jont828/tilt-labels
3d2575d7f4b0077f11d880157bb5fc65ac292f10 Merge pull request #1649 from sonasingh46/scope_tests
037a763826d35b6dd3a7942a834a83a137a8588b add unit tests for machine scope methods
d4d9a3d4f1249bda5b03f6f517caa5dcc4e07aaa Merge pull request #1655 from nader-ziada/capi042
c5b0d75a02fe541f2ed1ff5a1148e66402c35527 Tiltfile uses 'AZURE_SSH_PUBLIC_KEY_B64' to decode 'AZURE_SSH_PUBLIC_KEY'
cf7b3eb1de6e45766d5fa594a9803e2d3e0b31c7 Add labels for Tilt resources
534c9ea13889fc8ab747def9d341bcd13189edf0 update cluster-api to v0.4.2
d74b9b7cad4dc42b1d73c6c62fa29e366fba3a41 Merge pull request #1658 from Jont828/tilt-settings
b9c80480caa9a7087bb2138acc08903cc9a03308 Merge all Tilt settings into 'tilt-settings.json' and refactor Tiltfile
eaa371d7740a23621046c909b3704c788865df42 Merge pull request #1666 from sayantani11/contributing-update
44366e033285854b74a9b248c13dcbd787ecfa3c Adding jobs.md to CONTRIBUTING.md
b1fd86b0b3cd3d4d7b08b096efb33cd725a8151c Merge pull request #1654 from sayantani11/e2e-jobs
b58554ffaf8f678051370fb0a4d399b6c2515123 Documenting build jobs and e2e test coverages
feaeb169986b574c849724a526d6b243b2178054 Merge pull request #1574 from arschles/corr-id-percolate
3640e0050020982f2414cdbeb2433b6b9373829c Adding functionality to add and send Azure correlation ID headers
1b8724890f88c4007f6518c9239eed43e11a25dc Merge pull request #1653 from Jont828/tilt-flavors
cd4342acaf97e6596d807332b886a541b75ae1a2 Support Tilt deployment of multiple workload clusters of the same flavor
072bdd00166705b829c69627ad90a28f67dabcda Merge pull request #1657 from nader-ziada/nginx
78839b3eaab8b1f1876de54a774d377aeb8ec8a4 pin the version of nginx to v1.0.0 instead of master
ee281e0a1c86e94bde8e8d214d81c2dd161cadc5 Merge pull request #1619 from ThorstenHans/feature/webhook-checks
14394c9e710c7931438aa7cf9431359565e1ff2f add webhook health and readiness checks
6cb2beb8449b47b9ad0a15fe295cc45ff066bb9c Merge pull request #1650 from nader-ziada/remove-win-k8s-ver
3ebb02e201ef090b3c20cf66b6c1cc40be774edc Merge pull request #1639 from Jont828/metav1-rename
d41d8a03fa9a6f9b4a5b011ac0381d9f5362bac4 Fix redundant import and rename instances of meta package v1 to metav1
6029a88a55e478345604c2a3dae296b8a9f1aba7 Merge pull request #1651 from CecileRobertMichon/revert-make
24d3e1803c2c7d9af5916072511ae42049c15567 Merge pull request #1645 from chewong/do-not-declare-log-dump-pods
2f55093126c4ed67c037ebe58ef4d2fa220b8e50 Revert "Cleanup Makefile and remove obsolete targets"
a4279d6674d40c964b5c773ea64bc16f00ab0f2a Use same k8s version for linux and windows tests
31a0eb98ae7a806c86249bd5ee98595c94b4da69 Merge pull request #1632 from Jont828/cluster_val_tests
50e446a4d06f2dcdfbf09580e0897594e6732d7c Merge pull request #1646 from jackfrancis/2021-04-01/compute
a3d79f8c9ffb3ef90f83a1b730d3689d9ff0578f Merge pull request #1642 from giantswarm/azureclusteridentity-webhook
07ab826b34ea8c276d14b8a1dc466f956f8ab103 Merge pull request #1625 from fiunchinho/missing-watch-filter
3bc55d0a052980f966ce8a0db543a1f8d9155726 Merge pull request #1635 from jackfrancis/etcd-db-size-8gb
b6c09c4ff71d60ad50ce57aeb44b658980dd08d9 Merge pull request #1589 from jackfrancis/nat-gateway-lb-fix
573f76b9d0e707637ef5b045f58e7e0812f61341 fix: don't create outbound LB if using NatGateway
e9a2f2a37b15e536420079c7f69f963a6a2935c5 Merge pull request #1588 from nader-ziada/k8s-1220
bff7e1727177124636b492402c1e955acd779e2d update Azure compute API to 2021-04-01
af62975e9e1ceb9825c4025483a34ba31998c085 update flannel for windows
1f0278cd4f3e5fc3ab7567f8580e38ece94c70c5 update e2e tests to use 1.22.1
bf05fb9d9b80e61e066c5a60134eeb5ed2e98dd3 Merge pull request #1643 from jackfrancis/azure-sdk-for-go-v55.8.0
7e8c5a3a54e21d268d5a4ae70a6c8939f0559707 fix: remove log_dump_pods variable declaration
34bb4c6642ff1af7847b990e02b12c4135699474 Add skip cleanup for private cluster e2e spec (#1636)
a18056c5ed2cedc23c7e2cb3cc67310220dba74e update azure-sdk-for-go to v55.8.0
9713056b1c2e1bf4d3fad09b3f7231eb648776cd Merge pull request #1613 from shysank/outbound_lb_fix
8a16363e4461ddd64d7cbf35ec967c185a42e484 Merge pull request #1620 from nader-ziada/capi041
b27d39aa180ff6bc839ab38739701595525cabbb Fix AzureClusterIdentity conversion and add missing webhook
a8f7d33e818ced98c646d89f3ca114e0939241dc Merge pull request #1541 from CecileRobertMichon/async-proposal
5017f249abcf9a0497fea6e306aa23a9ca20ab54 Merge pull request #1641 from feiskyer/patch-1
2bebd5aa10ca0417eaca55b6ee2b9158372344b7 Update MINIMUM_KIND_VERSION to v0.10.0
71c62e77690197a8892061666fe016b7e2b3df64 Merge pull request #1633 from sonasingh46/update_docs
ceed797d5496054b6ca0357439fff2457fcde5a0 Merge pull request #1637 from CecileRobertMichon/fix-release-notes-branch
703898b00ef7cf992be76ac882a3a94c1babd42c Add proposal for Async Azure Resource Creation and Deletion
57dff6b91800bf50a0fb3cfb22d1e5616d4e7b5e Merge pull request #1623 from shysank/alpha3_ob_lb
24289d2bb798b9bd6bb3a06f5a77af7dac90eae0 Add branch to release notes command in Makefile
e58ffb731714be3654585ab778fca1912892da0e Streamline error matching in cluster validation tests
3585dbe9671867865cd072e0ac68c5a323203610 Merge pull request #1630 from CecileRobertMichon/clean-makefile
53710ca1ee59d12574e9f32e3c3f7c589f653d97 incorporate review comments
621f596ed7a2f46d7c6a6a239a35e9eea7385380 update templates to use 8GB of etcd db data
6566d7a759806c0ac435665dd369b233b05a3162 Replaced Windows with Windows + WSL2 (#1621)
98796ae256d444a448df60bcbf30557a9e3e36be update the tilt doc with screenshots
7bf041ea093f6fc0630561a2452e17d9bdceca41 Merge pull request #1626 from Jont828/vnet-error
830f0e33e31d0e12ea317e649416dce0ccac71e4 Add missing watch filter label
d33396a742f5ab77035ec2c19c6606ebc457bb40 Merge pull request #1631 from fiunchinho/fix-validation-message
e93deb96b381d70f2b62102767f129c6ef320b72 Merge pull request #1628 from mboersma/update-issue-template
e199f2d77bc984f7cb9428a3bde315034190129d Merge pull request #1624 from CecileRobertMichon/gh-action-release
8320c357aedf7d4b2f7450f0ec0d98a1ff8cdda8 Update error message and tests for when subnet CIDR not in vnet address space
bf3469067c6cc1889148433281668e3096283993 Fix immutable error message for AzureEnvironment
e69472b9e9bbe65c9b8c7a704d56d22611d0d671 Cleanup Makefile and remove obsolete targets
bcc5c3bf5ca7a8a31ac2b05160cd435b9d640ccf Merge pull request #1629 from mboersma/tilt-versus-quickstart
fa269008c34774960bd41c788c7eb2bcc5be0d80 docs: clarify deploying workload clusters with tilt
a04f7f3a71685511bf3c43e57910971cb11e661e docs: mention Troubleshooting in the issue template
86f6da8ccd6cb42bced8e6004871327b60e8bd98 return empty string for outbound lb name if there is no outbound lb (for private clusters)
395505517990ff5f669b7356832692477f4b3c85 Use install-go for cover.yaml and bump to go 1.17
586a7c78858a5f00478a628e457f595436bd5fa4 Update release notes to GH Action process
83c5842640ba30f2b05571a9bcc6f327f8dbb7ba Add release GH action workflow
51d90bbe35464e8cdf56274118b8cd4d477c75a1 update cluster-api to v0.4.1
9bce317820a4c67bddc4ee5e30b5f1ce2250abc0 set default outbound lb for v1alpha3 clusters
2e16aff8874011f4bfc6450824c2436c49f44be7 Merge pull request #1617 from mboersma/no-dogs-no-hamsters
0d84a74eafaec25d246bfa2180d14cd5cf7ead50 Remove dangling references to old branch
87d3a087dae4c42d915f9cdc0751f799af430a49 Merge pull request #1616 from mboersma/rename-to-main
1e4a5d3d4cd7aace3110ee95effb7d821f29d7a0 Update docs to reference main branch
ca38cae4d99b0a5e5d695a0c812643841e135fb9 Merge pull request #1615 from CecileRobertMichon/gh-actions-main
82bca116b2b5f10379ebb57371326bccbc083f11 Ensure Github Actions run on main branch after rename
ca3b6b3abc2e63f01096eacf4ba4c4eee22eb8b3 Merge pull request #1611 from mboersma/freshies
dc788d34d54adfa9b70f2203c814b6221fdd1847 Update dev kubectl to v1.21.4
3628c9697f3ec376c6db3d8cb457b484298f3451 Merge pull request #1603 from nader-ziada/calico320
7e769db4c026002083c7633e174d518eb907931b Merge pull request #1600 from sayantani11/docs
02421f96fd7eb817e2efe17cd541d741e8b4da52 Tilt requirements section added to the docs
4f0e0fc3f8a5798b85ec134264ce121322d90595 Merge pull request #1598 from spectrocloud/fix-managedclusters-custom-vnet-delete
b9f62a3863c5edecc2e0245f5d727e8cceb25803 Merge pull request #1388 from jsturtevant/windows-custom-binaries
079d2ce27c3a89a2046ccc28985cbb7fb14fd709 Merge pull request #1594 from CecileRobertMichon/owners-matt
b2986fe17c0cc573b4d46f9be2d484267ddc5fd0 Merge pull request #1602 from nprokopic/refactor-ammp
d90f70226c70c0cb1daa09ab2310be6a6f5ee863 Merge pull request #1593 from CecileRobertMichon/owners-ace
3a1557d21faa9857615a79feb2435b2b09cad4fa Merge pull request #1560 from spectrocloud/aks-aad
52dfa525234b73f050bebd7539d3f053a43a29c7 Merge pull request #1514 from shysank/manual_sp
5df84fc802dd77906ad034a91b9734fbfa94c90d Ensure we don't overwrite pr templates during generation
c83ac48ef284a6ac0f7935470d60a96911434572 Fix miss match of kube-proxy versions on build
e346d339b81f2d3c489ea56e56b199c0e5ae91ef Resolve Repo list for Windows
7447ae7eb12a35a0164eaebb1221d647d0db8fe6 Don't run slow test for basic e2e tests
f2809eb94983c19260b9b38d3003eb8b1239f776 Ensure we don't overwrite the values during prow template generation
da0975a4c8dfb4c68cb5f34972ef8f6fafbd6389 Refactor managed machine pool
dcc9efa41cbb3dd014acf32cca075cd65a226cd0 Update flannel rbac to to v1
2c688c65d20576cedccb909ab3c8be6d818d43fd Use unique value for linux workers count
1391e5772532c3d508101551834a3f1b8ddcd0aa Use CI binaries on windows
fdfdd7909a8fb087733bc1f281b99ad507ed2f39 Build windows k8s components
075c89ff80e0e16586571b230bee48f73825a6cb update calico to v3.20.0
d411a1deff85ab8456356211f136301af43cad18 fix managed clusters custom vnet delete issue
e1652c3636c593de03fad236412826982b8ed07c Merge pull request #1583 from CecileRobertMichon/calico-3.20
7f1796c14e85a6f391b56bed6fd1e491f455d1ea Merge pull request #1586 from Evalle/ISSUE-1585
0607727d1553ae97e73afd33e556364d41ac59b9 Merge pull request #1579 from sayantani11/issue1573
016ec0564079f07a0cdd9735446d16586cc00c36 Add mboersma to cluster-api-azure-reviewers
d314392c7938db8b07b02a0ee407dfcef2eb7927 Add alexeldeib to cluster-api-azure-maintainers
47d5dea8092c87e76dbd54ad8722219788082bb5 azure active directory support for managedclusters
7f6a9ca8df9190ae35ac49a259cdf0d23c0bc776 Merge pull request #1582 from nprokopic/refactor-managedclusters-scope
cfd092e4e79b89b5399f0b28eb46b00e82d45a0f Refactor managed cluster scope to interface
0a825e3523d34824957e7fe80d796072d0bf03c9 lowercase AzureManagedMachinePool providerID
81c417ec4ba4b3197a5377b04fd271677e46f583 Fix MTU to be under 1400
fb2acf322d08c6ce8b083ece126d9b6c2452a10c Add AzureClusterIdentity to private cluster and self-hosted tests
7413ad2ee992585bf2209849ed8417f1d4cd86f3 Update Calico to v3.19.2
47fa01338e5357bc27ddaa7765db0c70485c7810 Tiltfile should tolerate creds set in base 64 encoding
eced64af3f168b8e76dfb16c76c221bf079c7f29 Merge pull request #1498 from mboersma/export-to-jaeger
945b35549abec4a68541e7e93affe3a611dd6ecc Update opentelemetry and export to Jaeger
84192b4112e049580fc8081acfbbc6e038242924 Merge pull request #1577 from shysank/imagegallery_panic_fix
dad5164e0ae427a66e9cac06a9f97bff3ff92667 Merge pull request #1571 from CecileRobertMichon/acel-net-test
0aa677900ddde7dc3f18c4a02ef776f1c239a77b Merge pull request #1460 from arschles/corr-id
b8676c5c2517c9a6df08753486b3739ef5616029 fix nil reference in azuremachine conversion
eb6d336e0fb86fed78ad19fc5d1b3e231b3bb3c2 Adding correlation IDs to reconcile loops
8f1786f3b41226e6a0987c8afad8d17ebbf7f046 Remove accelerated networking test
c80922cb447085ebbcc9580349c2baaa11a2a3dd Merge pull request #1567 from alexeldeib/ace/cover
d2cf344f1bdc16bceb53a7c1919cb980dcbd54d7 Merge pull request #1508 from mboersma/twenty-oh-four
039a4340b5129c7b40f4a6799c9145d806a8ecf4 fix: update go for github actions coverage test
2380d608c152778472c29aca3f38e3de52f9f76f Modified all the hardcoded GCS URIs to dl.k8s.io (#1561)
10e1f1daaba03ef86f358da71d71ec781d868b88 Merge pull request #1544 from alexeldeib/ace/nonterminal
6478383c50861041486c300a3b0952ca4345fa3a Merge pull request #1562 from devigned/fix-artifacts
cb2bb5ab440d434d74ab908e3fa25f37e8a05abe fix artifact collection during e2e tests by adding artifacts folder to input
6ada0321d98e37dae83484460c3717d6f03afde7 Merge pull request #1520 from spectrocloud/system-node-pool
833c2de0b68cd67d2e111d5b9993abcfdadf5275 Added support for system node pool
5e7eb7c29fa730d1598e83de39f4303bafd55ee1 :bug: managedcluster/agentpool in non-terminal state should return error
d52c4046c8f613e6173e0cf37508e45d5b5f9dbb Merge pull request #1507 from devigned/verify-az-delete
a635f6a47853789a6f9c63ed256873caa8727249 Merge pull request #1549 from CecileRobertMichon/clarify-multiple-uamis
c5843a82801412124a60286fb418af6a91262057 Remove AzureClusterIdentity Owner Ref on upgrade from v1alpha3 to v1alpha4 (#1550)
6644c96bfac807259bdd8348213691c5111e0052 ensure e2e specs fail if Azure resources are leaked
5dcfb2017720052ef33e9eb91258c3805d594ee1 Merge pull request #1542 from praveenghuge/azurectrlpool
e8507d2bdebd12fe366134634da8382479fa24fa add docs for manual sp
d12d7a93bc960a10b9b9590d0c9ae720174f87a6 support manaul sp identity
aa096e8facc2860c71f98fa7881e3774bd15e465 Merge pull request #1478 from Ankitasw/ultra-disk-support
e1faf08f76253e8b4200340a41b2e26dd86867f5 Add support to use different subnets in different node pools (#1411)
13e42069ecf9781e20dee95cdc5ab5a3b0ff7698 add support for ultra disk
e6b3f55278fab4e0ce1d0fe241431cda7f69169c Merge pull request #1535 from CecileRobertMichon/e2e-cluster-names
e308412fb858b5f93b8f7d21846af759aacb548c Add note about additional user assigned identities in docs
2f4d63968673ccf5cb03fd21308e5a20f29dc13c Merge pull request #1547 from alexeldeib/ace/mpMapper
b4ace579790e3f89b02cf7ffcc2c9fea04dc1146 :bug: wrong mapper used for MP -> AMMP
361baacad67976c1550c75772e80e3b803e4e37a Merge pull request #1509 from alexeldeib/ace/dsTimesync
1da1805a5852400b55a516f5c0560252ef4c0615 Merge pull request #1539 from praveenghuge/azrmachinedefault
62a0b5077f6a6f4fd263679765f625a642b8848e add daemonset implementation of timesync validation
0fb5a11a3bd8041423a2b0ac67d97491e27a77c3 add userAssignedIdentityIfExists to azurejson machinepool
2ebfc4eb871c22cb3c12fb5c93a1818ce30745a5 add testcase
fd7f1973f610dd43aebf9d14b697456294662919 Add e2e spec name as cluster name suffix
6b30006fc66e51e1242c1ad2ed471017f4c6738a Merge pull request #1540 from Evalle/ISSUE-1528
7f2d062a16af31fba6ee81f0a9fbf03893132ca4 Merge pull request #1531 from CecileRobertMichon/cert-secret
ee81d7e8d43e91a262e920b007dc2dce0140fd6d Improve docs around identity and add certificates to SP options
e9ac1f25b8a2b17054df487df2a45f3070c3c287 ISSUE-1528: make webhook registration accept v1 admission
5886b34071e55320c32ed2f9877a23f18f0d29e7 add SetIdentityDefaults to azuremachinepool_webhook.go
64ac1d7adf0403400ee9baeed3c1180965ece85b Default Ubuntu to 20.04 for new k8s versions
40fde825296677d91daef3fbd083a118f2aad3b7 Merge pull request #1524 from nader-ziada/k8s-1-21-2
08f456963fb47f801e75eae730837e3cffe57bfc update k8s version in e2e tests to v1.21.2
6c1ed3b1d50e341dce2f7b006c334bc2060239fd Merge pull request #1530 from mboersma/fix-link
7fe253d2c3b61181469cc7218b0984dcd22d249c Fix broken link in proposal document
10fd43ec671ff04d391d205efe3f5fcd5f06efb0 Merge pull request #1523 from CecileRobertMichon/azurejson-creds
ecbe2848c05add168553988000ca5828d8653d4a Merge pull request #1439 from mboersma/export-to-insights
ba176ee451551ec5b6b18b5b006341cb6e665613 Merge pull request #1527 from shysank/natgw_pip_fix
df0fe5c81ca4d10be0576c648b25dfb3aee25581 Merge pull request #1465 from CecileRobertMichon/nodedraintimeout-test
e96222d5981e0b69afee473af819feef4263bea4 Add AzureClusterIdentity for the prow template
07ea6b9bc2ee2311fe0723376a31cb3d1743c024 Add warning message when using Service Principal
8040e4154e31deaea48aa37221315d78b632d525 only update nat gateway id after reconciliation
4554208cfa8ebd35a5dfe0f956298d6c0d561f6c Don't set b64 variables in conformance and tilt
dd6fadb1ee9992dd05327de6d879dd2e55ae79c1 Merge pull request #1516 from ykakarap/machinetemplate_validation
6bb7bba1aa20304bc845631c3a316d9603551e9e have consistent validation/defaulting for machine and machinetemplate
7f2c5e05f6f88214f42a1f1dc2d77b1cd456d4c4 Add Getters for SP credentials to credential provider
92c88f2a884a476306a7ddaf66ef087d8e9d0e23 Merge pull request #1512 from jackfrancis/k8s-staging-ci-images
01b961b9c4dfeb8bf839797f8aef099d53a28ec8 update upstream k8s CI image store reference
36ace98b37bbe890f6a4b90a0f03fd8acf9d69f7 Merge pull request #1473 from CecileRobertMichon/readme-v1alpha4
15da9c80de36e90f3f564e9c75e928c8003b7614 Merge pull request #1506 from nader-ziada/identity-owner
0dea87d60bfb8f29b0873544871fd1b3f7b0bae5 Remove owner ref from AzureClusterIdentity
0d7b8717350b406d2da451ffa4c22f8097c00205 Merge pull request #1504 from nader-ziada/create-cluster-env
ca2388876d2981b911aaaab39010f3752f1bd395 set identity related env vars in create dev cluster
2bb61139dd4d05f99b3b6b07f71e45cb260765f2 Merge pull request #1502 from CecileRobertMichon/fix-id-delete
d7461357350db6abf35cf3703d84941e92be326c Don't delete AzureIdentities from other Clusters
625daf09418dd680a8923358e8f6608081837c06 Merge pull request #1360 from nader-ziada/ci-identity
c85e4dffb10131bf1fde5fd61b4cd96a4f5b02b9 Add azureclusteridentity to templates
d6a8184d4779bfddbc1efb87d0c910c55782e44a Merge pull request #1492 from jackfrancis/singleplacementgroup-false
75a3eb440c25633d4683ef15274c0056ae87333d Merge pull request #1491 from shysank/natgwipname_default
d9c48064c8051d644fe516a6d8bc3b9ebb42828e add script for identity secret
1aa9837cd2f9d9efe4e4eaceacb22a1b55e13969 add azureclusteridentity to capi tests templates
b665b213101153f673dcc7fdfddddbb2b032b58a set identity before running conformance test
4b56596ebe7d0bb1b47b272f8f46504472ba5073 remove using a different SP identity test
d49cbc70aa6a6006e19fd0aabaf6b297fae8c856 update calico version
2fa007bbdca98f50792970ef0bab9985fc03f001 use AzureClusterIdentity in e2e tests
d06e73e4e830c80f7b4cf726047eb098c0d372b6 feat: SinglePlacementGroup=false for Azure VMSS (MachinePool)
300757bdc09eee1ff5be83eb1684c55fb15be394 Merge pull request #1490 from devigned/nil-drain
02a3af00429eb1a345da7a6fe9b6bc568450a45a Export traces to App Insights via OpenTelemetry
f68bc81b1e44cf2aa2c06a926779c907c4ec3830 set natgateway ip name in defaults
c69b23e7b69ca4fc556adb2b092c579c75a9d283 fix nil panic in AMPM when the node is nil
e70f158c69e2504ae1bdd33af8bf2745eaec57d1 Merge pull request #1489 from fiunchinho/reload-tilt-azure
c88f20802923103b538ae2dd74755c694502d5cc Merge pull request #1486 from CecileRobertMichon/cloud-provider-1.0
2ac653f45442b88535f41c4384739616148959d0 Merge pull request #1445 from CecileRobertMichon/make-creds-optional
85a276a455dd9a1060dceb60175a176f1acc3125 Make tilt watch relevant folders
69cac90761a0c0697e049f6b07e34dcd5dfa7293 Merge pull request #1466 from shysank/cp_lb_config
7d293d5f241957bbd5fcbeb4f1e885cfde8793fd update templates with default cp outbound lb
5fb670b9264b193117d7251b2645150d75dd5674 add docs for control plane outbound lb
e5c40a4f727d51be6e0c819ebbaad01580af3871 add validations for control plane outbound lb
8cf5162955d7d52ed7cc99dd17841e48c9eccf6b Update external cloud provider templates to v1.0
b34671d4d50397ff49b4d227e1d05e0db7af10c4 Enable node drain timeout CAPI test
217c1d7bfc96284e49d7cd09b4f8ee8f7ecc7f55 make control plane lb configurable
7344eb9dd7160d073daabb492097dd2667052d8c Merge pull request #1188 from fiunchinho/subnet-nat-gw
f10b41a5b38099ef953f7b30dbb42a248cba3337 :gem: Add support to reconcile subnet's Nat Gateway
8b33711b4a3aaa460b0ce7cb43fa297deecdc47c Update README for version support and add v1alpha4
c2fa089c7c48be14dd20f8ec79b8ef374544802d Merge pull request #1477 from nader-ziada/deprecation-notice
24bce1edc3aa5eaddb197fec15ed640f3afb3f31 Add deprecation notice to using credentials from env vars
fc7e6eeccd9e46f6c9935f254cfe7d64a5300e1c Merge pull request #1480 from CecileRobertMichon/capi-v0.4.0
6a8d7e6c28866eb05a277d511064da31e86045ef Merge pull request #1469 from whites11/add-plan-support
cbb07e8db1d69b7ae71d835b0df01eb4f38f2e57 Update CAPI to v0.4.0
5dc58ab05ecc9f650306831b8767bde757e379dc Added support for specifying a plan for VMs and VMSSes when using a SIG image.
076a10d631561a71c3059e590591274b58c9fdbf Merge pull request #1476 from fiunchinho/fix-broken-link
8719a56f28a353d14c371d2306cf8351c31f0ce7 Fix broken link in docs
54da075b1d73f99754d373858dc8f4a5b10703fc Merge pull request #1467 from CecileRobertMichon/makefile-versions
df3cb5bebb4c8b8a479a677ec36c5edc5d198f33 Merge pull request #1464 from CecileRobertMichon/capi-0.4-rc
9826c5dd2feb0a9ffdece9d6c8c50b132ce071b0 Update generated files
81acabe1a2a3831c62ef270270245b323db9b378 Update kustomize to v4.1.3
40c3f786367ef6ff37cf08f100a8e3b22b5f3ce1 Update ginkgo to v1.16.4
6e089c227f867ed68a995c13500a8b7f49f86eb8 Update go apidiff to v0.1.0
cbfd840aef350dbaec34e0307eb1f0e57595e0f8 Update mockgen to v1.6.0
a226733c4c80d16e933d2cbb3281e12dfbf2a7b0 Update golangci-lint to v1.41.1
57629b4176e712e6391c4902431c1283feb986bc Update conversion gen to v0.21.2
563f8dc6e76eeb91f5483ee076fecb4171656a3e Update controller tools to v0.6.1
bc4a5b640a3fdf52a40e70b006f0e79d21c619a1 Update release-notes version to v0.9.0
e4553dbdb0a6561ed7aa8cce45e22d1e59c0b4cd Remove unexpected logs in helpers_test.go
9374108bf0d63da1dc78ae6e18177510f4173995 Update CAPI to v0.4.0-rc.0
f3ecc734ea7b1c216cf46659baff191dccb10e6e Merge pull request #1423 from CecileRobertMichon/capi-test-templates
99748d4eadcbb98d7df50e9afa043048e5b1c7b0 Merge pull request #1425 from fristonio/pr/fristonio/shellcheck
3f8b9f1e427877c61ec69bca60a39d5b76e096b7 hack: add verify-shellcheck target to validate bash scripts in the repository
9cb9556aa235e447f0def90727030f23fb92cabc Merge pull request #1459 from devigned/ampm-docs
e834444c79579755b103b2799afb4811a7f6ae87 Add more tests to CAPI tests
6e02eceebde41e89984de90173be8cc40bd84727 Refactor infrastructure-azure templates required by CAPI tests to match CAPD
12f99f0a536a1db97562ce9774cf9de10a5e4fdd Merge pull request #1435 from devigned/ampm-drain
8230f4306b4dfd51457efad102375548946fa813 update the AzureMachinePool docs with deployment strategy details
27cd557e53306d15857d975c8835f9b641a13771 Merge pull request #1453 from alexeldeib/ace/deadlink
31c487d215cdc2eb90612bba82b75d5cbd144538 Merge pull request #1431 from CecileRobertMichon/network-api-2020
d1c01511604f40360cfa7db9ffc61dabec3e702a cordon and drain azuremachinepoolmachines prior to delete
1d7a2866525ec2a023a043c1a20d9a710876e863 Update Azure SDK network api version
fc15cb681c51a5ed28e75ff5594bb29e6a5a3f3d Merge pull request #1457 from CecileRobertMichon/capi-beta.1
0a41ffc6d8e26e3c0b334011efdba70419a49018 Update CAPI release to v0.4.0-beta.1
15bde649eeb9a656314df66e665746cf9010ac5a Merge pull request #1386 from shysank/aks_multitenancy
5a6a864f3de2e2dae24dc7c274e6516eeb236354 make aks k8s version dynamic based on supported versions
76537af0e44d695595b6aadeae71aa058718b7d9 add e2e test for aks multitenancy
95fe8d90449652016afbbbeb77636fab6456e0c7 update docs for aks multi tenancy
8c678ebabcbe313921d7f245ac6788665e1e61b4 reconcile azure identity for managed control plane
1b2ace7ee0183575040edb0887371da25ee5e706 add aks multi tenancy flavor
3451e3f7b68341fca227011b13c1a51c95966b81 multi tenancy support for azure managed control plane
61453798a743db9b68a56fe5832dfa87fa4a30a0 refactor AzureCredentialsProvider to make it reusable
908cbfd337fba156e532a3e4ccd06014ea382091 Merge pull request #1450 from CecileRobertMichon/improve-extension-msg
53acd8f2bf28cbdc84d9a41e5d1b8d6a7d3c6f7e fix: failure domain version in docs
6146560c04cdbdfb4d7fa8dfa1bb45c18cd3d550 Merge pull request #1452 from mboersma/add-whitespace-linter
70cdda05b78a7fde68253f99bf907b89949f8915 Improve error messaging around bootstrap extension provisioning
43b8486be37f4bede2a209d0d35400466e82b3f7 Merge pull request #1451 from CecileRobertMichon/fix-ampm-test
b33ee6ab52e61c78ab7ef471c5ceac795f18fe82 fix: dead links; add ci link check for docs
f6535af0e7699ea63c6686a4adbafbe58ba96abc Fix AzureMachinePoolMachine controller test MSI error when run locally
d9bef838ee09b91f611d3a0ff6cfcae76403a44a Add whitespace linter
267973058257eb3472ce53b23e85ba6ffe2b9ae8 Merge pull request #1449 from CecileRobertMichon/ci-verbose
2dfe1ff8d78c8abd00691881d0bd6a413c2d2464 Lower CI verbose to 2
128493dd756748e9d3efb0bd274064de48491a86 Merge pull request #1444 from mboersma/add-godot-linter
d3881d2d2eee85b36c370bc40045323cf63ef678 Merge pull request #1446 from CecileRobertMichon/conformance-result-cluster
09b98ce81e3459be572e2b62c7ab9a48589f2e4b ensure cluster is populated during a failed conformance test
fe01418401196933c87b3835d17927adca225519 Merge pull request #1412 from mboersma/refresh-otel
bb5246701ede7c614de03f7b5b927120020b7897 Merge pull request #1442 from spectrocloud/capz-1441
c878bb9211f9fd118b7a85e141e4ec1879f94221 Add godot linter
ce809f09e95f73dc132e433966883916d545cdbd Update opentelemetry library
c255f36af07e8982c638dba89628d9f2c06cf97a Make azure credentials optional in manager deployment
477a90eb0e620283efa29b628eb3dd3f112bc3e4 fix for build failure
b2edaf032bc6497f8141e9dd462ea50faa2268c7 fix deletion for azureManagedControlPlane while using existing RG
10b7e2e7f2a49dac210f180301f5d8916479fdce Merge pull request #1437 from CecileRobertMichon/rm-westus3
00445426a388326256a66db974aba59bd369bf88 remove westus3 from test regions
351659084129d9dfc31843a412c0c5c710f210f9 Make cert manager install in makefile more resilient (#1432)
9d71f9f07ac638299919797ab97ed85829fbe2eb Merge pull request #1430 from CecileRobertMichon/fix-tilt-2
27dffa96c1422e2960a567854a5d1e72a4fb3a39 update k8s default version in tilt
492eaf5d479838de9f823422952dece86df0094a fix release link in tiltfile
4312c6c386e381f11708a8fceb395edbf9f2b89c Merge pull request #1428 from CecileRobertMichon/e2e-regions-2
2cbcf3b58ebdd4d33b1fed8f3131543ea650f91f Merge pull request #1332 from devigned/surge-take2
d1ada8a9e2f3a807862618cda3299b1a0e831db5 Merge pull request #1426 from CecileRobertMichon/capi-v0.4.0-beta
ab7ede11772f531c0a4ed97fa74284c5139cbc7d Remove centralus from test regions, add westus3
f96fba5aceab04fbd5f15e67885e02b4c0cad8e5 add az machine pool rolling upgrades with maxsurge, maxunavailable, and deletepolicy
7369cccf4af81cd2c75620c6816c475530cdadc3 make time sync e2e test more reliable for dynamic infra
b6b38b0e6f81b57e98f9eb933e3e6a9cbf2f5936 add coalescing reconciler to enable debouncing of reconciles
b2efc45e75e0c386e36e1cd081bdd47e79423aa8 update machine pool templates to include rolling updates
cb665029eaaa1b15098f39d62583bd7f14208b3a add time to live lru cache
b9200dffa0652bca72d32c05b362446a18f1584e Update CAPI components to v0.4.0-beta.0
bd904772ec98f83631c4528260f0c55a2a6efbcf Merge pull request #1415 from Ankitasw/backoff-config
bd47575a6b2a2a9da54ee0d04ab0992e74693cf9 add spec to override cloud provider back-off
4340e1d76ca303f48ee3cbf5541ef1a07b3a9c70 Merge pull request #1421 from CecileRobertMichon/update-capi
5a1da9763071c37bf215b7c2a275bdf5b4f5b8ee Update to v0.4.0-beta.0
c1df977e7c2785d33aedb69a46f215918bd13cb4 Merge pull request #1214 from Nordix/furkat/useragent
11b43469ba9f8fcbb347c4739ee4a4dba6d8c555 Set the UserAgent to "cluster-api-provider-azure-manager"
e06c3d4d18681797cd9e5dbcea99fa6f7f8875df Merge pull request #1424 from chewong/select-custom-build-mp
12bab6ff6b3145c45513f66a098785b5d1f36986 test: ability to select cluster template with MachinePool for custom K8s build
7a0f33ba699941984284c14d66525a7268685c79 Update CAPI build to 20210608
745c25ed33230fb80e889901fca5d9713a4a105b Merge pull request #1419 from chewong/custom-build-mp
94f15671c6798426e25fae6eeefa831314c8025b Merge pull request #1422 from jsturtevant/upgrade-kustomize
f3ba9f12af48350dfc7f315d71f84b3e8cd49bc2 Update to 4.0.4 (higher breaks whitespace)
ea79cc8cfa673dee3e927497f1851d454c532861 Upgrade Kustomize to latest v3 minor  (3.10.0)
9f2043ee72628ef0a821f7b15110d836c4cbf404 Upgrade kustomize to 3.8.7
a2f84cd7ff2085acd96e1175328b01b88d26732f Merge pull request #1408 from CecileRobertMichon/windows-naming
cb5360cab26e5b203e42b74e514080ee7420cc5d test: custom K8s build on machine pool
d735bb842b0d542311c7c9f61f3fb3386a6465f7 Merge pull request #1413 from CecileRobertMichon/lb-idletimeout
cc7b477f16e4c3cafe0820ebada7d64c5960b29b Make LB IdleTimeoutInMinutes configurable
a777af821a4f6103d4911b4a68afc424e73275fa Merge pull request #1410 from chewong/ci-entrypoint-var-overwrite
9663e434f3806332a2b8922215a6db67f03ad843 Update Windows VM naming
fb3a29d19b30e428f26e91fefc62a1f09fc2bad4 ci: ability to overwrite CLUSTER_TEMPLATE and CLUSTER_NAME in ci-entrypoint.sh
bdd9f8c0c92505224215a2e5e234088ee8234d32 Merge pull request #1401 from fiunchinho/fix-save-state-from-azure-api
e101b68afe8ad95aafbf0843ce02ebc77122ac06 Merge pull request #1409 from shivi28/azure_558_again
4cff58a1e31902f79dedff1b7ff8332af3e67997 Save subnet details to scope
98d7f673a8cb12832fff0a1921798d83b8454da6 Immutable validation added for Azuremachine update
66e4073d53eacae4b138309d595145c8485e991b Merge pull request #1300 from whites11/azure-bastion
f7376856cf2d8f26cd60fee4ca2d395580665c9f Added azure bastion support
8791fa90e797955d41d79d9b7372325722116889 Merge pull request #1405 from shysank/cloud_provider_secret_fix
b201e4eac70e0ca741758a5ced4eec066516d119 update docs for cloud provider secret changes
38e6656219dd2878ce449fc5e800f3ff8a76b25a Merge pull request #1404 from CecileRobertMichon/fix-uts
c7956aab57adfc66eb3c99e26e8c3f03a00a0acb Merge pull request #1398 from nader-ziada/osdisk
f8f844e521183388ab8b29994ffd8160fca38b99 copy control plane data to azure.json for backwards compatibility
7d2f4aeaafb461f3259d3336d8a2e4f81f36de06 fix MSI not available error when running unit tests locally
05b770f2ce7c8eb007351ff48a5acf058572da1c Merge pull request #1397 from alexeldeib/ace/delete
49a5984f92eafbb5924e4e832ed6358ffebe140a Merge pull request #1400 from nader-ziada/gettingstartedlink
aefb30be752912b33a8102db37de0e7878393166 fix broken getting started link in docs
e622d565448d2733f134fe1b862856bb8c1038a1 make osdisk size optional
bf7335608338b9290b13087344842bf29767621b :bug: fix deletion, speed up creation for aks clusters
43d44241128b53fca2d1ca233d5c9e552ecfca67 Merge pull request #1389 from CecileRobertMichon/update-capi-nightly
23039e8654865ecf75af6d0d558cc12c02436dd0 Add IPFamily to CAPI quickstart test
5a881ea27fddfb05cd85097deb1b247b6faf7e3b Add template for kcp scale in capi e2e test
b951b0b9362abe07245aa442ae5e2236212db6cd Rename KCP infrastructureTemplate to machineTemplate
afe9c203b223a842c0788a7eef5d8147f5dd0de2 Rename AzureMachinePool template type to AzureMachinePoolMachineTemplate
5faf1572a6f080a5b9b6bb20f1ed1e093e91d9db Change AzureMachinePool experiment API group to infrastructure.x-k8s.io
0287d4c39d720a8f025bf1960d2031e7166cf50a Add AzureMachinePool log collector
fd2a002d963d691f6940303e9022018a2e35f779 Add externally managed predicate to AzureCluster controller
fc622741b1f3290b50530c525e396dc4fe1c1102 Update CAPI version to nightly 20210526
8a44c6d6f7b394b7929c3ae5b0e79730609c6cf1 Merge pull request #1393 from spectrocloud/capz-master
ebfd39ffcd1f7e0e15d9fb9607cb40d3b828f11d Merge pull request #1304 from mowangdk/add_logs_2_e2etest
957525aa1ba83178af2c0fe7269982840140321b Merge pull request #1390 from nader-ziada/cleanup-allowed-namespaces
d0f57221f58fa7327a0458157ce46bfa24c62d83 Add logs to e2e test
55222482da2ec424561c162c7ce6cb4a9bff2c0f move allowed namespaces check to fail early
7d417c7f5f1965ff439ad76b96f1f028cc06808a Merge pull request #1373 from shysank/rate_limit_config
42ff2ba2d6d8e5afb51caf606e98fe9ccfdde8e3 Merge pull request #1392 from mboersma/update-cert-man-ext
880a5462631f11251cde5b4a0458d270377256f0 changes for adding additional tags to aks cluster
5ca0ab444ab440f406448d7650ddd3f2fcb8f23c Update cert_manager tilt extension to fix startup bug
8ebf049dd162a74a579ac7d25db726f8238dea86 Merge pull request #1119 from jsturtevant/windows-upstream-e2e
83853b7148355637cd8329e9edf64b67ffa9af79 Merge pull request #1387 from fiunchinho/tilt-config-typo
aca982041f02a1fe924424364498664906151108 Trailing comma breaks tilt
f4da85e6f68c9711a628e21183206afb9908532a add docs for rate limit config
4bda43cf4d0a65c1a9f52f6c7eb4f4419f8c7302 add validations for rate limit spec
cfec2c90fd95ba591c6342e36e6708b5404bd986 add spec to override cloud provider rate limits
d026cc3a381af0ddaf304797599dc3e55182a64f Merge pull request #1383 from CecileRobertMichon/boot-logs
3cc5960433b64b6d45c5b4849ad81446e3e45f88 Upstream e2e tests for windows
c94314be24467f07cf1472071905998177ef9972 Attempt to get cluster  to fetch logs when result cluster is ni
07631c4bc55e008b52c9799737cd1f460dba652d Merge pull request #1380 from CecileRobertMichon/fix-capi-e2e
f06aed28be3b3d02e9cf0b2d6f71600355ff7b46 Merge pull request #1374 from lastcoolnameleft/master
45d31b4add256f25b6bb7a76e7e6401c6b2181c5 Re-add handling of CNI variables in e2e for CAPI suite
b8986b41344a2d3404f30c12d7a5a1a77bb9692c Created flannel.md and updated ToC
430fb0fbeb1a2d3a9bb20e30d6edfb8996d30827 Merge pull request #1379 from CecileRobertMichon/fix-azurefile
6eb0997f8bd85bb97bd0541c5c2f652b2d597d57 Update AzureFile and AzureDisk templates to v1
63b7c675868ad9bea8de5b60060ff6e16f18d08f Merge pull request #1323 from CecileRobertMichon/oot-provider-version
61d4cd3be284f433a36d96274735e18de53fea67 Update OOT cloud-provider version and enable LB test
45c79dba3231fbac073da840c3f9a6d092a6cdb3 Merge pull request #1351 from jsturtevant/windows-e2e-logging
0e732ef39ecdf777fabf032663f1642f87493ffd Enable windows logging
9d34960d60f48a8b4a1723af9cecd747d7885aa2 Merge pull request #1371 from jsturtevant/fix-windows-cni-ci
eddb72daba7e0483fd832704565d8574503ca990 clean up the CNI CRS which is done via generators
b246fde485fc2a54d28b64df40357a57523c6fde Merge pull request #1356 from CecileRobertMichon/docs-fix
f4704bf13e9a1dc10e6fb92b861972e50b57756c Merge pull request #1368 from devigned/patch-conversion-gen
d6a69a54d8a61681a8603d89a56441ac8a10d37c do not conversion-gen v1alpha3.OSDisk due to warning message non-determinism
c8f153cfa62ee06f3e3b68bf9fd143418850085f Remove duplicated getting-started and development docs
1bc09c5fb652c765e9168524a2993fe2a78bde2e Merge pull request #1364 from chewong/custom-build-docs
d31799bf430454983ed426b482610ad9d080840c Merge pull request #1330 from CecileRobertMichon/ccm-presubmit-tests
6156c33c7c1141d091ad9834b6d7e77cf5ba0486 Merge pull request #1366 from jsturtevant/fix-1328
a38816471bbea8740b30d693ca1f2cca425ec964 Ensure kubelet restarts
51fd513e7fc4df71e28df479ba5b6d724960d961 docs: add docs on using custom K8s on a capz cluster
660a35f033be0ba52f54e1a03b79fa370ba8a5a1 Merge pull request #1363 from CecileRobertMichon/conversion-func
4b50c93f757c0f01116c117ad58bf88716c0d5ec Update zz_generated.conversion.go
d0e5a9632266bb78981794c0c50661eb9af1ccb7 Fix conversion function name to remove warning
62fef6f6b28e9fbcf160d827d32b12d7b1a564a5 Merge pull request #1350 from jsturtevant/enable-tests-against-existing
d324efd354e4e772a64e2b7f94c355b7f4b6cec7 enable tests against existing workload cluster
739d03a6c9a52a7b9a098d992bf9394c6e85e320 Add azure-container-registry-config to all templates
c43929553edd2aac1523e671114798ab3caca6b9 Add script to build custom external cloud provider images for testing
d1bf8dd7682c4c4013d1e88c001a5dc684d62dd4 Merge pull request #1264 from chewong/upload-build-to-azure
a92161fa208a2cd46dd1eac9731d03df1abe1170 Merge pull request #1331 from nader-ziada/allowednamespaces
62640c81707956f3795522189ac99d008d102702 Merge pull request #1348 from nader-ziada/nmi-kubelet
24c352a1768c0fe4401e53e82d2b313a238b805e update allowed namespaces type in AzureClusterIdentity
1887f806e738f76524f75a3a5621b3cc39d867d5 ci: run conformance with presubmit artifacts hosted on Azure
2203c184b97eb8bd3e95bd9ac5ff099c6e235c04 Merge pull request #1335 from jsturtevant/fix-packet-fragmentation
c626e1d989869fda59bb2d4e990719f78ee15468 fix issue when packet size is over 1400 MTU
5fbcdd890ed623e2106f416bd6852ccff6f736ec Merge pull request #1344 from Evalle/ISSUE-1341
d3707c94807640c9537a19232123dd4aa7625423 Merge pull request #1339 from alexeldeib/ace/tidy
72d9cd9c9cc61b3710d863369a13994fbcb892eb cleanup: error handling on machine delete
924cc8b7e00ec4ac4f993464e184ebad03d017eb Merge pull request #1342 from alexeldeib/ace/reqd
71e189918d4dfb09449408fb0dd782114182bbb4 fix: subid spelling in type description
2ca9893bbe992fdc7c44e37dceecf78b25dcd683 add FileOrCreate to nmi kubelet config file
14941f8e1e48342d79a740ae32bcba1aa4adb7b8 Merge pull request #1333 from CecileRobertMichon/cni-prow
36bfaad2e92d04f574eff3b6201ea5007e68b66d Merge pull request #1343 from nader-ziada/nmi-image
e8c8427c7882445dbffe5b5cf94a44c5f57b80f2 Update GPU test job image
e65ead81ab0f18090e1c2a006c96784d9888f1b7 fix imagePullPolicy of nmi image
1333a62677751ce2c106b5584dae858e0d8a1f64 Merge pull request #1340 from shysank/vnet-cidr-validation/1311
3eb45be89f7d116ac20238e7494a14576df81e2c fix: node resourceg group name is option/defaulted
d36a2f6770cbb49cc422cce9bd23680f0d2abde3 add validation for vnet and subnet cidr blocks
59f2fb4b85fc8c1c6789f1c7c21a75d16028ef76 Merge pull request #1296 from jsturtevant/windows-ssh-update
57d8e6165bfe418be925be03e568445eac32fbdd Merge pull request #1321 from CecileRobertMichon/storage-type-optional
e91aa7fccd80ddea6a54e1c873e461f165c77ee4 update ssh configuration
19d8d738749e1e4dc0cf0d3516aaa56369461b89 Make ci-conformance LOCAL_ONLY default to true
04ea0024815cf755be289cf3f45ef9daaf8987c5 Embed CNI configmap in prow CI templates
c80f2090a43d5a0d5217f48d61e0c32a0dc9e2b3 Merge pull request #1336 from chewong/add-fi
17437225649dcc3df92a64716a5495efc6fdfdab fix: add missing `fi` in ci-conformance.sh
f8b2304ce244e60c8b8c4c6eb78f211e91a0e031 Merge pull request #1334 from CecileRobertMichon/fix-scripts
a58e6a220450b9c676322c2787c03e342ce1acca fix ephemeral OS disk caching
30ba1e1e2713218df3ab49bdaf4ae25bdaf12564 :sparkles: Make ManagedDisk options optional
35f86c2ade7e9ccb814dd5a51b2bd6bfe977470d Make REGISTRY var required and update acr cleanup tasks
512c0dc51f37a5be380410aae3ad68e003d74dee Fix cert-manager version in Makefile
5281531830e5e23b9e237f76a3ecae2caf7c4e04 Use a random region by default in ci-entrypoint.sh
adaf9c6d4b03bbe42174ad2dd1a7c0fba66a56dd Merge pull request #1327 from chewong/remove-calico-installation
8f33a89c4de4afc55d1f952ef0a37167520bbe1f fix: remove calico installation step in Makefile
319d9b1a7dda51eca012d353f391058f9177c93e Merge pull request #1326 from jsturtevant/windows-timeout-e2e
de9df774a7604226908d8442d196cdb01068c25a bump timeout to accommodate windows deployments
e6edff7b16eab72bca70dc4d95b82feb407647ca Merge pull request #1320 from Daimler/monitoring-annotations
6b59c6f922e18029f074b11794907ad8fefddc39 Merge pull request #1324 from CecileRobertMichon/fix-doc-link
b5ca6072223d033e482e48c95495961a10ad2af5 Re-add getting started doc
bbb0867c95cda588f8f8df82043d8ff82c03f415 Merge pull request #1246 from jackfrancis/custom-images
2e0c1d68f70efa2390d486c2728452dfaeda1b79 test: cluster template for building from custom images
36464d8a5eb897887c3558ce94be40ed12375db7 Merge pull request #1318 from devigned/fix-sg-convert
efd7005e620a20a889e68ba62338775c0e1a182a Merge pull request #1315 from CecileRobertMichon/deploy-timeout
86c2c0ddbd2697e9dcf49d4ee7a0e4a0ad45b1b4 fix an index out of range bug in cluster conversion
db61d513c03cb5277ab35cab165e5e8b89a34a53 enable metrics scraping via prometheus
f5c554b21f42e645a34050772a0d32fa42264c3c Merge pull request #1316 from CecileRobertMichon/docs-book
0eecfea8621d42851abe99ba2ba2e940e980289a Improve external provider config doc wording
9088140ab681bf7605086dad8d8bee9097d1357a :book: Move all docs to the book
6a1e791725e659c6faadeb40d1fe493a1d88de08 Increase wait-deployment timeout
039d77a7f45ef95771890b0f89360ae43ee84c44 Merge pull request #1309 from devigned/latest-check
cbe0ac97bbf1d60b34bc71c94017f8824c274c82 ensure no latest Azure SDK API versions are allowed
f6f6e8381769089a9bf7ffb91373e51d8bf6226a Merge pull request #1312 from chewong/test/ci
7e8a7f25eda5c57398a78597fb8add592003d41c fix: point cluster templates to the correct location
874a8094c61b45cbae775cc9ec5532dac1a8ae9e Merge pull request #1306 from jackfrancis/test-ci-directory-change
f8cbcda1a7664bc059f3a2be266e24cc872cbfca Merge pull request #1299 from CecileRobertMichon/egress-rules
75fe165b2663a6a64fed26459d93ec5f3c1752a8 Merge pull request #1303 from CecileRobertMichon/sdk-53.1
92e0cdfd6607c1229e0171ab1af2b39fa5af5e47 ci: move ci test configuration to templates/test/ci directory
307eb5b0c655bb5596cad3d8282104a14cdc0507 Merge pull request #1301 from chewong/conformance-release-branch
715d5fd7363c92713086a0304152a3c3612315d8 :sparkles: Add optional direction field to securityRules to allow Inbound and Outbound rules
c0e12494969371d11debdabda7593d54b1b23f95 :warning: Rename ingressRule to securityRules
0238d1c9f4b0046d23ec5fb045dcc5196411168f Fix "latest" imports
f4c96497fec5202664c904220f654da13e46dff2 Update azure sdk for go to v53.1.0
1a16ceb38ec1437bd4de75fccb048d3f5b96ab99 test: ability to run conformance on release branches
90ec1442c466f2c01e986c59bee9e1747dd6bb20 Merge pull request #1302 from jsturtevant/explicitly-turn-off-ipv6-for-overlay
aa3e557e536eb71b73d702cc3f3c73990e165e3b explictly turn off ipv6 for win overlay
e34e11d44a5ebd1eac3f1c18b608e3ec513d40c1 Merge pull request #1298 from CecileRobertMichon/add-shyam
33629764893e5b0cee4910c1d5b4f503a7cdd000 Add shysank to cluster-api-azure-reviewers
37fe934005c1de21be479472f1741f313e8067a4 Merge pull request #1029 from nader-ziada/dont-use-retry-join
7cf0018dc6ec27d84d42ce84c92df95cfd4a7ccb Merge pull request #1289 from Carrefour-Group/feat/custom-dns-zone-name
d5e19b7c1f5a5bd6a7fc140f45b50f4a4ed59cc4 feat: add custom dns zone name in networkSpec
7fab35ec9e0b71e95976fbea8b2e7c589d6c0f01 Merge pull request #1229 from shysank/feature/541
3a8f70f6b092745d29100474235312889c7e35ed Merge pull request #1294 from jsturtevant/use-titl-only-settings
7b8e79295d82d0371bbd82844ff189bb79e3f41f Merge pull request #1293 from CecileRobertMichon/fix-providerid
7c4ec060c738ab7bdad745bc4ad700824fb472ba Fix VM provider ID to match node ID
cfdac96526e388eb6374cad5eef581fb1767627f Merge pull request #1295 from sbueringer/patch-1
936470fe434032c3729cfa9dda7ff4d66098349b add doc for node outbound lb
48152ff0b17958ec4b58d1a4fd366817eed5b83a strict validations for nodeoutbound lb
168d16e27b7ebd7acff3ed0305c98848a40f837b Update cloudbuild to Go 1.16
0dc0540eff98b8112d6e112179663709c38fcb79 wait for resources and don't use envsubst
cc4b3a5c0fafcab9cac243659fe4a6faa15a1370 Merge pull request #1291 from CecileRobertMichon/fix-crs-oot
92cd35e8fe819c5d90093667900b473e2e9d22ae update private templates to include nodeoutbound lb
5a424e566a08eacbb85fdd42d44f7554dc247ca2 add separate lb section for nodeoutbound lb
1c7ae8b0e46aa44a7a76691d53d1dd20b0715457 Merge pull request #1275 from mowangdk/validate_azuremachinetemplate_immutable
6ca5211291c3dfc27e7c14ee9f133ea598d97d4f Add AzureMachineTemplate immutable validations
465d0ef1887d606ca06cb3e9b9c2ce92def9bf61 Fix OOT cloud provider test template CNI
66b7f3a6d0265b8e7f3c3672db7d0a03b9726c5e Don't useExperimentalRetryJoin
4618030de1fa3faa4db51ca0409758a7b833724c Merge pull request #1254 from shysank/feature/1017
310bacb7bbd7567a5bde9e7cdf07cdfa149d4a38 Merge pull request #1205 from nprokopic/aks-provisioning-errors
d46f10545b740a383091b357368f1742ece2b13b Merge pull request #1287 from chewong/remove-mp
a58d1459d3d37f0f3e5bf74bcbaee3e6d91faadc Merge pull request #1283 from nader-ziada/kcpadoptiontest
d0a47957ff1459d58f893334cc5df3e591e475cc test: refactor ci-version templates
bbf2bcb783b1acda6ab3a3641c8c6a68f7dc3c88 Merge pull request #1282 from nader-ziada/getnamespacetest
cd51c9af683901f98f51265a61ff53a076afc724 fix flakey get namespace unit test
4f17b6d6844aec4cc3e71838a4a156667789a1fc Merge pull request #1285 from CecileRobertMichon/lb-windows-test
3aafa8ab29603ca7e4325735296ebb789a2ec64f udpate docs for gpu enabled clusters
a9dbe5e4bd4d82d3b22d2ae7e563333760451396 Add timestamp log to e2e waiting for deployment helper
a4e7f024058b143cba7f333ffb34aac9024bf93e remove old invalid field from template
b3eb506a8e50af2dbd34d30544b55d4760766b49 Merge pull request #1281 from CecileRobertMichon/api-cleanup
4d068b92092430d83022762927530d82ca42f1a3 server side apply for gpu cluster e2e tests
dfab8699fad5fdd86d3b82c241017d3b37516b1b update nvidia-gpu flavor to use gpu operator
b5d8dafc63a7ad76cc4d8a60cdec7bdc42b10b94 Remove unused SecurityGroupRole
15c0e592ace20ca93bbb7c0cacfb8e67f89b5125 Merge pull request #1277 from chewong/ensure-tags
6a57f89739a15acacd1cd436a8275a35832cf27c Merge pull request #1278 from nader-ziada/kcp-templates
7056251bdaaec5c41203b2151d53bea78d2058c0 update kcp templates used by e2e
4ba3dc99f2f12cd58cc3bb332b39cd9db91e1633 Merge pull request #1270 from shysank/update_cluster_api
77f9d6fd54e8f39f8743e4f479ba0cda8f750303 remove named pipe "\" patches since we have upgraded envsubst
be255afe846b7fe4dbd03164eafd82699637d59e udpate nightly build url
4b543d1fe35f4182d317e3308f6a1cea26cc5ef8 udpate capi to include e2e framework changes
a97fece063c90b074148d67707c9a6a03328e466 Fix AKS cluster provisioning errors
a62c68cba8b9766677815e32d6747d3dbe2b62dc ci: add ensure-tags.sh and remove upstream test from ci-entrypoint.sh
4f3f98b5e1d8abe2dba2a9658b4501acf42a6626 Merge pull request #1232 from CecileRobertMichon/extension-script
b5f971c1c7f512c89941e02c6f66feed569276c6 Merge pull request #1233 from shysank/cleanup/1199
4c8293fc8b8ebdebe53ce7a0382d57f110b43b71 Merge pull request #1191 from devigned/ampm-proposal
a11e517105efa0ea8ba431525d2a880436e37357 Merge pull request #1262 from mistikel/update-golongci
523431f125a9f33dde50c8eb62d3fd9200ee308d remove deprecated variables from templates
a3f3b6513460d8161c76a6b4c87636157a0cb364 cleanup deprecated variables
bc8fb005e57c54ddc96d8feb9b79225f57c100f4 fix ineffectual assignment to publicIP
b5ad5c4c8156cd02eb5447e4405c412c1b9dc64b Merge pull request #1265 from chewong/add-kubectl
fd91632297879bee8d56462b28d5be92af02b88d ci: add $(KUBECTL) as a dependency of `make kind-create`
c340b19366984943a9a711779c22de174957402e Merge pull request #1256 from CecileRobertMichon/fix-ci-version
c1e1931bb3c3c37086418c051c32bd73bfd20dae add azure machine pool machine proposal
ac6e2c260297a10b41da39ef220f2cc2efc40b51 Merge pull request #1251 from whites11/managed-identity-workers
8edd425e4f7beee27f67a864b33ac2ac687c5c66 Change CI bucket for conformance tests to the non-bazel build
60922751fdc30a0ec3e515d6f6f7c969f11913a4 Merge pull request #1261 from devigned/fix-test-output
d6fb0338b4970b0d8de6ab5bb6776bb546725edb ensure cluster is populated during a failed e2e test
a063aaf7e971c0a64c377f0de9dd5536f77f7b44 Merge pull request #1260 from CecileRobertMichon/increase-timeout-e2e
07553417a56d68755c768e2f3ad540e9c6296367 Add timestamped logs to loadbalancers e2e
83f2baaa98f9637297f3aba102554af73a597a81 bump golangci
39d55c99d4edd2b54ed365f0da3e6031540318c4 Increase E2E wait-service timeout
eab3a859b0c4055975740675b854547eeb157f34 make azure config json file generation use identity settings for worker nodes as well
d5124be8c5a5ca3fc0d7aeb977222b4a59387ef6 Merge pull request #1177 from CecileRobertMichon/re-enable-vmss-lb-test
d0cdf5c05ad83c2de495270a94965ce39d3bc78a Merge pull request #1250 from CecileRobertMichon/fix-unboundvars
c8fb8955ac8e3d9463448c323e7317a6e35b38a2 Fix unbound variable issues in test scripts
638c14f4f19fbbb665529b64c16c3677c237128e Update troubleshooting docs
342ef15a71930eded27eb4bb5fa35f37bb33e40a :warning:  Rename VMState to ProvisioningState
9027dde0b5134f85ebcf56406ea52daf13495dcf Set AzureMachine and AzureMachinePool BootstrapSucceeded condition using VM extension script
2a57133a518762a41ce3a44ceb79b96e801a5342 Merge pull request #1248 from CecileRobertMichon/fix-conformance
95ea576613408bbccc718ae85e9d8152e822131a Add BUILD_PROVENANCE to conformance tests
0969253faa8bfd4c69fe4926bec10f730aa673e2 Merge pull request #1244 from nader-ziada/azure-env-spec
59aa41837615830c946b5d32d157d1680515ac8f Merge pull request #1242 from jackfrancis/e2e-vmss-accelerated-networking
ef6fdd6c31e2d0a97e41c6f76b3f33bdf117f7cc set AzureEnv as part of the AzureClusterSpec instead of an env var
9768df7f263ed351ab839cccd3055081ab73359c Merge pull request #1247 from Evalle/ISSUE-1241
f60e91e5cad041a6b1a33d7340cddf5e907a2de1 ISSUE-1241: Bump Ginkgo to v1.15.2
63bd284d14e479a18154afd9150c7b12a2dfa205 Merge pull request #1231 from stmcginnis/klogv2
e2f9250353e42b4fb313bd77acde124f2cb21275 add test note about VMSS
0a637253ef6e87ce06c1bef9e9bbaa54a6652a6a test: validate VMSS accelerated networking during E2E
e28a93b21bc211eb796f2d48c3784c0fe600aba4 Bump CAPI release to nightly_master_20210315
6fd67de638cb3f91ab3c0a9eda2fbd9214c14285 Update klog dependency to v2
228872df531ce41446cb7e5ed16037ba56f547f7 Merge pull request #1245 from CecileRobertMichon/e2e-regions
4d03fa7c652dd23a0a0a563e17115d815211ea96 Remove southcentralus from e2e region selection and add others with quota
7744b89fe0aae67ec3f282ffd957c1214dc33a52 Merge pull request #1239 from jackfrancis/AzureCluster-PR-tags
1725218b1ab5418887a92294032d04de02c734df ci: add build provenance tags to E2E-created clusters
289f521a64021eebfae88fd739c66b98502c9274 Merge pull request #1216 from CecileRobertMichon/update-external-cp
e1149af62970a2dec8288b3f60c0a4d08db86cc8 Revert Ginkgo version to 1.14.2
89e02372ae6b65e447f9bfcae99cec529281e552 Merge pull request #1236 from nader-ziada/metadata
e4516ff018c6c2c39972d8f78ac4d35213a1697a Merge pull request #1234 from enyinna1234/update-cert-manager-version-in-tilt-module
bf60c66ab64f4bd89ce64725da6f1ab8d1cd3d82 fix incorrect clusterctl version in metadata
9a28df097ba47aed781a37f279184d13c1fc615c Update external cloud provider flavor to use CRS and add test
3f4303b395a95ef324e6773b27206a3bfcb0671d Update Cert Manager Tilt Module to v.11.0
02ca6c383c4c459efb79c8d3673f332f212f4046 Merge pull request #1228 from cpanato/update_wrapf_wrap
158a75977127edc66796b00bbbde0b0710f87158 Merge pull request #1225 from nader-ziada/dep-update
a3872cf4849edff1c3f034e4cb37d63f2ffd7a8d update capi nightly image
1c0b0505568f46ef68b0d9c69bb03a767bd91ac1 Update versions of dependencies
534db6c0d6cbe1bd6b3fb7dd3aac08b7b05c0398 Merge pull request #1210 from Nordix/furkat/use-individual-sa
d94df7695b9b1105e0576a2d66b3ad15bc2f814a replace errors.Wrapf to use errors.Wrap when there is no variable to be added
ccec4c0186af14c03219aed4aa2466800329e55f Use custom service accounts instead of default for controllers
e6a7730ff546aa6c7885083188571f06f5492a32 Merge pull request #1219 from nader-ziada/capi-e2e-fix
a31f0f1e0c83231581f0185504a0f3978f8c4dff Merge pull request #1218 from spectrocloud/capz-delete-non-managed-clusters
2e25580076af010974c0beb0fedd9d01155d36ce Merge pull request #1217 from CecileRobertMichon/fix-vmss-extensions
12b7e95f807fe34798657cc7fb7f78ea42d966ce update template for capi remediation e2e tests
a4e4f90073628ba8ff887e6b6cb3e2089dccf1de Merge pull request #1209 from nader-ziada/namespace
2c3b73789522d65f864c187f815990dc216436d2 throw error if err is not azure.ResourceNotFound
31e53a7a9b7fd93b03689f880b7c74c42c9c5d31 dont use hard-coded value for manager namespace
65b62e65c90a590fb362919d24317838bb05603e :bug: Ensure VM and VMSS extensions are applied once
b99972892a98d054bb001c9e0a6f53d2ff9ad106 re-enable ILB test for VMSS
451d034dc0c0995ab2fe88aa04c69274e8e18f2e Merge pull request #1197 from devigned/customdata-hash
9d2dd13f5f91ed5d6e370f3d1575008d336fbf48 do not include customData in AzureMachinePool hash calculation
2d51dfe4464d979b6c7753c8c1b6bf4f42f02402 Merge pull request #1204 from nader-ziada/fixtilt
5a44e4a69ea5e353b35266fad258bc0014499219 fix set network for kind
df6f747455c9ee093c00a048f0f1074ac3e7b266 Merge pull request #1203 from jsturtevant/e2e-curl-retries
4880671dd09945adb132f09c2e8d9fcde8c41798 add retries to fix issues in test env
5746ea3681a2f2c3b197b394b8978991d217dfd6 Merge pull request #1200 from nader-ziada/ctx
38b829d38ac146e16f131f5f12222092e3888e28 Merge pull request #1201 from nader-ziada/docs-type
9a151dcaec2d3ccfdb182f741941e9a351021bcd fix typos on failure domains doc
b20fa0e40dd018677aa3f8acd3a2b7bb9c919573 pass contexts through in tests
2d58abba334517ad59a3f2c7f6d8dd476bfb0f49 Merge pull request #1144 from nader-ziada/v1alpha4
55c757c661f689fff8fb818e7171472ad37122a1 apply change for Added managed disk option for data disks to v1alpha4 types
a1933198b39d3b3a2052a0590f6cbf8de49da76d apply Added omitempty annotation change on v1alpha4
a16ac69cdb04f419570ef4076139edfb8524bb38 apply changes for comptability with latest capi
70f6c5b025c2968c5c0bd0210ca0798ea377d211 initial change to v1alpha4 types
27f1cf5404583e96e076249e3c5300ac9ce49ffb Merge pull request #1196 from CecileRobertMichon/aad-fix
743055f90c36c4fed473ab8b9d30a34f3bb640c8 Merge pull request #1187 from Evalle/ISSUE-1185
7b1949ce3316f564c40f9d905694f4a7436cf730 Merge pull request #1180 from fiunchinho/failure-domain-amp
8891f16a77ee47076d4e4d6a0892fcc87e11eb84 :book: Add missing step in AAD doc
31fb9a698fbf9d3d2328a2ba4a708b2294858d0f Merge pull request #1194 from devigned/fix-ci-image-purge
b5b00cc9d23a5cb2b4736bccde8d07fc70a4f2fc fix extra single quote in e2e image purge and second repo job
e14b25dc2f22da4297bc62385f83b96d1320151d Merge pull request #1158 from CecileRobertMichon/aad-support
bba3ef7bce9a3b4aee4adec7e705caefe65f3f4d Include generated files
05ae2259b61513ed97c5f63c16803b6c58630aec Reconcile FailureDomains in AzureMachinePool
d08adf614afe66223b9fc4e29d6afb1d039d1aaf Add documentation and templates for Azure AD integration
1063282720cf2e1347955faf7170cc8566a14585 Merge pull request #1183 from fiunchinho/cluster-name-validation
f8cf6f54db7b2d6f93f2d097d5207a5e4d9c1931 Merge pull request #1186 from jsturtevant/windows-async-hash
ae7110b406ddca5a129d17ca8387bc4e69c352c0 Merge pull request #1175 from nprokopic/aks-nodepool-set-ostype
6528e9b071c0c2a59c95aab074b9205fb2c604a8 Bump mockgen to v1.5.0
a3c45cf7d831240f2e8c0426b961d5f60ea7aa72 do not include windows password in hash
0cf9e6c7c35a637bcf419b14fd0bc866f159c2ec Merge pull request #1178 from CecileRobertMichon/quota-conditions
9ffddc05bea4d7b06ead35ebdd84bd8925f29a1c Accept cluster names that start with a number
24004d5fd3b59bd487814dce49303b1773cf756d Set OsType Linux in ManagedClusterAgentPoolProfileProperties
b9c90e48157f63f9b3321a1cdccd0e5f2a3f21d0 :bug: Fix AzureMachine terminal errors
7da9a97f9c10afb26afaab3ea18435312a94dcc6 Merge pull request #1163 from gdhuper/gdhuper/add_managed_disk_option
9f6f5a250c29914df8328d0f2e68621eca6645d6 Added managed disk option for data disks
8d535973df7ae2c40589cce945011cae1439d28e Merge pull request #1170 from CecileRobertMichon/tcp-probe
f38e930650b8aace014f8e1b0e490dd9f7ad7748 Switch LB Probe to TCP
417eccbe0ca8a433f44d1fb2a3a473c494a5ada3 Merge pull request #1169 from CecileRobertMichon/owners-emeritus
9bc6d4fc6310276aea76dae96a468db82a5175f6 Merge pull request #1165 from nader-ziada/cap0314
fdbccbbb964e25376e258e5842d1cec5a235e57c OWNERS: move awesomenix and justaugustus to emeritus
2276bf0780b3d6e6479e57a88a1b215e4487f493 Merge pull request #1164 from whites11/azuremachinepool-status-instances-omitempty
e7ac15ef00cf9e67d791f032bd8804068ed3d6b6 use cluster-api latest release v0.3.14
6f51b4ed99e0816761eadcfb26158f745f54f1d2 Added omitempty annotation
779bd18ca8005866ba944c09d65efc7cf7cd1d91 Merge pull request #1156 from Evalle/ISSUE-1154
e15f742eacdc4c684c47283d3b348216a74643ff Merge pull request #1160 from shysank/fix/997
b366f62f5f147e796b36c0f83011ec61e7fc8a0a Merge pull request #1161 from garvinmsft/master
5191709227e92d0e6345a9135bb613c008f8aabd Add a missing code to skip NSG deletion if the vnet is unmanaged
8373a92dc96205bad9c9fb5834709e379ad23bf6 use internal kubectl for tilt-up
8924038de4642517d50ba7e941fbcb11dd958e03 Merge pull request #1149 from CecileRobertMichon/managed-clusters
ab7cca07fc16f89e9faee7f3b1ed243c3f01b011 Merge pull request #1094 from surajrana93/master
aca87615b0b57f92bd7c8fdc713eb6328eba473c Renaming Azure.Service -> Azure.Reconciler and modifying the cloud package to azure
54397bbd16532ab663730f383efc1e4d48fc6fff retry ssh and collect boot logs for machine during cleanup in e2e tests
2fa0cef02fd0161e5b51478b009852ba039d7c81 :book: Refresh managed cluster docs
8df269291bae09a1873fa13619c03617e0d7e71f Merge pull request #1157 from axbarsan/fix-amp-spot-maxprice-not-serializing
3985d63c9f370e8a87f757f79515d989c23b0ff1 Use apimachinery 'resource.Quantity' type for the AzureMachinePool.SpotVMOptions.MaxPrice property
9f1dd0c9105afa182aceecaeb5e8949536cca31c Merge pull request #1136 from CecileRobertMichon/activity-logs
68169f8d57550cb7d6f944540236935c95787dd1 Merge pull request #1146 from CecileRobertMichon/images-warning
81d8798b59330a9ec83d4403a99e9bd3cc1c935a Add Azure activity logs to e2e artifacts
f5a7f42277062037bcd00f333826a628d0e19d29 :book: Add note about security fixes in OS images in book
1a1269a1a99bafafa5a4945d115149bc413d5d22 Merge pull request #1143 from devigned/gosimple
19ea37919e2c98a2bc632688373a57b44be0cbe9 add gosimple linter and clean up linter violations
e1e60e2bee79bc6bef856752910bae23962980a4 Merge pull request #1137 from shysank/feature/as/workernodes
f820befe48bdc94e436e3ca006956731c6652e15 Merge pull request #1142 from cjcullen/patch-1
a8cc6750fa8fee4a8c68fde03a8ef363a660e06b Update mdbook to 0.4.5 to fix CVE-2020-26297
8bfb7bc9d7f76a089c2fa752e5ae7b30f99b71b7 implement availability sets for worker nodes
5cbe35262bafffbe533cec53b58d1e61c35a509b Merge pull request #1081 from shysank/refactor-1047/part2
e8f327d183af7a2037494196faf4fa2ebe401797 Merge pull request #1141 from CecileRobertMichon/lb-reconcile-merge
bc3657dad85dbff58038e3b95105408146d33abb Merge pull request #1140 from nader-ziada/0313
5aa90f6999fd3981a7398fe22fe233a010859e23 refactor to decouple service instantiation from controllers
986ce131d6999453328b898cb6c876d130a9fd6b :bug: Merge load balancer properties with existing properties to avoid overwriting cloud provider rules
dc6cfd70c118d18ef60615904f556f2fed26122e bump capi to 0.3.13
e52b0cec87d1d8c58e045c4c5b5eb43d2f15b7d1 Merge pull request #1138 from shysank/fix/1133
f13336999f451858c5cc65d97e018788348826f9 Merge pull request #1107 from CecileRobertMichon/linux-extension
ed0de07741fdcf560d70d10d3e14380030ef4e5d Add Linux VM and VMSS extensions
78a4ca2251f9f73048759d887f2bfabd6c0828a0 Merge pull request #1135 from devigned/fix-iface
e7ffa8efe0cdaacefff759ce73d990d91931eafb Merge pull request #1067 from devigned/async-mp
1eb1438cc51666ce3b1351136b453abb3494abad use non root numeric user
aafdac6677ba5c605457c8188c146a3c8338d83b fix availability sets when fault domains exist but no zone specified
edaa96440c149b987329c322dfe9666671dbe058 implement capi e2e.ClusterProxy in AzureClusterProxy
87561e006b62add68700ab32665c16572b4a3571 enable async reconcilation for azure machine pool
4141d33d7e897f46274ed01b1fc133c13dd802b3 add time to live least recently used sku cache
522db2e1968622ffd43a7bed1840f851a0dd1afd Merge pull request #1132 from devigned/elb
dd0d7acd32f9c17c1268fd4bbd9fd6482c49e04a Merge pull request #1126 from CecileRobertMichon/k8s-1.19.7
9f44c78dbb3caf27bbfcae5bbd9985d1c2e25290 Merge pull request #1110 from Nordix/add-errorlint/furkat
137d145749285bf20ce3cfe2e87d8f1daa0ebc0a reenable direct connect to elb
87cffe17148e5a3c9ae7a7620d5faa368c9782ba Merge pull request #1131 from devigned/disable-ilb-test
c0d8e366f12de60733dcf8d20ac456ef79ef3a71 temporarily disable ILB test for VMSS
a25e5176015383454cd2bb8fe6412e78b39e6598 Merge pull request #1117 from nader-ziada/identity-doc
e218a13350eb60305471c257f6bf9d19a5545019 Add doc page about identities use cases
a90bcc0df92812165db0785b08a8004d79163c0a Merge pull request #1121 from devigned/cp-logs
51851ecb6f6ea53530d6acb3eda6dfaebe88a76d Merge pull request #1128 from nader-ziada/windows-httpd
fd806fc9353355dd92cbcf20f5f4f0c79710c368 use smaller windows httpd image
ae02111be7c2c7fe2ce064f8db02ce9c5f6986b8 output kube-system logs from workload clusters
6a80ae3fd5d80267b55432913ede0c3fb0debc49 Merge pull request #1109 from CecileRobertMichon/update-roadmap
b6ce82b41493596b0f15f3cfa94a2fe0e68da569 Merge pull request #1120 from nader-ziada/delete-stuck
9cbfb3371a78c800684e3a92a3b22ef57b2cf11d Merge pull request #1098 from Nordix/azCluster-validation-furkat
fd959a87b2f8feca2f25754f315dc1afad6b138e Merge pull request #1099 from shysank/feature/657
f1430845a22e952edb20b55f2be198eb4795bdc8 Merge pull request #1123 from devigned/lb-test
2ce27e6783e6f83624e3a90587b070063ef32dfe disable external load balancer test from outside of cluster
dfb9e66f2d2c853edb472683cf2f5354997ce152 Upgrade k8s version in docs and tests to 1.19.7
e7ebdf3bef11fcb5a6e001b2860ae8d6654e0202 Merge pull request #1122 from mboersma/fix-gpu-book-typo
98481cfeedfe0b17f685c4c0362fb7489ace87e3 📖 Book: fix typo in path to GPU topic
4fe0c58f5c75544894bc3ecf4cd948523343968e add a check to make sure group exist when deleting
ef693da03e00a7a6f2bad72456e603f1c09856d0 implement availability sets for control plane nodes
9c0af5b747a4da506c0b55db44c501ff03754a4b Add validations for AzureCluster Updates
a3525d2d89821192dbaeef270f46eff09e4c4587 Merge pull request #1111 from Nordix/add-multitenancy-to-summary/furkat
6fd9a796b31592f99bfa7c8008e11fe7957c06bd Add missing multitenancy to summary.md
2e5dc062dfe7076919a46eb20a7feb1efb6326ea Add errorlint to the golangci linters
02cbfe62a184ea5313aa758ca71be109dfce708e :book: Update roadmap
f46baa1119d1441f263a4a5437d589b46367eae2 Merge pull request #1106 from Evalle/ISSUE-1088
725a7de792cb03e5a4a7229e59a343bc65abcc37 Add gocyclo to the golangci linters
c3ec13f5f22927cdf6b41ab164157f6a188ab30e Merge pull request #1101 from cpanato/update-tools
7fc51795a55417095be8a2129f5c70231ce436d3 tools: update tools
4a568429070b839020f27085f94e7764274f6add Merge pull request #1089 from devigned/mt-proposal
20aef6943de9930f567d6b75c2983415e54453ea Merge pull request #1036 from jsturtevant/windows-support
e22855d7a19ebebc5e40020db7b1637c053676f4 Merge pull request #1100 from Nordix/fix-typo-in-cloud-provider-az
3ef3ab56e85d3b815880395eefc094a8d42f7910 Fix few typos in docs under /topics
b69480fc45af0426f3264b4529a030793eb0ce06 Merge pull request #1076 from CecileRobertMichon/bootstrap-detection-proposal
313cf0771c95d7f393a5e2b65795287ec175ff21 Merge pull request #1093 from laojianzi/issues-1086
5763b8b7bf859066253d2980e4d9267f20978f76 Merge pull request #1092 from laojianzi/issues-1085
35bf449242c91006a5abf5b61509a5faa2c5f309 Merge pull request #1091 from Evalle/ISSUE-1084
b1087d641cccab2ebf5e331463215b4e09884070 Fix a test
00ab476a72b97d6211ca71f6565973e2351da198 Merge pull request #1096 from jsturtevant/chore/default-logs
a90e722689e4595917a83470876afb9cabea6965 Add default log container for kubectl
507da8bb110dcdb7ce0c752a53ab119bd5bdbffd Use windows httpd upstream image for faster deploy
9f4589d2578e745b808446191fa535a83801ae43 Add tests for machine names
736a04e8e5a2045b146e4a8c8a2c4084dca202be Add Windows Default image
2758760f7e4ece6115d60565464d8de5d160e0d5 Fix for crs which drops \\ on windows named pipes
b895dfe06b1b29e03e63ac8a5e5e2d6f61b15d8d Add machine pool tests
68dcfbf43e162445bdeebfd535c1a697a109e7e0 Add Windows support to vmss
2bc6a358effcb1f119150446be5f1de63a5ca397 Add documentation
460b51d8fc4e6273a0ef2f4473e0c175948e71bf Add Windows e2e
e753a32fccdf6b825b606f12bb1acd6e34a70339 Initial windows code
980b22e2e4c9bf24355cf6ff16f7787d35b0a5f5 Merge pull request #1070 from cpanato/GH-1058
1a27ca152c9fffcaaf490075767897f2bec1e3b1 debug/kubectl-capz-ssh: add AzureMachinePools option to ssh in the vmss nodes
3e168e89ca7f5e4613e050b0c55ceb1c23893d32 Add errcheck to .golangci.yml and fix issues caused by errcheck rules
f7609013b258d74a90a351f0db9059611fbf8d5e Address linter errors
6d9d41992e0da498b7d7ba44a1ce0432813faff5 Sort the linters alphabetically
d866d3aadd588f86a3fe36e1aa07c71b80e960c2 Add unused to .golangci.yml and fix issues caused by unused rules
c55aa65247ec97957fb2c36716a42432aaf2cbd1 Add staticcheck to the .golangci.yml file
b54731647d45aaf43446419bb56057524bcd991c update multitenancy proposal to reflect our learnings
7487093d94453ee60fb64bbf5152fabe7f7afec7 Merge pull request #1083 from devigned/imports
82277309a2bb2cc402340561327a1516ed4e5558 ensure imports stay organized
591631eb0d19557bfbae1ac625b620db27b4eabc Merge pull request #977 from nader-ziada/multitenancy
06a4b3c38dc43190bf6c19bdec66dded7fa5b517 Merge pull request #1080 from CecileRobertMichon/rm-flavors
73ad2c857bfa5a91d413bc261e107501a1053989 Merge pull request #1053 from shysank/refactor/1047
368ebd0afa65c1258a532cad0fe4632da30c75b8 Do not delete existing templates as part of flavor generation
d52af1abd6f530b10d906819b1af383b67f04239 switch to using getting identity values from internal type
ea3c5780265fabd5a5c11eaf7a7faa20ae77533d add e2e test
df6bd318bb28b717d6f7c17d7cbc296fac497135 using aad-pod-identity for multi-tenancy
2ac0c4ee805c15b88a668d2d472dcdc9d62dcb07 Merge pull request #1078 from CecileRobertMichon/capi-v0.3.12
dcc68d6f31c50d16e7389a25917d546c60f62d07 refactor azuremachinereconciler to inject azuremachineservice as a dependency
2518d26ebfa75043c5dbff713beae92bf2492495 Add bootstrap failure detection proposal
d1c81f0f3e0336c8631a32c75c06e5abf0e1de92 Update CAPI to v0.3.12
700eeeefcc28e7b53e6c582129ace4d7c796825f Merge pull request #1073 from ncdc/ncdc/emeritus
6f9e3eb97a79763ab5ad03e1f47545d25f8860cc Move ncdc to emeritus status
f591d6077623e77388901465e0b7aa8bb40cbeea Merge pull request #1069 from cpanato/GH-1068
eea4b799765a903f9b6612b0c0a8c2c97bab2c94 vmss: Use computer name and add it to the status
6783e86e73a7c6f3c1c5cd0479a684f2add9afab Merge pull request #1072 from craiglpeters/master
43f2d992c115beea438b4baa88a1bff64a9b981e Removed 'Implementers' from office hours
2942bf32843b404b71bb259843e6c68fbcc435ff Merge pull request #1071 from paulbouwer/incorrect-kops-reference
90e89101d1a4ddb6a56c528a12f2b056a3eeeff7 Correcting reference to kops
fbfacbbff9b9a17c2696a01415da23e95012b85d Merge pull request #1062 from dr0pdb/spotvmss
f5817038c1df10f446131203a450cbab0097c303 Merge pull request #1065 from CecileRobertMichon/getting-started
9177ff93e2fba764593692af661869fed78fd137 update docs about spot vm support for machine pool
73965884d2d733595ccf16941797e3b9118c6044 :book: Simplify getting-started.md and remove broken links
5b4efc4883d6625a8e025abefaca793b7e8b38f1 Merge pull request #1063 from nader-ziada/nsg-rg
6c24d95f56061419573acc12254c49f207c26820 setting securityGroupResourceGroup in generated azure.json
5d607e013c86c0cb7eb7bab32c534c34b451605e extract spot vm option helper to cloud/converters
b608470f59d54707fffed8c3112a47b201c4633f Merge pull request #1059 from nader-ziada/1031
8ef20c68cae8aca81a5d7635592a63d24a88e0cc Add support for Azure Spot VMSS
d58a89e486a10e7168ff2978c9e7ac38ad0d5eb8 Merge pull request #1061 from CecileRobertMichon/image-buildx
0e65fc3448fc4564679160096681d4548962ed8d :wrench: Update Docker image build
99a04899a5196cb2e27572d3427480add9d953e6 Merge pull request #1057 from mboersma/always-never-always-do-the-right-thing
9a0a059ff91ccc4bc94276f5a5cc4cb908d7347e Merge pull request #1032 from shysank/feature/1014
e02af4b28cd200a5a28cb962a7393386ab0c9656 update error statement to not show stacktrace in resource status
3004a5e0a3202c151e9583dd0cf38c54a481e705 💚 check for cluster == nil before dumping logs and deleting
1b99af883b931b02fb09729fbfdfcede55db9bb8 Merge pull request #1055 from Evalle/ISSUE-1054
568062434557672c9215c1ad3d7f77d8e7cdb55b Parse identity parameter correctly in kubectl-capz-ssh
37b83321997721f8268bc99b43d95a45fede7db8 handle terminal errors to prevent reconciliation failure loop
64c6f5320fb074da5b272d22917248153c7461fd Merge pull request #1049 from Evalle/ISSUE-1037
8f3dd96310a5106a2086d4a3118f7de1f3c90598 Remove failed provisioning VM deletion logic
d1fe59be07c10dd6a66681f89448feb69585a78f Merge pull request #1046 from mboersma/keepin-it-fresh
c8b05609027041ab52b4709c0acd7f251b0bd5f1 Merge pull request #1052 from nader-ziada/capi0311
4a69ac7ab639e3417741e29b82fddbb13788485c bump capi for v0.3.11 final
9e1eeaa4d7fb3d5fbb10ce8f37c91d4a2393e22c Merge pull request #1050 from CecileRobertMichon/force-delete
48cc6317a288589c466a2a8fc7751ac41a6af644 Merge pull request #1051 from CecileRobertMichon/book-readme
50d686d270cbaff4201ccf9246f8a6b275e7f9e5 docs: Cleanup docs readme
8e70ad63eab71ecaee62eefd90f6bb5d7953f869 Merge pull request #991 from CecileRobertMichon/calico-1.16
2a3e737f129f6ab6653794dbf86edfff2469c271 Increase wait for ingress-nginx controller timeout
1f3f742c2669c63f1b60fa2abf570ceb7d87f87f Update Cluster API to v0.3.11-rc.0
33345d23e38592afad0144c1f327707b73285b64 Merge pull request #1033 from CecileRobertMichon/private-dns
a42a1490599b5682ecda15e4b07a042d60dc2c3b :seedling: Update Calico addon template to v3.16.3
0477320a794b609be2e8c64ce7ea929d29db7821 Merge pull request #1041 from cpanato/update-deps
10eba4793cc7f90ce82a7469b08e17b6761cba57 Merge pull request #1044 from shysank/fix/1042
9f5e341e34b7d37fa41a809dfb654565535cb8e4 🌱 update Kubernetes versions in e2e and docs
5ce2cc61a6862852cd7ed7229757422c6f6b7dfb Merge pull request #1043 from CecileRobertMichon/fix-creds-parse
35e6c264b2211849597780803faddc9b42af4a27 fix error handling when vm is deleted
b40de4c309f4d3eb88c1c0d880d023c6f2c1ed56 Update prow creds parsing to include new multi tenancy SP
a0e422a4c947cc22dd388617e763f2814da73c3b Merge pull request #1040 from CecileRobertMichon/tilt-flavors
0bf5c238488ba0299c0007668852491de871cbe5 :sparkles: Add support for private dns zones
0e7584aef2254e7b5800f234ea6e158e69f93dbe :wrench: Tilt auto-detects local flavors from templates dir
4e9c0d8ef4b2b6a90f82bd0df88fd3d15723a7e3 dependencies: update imports due to deps upgrade
3dfd1e6e0e32471e44ef1e6c5f833a8504566150 dependencies: update several
b77c94a09e03bb3b54b5f016be7eb4b3ff16daec Merge pull request #1039 from shysank/fix/1008
34ebec59980ee43e30ebc7c4db4bf01de1091cfc prevent vm recreation if it was deleted outside of capz
95283bed2b4b044269df5569880fe3ed39fa7095 Merge pull request #1038 from cpanato/update-hack-tools
1cee310a3e5d83965f368f011ac6a3c0867fdd60 hack/tools: update golangci-lint to use release v1.32.2
cb486c3d7b26dc84ad5156fa97773ccb97578ebe Merge pull request #1018 from CecileRobertMichon/conformance-ci
e678cd2625ad11fb81316d1e3dfc6295fc6b9aa4 Merge pull request #1030 from CecileRobertMichon/export-rg-name
908cfbc5ab2c0c8abc86243dc9ae0b4624d4c479 export Azure_RESOURCE_GROUP for CSI driver tests
a408cc4c4f2b3e45f31a5bc0b2f7fc90afb76b98 Add ci version conformance test in conformance test suite
d531755078486360b78b0d0cbbbbe5a1d01a5552 Merge pull request #1027 from shysank/refactor2/1001
b1b0a0b95e052d08f1dab433655c1a6570b61d8b cleanup virtualnetworks
ae4dafa74c2ea7c7e632ece30d6758fb488af6b3 cleanup virtualmachines
1787fae9d26348f0957d88b8db3aee209a11802e cleanup tags
fca728a81861b77452ea4ecbb37f044fe8d34f70 cleanup subnets
1b229583798037e6c022acd53f57c4c4d36e67b3 cleanup securitygroups
24176a2a0cca8f7f02a75a5957ba39cc47a8d262 cleanup scalesets
9167e8c8753a31dc25e3fa9dc37904587ee9bd36 cleanup routetables
f6faccb0956e209c99fba458e0dfe78994ee0f4e cleanup roleassignments
feca9a46acc5870e37a6f652760df109c9980e8d cleanup publicips
422be0e2a5229345bea96edc86a350c2fa59304b cleanup networkinterfaces
3ceff1fd7c454da65cc64a313e494dd8ca4c0a83 cleanup loadbalancers
79849e951d0b5ca1c46161ecdd0f4fd93845e1de cleanup inboundnatrules
9e254f247914fb75a1b94c81be4a5ab4e9f180fa cleanup groups
a8b9860987c1d5b21bba6ea9184773057c6dd64d cleanup bastionhosts
1e68dad9846ce5fc67f258f9edfc99c00a049e3e Merge pull request #1022 from CecileRobertMichon/spec-array
dfa066298817861f39d827381606c402b7e90156 Merge pull request #1026 from alexeldeib/ace/skip
f860dc489b44757cb7a847263d1179a2730eec3c :bug: fix e2e skip for local testing
45fb80d54ee124928f4a713a6fdd866f25e4d913 :gem: cleanup: VM and VNet spec no longer return arrays
2dfc5ea4acb9bc037349516d6a75a262606963f1 Merge pull request #974 from CecileRobertMichon/private-cluster
fd5c6ad88d9cf6175e8991f5a03b88a2cd9c8033 Update managedcontrolplane.go with added NetworkDescriber functions
d165cc7c38f64a02e46cb101ee43401fb46c325e Add iptables workaround for hairpin routing kubeadm init issue
8f7acd9e51635bd8200dc93bcd1f0e524966abf7 Add control plane outbound lb
bdb8fc3d912b51a03553b038d18911808f15e40a Add private cluster E2E test
aec76b10d5055790ba2387192ba61d561c372d0a Add api server lb documentation
8482bc80fc342e59bb75fab87ea8a165f5d4cc9a Do not delete public IP for BYO API Server IP scenario
12032805ca563966adb6ef561d439928151d19a4 Enable configurable API Server Load Balancer
f8f2ef1b0155330473df2b6abe4c44f5107f7f8f Merge pull request #1019 from devigned/metrics
74df4e260dbf1ec76c26b044d5ba0db05c9dda99 Merge pull request #1024 from alexeldeib/ace/mcDoc
9c8c56d9200b795ad7ec591d7a23b973434a01f3 :book: document required feature flags for aks
33c5e7b415e44856d3924b397ece15ae3c64333b add developer documentation for metrics and tracing
5ff8051703afaba778442b48f76bc6a34a3bae81 fix context matchers in tests
2cc75f4e6be222b7340139614adfc7b03f8cb612 add prometheus and wire up metrics
bad0f62729a252611fa02f1d653fabc96a83ec3c add ingress support to kind, deploy jaeger and trace AzureCluster reconcile
fd51606abfd0e34c748e7612ec0dedefeaf831fa Merge pull request #1020 from jsturtevant/e2e-deployment-logic
c613c3bef6e3619ec31c17f7c4aa71697175602d Merge pull request #1012 from dkorzuno/encryption-at-host
811d7afe0ab670b1feb3ddfe446a66913b323c92 Merge pull request #1005 from CecileRobertMichon/k8s-version-e2e
9c2b417d7103ec663cb2ceddc7bad760569d9a6f Merge pull request #1021 from jsturtevant/docs/e2e-mgmt-reuse
b06d06700fc0b45c82d56b86f1f2e48a35eabba0 Add EncryptionAtHost parameter
9eb212380db6895624c4fdacf2c03dcebafa0f14 How to re-use mgmt cluster in e2e
a724144aebc2fbad01b4462be2405c00463ed7b3 Add logging to local e2e test run
de88326e512b7fd5df17d8e2371ce0b421f973a3 Remove duplicate service code
c7421281d911229dcecfe095c6f468000929e6a7 Extract curl job logic
c12a58ebd631d50b903153a1cc5924ec505f22e4 Refactor to use common builder logic
3c5cb5b975548137d1675bf685766d624bcfa48b Merge pull request #1013 from shysank/refactor/1001
2bcdc7b00925f518f259c770fa8e94459a927667 Merge pull request #1009 from alexeldeib/ace/reVnet
ee66de2dd22be6190266025b2e1755ec30c96603 cleanup disks service
272261b395983b18247850dfb979ec4c41717632 Merge pull request #1002 from mboersma/nvidia-gpu-flavor
1d9ad209dfb5a3d8f93d871140d4f039066f3d05 Merge pull request #978 from nprokopic/azuremachinepool-conditions
254746e99cd7edd0a97edc61983eaa9d72e70fe2 Merge pull request #988 from mboersma/healthy-time-sink
140bbc3846702aad0a1bdce54215cbf84a8a0b00 ✨ Support GPU nodes with "nvidia-gpu" flavor
14a716da78eb0d84e4be1483f942cb9f39eb7c48 💚 cluster should have healthy time synchronization
7aae52315423dfd25baf29b6ae3afe24992b5718 Merge pull request #1004 from shysank/fix/960
b46363752fa379b899660b4e26cf7c57af7f369d Add support for managed identity in machine pool
59bc01a379e3c54912f389c98d857e58062e21d7 :gem: provision vnet for aks clusters
7e3a74057c72c7b1c5f73deb51be07ddc965af0f Update default tilt k8s versions
9fe0600616483cad2d2574eff48697d636f666ca Merge pull request #1007 from arghya88/redundant-nil-check
f68b4844e8831090e63a0caf1090ac3d30bea87c remove redundant length check for errors
e92bba9b95d18578e09a4eaad1c1150c0c6f5516 Merge pull request #1006 from CecileRobertMichon/wait-makefile
bd73de75dc1aa2613e729384b76142ddbab4f7c6 Update E2E Kubernetes versions
76d783635f3c1d40fb6a16091e4f44c381b199d6 Merge pull request #986 from cpanato/GH-971
5a0d4ad8fde853ffe8211f8eb2942cb84eb65ea8 add a capi webhook wait to fix kubectl apply error in make create-management-cluster
e47947c7ba30b05bca5e85c62d34c58db5f5af97 refactor conformance test to use the capi framework
9b8b494ed7324daa6ffaaa2756c81f587c178e23 Merge pull request #983 from devigned/mp-e2e
8a339cf388b7a521cfa76bf5fedba0145758ce73 add e2e tests for azuremachinepool
2307c8cf182db51ff8901e08356897caac9d4798 Merge pull request #993 from eratnch/tilt_manager_ext_az
59458afe3f11343e1641fd8b154474a1c91f0a78 Merge pull request #980 from mjudeikis/add.osdisk.encryption.api
6da6061738b972f8b0408a00e275694bc213b62a Add disk encryption option
4ab94abee09e37a8126d86ddbebb8d309f95028e Merge pull request #996 from mboersma/comments-required
3cb228ac7d42059798433eb7722a54f547b56ffc Use tilt cert_manager extension for CAPZ
d0494d2bea2522bd733a4328af7561c937801ebd Require comments on exported funcs
3da52a303b650521e86ff0d56dfcca15e926779b Merge pull request #995 from devigned/fix-tilt
0d68b3d4c73218cf508bf2d2f588b0e6b03c5d2b add a capi webhook wait to fix kubectl apply error upon startup of tilt
4b2fdbc3e11cac7174f16db7202dff6bc949825e Merge pull request #976 from mboersma/the-log-collector
144efc5b37ace910cc37d22cb9bfa3ad90d1fdc4 Merge pull request #989 from CecileRobertMichon/WaitForFirstConsumer-storageclass
2cc2b7bfab7cc661161cd3000a3a3f3d20994a40 💚 collect workload cluster logs in e2e runs
38c2360c4caaaf6060860c279f45b64bedd54406 Update AzureDisk SC volumeBindingMode to WaitForFirstConsumer
6d7647a1f35dc20f6cd82625528353c1dfa777c0 Merge pull request #987 from CecileRobertMichon/fix-ci-version-image
2a098cd762e9d01d3c0474254d961dbc5b7289ce Fix USE_CI_VERSION marketplace image version
a985e1e228913c293d972035e729fbfc03334d28 Merge pull request #984 from CecileRobertMichon/network-describer
3b5ed138b336f8021c6f467ebed590aaaeb7340c Merge pull request #985 from nader-ziada/conditions-delete
f621f73f67d65f1dc2e392898c464ad7a4bfc021 :gem: Add Network Describer interface
a62acc83ddef8368439b84868637ed8bf68f6020 Add conditions for deletion workflows
2e100d19787016a78130fd5b9440dedbad754c85 Merge pull request #816 from nader-ziada/2routetables
c3ccf47ce4e367536dda634944c6c9b6acfe564c Merge pull request #967 from CecileRobertMichon/rm-calico-apply
d2d727c0fffa1caa41fbca2f8c0f47a056950604 Merge pull request #979 from fabriziopandini/remove-integration-test
81728bb006490dfdc1d99eb4f30251ca018e9534 Fixed copy-paste docs errors
45c7a3ee47b0b2ffaea7a3c9878d6680deedc09a remove integration test
c5fed9ef9b520c2032fe39e4a5e47c1b247b7d6c Initial support for conditions for AzureMachinePool
27f33d583c749c6e8f4b28178e988500e7ffd885 Merge pull request #972 from CecileRobertMichon/readme-1.19
29ba7f37f1f1e2274bee24bc66ef9561dd158c73 Merge pull request #975 from cpanato/update-deps
665d996178d91596f3d5de5e2e2c668424da311b dependencies: update several dependencies
bf9bdc00c1fd6356f53c892dfbacd8359d2785c3 :book: Add k8s 1.19 to readme support policy
3a817fe6bd971d91a25e0086d3658d32fe113f24 fix make create-cluster target
d4584fa483f4ddd18ac893730c06dd1dce51414e :seedling: remove calico apply step for non-prow templates
5e08e505dadfec65ecc6cf3ab0c5a44cc474bf16 Add the ability to have different route tables for control plane and worker
4195d4cbca1224ff2f552a608f7cab2fc3d1007c Merge pull request #954 from nader-ziada/capi-3-10-rc0
9eb31409ab83b568687ee5c6388719ebe7c0d435 Merge pull request #963 from nader-ziada/ip-across-accounts
611bdb7d66b228e34146306246856a978789bccf bump capi to v0.3.10
d82721b2694d360ca677468a8b2f03d877be40a4 don't set the DNS record for the outbound public ip
5392d74bfdbe3f2ab387eb7900274181241b5d8e Merge pull request #959 from CecileRobertMichon/fix-uuid
2ef20456b232ae479c60b65ad5cfeda4f8c3e6c2 Merge pull request #925 from cpanato/GH-897
b28e91b9db52d2e83cc0c78ee3aca2489a3819b8 Merge pull request #969 from CecileRobertMichon/third-party-optional
360dc476793723f13c7bc633d916cfee23df1d82 :bug: Make thirdPartyImage optional
4d75fcc03d81562a7fa24ba0bbb20cddbf4cb765 Merge pull request #965 from CecileRobertMichon/fix-kcp-adoption
84885cef0c93bb9d3e7f560e1587bdadebd46ef5 :bug: Make role assignment name deterministic
121244f2b3dc885374e90f57e6b37954cdfe0676 Merge pull request #951 from gab-satchi/cloned-from-template
fbfd231065a4c3359be8cd3f312eee41d40a6a15 :bug: fix kcp adoption template azure.json secret key
0c45468b245feb28565bba57938511c3cf3f5f59 Merge pull request #927 from cpanato/GH-909
20517fdbe8af9ba47b3d80d2aba789c5d4935c6e Merge pull request #947 from CecileRobertMichon/crs-dev
7a23372acc26849bcca8725aef5874bd7a58791f Merge pull request #962 from nader-ziada/pr-kind
5f71ddc4e2f6d183bc075d78093e1e281b3c502b Skips creating secrets for machines cloned from AzureMachineTemplates - Specifically applies to control plane nodes which don't fall under previous checks
521cb92d6e81983453df0dcaa9194b2821a014b5 add a comment in pr template for for pr authors to add a kind
d816b6a176a21097051b0c684c9048aa585090e5 book: add documentation regarding storage drivers
f3e7a3531e08038b448562abb18cc828bc2310b0 refactor ssh key generation
3c82eafd5695514ee4a162b09df947d37045e4f1 templates: make AZURE_SSH_PUBLIC_KEY_B64 optional
723f2415eacce14332993ff637a3f7f0bbdc62db AzureMachinePool/AzureManagedControlPlane: generate ssh key when is not set
111a0de90b575fab1842d487492f01a316c944e9 :wrench:  Apply calico ClusterResourceSet to tilt and dev clusters
110f084337f64c49a13b01744a2e6d03dba55d13 Merge pull request #646 from jsturtevant/ipv6
c05182f6e9871ce529ddd645ea0433bc262ea5eb Use ClusterResourceSet to apply ipv6 Calico CNI
73b0396227f6b08e933e086f40c1ae34fda5993a :book: Add IPv6 docs
4082ce3de1835ba6c35c1e3cf612a51210687a73 Add etcd health check and CoreDNS postKubeadmCommand workaround
148da2ddf7adf3fb9998ebccd211cd5975734c50 Add CIDRBlocks, deprecate CirdrBlock
138e5c58d5d9e84e05e97fdb694489bd27fc14da Add single stack IPv6 support
bc043d3ae054fc34de3f449a274adfbc15522390 Merge pull request #955 from gab-satchi/921-worker-creds
5f7473fd8221248ca01e35365e4e862a27bf5acf Adds both a control plane and worker node azure.json - Modifies templates to use appropriate azure.json secret
b19460ee0912ebfcc3c9e0acebee7f221c368ca9 Merge pull request #878 from mboersma/http-more-retryable
d1c24e6b60b1eefe6a687c4cca4b23cee0c076d9 💚 log failed e2e resources and related events
fbb2d55b0e72b4ef8fc6aa56d6383cc37c4a658a Merge pull request #956 from nader-ziada/delete-disk
5e9c2fb55eaad02a13853754103ae4770b2d7ca5 Merge pull request #936 from mboersma/e2e-parabola
8ecb0da5017e4f838bd96548cf25639ac7742b09 💚 log elapsed e2e spec time and Ginkgo node number
cd8f5e7ee5f8abf4b4923409e3f74f1bcbe078e2 Merge pull request #938 from CecileRobertMichon/fast-delete
81df8291b5ed12a2d1435627de89200ef8c6d1fe delete data disks when deleting azure machine
8a15f6cb662b3fc0cc55a740f258633a2bdfeb0c 🚀Only delete cluster resource group when entire cluster is deleted
76128245f97a0f50a9ae2c49ce96793459503d07 Merge pull request #950 from CecileRobertMichon/remove-bastion-status
0d347d9b4dd78d9e34a4dd4184c6b39a282bc110 Merge pull request #949 from CecileRobertMichon/ssh-priority
4ea23faed7480e7577f88777b3c543a1bc97d29f :gem: Remove unused AzureCluster bastion status field
a228edab322fc9178a15d8c1f3146c35addcec38 :seedling: Change default NSG rule priorities
12f49d8c160e8eac05b1eec103f468451164d7e5 Merge pull request #939 from mboersma/lost-focus
5e1d612a196eb16424a5e5c06e42b2754e268e6d Merge pull request #946 from CecileRobertMichon/fix-system-assigned
8cdfe2d87476abc3467446a982483421d67fe9fb :bug: Fix system assigned template
0c7c50db11722a83208322d57832fa07bffa104f fix: quote GINKGO_FOCUS flag in makefile
0184f1deeebde5caa42ca067390d476efc148c2f 💚 default e2e focus to Azure cluster create tests
0973b4356263788293609e27ecdaf05208402a8f Merge pull request #933 from CecileRobertMichon/e2e-fixes
f6df267ae375c380b4f1dba41d32513d5c29dca6 Merge pull request #945 from varunpurohit76/#940
79efc61ce4abb26580d6ecfd4488d046d38e7563 bumped mdBook version
92b465d97ce2e5535b87993f88e9b565bc66f41a Merge pull request #941 from nader-ziada/pr-template
5a8fb9a459dbc56ab34279c1b3c93f54d3c57352 Merge pull request #942 from nader-ziada/kcp-upgrade-test
dad101d8a0b1aeb0dbe45f5c452239971c0cad35 add title icons to pr template
ec1693d405d13a13c13a8d4ecc08169c3e89c927 increase wait time for machine upgrade used by the kcp upgrade e2e test
677a920bbb3af72357b52e2dcb21074df48475ae move test template patches to common directory
4b9b1110f3305daf28f8164d20e25563bbd8f268 Use a different kind cluster name for e2e
3138254c984cfd63706cff1ff4e69fa932c7b121 Merge pull request #934 from varunpurohit76/#562
d3a24a951c1224b5c630d0dbaf7b247308867fcc Merge pull request #879 from alexeldeib/ace/creds
0b611b649581dad9ca2a97b12783708c6eeba01f events for azurecluster_controller
10dfcd63fce6627bbb2cb36277939d95718a1180 :gem: remove unneccessary function
dae11e84e07c3e9d3c87f2b1c05f069b2755b4c2 :gem: adjust failure cases
4ef369626d21c997c9f6d0d661f2a1c5aad51899 :gem: simplify credential instantiation
cba51f21d701a4c783ccde2368728a3b99ea8dff Merge pull request #930 from alexeldeib/ace/imageDocs
33f1b6bbd4ce90aada6757c464795b27bb42afd8 fix: don't allow multiple images on update
2ee219c2474f69b8c6a4dcb6f06d20364485f999 :book: fix custom image docs
7240721cb206a7e0eec43cb7fd2a0ccc5491531f Merge pull request #928 from nader-ziada/imageplan
5c680a6c2dd4cc0316658b492770890e77eef136 add thirdparty flag to marketplace image
fe6ada8605345f669d729fffe0733e6bb1490e3d Merge pull request #906 from cpanato/GH-836
d6b9dec21b10457ee2f284e04abdf202d18cc374 Merge pull request #924 from cpanato/fix-links
f09265dceb8a09d0432bea4d56ddc53c663d41eb book: fix template examples link
69ebb3fca3fb382ccd44050c2bfa02b6e541493f Merge pull request #926 from cpanato/GH-920
7f69008235fe5938a95eedafebb5121fcfc00805 AzureManagedControlPlane: validate version in azure manager controlplance
68ae979fb15e0ed5d826a9646f7b25fd4595a1fc cert-manager: update cert-manager to 0.16.1 to follow CAPI
bdecbfe44821bf126bb4f94986cbe92619c26116 Merge pull request #923 from CecileRobertMichon/tilt-crds
a2bdbef2e4ef5d9dd49344bc3c9ca8aa391161c6 :wrench: Use k8s_resource to move CRDs out of uncategorized in Tilt
8e6cf27fc4bea69ac2abea85af475842e4d2e431 Merge pull request #922 from CecileRobertMichon/conformance-crs
85c984e1ae457087f65d97aa89d60f941508d175 :green_heart: Enable ClusterResourceSet on conformance job
ef306a47db45134ebd427c19827eacfdd8937a28 Merge pull request #919 from CecileRobertMichon/release-doc-fixes
e79a2741a8af5c0139eda405709c8aa17fd173fd :book: Update release documentation
056c641ec8454e31b3a4776becea76a985d741d5 Merge pull request #918 from nader-ziada/capi039
95a1657cc3f2ee596d7ccd41488782694eea30d9 Merge pull request #896 from CecileRobertMichon/ensure-tags
6d18ed80bacf99a738d1b782431b56f06394c65d bump capi to v0.3.9
227bbdec3a6a691a90fa82624b42d200aaa627a7 Merge pull request #914 from Evalle/ISSUE-908
e8da002290950201c09eee45b5e48eb417c471db Merge pull request #917 from CecileRobertMichon/mhc-space
2de9262e00712fee6299c836dfd434c868cfdf51 :seedling: remove extra spaces in MHC prow cluster template
6eb879fd81a5168efa82fb281f6d51abce2828fb :gem: Update tags at scope instead of updating VMs
3c0b4df0fef849a8607bf6decf3e4c5eadf2376f Merge pull request #901 from CecileRobertMichon/boot-diagnostics
3386cdd997fa32f3d9a394e5f0b1f91ee2276aca Merge pull request #913 from cpanato/leader-election-namespace
7d1b0dbb45848031e48b4c859f01fdc45456817e Merge pull request #912 from cpanato/deps
08f13e1c1f7c06c0e382479a4e89df82e40dbe60 Merge pull request #911 from cpanato/bump-golang-13
b6831cdf4b3a77a585df190795137a736b97349d Merge pull request #910 from CecileRobertMichon/default-ssh
995da71c822c201cfa72cf99ae1b96652544e352 Change AzureManagedCluster LoadBalancerSKU values to Uppercase
460b8bd0daaa90849410dcf6b084b4fa621d80f4 manager: add option to configure the leader election namespace
b60e7cd152bdf735c0e6219e91e0b59c5e3c2d50 dependencies: update several dependencies
2a6c0cfece5f675ed2ce1ef5770d8fa81f6eea36 golang: bump go version to 1.13.15
a86fec3a9f9513c7c413986d98e852407a120b88 Merge pull request #904 from cpanato/GH-886
70304536e5690edd491a928de2b9c31cecabf222 :seedling: Make AZURE_SSH_PUBLIC_KEY_B64 optional in example templates
78d319ededce4ff2d17c3a7e28afd24fb3bf67b8 Merge pull request #907 from cpanato/GH-903
c49aa73a2d967797856bae09993a47d5a03647c1 Merge pull request #905 from cpanato/GH-868
19e80de4a7e92082ca0c5eb672e486801da23766 update AZURE_SSH_PUBLIC_KEY variable to be AZURE_SSH_PUBLIC_KEY_B64
07b7495d42c4f0479d8bdd1a479c2848005f5d88 Add metadata.yaml for defining contracts
0ccb197364a5ed8623cdf500ebedbc9099609d19 :sparkles: Enable VM boot diagnostics
9476396471ddb11f892c35e371a9ee4b7cb98001 azuremachine: deprecate Location - to be removed in v1alpha4
b4704084c698b3fd81a68473300fa7e3f71e9049 Merge pull request #869 from CecileRobertMichon/refactor-vmss
07e2ccae1dc0c992d6455606e053e102ed28a6ba Merge pull request #764 from mboersma/accelerated-networking-e2e-spec
3ad5e9e00240d05aef83a293283849064f7dcf94 :gem: Refactor scale sets service spec
100a9e5ccdeb3b33fb92cc6b51b473a13a4631c0 💚 add test to validate accelerated networking for VMs
cb9b07faedd74b146bcf67f0a8e76dfa1752dba9 Merge pull request #890 from CecileRobertMichon/roadmap
77b1656fdf9c10225b348acbaa2e47a71d5c586f Merge pull request #888 from mboersma/restore-elb-connect-test
be6da12152233f75d1c85d248b0703d34348e43f Merge pull request #899 from mboersma/e2e-zones-to-seprate-file
5a9cf7ba56c6bbecf03af52c330a2bc8a8cdcf87 Merge pull request #900 from mboersma/quieter-e2e-tests
f8844c6a2fcddd809d252d286183ba18d3d67e60 🌱 move e2e failure domains spec to its own file
14af81a53d8735c314b4ab84788a046e3d4a8abd Revert "skip LB direct connect test temporarily"
3e1f071aae7f81d6b4c8638414679821f7ff1659 🌱 [e2e] silence output from curl commands
47d19896ac4f0b9c618eb17fcf6616a26aad01e9 Merge pull request #893 from CecileRobertMichon/fix-nic
b185781e9547bd6c9ba3b0a87ecf13d23ca6b637 :bug: don't return nil in for loops
b2514b11a1114f4b7b8662cc93f2ee1faafd15c1 :bug: don't update network interface if it already exists
6f0baa64a9533f3ed7cb8b487c934c92d6cced38 Merge pull request #891 from awesomenix/terminatenotify
49a2804b8a8b5f12b0df7ce4ff99fec0f9fcd1c9 Add support for TerminateNotificationTimeout in machinepools
ad84605ead343db3d6ebe2a24bdb3ccfcb8d0be7 :book: Create roadmap document
92164bbf8c1ae7073c7d3f63ade6cb9c9335f971 Merge pull request #858 from CecileRobertMichon/netlify-book
d1d309038c1d03bdb97f722093daf3139830aa8e Merge pull request #884 from cpanato/GH-765
4958b9a02b2bed682d76d519cf3cccb7ce433b16 Merge pull request #880 from alexeldeib/ace/cover
ec590aaffe680402738f89690e3f9188e1d7d72b :book: Add Netlify book
6fb7fc1a441f8953a9b31d9f44961a591d322f63 Merge pull request #851 from gab-satchi/820-az-e2e
d78efa460aa1750472e00e95737b8e61bc9e476a Asserts control planes are spread across zones when possible - Checks FailureDomains against expected set of Availability Zones
67b7e6f1b13c1b50da44797d31de169f5a4f0a7b Merge pull request #889 from CecileRobertMichon/tilt-env
d8f9349217ab0b41f0029d0b917b4d179c0bfba2 Remove AZURE_ENVIRONMENT from required tilt vars
05c6c9afd383a9c0fb6367ab52593d8575986bd3 cloud/vm/vmss: validate if vCPUs and Memory matched the minimum required
bf691a6555ee568b6a39d29daf64f02d05df5154 :gem: add coverage
1109ed7d01d1a3d0dcbb700c2418798e749170d0 Merge pull request #866 from nader-ziada/capi-tests-2
f65c209f583affee815852925eed7ad0442e6afd Merge pull request #887 from mboersma/bump-k8s-in-e2e
6c1e1f46d7e808aa2df749420dc23b426a46768a update Kubernetes versions in e2e test and docs
afed79ecd97bd2c7f4beb4c30b0be1cf6c1951c5 Merge pull request #885 from mboersma/skip-lb-direct-connect
eb860aefaeba3431f1c00f7586a88179193d50aa Merge pull request #883 from cpanato/add-coverage-script
3687d743efc7220d4a15f5e308d1c1103536e809 skip LB direct connect test temporarily
01aa442dd6eab4338e646153249043fbd25dcb75 Merge pull request #860 from mboersma/fix-e2e-adaptors
f96be68f3da8a2eae93f4a15cdc6aab81bc7ac3f scripts: add script to run the test coverage
075631160f58ccc26b6ea657ebe5cd05b2de70af Merge pull request #881 from alexeldeib/ace/owners
59a5442bee363e873531d287dcb488e3760ccdd2 Merge pull request #882 from nader-ziada/conditions-conflict
48b6d578b001f8b8afc02713fe5d054089783c46 add kcp upgrade, mhc remediations and resource set spec to capi e2e
ed614562a366f4ed3234cfd5466f43f71a3ac818 Add Ready condition to list of owned conditions
dd3778d42289164550a10c0d0fab854feff20c3c Merge pull request #870 from alexeldeib/ace/slow
c6530dd894a0c0e496aff5b53b0925186a015d65 :bug: fix incorrect owner references on azure json
c4b52027ebd9d4a963e015e50105c105c16c1320 :bug: fix requeue, labels in azure json reconciler
9ab1faab9b04e7a3d8bc3772ad6b085226da0e6a Merge pull request #876 from nader-ziada/machine-json
4ad7b2ddf79d5d3a083ff612e31907685ca0f4be Merge pull request #862 from jroden/amcp-webhooks
d2a26ac51e768fdaa26a07f9f686ce328ab40409 Merge pull request #875 from CecileRobertMichon/office-hours-time
5098a460e1213efedac44f2a1fff01e227724478 Allow the json secret to be created for controlplane machine
fb6bd1b92cb6e5bfc3fccf0f8b506de42a7e100b Update office hours time in README
709c6ea64a44d3cadfdac97b79b019f0cfe9e096 Merge pull request #867 from nader-ziada/doc-release
f0774380c94c61e8ac76eead6af47e0ca38d3cfb Merge pull request #854 from jsturtevant/k8s-devs
3f5387a273eb3595af774c124365c272179928b2 Merge pull request #872 from devigned/fix-ci-e2e
a22d46f267958415a82fdc1d74ba256de9cb4814 update release process docs to match current steps
c8cbe86825782e9e87347381a09ec99fb8eaecf8 chore: make LOCAL_ONLY default and remove REGISTRY override
06f066bc2ad82271ed8757648fb9d79b6856b1f4 Merge pull request #873 from CecileRobertMichon/exp-typo
f18db767000e1b3144a6f803a3149ffd41dea54b :seedling: fix typo in e2e config resource set exp variable
9241b7edd4f150554d109200b89046c821037ec4 Merge pull request #708 from cpanato/add-bastion-service
99f90b1a6392d4e3a671498d47a4295aaf298f25 cloud/services: add bastion host service
bed65b6441f9c739c50670641546a4976061ec18 azureManagedControlPlane webhooks
330d68c973e11ff224d98a740e818581f74ff712 💚 add debug output for e2e service and job failures
8b2866123ccce2d63c0df52c8507d0e2996857e9 Merge pull request #852 from devigned/fix-ci-e2e
250b07fa4dbfd80ddfad8917a11f4d8f6f9b2db9 fix: ci-e2e pivot cluster scenario
96eadddf9d6af490855f42633f0d5ba95c1bc5e9 Merge pull request #849 from jroden/#584
052a5fd3debe0e556d8eb7132ea4e2730a40652c Merge pull request #863 from cpanato/reconcileTimeout
476d9d9628223962d6953b5c308fb20406419d3f manager: set the reconcileTimeout variable when initializing
df22023917a8b856e2960f5f199b9281f96decb4 Merge pull request #848 from CecileRobertMichon/remove-gets
5442e23869219f601dac4bd856104078bc01f72d 🌱 Remove extra GET API calls for resource IDs
6dee98a941778ac36361f1ae37982693e83f3efe Merge pull request #843 from devigned/fix-unpause
f8ca63979c28b5bc4d2d53c7a2cffd4d7edcbda4 dataDisk caching, conversion support
d1287776e41f591937047f86dbda829164627c1d Merge pull request #850 from Evalle/ISSUE-844-2
a4e0b70faacc213d02843c6aa03402ea936a7ebe Merge pull request #853 from cpanato/update-deps
c28cdfcf368a666d8a2c7a4801b0820ed6f98e52 Merge pull request #809 from devigned/multitenant
ef30b32fbe9363e0d8baf646b0bd1ba527f402be ISSUE-844: Doc: update failure domains doc
1059293d05f0ec9fd171d8ed7c5febd7fb2cc664 Add docs for customizing controll plane components
58033d258e0822d459eec884c90a98bfc34ebacf fix: group, version, kind not being passed into util.ClusterToObjectsMapper for unpause events
5684af2a947837eab501aa8ae0c76e59943a5605 Merge pull request #779 from cpanato/GH-692
0e846b52b95c0f371c1d830da48d54bdabe14ba0 dependencies: update several dependencies
3b2f7fdca03d0e001256357f18b8530578dc3158 Merge pull request #827 from CecileRobertMichon/vm-refactor
d2f4b77e6abd74ef42ad7d89ca8b875901017c9d :gem: Refactor VM service spec
b431f06b549b2ba542c30c6b944bf9e49f5a2297 Merge pull request #830 from CecileRobertMichon/refactor-nsg
c1dccd681ce98def5f30c22cfacaf760406fc63f :gem: Refactor security groups service spec
1958c8a512cc2b848c8dd9ed1bbdf38ea6e89c88 Merge https://github.com/kubernetes-sigs/cluster-api-provider-azure into #584
4b92107fb2cc824fc6ab3e70e65c24c12df20bec Merge pull request #798 from devigned/fix-aks
af4a9582e37b153b8dd2fa004c103c5f6b2841ac Merge pull request #828 from nader-ziada/clustername
f1e81c1ac979ba57c24642ce9fd8430449817e58 fix AzureManagedCluster deployments when the resource group is not present
928f0c492b8dccf78703b343c7bbe543a5861210 Merge pull request #793 from mboersma/custom-image-docs
8b2d4d5d726b5c0817bcc5e044a051e41a41a0a9 Add validation on clustername
03df29cde9414c1234f8b840c9c3661d6cd8ab2f Merge pull request #802 from alexeldeib/ace/cloud
6db35b44f67c1c83b9f12f4de4518ffe548d57c8 Merge pull request #837 from chewong/patch-1
16d9e12fef3723e96aeab015206cb6ba774a2471 Merge pull request #845 from justaugustus/version-markers
2c6ec7d6017ad3e7eac0f94557c7ce7801ac757a 📖 document how to use custom images
5ff5deb74f52915ab7122a51ae48ab0e9539ac44 scripts: Use ci/latest version marker for retrieving cross builds
dcbe30dae4dbe0d73fa816556ec346705300bf6a Merge pull request #841 from ncdc/fix-cluster-paused-map
e732c32e5b9decd1c6a25f7a718b1d18829a346e Merge pull request #839 from devigned/fix-tilt
013374ceeba4892cf2d446456582b5f439cc0334 :sparkles: automatically generate azure.json
b8b88f6d8aa202ef6f2930c5af35b2697c913d6a Merge pull request #838 from alexeldeib/ace/vnetName
cca9e61da48800d369e3be52825b651e5abe6c9c Fix issue with cluster paused map function
0213da1a181e6ad80145553c71d152511f20e44f fix: load k8s substitutions before envsubst
b9eef390f295348dd17d1ac0f96761a02bb9c1c0 :book: fix tiny typo in docs
877654846827524e8000b4a00b436ac32627cb7c Merge pull request #818 from alexeldeib/ace/mc
6958d5af610f275dae1dd4ad914a1c4047b52c1d 🐛  use versioned image for log-dump-daemonset.yaml
47524f27ea9c307dbcf2d7aaac24c4d6dcd73c00 Merge pull request #833 from jackfrancis/kubeadm-config-worker-node
0deb03dc121e5099dd07f302d0961252e1b37870 add first draft of multitenancy proposal
4e3bc9bf3273ba9948257dad6e82a40d8ee316bb fix: use useExperimentalRetryJoin: true for all KubeadmConfigTemplate resources
62f466058de45d9f55a37a7312c4d641aeabf934 Merge pull request #835 from alexeldeib/ace/bugz
36e7e1fb0a768abd57312762807300dc6cd5f9f8 :bug: sku api should use resourceType, not kind
9dec43b034f8f47460f9b835444e65a1af762615 Merge pull request #829 from jsturtevant/fix-tilt-up-on-linux
c367ab8a052f87560ab545a81cfef52f0b2edaa5 Handle large yaml files on linux
bceee96d979fd164662ff6a4dcf10676271555da Merge pull request #823 from Deeps-1989/dedupe-reconciliation-tags
e42e1ac24a9ae91bd841b8884c5cf24c454b10d2 :gem: dedupe reconciliation tags on machine pool
38303cfd9351bc3ccfea9ad28e2a8fcef4355cee :bug: normalize managed machinepool version too
6ad50d0e79546d9f3c5e5d632836412df91a6a9c Merge pull request #811 from CecileRobertMichon/refactor-role-assignments
9f28c6fde68ecf5bdc65f500a3a3bddecec6ea20 :bug: normalize version in managed control plane
5f99b7c24254ff67c0d44304fdd72dfbe9b64afc :gem: refactor role assignment service
92da24fc749203f708f1c1e7546d4ed37dbcbe34 Merge pull request #783 from alexeldeib/ace/cache
a8f1a68e3d2fa5eb6ce08988c5dad16402a745b8 move cache out of scope
8d6aa89d83a55ed81a2350466b8f4e484e692469 :gem: refactor skus client
06649e1090c393e38462c8513b62226c918717cf Merge pull request #801 from cpanato/GH-757-virtual-nets
4b327b221fbce133811a6556173b540595b79e52 Merge pull request #804 from alexeldeib/ace/default
9d9227554c149fa6db3f68bafc6fbccb3b034a7f Merge pull request #799 from cpanato/update-tests
4ff4326be9c75d8d0de804ef1af77d3fb2bd6364 cloud: Refactor Virtual Networks scope to interface
7b418861e609584f3abed6f9397c04994d6e3982 e2e: rename tests to be more clear and set worker nodes
1a5728fb71a7c96fa2a657011b61d71aeb03326b Merge pull request #813 from ncdc/no-gvk
eddf931e60c56a98dd3ee61e4b53ee5bfea4af39 Merge pull request #768 from cpanato/GH-757-subnet
3018ac72ef0b9b801cddf7a8c6a2559c02c60a43 Only look at GroupKind for getOwnerMachinePool
f7cc9dc5e70b8e4d8d4e2081c217f6848db3ac59 Only look at GroupKind for GetOwnerClusterName
5d75506dc2c51866f18177cbe2af40abcf1e599e :gem:  add resource group defaulting
b88f8e8064bfbc9e12fc055e7641b763fdadc02f Merge pull request #721 from cpanato/GH-704
299e266f7ae51cb0d0e58ca4a4db82eccf9bcb52 cloud: Refactor Subnets scope to interface
48d25a3372d2c44f46da32665f88ecae0476418c Merge pull request #800 from mboersma/bump-default-k8s-versions
2dafed276259a68b90c7774bd7a3d00b9283631c Merge pull request #790 from CecileRobertMichon/inbound-nat-rules
6ca13ab87a186683c1f735fad9fea0ccf34ed024 Merge pull request #810 from nader-ziada/parallel
d73c831095460497b9cc11ad3cecff0cc8c42c7c :gem:  Refactor inbound NAT rules service
0416736454ed8b98b40ab57eb0a26ed810e4114d Merge pull request #806 from jsturtevant/fix/unit-tests-parallel
ea25851aa6ddf4ff0ce00cae1ac83e30d6ffddfa enable parallel unit tests
94346409142b9e97ba8066e013cd5d56c4cfbc3f Merge pull request #808 from CecileRobertMichon/envsubst-drone
b44768185345a06c069a38547dec3e09054abb88 :wrench: automatically change from a8m.envsubst to drone/envsubst
896d62e5d4ed643c180776c39761bb1514f7a079 Merge pull request #803 from CecileRobertMichon/fix-default-vars
d9ccde94fd247a701461868c6f6da3381aa2fe72 Use drone/envsubst to be consistent with clusterctl
d87fbb94719706ea1e3122bbde256d2a07479818 Fix parallel and network interfaces tests
5dafe9d4e2b64c85bd6964f7210899ba23e36443 :bug: fix template default variables
09259ca745e874d3f19a41f2a549954688b9cae3 Update Kubernetes versions in e2e test and docs
206e3d865da1a0e74bd418e17ce71f1d7fd4107f Merge pull request #792 from nader-ziada/routetables
c210ee4a904f99230fefa7c8c2d9b99eae58b570 tests/e2e: testing network policies
ea8ae550ac81ff3db5468647b3546a62484ed01f makefile: Add a make target to generate test coverage report
e45efcfa64739c9dce04fc441b4a98c104730d52 Refactor routetable scope to interface
b62341be6d8c3acdf05bc17bee9c271bb79b2843 Merge pull request #777 from alexeldeib/ace/ephemeral
0aa24fa6c70db423444d8b4e643f582aee80d8c3 :sparkles: implement ephemeral os
87f35a2bf537f106c249b57a652c0625c7faaeb3 Merge pull request #796 from CecileRobertMichon/docs-getting-started
1b9d71123c6c6beab4e581e5cb280dfeeae48af0 Merge pull request #795 from sedefsavas/EXP_CLUSTER_RESOURSE_SET
7a27b1a25419b0ff77e64a9dffce359266303608 :book: Documentation updates
a0c59497413579de8d7d794461e01b5b8e73724b Fix for EXP_CLUSTER_RESOURCE_SET typo
6cf2090ab4298b695afdff2330f8c3e651e1a5a4 Merge pull request #789 from nader-ziada/defaults
dadb939702a37a20b30a67c532dbec8f150e0105 add variable defaults to templates
82b903d6eaef7eff13b4c89602f965dc2fa76b0c Merge pull request #787 from devigned/e2e-exp
013ad0cfe7bf64ff8a5d412e279f2ad7521dc785 enable experimental features in e2e testing
81330946a541785e36290044519bc262e5a166ce Merge pull request #754 from CecileRobertMichon/pip-nodes
387db5a07600fdab823a56da465cbaa355deabeb Merge pull request #788 from devigned/capi-upgrade
9b6b28264cec6b266002e668cdcafbf68fb45fa6 :bug: Add secondary network interface for node public IPs
eaaa3127f0b71352e1f74436d1a94af883c5fb38 update to capi dependency to v0.3.7
43cc7fed41a2e2047bef0305fe07dd46dd815f37 Merge pull request #786 from CecileRobertMichon/fix-tilt-defaults
11aa5e5b5963bf14ea539a3b8cf4af2ee80e0a49 :wrench: Fix default tilt variables assignment
cf2473927944a9585de7ae7d80abb2ac3369739b Merge pull request #771 from CecileRobertMichon/refactor-lb
035a32d8e776684a97a9f9e7bdf976e5695a7e42 Merge pull request #784 from cpanato/update-makefile
2ac0cb2b480c58ca2e38a0a5527c145b29c08f8a makefile: remove hack/tool that is not used anymore
a9d8ae581aa938edd47ef3222342c8da448421fb Merge pull request #782 from nader-ziada/exp
94b559befcee76e7b94649a4b9bbc42de0394add Merge pull request #781 from devigned/fix-tilt-az-json
f69c77e56defa20ba3f66f47d9d1aa8397a93d33 rename feature_gate_machine_pool to exp_machine_pool to match capi
371f30b6cf26ac1ce1c3e60e38883a13a11f08a1 :bug: add azure_json_b64 content to flavors
c50f2cdd1d65e2515d285b45082c13c209a46fff Merge pull request #770 from CecileRobertMichon/owners
88d2cedf4887addae320f86ee917be77fc2c6c76 :gem: refactor load balancer scope to interface
3a0bf3ca9ede4850b78753745fa45693620ad77a Merge pull request #774 from mboersma/vendor-capi-0.3.7-rc1
02d21b3a3c607f23847103e13ac39579de00b856 Merge pull request #750 from CecileRobertMichon/cluster-scope
004e869043e70878ede1d378d3a2374a5b5b63ca update cluster api version to v0.3.7-rc.1
bc334bee2919a4ec113dd6d20203b0e85307c470 Merge pull request #740 from mboersma/e2e-lb-svc-spec
0bae181000b769c61344125d11f86b97334397ba 💚 add e2e spec for workload service and LBs
4059470a77fd4292fcb8cfb3bcc63ca03e9b8acd Merge pull request #766 from cpanato/GH-757-groups
b0e2d89ea5e941c114713fca837520e64266676b :gem: Embed ClusterScope in MachineScope to remove the need for duplicate Cluster Getters
23e3998f60f1af7d656e99c4c1c2dcbc27fcd43e Merge pull request #769 from mboersma/tix-fypo
e20d9d8f8d289c6b3ae27988c8a9126b31944844 :seedling: Promote devigned and nader-ziada to maintainers, add cpanato as reviewer
c20469d21ff55938b7216f3a52467608f6e0bcd3 cloud: Refactor Groups scope to interface
6f098c902c601e3ca3a4ebc18d1addf1fed95ab2 Merge pull request #751 from cpanato/add-scoped-log
9b05c6b12bdb4a9ea8bfb17573a9de7eba386eb0 Fix typo in e2e test case spec
27d9fb6ebdc5d2876b5fe6545eb927aaf32f297c cloud/services: add scoped log to delete function
75071549a5196436b57c680bdfc987a1909554d1 Merge pull request #758 from jroden/#737
7cafe962c04adb390fedb3687674f9a18098eb4c :sparkles: AzureMachine should publish reconcile events to CR
b4faf16b50329b708ad5b879b630ffc08727f276 Merge pull request #763 from nader-ziada/capi-0.3.7-rc
6908f7cf4c95807da8a7c714944d433ab367e1c1 Merge pull request #762 from CecileRobertMichon/fix-json
df2e7d3213e8842fff9d0e929de14d8b17c50fa3 Merge pull request #760 from nader-ziada/lb-subnetcidr
dbe493e8f250aa0c90241d695945faac9eb88fd7 :bug: use AZURE_VNET_NAME as vnetName in azure.json
e893e2792de8059ad2ae9cae8760042ba0e1132b update cluster api version to v0.3.7-rc.0
9bf0121e2977509835139a8b6642ca4dda1caf85 Merge pull request #759 from cpanato/GH-757
254f75c660609d09d37411e1e8d82d603239da75 Add unit tests for internallb subnet addressing fix
e45d6c558a0fca5e4c840c779989fcfaa7e5cdd4 Merge pull request #724 from dklyle/fix-internallb-ip
7741cd61bde284a7b7b2f58264361abbfa24de4e Merge pull request #661 from CecileRobertMichon/etcd-disk
e06c352bdce89d3c7ceeb3723e4b4c27bc7e2d0a cloud: Refactor Disks scope to interface
ccfe354acc9c4e13f3079583603e6ec814a27726 Merge pull request #756 from CecileRobertMichon/delete-os-disk
0a13b3104008bda9612f144b1f7c8d13f295259f :bug: Delete OS disk when failed VM gets deleted
033e7f967d632ad5abe244534f0b2e6c76b5fec5 Merge pull request #753 from chewong/azure-json-b64
754912d42226a996f4fa286c89ba882a9081a556 🔧 combine AZURE_STANDARD_JSON_B64 and AZURE_VMSS_JSON_B64 into AZURE_JSON_B64
e73f75c05457873d1fd09cd226d930cb10f3ec30 Merge pull request #752 from cpanato/update-deps
01ced91b4182f5a12999460d6ec5ed694a36d049 :sparkles: Move etcd data dir to a data disk
48f91ea17e4aa85c30724e800a9976a9a2ecb2b1 Merge pull request #714 from nader-ziada/conditions
8ebb54e275186eb07b4ba0bfc1e1b2384311e35e Merge pull request #747 from cpanato/followup
3735a0e69eb455896484c5c26737cc4f792d47fa update compute library to use 2020-06-01
c9e2a7fe7fe7c3488ca82de5091d8c4954129192 dependencies: update some dependencies
a585f0a52a9ce8c6413b9feb993af4609a2c3109 #584 osDisk caching + webhooks
b5cdc594492295a91c9daf57bf000a977ff760ee cloud/publicips: add logger scope in public ip service
d42e44640b186de75e31e4a4e04461863a32fadf Merge pull request #746 from chewong/remove-env-var
d18ae621339235ef623398b0cb749c03bd50ac39 🔧 eliminate plain text creds from additional template files & fix e2e regression
da0a5cd48b4be8f6626badea911252fc76910689 Merge pull request #742 from CecileRobertMichon/refactor-nic-scope
13dc8099fa77c59442d682be86bee0552f488bf9 Increase timeout in azuremachine controller test
edee30d4910c85c41f200f860b0a5a059345bed2 :gem: Refactor network interfaces scope to interface
464e94377fdc0478cca4851bdcb5d5d192085fa8 Merge pull request #748 from cpanato/update-cluster-api-beta
ae25234e6d128c38de5252bdc51500f61aa4ff95 cluster-api: update cluster-api dependencie to use v0.3.7-beta.0
9e4ee99dfd231633fbae90d60d36c8930aac17d0 Merge pull request #739 from cpanato/GH-725
75ccd668655bdff15480fa0cc715a3d14a00791e services: logging with scope logger to provide better context
0f4f5a2a19b7ff6f69904cc1e5e2ca86e3136786 Merge pull request #745 from alexeldeib/ace/v
435f4fa2d77bd50f7c6ee5a7d7c5e222f11d0d11 Merge pull request #653 from alexeldeib/ace/docs
1faff4b0424e6b32fcd2312a3e162b4220d93ab5 Merge pull request #738 from cpanato/GH-720
b3ebfa5de4c709c9b7ddb51212c3b9b83218f182 :bug: fix serverside validation for version in managed cluster
1443cdeaf5ccbf71ee9aafccdcd9392fe80ff1af Merge pull request #744 from CecileRobertMichon/remove-master
3b7be045ea46b3a5f40035e460ebbde2cde21463 :seedling: remove incorrect reference to master in managed machinepool types
7958ebc7f818f373087fbac3b334c877cfcbc6b2 :hammer_and_pick: eliminate plain text credentials
446585ba0fa5cdef27c98a4d7743df9d2017c922 tests: add missing mockCtrl.Finish()
51c55dd5753460404e0da5f4c46549dabbd664e7 Merge pull request #729 from rsmitty/master
41f7dbcf05d22abd1226b0c49a1d875e98e4547c Merge pull request #743 from CecileRobertMichon/capi-owners
f9a6515ac55766f862124f27b2804abfaaaad121 Merge pull request #741 from CecileRobertMichon/use-clustername
060b330ce7e8e6be1dc0bcfd4acb969bd2223ec0 :seedling: Update cluster-api OWNERS to match CAPI repo
c7766d10d4fe2338c4d17f5cc0005de376b132a6 Apply suggestions from code review
611488581c6d45aa9de2c61471c3caa02540b2fc :bug: respect ingressRules specified in security group spec
e84fee9e25554209ae0c84be9e4d3ce74afe69a7 :gem: Remove use of deprecated cluster scope Name() in favor of ClusterName()
20dda3357e3a4778d4f344f8897aac4cca0147c8 initial support for conditions for azurecluster and azuremachine
5fb8ce3598a6f9f0514b2418d7f1922252da4537 Merge pull request #716 from CecileRobertMichon/public-ips-scope
ade4bbf0acd187361bb789fefb16f34471892403 Merge pull request #732 from devigned/fix-subnet-reconcile
f753c3dbc7d4790354472e1f5a536f29eb63d9a7 :bug: fix AzureCluster reconcile loop cycle
a89eb3c71fa688b7b61dd78172dde8e90d59872e 💎 Refactor public IP service to get Spec from scope
ac7fd15bff558ca29ade41f2ce7249e41d836344 :wrench: Update mockgen to 8a3d595
5657bc71ae24e9ab284c607ae347db9b0f01c5a4 Merge pull request #736 from CecileRobertMichon/hack-tools-versions
d29f52ce8ae5d55fad564ef24a877e36959fecc3 :wrench: install hack/tools when version has changed
83876563cc044fb00dda224b0f5fd1df8973ddd9 Merge pull request #735 from CecileRobertMichon/remove-sg
4c759d96e7442ef16d0e462b45c0da8891904b7a :warning: Remove SecurityGroups from AzureCluster Status
4833e5043cfb0d93fac5dcacde6a5584df5e13ef Merge pull request #559 from JoelSpeed/spot-support
6a24966043abf86f4607a8c1f8e6e35389c3fd6a Merge pull request #734 from devigned/foo
03a76e30059c9d467ee470600d3471f8bf6ba4fa :bug: fix conversion-gen not using --output-base dir
59c726efc69189d7048f5f31899cde25d70bc515 Merge pull request #727 from nprokopic/azuremachinepool-subnet-fix
2e1b96ee26541380a397ebef3b11ec5050948e9c Merge pull request #733 from vinu2003/replace-deprecated-newclientfunc
6be0b72740c8e40efc809e64727c141a1735ec85 bug: replaced deprecated NewFakeClient with NewFakeClientWithScheme in go test filesO
04b9e8210b088eba82afc8d4967c3604e1fcc10b Merge pull request #730 from devigned/mp-delete
1f1b0447c467a842b2880b15d4e3eb65e013c4f2 Merge pull request #728 from nader-ziada/capi-0.3.7-alpha0
a4f91e825588eff8a05df53643e5a678bb1728df :bug: Add resource group to the spec of the delete request
c9366d360fabc9b08efab15ac6f93a04eec0caec bump cluster api version to 0.3.7-alpha.0 to enable development
9e423ff201cd1ee9008e307e1ef1b845476625a1 Switch maxPrice to a number
1040ee8f83ea9bc7de7bb47a9c52651fe38abe00 Add SpotVM doc
6046974cc4167050e8a28d83ba6af899bd96c400 Test SpotVMOptions propagated to Azure instance creation
316f57e05f4a4524d00f69f8484e7d881af4defe Use SpotVMOptions when creating instances
ddfb1ab7cd65f91bb52d0b502cb4d261088101a4 Add API Fields for SpotVMOptions
04836dbf9377731539c697b4a10311e39fc83690 Merge pull request #640 from jsturtevant/cluster-creation-debugging-notes
b45f6cf73975ad7fca932df1789667129257adcc Use node subnet for VMSS
3ea4eb4406a0db0cf588f005cdb591a7fbc70a5d Add notes on debugging cluster creation
b006a055d13ce793a98e0d59d96ffd156374c6b8 fix internallb subnet addressing
c5befecdf1714cf3fc69c2cdeb0f8105c53bb07f Merge pull request #701 from CecileRobertMichon/capi-e2e-2
37af4d734df6aaf103cbe3c5406020893dd9aacc Merge pull request #722 from CecileRobertMichon/add-tilt-key
bc614598dcd4c35b06e2862715f7523661ec0139 :wrench: Add AZURE_ENVIRONMENT to required Tilt keys
adf6c09a8fd2e022f16921b67cfe769ea6895f19 Merge pull request #719 from jsturtevant/fix/route-table-reconciliation
fdf7229d974466d7c30eeb381626ab06d67c17f6 Use ginkgo to run E2E tests
d3d545c3467a63d0c314f1eb7d016a8ecc6e2653 fix: Use the prow template with tags for E2E tests
fa3a2814391c6f4850dc3f648c279eb2989bf81b 💚 Run more CAPI E2E specs in E2E
f9da6a5e82da5ccd7c692f47704015be27f7ba6e Merge pull request #649 from nader-ziada/gov
e4f3ad94ce351c958455896b145c6ff6c016e873 Merge pull request #686 from alexeldeib/ace/mcDocs
b294059ec2d872e58d0b8f65ec7a292f5c4913af fix comment
6f3c1d62df52c8626e7a10cce823d8a792f9cfce Merge pull request #691 from devigned/paused
f7f6dfe3c6ce8b5f25296eb1be0d7eee386dcc20 feat: support cluster.x-k8s.io/paused annotation
d940ce34cf2f41004d057fc3c8cb57f6737731a1 handle route table creation
6435e5b06008a39a0c7373c7f0b3b613a796d333 support for using other Azure clouds than default
790ec1caa9fc79942655c6621505796f1094d137 Merge pull request #713 from CecileRobertMichon/reconcile-delete
304e47dc345bd1fa87b3ca16e37cb73b4aca1adc :gem: refactor most services into Reconcile/Delete pattern
e843409f896981185ca31d6b4a4c939f27d975de Merge pull request #709 from cpanato/add-tests-agentpools
c6d1e07522b37c8b3cfaba4b9cf9e374707807a5 Merge pull request #710 from cpanato/update-deps
a8da4fcf73593324542e6db738639fc8a2dde6f6 Merge pull request #711 from cpanato/update-makefile
2d8d52a52c96e67bcd37cb1e8060ffc0b5a31c18 services/agentpools: add unit tests
94bd73ec86d96bc3112bed3259a49357463723d2 deps: update several deps
020e516e036d58ae5637f5a0de9d8031b014f129 makefile: update makefile verify-modules
bc04ec77632c685e777428e26d03fc9fa9a2163d services/availabilityzones: add test to check the spec
e490b54fa88ff0d4861f183f6fd913d873685366 Merge pull request #707 from CecileRobertMichon/fix-contributing
15e928d78439aea2e1fb6138504e473736b59f1e :book: small fix in CONTRIBUTING.md formatting
aa979f27a021e4d87e2bf2926344833042f400c3 Merge pull request #698 from CecileRobertMichon/e2e-log-dump
edb9142488209920cac7bb4b2fc9c06ecd27598d Merge pull request #689 from jroden/master
f1d4282d6255865c878ca4eecf28af2993a4869f Change all example k8s versions and defaults to 1.18.3
40acdc30e3d2bc8c81f73a650b9f418758e0ffd9 :bug: Validate managedcluster provisioningStatus before updating
a7b849ce0b32b68312a025958f34e4484a8d94cb Merge pull request #695 from CecileRobertMichon/vmss-vmtype
6c11ec8f0e0030819adfd8ebf669aa72cefe9024 Merge pull request #697 from CecileRobertMichon/reviewers-update
942691fa3c7ebf9e9f69214ca3169a929e755ca4 Remove serbrech from reviewers and add alexeldeib
5e1b7bc02bf51ca024fdec9ca344427e3d9c8bba Merge pull request #690 from devigned/context
9765463ab28091dfcb2fe84c99179516e93403c4 feat: bound all reconcile loops and network comms with context
ead5f99f306576a2b8fb659e8c5d584b4cc24373 :bug: Use vmType "vmss" in every template to allow mixed mode
225dcc8237e8e43e3d57ad08d78b9fa400ee3b3f Merge pull request #694 from vincepri/rm-reviewer
f494bdc35d80419a2e48f1b26becc859ea4d86c2 Merge pull request #685 from CecileRobertMichon/reconcile-vmss-preserve-rules
d0e5793f6c561555873709f294a5801b312f1596 Remove vincepri from reviewers group
e185705fc28e489c3841524901d435dc7f2c7f10 :bug: Do not update VMSS network profile if scale set already exists
0d346736bfe8f612444ef06ccc72fbe44f40ffe2 :book: document managed cluster
1cff4e64fe213bcdc1bbf7bceb9da85eebb85123 :bug: remove load balancer sku, fix version prefixing
72afeba886476049dace3e9bb39e66703a1e26aa Merge pull request #688 from CecileRobertMichon/cleanup
5563ae10c14a971647e48b8d8f3a816f73e3ad36 Merge pull request #693 from CecileRobertMichon/pr-template
acf63a926ddc6ff40b6bbc58535cd95c834e9293 :book: improve CONTRIBUTING.md PR process
4f2a7601268df1ba1453e300751771b15c69fc3e Update PR template to assist reviewers
1274b053827d26dfa5ef4fe36a4a8fc4de26f8bf Merge pull request #687 from chewong/fix-log-dump-bug
649a5c6dd4367699e5c0fe76ad3adbb750dee1be 🐛 do not use 'source' to call log dump script & fix 1.17 test failure
bdc13ed25f62c06f7f58c8a8e7b89a0ee7373424 :seedling: remove extra image validation in the Azure Machine controller
85ad9d4d53c8a9448984efe23e72f59f249abf84 Merge pull request #684 from devigned/vnet-cluster-rg
88b64a1c777df08731163704d7783105d4ea3699 fix: vnet resource group to be AZURE_RESOURCE_GROUP
7bb617016f359b3eb2c0176c6ab630306b2364a3 Merge pull request #683 from chewong/machine-pool-azure-json
3944724c735293a6da5db1f52cf582c95d5bfad3 Merge pull request #674 from CecileRobertMichon/provider-slb
fd8ead66d6e6d3bbff4a5a613abf6605635ebaeb Merge pull request #681 from devigned/added-flavor
c5299b4e742908eeee934052eb8e262dc89dfcd4 🐛 s/vm/vmss for MachinePool's azure.json
c99a8bc9bb061e69dab9f5b40c67b031fc2457bb feat: tilt flavors with b64 secrets and default pub key
ff37e097b6cdad039e1df89d8887eb67436e8b32 Merge pull request #680 from CecileRobertMichon/vmtype-vmss
f085b86626793adde3657c8136034c4e5154fa58 :bug: MachinePool template must have cloud provider vmType vmss in control plane azure.json
b426c8f8ba038b494ccbc960ac12ed650b2a0ed2 Merge pull request #673 from jroden/master
6be4c90817366a6348fd0ebef2cec3e3fbc0214f Merge pull request #670 from chewong/ci-dump-logs
bb2e24bcac540b9a5e59c04a6cd25b1df38106e8 Use DaemonSet as a proxy to collect logs from CI
6e3a83d9f2ab341ad4dc0565a0d151e68e5199da ✨ Spin flavor clusters as tilt resources
244677ad628cd15df07ae8ac51f11c99fbb8f3aa :bug: Fix nodes outbound connectivity with SLB
5adbc2d5e066d5a82bff3dfd69c4676f12d2f3a3 Merge pull request #659 from chewong/machine-pool-e2e
7f7c1b562c55e53591fbff25037bb6b7b40bde14 🏃 support MachinePool clusters in ci-entrypoint.sh
243218065bc9fb601b1da6208a355ea8b62268fe feat: create debugging script
9fc12dcddbf48d5a9c6749bf6e7f31b13ae56c50 Merge pull request #658 from srm09/feature/add-validation-for-osdisk-spec
45f49d9f2ecdef82f2cc79cbc722e414d12b79d8 Merge pull request #666 from CecileRobertMichon/slb-vmss
1cd7bdd73d2a3d833e857e9b04cd419f98c743e5 :runner: Add cluster-name to kubeadm controllerManager args
4a0b011a5c2ac8e0b106f4863850761f805a5916 Adds validation for OS Disk spec
5a7bedf05cb574a7825608561192d35b535abb9c Merge pull request #665 from CecileRobertMichon/user-agent
6d7fe655ddecba2497cab1abbe3b1d3a772571cd ✨Add version to user-agent for Azure API calls
ad847ce89fd7452b80ba66f1c7bc8c376a4620b2 Merge pull request #643 from CecileRobertMichon/move-network-defaults-to-webhook
82ed0727734d5d0d44a8080ae1e3ca88f7dd65d3 Merge pull request #645 from mboersma/enable-accelerated-networking
ad2579d97c6af7b65aa251e8dfb375d8206b8d36 Merge pull request #639 from srm09/feature/add-version-info-to-starting-log
ffad0adaf9085c504cb08b8369afb2210abb1a74 ✨ support accelerated networking
87de68f2cf49eda58177ef89e05df748335d50d7 🐛 Move subnets and vnet defaulting to AzureCluster mutating webhook
23ef7e54814e36680d36f5c649b9ff47dec5859c fix typos in subnets unit tests
f6de74114149e0bbb809f8737af0acda3284559a Enforce unique subnet names
e80d4802838ed59c9100fa102e3433915834771c :bug: Fix mutating webhooks patch
c0d09b2beae22774c418a357d5ce2e1cb12e84d0 Merge pull request #655 from alexander-demichev/providerID
e90c6504387dbe653585e47e4f35af3e923bf3c1 Adds version info to manager startup logs
f2f5c9b95870d3dff45dcedc1382e1491d4c6968 Merge pull request #638 from chewong/clusterctl-test-framework
d4ba8743322f8ec6c4699da0dbcf604f1243cc36 Merge pull request #650 from mboersma/delete-the-deleted
b34932607c76848a8710cc62b1d7e476e352b74e Address PR comments
9e3562d6c6c5dea9471f6cb2523765a38aef3224 Make machine providerID consistent with node
214c0d7b10ec09df9b638a63b4b4472c203a396d 🐛 Check all chained errors for 404
28ede51fdaf6a95e878d6dff244660893232d7b4 Delete test/e2e and rename test/e2eclusterctl package to test/e2e
4f666e4af22e5cc465d91739f025e5a30c564e52 ✨ switch to clusterctl-based e2e framework
09459f72be89d1da91f1a065255fa1fa81f6284d Merge pull request #642 from jsturtevant/fix-template-namespaces
735f16abf2a2ed0915c33c92007b2ffcddd3b9d0 Merge pull request #647 from mboersma/python-doc-update
32143ef9bce121d753df5904a829150e0540c6ac 📖 clarify that either python 2.7 or 3.x is ok
86766a9f651bfda752decded44e16afc5f067810 Merge pull request #636 from chewong/patch-azure-file
bba95ac11805b479eb7de8f7ae5405182e2b0ad7 Added namespace override to all kustomize files
fac05587942ea4added3927d4e825341c02a4a5d 🐛add ClusterRole and ClusterRoleBinding for Azure File
fc0a458d16bf9c7e377680a59dbd18e6bbf165a5 Merge pull request #634 from chewong/patch-ci-entrypoint
e5e73b539501f058dcd5796d10804d09de16a4a0 🏃 remove unused ci script and rename templates
b6738e612d0fb307faae36f650ff0c3cdd88dac0 Merge pull request #633 from mboersma/link-to-flavors
527a5d8de57edf28cd5f3f2eec51895ab7d6e547 Merge pull request #630 from CecileRobertMichon/move-node-ip-create
6be8d6f4366bc5d9a533b71239e4d65208ff575e 📖 Add front-page link to flavors documentation
5cf2dbdbc5ef9e07147eb6ff998798b92b4224b2 Merge pull request #632 from srm09/patch-1
7efb212f5a17cf08b2d4260819132386749b2a54 Update getting-started.md
8abcd6d8838101a9d6a39487027b51a1f0f95bc9 Refactor: Move node public IP creation/deletion to NIC service
b27fdafb97fc7b40b3c61085bef9ac0540674590 Merge pull request #620 from CecileRobertMichon/api-diff
53b643a4c11f34277f0aa0adbda8b0261b066dab Merge pull request #616 from nader-ziada/user-identity
5be0efc04f0f7b44f8c55329e037d16bbf72c91f add more details in the topics page about Service Principal
e5a8201e433be79fa2493a5b8125ee0faa6efec9 Add support for user-assigned managed identities in AzureMachine
e0fd9dea24bee297d6ff036334843cbca6185239 Merge pull request #617 from chewong/extend-ci-script
2056f2fb2be94fa720617dffe994b3f103ae51bf Merge pull request #628 from mboersma/fix-tiltfile
f981465676db1fcc54f81dcda9e01a92fd298e2c Address PR comment
55c9b435d0e180beb24c6322b956730d80f43e57 🐛 Remove errant space that broke "make tilt-up"
d71f5f097819a43e549def7821556b5ffb5aa62d 🏃 Add ci-apidiff job
55ebfc34f3342567ed2541232cecd36dfde22748 Add azure-related storage classes yaml
e0f3732bbd5b57f16903ea5acc0b0f1fa1e31882 🏃extend ci-conformance.sh testing compatibility
1cf1ec4a1effd9340fe7370ab45b173a4979dc8f Merge pull request #619 from devigned/go-install
4ee9c1129cf743c2727bf3461b305bae2f06efaa Merge pull request #625 from nader-ziada/capi-0.3.6
edaee997aec4390b0dbb62f2c09274007a761199 Merge pull request #626 from CecileRobertMichon/fix-image-validation
b9b11aae33fe293e2b19a7d2f8cc781e1b130547 Update azureimage_validation_test.go
835d14998450b46b383daac848639dc733d3f08c :bug: fix: allow nil image in AzureMachine webhook validation
8875972b3a888b99b0c0695ba9ea6c7128cefeb2 Update CAPI to v0.3.6
db93854615376d44a45a88f6a3e44fd39f754c4d Merge pull request #621 from alexeldeib/ace/hook
6c7c5c69be0a21e1c42944ecdd55d1cd3e0c1600 fix: memory alias within a for loop
7d0982b50fc9d3bc44ac9becd3910af32755bf5d chore: install via ephemeral go module rather than tools module
9faa72dab7fef49b908df7dd746dc6df2b73f543 :bug: fix defaulting/validating webhook tests
e2bd780ed4f7c1045bc26f4752963680242d7ac9 :bug: fix machine webhook encoding consistency
59dc2ea6cb64985527bc199691d6f4d0ee74f9aa :bug: fix e2e with webhook
7cc71a1e4bdd1c1b9fadd64d44376682cc9e91da :bug: fix webhook pluralization
4b049939e18f0ba735735c41ac3fa9f828cd5236 Merge pull request #482 from alexeldeib/ace/caks
8d4a40f6e6c86bba0a50452ee38b71f336a81d63 Merge pull request #610 from CecileRobertMichon/side-effect-none
189c0a0278650128448c8ad041df0345ca437a18 🐛 Report lack of webhook side effects
a2760bed0f09f6a2533338686e718a47d6cec6c5 Merge pull request #592 from spectrocloud/NSGUpdateIssue
2f3e9dd27347650580a57a196d7d3f77be047a31 Merge pull request #604 from weng271190436/weweng/validateClusterVnet
5d80ea5ef593389541d6d47f615896934de3faf8 Skip NSG updates if default rules are present
ad330a200b3dfbc06a02fbcf6fd64cda9106414e Merge pull request #597 from CecileRobertMichon/cleanup-types
752728db490b719f2f935b042dde0defe29c246c validate cluster vnet
e09bf5aa5e42b812e2954ed58a6dda1be1f9f35e :hammer_and_pick: cleanup from review feedback
8fa937a970b1d513bdefd8bccf24ccf22b040736 Merge pull request #595 from CecileRobertMichon/conformance-rm-mac-workaround
451a0ff7d3400ec97e5f8836381925ccce7656d4 ✨ implement controllers
fde4598fa355e12aaa5d2fd1df7418574562b838 ✨ add azure service integrations, scope
3cd7612f2c1855f5ace312cd21141dbd409feac6 Merge pull request #594 from CecileRobertMichon/remove-dead-code-vmextensions
04d10c51ebb74c084b9c6fe1fbaac4fa49eed57e ✨ add CRD, RBAC manifests
96a61a732bcfb3c3d39f9b5ba13f6198cfe4ebec ✨ add Go structs for AKS
4076b14cabde992f9be56bacd8d625a9d73335f0 ✨ introduce AKS feature flag
f38608405daf87134b2c10c53d8fd9a35f601165 ✨ sample templates
1bc3edd7202d503cb2efbfdf812657b66956b19b ⚒️ tooling changes
76ecd0fc93d0c4330af14da035eef065b559df92 Merge pull request #602 from devigned/move-exp-cloud
687f3707e69072bff63251a0936bf94488b7d643 chore: move ./exp/cloud into ./cloud
eae49f45dd60fefcf5d4723eb4d36fe35531e1e3 cleanup: remove unused VM extensions service
3bb748bd86427c30aa4cc49ea19e86539129f22a cleanup: cleanup types.go
43b083f2f7666771bc187191ea152ea4776544ea Merge pull request #599 from CecileRobertMichon/template-ordering
fbdd44e716db09de00a22c9fab58f5b14ceafe36 Update generated templates
038d9931b52074670f11d24c98360edcd9eb2476 Add --reorder none flag to kustomize build commands in gen-flavors.sh
bfe62e1102d6bf6f0948a5cf4382a5c515cce7ad Merge pull request #596 from CecileRobertMichon/delete-decode
4778ca551a5ded2b3da694bcea12b4753e8ee163 Merge pull request #583 from jseely/master
532c62188a1911346840f0fdc85b80bed2516215 Merge pull request #593 from devigned/fix-kind
e29297971b312c3c02a8e946df75b42bcbe80d68 cleanup: delete unused decodeRawExtension code
03d417aaa0d009189dd14fc63e431a814c43d793 Remove conformance script macos workaround
4378504f911bf5418fbad1adc057bac7fc0d5255 fix: with kind 0.8.1 make tilt-up will fail with imagepullbackoff
a287b26136bd7366c90c57f3e20fd2dc8bc018f5 Add SubscriptionID override to AzureCluster to enable deployment into multiple subscriptions
4afe3c2226f885cb1607e7ccf2526bc09b63b816 Merge pull request #572 from richardcase/439_failure_domain
079b32c9057b13ebd450ec3256d6db7694a95d9b docs: added failure domain docs
4c82fa7c0058c52bb01486db6bea80ee236a1324 Merge pull request #591 from devigned/fix-log
fa22af4399d4253fbb709e6a2e74466b5dcf2c35 fix: log for AzureMachinePool specifies name as azureMachine
29127757fa2063b23f4dc6a516739705841a7f17 Merge pull request #590 from jseely/fix-gen-flavors
4d682a1017cd6c849c7e73e7646492d0941c4ed5 Merge pull request #483 from devigned/machinepool
f33e568966d2b31743c7e94bf51b4bb93a1a037f Fix 'gen-flavors.sh' to work on Ubuntu 18.04.2
527e050cc65a680ed5f36b55fe5f8236f8c3bfa3 test: tests for AzureMachinePool
d5e1b5ca11c56b0182144a34a5c2e0b8f5ebdfec feat: add MachinePool support with AzureMachinePool
3eacaf3ba239e9ac77658580432291895036ccff chore: change Tiltfile to follow idioms of CAPI
bb2119a1fbf680e2972d772d19b6042c87f12bbe feat: AzureMachinePool flavor
9e0dae2b7c4045a963fa5aeb86d7d5f5a3a9f6cb docs: AzureMachinePool documenation
fcbf48e9f0608c84698de0e035104d3225d144e1 Merge pull request #587 from cpanato/update-deps
134c9d2eb1a0c9797c2ae812ffb9f3a7d0106c66 Update several dependencies
f1c8eb696028df6a0bd5ee7de8e296713d82fb1b chore: removed debug changes to Makefile
cfc09838ee0ec0cf873d164c898350f61106dd1f feat: add failure domain support
a8dee20eb4c2b3ff3f9d3393cf8a7ba7542ae066 Merge pull request #581 from CecileRobertMichon/kubectl-macos
aea80dc1488b7e20229b6e5fe59fe949d00eb3a5 Merge pull request #577 from CecileRobertMichon/capi-0.3.4
6efc4da78fb697d347e00a465dfe93e24b2ab6c2 Merge pull request #565 from nader-ziada/identity
ac4ee9e10f1a24b0437b2d7dcb0eeddcaf6bd8d3 add support for azure system assigned identities
33d18370d2badbf66ae5dad7cba0d7675cc0e932 Merge pull request #585 from CecileRobertMichon/devigned-reviewers
8949c7f68081b18b69613b43768b0cf7654127b2 Add devigned as reviewer
ac3728ce593cf99f3ddb88e1b4c62a8a1d8830f6 Update CAPI to v0.3.5
3e537ac6fb7c78d59f01e0646f0c8ca73c4528f9 Update controller-tools to v0.2.9
59fda7b1e67ac0b3ea58e2688b2f8d31cbda9190 Add workaround to find kubectl binary on MacOS
7177d6a5101b74c857361bd38331b18b18388b31 Merge pull request #576 from mboersma/getting-started-tweaks
7029569682ef0db2addcb7097b265235ded19e40 Merge pull request #574 from mboersma/dev-docs-tweaks
2f7969e90dce2911d34f516b1f2966c4e93a6011 docs: fix kubectl link in getting started doc
330d65561caf8f80954d8c58b9a219766168a533 Merge pull request #573 from CecileRobertMichon/makefile-fixes
15ef62f38233342a95748e0b3631cfedad9920f4 docs: fix a link and some typos in developer doc
61ccbe8322f39ca8d077c7a7b4985280b2da1167 Merge pull request #571 from CecileRobertMichon/kubectl-path
eedc11b11341504c3b21122339362ff720a2d2dd set nounset and pipefail in kind script
ca5226f0f202afb3d6961783e9bfb1b7881b538f Remove kustomize dependency from create-workload-cluster target
80b693415ed912d9ea7e9391c49200b58f973370 conformance: fix kubectl path
6a820e03f2ca57f54ce3f2845cc5e0a99fb41b87 Merge pull request #568 from weng271190436/weweng/validateSshKey
3f8c2d320dc24c61b7278c07a14695ab5bafb49b Move SSHPublicKey default and validation logic to webhook
5cf486a2a6f6ccb037d78fe0796d916320ccdbc9 Merge pull request #570 from CecileRobertMichon/fix-ci-version
963b0e304c5388f31902b8d27481ebf087b4f35b conformance: fix Kubeadm version when using CI_VERSION and change default to 1 control plane
73133074c9cca15821bc5b36732f0768987bbb71 Merge pull request #569 from CecileRobertMichon/remove-capi-generators
e80b344a8d25d42e10142e730b8bd22fd7c800ea [E2E] Remove capi, cabpk and kcp generators
3db249f2c0fb16e5d1c3ac37850161bf9883306e Merge pull request #555 from CecileRobertMichon/sweep-todos
9734e9ff7e546b16f0a8d961cd13d12a068a5beb :runner: Remove all TODOs in the codebase
994b3804cfd85a0a8dcbf9c8a714aa7af7fc20e9 Merge pull request #567 from alexeldeib/ace/exp
9fb23570d699d2fd5af8ccbe3a9bb320be95f4ec :sparkles: add exp folder to prepare for aks/machinepool
7613ea0385d524ef458101e23586d3d67f919a23 Merge pull request #566 from CecileRobertMichon/reorder-generate
a46cd1a58740c05fd0636afdcc5a6bdb34b46841 Move go generate to the end of the generate make target
259ffb25685d582fb2b40a70947929ab8a78efe4 Merge pull request #560 from CecileRobertMichon/fix-template-name-conformance
ab3fa86ea3208382416d3cf909d56900a8d44293 Fix typo in conformance template name
f96048323362b2ce907e6fb00e5a6210a485be67 Merge pull request #540 from devigned/template-flavors
20d22ee601320ede392f210cd2d7d0c69386aa29 Merge pull request #552 from alexeldeib/ace/tiltfix
ab98452225b275912cf067860b92a881769a6e0c Merge pull request #544 from CecileRobertMichon/vm-state
a47f3a85a5595f9672b708b9497de1685a020aa6 :running: fix typo in tiltfile
ac00b33b0e09d52a321026b9efdf191c415bbb3e feat: enable easier flavor creation
085098b35d062f7b094d566400f540fac12a170a Merge pull request #547 from alexeldeib/ace/tilt
688bb34189c8fbe3186bf47c392a7c57b6e2f662 Improve VM provisioning State handling
d61404785c32750ee7da66be8eddcaf60cbb2b9d Merge pull request #543 from CecileRobertMichon/print-columns-ux
7db0e4448d9ca2c1902505f6671ea6d608015715 :running: allow for extra args in entrypoint
59e2947a86401253ab55ba80fcc61fdabfc7a965 Merge pull request #546 from devigned/dockerignore
ebcb01eced00cb9f345590770feabc041b9fd0db chore: by default ignore all files in dockerignore
3e567eae47a5c19c5a48b983de51ef64d407b168 Merge pull request #545 from devigned/faster-tilt
50c32119d21ee6e09eeea16c75e232d0c100069b chore: speed up tilt start and rebuild by a lot
8b58a223405182da0e051694bfb4bb485fcf1789 :sparkles: Add printer columns to AzureMachine and AzureCluster
ce5074a74fe55c664f8a4d43879e2ced56f2d41f Merge pull request #538 from CecileRobertMichon/ginkgo-ci-conformance
2cbea8199906f8a518e12ba97cc07d63c9f4c174 [conformance] Don't fail if can't move ginkgo binary
147f6fab9198b8033c2a7af7ccd1dc3896b04415 Merge pull request #536 from CecileRobertMichon/udp-rule
5d76898e8415ed9a0d90da655e1491623db591cf Add UDP and TCP standard load balancer rule
441bad0c5728652f3cf299b3e919bcfae1ad7e43 Merge pull request #533 from CecileRobertMichon/conformance-creds-regexp
4dc19785ffebf1be3b6d154faac4cbb9b15bcaf9 extract parser to its own script
c580dcb4d44ffd63202c8dfc720e2e32376c4db9 Change prow creds parsing to allow no new lines
47ebb3ae93e3d3b3ebc0cee66b4e1c22ef9e12a4 Merge pull request #527 from sozercan/external-cp
673ae475acb974f83daa932cb11df009e876a295 external cloud provider yamls
9fb2f9e56ffb2ee4b646f27461c25b20418d5df9 Merge pull request #531 from CecileRobertMichon/controller-tools
4ba7cb7929b6b4f626a9bd3c3d07808011d298d9 dependency: Update hack/tools controller-tools to v0.2.8
4fd63a5bbdeb520f14644f326e9c60384f96e983 Merge pull request #529 from CecileRobertMichon/conformance-tags
f8ebc07137a994f00389328e97ded9251318f52e Merge pull request #526 from CecileRobertMichon/conformance-logs
415aab57b83e849740184abfcd2d7412024c554a Add Azure tags to conformance resource groups
81bbf98f7cda0573a4b20fa84da20478afadcba6 Collect capz logs in conformance tests
efb5e12f6234ab3fbcabaac75e3fdcebfde1c564 Merge pull request #525 from CecileRobertMichon/kustomize-bin
4ecbcc210c69d418851bf8969646eaafd9109375 Add timeout to dev requirements and add kustomize to hack/tools
af6911b2ed5c330f7ac725136f27b39460755c9f Merge pull request #523 from CecileRobertMichon/dev-docs-toc
9934593fb7cb02a502dc37e1ad37c9fcf2bcd90b Fix development doc table of content
59e909e6691b7fc36f49aa4de3b12433df4eccec Merge pull request #518 from Prabhakar-17/514-update-clusterctl-docs
71eecc2775580bf643476095c20f778e2748a0bc Merge pull request #517 from alexeldeib/ace/creds
61d2df3f039e26847c10a0c7ae2defe9cb5747aa Merge pull request #516 from CecileRobertMichon/unbound-var
868f1fd843816307dc936a7e4f60a6097d1f8d4d update clusterctl docs
7db8cf77790972bbc074b33fae3e42ab44031842 docs: move creds before tilt for clarity
2c3a31164b9835d8552396169e390f8e0b39a0b8 Merge pull request #513 from devigned/tiltfile
9dc5df04f52cf396d6b7b04438cafd7fcba78a3d fix unbound AZURE_CREDENTIALS var error
970a21c16939abeda4b97d84f4651a2561d28940 add boilerplate header
0d4c2269818358281298fdb1d80f6818a7c60ef9 feat: add tilt support for capz focused
43d7f6e54203e5bed42312d3e16f645d05bb4be4 Merge pull request #512 from CecileRobertMichon/prow-conformance-creds
3f7afdcd8357cf78a2f8501af84ac53a0c3a4909 Add step to parse prow credentials in create cluster script
1161dc84602313e759e2d7890157e1ea172ee87d Merge pull request #500 from cpanato/GH-348
f2f7ef66f9445741cf4446f8dd7f0191314254c3 Merge pull request #511 from CecileRobertMichon/move-tags-log
56ba2694dd073e40c6365f56d99e0d65e1578486 e2e: making sure there is no leftovers in the testing session
425b4a70236c67cef9a74fadaaffe5988d633cea Merge pull request #510 from mboersma/update-dev-doc
a8411bccf7954fa5ea8ceef1f7e3f05f9a4d601e Only print updating tags log if tags are changed and get updated
08d4ac0833dd201ee7fb39f27003cbbdc76f0ff2 docs: remove specific line number linkage
9f437e80c4efce54f0cae77b71b4423e23364b01 docs: update link to current cluster-api vendoring
c2472ce08b69f06fd2ff6ab91a17c53b0314c5eb Merge pull request #507 from CecileRobertMichon/conformance
a04fbed6a435c88d6a8ff6071d38a6e92b4250bd Merge pull request #509 from devigned/no-registry
1490f4c4612e80a27d8d9ef94b0ba5b516054862 Fix conformance test script to allow building from k8s release
f0ae314d8034d216e40f8ddc7397d7661ab76d64 Merge pull request #504 from CecileRobertMichon/calico-config-2
dc5ee2c442b792278f25f3ce7f25bc73ce47015b fix: do not require REGISTRY in create-dev-cluster
01e1382e4b2d0d01f38ede5207f51c95d06a2dd4 Add calico config using vxlan
3b0ad944bb0341ddd0bbb0015c0245115b64351c Merge pull request #495 from CecileRobertMichon/readme-1.15
9adcc4b0f29933de9725e202826acef271c1d5b2 Update Kubernetes version support policy
d6121a16f591abbede8dce48915837a0fdb80cd7 Merge pull request #501 from FranBarrera/task/disable-password-auth
a042e45a289f664f5a0d8108006f58e0329feace Merge pull request #499 from jsturtevant/fix-failure-on-create-dev-cluster
97d6a31d747ebc894fdb7f73b03dccbd18effdcf Disable Auth Password
b70a244ca18c9c697f16fbefee77169201c39b9f Merge pull request #498 from CecileRobertMichon/fix-typo
e67160cdb19056883c0b23ff23be7b4d05b80b33 fix typo in cluster template
38fc61367e57af5ff3fce8bdb3e6aefd4d0b1448 should fail if errors during execution
c69a15665d5e7ca8cff63d848abe5398bca263ee Merge pull request #496 from CecileRobertMichon/add-exp-retry
c6e8899d2c8d31ebdfea28ceac8ba4b9be6e24ba Bump E2E delete timeout to 30 minutes
cf46dd003dd2cf1288df4527c364af05d5582b76 Enable control plane retry join experimental feature in cluster template
a347707e3c1d77c09c2a4c81d290d43dcf55ddd1 Merge pull request #470 from nader-ziada/3nodes-again
56bc6e4a1506184fa759efdc5aa65f0617297fda  enable e2e test with 3 nodes
c51eb63bafa42d0a7173091c2bd26a713b46478c Merge pull request #478 from cpanato/GH-346
e309a4b7c2b878dc5a126d89b8177fc8e91b5ab7 e2e/tests: add option to configure some testing values
43802a1bae0976df661ea35b0dd536935dbd2c80 Merge pull request #471 from CecileRobertMichon/kustomize-versions
292af671aa6df5074088c3d2b16c96050d665686 Merge pull request #477 from cpanato/update-azure
6b5755215209f095abd43f79fec35cb54c5bf781 Add "e2e" to E2E cluster name prefix
b19afcf7f2330544de8a76855f18bde8531ecded Add script for running k8s conformance E2E
b78d7dd6932e8c64c8e1e77f626e131549b1ba1b Load capz dev image onto kind cluster and make docker push step optional
9e2215b4b818e139e6df8c981fae57bc247e32eb dependencies: bump azure sdk to v41.0.0
cc16ce1e7a725a19bef4b319540876e5805175eb Merge pull request #476 from CecileRobertMichon/capi-v0.3.3
cf1baeadbd5c26cacbb2b37f6f232043751a512e Update to cluster-api version v0.3.3
6b74372dfb6cb61484453b839e012039351141ac Merge pull request #473 from jseely/patch-1
5ad3ea16c88c871531efac73092566dace993b60 Update kustomizelinux link
bccc58c3d0821b2852558db2f4b4ecc1153cc9cf Merge pull request #468 from jsturtevant/update-tilt-instructions
061aea894bf181dbda129433d9851dec36620527 add convenience script for manual testing
7c415c3103ea39d3679a67eb57582a5798a179f4 split cmds in makefile for new tilt instructions
70edc5198b79bd42cb7f96735739bb1c5f30b8fc Merge pull request #464 from CecileRobertMichon/capi-v0.3.2
82356c0d30c441be4933cbeabd6387f3a88189e6 Merge pull request #466 from cpanato/GH-440
eac4633c7afdc32237594b89291118162ae3a816 Exclude conversion from golanci linter
e2fc9397cff03d81096a1c8c69e8aca426c0779e tests: set E2E config Defaults with framework func
07eb25b871397a453cf957444338580b9b29bad2 Bump example Kubernetes version to v1.17.3 in development.md
c125720400c45405144d8d48b92ada7a4f511f92 :runner: Update capi to v0.3.2
01693421cbdf5617592e703e2ca4c33c11247be9 Merge pull request #465 from cpanato/GH-454-controllers
102ae12012e13f406b34e4fa4081d600bf75a543 capz: implement --feature-gates flag
266a2500654ac1e2d70325a8d81d2fb1dce0236a deps: add dependencies pflag
e13e38449e621f88dd2f3fd4597abae9b686da7a controllers/tests: standardize gomega usage
d28e87b9ff86b4bdb519ba583cbd35e17956d959 Merge pull request #463 from cpanato/GH-454-cloud
61b6a1e3dfb39f40648850461656d5309f3e5cdb Merge pull request #462 from cpanato/GH-454-api
64efc35641620b203d6c5c70f6b41c8d2a481516 cloud/tests: standardize gomega usage
2ebc7b4ef4c6fa6b1b130c9da3ef71bec2f0e9fd api/tests: standardize gomega usage
92ef2b666db93ebe70ba0c06479a3e1d46483904 Merge pull request #461 from CecileRobertMichon/image-readme
c89d8c5e6f79b43b0c32f730c9fce719949d2e70 :book: Update getting started link to build your own image
d648b6fa7f1ddd26ec67841a321d676febdcd102 Merge pull request #460 from CecileRobertMichon/readme-office-hours
a8c73496891c6bd383cea0d15d4e45ee7a277314 Merge pull request #451 from CecileRobertMichon/natrulesfix-2
e9fce5f30176afa9763cec81a53431bf8f2affd5 :book: add office hours to README
8333398b7fb04abe62a2689281aee5c214605419 fix: make NAT Rules creation and deletion owned by network interfaces
39bf9efe69267ee08d52bed0756dbc81ac1c0d70 Merge pull request #459 from cpanato/bump_azure_sdk
18cb62bcfb28e735af9e2679db5f096d057769a5 azure/compute: update SDK version for compute to 2019-12-01
994c6a999e28a064fd1d2f3e10cc69b192906050 deps: bump Azure SDK to v40.4.0
228976bc080c364f8aa658b36f59ec60da5aee30 Merge pull request #452 from CecileRobertMichon/readme-0.4
6f0b744304be791a831c49537c2057d46c074eed Merge pull request #453 from cpanato/GH-359-netint
d1e096ec7c1e71705b461b7e0af4c509588d5ed7 :book: update README to prep for v0.4.0 release
eed85879256714dd385a63be1ccd565d386f2a65 Merge pull request #455 from cpanato/fix_typos
30f1e8fb6648e2e27ae58c724d37d58da406c10a typos: fix typos
8bfba858a32850689127bd72098d13714d5b6006 netinterfaces/test: add initial tests for network interfaces
31c6670e5573548fedfae0336cf40cdc7c2a6af6 Merge pull request #445 from CecileRobertMichon/change-default-OS-disk
0dfe4ebd993fd97bf2a49c7b83339ff250dbadc9 fix: change example OS disk size to 128GB
905737cf81e32a49acb49c108455e374242df8be Merge pull request #429 from cpanato/GH-349
fa8e8c2726776fc16d1cbd389633555b44f5f7d2 tests: Load SSH public key from file via env var AZURE_SSH_PUBLIC_KEY_FILE
5c3e56e0ba0013515bc2bc43573a17d1520d2f4c Merge pull request #444 from CecileRobertMichon/https-probe
316a2a694bef75158af76a99084734517bc0f457 :runner: change the APIServer health probe to HTTPS
85d69865cb54f67a94dbae8762f164e74f0183a3 Merge pull request #443 from CecileRobertMichon/fix-conversion
88ab09c8169d02890b2391e61d79077c5bc2fed4 fix: conversion webhook should not return an error
725e1d8d0ee00053967ef3787305af9693b6cba8 Merge pull request #441 from CecileRobertMichon/fix-cert-manager-config
3091a8a59c1ea4beaa32c3f70e622766959810fa fix: fix typo in certmanager config
40223ab188645fbff570394adf0104be75683a3e Merge pull request #438 from cpanato/update-capi
1e281fc75df68b7cafe4871c31a232fceeafd89a Merge pull request #437 from nader-ziada/prefix
0dcc6ff038496b955750113a9eaef3901983373b capi: update cluster-api to v0.3.0
3985db222593164d43c4c9dd93ef1445fe53779a add azure prefix in template to avoid clash across providers
abb836403ebce4605300b72326d6a68f3110de9f Merge pull request #434 from CecileRobertMichon/fix-dev-docs
f07895865f9ac70c0abb1f8e9c248558152ed104 docs: small fixes to development docs
fe2753ad3ff5e30bc8c31b3fb36e66477fbe5a67 Merge pull request #432 from CecileRobertMichon/fix-template
f0e23ceb8691d34d01199e54c42f1494585c13a7 fix: point to node resources in azure.json
f1420f9f2a64f0f3f0624f1379fb52e545088c2c Merge pull request #431 from CecileRobertMichon/fix-template
ddee35ba57927cbe217e0ebf92bf4a6b6ee104e4 fix: add joinConfiguration to cluster template
5b9e7fb6e8aa17f54ae848ca1bd75b239afafe54 Merge pull request #424 from CecileRobertMichon/cluster-template
b10718906969905197d25de329e871ad99567f1b fix natRules assignment to work without name index
c13c5ed99f3373ed9ec46089f2f062ef61dce189 :runner: Remove examples and switch add cluster-template
cd396583e06e5be296862648867984ae78c4e3d9 Merge pull request #430 from cpanato/update-azure-sdk
f0f184c9033bdbbce3715e8560a36643671e6e71 dependencies: update azure-sdk-for-go to v40.2.0 and go-autorest to v13.4.0
70748174d52322b10f7bead5176b35a366708dd5 Merge pull request #334 from richardcase/image-properties
4780948ecfd5374154915da900a8c1a4320dba13 feat: image no longer uses runtime.rawextension
68c698c075d25d482e25ff65ddfb64a95ac90c43 feat: add new image kinds
3773c121f14da0a0cd8844e165bb3565d215e998 Merge pull request #421 from cpanato/GH-345
b20e05b89d2e45c57abcbb0bdf41c54a23bfdd00 e2e/framework: remove local e2e framework to use the capi framework
ceb3eb0c5c678e63d47f903ecc70b26a8a81dd2d Merge pull request #425 from cpanato/update-capi
4c95f8541295862c76904b360471b8b7d723da93 dependencies/hack: update controller-tools to v0.2.6-0.20200226180227-d6efdcdd90e2
de1a5d709f4c21a9d43c0d3008644e884cfb6031 dependencies: update cluster-api to use v0.3.0-rc.3
42b852a33883576f14fbf41cdcaf1768581fb956 Merge pull request #422 from CecileRobertMichon/capi-0.3.0-rc.2
08b7758503ca550aaa636bf841e72b45ccd8c7d4 :runner: Update capi to v0.3.0-rc.2
373826e06bb597c9ed33f1e3a84f06ca10c3691b Merge pull request #420 from cpanato/GH-385
3063eca65b2a1da4ad47481874ea8d0867f51d88 Merge pull request #418 from cpanato/GH-359-vm
5c4eb65404c04de81d1bdab7c4adfaa2aec33cb7 docs/development: update Mock section
66c7eb0eb3ce19e45501e9a280ea37e2e10b4dc3 vm/tests: add more test cases for VM service
fff8764f9409840b970467fde6ba6de5db76af6d Merge pull request #417 from CecileRobertMichon/vm-image-list
cded392cae2533efbdb5569e149f89ee7dd5d886 :book: Add image list command to docs
3c4f9892f6eb797784806b6e97cbbd4d436655b3 Merge pull request #414 from CecileRobertMichon/k8s-default
7a32c4ac49480125b5c799448303b34e5f8e2c06 Merge pull request #415 from cpanato/cleannicget
3ad66b2032891ce4f1c3ae79acb95843045508a1 nic: remove unnecessary else if from Get method
8679c032fd0804fa8a4e2863575e09b6dbd88aec Merge pull request #401 from CecileRobertMichon/clusterctl-settings
7997ccaa0f0033762abfc46b65dbfcd49c7dfcdf :runner: Update default k8s version to 1.16.7
5388cf1d10b4509842158510d005836ba3b24c67 :runner: Add clusterctl-settings.json
85ab17f3577b6de875658988538dc81936511605 Merge pull request #413 from cpanato/updateGetGroup
d2da121a3beaf4a084dc45bd91a68273584c0844 groups/test: update test and fix test names
98135dcf54b99adca5daab94a3fbc48aa4df8828 groups: make Get method ahve similar behavior as other
bdaa9df3a934bdd8485781b9d7d7159a240e052e Merge pull request #396 from devigned/proposals
fa08b71ddd34a64d5e69016181d8bf1a91fa16df Merge pull request #402 from cpanato/GH-359-publicips
22d44af516c3b3323dbd4fa4e3709d1d3fd2f9f0 Merge pull request #411 from CecileRobertMichon/remove-webhook-namespace
821a4edb664bff7a573e26ab04de50e34070aadc chore: add proposal issue template
f55ad84fdc51b674d35f1430366f62e0100a954c publicips/test: add initial tests for public ips
112817e5a89ecdd82e66276d21272860652b6e28 publicloadbalancer/test: fix test case name
930aee18c0ba51c088349e35aa04bb027e8a390d fix: remove capz webhook namespace
4ab2bc41cb53d1085fb9ef5ee845944907b2fb9d Merge pull request #406 from cpanato/GH-359-virtualmachineextensions
75cf4cb7258b86e1c6cadb7bec3387c55fa7f52b Merge pull request #404 from cpanato/GH-359-groups
c2875f8b773b487d13af1d902ce2eba684b880e1 Merge pull request #403 from cpanato/invalidspecs
74855ebcc4b048a00c4193511bdb10275d839c26 Merge pull request #408 from mboersma/fix-gitbook-link
fea95a948f56990a2bd511f4993114eb9e28ebcc groups/test: add initial tests for groups
0f8f23a65055e7e48b2f4bcfa1e5401c52723182 Merge pull request #405 from cpanato/GH-359-routetables
bd74b7f0e488be651b337c54dc2b3fe35f4f48ea virtualmachineextensions/test: add initial tests for virtualmachine extensions
b8f68d79746e01d30876fc4ec08f249433358636 docs: update link to Cluster API Book
976517ce9110caf6cca15861bf2c609668eb7589 routetables/test: add initial tests for route tables
40b2717bc9015864be8801fb138d8f886d22a122 disks/test: add invalid spec test and already deleted disk test
e368d083831afddbf79957ce7ffacd62727e5175 publiclb/test: add invalid spec test
aed17538f09ee47eb4832cf2c1e4823711f3bb85 internallb/test: add invalid spec test
2268dd08c4725f5f20d13e016abdbe7f5ec7beb2 Merge pull request #393 from nader-ziada/config-folder
5e0a7d94dfc605fe3fb64efd0797fbc7c21b2381 Refactor kustomize config folder to support multi-tenancy when using webhooks
ca6a0d0186d97162eaabe44c1f211726848b188b Merge pull request #399 from CecileRobertMichon/fix-selector
7e2a4c03d067478fdff22f490fc5d37632ca1e6f Merge pull request #394 from cpanato/GH-359-publicloadbalancers
26892d40baccf4553d30a4e10e7086c6ad6f8eb9 Merge pull request #395 from cpanato/GH-359-disks
9807624b6eb9c849829f1ed4f90a0143cbf95a28 :bug: Fix capi selector in make create-cluster
dfa19406406b56d10b98601432276c81417ed665 Merge pull request #380 from CecileRobertMichon/conversion-webhooks
65397b698c74d445c9c364355978da3dcf3321b3 disks/test: Add initial tests for disks
03596928b92c96f7dc95929e397c955f873029a9 publicloadbalancers/test: add initial tests for public loadbalancers
5295e9514373579d8f21a1ad5e8901cb476c0c34 clean: remove empty blank spaces
825388b77271236ab05ad62feba7c2b1e89ceb98 Merge pull request #398 from cpanato/bump-mock
18a581df206dc5e9a63ce42071f3d859062031e7 deps: bump mock to 1.4.0
14bd6a92e46c907ba15a58bc32efa6ca6cba50b6 :sparkles: Add v1alpha2 to v1alpha3 conversion webhooks
393be8446804ddb4a02f01695e66815e25f30db7 Merge pull request #389 from CecileRobertMichon/fix-tilt-docs
3b4df62e51224d2533c07c9476f218645af42467 Merge pull request #391 from CecileRobertMichon/crd-v1
f303735fdafd0df233d437a083083c510413333d Bump capi to v0.3.0-rc.1
d33561f4eb83999548481469b1da30f139d6c9ae :sparkles: Update to CRD v1
84db32bf7d2ea1e5e7c25d210cfe71e13beacc49 :book: update tilt docs
e5ed5319290bc07ada0ea082aeecf07421e2e856 Merge pull request #387 from soggiest/soggiest_remove
c94e1c1dc6010deb7cc7492bb5ea26726d198fa2 Removing soggiest from project owners
a6c1e38c0605fc1cb43a6288e8db2a78e7a68612 Merge pull request #386 from cpanato/update_azuresdk
e53a880601df6db3e1df8e1903b75585957f9137 Merge pull request #383 from jsturtevant/dev-getting-started
d7ae574322afbb6bf93c00b19e50d28e97090aec Add links for developer getting started
e9b83ba7f60035acc1ba7452e32b4e1f310e8b2a azure-sdk: Update dependencies to v39.0.0
83bd3d37c491155627aeb6a9c85b51477adf1a73 Merge pull request #374 from cpanato/add-health
270365c864e0509c38995f84e5277ebbd4b51f1f Health: Add liveness and readiness probes
920be2039a800ff7c0c7e6c6519e34b0d0e8278e Merge pull request #382 from cpanato/update-controller-tools
8efd21e25b5adb561785c88047969e98d481db2d generate: updated crds
b955ea530041e25f5323dbf8cf9a6ddf835a0dcb hack: update controller-tools to version v0.2.5
2ed8b47b7959f71a83431b55986225fb0ed7ef34 Merge pull request #377 from cpanato/update-go-113
d3f136814d9a37a97f3337088ebc098ce2707249 go: update go to 1.13.7
f9a6f8b3b7390bbee4ce0d4a6e9ceb96fe2f79ca Merge pull request #379 from nader-ziada/kubebuilder2
1ba567e0d2fc60fd7b977e270df7a4a1523ed412 Migrate repo's PROJECT to Kubebuilder v2
2ee4129afd89ab925fd318d020715e1b79bc1501 Merge pull request #378 from CecileRobertMichon/e2e-logs
2ac9448b3f06ff4144a0f332c4a3ea918a73625c Add log artifacts for E2E tests
9c96499f05125c40da3116153fd0490c52be7b1f Merge pull request #381 from CecileRobertMichon/change-e2e-vm-size
28c3bb5997227b60f4c2813b0dcaa0b901cee310 Use random region in E2E and change default VM size
b2f613f22fb046d41009a4ccd29cbbd51ce1473a Merge pull request #335 from nader-ziada/v1alpha3
107676e2bd977737773807913374eb4de7a1f0ca add v1alpha3 api types
767b0c06d57525ca9eafcc50fcc16d7741162684 Merge pull request #373 from CecileRobertMichon/docs
d5d393c393b56e68e7244f6fc47ed9c9bc7031a0 docs: update the readme to point to capi book and cleanup getting started
c6c4b764139b1a3aa564d31d63a481513ff7489a Merge pull request #372 from CecileRobertMichon/add-tags-e2e
fb0ee2ad1dd9ea52662b53beaadd99002202d046 Add tags to e2e resource groups
9200642aaae900065cb9c33d6bdac2ac4b745949 Merge pull request #370 from CecileRobertMichon/k8s-update
9fa53070786ad4a8937de8b272847704c26a762d Merge pull request #369 from CecileRobertMichon/reorder-owners
acf2ae1bed27bd15cb7e57fcbaa0ce8d45091795 Update default k8s version to 1.16.6
a902ddc3720a4d5b48c2ac31bc57271e6f879061 reorder OWNERS aliases alphabetically
2c5b4855d88a919fb3c2a95a6c7d91a4f8aa0c17 Merge pull request #364 from CecileRobertMichon/e2e-tests-improvements
4396e97c6c22091a81678ed4eefa5ffefdbf9044 add 3 control plane cluster e2e test
c3cb013c81fbcdaae40d6e9136f3fc54d31d6453 Merge pull request #368 from CecileRobertMichon/add-nader-ziada
f5e6d279231de9df64fb45c370675cc6728a5889 Merge pull request #366 from noamran/359-az
e3fd64edb02bcbc918469d1a371d0064a124874f Merge pull request #365 from noamran/359-ilb
c390c16b19089f0070bb479d301105cdfb75a7fd Add nader-ziada as reviewer
6135007bcd70d569c5df4574c63d024c27de58d4 Merge pull request #367 from nader-ziada/timeout
51fc71b21fe6a0d534a8c52a6ad3398707865def increase e2e timeout for delete cluster to 20 min
3abe69ac7913477254f1c4b17abe674aca1d9aba add unit tests for availabilityzones
95eefb31c967ea54ea68c00ce8325b006eede968 adding unit tests to internalloadbalancers
07d47dc06571bf8021957e9ae6529c5aeb4ecfa2 Merge pull request #363 from nader-ziada/subnets
d49de06ca6a59c04696f33119b70d39a55b107b0 add unit tests for subnets in the cloud services package
152c0e1ebb22823696e128d898bd69436c21645c Merge pull request #362 from CecileRobertMichon/capi-0.2.9
b7c4749487b7fd221dc00b552735cc0097d88a4d Update capi to 0.2.9
b4ffb377afc10239e84906d19761fd46597d880b Merge pull request #361 from nader-ziada/securitygroups
179f29970db5ab2b1ea056c8b1d489b91e64df63 add unit tests for azure security groups
3ea9e6ba120875dd785591ac29f4fb03039b0e27 Merge pull request #357 from rbitia/master
e2f7b18a1c6f4327a458f2b53f688afc9b1414db Updating getting started docs
178e4ba3982213c5b6d2327441f8bab13947c1fe Merge pull request #358 from nader-ziada/kind06
a77f0ab533915c4f2ca4d0a4cb2d26f9fd312d47 Change kind min version to 0.6.1 and update Makefile with related changes
90e00dadfd1476e777b93120a67bc8268d451afa Merge pull request #340 from CecileRobertMichon/byo-vnet
ef8b3aa16f5142a857a230b3fe930aeb0318f847 Add support for custom vnets
6df08dba6927b091f4ae3364ef77b8c3aec77896 Merge pull request #354 from CecileRobertMichon/services-tests
234942263df22a8e7dc4da85be3dcd5fdf3d4dd7 Add virtualmachines test
6a003f8d1ec364f39f5cdb09e61d19b5d11b116e Add generated mocks
9bb84dd15a4fc7d86d2f32f149dfd8dc1c7476fa Add mock generators
cf33d8b3a99a53030cc813d13600e59dd7076648 Refactor services and Azure clients
575b26a479985e604120e788a14052a216c672ce Merge pull request #353 from nader-ziada/tilt
4ff00d5fef09e322cbadf0e610b7e5c2e28537eb Merge pull request #343 from rbitia/gettingStarted
582cc358ea63ae2d52ed9cacf6c30867b90b322e Add tilt provider to work with cluster-api tiltfile
55718dc7d389f48b303b4aaa734550216c6932b5 formatting
614bb021e01219afaac7e46e85607a8a883acb7c updating link
c56681126a79d60e176acef5c9911b87068d2514 Merge pull request #339 from jadarsie/e2e
e2a6553e7eff4af2d0a66cafedad97c32d04ac13 adding links
c33eb04437c6941377e5e309218576dd467a50ad Merge pull request #342 from CecileRobertMichon/get-image-skus
b6d55487fae74b7240e7467b23f2209d8ff2825e Update default SKU ID naming format
d7990ff5b638ebf8b96f651a6dbfae6d61eebff4 Merge pull request #341 from nader-ziada/tags-unit-test
4f1f20b64a0e1bc6adb21421de6345888d66a1e0 Add a unit test for machine tags functionality
1567581fffdc2daa272aac227b5b6c6a3961e191 [WIP] v1alpah2 e2e
ce38b440123e1ffcaf04fcd2089a7b5277eb2f9e Merge pull request #333 from jadarsie/e2e-script
b5e39ffbe0913daddaf40688c3665827a61f3c8f run: placeholder e2e shell script
f16ba50f965deac2ece142b0d9ec2dccb0805dd7 Merge pull request #332 from devigned/make-test
106a6d3edea5e25cda5124b1f6bbbb656bb61571 Merge pull request #331 from devigned/getting-started
5da22fb0147e138823e77022becf69b2083b8394 fix: correct developer getting started docs
5a15505bdd9186517e4f233e2949db2177af9aea fix: make test should work without having to run ./script/ci-test first
2a27d0337abccdbe3f87effe936465225fc1ab14 Merge pull request #327 from rsmitty/public-ips
6a5654b7d761b42ee1257fd107f2c3a7c89443ed :sparkles: support the ability for public IPs on azuremachines
7e6d4ec2faab649086bbe648827696a89abfecfa Merge pull request #329 from rsmitty/master
db730adb8b658c80337336ee7dd1a676e3de9907 :running: Populate address status fields on azuremachines
3eab7980efbf92e19623e0dc56f6a62b17477a0d Merge pull request #328 from CecileRobertMichon/get-default-image
aa80ffd1a6c3130cc5867ed6c0f77cdd5df31e52 :runner: Add default Marketplace image logic
a5d3f054f429b1ee14573b0f2a5544e8c777cd34 Merge pull request #323 from CecileRobertMichon/update-capi
52322bd08b1308081810e400fd6461bc129ebccc :runner: Update capi to 0.2.7
f0167525238edce204f36fd7eef606d83a1aeed9 Merge pull request #322 from awesomenix/addcecile
7d158fd1c68512e5d1fc43dd4116147a29895e28 Merge pull request #321 from sozercan/fix-cp-identity
8f7e5170bbb77869909befe803243597dbb90f63 add aad auth to cloudprovider
25c8b482a52eef5eb3b5a3bfe3358a8186dd95d6 Update OWNERS
c618f8e717eaf8c8fc1df092d7bcfd917ca7b9f0 Merge pull request #320 from CecileRobertMichon/update-image-to-1st-party
b703ddb6bed2d8256a68cc7f7aa205919e2f28f3 :runner: update image reference to use first party image
46e257ccfd36af04e30e8d41d6246c9edd22a7c1 Merge pull request #317 from CecileRobertMichon/existing-rg
50303316b470233aa75163cd70d4dddc3a8ce16a :sparkles: support exisiting resource group
d93e75deff2be3c7647c2ddfd387ce0ef022e1cd Merge pull request #316 from CecileRobertMichon/tags
7f2ec765f9d813b6cd002ccf1b5aa42526e682e8 ✨ implement Azure resource tags
e2f14d83baf3bf766783d8167710dd87ae48480f Merge pull request #315 from nader-ziada/bump-k8s-in-examples
d1091dffa7cef3655f2817f62e7b28aebcb839c9 Bump kubernetes version in generated examples to 1.16.2
ba0a8cd769eae300e700a3347eb2e67255707ad2 Merge pull request #302 from CecileRobertMichon/remove-prekubeadm-commands
506c475371f3da2031e1332a600ab85706c85b28 Add default 1.16 image and remove prekubeadm commands
74913681a01380865742f34782436a6a1d1f57f2 Merge pull request #308 from jadarsie/jadarsie-labels
a609e71ca0c37ddc85580f780db1dac679cd3b1d update labels provider prefix
8b65efc5dce3f17f0d4b96f6fe0178f97fe38059 Merge pull request #306 from CecileRobertMichon/golang-1.12.11
540617c248aa47b5e08a32e3fa1710a767d54fd6 Update golang to 1.12.11
71e3912157de17494a32a14c0b7f8681f399c6b3 Merge pull request #305 from CecileRobertMichon/update-golang-2
c8ad69a1b05d6f2c694b38d0353b9ec7664c2739 update golang version in Dockerfile
d9cb4e34c5dd7aefcd2624095120652c0881f698 Merge pull request #303 from CecileRobertMichon/unit-tests
518b2bf5bcdc8d2330c0f43da46ccaa9daf9d3e0 test: add some unit tests
576926e553f14850b0eccb3634adb7ae22735971 Merge pull request #304 from CecileRobertMichon/update-golang
e596546d9090828932eb334a876ffd57af8d7212 update release binary golang version
c373acd0911cda1ebabc42e806c2e545981d7c7f Merge pull request #296 from tahsinrahman/verify-codegen
ece5ef11a3ee7d61b150cdffea143c937694f455 Merge pull request #297 from noamran/LeaderElectionID
026dc164f8d1e875822947e236aa87ea59ddf382 Add rule to verify generated codes and manifests
4d26bdd7ccf558c430ddb9819b37e68f65e0b568 Merge pull request #295 from justaugustus/az-fix
ee4f76e799c10d06b4c784f21367ab898b63c660 :bug: Validate a location supports Availability Zones before VM creation
273afc804bf1f88c4c32b0c624275b88f05d443d Adding a unique LeaderElectionID
7f17ca164331dcfbcf9f1fa9e268635146e19c73 Merge pull request #291 from justaugustus/image-ref
79c3d1bf7e0e8b105377ed214984f18b78491b31 :sparkles: Support specifying VM images by ID or Shared Image Gallery
2688c11577dd4ccdfce0c9f14dcbe97cbe449e34 Merge pull request #290 from jadarsie/group-client-delete
4968285e0f13a696b8cf3bfb6348f9916a31851f fix: delete cluster retries forever if group does not exist
f9feeee42b3b4fd854d3dc2a3346b496f5b6e723 Merge pull request #289 from justaugustus/containerd
5d9c2a0a2c88dcd9b8388bd147afb8937ff131fa Update containerd to v1.3.0 and allow configurable versions
c1030c7a655253911cc8be93ae78f7636237869a Fix manager_pull_policy.yaml references
18cb528c3d9e75a9a8614c1a02a62dd1785ac4ca Merge pull request #288 from justaugustus/116
7abe8efcf5117073df08805fa9a81f715b9bc071 Update default Kubernetes version to v1.16.1
df7b7133bd18b2764d056a57a9b1280be05ce4c5 OWNERS: Add CAPI maintainers and update labels for SIG Cluster Lifecycle (#285)
4ee226173e59472c65231aec624c87eeaea4e2b9 Align Makefile (release) and hack/tools with other repos (#286)
b02098a1bd991619c299d54bd4a1bc262e12158c Fix manifest generation failures (#282)
6edf5c9c47c7190bb8b98a4ef68a8f80ce30d329 Fix CI test failures that were based on v1alpha1 tests (#280)
c70301d3c2ebae15258ef90f6f5ef9b139ad5dd3 Merge pull request #281 from justaugustus/v1alpha2-reintegrate
03c82d01ae35e78873aae7df3fe173958b41f67d examples: Point CNI manifest to master branch
c04dd4863f999d395984f1f728fa009187f4d5fd Merge pull request #279 from justaugustus/a2-data
b5c9e4e4672850180babd1c0a7c67b16a7f9cd07 Update Calico to v3.9.1
853c6a65bc76867ef186f79579154d7b4121df1b Temporarily move CNI deployment to postKubeadmCommands
9272174757d8d20371a1f28fa00785ca20eb3d24 Merge pull request #278 from justaugustus/a2-data
a4e429fa1adfce46d3c75e16192c7880b40cb5a3 machines: Re-enable support for availability zones
9bdbef6dbd33297678c4bc43095c923b3e5d2533 Merge pull request #277 from justaugustus/a2-data
8e7bcd41519e3fba5891923b050c914c0650a3d2 controllers: Comment out/remove some logic that isn't wired yet
2225acf15eaeda24c74e27bdac0388a5fb6392be controllers: Add reconciliation logic for network interfaces
6b38be5d0e8c359384edd393f9ff2bd0b1cdd4f0 controllers: Rename azureMachineReconciler to azureMachineService
4b0ffd0e3135fed786d01ed2a3cbb077e0ba917c controllers: First pass cleanup of reconcilition logic
b1431c28bf3365264374421cb55b5cacfbc4352a controllers: Make logs less verbose
e07d790af666b84390e3c5b1c65014d601fb7ed7 controllers: Set VM state using compute.VirtualMachine.ProvisioningState
a8759da01a62bf7e3f01516b9e7accc4fa5f0ce8 cluster: Allow configurable APIServerPort
15df001a04ac305fa2b23ccc38e898827439c9dc Configure nodes via custom data instead of virtual machine extensions
95b36b3c8b98f418368274b4d2a15c498ea4661a v1alpha2: fix AzureCluster controller (#275)
50be4e260edd7971eebd8d886101e5f1db29ac42 v1alpha2 phase 3 (#269)
af9c3c6c349fb182cb586595dadc7e960ec02aff v1alpha2 phase 2 (#268)
69c248de8a88a3b9e7fb1dc4e11ccd1301f8fc05 v1alpha2 phase 1 (#267)
60b7c6058550ae694935fb03103460a2efa4e332 test/e2e: Quick cleanup of presubmit failures, deadcode, copyrights (#265)
a994d89af6b7d43c51592a461ed102c5c110e4d3 Incorporated E2E test changes made in CAPA (#264)
7bf6590e249c62d8a99509ad0dcad487aeb0cfd3 Update kind to v0.5.0 (#261)
31ca800c5c3c59009f8525c3da3f93c170f821d4 Merge pull request #260 from justaugustus/bump
696cde98f4b575f2e9d11233019224de4598d133 Update vendor for Azure dependencies
022450e71e313f3e953c18ebe09177e5825555c9 Update Azure SDK and go-autorest dependencies
7f8dde86ae19de3247ad92eb8a0bccf160fceacd Update Kubernetes to v1.15.3
c79b9182ee425cf2d814e72339fa8f22ce1d9387 Make scripts more compatible (#257)
588ac83f44173316cee1d74ead06eba1a37fb6c1 Merge pull request #254 from justaugustus/bf-2
a8c97535e6ac2ca6ecf5460aab32b125c8501162 Update Calico to v3.8.1
03229f2ef6d75c9c58855b48506e3b3da389babd Add additional retries for containerd downloads
61d388168aadc84096f807355442b1125890acdc Update vendor for sig.k8s.io dependencies
42d1a7ccbdb17fc7eab061e3ab01bc42e069c8d6 Update cluster-api to v0.1.9 and controller-tools to v0.1.12
c89149b2ef65b16e6066366f9610e66b4e84bf51 Update Kubernetes to v1.15.2
1550c97901a59a2477e3348224757831da5c25ed Refactor certificates usage and update tests
e55ce6cf91ee7ea18b765bdb093e006a385a7039 cluster: Remove ready annotation if control plane machines aren't ready
90252958da2e3c12c8b8afc6d257f352f3fa54de v1alpha1: Remove DiscoveryHashes from AzureClusterProviderSpec
2a5db81440f7380a50725d0e191ebcd66e75733b actuators: Remove duplicate isNodeJoin() and associated tests
d6696c606ef01632078c13b6ceeb49a935103bbe Update actuators
0c3c3ae2a3bb095428d4cbdf76a3ec6e3dc0886b Fix control plane machine race and add support for NodeRef controller
1a16e86e576a1bf8e5c705311320d4de68e833ca Update certificates and add tokens package
4a1ad347d3e81fa932268a1e26ee291b05438d51 Added ability to select AZ (#256)
0b35ca0d4bf64c01b069ea3171ae3b3a797db5a8 Update Azure SDK + go-autorest API versions (#255)
429b6bb21a130fc86a3002c1e20a9f3030701c0a Merge pull request #247 from justaugustus/backfill
ace1a622c2522c8e57750a5582b6c7156c22dc70 Fix backfill of clusterctl and revert some portions of Makefile
6aaa10e5bb6a96016fdfe944501c9bfe316b30b9 Update vendor bazel files
720ff2e26cddb7e4509a7f505b3dd5dbdb4945f3 Add pkg/cloud/azure/services/kubeadm
39d7d24cf8630baa3a37f5e6defae2743693e7e6 actuators: Wire logging to cluster actuator
82327ffc8524834e7edb7e58720eeaf12694f783 Update hack/print-workspace-status.sh
269d1dc0494aff4340abffab6e725ecbe8687131 cmd: Update release tool
1d57509eff9cc7882eb566261792ff68af0e9633 v1alpha1: Expose kubeadm configuration in AzureMachineProviderSpec
f26321c82d4552d3e217b744b67fec95b33ee802 v1alpha1: Add register_test.go
d06ade7888d276060e9ece286697aa0c1b6b7dd7 Update cluster and machine scopes
1712d00358d8dd414835a1c5f613990df0febd2f machine: Set the ProviderID if unset
763fc38d0f021d6ddd6a6d2fc454e056c7979b11 cmd/clusterctl: Backfill logic
b2b0dff808afaa859b23d88b438e5cdd1c8f6376 cmd,pkg: Update manager and backfill logic
37547f8e5cf605646586e018a4b68d10c17b205c Fixes cluster-delete in Makefile (#253)
032a3313222c2c87112e4b322ce360245cc7e528 Update CAPI to v0.1.8 (#252)
ef5922f4b16f8688d15de60c7170a06a8abb5c50 Update OWNERS (#251)
bc5d30734fb6b3c05ab246b8d39c539de49a1c03 Fix secret list RBAC for deletions (#250)
bd86562830f2a618456e841586ba658ef263556e Update repo documentation and dependencies (#249)
1c57a13858acbb89a480cdac6137894c39334699 Remove SSH private key material from AzureMachineProviderSpec (#246)
31132e7f4602b1ffa42d714996ec1b2c727050f3 ha: Add logic for NAT rule selection (#245)
e771d8c3a69705ac1f3821f7b8ed7fd112d095f3 Add e2e tests (#212)
92b9c2a2b0d8fe2470d92d8f79606448af6299d6 Update bazel workspace (7/4/19) (#230)
99fbe5700f95d6d55a4f60a53d6e2f4073280251 HA Clusters: phase 0 (#243)
73ca815302cab91ed3fe9c5b83e390557a966bde capi: Update CAPI to v0.1.8 (#242)
a31c5315a5191cf3e5390b0bc8918095b0f29f87 Update Azure dependencies (#216)
be2e51956570c93e4a74c3f5a8764a34d64f639f config: Update cri-containerd to v1.2.7 (#241)
8c6bb82a1f09e47d4b83f89ed1086c48c18e07c6 Update Cluster API to v0.1.7 (#240)
56eb3b459a6d7e5fe2ad835c11960b1648d78aa1 Replaced the echo commands in cmd/clusterctl/examples/azure/generate-yaml.sh environment variable check in favor of colons. Using echos here is unneeded. (#239)
23aae3f3ca85dc6f8b9e58a179294ff9b12079e7 Added check in generate-yaml.sh that verifies the Azure EnvVars are set (#238)
b24fc9b1ee0a7e54c179524ac063044b2614bd07 Add mock dependencies in tools.go (#237)
efed85ba1d603d9702a804ac8c31144b13ebe2d1 Go modules (#231)
64cf98149cec16a5e476ca5457ebc5ed85fec12d Update to Kubernetes 1.15.0 (#168)
9b553da079817f83fe7659696d5a88b60724463d fix: infinite loop in SKU iteration (#229)
72b033205500e85730a496517a3e58b036b257ac update Bazel rules_go and bump go version (#227)
2cb119f4a01ea085d4af00e812e66b6e54a9bd31 docs: add note about custom script logs to getting-started.md (#225)
6854376800e1da2b3115dc77e7eaa2825765ce3e add retries to containerd download (#226)
8ba867dd9521fd705df9967390627ca5325b252e  fix(availabilityzones): iterate all AZ, consider location/AZ restrictions (#223)
4b9a297dc311eb2a539f09053a683448bbaa0169 updated link to the k8s bot page (#220)
c1ede557516c6cd99917a02083e33d0b343cb1ab Setting Dockerfile FROM 1.12 instead of 1.12.1 (#219)
91aae2d923a13c897a0bb5dbcf3e04aa3222dcd3 Small fixup of getting-started.md (#218)
75320e02e236c34366ad40971174c120d578fb20 Update CAPI to v0.1.3 (#217)
50fe273556fbe66aa3e796901255167fc1cab878 bumped version of go as well as kind directions and added make (#215)
528b8a7a13c47a23f8835456fa4bcfe0866c3008 Wire context-based logging in scopes (#214)
1db1fc42d4f57a80537526747ff4a9927e7dc52d Add GetControlPlaneMachines function (#213)
c4131eeaf4ffc8c115b9084ab0ce970cf4fca36b Update Cluster API to v0.1.2 (#211)
34e40da451c1e49635c713c07a024e30f03cb5f7 chore: bump capi back to v0.1.1 (#209)
98f2d4de311ad025d0d0bc3d66944f9195149e55 Update Kubernetes version to 1.14.3 (#210)
07dfbf8e68df887e26fea42796e93c6ce950377c Revert "Update Cluster API to v0.1.1 (#205)" (#208)
8d5d5c398a14fd0bfdc5860b09178bf4ed14d7d8 Use Calico 3.7 (VXLAN) as CNI (#206)
d8065d7c20efea1afbd4f14e1391a22594dec77b Update Cluster API to v0.1.1 (#205)
e1f358dc8cd5675911178ab180d04e613aec9e18 fix: delete OS disk when deleting VM (#202)
e0aae3da8875ef63cb38c4f32df083894b33af3a Review #186 (#187)
9d988a5a7025840b0842904a776f77dc91ae0066 Fix containerd checksum (#186)
93549f26c239806a04b86ab703e940511d8d809c s/BUILD/BUILD.bazel (#185)
08ac1b36f7a44a4746209177c3632b421ea423c2 Add mock interfaces (#182)
0345fdfded5022f0afc9ae053f3f5c1fee8c40cb Update dependencies (4/15/19) (#184)
3acfcd4ffdc89c0702b1384885f14c35d33adae9 Use Canal (flannel + Calico policy) as CNI (#181)
ce3edcd0e01b37e8c4f6e40fdd819d7f93292338 Update Service interface to use Reconcile/Delete methods (#180)
f34798460b7a9150289c2f81867c8e5619e69e8a fix: align comments to behavior (#179)
0b7cf771058e2cef05e99b048138454afd12616e Use errors.Wrap() instead of fmt.Errorf() (#171)
8a2fc409057c863f87c917ab6abc39b00d259a0c Fix frontproxy ca cert (#176)
b741bfc1833b9a49870665382ce5f8a7c3b7f52d Fix incorrect internalLB deletion name (#173)
e95594b59eefe028ed77056c898f1efc1bd7cfc6 Add design diagrams and notes on code, for easier development (#158)
0aec2b5b51b733afac736f1f946a7c726badc883 Add node role (#170)
642d563b9e45ef27840fb59eed55229d9ba2878e Fix kubernetes version for node startup script (#162)
6c364f9b67572effe331f724dc3d67fc10eb7f4d Update dependencies (4/1/19) (#166)
17139470c67b229d28657d398efb3e67c2129868 Update to Kubernetes 1.13.5 (CVE mitigation) (#164)
149815f8b5d8c049d829c1fa561a8a3ce49fc73d Update OWNERS (add juan-lee and serbrech as reviewers) (#163)
7ddbfd8b96ed2a296f495dd2b7c971a44db3b41a fix: Support Availability Zones based on regions, automatically known using ARM API (#155)
912967cde31f3d35857c8d4b9a6829d9792bd0cb remove tariq1890 from the list of maintainers (#161)
3d7c03326b06ea6c825cd4e899b61e2134f61469 fix: minor fixes to increase mem limits, ubuntu 18, kubernetes-cni 0.6.0 (#159)
90d73c3506c004964ba572f416f59aa5ab48ea7e Add md5sum dep (#156)
f53efdb852dab776e412e4c0cd5a91cc3f760019 fix: Release tooling and documentation for v0.1.0 (#151)
27261897f5535c5f6dd92c26fe0a5938aa39b2b1 Enable deadcode linter (#152)
9499217b0cf0ae2b2c5de1b95c0f85b5723726c5 Release commit: v0.1.0 (#150)
c4896544d32792f06f5302c4fd9d2b4fdff358e1 fix: Generate consistent names for Azure resources (#149)
16cbc7c74482f25fc94d990f05ad2f8900b00656 Update developer toolbox and documentation (#131)
9fdc475c6b5145908d3d9776df89a7dcdb850d9d fix: Restructure machine actuator for unittests, and add unittests (#145)
592c6c2a74777a7efd359759850ba6e82dd5b094 Remove hardcoded values from virtual machines, respect values from machineconfig instead (#147)
d40b7048e5563e1480e3909b0edfa5cc84a6fb4d Update OWNERS (#146)
1385811a67e1b1ac75b7ffb726cb9a162e7d5b83 Update dependencies (#143)
b55f066db9cb0f96e81257150a2468942d3996ba fix: New Compute and Network micro services convering machine, cluster to pure ARM calls (#139)
337027423d9bc50c1df194711ee3c6952241c228 fix: Create a new Generic Service interface which provides an individual azure service easy for unittesting (#138)
4b67c07f265af112476d744233749fe9808d2816 Create certificates, admin kubeconfig, bootstrap token and discoveryhashes using kubeadm (#136)
4dde368b5d0dca9a75c3f7c90053232b9f975b2d apis: Update types descriptions (#134)
ac592b875eb7f7860d2de541bf38bc21d3bcc9f1 Update cluster-api dependency (#133)
1933018cf27438c6a5a3773a50cb1547fb2c285a Bump dependencies (3/11/19) (#132)
cff198e983d246eeeb3b1b650dd2792ac5b95c0d Update types and actuators (#130)
92a4ac45c4b4bf4c8482e7af0a1eeb226581b135 docs: Add support policy and update release doc (#128)
0ae66db77cfb3c99873173d6d89f068996f03c7d clean up bazel workspace dependencies (#126)
a88f7ccd14bc65839c46c2a56dfbcc94b60bba33 Update public IP creation/reconcile (#124)
3fa0d0d9031c7a33f66489da15c181334f97b3fd Additional golangci-lint updates and lint fixes (#121)
bb35bf3c2aa1b92ebaa5d6d4f6a5c75c2a7eb5de lint: Update golangci-lint and fix gocyclo issues reported by golangci-lint (#120)
bd0edaf97c13cbbae57a34e10e527cadcfe16312 Update dependencies + k8s version (#116)
a6c7122c9932a0fd7d686740e96676bb622dceef Update configurations and package logic to enable builds from master (#99)
9e84860eb9b1b00b3457da78c621eb4c51b7f591 docs: Add documentation on the release process (#117)
53d79c5cd1d04f01e4af8380bd6cf66c29d626d8 Adds Bazel code to generate necessary RBAC rules during a build (#96)
e22395e2b0e66c1d65549fb24c6d5ab2fd37ca82 Add kubeadm configs, load balancer, public IP, refactor actuators, types (#88)
7f482be1078f6836d8e59d4d4aa7622b4ee5ade5 Bump dependencies, backfill capa (#90)
dbf51ef64d71c9bbfaf97b6c9393266406200c11 skip e2e test if KUBECONFIG not specified (#81)
a2b540afb1eb4eb11c478e0906e383661df0801d fix references to bug report and feature request templates (#87)
5b646bf402330a689fb68066402e997377b6d550 Add Azure manager template (#84)
fbaaf16f275893b04687f3965afb14d9238534d8 Add bazel, improve documentation, Makefile, workflow scripts (#83)
2c3c12e79aa0072e7c092a94c16d15569f049b46 Refactor cluster and machine actuators (#68)
6cef53ed62edb88529c2d3a6204e58d0e419c273 Add boilerplate for scripts (#80)
5a8ee67ba46dc0e8161ed19382a7575571dbbc31 Register all default controllers, which includes machineset and machi… (#78)
0f14a6bd564d7c709e4575d553568473bd5b8fb3 Removed files related with az pipelines (#79)
93a9313a3f680a17e6505f3c5478303b80ccc0be Fix issue templates (#77)
235e8beaacc05954ec3f25480c58e5f7756d0cab Added kube.go back, and its imports in gopkg.lock (#73)
fa4c96bf33d2c749e5b56753d761e4148cf2bdbb Added GOBIN path in Makefile if not present (#72)
827e9a2bf5a3eec792d17c56b8e6851b451c509a Fix all linting issues and improve the make check workflow (#71)
7bca15df1bbf5f0254240ac430899c95898cb95e Update Golang image to the latest patch release (#70)
072605bc38b18229119ee78bd232875577ea3206 Misc cleanup to unused packages and adding copyright header (#69)
c9cb138b0b6f47dd246e4875545b18cef0af98ec Update packages (#67)
c85a040442826ef5de1b043438661612568bda9c ran gofmt on machine_status.go, machineactuator.go and virtualnetworks.go (#66)
7c629f0b99449b0a189043431c3bd2caf16da0db rename cluster and machine CRDs to reflect the latest cluster-api specs (#65)
af9ad77181a71e2d98619fc74d86605e7f517adb docs: Minor improvements in README.md (#64)
e96e43d21d5a08be30b2ee66c52abe36e1c18dcf check command, used in test-infra (#62)
ba8a03dd577cc2293d25efdd430f7595a19da299 updated the golang version in dockerfile (#61)
5ff65a964cbf1dfd5488ebf11c31d17244ff1475 Adds pull request, feature request and bug report templates. (#60)
ba0541df584146f3d75c9ab307fb8b0546ea69f6 Fix golint and misspell issues (#55)
8b7a6d519dafca4fe4b73320f7577453bf5677e2 fix goreportcard links and ineffassign issues (#54)
a5f718477d87b208143878ce8a493d22e97ded9d Update cluster api to latest version, which changes renaming provider… (#52)
e793396819f48f75e39053f0ebe7eddf88268f94 Update remaining platform9 paths to sigs.k8s.io (#51)
51be9a38eecb800d1a344ff8f48192cef7563240 Improve generate-yaml.sh (#50)
01eb190bf77fc42da776ee3a097956e5d670896b Improve readme for better usability (#46)
80ab958cb4147d729c67fce6c46024d320fd69cf Update import path for kubernetes-sig (#47)
167c604a3a04b37b77f0131a58051b63b6d40464 Use latest versions of Azure Go SDK and go-autorest (#44)
c484154cb025b3715db6b7a3dff5dca4efc4738b Conform to Kubernetes repo requirements (#40)
bdab4ef6f42f5e876679e66fae537d85fdf8a63a typo (#43)
a40a2dc41b8a590f13554d09adc3df5a4cb1ff62 Revert "Add node e2e test (#37)" (#39)
8af53a5e097dfbac3036c12bb3c8f6bbf4c14b83 Add node e2e test (#37)
0e3576b5831bf59b2699a50fee8b43e200f58db5 Add Actuator Unit Tests (#35)
f9b7cad360327c1c4deb25e31e3faa4143d1585d fix output paths in E2E scripts (#38)
d59fa420f89a00846da9b9e9d97eaef69abb8003 Fix E2E tests (#36)
9906ecdabc13ca3b63e9c7c376cbe285b8100ebe Migrate to CRDS and Kube builder (#33)
e522d1e6c27a026dd7bd119924d8c8bfa63e959e Implement Machine Actuator Update (#32)
50fc766fdb6cdb916d04cc54920c6a54e8a474cb  add e2e pipeline (#31)
eae2c3ad9958678566b40398d8e1f6b586c04145 Switch to Azure pipelines (#28)
67de789d5020186368422f434ae848464fb32116 Refactor Azure Clients (#26)
69cc2d532125886dd2678fbe653ce0e7d572980f Pin kube version in startup scripts (#25)
35cdb8144b5964815d925c8ed6f945cd39fbff67 Move VNet Reconciliation to the Cluster Actuator (#22)
005f1a62a5b7f835876ad6841738c9c582a6cfb9 Refactor unit tests and remove integration tests (#23)
666e6d0e75f75148761618b070a3574a298535d7 Implement Machine Actuator Delete (#21)
69098671b12ca3ec71b6d35d68219607bec6cd1c implement cluster actuator delete
e8c57e372c4385c326873475e811eefb95003b05 define default string for network SG
bf01c1b2283decbdc1d0035c59fdf734abe662d2 fix integration tests
40cfc1929269d0cb7f33ed33da23a4bf0e64be9b move resource group creation to the cluster actuator
52a2427b997f3e18249fb0f6919966457ce1c1c0 fix deployment template
2459bdc835fde1bccc225cc79f3a3bc93c8342d8 use concat instead of resourceId to reference NSG in the deployment template
ee31765151329386be965c61728d608667949bde cleanup cluster actuator and more descriptive error messages
74004f1704616a1c5219cf4ae369a3ee1a2696b7 add cluster actuator unit tests
270140ebc8c5911adb3c739621329ec7a791eed3 remove NSG and security rules from the machine deployment template
60e6a4dabfb9b83b69f3d555e3e353f84d072c69 implement cluster reconcile for network security groups
7eca727b583ed150fe835d24bccc7fbca5889fb3 add azure clients for network security groups operations
bab9fab2902fc68ae65ae1d974fe018755d3310c update makefile (#13)
c89cd416ad67b86c9ab4a20f52187fdfa7079aa5 Run gofmt (#5)
57010d198b86050918d619609a1e6485d5197f68 Updated Vendored cluster-api and Provider Configurations (#4)
ad7b0014d1e7591f53ac8565cd392b8c15f94d70 Merge pull request #2 from platform9/make-it-work
4f463fc58e634b6d5fcbc75d590c3fe3ceab6bf1 change to go 1.10.2
dc3bfac826b69c2691d7a358cb73b147f964f5bc specify sshkey is public key, change to use go 1.10.2 in travis, add generation of different machines.yaml
4ee9ad5b8fb4c91064492c0616dba8db55b294f6 remove unusued test until support is added
c827f2a6fb28683b7c9240ebc6d3c5204197ccb3 change test machines to only use one master no node
03b17929aa5bf5f22bfee0da92af1e514450dbd1 fix tests failing to compile in travis due to ignoring key* which untracked a vendored file
91d81b57619dfd8e9597a075877a814eaf408d3f switch go version
1ded36e57ee37cab6522318a0c241589a27f22dd change testing flags to remove unnecessary logging
8ada346681ce72a05e348714aa43ac750d3e1af7 move unit testing out of travis_wait
d829cbb46b962e715a867677243f4aa57124859a disable password authentication on VMs
2a35de89c9ff066d4589475df586ecf7ab5ab547 make kuberouter apply correctly in the startup script
96c47577a1d3fa618706614739ed47eee52352ed use new controller images and add logging for startup script
451efaaeff5886e0497c123d29601ebdb9cd9541 update to support new directory structure
7f20a845685b0e80b999b9ecb701d7f746778652 refactor directory structure
771dddae3cb773fd7d1af425c850ebd207a603ce bootstrap kubernetes on internal cluster but with no dns
279219a7404b1e92d4ddf1f270f369e0ebc955f3 add more tests
414e8c8179ffe3e721fb2656a95675291eaa4e79 run gofmt
612e5c6271f3387596e38b429910e645705e88c6 refactor wrappers to be in their own directory, add more unit tests
caa57e106bf453ea00965d11347d7c8161edbb40 vendor cluster-api
fe03381f4093d8de263d6584998a87406b20a7e4 update readme with valid info on integration testing now that the cycle hack is gone
d89ca0a6a09034571546fe0ffdc15b8ae3f6a494 Remove hack to avoid dependency cycle with cluster-api
8e4f878a04ac278942d2ae5f7cb3b90a98e76c12 host local clusterctl
1b7c1ab975ca58ba0cab332f3c42d4c0c8f68390 improve clarity of why clusterapi is commented
1c9e6292e5b1cc2533d7ab2ab582ab8f73fea7b5 register self with clusterctl as a provider
86fa6dbbc2c40049a7c82d6011423ae5bc78055e add instructions in controller make file for dealing with cyclical dependency
a44c14a2874ab76a96742c967908a1f58eb9af1c add comments to improve clarity
f61a3e3fc85162da7f9ae441c0373076573af801 add more instructions for testing
10878cbf2e016a9ce7480b6f02b048013718e879 add makefile for tests
3a6d659b4718f7e7257414e81cbfafde9505e22a add instructions for creating and pushing controller images to docker hub
81213ed78cea1976022f4cf02f53287ef3bef562 actually call all unit tests
372e3a291933e53d70f38e48e25fc4bd64b68488 add more unit tests
34833c62923cf6c7788556ba697cbad4ea834e02 remove unused file
a6ea77548c0791c867b69fe33846f0d2dd139532 remove commented code and improve clarity of readme
dba0bf1b5db74e44097186dc7e15afc7e91889e6 add ability to parse in machinesetup
696ef94ab126205fcca9a7c080a012fefc716c11 add base64 encode function for use in encoding commands to be used as a startup script for arm
bf5aab21d203e42d6639c2d7b64c8e808b91a61a run a startup script that prints hello world on the vms
b9dd787b1a1c61976f2aa303d95d6e12c4947fc8 fix yaml syntax
af24a9e7a34370a9121039dc382b4a85e41210e8 test parallel integration testing
1be59ba5a770472afa77c46771f62cd6deabf7ff fix typos
0eed4cad6dba9c0f07dafeac07dfeca24da4fb11 add usage instructions
d0cf09d69f5259f22d4b102e0316ac4c0522f617 implement initial generate-yaml.sh
5f959acf4b9cbac193c233ad7bfb4eb91cf77788 initial generate-yaml
5d07cd211ea9f135305f5ad4befacbffdff2293f fix test file paths
eb1693fac4da9c183495c6d81b08a292deb4e51e refactor tests to use seperate rgs
385d11e3a12966ccadd990dd85fc5dec9c2f6f92 remove defers in deployment tests
91f5f834a8bc6480eea9b35e319d9d2339276609 fix everything
e261a8f589d7d4fbdc538d3f6ade861f677462d4 use seperate resource group for ci testing
1bc6374ea5cc047f953efef698d1494d556c3b72 make machine controller work properly
be2032578f67b13af6732cd61885a927e45d5659 fix machine exists when rg has not yet been created
6d2438d17c4f03f696eff2754f13209260cb14b1 remove azure-actuator dependency
a7595ac03e95554fb5e260f923a5526cc7873c44 comment out unfinished test
428590d4c1c1b214cd967dc4c94daa2e48c8fd10 add ability to create docker image for controllers
b4321d08c5ff397caf2ccafc0611d1afccdfa721 initial, non-working commit
00de259367e7b9bcc82d262d54a2e372fc825b77 add ability to delete a specific vm
1c95de9c5b67a6d9029b5a6484c496a8ed7226d2 fix testDelete bug introduced by switching to defer to clean up resources
e9d2fec6b6149f70c58aa9d04d345ca9b2e909ba use defer to clean up created resources in tests
5ae958d0a1dc176fa877665508e5a28b927a5a33 update name getIp uses
31d50a311426b3eae3a5851a23e9c1de56eb80e0 move tests into their own build stages
2b5fef369bf481a5d4d4ec759d62ff20cf833a8b enable waiting for CI tests
cbd4d4aacbe56f978bd2ef0846f64a141ab5544c Merge branch 'master' of github.com:platform9/azure-provider
94823f5d1ab36238b8f1413fe63245e6de73c8c4 run all tests in CI
c3af5206834f8f002ea9b89074b7fe54c5ffcbad parse in environment variables only when necessary
92325fc5ee767a421129f5bc18179b6fd6489ca1 disable test timeout
164b2127705b0f9b957fe22881ba17fc700dc793 Create LICENSE
048fcdd022e9d211956d608f87d85db24e4318d9 authenticate using environment variables
bd06ffcb70a45e9b9b72b743c0ff409283c3b6dc add initial readme
33f9f6857146e525e13495e4050fef92d9948b6e only use go 1.10.x
8d9f21518801bc939d8f0c832586f027b67c93ea add travis slack build notifications
ddf88f7a4b4752ad964b30259b470461acb4a63f add initial travis config
377468a3ed22742414f01058157dbf15fe817c57 remove debug file
d22c42fa99e948c14d295aec0b33c4cfb8e4ea25 add gitignore
290f7d226a7bad2c0a5a4a727a85d138d411fb3b initial commit
```

Status: Fast-forwarded successfully.
