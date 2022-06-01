## Fast foarding of openshift/cluster-api-provider-aws into stolostron-engine/tracking-openshift-cluster-api-provider-aws.

## Status Summary:

release-1.1 -> backplane-2.0: First run, created backplane-2.0.  

### Branch release-1.1 -> backplane-2.0:

New commits (first branch sync):

```
0b2e34680d117b1d8146965f3123c04709d37951 Merge pull request #2957 from sedefsavas/ec2-double-creation
07aa1f0ffa69139ad4ad2771db41fc47a4a08b18 Merge pull request #2933 from sedefsavas/k8s-versionupdate
3f07181239c4b9f1f9f12d92701473e57d28a1ef Merge pull request #2870 from codablock/missing-eks-actions
1f2d104e6119869f76d841599d81fdeb5f7c1d66 Merge pull request #2960 from Ankitasw/non-root-user
3e04cbbe1f43b5c0765abfc217ffdcd46e6573b7 Use non root numeric user for CAPA containers
34da7485a3e2f49b6e6ffb57accab0b3ec54422c Merge pull request #2952 from sedefsavas/ssm-fix
734419dc68e9a9e60cdde55be6dde6d89c6fc8bd Return error if providerID is set and instance cannot be found.
0d254d8cce376b225ee2f6879a29d6c944f56f47 Merge pull request #2934 from sedefsavas/imagedoc
3482facfa1260d93dedc2dc8c8034b2d76f9b716 Merge pull request #2950 from sedefsavas/enable-upgrade-test
a52493fc044bb8faeffb22897018199bd9d414e2 Merge pull request #2956 from Ankitasw/e2e-makefile-fix
cb0a385b53fd75327956834bed126edc67a7daa7 Fix unzip command while running e2e tests locally
d6dac9a52677d3f2119ee863bac3821eb8dc59cc Fix ssm parameter
329f14506ba63c1a87dff3ba654649cac0cae6ed Update e2e Kubernetes version
a971ad4e328600fc85f1766bb4a8f66f5ce3f84c Enable v1alpha3 to v1beta1 upgrade test Enable v1alpha4 to v1beta1 upgrade test
571f447e7f4374eaca75a1dd6c0f2d9c9e8b1f1c Merge pull request #2943 from sbueringer/pr-upgrade-to-latest-capi
84c34b6e437243333c4f5c2b884fc4837da3e20a Upgrade to Go 1.17
4023bd0728981b3b6325de970514de600e6fefa7 run: make generate
91b91d8d441e3dd60a3b50586b5d19967cbea547 Upgrade to latest CAPI, CR v0.11+, k8s.io/ v1.23.0-alpha4, go-logr v1.2.0
c22cc989f0b22423aa03490851d66e10bd61c7a0 Merge pull request #2920 from kubernetes-sigs/dependabot/docker/golang-1.16.10
626ba3b617d432492e419b5ae5594d76a7a83e11 Add custom image generation to the book
aae8297d9e576028f9c7bb378455cac7cc513302 Merge pull request #2914 from richardcase/eks_addons_bug
322f25c28bce7cff4da20504fbe355c7d0807477 Merge pull request #2919 from Ankitasw/gpu-test-fix
a84d651630cfad3ce6ba45b13f22e9ad84abdf1e Merge pull request #2922 from kubernetes-sigs/dependabot/go_modules/github.com/onsi/gomega-1.17.0
438ad786fb41c4a85442622e30dfb6153c236f5a Merge pull request #2923 from Ankitasw/golangci-lint-bump
8803f1257dbd2c7a6bd1261ee39b185a965b2235 Bump hack/tools/golangci-lint and fix lint errors
8d5c79e0bce9f0a45dde5548374c7fe22227fd61 build(deps): bump github.com/onsi/gomega from 1.16.0 to 1.17.0
9ad3da5b9e835a17ae9bf37af2a977193d4e71ba build(deps): bump golang from 1.16.9 to 1.16.10
3120c34732f2033546d7a1a907aa6c631ff9ea3a [e2e] Fix GPU test cuda vector pod creation timeout
10cb56be7f9f4a052d234bfa3ee2c0db8e2225d6 fix: support more than 1 eks addon
af4d75d1c892f029cb2c241d22196bdf57b8e273 Merge pull request #2917 from kinvolk/invidian/test-flavors-small-improvements
c6348771b2d5ba801407fb7a8c332403f2333c7c Merge pull request #2916 from sayantani11/issue2913
62b5584b4eea648b618438fe4ad1143d9384a2ea test/e2e/data/infrastructure-aws/README.md: fix example path
9e07ad9af00f52d7a76d4a53e06c915f4a3d119a hack/gen-test-flavors.sh: call grep only once
f6ffef9dbd2b739858958f9ea46bffe52b2290fa Branch name change from master to main
930bbff11d3388ac948f1393b523fdf3b4e94355 Also add eks:DisassociateIdentityProviderConfig action
0f9f737b578334132cd292395c921694d1d418a0 Merge pull request #2909 from shivi28/update_clusterctl
71c24f7a805523f1efaac6cb1ad8ca1db1960b35 Update clusterctl-settings next version
5861a676166cd7427b53950db502f81a5a27b24d Merge pull request #2889 from vibhorrawat/vibhor/doc/url-correction
851838c7cdd5ed88f37e09a7794c7f266aa0aee6 Merge pull request #2895 from enxebre/docs-externally-manage-infra
8d1f424fd395c9e9243c8bf84be57391a554a48f Merge pull request #2896 from zhengtianbao/fix-nil-map-panic
461ef72c3b647e729298ec5507c3387dabf7b015 Merge pull request #2787 from dlipovetsky/user-defined-elb-name
138bcac6806c13d54154e4a51545177fda7c4dd0 docs: Add control plane classic ELB to existing infrastructure topic
e1977c6080307aa032dd73ca9d24179676286f45 tests: Split load balancer delete tests into TestDeleteAPIServerELB and TestDeleteAWSCloudProviderELBs
f8cb49619241a82d76c1ff80eb30a2ff830b04fd chore: Rename  deleteClusterAWSProviderELBs to  deleteAWSCloudProviderELBs
42c20280a467ff35e353091347f9d83ecc19e4be chore: Rename listOwnedELBs to listAWSCloudProviderOwnedELBs
fcfc348bb815ab7d017cf7e54d8aca62cdc238ae refactor: Populate ELB Tags in describeAPIServerClassicELB function
c2f435737293e6ecb284e98f78ee942bec794f2a chore: Remove unused RegisterInstanceWithClassicELB function
e6c6c88bb382170bb13b4dd49d2f8186e15b76c1 feat: Skip reconciliation and deletion of unmanaged ELB
1eb92933d2ab39941d6dc70dfb4341c4b5e22027 feat: Add Name field to AWSCluster.Spec.ControlPlaneLoadBalancer
d2c1932d2740c369f980afb718dabbf06bfeebd5 Merge pull request #2900 from shivi28/replace_ioutil
aab07ec84e6406f5883bff3ef94ba198229310f2 Replace ioutil with os/io packages
890063a841cf6abbaf8bb6f4e4218d9b902ad475 Merge pull request #2897 from Ankitasw/kubetest-v1beta1
85dca27119ebe228937902d8ba8a6ea73ea36bbe Bump CAPI version to take the fix for periodic conformance tests
b9e293ba9d4217cb5c4bff799e073ca97c68a96c Merge pull request #2892 from PushkarJ/build-deps-remove-indirect
3e64a8a2933b7884c6c8800040376c8a228ac157 Merge pull request #2873 from shivi28/az_add
3ace8cd9e1ea72f667e9da2aa2837a1a24fa3f8f AvailabilityZone variable added in template
a0ba2c5879ca35e4ee42aa19005bf4bd13aeb0b6 Fix createLabelUpdate panic in nil map
1527364c81ec82a3f6ec1bea5f3cd885a030c795 Remove indirect deps
f575759c3da3dd23ceeb0e381d9adaebd0586031 Add externally managed infrastructure docs
58584daced7d8e4f021b913c1c6b5672710ad6eb Correct URL for Flavor(s) in Machine Pool topic
09afe190c1f4d3f844dff6c6c402db4aa9daa84f Merge pull request #2885 from zhengtianbao/ControllerIdentity-update-nil-check
116ece8912083ea64b1e0f50750ed381cd197434 Fix AWSClusterControllerIdentity ValidateUpdate panic when AllowedNamespaces is nil
2d89e9ef6f405630b059f8cfc342c6b8e8b14cee Allow control plane ELB to use different subnets from the node subnets (#2877)
b059d92aa230bc2264d06243c6da92a475d26911 Merge pull request #2878 from sedefsavas/fix-panic-eks
b8eab9f91ed940b481692cadc47512ab906b4cb3 Add missing permissions for EKS OIDC provider configuration
986262a0bac2448116779f237a3615f7a367e864 Merge pull request #2874 from kubernetes-sigs/dependabot/go_modules/hack/tools/github.com/onsi/ginkgo-1.16.5
47748b47a8e89fd3c54aca93ff9228ef0e75d8ae Unsurface error when getting the remote client
e6ae8d02723fa0bdb8d39a00f542365d66bf37e0 build(deps): bump github.com/onsi/ginkgo in /hack/tools
0dcb6574f0fef1c1de324e5c324238c0792772a1 Merge pull request #2867 from ameukam/use-k8s-infra-gcb-docker-gcloud
9957249adc1a65151c039ee59c2199710d3c8f9c use k8s-staging-test-infra/gcb-docker-gcloud
d41f8cc91c992585fa4e1e0d693d408c89dbfb1d Merge pull request #2790 from Madhur97/aws2189
26589e22fd6b57d0946a14f6535069858ef3ed9b Merge pull request #2850 from codablock/fix-eks-additional-nodes-sg
4d49b3a3016895f51e5c377018a3ba28d0e80af3 Adding optional IAM policy creation for EKS Console
177c83e440527ed0070e38127d9970755f000a4c Refactor SG service to always require explicit SG roles
7c7ebfe7e2256a092caa8df1481a838feee35836 Merge pull request #2860 from sedefsavas/e2e-upgrade-test-fix
1760956f5d76b7f6bafd1f48e8d0b76611c9426d Use s.roles instead of defaultRoles in describeSecurityGroupOverridesByID
d224550a56ca91727b435fd197ec37919181e8b1 Push e2e images to AWS registry for upgrade test
e0923d633b300f86b064ecd606e4ac14b285018c Merge pull request #2843 from Ankitasw/gpu
c5a79102f7c0a5f6782123958f1af96119e328bf Add GPU e2e test
bc5d8cc996d2b047a7661b25d73acbb18ed31e20 Merge pull request #2851 from kubernetes-sigs/dependabot/go_modules/github.com/aws/amazon-vpc-cni-k8s-1.9.3
1c6d0facba36e96fb38e5fdfa3dedc9e982ed0ba Merge pull request #2846 from richardcase/fix_eks_max_sync
0ab6eff6862005849f84ef31053be51b79871e62 Merge pull request #2837 from scottslowe/issue-2836
3aa294d63bf36368df58b7cda168dfc2a099bb09 Remove e2e test references
8a58fa7118aae90d4773debd8752e6a10240518c build(deps): bump github.com/aws/amazon-vpc-cni-k8s from 1.9.1 to 1.9.3
8cecefca2c830fdcebbf8dcf0934e9be57fc6abf fix: added may resync check for EKS
bab7f7ebd1c6bb02bf934185aba76f765aa8cf6f Merge pull request #2842 from kubernetes-sigs/dependabot/go_modules/github.com/onsi/ginkgo-1.16.5
c7f85e8105489a3a04f6c4b04be94a2c05e7ca96 Merge pull request #2839 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/klog/v2-2.20.0
91bba6a73fb5704a7a3c56e6f0073ee8961eb880 Merge pull request #2838 from kubernetes-sigs/dependabot/docker/golang-1.16.9
3a2358f5aecfde215ac6e970b8c200e316a67a0d Merge pull request #2841 from Jacobious52/main
bc9f6b767ca0db4131a878e1fd63bfc93c8eff18 build(deps): bump github.com/onsi/ginkgo from 1.16.4 to 1.16.5
6b8744f1e3ec66cb88f556007ba78d96cf833613 fix create-cloudformation-stack command
8db37bf422e8d45574f11ef68c489e025eba0ffc build(deps): bump k8s.io/klog/v2 from 2.10.0 to 2.20.0 in /hack/tools
3bc64ff98b92d706fe5b4c2199809af3927b2838 build(deps): bump golang from 1.16.8 to 1.16.9
ac4f0fa5c57cb3a62547c460bd442af83df50349 Fix documentation on external AWS CCM and AWS EBS CSI
0fb108ac19f544a33a7c31a5278f212fbb88ccc5 Merge pull request #2830 from randomvariable/readme-v1beta1
82f3c98f2956d27f3713ef76a25772fd17f254ac Merge pull request #2833 from randomvariable/e2e-upgrade-test
cc00bcced531f44f4e4dc9288b4955b19a2ee5da Disable upgrade from v1alpha3 to v1beta1 test
f3aa975a0e96c539865487cdcffbd6fc07579c22 Minor log fix
676e981bdd420ee5712d4f16c50d25286c1deade Enable clusterctl self-hosted and upgrade tests
1d97ec3d45ef77a5689e098f3e5ea179b0f57c7e Merge pull request #2831 from randomvariable/capi-v1.0.0
1c8f8b962cbe28e610c0256fcbb280c65ae8e70a Update to Cluster API v1.0.0
d5ac5f14ac4fa3165a254b95dc784e1992052dfb Merge pull request #2832 from sedefsavas/internetfacing-beta1
a4618b8d7bae4cca74bbf33fd095c51f782bf5de Fix for internet-facing ELB scheme
5e9760e19fcd77faca711ff6b4e41f56e3cf1979 Update docs to v1beta1
1a61dfc39649749b8b8dfad8334909a388d675a7 Merge pull request #2820 from randomvariable/v1-update-attempt-2
4274a5ab5c9dc391045840d6e45e17fe0cbab3dc Update to v1beta1 * Graduate CRDs to v1beta1 * IAM types moved to /iam/api/v1beta1 * Graduate clusterawsadm configuration types to v1beta1 * Add conversions for v1alpha3 & v1alpha4 --> v1beta1 CRDs * Add conversion for clusterawsadm configuration from v1alpha1 to v1beta1 * Improve error handling for clusterawsadm when incorrect configuration is passed * Add defaulter-gen to all types * Split up /api/**/conversion.go into ones for separate types * Controllers will now recover from panics, allowing webhooks to continue running * Remove kustomize generated e2e test flavors and add to Makefile targets * Ensure CRD docs generation actually occurs * Rudimentary build caching for API go files * conversion-gen was forked into hack/tools/third_party to remove incorrect duplicate static function warnings * API packages given consistent naming and set throughout the codebase. golangci-lint configuration updated to match
bbaeb11e95a1c362e2ee905526eb1b8be23b86aa Merge pull request #2822 from enxebre/leader-election-resource-lock
2b09536ef7fb3806af97169437a28c808c970971 Merge pull request #2821 from enxebre/check-nil-deref
d9cefd4fafbc409242522443268bab8b6865ad31 Default LeaderElectionResourceLock to leases
baad872f5588877b9966ca026085200cf3d4ebdd Add check for invalid memory address or nil pointer dereference
048a58baca07c56650e5bc2978dea975fe3c4298 Merge pull request #2813 from pydctw/fix-security-groups
8d9eda4bd9885a95b5537033138186a6a63f2060 Merge pull request #2755 from richardcase/go117
8fa95d05438d8d73a1e678bdd223887b5e3e30f3 Merge pull request #2751 from spectrocloud/nodegroup-role-additional-policies
b2ed789aa803401cbbcadd07cf9ecead97ffc52c Merge pull request #2785 from Ankitasw/bump-cr-version
42eafcd4ff1e4a294620dddb77b098acc460f4ca Fix ingressRulesFromSDKType function
9673b368f6af1f7718069de0f5162d6f36fed69b Add tests for securitygroup Difference function
d2f76e1416dd1b840d1e5ec34b754974e900f2f5 Merge pull request #2811 from randomvariable/crd-docs-in-generate
38daadfa6b9b65ae367b5e7f1ba8a09021a0e3ac Move generation of CRD docs to the repo to speed up Netlify
ba219ddae9bd2b79b5572835d2fef8f71e84f1b0 bump controller runtime version for v1beta1
f629821290df8977a5af3c886b27bab794bad02b Merge pull request #2810 from dlipovetsky/testenv-build-segfault
d61e9d450a8ec0688bb89943b3342600b8588fb9 EKS: support role additional policies for AWSManagedMachinePool
ca769c37bd0d4db6fec4a0eee85a566ead902630 Refactor duplicate codes
28bbc79220baaed1a8b2e161b998dc94deac4714 bug: If one type of webhook is not defined, testenv.Build hits a nil dereference
3949f5376410f694defdf0ffb257a27835d7f9e5 Merge pull request #2808 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-lambda-go-1.27.0
c8575a2591c6b20165d39d4d18bd8dd88c76cda3 Merge pull request #2659 from spectrocloud/nodegroup-sg-fix
1907d00a588bdd459ce13daa258ea26bf8ed72f0 Merge pull request #2800 from voor/patch-1
01d5ec5140bc110f4bf14f39c76314f5718c1c7c Merge pull request #2809 from dlipovetsky/fix-v1alpha3-restore-pointers
db2540b1fb01fd3b829502de356580e113227c14 Merge pull request #2806 from pydctw/update-tilt-provider
4841b21f793b36db18452000be9a40a503cf3265 Ensure destination pointer is non-nil before calling restore functions
8697db2bcc1171a14d3fadca3009af874ba7d537 build(deps): bump github.com/aws/aws-lambda-go from 1.26.0 to 1.27.0
6cedecd331c0e4429b98eecef64dc060b932b143 Update tilt-provider.json to add CAPA label in Tilt
e5cf5070ab6f08bd4651b7b56f81c6e45d04bda5 Update manager_iam_patch.yaml
06e02b2d242d0496d0b0855d00d88b7f51b7e277 Merge pull request #2796 from Ankitasw/e2e-fix
f70429e64c11dc281b8f8b712d3c0259925d7049 Download the restart scripts outside the dockerfile
f3f5acf0cecec2437922e7eb9030656713dfb836 Merge pull request #2789 from dlipovetsky/remove-duplicate-conversion-code
4effe9484a367b3dd8aaf10aeadd330cea1419ff chore: Remove unnecessary conversion code
e2d9dc702ed12f02cf619a7d6f4fcacbe0d57223 Merge pull request #2740 from shivi28/aws_2686
4b7955d5d41b15d9c1610815f22b373571eb226c Merge pull request #2772 from pydctw/awsmachine-publicip
66e83583313c57fe4f634f011721e632b5218389 :bug: fix typo in AWSCluster validation hook error
fd7b0449b8cbf8ebfb71cb6fde7af80c6a94a543 Merge pull request #2786 from spiffxp/sig-k8s-infra
25710947fd8235f057924b9beeb8ad016bb176dd docs: mv wg-k8s-infra sig-k8s-infra
5aca29c9645a670fd32f1968f9ad799c07a3932f Make PublicIP field in AWSMachine Spec work
151fb40cbaa2d87d846f4a0f620c2dbf8b440283 Merge pull request #2777 from Ankitasw/multitenancy-fix
50830fe326c89a51780a8e07033bcd223e9323e2 Fix timeout due to delay in bringing up control plane in e2e tests
5dbd9d0bb7a6a017512b5e82ae7cd55465fffc91 Merge pull request #2773 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/release-0.11.0
415ff3b3eb4367f44e343e191b3aee1216f7266c Merge pull request #2769 from kubernetes-sigs/dependabot/go_modules/github.com/aws/amazon-vpc-cni-k8s-1.9.1
1035591b9e60d32c27ea7dca2f75083d449c0c1d Merge pull request #2770 from Ankitasw/upgrade-test
dee3f14eed39f62ca473ad5b6c03a8f6eeb49f7d Merge pull request #2766 from Ankitasw/log-flooding-fix
fabf231b87262fef79295d9a23d4a8e7a865a6a4 Merge pull request #2768 from dlipovetsky/fix-elb-scheme-name
4e0c2fdc3ba7c563d2c74ac6dd5758f71ddcbf3f build(deps): bump k8s.io/release from 0.9.0 to 0.11.0 in /hack/tools
38f27da985d3d1d272ebe92daff35b515f6fb122 Add v1alpha3 to v1alpha4 upgrade e2e test
57aabc28d849f6acd9a4582372b745257376e8d2 build(deps): bump github.com/aws/amazon-vpc-cni-k8s from 1.9.0 to 1.9.1
51cd1b3ee0cd4c1e70df19d514805e6e923aea9a Rename the ELB scheme from Internet-facing to internet-facing
214d5a8a0a6d165453eb18bf53ca94930f342bbd Fix the timeout for conformance test
66626bdd0b32f3d8371526ce897256a3bea989ee Merge pull request #2760 from kubernetes-sigs/dependabot/go_modules/hack/tools/github.com/golangci/golangci-lint-1.42.1
4937d1c6e6967662c2caca7ac374b69b478c1839 Merge pull request #2759 from kubernetes-sigs/dependabot/docker/golang-1.16.8
e6e5f920258b8fb391f62f2c5486915cdfdf11f1 Merge pull request #2756 from richardcase/devdocupdate
fb041dd809707f8804703cb8f4b7126a71838da7 Merge pull request #2715 from pydctw/tags-on-existing-infra
7f92a25c4b4bd0ecf926e3279442594cedd46b1a build(deps): bump golang from 1.16.7 to 1.16.8
7c994b213beca6b522503ae5d9305fa0e53180ea Use same golang version everywhere
a7040f4490d5922ea668362db1f596dba1323124 build(deps): bump github.com/golangci/golangci-lint in /hack/tools
5bcbd78c101971f962d7ddb90f77668804ca15c0 Kubebuilder required validation added for InstanceType field
6dbf6d570cb9bdd22048cec35ca15394eb71c3b9 docs: update to contributing to reference developer guide in book
d1a3280fc8742ed0e89c69b08d59e5c8b81be49d chore: updated verify to support go 1.17 build contraints
c1f17e0ee15ac002502fe749a679797e45b2e46d Merge pull request #2739 from kubernetes-sigs/dependabot/go_modules/sigs.k8s.io/controller-runtime-0.9.7
b7e0c11096a53c00fc7490251071c9c77c629b11 Merge pull request #2737 from kubernetes-sigs/dependabot/go_modules/hack/tools/github.com/itchyny/gojq-0.12.5
5c977ae7fd64cfb771202b1c1bfa24bc45bb6aea Merge pull request #2745 from Ankitasw/gomega-fix
21350b18aacaeeaba672df8405d55883ab909929 Fix the gomega errors in tests with the gomega version bump
e9480762c7cdc45f200bc9d65756f37a01b9a37a Merge pull request #2728 from pydctw/fix-findSubnet-logic
8bcdeadf83349d8f586e9a5275dcf8a7296db2c7 Merge pull request #2742 from mkumatag/fix_broken_link
253d15f93cbfa9573e747fe5c45157b61a3046f7 Fix the broken link in the doc
64dae2f2eab632165d48313e9052d32b77c69c6e Fix findSubnet function's logic when subnet ID is specified
b493d497d0048e04f6d9eb6866cd7de5f829b9d9 build(deps): bump sigs.k8s.io/controller-runtime from 0.9.6 to 0.9.7
dbbce68e1596cce76c54129044c395bce46e7e14 build(deps): bump github.com/itchyny/gojq in /hack/tools
4a14a37be7caf0b9239a59431d0a73fafece23e3 Merge pull request #2731 from Ankitasw/external-cpi-doc
588aaa67512af9b343fdfefbb8ca8bd84cb94ac7 fix: doc formatting
c43ff1aa0bc5725445c3ef6f2a00c9e981052f81 Merge pull request #2724 from Ankitasw/external-cpi-doc
7a2510e705bcf1fc2e5d3d1c629302ebf6eedd38 fix: add the new doc for using external CMM with CSI driver to summary
8e95619c741929b5fe11a7b22efbfd7553f6dafa Merge pull request #2718 from Ankitasw/external-cpi-doc
f125b764f9c73e52fee2e6cc756b5c1f382ede45 Add AWS cloud provider tags to pre-existing(unmanaged) infrastructure
08992011ac828f852e5578916d1030534f3b562f Add doc for using external cloud provider with CSI driver
762e320e9dbe208672df195bb9c3b1222c0d24da Merge pull request #2723 from Ankitasw/ccm-affinity
7922fcf4faa68b0368725d69e77f1e83693b532f fix: node affinity rules indentation in external CCM CRDs
8c54bea4db8bfd805a705abbb0659fd1c68f16bb Merge pull request #2722 from Ankitasw/ccm-affinity
b606805863a68ffe56b715ff66b151c685cc2261 Merge pull request #2721 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.40.33
4db9673d6f136512563cc6d6bd002d490c59d3f0 Merge pull request #2719 from kubernetes-sigs/dependabot/go_modules/hack/tools/sigs.k8s.io/kustomize/kustomize/v4-4.3.0
c0d91b09fe7454d15ac072029dd6d81f11636e49 Merge pull request #2705 from muxinc/dilyevsky/fix-route-pl-dst-panic
171a52fb899ca9188f3e57bc23a18877fa05f3f6 fix: node affinity rules in external CCM CRDs
0067ad35f861282c4f1f9899b141d36c465158d3 Merge pull request #2720 from sayantani11/issue2710
e0f29e46ec576ea94cbd9c20a0bb1298b9d5cd96 build(deps): bump github.com/aws/aws-sdk-go from 1.40.28 to 1.40.33
7777a6b98bbe0a99f6658a66a6bcb8018bab5242 Changes which were missing for v1alpha4
469328ec31190e7a75119676416cdc701fcaced1 build(deps): bump sigs.k8s.io/kustomize/kustomize/v4 in /hack/tools
3c209f1ad2c075df87099ca981fa38585086c7bb Merge pull request #2667 from richardcase/owners_changes
da4221bd7e3146fa6a2e5f995c4802be94b9269c Update CAPA reviewers and maintainers
98c21e56f9eddb1c5ba41de379d0c808ce6ffa08 Merge pull request #2716 from vincepri/vincepri/emeritus
ebe0d5665206120dbbb13b0bf9abe5a8d4216c01 Move vincepri to emeritus status
8b518a064076f9713a0249f586a7d1f4953096c6 Merge pull request #2713 from richardcase/scaling_config
26e8f680b7741ddfc9fb3ad55de3f844d95b1e72 fix: ondemand immutable field and missing scaling config
1a7e43a6683d88aab3a6cf43366aaee6af7bb5ff Merge pull request #2647 from Ankitasw/ccm-with-csi
0597de7b6913ad65c99ce991c70ff2a04e2efeed External CCM e2e test with CSI
b421c0a9a21632cd3d9455c3f7902d30601d9528 [cloud/network] Fix panic on RouteTables reconcile.
ab7402765629e674ce35f0203985b9f88eaafeee Merge pull request #2707 from kubernetes-sigs/dependabot/go_modules/sigs.k8s.io/cluster-api-0.4.2
437c3f9f9e767545d9552a568b1f52659f84f70b build(deps): bump sigs.k8s.io/cluster-api from 0.4.1 to 0.4.2
c5cc835cfdd5165cd8f5ec3dbd17305c9a7a993d Merge pull request #2706 from kubernetes-sigs/dependabot/go_modules/sigs.k8s.io/cluster-api/test-0.4.2
a4f7010e962e8508ed70910bf96f71b28c83ad6b Merge pull request #2685 from geetikabatra/webhook
ffa71a6c024c02d6def4633dc5f20aa2dce97529 Merge pull request #2702 from spectrocloud/eks-spot-capacity-type
802489996e93401f8c601a0ba0becd2afc6ef5a8 build(deps): bump sigs.k8s.io/cluster-api/test from 0.4.1 to 0.4.2
77c0d36e61281d553f116edf75b90c274b6dcecf support spot capacity type for ManagedMachinePool
e0b853654a841a4256aa2e720782c73ad821c933 Merge pull request #2703 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.40.28
5eb1a6772cc9452ae6f443cc16c373eb8b36ba88 Merge pull request #2695 from kubernetes-sigs/dependabot/go_modules/hack/tools/github.com/golangci/golangci-lint-1.42.0
0c36d9921dc63c33c32af9362f763ccabf7fea61 build(deps): bump github.com/aws/aws-sdk-go from 1.40.24 to 1.40.28
991031abcbe87683f6d96098ab169ff699160a89 Merge pull request #2676 from spectrocloud/fargate-profile-tags
c6dfb7a37efde860fbad35f9d1995d9f22762f00 Wait for webhook readiness and healthy
9c2e02825d006d997c1e2b762ebac2f3555a6a67 Merge pull request #2662 from kinvolk/johananl/compact-iam-policies
6ae509dff0128bc7cadee83a7a4ad911647210d8 Update README  - Add godoc reference card  - Images aligned to center
1e881159b8c30b949fb5b6dad5836ebd7bd2c1ef Merge pull request #2682 from randomvariable/netlify-fixes
9e891e5299ecfb9ed2827e5862c784772df377ee Merge pull request #2692 from rayandas/rayan-fix
2f3b6096a7eb6bcd1f753416f678f575524ac2ee build(deps): bump github.com/golangci/golangci-lint in /hack/tools
d7e641eace16162dec318a735c40748c36de0e20 Removed elasticloadbalancing:AddTags duplicate entries.
465f80457ac46d38a94319c2684eb93045ceb162 reconcile fargate profile tags
86adc8cd6fc48ed99fa719e640d44a6f9078d1a4 Merge pull request #2681 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.40.24
7cbfe52e53e109c3fa5c7515112f12a56a622347 fix broken link in docs
25ac6a84bd48c0b526af5a5497753b90b49546f6 retry fetching managed vpc attributes when vpc is 'NotFound'
a072304d97243b8a7433653ac3205c646b272f8e netlify: Attempt to resolve build speed issues
e88f174bdcacb4aa1ee6b39d18860792cf3d8975 build(deps): bump github.com/aws/aws-sdk-go from 1.40.22 to 1.40.24
327e9b8a0a81d05ede3a9f61c30fef2947fa05ef Merge pull request #2677 from randomvariable/metadata-fix
8982b301e4b7c2aebfa97ea8b05cb8a49c046b9b Merge pull request #2673 from Ankitasw/e2e-logging
784291615fd89cb662a49df0ff62d01304f57899 metadata.yaml: Correct version
aa68f949dc496116155c73fd61ea5760f493f6cb Merge pull request #2671 from randomvariable/august-2021-updates
e658991674362266b233e7cef786be7f6186155e Add log-level4 logging in artifact logs in E2E runs
d3f0ff1da44e1819e11c69348b32237b4860f280 August 2021 Dependency Updates
c13de5c2b8f633bcdb3e04ebb044c649caedb182 Separate EKS-related resources
e7d56364b37620241546835b67332ecf6be275bf Merge pull request #2648 from richardcase/graduate_eks
5c2c08aa4bc3037afa395c4567547d5e6a385568 Merge pull request #2661 from kubernetes-sigs/dependabot/go_modules/sigs.k8s.io/controller-runtime-0.9.6
ecec21044a6236eccc52046e009b3eb312f4a714 feat: graduate eks
f1a4dc034a529a9aaa7d07c01c1332a3e1226dbf Merge pull request #2422 from spectrocloud/2248-attach-oidc-provider
dd955b262c70147911ecb7d513d1b86e0fa2c81c Bump sigs.k8s.io/controller-runtime from 0.9.5 to 0.9.6
8bdb30fcec9dcdae26604c2252d48231feb4e4b4 add bastion-sg to remoteAccess source-sgs when bastion is enabled
528de47989054753576da33dcedfab9e7c8dfbf2 Merge pull request #2468 from cnmcavoy/cnmcavoy/volume-throughput
d411aabaeb7cd1732dded820e6b9d49d6977c728 Merge pull request #2649 from kubernetes-sigs/dependabot/docker/golang-1.16.7
0975d2087ee6989f0108090a3ec0931b9a6fa4a4 Bump golang from 1.16.6 to 1.16.7
9780ac55832b2c788098382116dcd4ad7ec4163c initial work add plan for identity provider
e69740275ca5a14b51eeca3ed74cff2d88dd8cdc Merge pull request #2629 from sedefsavas/reverthealthz
9df2a870902f5dd8c82e3abee5b662520c0ab39a Revert healthz changes
4259d838c29ba73f96d3f99a336908869a919c7c Merge pull request #2628 from richardcase/fix_scheduler_eks
1edf06f85db709da4c367134d44f87541d976c67 fix: changed the node affinity for the managers
362885f99be9e0d2e9ebbf72c645561bcea7a869 Merge pull request #2626 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.40.11
0463aea7cdfff8d0b8140470c532a921f34ee922 Merge pull request #2625 from richardcase/fix_scheduler
f5ea618090b74d65ae0352b40a5e9e3cd72a2561 Bump github.com/aws/aws-sdk-go from 1.40.9 to 1.40.11
092f06fe77ffe1a2beb1b3f9783e4d5b7fdb5bec feat: node affinity definitions incorrect
7f4ff45f262e66849b8e85ebfa22591fd362e92e Merge pull request #2601 from shivi28/aws_2270
4ad04d1fd2f9af4009377698583aaeab854d4498 Merge pull request #2618 from kubernetes-sigs/dependabot/go_modules/sigs.k8s.io/controller-runtime-0.9.5
64e8cfb04a64b73d2e38b6baa28428b67f4641a0 Bump sigs.k8s.io/controller-runtime from 0.9.3 to 0.9.5
0792c9704d6456de2a141ca653fc097a15c7aa12 Merge pull request #2615 from kubernetes-sigs/dependabot/go_modules/k8s.io/klog/v2-2.10.0
a4db1be2699609812874df9759f7b017c6c91984 Bump k8s.io/klog/v2 from 2.9.0 to 2.10.0
f19c125c4fa323c12427f060a86db29a887350bf Merge pull request #2617 from kubernetes-sigs/dependabot/go_modules/k8s.io/cli-runtime-0.21.3
672acaa9ffffdec1cd8653d6d322cf2735a29aed Merge pull request #2614 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.40.9
4035188360ad8fbb3f98842eb59fb08776d3dce5 Bump k8s.io/cli-runtime from 0.21.2 to 0.21.3
1bcb57cabc0b8afc1d0a22c3bf216936493fb656 Merge pull request #2612 from kubernetes-sigs/dependabot/go_modules/k8s.io/apiextensions-apiserver-0.21.3
39dcaf56408543b12add769d36d6b64b9acfbe98 Merge pull request #2377 from vespian/prozlach/control-plane-affinity
54f8c8902dacbc0a644ebae8cd06a641f35f301b Bump github.com/aws/aws-sdk-go from 1.40.6 to 1.40.9
deadca189f451c59dcd4602ac9ffefb6c8411625 Merge pull request #2616 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-lambda-go-1.25.0
7e19b857af94ca95abafb97f021d50598f1a8ec9 Bump k8s.io/apiextensions-apiserver from 0.21.2 to 0.21.3
476086c4689ebe54bbd79aa2bec3e2b4ec480d60 Bump github.com/aws/aws-lambda-go from 1.24.0 to 1.25.0
ba5a703819ffd58df21ff36905aa4ca55d74eca4 Merge pull request #2611 from kubernetes-sigs/dependabot/go_modules/k8s.io/client-go-0.21.3
6a6aaf2e9859d07b621cb3894d44a05e90892327 Bump k8s.io/client-go from 0.21.2 to 0.21.3
a0bf7cb64ef2da1ecd6db8c6a1976319f30692eb Merge pull request #2607 from kubernetes-sigs/dependabot/go_modules/github.com/aws/amazon-vpc-cni-k8s-1.9.0
0185272531c82a23e3597e8f0120efbaac5ae218 Finalizers added after first read operation on AWS in AWSMachines
7cfe801e51dd8fb0bdbc81f2f02d1bb24caa1ecb Merge pull request #2600 from shivi28/aws_2263
7b53e17b7d5c58fedfde78e280cba9f766e51c81 Bump github.com/aws/amazon-vpc-cni-k8s from 1.8.0 to 1.9.0
91dfb7f8bc786f80190466964cb705d93c0f8922 Merge pull request #2605 from sedefsavas/releasefixes
9f0319fc5f5208cb249fb7256fe8f349f58e84b5 Parallelize NAT gateway deletion
52b5912ebcd303f8616af113379a3b0f70b6ec0c Remove removed source field in docker volume commands.
d8f5987b685e328a43812d3540919cffc57a7702 Use production registry in the published manifests
947ad1ed65128865b652ce92ce15ebc64bc1a079 Set branch to main for release-notes
d44e4a4c8c19cc3562e58ba578b80c43432d6306 Merge pull request #2603 from sedefsavas/webhook-health
4fc730a3bbe0acf6b3e375a35f129401762b6a99 Add webhook health check
eb9f27511a9a318ac7b69a8493643bf2901e437b Add ebs throughput field to v1alpha4 Volume
49e537efd9cfd2befeeb69de70dd8f3691a1f0ba Merge pull request #2599 from randomvariable/eks-reconciler-fixup-2
1af5eec5b5df9add5244631eae6b48e36dfb4907 eksconfig_controller_reconciler_test: Eventually test for updated secret
841195d7c3ab84a76df5fb7d2e2812b2787e72d3 Merge pull request #2571 from Ankitasw/api-change
1c529d4fdc954fc74de877cbf5452f7016acafbf Merge pull request #2556 from shivi28/volume_bool
55df68a6f34fcf0c01ffc08c02d077bf2e337fee renaming spec.networkSpec to spec.network
69246ee537266e18ea48e131b9aba40894f96290 Merge pull request #2596 from randomvariable/test-fixups
5fdf654d75932eee61490a2c7a6aabb9392e2ce4 make control plane tolerations configurable, change to preferredDuringSchedulingIgnoredDuringExecution
03a9008c0017bf64db761b2af573fd8607475603 bug: make sure that controllers run on controll plane nodes
262ea265485be9aaf58d2a3e46f33da6f30d888a Volume encrypted to pointer for v1alpha4
5b0b820bd7aee327f71fb06a29beffd0b34ce06f eksconfig: Refactor tests to avoid race conditions
33c9ef97f852bf9b0866977911184e4e0f651ba5 Merge pull request #2585 from ykakarap/awsclustertemplate
11e824649230b31f68e0442e5e520ada0ac7e4e0 Merge pull request #2549 from shivi28/aws_2275
8c0d921e8596861a5a774098b2eb0e9b79dbfe0d Merge pull request #2593 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/code-generator-0.21.3
68592bb4f5013f3689a09c8cffec0158ee1889d5 Bump k8s.io/code-generator from 0.21.2 to 0.21.3 in /hack/tools
d8ac4dab380a8eacb7bc51cac6fa9bdf088380d5 Merge pull request #2592 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/apimachinery-0.21.3
9d2cc047d14567ec4a59f253100236227f996228 Merge pull request #2591 from kubernetes-sigs/dependabot/docker/golang-1.16.6
01f433dab26ab51c469060eff129e7bd9cdd9c61 Merge pull request #2579 from newrelic-forks/rtorrents/fix_secret_reconcile
daf59aba4f8918696c9d9913e9440c147ded14b3 Bump k8s.io/apimachinery from 0.21.2 to 0.21.3 in /hack/tools
1ceb80e48a24ca2923039f2e29492507bd439c28 Bump golang from 1.16.5 to 1.16.6
1956af1cb5fbfaf8469c5c215181e6acf5551f69 Enabled GPU optimised AMIs for EKS Removed unused field like ARN and Filters from AMIReference
f192929513bbe39f61899e022ac3907f17004e33 Merge pull request #2587 from randomvariable/reconcileVPC
fea802e973f0ccbc185cd34134eec2a5bda4d33f Cleanup ReconcileVPC() and set id early in reconciliation.
51164fb320e65058b6cc74371c0fb622167c5577 add AWSClusterTemplate type
d38fda2ecb7ba7a463628d882793231b03493f46 Merge pull request #2583 from randomvariable/conformance-fixup-july-2021
880cb2549efeea5ee4d7c008a34b764f22f67cc7 e2e: Pull in newer Cluster API for conformance fixes
69fababdf35d766f65241e8db452102524f72d5e Merge pull request #2572 from randomvariable/e2e-cleanup
d3a7c65106b78168955d03516167d044e0ab793e  Major E2E Cleanup
e32c8346ae6aeed11b1bd42c42064a574fafb4de test: check resulting userdata Secret is correct
2ab4bbfcdb716795ad07a6d9c6fd3c4a5b6d4d35 fix: reconcile Secret when userdata changes
1a29aec7bb94d44a38e2df6a398a681b2ec06d34 Merge pull request #2576 from richardcase/e2e_test_changes
9739acd9cecc233a53a142089a20d5b892c21462 fix: ensure subnets are updated
fc7ae25c0e6d5334f137fcd2c18c3579b77b1f58 Merge pull request #2573 from randomvariable/july-2021-updates
633d07165ed57196797100ece80fee48e0c5421a July 2021 Dependency Updates
289117d1e5a57028d3c17f1184e16754f1367f6d Merge pull request #2505 from Ankitasw/encryption-config
1ea61aa5732d2d0b130ade6d57c114ec2d33f04a Merge pull request #2555 from sedefsavas/sg-fix
4ba309ae842a044a1453ee46809df14a62ed9eda Merge pull request #2567 from kubernetes-sigs/dependabot/go_modules/hack/tools/sigs.k8s.io/kustomize/kustomize/v4-4.2.0
796b3e7ff84f6c78e6db595e17ab3bcd61204976 Merge pull request #2565 from praveenghuge/2554-doc-change
d48f5e556ddb05765fb8a8832348b43ca8117105 Bump sigs.k8s.io/kustomize/kustomize/v4 in /hack/tools
941ea3b799434433774c7a2ac35acccefa954120 fix: replace DeepEqual usage with slice cmp pkg
5273444babd5fc5e880715946dced52a65f3932f Update EKS clusters to enable encryption
0cc0d1f1e74f9c42aac0c051ef0ca8705d8c6de5 update clusterctl config with new capz change clusterctl generate
798bbc98c37f583e94b70027bd49202caaf62713 Merge pull request #2562 from sedefsavas/prblocking
cd054aceee43090ba839138b9711dcb3216da2cc Only leave one HA cluster CAPI test
fcfca6ceea4e114a83d4dfc84ca49223fb039d1a Move quick test to a new file
5bae6cc7b1107f82f70ffc84ac73704a0bdebf0e Makefile fix for pr blocking e2e test
7126bf6fd1a2753c61c1e2833ddacb74f6de1caa Do not delete overriden security groups
671152a05378c50e19e26a5f0751a7dfe821545b Merge pull request #2559 from praveenghuge/awsmngpoolrole
47a4f1af28257aa378e6014b31853db22a2eb337 Merge pull request #2558 from praveenghuge/clean-up-master
81268592eba6165a735b87b3ab48763fd7008d79 add 64 length for awsmanagedmachinepool iam role
b57b35d38071b65f7611c2c5b52b7139941ae03a master to main cleanup
522cd0fe148bd08d9a388ec53a4a6e5fce20c90f Merge pull request #2557 from scottslowe/build-arm64-linux-darwin
55b503f72f5f17f797b4b85fc475adc556ddb116 Add Linux and Darwin ARM64 builds
a697a30e16a2ec09c2aaedf049e8de9cb2192f4f Merge pull request #2551 from Madhur97/aws_2207
59d7d742d87c9639d3069c7899cf1c018b83a68b Merge pull request #2553 from randomvariable/triage-party
75349831d4c5b44f41da20ea1503842c551808fc Add initial Triage Party setup
4a903d91b300ff6dd1ef272f083d390739eb00b1 Merge pull request #2550 from shivi28/aws_2533
a8b547b5e583af0f644bd57b05a4614684d67337 Tagging elastic IPs on creation
7ce361d578c417af254d40cd292225ba1d92cd8e Kustomize patch added for move label
52941e94e4e8522ee2023d8fa16f4ad72a4609b9 Merge pull request #2545 from sedefsavas/capi0.4.0
725f8b0f86add1d8daec400d09be38648ef9ec32 Minor e2e test fixes
f3f7edfe6cbbd4f6a0a8eba0270d5c60e4e684cd Upgrade CAPI to v0.4.0
7d52ccebb87b9de48b9a747863aa446951f95042 Fix coverage tests
101938796a634e8a51fc7e5491b822b793c83318 Merge pull request #2542 from dlipovetsky/version-skew-v1alpha3-1.21
60283c14a65e4cef37115a485b6a9d310c56fbba README: Note that v1alpha3 (v0.6) supports Kubernetes v1.21
1120730e11a33a50ef1336ab022de3c4aac1910f Merge pull request #2541 from xinydev/update-kind
b7e36bf33505fbd136e7690cfcb5ece1fa96d606 update kind version
028bf2b34a87b9aa6eea0f8104d4ac61bea0547e Merge pull request #2538 from sedefsavas/lb-scheme
52ceed7f572b5d1800384f88aa122d477e3c1ba4 Merge pull request #2532 from sedefsavas/scale-in
b6555f094140d6693ac05e7d4257c36b9a7ec60a Add KCP scale-in test
c038eed7e2862434486b108093df96201700c4bf Allow setting ELB scheme when previously not set
f3ce37917aafd6f8d351340846b37cdd42ecf7ce Merge pull request #2537 from sedefsavas/bumpCAPImain
47a0acbb45df8fba04a2e9d3cd84a07a094dc99b Update CAPI to v0.4.0-rc.0
260192f60b9fe8ee3229e0d1fc273f552323d737 Merge pull request #2524 from shivi28/aws_2415
bb1c637ce197ded799983a82982151e47ee3a1e6 Added clusterctl move label to global identity resources
2f0b7e10ae17a6627478c50293fb3a2876bbac4d Merge pull request #2463 from Ankitasw/root-tags
6297c7d8c1c7850463be1aeaeb4412d59182b39a Merge pull request #2525 from dlipovetsky/dlipovetsky/prune-launchtemplateversion
63f052c3f99d64da25bfbf1c01bba1bff7583ba1 add root volume tags through additional tags in AWSMachine
9c8e0259c078afd753b15679df221019449f98be Make a comment more clear.
b5559168578d0ffbb98de7e9d5e882ba3df70ad2 Merge pull request #2529 from njuettner/fix-api-endpoint
92926838390c97a464e4c54dc6c5eb949ae53ee2 Merge pull request #2526 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/apimachinery-0.21.2
e1e777d6dfb34dbc2c807c22df28922df57bf77a fix kubebuilder pointing to changed api-endpoint
1336a5a87abcfb97f391c06aa7b37f9e8e5632dd Bump k8s.io/apimachinery from 0.21.1 to 0.21.2 in /hack/tools
090204453979d1754688c9052177e153a7fdd10b Merge pull request #2527 from kubernetes-sigs/dependabot/go_modules/hack/tools/k8s.io/code-generator-0.21.2
ffb5435d4c8217dd346eefc5a520b993628ca223 Merge pull request #2528 from kubernetes-sigs/dependabot/go_modules/hack/tools/github.com/golangci/golangci-lint-1.41.1
3dca461bdb123aad7d58f87b84f01271d8eb4dda Bump github.com/golangci/golangci-lint in /hack/tools
59a2b3868b583a76b34cf5e0d5a5f65d1047854d Bump k8s.io/code-generator from 0.21.1 to 0.21.2 in /hack/tools
a1bba0a154518f38f757251e27c01f8ffaa037d3 :bug: AWSMachinePool: Prune old Launch Template versions
e6fc82b65806d0fa03cf86bf4481669257f4542e Merge pull request #2522 from randomvariable/f-in-the-chats-for-go-report
4be1abfbd3e619bebc6985bd9eac711b2407c085 Merge pull request #2518 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.38.63
5f36d4c73431146961a8d750124c826b03c839cd Merge pull request #2521 from randomvariable/dependabot-author
32b95cff2bdd376d48bd1215c2490f04b2845740 README: Remove go-report
e82a2a508788adbcdca06838fb2f870b3a0e498a dependabot: Update author of autocommit to pass CLA checks
1835e109ff9d855e715e0d427f14cd892b3be290 Update generated code
9250c65fb3c4d1ae016cad3cea9985db24763dda Merge pull request #2447 from richardcase/eks_encryption
9dd9eaf9c78f0a039e92022f121c5e90d0b75eaa Merge pull request #2520 from kubernetes-sigs/fix-metadata
1dff4d694aa5cd6e2800d52cb12631f975f15f43 Merge pull request #2509 from shivi28/aws_2381
6ef7f7a92b07ce206473e14aea90156d83537e6e fix: added missing kms permissions required for EKS encryption
e55d3ed297b9608aa229cf96caa658e64ef6373d Merge pull request #2495 from richardcase/2494_slice_struct_pointers
91651bb234b430dd70b478e380d70e3b0cbd30d0 CLI command added to list aws resources directly created by CAPA
3712f6f599ada4db3ba3c3e354804584ac0976e6 Fix clusterctl metadata
48229af35b87eea7a5079abb69d8599712ee8f3a chore: fix linting issues after addition of new linters
42b04c9115ca98d9908de9f35d5ce468ec732014 Bump github.com/aws/aws-sdk-go from 1.38.61 to 1.38.63
9bb81e375bf53f37e6adc633bf4145717621bd7c fix: remove use of slice of struct pointers
0f1149c01ce7b3e37512d0f3c6387da419beff5c Merge pull request #2511 from richardcase/eks_e2e_fix
7f14d22eedf00dde32354310b911dacb5970f964 fix: explicit cleanup of eks clusters and using static identity as well
006b1ef8ce6b9ada16fe62c4e3efeeb2f283f220 Merge pull request #2519 from randomvariable/update-dependabot-github-action
65c7adf5a6017c71b49bdeeb899826f74f8b3dc9 Fix dependabot Github action
e4d6c3ce8ceb2154d934db7492af0695bd5f9752 Merge pull request #2506 from sedefsavas/dependency-update-june15
0f6bd2320a7eb5afc002f62d1650376127dc7531 Update dependencies
159c13f18ec81243b9f2f1ac700e41a144863b96 Merge pull request #2517 from tech-geek29/enable-additional-linters
31bb3d885c8630b08cf035a6ba4bfe4c57aa62ee Add addtional linters
e3916f215d415140308175c78ae8cfa7f9ef1954 Merge pull request #2515 from enxebre/fix-capi-aws-nightly
6dc7290420fa523856d2d1d539dd9e90eaebff3b Merge pull request #2443 from Algebra8/issue-2428
0de0639c4d90bd1ee26f4e778dad1ee1e8c60357 Swap Golint with Revive, enforce Revive's exported, resolve linter
6797e968c978e23a062105e20e6ba4cef48f5faa Merge pull request #2516 from randomvariable/autocommit
a2538c9535d3024e9d23cc331fb4dcafceb290df Dependabot: Add workflow to automatically update generated code
678d99cf747fc2ca849178714aefcfb51a4c8945 Add file and make commands for nightly build
8db86ddba56f28629ddaad5b8bab677cca6bf6ce Merge pull request #2510 from tech-geek29/add-shortnames-to-resources
39c875ff79ce8b0b628151793940b54cd91b7cc3 Add shortnames to all resources
6f728d1d1f86905c85bde785ada7caf8cf6abf7e Merge pull request #2507 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-sdk-go-1.38.61
e3f64731cb33de678cd92e49f637c7889822cf22 Bump github.com/aws/aws-sdk-go from 1.38.57 to 1.38.61
daec13ddf6b87d34364b353224256c72ae4af15d Merge pull request #2500 from faiq/faiq/fix-2497
a274df3432e788ae3f1fc7d16f9d2fc5a803648b fix: break down DescribeTags requests by 20 LoadBalancers at a time
469c2a2d461e8b28347e57c84c7b25fec73b270c Merge pull request #2485 from randomvariable/dependency-update-jun-2021
436d4aa265a809d85bc4547ac0b9397ab4077b17 Bump dependencies for June 2021 except gomock
df3c67f417ffac9e3a997b98c1ce6e215577de06 Merge pull request #2479 from kubernetes-sigs/dependabot/go_modules/github.com/sergi/go-diff-1.2.0
fc502e0395a8662fb3dc7495e3c3f22601ac5649 Merge pull request #2474 from kubernetes-sigs/dependabot/go_modules/github.com/aws/aws-lambda-go-1.24.0
1236bd9326d977fe8c6fa59f82fb5b6264415c08 Merge pull request #2469 from Evalle/ISSUE-2435
0ed4980324f07467e401da3fe05be21c56bfc9fb Merge pull request #2477 from kubernetes-sigs/dependabot/go_modules/github.com/onsi/ginkgo-1.16.4
b73459e0818ce0b2de7fdf71f8e26d0e36e792cb Bump github.com/sergi/go-diff from 1.1.0 to 1.2.0
41aa39b3b8537311960f7011fbf33469e33c413c Merge pull request #2476 from kubernetes-sigs/dependabot/go_modules/k8s.io/klog/v2-2.9.0
49eeb08a4d662071eef4820aa6c09180c7d6d58b Merge pull request #2473 from kubernetes-sigs/dependabot/docker/golang-1.16.5
ec08e8c7232a79494d0cd88fd15b4e1eb172191a Merge pull request #2472 from kubernetes-sigs/dependabot/docker/hack/tools/maven-3-jdk-14
2d98a99435e1ebd5ff11bb8c6fe0b686ea285eb8 Bump github.com/onsi/ginkgo from 1.16.1 to 1.16.4
77f0f939f51c63daf9a33195d96652179fd71ccd Bump k8s.io/klog/v2 from 2.8.0 to 2.9.0
722eb71fcbd5fca5466f57dfd7083c3c95f5006c Bump github.com/aws/aws-lambda-go from 1.23.0 to 1.24.0
8678b678d66df3bdf8a225a3513b82495288feef Bump golang from 1.16.2 to 1.16.5
2e1f0db05b146c6e6bf4d02e80c1b7eefe67aa4e Bump maven from 3-jdk-8 to 3-jdk-14 in /hack/tools
53b26150790801f39f4971a127cea4ce82840682 Merge pull request #2470 from randomvariable/dependabot
229394974e29c552f2bcc37f0dbb815e6ca4b910 Merge pull request #2431 from Evalle/ISSUE-2414-1
6a211cfa2819de8f06da4b6cfa27666d25897e87 ISSUE-2414: Add additional linters
ff492db98e68d3f2259c0be22dfb720c6cb24cae Add dependabot configuration
c68e91d5588b01970d2b99839affdfafbc0e0b5f Update calico in e2e tests
52a92ca1f65e4cf114e233af2db09902ebd1648b Merge pull request #2460 from sedefsavas/intro-doc
f0871546ac179c3fb589066edfb798ea3e80f710 Merge pull request #2458 from sedefsavas/envtest-cleanup2
0d95d52aa67fd0f07c409982881a89d293ddbf23 Merge pull request #2405 from richardcase/2399_node_taints
49c24cc6193371eb3cc8487f3e238acf41fc8a13 Merge pull request #2445 from spectrocloud/fix-fargate-mutate-webhook
260f1d282e44d7a88edc52f68d0aa00aebe359a2 Merge pull request #2436 from Ankitasw/webhook_validation
aa901e8e22651a8c01da37f9092354be982dc414 Merge pull request #2457 from sedefsavas/zerocredentials2
6761f954a28b29683d9d157285109fbe22de3322 Merge pull request #2418 from sedefsavas/refactor
6002d7a3ede2c267a2f70d227b448dd6581eb065 Merge pull request #2344 from sedefsavas/external-ccm
36cb486e9777873c47ef8fcf6f3b55904b77f951 Merge pull request #2461 from sedefsavas/minor-release
09492c615e8f539976fbd3405e769eb65924b273 Adding v1alpha4 webhook validation checks
85599dedc2231492f4232350a28f2db7bfeb3e4e Add new controller commands to clusterawsadm related to updating bootstrap credentials
b94966ea4f8ebcbb078586bc991733c3b78e8b57 Minor makefile release fixes
f3abd3ab11e338c1e2b7c80e2bf182534ef6f1b4 Minor doc improvements
9b294114bdbef8b99f3bb6ce3958aca9df229538 Merge pull request #2437 from Szymongib/bug/accept-extra-statements
c6bbd5f4360541c34b671eea53a2a9f0dfd9f8cf feat: add support for taints for managed machine pools
b8deec1e6cd39a8740385c07766b8324b2ae2858 Copy envtest cleanup from core cluster-api repo
337a8619b782dd62927c0be582c522af4e5b2a2e Merge pull request #2451 from enxebre/fix-usage
52625bea778c2b409815d7f2ffae15673c730725 Reword wrong webhook usage
ee839cd42ec2a9d9e304eba18e867ec35878e5bd Merge pull request #2425 from sedefsavas/2400
49981f4d489d3f06868a5e90a732ca5b1fcdddd0 Merge pull request #2439 from sedefsavas/developer
80fdeb77e9dc0813b00cd170b289e81284a38746 fix typo in awsfargateprofile webhook
f746ca8ba38cd9046561d3832356ed4bbf0a8261 :bug: Process extra statements for Cluster API Controllers
7b1162ba220b641fb72d3a87789b8136817a925e Merge pull request #2438 from shivi28/aws_2004
268e4e791ed6599732779ae254e277e8fc5c3af0 Update developer section in the book
9cfd4653d1abb07876e148db425167a24f4a82c2 Move IAM API types to /api/v1alpha4/
8e1d0273a154d3293694d6978ffabbdb356b7dd6 Use Kustomize to generate test templates
2a183f580873ed46aebdbba77da212a3476682aa Merge pull request #2430 from shivi28/aws2258
b8415b67d1836ca03d85801940c9950c472c80c2 Merge pull request #2429 from sedefsavas/capi-upgrade
09965ca59d28e76158feeecd3945867df35efb93 Switch published artifacts to k8s.gcr.io
b6494f993242d7849cd538177ccd74a7a60de1d9 Update CAPI version to nightly 20210524 Change MachinePool group from exp.cluster.x-k8s.io to cluster.x-k8s.io Change KubeadmControlplane InfrastructureTemplate to MachineTemplate
c53c107cbddb9e32e79455b1b7f96d46a7aafb08 Merge pull request #2383 from alexander-demichev/predicate
0aac237ba314b90954c4ed46376032e24e694f74 Merge pull request #2423 from Szymongib/bug/2392-align-cloudformation-create-and-delete-commands
716d12d7dfae9caa00845cab0cb1a3f112961ce5 :bug: Align create/delete cloudformation stack commands
4de5136cde981760940a8fa5d799112aef0638b0 Only read AWSClusterStaticIdentity secrets from controller namespace
7b82f486d58d276ba74b9be65a46ab80d656e2a7  Refactor tests to plain go
5a1266bcf509a4827c1d6d452cf10936bedc44be Merge pull request #2417 from sedefsavas/controllerruntime
59ff8c841b1f5cc85567f71c76a4d5c595dedf70 Update controller runtime to v0.9.0-beta.5
7c363708437fa9bd83c4aeb3091956d4575b6829 Merge pull request #2411 from dkoshkin/launch-template-notfound
b0256b273c90da933c7978b9d4cc1829aa09bcf3 fix: handle LaunchTemplateNameNotFound error
c062037ce1ae29bf7ac1c4206d82c171555f153f Merge pull request #2375 from richardcase/2318_asg_remediate
00fb0ecad79a1cd3885c81ac88fd5b5027a30d82 Merge pull request #2404 from richardcase/2389_ssh_key
d50c6c1b46a33b2ddde05a31fff958d0d4ed4e74 fix: missing iam permission for key pairs
1e41b01bbe253b3cadcf57e9db817c06605813ce Add externally managed predicate
f05e673943f4bdd5820c955a8bec0fc799d04cb1 Merge pull request #2403 from spectrocloud/fargate-session-identity
c91ff893a908ac2efb77a518a15a1084897f300b fix: managed machine pool correct min/max size
563eecf537ba56c97a6317a9a5bbebb7433b8d1b add identity ref support for fargate controller
c92d6a06e60563bb747137414eb1e747bdeb214a Merge pull request #2379 from spectrocloud/iam-role-length
0c969c50632c21224ddd9afba12c7dedef256d72 Merge pull request #2398 from sedefsavas/validationtesting
2025b6e63097813c81adbd62c7bc3a224c3d9626 Merge pull request #2395 from sedefsavas/lt-get-byname-main
8096533e05128206ae3c87ff21a5618060a0c504 Merge pull request #2382 from sedefsavas/e2eparallel
02f2a0232c7c4f85240878b1c16b26aee896b30c Add validation testing for defaulting
bf54562daab8d218808017de95757cf527dbc054 Allow GetServiceQuota action for bootstrap user
69f608f6b038f070afd3e83d5be0d9f81beae76e Add e2e parallelization
09002d444a57ac645add2236b979b77d78dd2053 Get LaunchTemplates by name
bc14da8fedc9b23c97261b93fedfdb7ad2a6ef99 Merge pull request #2390 from sedefsavas/conversion
d03df00a8c74642b7200894ee81f996464d2e3a0 Add v1alpha3 to v1alpha4 conversion unit tests
e1eaa10d5e95188b74245ada94768f4ac98dc932 Merge pull request #2386 from sedefsavas/remediation-e2e
cb363ac4a1c009969f143b22310ba61932c1015c Update template for capi remediation e2e tests
ca1cb6ad810570e2568b1ec8da2df07312c0cebd Merge pull request #2354 from dlipovetsky/machinepool-token-refresh
17c5c892f35a8da34102469e4bfd33f920806c3a AWSMachinePool: When userdata changes, create new LaunchTemplate version, but don't start Instance Refresh
3add395bc2e79bbc3e45fba6863959d1a84bb89b LaunchTemplate: Return userdata hash from GetLaunchTemplate
006b7efe9295bde200d30b22c214185394911217 Add ComputeHash function to pkg/cloud/services/userdata
50ed34302bbae8868db158bdfb7bae4bd874bcd6 fix max-length for nodegroup IAM role
835d3f606cce4fd1c813dcff0d8eafef3bf61254 Merge pull request #2376 from zhouhao3/fix-ineffassign
72f4dad21a8e72e7642d3e8327d9e4bbe14a19af Merge pull request #2121 from sedefsavas/v1alpha42
a19098ae78716a013c894366399ed181e479ec27 Set netlify go version to 1.16
dadf2646e7369a3122828d720a4d21be11c94edf eks e2e test config fix
8a81ce6890e5728d4c23f95363643b10ab89efb6 Other v1alpha4 type changes
c957d07c981dde0cff4dc7bd4e132fc943f040f6 Add v1alpha4 manifest changes
c09f55f8f2249d9fde6d7878a6595bf1c4672ff2 Add v1alpha4 types
cc5b6e919c906d30b0b63658556f3cc2d3745191 Delete v1alpha2 types
7e56f4e3ed961c2027fad9c7cf4cd87c44a42e52 Merge pull request #2359 from martin-ducar-gd/release-0.6
f8c504e67df09c3824b4b250b3ed5a276e9be298 test/e2e/suites/unmanaged/unmanaged_test: fix ineffectual assignment to err
7cc5d20972ac841ef674bad1eca1d7ed95a7edf5 Merge pull request #2370 from dlipovetsky/dlipovetsky/ensure-teardown
9411db872c3d5028b0ddaad427b6bbfd21ba6baf Merge pull request #2365 from paulcarlton-ww/identity-doc
06ea91bfc882b161f0af8e2a972611c787b519c5 Merge pull request #2373 from paulcarlton-ww/controller-identity-fix
1401f28fb0cd03ee5691beed5e3b13920f73944d bug: add namespace access to eks-contoller rules
6de2f7f9a9ae4f8dd2209bf817b07d646541f769 book: fix typo identityidentity to staticidentity
e31bfb7d11ad5e5435299e1483f343ca0bf83ca6 test: Ensure teardown runs
365779a14d0d1023b1e5ff4a9be3d19a02e4648b Merge pull request #2357 from randomvariable/branch-rename
262a4499ffeee9da8458e903e6d3f580d3376b66 Rename references to the default branch to main
2eb156fe885d3ca0e6a4d99c11c79128ad314611 Merge pull request #2337 from sbueringer/patch-1
c638a931e02125365e97c3a25d2ffde083d4a5b2 Update cloudbuild to Go 1.16
4e4bb370cd3413cc866c0cf3ed9e9324ea5e8b02 Merge pull request #2362 from jimmidyson/jimmi/machinepool-sshkey
8f3aebb02fd10db3d44928ae365f5b8dff25c254 chore: Satisfy mod tidy
7c7780a4762a85ca894c6905831f2e50ea52768f fix: Properly handle empty string SSH key name in ASG launch template creation
7c23c606e0bde1190b168b3c8d06f863afdc82d2 Merge pull request #2360 from randomvariable/ami-on-readme-update
5edd79206966a60a915cc1d5a851b9ef141c9138 Replace AMI list in README with link to amis page in book.
ce7026ec3eaae93dfcc5043753ce12a43cd06b88 Add required clustercontrolleridentities
ab3afdef21ab208a780810034f615fe0b48a6c1a Merge pull request #2353 from randomvariable/google-verification
c7c8ae1ee071afbb33c3b45b0f9adbea149581ce Merge pull request #2352 from randomvariable/eks-crd-docs
8be4b81ee8643944dcaca2d0afdb4fe5493b4ca2 Add Google verification
6a38c56eedcc99f252484350cd6726a21a0ad8b3 docs: Add EKS and experimental CRD documentation
e9d16b07b579b153c289c47e0c1a4e6cd5021a5d Merge pull request #2319 from sedefsavas/multitenancy-docs
5746097b034251e143f90f7a3bc9b7812afb2606 Update multitenancy proposal
69cf50ca1ce11e8a656f8f05dffe28594d1e3ac2 Add multitenancy docs
41110166021b430c8e2e55711b87a1a4983dd9e8 Merge pull request #2350 from sedefsavas/coverage
2bf3644d38f840087ba3dfa1cd1ef353434fa06b Merge pull request #2253 from sedefsavas/multitenancy-cont
0626b9b6d2c76b70b6408819fce6c2f12ac475e7 Merge pull request #2345 from randomvariable/clusterawsadm-ami-refactor
4c23de3c97a54e1f3bdadb66b08130d5c7487754 Publish dynamic AMI list
e07d61ac6f7031d84b5a3eb7fedd83fea0731251 Refactor AMI commands as libraries and with TypeMeta
10ed91189786035157a61f3b4e729d79d19ff733 Add test-coverage script
b8ff4b29055caf9dcbf289ee468fb666cdd6efe5 Merge pull request #2347 from randomvariable/crd-docs
b2d95c7993f7ea675a1a922d6fd17887a6a1b40d Add support for controller multi-tenancy
c6f0918bf0c4bd7902db151445627f2b8640cc7a bootstrap: Expose AssumeRolePolicy function for external consumption
6b442a3172287d95898d883d2e33c978b561de49 bootstrap: Fix policy statements for bootstrap user
aa5c3a05ac827d2257a24c1f4741faf6b9fd98c4 Merge pull request #2349 from benjaminguttmann-avtq/fix-machinepool-template-links
e4a1eae06004319ee7e77cf6f654093737815781 Update docs/book/src/topics/machinepools.md
22b5dae334366a3be5e6bb3f8a0034ae189e77ff Update docs/book/src/topics/machinepools.md
9b06729a6b7c647e4c42a0385576a7f43784ff16 Merge pull request #2348 from dlipovetsky/ssh-key-name-error-field
13dc8ba4e84d72a6828fb7d0ee8e1e59d4fa49f8 Add CRD reference docs
b70b4fcdf8c9d63f9f6846f4182b479502af34d8 :bug: Refer to `sshKeyName` field in error
f34cc84619ea962e3e79d1f3d31034638ffd9ccd Fix machinepool template links
5b0b59099984f7035f4701b5d70c6447d7177264 Merge pull request #2343 from detiber/emeritus
460edbfc2b1ca81815c9652532b31343c87d7919 Move detiber to emeritus
81850ee2d5392e7fe305ff51e1c58ba64033d5d1 Merge pull request #2304 from sedefsavas/listamis
f0f68810fef3c1708ad95fa382768d66ec737d45 Merge pull request #2342 from randomvariable/publish-permissions
28292542931267bf8c3017c5431caf09b4152386 Add list AMIs command to clusterawsadm
d32daf720c3e98b1aca26dfbe066a66d17cd0613 Generate clusterawsadm documentation
20713b17276358beacbfc87e2c785ec77f39da5d book: Add IAM permissions documentation
c8651317cc64b4be804e27578d409ab36384dadb Merge pull request #2341 from randomvariable/fix-bootstrapuser-defaulting
4a888b9d6af8d6ee636bffdf5e1e38e846aa98ca Allow custom bootstrapper user name
bdae887409e71a13e4695c8d671efee4a24aa5f2 Merge pull request #2338 from kubernetes-sigs/is-netlify-broken
e99981e3590f6f6eb2b07ef351e75d087a47d495 Merge pull request #2328 from sedefsavas/2156
2f820ea8c6300f760343e475a248f5e30a3015a0 Ensure mdbook-embed is in hack/tools go.*
76d4b0fea950c2ccbd8505d87ba0f2f00d95ddad Merge pull request #2327 from spectrocloud/vpc-delete-failure
6a10032dcbbad78bc4e683cd516aa023a8498056 removed space
1fb7b6693299468643bc1c07e975dde8f84c454b changes based on review comments
2bd1b21f4681d154aa6cacfa8229eb17756ba54c Add ApplySecurityGroupsToLoadBalancer action to controllers role
46f54e483889596c4033dbbb23cec764576269b2 Merge pull request #2325 from randomvariable/maintainer-contributing
c59508eaca8083e40e7a596110147ef2ad947303 Add maintainer docs
d1f5af6625c3a5b678236194478fe16149338993 minor changes
e91a69f10bd2d913f49df3b463d031d535533ead Merge pull request #2324 from stmcginnis/conversion-gen
022cda362396ac8faf34073a1c7073b4bd26589c Merge pull request #2312 from sedefsavas/apidiff
2b268a6ee4d6670ca4499d034f766e093846e191 Merge pull request #2313 from sedefsavas/upgradetomain
12169fb2c7e23e75d7d364a5aed54edefdbf1ec1 Add apidiff script
91dd72a61546fd439399edb969c336dd32f012aa Make conversion-gen output location explicit
5d899188dfcf7c5b6fcf63c055bfe5d640041290 Merge pull request #2322 from randomvariable/brand
295334c4ecc926257c685add4f7fce0e10cfe920 fixed vpc deletion failure
82c53e61a6186b41043131440c8f47ebb4ea82ec Merge pull request #2265 from michaelbeaumont/fargate
ef4f4417779669b9df08faa1f72565eafc96e256 Merge pull request #2315 from dlipovetsky/ssh-key-name-test-refactor
3181cf5a008dc19fbd62314d3cc16e14985675fa Add upgrade to main test
0745e18370d7271a886da947747b6426b102d7d5 feat: added fargate permissions
6ccea2fb5150c95f239eb6cf672a7b6a788b1823 feat: added fargate profile support
9a2cf01bb9f8145cfd885c487f8369aaebaabba3 Merge pull request #2314 from sedefsavas/clusterawsadmdocs
30ff6d31a7d7605ee27025996518e477ba1a7008 refactor: Validate SSH Key Name using a receiver
ee568e114b839f2bd1d190508b881c3d3944770b refactor: Group SSH Key Name validation tests together
5d3c76211239b3700d1f69a36c7819f94c5b2609 Merge pull request #2308 from dlipovetsky/ssh-key-name-validation
68bdb948af406ce7903630356383e4edfbafff14 Add clusterawsadm docs
4c042d4c83e32ce9e6abc7f5683dfa3f38c0aa52 Add PR-Blocking tag to quick start CAPI test
92eeda4b51f82a25b2b9f396b4f5615ac2ab503d refactor: Move SSHKeyName validation helper from webhooks.go to validate.go
cdd12eb12b4ff6a4fb80be83b79695477ed3de7d Merge pull request #2307 from dkoshkin/master
6ebae675aefefefc3525bb3476ff464208d1a8b2 :bug: Accept empty string SSHKeyName in AWSCluster & AWSMachine validation webhooks
852066b07b6f12e25e741f41a5b43c7d554f5cda test: Accept empty string or nil SSHKeyName in Machine validation webhook
005c10df5f3ad531565c4c49a20da9a2bd73dc28 test: Accept empty string or nil SSHKeyName in Cluster validation webhook
f7ef6f42cd5e19a8e67aceca1d68e02ef945e0b9 Merge pull request #2302 from richardcase/2277-machinepool-subnets
8e53fd70d0d84e8ebbd6e4075fc620841da2aa78 docs: clarify subnet requirements for existing-aws-infrastructure
06966c76975f132c8a6ba7c8751146a6b13f2625 fix: machine pool failure domains honoured
48f64dc6d364d7448bb43c5c7a80bfbc979024a2 Merge pull request #2295 from stmcginnis/klogv2
e1ecb6451a415f90e750d5d392dde088dcde25e8 Merge pull request #2303 from richardcase/2300-docs-link-broken
8de540ae1a7266e1b187983ccd5ae32cb79e1fd6 fix: broken link to pod networking
525834a1487b8b84417464d23eaa32a72d7508ca Update go.mod based on go1.16 dependencies
1006f61aa9e79cb9882e56bd5f96ec3b898807d7 Update klog dependency to v2
fd4cc9d3f8db29b226b3e1d24dd8e14602beb2e3 Merge pull request #2293 from sedefsavas/eventbridge
c3dd8d9dab0740454a261eb328b027b21d4d8245 Merge pull request #2285 from sedefsavas/useragent
6f6c9842917adb33ad4b0e951c0baf2183636ad0 Enable EventBridge feature
a44bff2f60be148d66ca4e2ab58831cab3955e81 Merge pull request #2292 from richardcase/disable-vpc-cni
3d2e553e73255873fb3166da800f186e7ffdd86a feat: ability to delete amazon vpc cni
dd78b066d11f7e8efc33927e93eb02eccbe9ef54 Set the UserAgent to "capa-controller"
f411c2153abc70aaf94e8424854852bf471f35b0 Merge pull request #2290 from sedefsavas/lbvalidation
5248d7897b74ee0f59479365cf868ab5ba960406 Merge pull request #2281 from sedefsavas/fixe2e
6e81d007627ef6af4754d22cb5eea31f6e86054a Merge pull request #2278 from richardcase/gpu-eks-template
87da075aec55f37a0479c7acf5126e0b7536998b Merge pull request #2288 from newrelic-forks/rtorrents/capacityRebalance
1b9d88d3efc9804679f737e0907e1c2acc7e461e Add enum validation for loadbalancer scheme
342067f060cbb02f013c1ed19dae67afc7919d21 Merge pull request #2291 from sedefsavas/conformancefix
d04ba5302ae54b1c4c52e960d26c3e4824f45e93 Update to latest cluster api commit
ff3ed1b9f6f1624d94752f57bc8a5dd79ae133a1 Merge pull request #2289 from randomvariable/govcloud-fixup-asgs
b592cef7480d0ba548f0f5fef24e13e5aeefccc2 Merge pull request #2279 from richardcase/sedef-as-maintainer
12b9c8f6b165829c0b4322d46f9e767435e21608 Fix Govcloud support for CloudFormation generation
dbd3b700f7eebe53e0cb1b44df797b6201d9639a feat: implement ASG capacity rebalance
6f497ef0fc0b5c2d382ee995ae7ce5dde164606c Merge pull request #2264 from richardcase/remove-managed-cluster
f576b5a6d463db320b74b48435bad4a5052cf410 Merge pull request #2282 from sedefsavas/0.3.14
d2be453e6abd339387a120c1f6b0de256d2b3650 Merge pull request #2273 from baldwinSPC/master
ff8ea2bcf1b91aa119a92aef72ed9fd9a0ed32e6 Merge pull request #2286 from sedefsavas/elbname
9e114cd08c44328420fc0f8c52b29a00540d4771 Add name tag to ELB
4d201ae41be37fb4f3b56405026e960bb5d00f63 Update core cluster api to v0.3.14
ab50a8a700dee3dbe04f6ff72f09a471551c5626 Fix e2e multi cluster test
5fcfc82e7509a00d3d3c5e131593c867243e436b chore: maintainers addition for sedefsavas
17c3144c5f0060526a005eb5a2927db22fcd259a Merge pull request #2266 from sedefsavas/spot
20576ef77f27baca8cd6281d25caad4974488be4 feat: add GPU EKS cluster template
7d1588334e9e142fd3a7365370d72e29364e1081 Merge pull request #2276 from pipo02mix/patch-1
c9283248cda4a1460a5a644f9b83363505afa8fe Update README with correct AMI link
2e22eae635ecfb7579a3a3f2cb8f71ba56ebaec7 Update README.md
d0c15cfd7d218947c6e0bb082edf61da551694f9 chore: remove usage of AWSManagedCluster from templates / docs
c5ec5d2c90bc22516950a03bb8ba0aa02268e1c5 Merge pull request #2262 from kinvolk/dongsu/fix-ensure-kind
e41e423e998e3a44d3aba5ae19e6954b1b10a7c5 Merge pull request #2269 from sedefsavas/multitenancy-proposal
03e964446c63914af402182ca8ef4a55cc750f50 Add AWSClusterControllerPrincipal controller to multitenancy proposal
3ec90df1c7ed4b58d5fa390bd826713490e93cb6 e2e spot instance test: delete spot option from control plane machines.
76ea0c9445caa2ecbdcf97a24dcaf0433a6f8139 Merge pull request #2259 from shuheiktgw/replace_awslog
b1de7b334243092bea5651e91e3e77bd601a4ed8 Merge pull request #2260 from sedefsavas/amis
831c206d9617f5d4996ad216fb63d1051da21f54 Merge pull request #2252 from richardcase/updated-pr-template
dd740351d3bd6f0effdaf4af2faed4dd30574f02 Merge pull request #2237 from sedefsavas/multitenancy-permission
ac55e9126a6bc51abf1a08fb9dab4fde77a10419 Merge pull request #2261 from michaelbeaumont/fix_args
b4e195719817e4d982584227d714df25de4e5185 Replace awslog with logrWrapper
d9c3d5a3b8edd524c0d4029b3582c0e60571c7ba hack: fix semver comparison in ensure-kind
eebdf60efd06143987a3050bc7d6acbbf6c57a16 Fix manager arg inconsistencies
1847a36a1a94b09c2a5abe871d90e994c6a1c682 New AMIs for versions 1.20.4, 1.19.8 and 1.18.16
fbf880963b07b2fc5f869faab0e0ab07aa06a729 Merge pull request #2229 from shuheiktgw/log_aws_service_call
f7aeb06dfaecdf7ee692a4c9a35de59c6e29aaf7 Add a logger to log AWS service calls
38007acdd23ed4cc091cb1f267b178fd195bd8ae Merge pull request #2250 from michaelbeaumont/fargate_adr
6287acbce416d6e5032baff8281fd360d918825b Add FargatePool ADR
a824b1f0669a036557c16cf85cd1468a198a260d Merge pull request #2249 from saamalik/patch-1
cfcfbdb9a664742c072bdf7307ee526be4aa0564 Merge pull request #2247 from richardcase/release-notes-automation
6b0e4fbb42d87ef68d27b581a838f720f9b5c3de chore: updated the PR template
18ba5a5968fcd6289f50994e3ffff856066c154d Merge pull request #2246 from michaelbeaumont/controlplane_conds
220b08d199d5c84c164870cee11a688c03f912a5 Minor comment update
252409e5b41c34360a7bda6d8097cf2671743435 feat: added release-notes automation
c4d270e1eccdafaa2ebceeb9cd159733788b98b8 AWSManagedControlPlane: Add conditions for Updating/Creating
95104b9b793d394a50dc2e95d98200c8398713ed Merge pull request #2243 from michaelbeaumont/remote_access
c54dd7aec62d98353fa0cacefe9cf1ffdd717a4c AWSManagedMachinePool: Make public access to SSH explicit
3ac3feb12e8f49152fc9f542408b80d6898498eb Merge pull request #2241 from alexander-demichev/sgfilter
6a99ef9bc76d4dbbdb68d571c55ae9bc1d705177 Add filters support for additional security groups
06b473d3bf5662008f6f599c22fd94d332023523 Merge pull request #2235 from getupio-undistro/felipeweb/fix-bastion-managed-mp
c3017397b440f0dc018a9551dd457dc1918864ef Restrict controller credential usage to only allowedNamespaces Co-authored-by: Naadir Jeewa <jeewan@vmware.com>
dafe0711b279a6c04735338f9ccffa392a6d0f36 Merge pull request #1933 from andrewmyhre/1137-override-security-groups-master
f58e99a4285caa55612c6dbdac8c32399bd97a2a Merge pull request #2232 from richardcase/release-notes
8d956a3ed099d59466f0dd7441fd8f696e2ee62a Merge pull request #2234 from kenichi-shibata/docs/adding-development-guide
ed4e36b5d96aed79a99a244152d3723e2cc48ee7 docs: Added how to develop locally using Tilt
40a56c73af050727f795ae1e606dfc258496da7e Merge pull request #2240 from randomvariable/fix-e2e-feb-2021
a538031fa6700456b3243ef30087b430cdba85f9 e2e: Disable EventBridge until we have aws-janitor set up
3611b86f0bd929441ce0a1870761d5154b20ac77 ec2: Standardise error logging
12913fd235e0a08cef390c0ce196335cdab89887 awscluster_controller: Make EventBridge failures non-critical
20bcb1906556c346e9ea307bfb9aa3fecb9114ff generated files
30b7e3703155b2bfacf30a51909182269aee6fc9 BYO sgs for load balancer test
5750cb5ebbda83ddc00531290faa51282539d165 support overriding security groups in AWSCluster spec
5721067c87ec597c8b7816d9e79851ca6bad5129 Merge pull request #2037 from gab-satchi/1871-event-bridge
6504b521b9d19bea4274ec60e75d662bbad7da7a Watches instance state changes and reconcile AWSMachine if necessary - Reconciles an SQS queue per cluster - Reconciles rule per cluster on default event bus - Custom event buses can't accept aws service events from the same account - Adds queue as a target to the cluster's rule - Adds instances to rule as instances are created - Creates a policy for rule on the queue so rule can publish to the SQS queue - Adds instance state controller to track queue URLs of all available clusters - global scope that isn't tied to a cluster - triggers reconcile on AWSMachine when consuming messages - Increase cluster wait time for e2e - Removes instance from tracked instances in event bridge rule during deletion of a machine
44be0da6f98f979646f3e0e7abdc78a05a0d40c1 remove unecessary function call
4d84bf665f6a0ce9d6114043ed6c14e64cd3957e added security groups to nodes
53ebbf12d97a53b5075f41ba4af5b5c4d2959d18 feat: updated PR template to include the release notes section and checklist
1b76801947bd31a0e8da64d3c4dced46ac76e88c Merge pull request #2223 from sedefsavas/update-release-doc
b2633d2b78db463298b7e9ef3be7285f163d0ec4 Merge pull request #2230 from cjcullen/patch-1
01338c6afa6c32099c26484eaf66ed92fd5d38d5 add node security groups in eks creation
6d22cccbfa4a8d655a3727edd132e5b5b565a601 Merge pull request #2228 from randomvariable/allow-no-backend
a4ef74cbed9cd881ae1d29437b8e8eca6a1538e8 Update mdbook to 0.4.5 to fix CVE-2020-26297
643b19f9bc87197ae6dc394b453584b72437521a controllers: Add conditionals around fetching secret backend service
6cfe6049f93d5b4b9b598a0d0490c4f7b077c826 Update release doc
634f30eb5a3ab42ec21e358cfb86da740784aed7 Merge pull request #2138 from sedefsavas/capi-e2e
cc5054a883a519d432080e75be4699595ed513f8 Merge pull request #2221 from randomvariable/revert-ext-cluster
a9130eb6ff632497f177631e3ab5196527a98207 Revert "Add externalInfraCluster"
ea42418f9349c1140c072a515b72452a5aedae1f Merge pull request #2202 from richardcase/2139-eks-addons
f469af8010c76cf54d6aec727a5d0db426b2989e feat: adding support for EKS addons
fc2de5b2ac5ce00b50bf481d217e45017d63feca Add ASG CreateServiceLinkedRole and DescribeInstanceRefreshes permission
b58296acae3927a6ac122e78c6dc9049d2796c30 Merge pull request #2220 from randomvariable/preload-eks-controllers-in-e2e
5ea54e88916a0ce6c5363444e3900a6c743be7d1 Ensure EKS controllers are preloaded
f2cca5f30edd932fce4b12b32a34350e895c3e9d Merge pull request #2057 from MarcusNoble/eks_ami_lookup
458025d9e8783c29356586e06cc4f88c36ca755b Support custom AMI lookup with EKS
f9e06793aab4269675b3a841c5d9094641ee11ab Merge pull request #2217 from randomvariable/disable-cgo-for-kustomize
dda9d8c824aecd16c7e1bf58a62faac1d49cd77c Disable cgo for building kustomize without gcc
d59d4fd8789c036bcd8ee8c911c177d41dba2bce Merge pull request #2216 from randomvariable/fix-docker
065b727dad168d40b6830042d229da4a8f0036ae Fixups to Docker build
c76bba72c4b0a92524a1125d9c57831465cc9f10 Merge pull request #2215 from randomvariable/bump-dockerfile-experimental
35a7e9d4e920724cf964a6315c6b9a8ebb03bc08 Bump dockerfile-experimental version
1e5c60540974e29ebcb9dcfb6df46e5ce44044f7 Merge pull request #2214 from randomvariable/ensure-pull-image
ce7bbf76de184540f9d8ad416f9ffd1acba42bdf Ensure mirrored OCI images are pulled before building Dockerfile
88014bb31bb149bdae51c7fd4acb4772c1662fdb Merge pull request #2213 from randomvariable/update-gcb-image
d03cac1c52be6a18787baf6b7b2ee5b268e843c9 Bump GCB Docker image
1df714c4b76e7771c6320b7cf179260345cc43dd Merge pull request #2096 from randomvariable/manifest-updates
bebdfecb2cae91b4729f1d6993e895463eb4b206 Refactor release process for Github and Staging
d23cc4e599df3c82974c22327c35fb4834b9aca7 Merge pull request #2086 from MarcusNoble/secondary_cidr
4cc8d962779a22a1338c02e5235768b3d1a17ab5 Added token method to test
d9a6e5e3b31b182d97b90c1cc0f8f5cf8c26bd76 Clean up old ENIConfigs
e71c6c493593b2b8a580c77f51740ab1c6aee16b Secondary CIDR range for EKS workload clusters
7470b49be4c65865676d7833b37133d4da5a8f82 Merge pull request #2201 from sedefsavas/rebase-ratelimiter
29f7b242668dbc6743d02e2a5361a065af7feedd Merge pull request #2070 from michaelbeaumont/oidc
f58da95330c2b694776e8282fd76668deed9c328 Add OIDC provider creation to EKS control plane
0b385344b3af73823dfde50d7b9df8f6de42d352 Merge pull request #2211 from MarcusNoble/skip_eks_upgrade
4d728535a9d8f795a00009c781951cf9ea078134 skip EKS upgrade tests when running e2e
8809603dbf5abc856bbad9375a946501ab664a03 Minor Makefile fix
9a0e8cb6ed3f9785bbf79af57b04532bf94b78bb Add CAPI e2e tests
d3db52ac6899d4b3ee09a2e8360230a3dc7c57fb Adds a AWS request throttler based upon per-operation type request buckets that can be reset when AWS returns that it's throttling us.
58bb690de59679979bd3a4a9ce5b0b10d48e2c25 Social card image
cdf971f721f99d161fc1b7f27a2c3f22257cc6ad Merge pull request #2206 from sedefsavas/new-ami-1202
cfd02cd8bb33dd10a9bf0635d6e05028eafd1b94 Merge pull request #2193 from sedefsavas/refresh_instance
91a7dcbf8e376b4e15656ec9da3b5edc7dd6be24 Merge pull request #2203 from sedefsavas/encrypt-ami
a054fafc3b84dad0940b8e3acbeea8feafc18a59 Add presigned url to copy snapshot request
22d7d92614231ea1db2209ef38868345cdf0d424 Use aws library for pointer conversions
115028be7f1cd87e1c9e96c04b44418293104d8d Add encrypted AMI copy
882291c4e0ab7fdcf7eae8b33c13d472688ec78f Merge pull request #2204 from sedefsavas/sdk-upgrade
2c1f27da4f7a2a31365772d85930f033467bcd19 Upgrade AWS SDK version to 1.36.26
1c74097b98bde94652347ff1040532445b197030 Merge pull request #2198 from sedefsavas/CAPI-3.12
da9aa55e89d4321171fc8fac163cb4ae651afa4c New AMIs for Kubernetes versions 1.20.2, 1.19.7, 1.18.15, 1.17.17
8b6b7f8d942d444e711db9268831f340ac28e442 Add instance refresh preferences
84ca10479f2a6db8d59976e76da7ec2ebcc280ec Add instance refresh condition
3a1150914b2d9dbabb159db6472f97538030895e Check if there is an open instance refresh
8b8581b7e367f66e43ff4059fb7a4d8a785e829b Merge pull request #2199 from richardcase/eks-e2e-fix
4a0f9d9b9f6ae01f05e59e465ca11e5591a2fae7 fix: updated the eks e2e script with lateset boskos changes
b9905e043c888f72f144e284f95baaac486970ce Merge pull request #2188 from richardcase/2179-eks-e2e-failure
a9ab4b72f7f320057fab3b8aa051a452bc821910 Merge pull request #2187 from richardcase/eks-console-docs
8b95eacd948d13e0151c107ddd12b9ffc6399ed2 Merge pull request #2135 from randomvariable/webhook-tests
39ef2227356cba24abe7957169f6a7adfae46b12 Merge pull request #2101 from SanikaGawhane/sg-boskos
1fd6a9b9e1f1301847645a278535f2c4e5af2c7a Merge pull request #2194 from sedefsavas/updatetemplate
9eacc04cf88ad45819231cc6c6175c0b4c2cbdb2 Merge pull request #2184 from michaelbeaumont/lt_cleanup
d67e98f3ca1b1f7431f8b88cacbb5fc65bb83a26 Merge pull request #2197 from sedefsavas/mp_instances
14c924dc5426e2d8209bafd73b9545e5562fecad api: Fix OpenAPI defaulting bug with secrets backend
3e0ec6aae1b306404c7153ff9078f5a6d3e6e21a testing: Convert controller and webhook tests from fake client to envtest
e7d104f765ef5bca05f7460c8abef7409825fd5d envtest: Create multi-package envtest helper
b02b194a75730d4df97a2d69937c100e5e0ce67a Upgrade to CAPI 0.3.12
dacb97214a2223daf3e394be9eb377a4606783ae test: enable upgrade test and improve test stability
415fe086cd806b793286fa7d53524672c39911fe Add instances to AWSMachinePool status
22194000b70fa8bdb34af7beb8f7ed50ca9805de Merge pull request #2112 from sedefsavas/2041-copy-ami
c6bcf3d8ecc91170595d9cbe199c9ce306a30954 Add UpdateAutoScalingGroup to controller IAM
1dfff6e861779c7546f6605e316cd04d8fc58359 Trigger rolling replacement upon launch template change
6e5c71ca7c1b105fd3521c227502719968ee0a96 Merge pull request #2190 from sedefsavas/newamis
256ddbbbc60ce7c0f0b6ed8f67ab84303eca0e2c New AMIs added to the doc: 1.17.16, 1.18.14, 1.19.6, 1.20.1
935418ad3948d3629a47f2d50db46e557f37503b docs: eks docs refactor and added eks console docs
2c0e9ddd78bbaafa3e8099fec79262ff4fde474c Remove unused ID field on launch template type
da8c0c4539a2aaaf64f570d95da7596d2bc683d0 Merge pull request #2183 from richardcase/2177-leader-election
a3d1948feb2fc704b4df5799fd676c09930e6adf Merge pull request #2175 from richardcase/e2e-upgrade-changes
68b277e1b8913dae1964cfd127a8f7b8cb6543cc feat: added dependency check to control plane delete
a1cbce63ea37d4e830b0d0c75b0199f3395e16cf fix: updated service account for leader electiom
30d870ec085c498df7ed30476a12387c4233e0d0 Consolidate BOSKOS scripts for CAPA
2afe9e17b73f1194b85444fe1f7ed3542810e6c7 Merge pull request #2168 from richardcase/1907-eks-e2e
9e1e24191c485fe76a682ca4b80ba618c2702590 feat: added explicit cleanup options to the specs
a75251b9bfec9d5f87223c87958bfbb9fbd2043d fix: adding required permissions for machine pools
78b5794ce2f8f629b10851978127afd368f266bd feat: initial EKS e2e test
bff3543f25f6316358e1e11f11492b594a94b168 Merge pull request #2164 from sedefsavas/amis-2160
a5a138154d8cee28011c403fef60c7fa9c44434c New AMIs for: Kubernetes version 1.19.5, 1.18.13, 1.17.15
e1fd3ca87e0b3445d17d5aab877d5b90046dfa5a Merge pull request #2159 from kkeshavamurthy/update-doc-links
16f13f3baca4bd4e6e6406f97a2dbf42285f338e Merge pull request #2163 from randomvariable/elb-npe
334a0b45997e0b8e3524486efed6975149c3c7a9 Merge pull request #2161 from ncdc/ncdc/emeritus
3e8a57696c80013520eb9084a73b81e907736f81 loadbalancer: Fix NPE when comparing load balancers
081e1adc9a97e68eb6f08cbb4ad5cb1e1aa49697 Move ncdc to emeritus status
1ee5b46ea3b76d0f9344f31dfd914faac044fb92 fix broken doc links
4eef0b74534d672314cb05d1779c76e514f2aed7 Merge pull request #2154 from sedefsavas/2008
14a94f3c48fd76d298121b6ab517ccc9d1a2bd5c Merge pull request #2151 from MarcusNoble/iam_role_controllers
d616e9f80dfe912cb1db552fbeec3fcf5f05d35b Merge pull request #2149 from MarcusNoble/prereqs_docs
6d254502a7e4ade3982ae4c926bbf5d45809d373 Updated wording on prerequisites doc
a45e9f0b9e66b8ebcbf7e69c0fa471bad4162da8 Merge pull request #2150 from MarcusNoble/patch-1
08d25471ae79b30861fdbb603ab33bc8aa115188 Update amis & eks links on capi book
46f8d56f2fcb8037815747e632e1a341f48d2637 Merge pull request #2077 from randomvariable/clusterawsadm-shared-config
ce719427af07ed8cb3fe8f8657200ffbf6532c00 Error if a loadbalancer exist with the same name in the same region with a different scheme
d269842417540c49cffa82a754187d73ffa21e86 Merge pull request #2147 from randomvariable/clusterawsadm-policy-configuration
7b4c169d645b45015aaca13038e850fca0a2567e Merge pull request #2031 from randomvariable/rationalise-owners
fc4628d8b9300b0005d53a3bc6dd6d60a022ac62 OWNERS: Promote Richard Case & Naadir Jeewa as admins, add Sedef Savas and Dane Thorsen as reviewers
32dfebbeeedbe40a7961e3e6b5f8412dc381de76 📖 add config example to docs specifying IAM role
42f6a3e2bc3373d6e11abdb6c691ed59bcc14d44 📖 fix emoji display on contributing guide
51f466e9aa8cc6a40d43c1c7b58138be041b20b1 Merge pull request #2140 from MarcusNoble/awsmachinepool_subnets_optional
576f0cdab3eece5932e778a5dcf42f0d3957f720 Merge pull request #2124 from enxebre/decouple-external-infra
2889ae4f1cfedeacabe12092dfe8d47ef2593987 clusterawsadm: Allow CLI to take a configuration file to print IAM policy documents.
5437038ce7e26e8e65d249d4f3f363959893c388 Add externalInfraCluster
947d0126e9fde6c079a5fbd245879e94ed6ba723 Set Subnets as an optional property
1cfb54abc2dcaa6b841753495879d36b1bb13f76 Address comments
14282e49eb41455bc46a008ac2478586fce7b053 Merge pull request #2100 from MarcusNoble/irsa_management_cluster
25bfe12f550fd59500681df6fa521fcb3996eee5 Merge pull request #2126 from richardcase/2078-packaging-adr
f37b4d71e04d0cf3ff364b5c309ab6436f6c8c23 Added comment regarding use of drone/envsubst
2286bf7a3e21b14950732aaf73861f77f46f517f docs: EKS packaging ADR
7de342e215f8a91e67675ced6465376ae4b1fc57 Merge pull request #2120 from akash-gautam/machine-status-interruptible
2aaa967eb722797ed5d803ec425318677df84123 Merge pull request #2103 from cdenneen/patch-1
8d25426e21e71d66aee59c2af8377c2896ad387e Merge pull request #2133 from sedefsavas/fix-bump-capi-311
0a08b75a3f2d3e02d9c72c0f60fd315502ee7aba Merge pull request #2127 from richardcase/e2e-refactor-adr
1b21f3ef2a8c5d3cb69d944f301be40b20ef4fa6 chore: incorporating review comments
e99f6eb31ac7d0419222593223ccd5c248991024 Fix for CAPI 3.11 upgrade
aeea340c04fb7db82c9823786d8a7a2c39e53e7b Merge pull request #2129 from sedefsavas/bump-capi-311
61471debf11e2ab93735764b4d6593a66d274f62 Bump CAPI version to v0.3.11
7d66042f0135c4a3a3e1cc43fa666cbbfeb08ec1 add function to restore AWSMachine status conversion tests were failing for AWSMAchine type as the value of Interruptible field in the AWSMachineStatus was not getting restored after running a part of the conversion tests, a function has been added for the same
0bd2e39635d26ebe7b1b792b8c0d5dd65473b857 add Interruptible field to AWSMachine status set Interruptible as true when SpotMarketOptions for AWSMachine is non-nil fixes issue 1899
07601c3cb936bcc6822c64a7cc7fc1b7cf31d3c1 docs: e2e test structure ADR
f9b3593c998fd9896c7a79ab41d9542fd98ea6b8 Merge pull request #2114 from sedefsavas/upgrade-e2e
3feaac9627d3999f367a7c896272f1e7b7bd1ada Upgrade e2e kubernetes version to 1.19.4
056daf78c6b6b22d06861a31da84dbd14c983445 Merge pull request #2102 from richardcase/e2e-reorg
ec8626b237941bd6f0373a61110ba9e1450f5433 Merge pull request #2111 from randomvariable/admission-controller-update
20d737f9fa2256051dd58ff27aa3144087a64441 awsmachinetemplates: Allow cloudInit.secureSecretsBackend to be defaulted
e61516f73f0f1ca68d351124b3ab311842b15899 Merge pull request #2113 from sedefsavas/delete-terraform
42e832a3c95aaac099aa7717121f95fde4b04a30 Merge pull request #2108 from felipeweb/fix/asg-event-msg
4593e5523c3a3925dece915127a83f8f4e14ca60 Merge pull request #2109 from sedefsavas/2309-amibuild
3c15d75e7784b18cf37a04d63d78c3f9af437d07 Remove old terraform testing scripts
590cccff3c6e08a17b5e37cfe6b527eb2c422a31 Add copy AMI command to clusterawsadm
b1a5f396f94007d546eaf724f15709b0164fe695 Changes
9f473ce4a4d689f5ee20611736ad747f5804e6ae :sparkles: fix ASG event message
7ba281ae9fb78e30dbd968b7a15f65a4fc01ab2a chore: removed duplicate session code and tidy up comments
25d964635257b5b34430b9b5fa250982a47ca152 feat: added data-folder flag to e2e tests
af208b348f5a8612c69224c72f8749784a1008f1 rerfactor: changed the structure of the E2EContext
bda67f14042e61f96897051d1df60f2c9aee62ff Update consuming-existing-aws-infrastructure.md
ca94c4ee857fe462202e33b7fa18ef7f427c9faa Update consuming-existing-aws-infrastructure.md
e426a306d07049f0a8ceca69c122943d6f658149 refactor: conformance tests
99759fd01ef6be08f7433451c60819b3d6162d92 refactor: e2e tests structure
077b4a2698e161527b748452dcd83a89a5458e39 Merge pull request #2072 from arghya88/validate-filter-in-sg
7636198fe52197decbdc13b371d8c301577cdaf0 Merge pull request #2035 from Evalle/ISSUE-2001
b927a331c5a290f9d8ce0b6b2bb496cbf466c43d Add support for AWS_CONTROLLER_IAM_ROLE env var
b7294cef139c2642036592489e431b0fdf5bb59a Merge pull request #2085 from michaelbeaumont/cluster_key_name
d3e9e7b35c36ced61f819087f9afc040631e23c1 Merge pull request #2098 from randomvariable/test-manifests
a956f22f02af220d75adb5d10e7116800a1bdd36 Merge pull request #2099 from randomvariable/revert-sa-name
4baaad945dd53b3bc2be1ed87694b44c40f4e048 Revert PR 2052 as this breaks the release manifests
c16762b2c53dfffa90d24e1fe450948cb696b574 Makefile: Ensure manifests compile during verify
f93d6b8691ac20a80992aaabf46384d708698156 Merge pull request #2094 from seemiller/update-changing-creds-doc
3be6d795f347e12aa6384fb07d5369dd9e2adf9c Merge pull request #2095 from MarcusNoble/fix_update_asg
eccb0255825dce61ef513591b63e0adad2b81236 Merge pull request #2092 from newrelic-forks/ownerref-group
fd8d960a74d7d2ce1e3310407d92a9e13d8fcd17 Fallback to cluster subnets on update ASG
7f22366fc90a5439d8c31dc9fa06be6bd7dbd7ac fix ownerref group on kube secret and configmap
e526925b25ff006774885d129a16de6da504f196 Merge pull request #2090 from sedefsavas/defaulting
93f543c6d37f7ef5b199bace34cdda64bb5d642b Add cni defaulting to the controller
75951d2d07c1f3905c5366f7ae676f4a8d9e6bb7 Update docs to use capa-system namespace
389375cf9038c89c5e4d488c733393ca704cb4d5 Merge pull request #2052 from MarcusNoble/iam_for_service_account
1824003534bca8a4c65c806ee6ff62d9ce91cd9e Add EKS cluster name to nodegroup role name
e41b80fa920272f15a8e623573229eb6f2cb8eaa Fix usage of cloud provider key and nodegroups
2e24bd127d875995ed13699966e60b9e12060cb2 Merge pull request #2082 from srm09/bug/fix-awsmachine-defaulting
627104a4affeae6a47b7b5b4b8e91a90a83960b2 fix:validate filter in security group
9f13448a70c47c6bb87874d27ec4b91b39ace9e8 Updates AWSMachine Defaulting logic
55825c3cb8a5fedddace8dad8a6c974b051894dc Merge pull request #2080 from richardcase/adr
4da8b88e0f9b5a7a76020465c6e4d786abd7c585 docs: add ADR template and first ADR
2eae68dc405545193daa29cf26325a83e03c2e6f Updated iam role docs to cover kiam/kube2iam
4cc2f4fa5a7bf1673033c1cf13fc47e8205846b2 Added annotations to support kiam/kube2iam
9a92b0c807ccf24937c5a08fa664aba897a283f6 Merge pull request #2051 from MarcusNoble/asg_subnet_fallback
827cd48dc874217e8079053bc77c8828e46f350d Merge pull request #2071 from arghya88/regesx-sshkey
1f3161b6c02e85f0946fcbaa318f00527f9a2c1e Merge pull request #2043 from richardcase/2042-managed-machine-pool-fix
a25a8be6c8d6e8b54c48e9d0420ecdec0b19270a Merge pull request #2074 from sedefsavas/conversion_bastion
b5305c1e1d86b5fff27166b698204a47c0dbea00 Added docs topic for specifying iam role
2bad6d8b536c1fa05034ebdc68ce59c1baf66414 chore: review feedback changes
6311b3a7fa160446fafffcbeae29ba958b210495 clusterawsadm: Enable use of shared configuration file
08f2f0d329a3943c8e66782ce851702c69e37219 Some fixes for conversion
40026657b1787b633838cf75b385d1bc2fa129f2 fix: relax regex for ssh key file name
16b269fee8d6227dfd4aa717f2f3e4e11896ca56 Merge branch 'master' into ISSUE-2001
dd85f96f527b20a1bb8250ff04e895ce1539f850 Merge pull request #2046 from richardcase/2045-machine-pool-register
b3f23536a603e6b2c4c50e238ec025c548c99a8c Merge pull request #2044 from richardcase/eks-docs-update
e46428dfad1f64326b774b1ae4a7fc4f8f91d8e3 Merge pull request #2068 from spectrocloud/Ticket-BET-1306
1b9f5f1f87d8da60e8bad7774ae50397bba1bf19 Updated Bastion node OS version to Ubuntu 20.04 from Ubuntu 16.04
d3212930c4faf6bf9f8bddfe477944c73f71bdf8 Merge pull request #2018 from randomvariable/rebuild-amis
a7811256393626f35f7f03fba5930885a0f0f8e0 Add conformance template sourcePath to e2e-conf
16515f764e272018be1cf0a56c2ea7c64468a508 Merge pull request #2049 from tmaxjmc/master
b9889a762de0b3a0385fbbc3aa14084d031adf52 change env var used
6f33bcfbd3b347cdf42cc75c22f0f1544a058f25 Added service account as patch file
f18202e2b9e1465687f98725989f98719b96578b Add support for MANAGEMENT_IAM_ARN env var
af08074939849810eb31831b9928a5115e90486b Add fallback if subnets not provided on AWSMachinePool
961b49fbda98cf000066f078399ebc39a6b5cfd2 fix: add more condition for resource's status filtering
32d082c9a4803d72ed80941e151e2674b434c4d2 fix: ensure env var enables AWSMachinePool webhooks
fefbb697fc75a77a59c73cc84c8be5f8d45f70e2 fix: add required iam permission for managed node groups
04145f03fd906d33cf7457cc519adeb969c0c002 docs: eks docs update for managed machine pools
98cc901a538466fb6ce0133f0b7667ab2a090e9e Merge pull request #2011 from shysank/fix/1838
e9ed728307d2a696e777af5f736f2d2f1def5123 Validate subnet's az with failure domain when subnet id is passed
8a56802a0ae3fdae95c1c5839b2a62b5ee663761 Merge pull request #2030 from richardcase/flavors-release
d06b3fc616ed3e0fdbb7f139f209ddf92e74c89e docs: updated flavors and mavhine pool docs
f723ffced8a24de4fe9745c5866cb37dc4bd141f Merge pull request #2038 from kkeshavamurthy/eks-typos
6a44578a2edcb14f1b6f8cc363894f608a15c324 fix typos in eks commands
a229052b19a7b4d976f312a6bf6a42a9ce09b5d8 Merge pull request #1924 from Promaethius/ssm
f9497e20ac0e564de479f2f5dc0e967bff750310 Remove unused allow additional roles feature flag related code
6e4da055615983cab9a8e9eeaf8175d3d3d6cc91 Support for AWS SSM Parameter Store as a Secret Backend
3027a63592d8e605ef1b07060da951c6a050b928 Merge pull request #2013 from michaelbeaumont/bastion_eks
f6a97de9ba98338e58bf1afafb71ece60db5b394 Merge pull request #2021 from newrelic-forks/dthorsen/machinepool_tags
0987c8d9f16a4f891d05a622aa92b4592ad5c154 Merge pull request #2015 from shysank/feature/1840
08a886cc60697cbddc7791682457b2dde2ea4547 Merge pull request #2005 from spectrocloud/fix-description-for-volume
4e438203db282f52668ba44ff2c10b1908526cc9 Merge pull request #1978 from evalsocket/fix/1668
371edd7252fb698b7b97fdd3153691e4d63f1b4c Merge pull request #1863 from newrelic-forks/machinepools-docs
f15e996decf0e62bf955e1c0624936e0dfc1dbae Merge pull request #2024 from michaelbeaumont/mmp_flavor
32d06c8b8f8e21898005a9698f2777da66d2b0b3 Merge pull request #2006 from arghya88/defaultcooldown-asg
d91ff17c55c52128eafcfe9e65e90ab7614ebbbb Merge pull request #2000 from shysank/fix/1986
3f45fa79d11ccf0be663620b373ba31df85fa839 Merge pull request #2028 from northrup/docs-links
863a37b0e30fb2baf9cc4a27d251ab94ea0a9e32 Fixing link to docs site and moving to top of repo README
9ed16052d249701042f59bc61729a1b5f7f74d6d chore: add machinepool docs and flavor
78fbded815855af15e23ffb83c95ebf0c735b123 Add AWSManagedMachinePool flavor
b1b486639e1b2cf9d2c97ff3a4d82941d214c210 Remove machine name from buildparams and move it to additinal tags, some minor refactoring
488cdafd01df825e3a56fd440c54baf2518db296 Revert "Generate boilerplate exluding machineName"
c6d62a2eafc5861a1671153b06a48a4f1d50b024 ✨ Add tagging for AWSMachinePool resources
7a2eb53122ed67bd1ad67a3fb5d5b55c63ba1b6e e2e: Ensure CI artifact template is registered for AWS provider
b71d280bac01cf59bf1be2e66737684baaab7d31 docs: Provide AMI IDs for rebuilt Ubuntu amis
28800c8339350a4d9036ebc9b71a35a6107261e3 Merge pull request #2017 from kinvolk/dongsu/eks-fix-broken-link
4b6e94f74dafd7ace49bf3d15387e7f7cf943fdc docs: fix a broken link to prerequisites
ba73d6de15e25917646f3458466059169ed8cc4f Add support for DefaultCooldown to AWSMachinePool
83fc261ce94bb5ce4a9210c40801ae4610573dc5 Generate boilerplate exluding machineName
618dafd7399286ad9152c2ec3086273d43b327e4 Improve AWSManagedMachinePool remote access support
0b9cf5b36bf4f7f129d0323b1d53f77f6d0a3916 Add machine name tag to instance on creation
2ab683dc9b765f8e76117a7139907c5c26f051c1 Merge pull request #2014 from michaelbeaumont/npe_sc
80fca0480e69080456a98cb85e4c6f6d2a03bf85 Fix AWSManagedMachinePool NPE with scalingConfig
d913dd7babdc13102622ea26ff6d3da62c763c14 Merge pull request #2010 from arghya88/io2-ebs-volume
be973da1a63b79b583baa433cc89173dadef5a89 Merge pull request #2012 from fabriziopandini/remove-integration-test
859a3456a6558e33da14f01cd95065d9ebc4244d Remove the integration test
03b96cbb8e55c6c8525a9480b0f77cfbc794e64e Merge pull request #2007 from newrelic-forks/fix-mixedinstancespolicy-panic
951395b312df7d7f24498ca043f811801793f034 add io2 as valid ebs volume type
49cd179e5de2baaaf0b4c70ed74fe84abbab812d 🐛 Fix AWSMachinePool panic when MixedInstancesPolicy is not set
2d0eb5fe6bccb82738d87232c4debf570a70ddc5 fix volume description to remove 'root' since it's also used for non-root volume
22d7ab8e8f9857ccb3c21027928ec9a31e4e7458 update openapi definition
3338cd440bfdcdcea4b7f7903c65136386c0490e Merge pull request #2002 from randomvariable/updatedockerignore
4cf41c2ffe6ee0904c2a9368f889f09e024c9164 .dockerignore: Add cmd package
e042503a799294e0002d64d057113cfb27f21121 Merge pull request #1995 from richardcase/1850-add-iam-roles
ec01c50af659157dcb489287cd89d490ff14dad7 Merge pull request #1916 from michaelbeaumont/eks_nodegroups
d2b61b710e9d2d390c33b22c7b31cb80cb9cd4b8 Merge pull request #1991 from randomvariable/e2e-port-to-capi-framework
aa18f97344f9b4ae23d3b57c50f16bae69c85926 chore: generate config to fix test issue
69483b04e0a84e16e746fad4a0dd9421bcc27259 feat: enable additional user & role mapping for aws-iam-authenticator
02ffb61f791266b51900241958faa397e16e305b Add comments for VersionNumber field in AWSLaunchTemplate
3c6dab8f73ebae6544c359bc1f21378269f65611 Reconcile AWSManagedMachinePool on AWSManagedControlPlane changes
e6f3effbae96842325e90d7e84316edf17d60405 Add webhook for AWSManagedMachinePool
b4d782bacbce3cc892fd714c8ae3d761b7fb8966 Add default EKS nodegroup role creation to clusterawsadm
3023f16ecf8ca2f0e8707898d04e7f2c0b8e61e8 Add conditions for nodegroup deletion reconciliation
78962cfb9bb05bf42168f9bd765b58f67b60d2be Add AWSManagedMachinePool reconcilation
4e5d22793b74ec16ea08d76783b3d17fa41a3fdc Don't fail control plane deletion if role not yet created
130dd5ade96d80279ccba28c6e2a8ba579639bf7 Refactor: reuse clusterawsadm types for IAM in service
e3230f382aad1e058ddd49149995ade732d3f975 Refactor IAM handling
25226ca60b6a9ebb9606aa9769e51174a1c2e236 Merge pull request #1997 from richardcase/1971-eks-docs-update
f188e8378adbf3a55e84506a4979297fb2a28fc7 Merge pull request #1998 from richardcase/eks-type-fix
f1f45b68591f7a6b682eba36dc3c2f40e72b51b1 fix: incorrect capitalization for eks fields
128ec94592de79707fa2b3c603448625644ffb7d docs: eks docs updated in preparation for 0.6.1 release
80ddb77ca095ed70ee087c0207d29e09c28d07f5 Update dependencies to Cluster API 0.3.10
b6abc662bfd153f05adea98b714d15e7ea605e92 Merge pull request #1996 from randomvariable/conditions-fixup
77050ffb1821d0c9d257df7bfe7b13a7081976fe securitygroups: Fix NPE on cluster deletion
2ac3fb9341318708857790cc6c97b38f57dc8d52 Merge pull request #1858 from Promaethius/master
5643eaf096c7e3b70991d4629ea836c5aa9fce52 Merge pull request #1994 from newrelic-forks/issue-3631
1dcb333449d2509cd4a52aeb03d86bdf87e4fb7b 🐛 externalManagedControlPlane status field should have been optional
5968d9733484cbd8869992cb7db12642ed812aad Merge pull request #1974 from randomvariable/update-amis-late-sep-2020
731f86ef4dcfa956551f92083b7e4ea6f3eade55 Custom AWS Service Endpoint support
47e25941afb31c0d01e851fff50326dd13542788 Merge pull request #1992 from newrelic-forks/issue-3631
ba286f8ccaa03dfa5f1ce8821eee6ac30deb5c62 🐛 Add externalManagedControlPlane Status to fix node drain under EKS
666ec157c58e8507907b86ae2c2e6f72efc13ce2 Merge pull request #1981 from randomvariable/update-topics
bf1d9813ba54c0ddf0283f77bf6fae3e94c4a184 Merge pull request #1963 from gab-satchi/1893-spot-instance-e2e
8da0cb5414c159c144f45436bce3f5185e7daa4c Merge pull request #1860 from newrelic-forks/machinepools
f05273a53b2d0cfb8980ca5574879880f5cfdb37 added awsmachinepool controller and types
30484058c1d530861c556a8f592772addb543b50 Merge pull request #1962 from richardcase/eks-nodes-fix
798dbd8dc14eff2f4bc67c68838297a7fcbaabd7 Book: Update published topics
edd33f22726eb7a2acc9f9a776a7913b7ff0ec48 Update AMIs for Kubernetes 1.19.2, 1.18.9, 1.17.12
ba90a46a910dff3ae70569e27ec3b35bf8414890 fix: issue with enabling IAM role creation after control plane refactor
1f72530eee16fbe6e5c72b6a2907300d87aa9d20 Added validation for SSH Key
518c7b861629ca0459b385f88454185dc288e740 chore: fix failing template tests
857c11a99e42651203e0a327a30ea652cebeb4f8 Merge pull request #1947 from randomvariable/netlify
afa683363db95677744ea70628dd33eb034cf56d refactor: eks configuration for clusterawsadm
369be697095b1e974f9fc4256203ea21771ac95a docs: Move docs to fit book structure
ad25f40e9fd0725ee9637f50e5f9fb4b4a6b10b2 docs: Add netlify configuration
f1858480b42644e0161756d871c5bed5da98b338 Makefile: Refactor
59ae34c9a309e92b330d4c67ba8a1203de7797b1 Merge pull request #1957 from richardcase/bastion-fix
16e6e7a48041d17e39e0065ccc9074bedeebe889 Merge pull request #1973 from michaelbeaumont/patch-1
8b229b9bcc17fa74ef5741aea9c251899a76443e Merge pull request #1905 from fabriziopandini/reconcile-delete-conditions
b65e27259ab65f946d801ff40401e6138e18f441 Delete webhook_in_ekscontrolplanes.yaml
6ace9ea49297e31ddc64ceacb91cb5a077442721 Delete cainjection_in_ekscontrolplanes.yaml
be9ff9392f97a2f9918c9f4042632daf4c5123d2 Remove patches references
3a6ba5e1655d48211cfa19bf4d70396ae146b36d Remove from /config/crd/kustomization.yaml
c0178c04c605d4fe05f1a69f7c48d433ceeca7b3 Delete AWSManagedControlPlane CRD from /config/crd
7e646ebc014402ea7ed2bf851d40d3bbf4bc25f3 Reconcile delete conditions
3a4a0a4969ce3d2fc00e2eaa642528751f93d189 refactor: created new iamauth service
e7dd4e454c7915c5b7f0960d512926744b5dde0e Adds permission for the controller group to create service link role for spot instances - e2e deletes any existing roles to ensure the role adding ability is exercised
a372127f137a03e411c279dad8c037a3e7292e3f feat: fixed iam auth configmap and removed old configs
33283b6aea8c34acdf45d46549197fd0f65a4fea Merge pull request #1966 from randomvariable/bump-cb-eks
d5fe0148dd2b921716089618e973d01546a22667 Bump codebuild for eks control plane
d2f5f140dfb9e779511f075814b658d13b6c9f79 feat: updated clusterawsadm to enable EKS node permissions
713d5b9ff6b48c9e3fae0dbf6c855ce069dc7433 Added conditions and changed the rolename
779ccfa602e0f023ff9abaee8509137ac29cbe8f Adds e2e test for spot instances - uses framework function to fetch machines from machine deployment
d9a19b12f027d9770be052032b89a4fe147c4c86 added code to aurnticator reconcile
a2f1d02a6b12d7591f15a013eee229a428cec406 feat: added configmap and crd backends with tests
e5e025e98c8dfcb4dcab2c69577a500c436677ee Started to add aws-iam-authenticator support
f68af29e95e5260b51166b2650a90cf215f55fe7 fix: added new security group for eks nodes
b7dd877d1f179a938ca8997c9ce2b5cb2661d124 fix: bastion reconciled before security groups for eks
c2c54cd1b7abd843d74a8098f8aef90eeb5364ad Merge pull request #1918 from randomvariable/richcase-owner
c098bef35d7931714ed7d7b1fd678d7ab4eb31ee Merge pull request #1952 from gab-satchi/1935-vpc-endpoint
9f95d2f90fe4b929729d6be9d14986d7f97e0970 Merge pull request #1949 from richardcase/extract-controlplane
c8993f716d99ad601304c40d711fc07f99565111 Merge pull request #1960 from lxlxok/master
828c101f73ca2deb6d808b5cd856fcb9590728d1 fix docs for creating a EKS cluster
972a982f43dd2fa2119a3b184cbc152eb8f46ff2 Merge pull request #1953 from varunpurohit76/#1429
4ff8d434d2a9493630e72452c7b4b96edf71e283 Merge pull request #1950 from randomvariable/bump-cr
2699686f46e68c86164cd95303397a846d65e6d1 refactor: changes as a result of testing and updated eks template
7b211c5d54d5175f810750d73cf43e62f42e02f7 added compile-e2e
d7fa4245b1ecbd0c4987932cff9b5ffc53cf563c Retry with listing all ELBs when listing by tag fails - creates mock resourcegrouptaggingapi - deletes API server LB directly by generated name
68eda9c2b6fc76d60240e58a7bf0c2af59d85eb2 docs: updated eks docs after refactor
7cf22f8745b39e75df18da8301ffdff484997c3b Update to controller runtime 0.5.11 to resolve memory leak
61a11ade155bb7912bdc440ccec6a43fe4b6bf3e refactor: split awsmanagedcontrolplane into new manager
0a86de52d438eca8bd0378bf7121294c2b6dcb00 Merge pull request #1948 from scottslowe/issue-1946
27c6c9b4f5eca7fb750522ed35d45d93a3f40384 Add docs on updating AWS credentials used by CAPA
ef86e8130357d08d541c66b7156466bc466b985a Merge pull request #1944 from randomvariable/bump-golang-minor
27fa175dcc2a58d3955122d32c544629154ba2be Merge pull request #1884 from andrewmyhre/1696-dont-require-public-subnet-when-unmanaged-vpc
086a468a6b3ee55e94279d4d396ab2b4ec9b233d Merge pull request #1932 from andrewmyhre/1728-ssh-key-name-not-correct-in-some-cases-master
d827e7a50f0b473f322389b8cc6afb62fce11fb5 AWSMachine ssh key should defer to AWSCluster when nil
13617fa198118cf8ffbcf252584da15a23445dd9 when reconciling an unmanaged VPC, don't require public or private subnets
ee5f2c9a80b53ac5a635bf7c271c6034e4abfcff Bump Golang version to 1.13.15
3262074d336c808f498c110fb98009f5459f0f8c Merge pull request #1943 from richardcase/template-name-change
5ea0cef2e9941b0cf2cb6a82f3723a79a20c9fe5 chore: changed template name from managed to eks
d6ec06aded09258e1093e10569cfa16326ef617f Merge pull request #1938 from randomvariable/eks-makefile
769f5a7a09adb16ebee156142292e20a287d36e1 Merge pull request #1880 from jayunit100/patch-3
1d9f63f4840ef23ce1868cb648b8c300b7b045b9 Make the VPC error message print the offending name and hint at possible rogue capa controllers
15fc9fbb655b28c23d09892ab9c542347a762a41 Merge pull request #1939 from richardcase/release-docs-eks
c25e2acef6252468905771863ddec8b6579b1a92 Makefile: Fix code generation for mocks and EKS bootstrap provider
fc47a784adf1707e98c54f05f10c58e49904325e Merge pull request #1816 from sedefsavas/e2eCNICRS
5d19ad4bfa70e8101a78ebdb0c852cb577236c7a docs: added managed template to release docs
a22b62aa43d489a927dafb49da8b593d0a70442e Merge pull request #1936 from newrelic-forks/fix-eks-machinepool
04d054460c9652e020c9a4c919dd6ab9f498e8f1 Merge pull request #1915 from gab-satchi/1906-default-subnets
4691bd47d09899cc1d78f9fd077ac1cadf620050 Merge pull request #1928 from randomvariable/k8s1165amis
639c3a36c380940b07391e1bc09515840ea765e2 chore: generate bootstrap
66b2922ebb0f60e153b5a988eb72871e476d7370 Merge pull request #1937 from randomvariable/tag-instance-test-flake
f7bd4f3a738ab29187b4c2f5e78309d9e5f734c5 Update AMIs for Kubernetes v1.16.15 and v1.19.1
679ddb2ad3d5dd0f544d8ad18b1d2915e84430bb instances: Sort tag keys so unit tests can succeed
a24331b84d865c4f1e520d84d6d8d8f87a3a5652 Persists changes to subnets spec when using default subnets
28d01d064cc2e5b0286ae23b3be7203f18b00447 Merge pull request #1931 from andrewmyhre/1180-byo-control-plane-subnets-master
bf36f72aa31d7e9caec5e653b5e49918931dffef allow specifying subnet IDs for control plane load balancers
967b39914dcdb99c1f30a8b2c87ac92f83529ff9 chore: add capi exp schema and fix manager args and rbac
437361932cd4cae010c6fc351b5f616f84fd54c3 Merge pull request #1926 from alexander-demichev/instancetenancy
57513adcae14739a9c66628ced8055fccd908a66 Add tenancy to instance creation input
3650deb044c30c0c8ce9638899ca7c2b67486c51 Add instance tenancy to API
6feb5867046bbfdc23fad872b938ba890cf0b90b Merge pull request #1920 from gab-satchi/1887-aws-sdk-bump
65bfb07b196e8145c900b8bd92cc832c58237f8e [e2e] Install CNI using ClusterResourceSet and bump CAPI to v0.3.9
f98b7a9fba63a2d120a52172c0c1272341ab7c09 Merge pull request #1930 from randomvariable/capi039-revert
7f5fcbda0cdb0a4472ae606c70cf789cdda782d8 Revert "Update to CAPI v0.3.9"
10653458265a62634129bcb6befb8a3e3fbda7dd Merge pull request #1925 from richardcase/eks-default-role
706fb4f7932ec79258cb650362e65cfc240d8df2 Merge pull request #1927 from fabriziopandini/update-to-capi-v0.3.9
9f578d4b1a85025ff0efd282b9577fdbadb28238 Update to CAPI v0.3.9
51bef78840096f3be9c79de1955a25e4ce4b15cb feat: default iam role for eks
745dd0576b256446d07719fb6322f5cce30e902d Merge pull request #1922 from sedefsavas/clusterawsadm
0f3aeff5f800b2fd3a984e2d50402bcfbf8e45a1 Fix clusterawsadm policy mix up
50e655b69395c243827441052371271ad57d2368 Bumps aws-sdk. Creates tags during route table creation
29669bc5ba049d1d1aaa0ff9c25c853ffd0fb3fe OWNERS: Add eks maintainers with Richard Case as initial member
cce479392cc19055b47a72a0109a0cc46a786990 Merge pull request #1917 from scottslowe/issue-1898
aa8c2138e8e426be3c06a95bc5021b56a15d4f62 Update prerequisites doc regarding bootstrap user
fe6975159029237bd639825b7fb8e09f64cdd0ab Merge pull request #1914 from richardcase/managedtemplate
90c6c9c38bca52a844658b20de9ec5fa521cb429 feat: added machines to managed template
3c18339c46661300bdce5451be950c2d4a8993e3 Merge pull request #1913 from michaelbeaumont/eks_tilt
7e29d10cdd6f4eaf964088f22897583076709f08 Reload tilt on exp changes
90cf5f8d7d6ba15adcad88031cf5a25108e661bc Merge pull request #1904 from randomvariable/update-e2e-tests
0dd4489f9ef970808a61aaecb32141a15ea7b15b Merge pull request #1910 from randomvariable/fixup-cloudbuild
7cf6e0bfe2ee04794f1b6d5c08938f49d0724009 Merge pull request #1909 from newrelic-forks/rudoi/eks-awsmachine
03c8851f4e1e3aa912218e7db1925977665f8924 cloudbuild: Increase timeout, use newer Docker image
dc2dde0f382862a725fe8bbd9610849cb8ae5f7b refactor: use type switch and helper function for infracluster
07d4d715272c59a6d4d017913fc465cde6c10d62 test: update bootstrap tests for AWSManagedControlPlane
47534dca0b9cdfc54e9404fec22e2cd92cafc49f refactor: create EKS-managed helper function
3fdc02b74385e70cc4aab749a119d657658fa645 Merge pull request #1903 from randomvariable/aug-2020-amis
9140b6eceb33f47e894073301fda8a652cad8a7c chore: update awsmachine controller to support AWSManagedControlPlane
00ae3e9e1df93c494e67217dcc662affb214cf4c chore: look up EKSClusterName in bootstrap provider
f31a5ff9d074a03a1a69fd541b2b4e7b6e136331 conformance: Remove google containers
8a79283d967d52e058bf58f9454ae8d2140b6f8c Merge pull request #1817 from newrelic-forks/rudoi/eks-ami-lookup
8d38ecc9c457595429201585903c07e3c823eca9 Update AMIs for latest Kubernetes patch releases EOW 28/08/2020
6c7e3fd1c0000556138b2c4b5e60ebc4321b3ca2 Merge pull request #1894 from richardcase/eksdocs
6dbdfa8d20fb69b574cd6927277cec0424ce2333 Update e2e tests to latest Kubernetes release
52f33fb2fe062f4442361367b3a0f39a8f1d9088 docs: add eks documentation
865a70c4e832c042bd4b4b1bd30a34fb9e3b3ec2 Merge pull request #1902 from richardcase/flags
e7d1c8d9e33d8a02ad62f7189653cdf0fb93e008 feat: added ability to enable EKS via env vars
cf87cd15eee35138cc5dc53d32d20e4be4c276f4 Merge pull request #1901 from sedefsavas/bastion_struct_rename
c4305cc2bf44c9ba4c7d592c3d88d6a909f3d464 Fix Bastion struct field name
27c055d895f65361b4023d0d88e2668c7cda277f feat: look up official EKS AMI when appropriate
fb2723c3db4f4071ca54ae82ea5df85bf0401987 Merge pull request #1864 from Promaethius/bastionami
32edbe2bc410abf626221f35a442c4b7cf6cbfe8 simple bastion ami code
e7ffeaa46ae68c062f859ab161f58f5bec6c9d9c Merge pull request #1815 from newrelic-forks/eks-bootstrap
9bb776a1b045b490b491fdf7240e6b021c488327 Implement EKS bootstrap provider
47a619f527a5a010309d00a43170af679210526a Merge pull request #1890 from randomvariable/new-e2e-only
ce4cfde76eed3a0de7f201897b4471ca1f68e022 tests: Only use new e2e, and remove old e2e tests
936a02473d1fc68f06b88c32f0b9250d6f3979b4 Merge pull request #1724 from richardcase/ekscontrolplane
8a18234a8237fdab7dafca951f4c7311b6dcfa78 chore: fixed typos in errors
23e379cebdfddf16c2f3f3e6aa62b85cb7ad44f7 feat: removed EKSClusterName on managed scope
d1df985b8a3aa6a2a287591c886ea760e809534e Validate and normalize EKS versions, be lenient in controller
8c919d8f2bbe6ed68ad36a05f9aaa351383bebb1 feat: added new KubernetesClusterName field
fa4ad222130946471d3a63ae0b2f9d28c0e26a16 Make new EKS template flavor conformant
6e6bc41bd5c36fe34454dc1d1f55f9642be361bc feat: webhooks, eks cluster name and auth without aws-iam-authenticator
ebf3367574a68001ee05e418c7fa509a289acd0e Add unit tests, fix logging, fix log output
feb3a0b75a19fe8662d542b22726395c259ea000 feat: introduce token methods and tag reconcilation and api refactor
70a0e21bda16b71974db1ddfbcdb9699b53a772b feat: changes from testing and logging structure change
bc31df8b1a82172db3f1d82b6807723691c9f2df feat: added conditions and changed finalizer name
61b5ce0ef60483eaf10110bb75d8932698d3f04e Add public/private endpoint access support
1047d21bf83a04abdcfe8dbd151cae5178b2183a feat: updates to enable awsmanagedcluster
cfe9f2236d2d6920a3e123f47138740c134dc904 Support EncryptionConfigs at cluster creation
7ef31cd5616ef8b152295144869803985fe72d80 chore: fix issues after rebase
bccc03f39d5b8dcf2e55129988e73420226da142 Support cloudwatch logging options
f92d6490eb0502c93665d3d178b7f6ab8fdb7d44 Handle version updates, set FailureMessage
08d50ca365fe68fbbeda3976ee2c903cc3db1f32 Set status of managed control plane
2a1772ad77d159e84b4b31bc5f05aaadbbf5e08c Detach role policies, no longer need AmazonEKSServicePolicy
2b68eb62a4762d9ad77b5f8d0ee5dc4ebb664121 feat: adding eks control plane support
da7d37f4314afaf38e852bc7b7485974470cce82 Merge pull request #1889 from ffahri/add-io2-validation
9fdcc39e21ec163322050d319533cd152b504343 Add validation and tests for io2 volume type. Also aws sdk updated to v1.34.10 Signed-off-by: Fahri Yardımcı <f.yardimci06@gmail.com>
a042e87b16e09dcc6f3d112b2f29e207a4fd09a4 Merge pull request #1883 from sedefsavas/metadata
500f9c64ded95dcf7ebfdcf422ae0272a37e743e Add metadata.yaml for defining contracts
38fdfa8978edc5b37321b97138c7ddd07b64e9e7 Merge pull request #1881 from nader-ziada/annotations-cleanup
1e0bc77c2aae3a3cbab44511e402c03837f0b947 cleanup unused annotation on Machine
fae65c1847a2343e918194b734dc06da11346350 Merge pull request #1879 from michaelbeaumont/eks-clusterawsadm
81699038fbd8ce70748bc8f917bfcbce4b101542 clusterawsadm: Add actions to IAM policy required for EKS
9bd647dae7686fc8ddb2232be11c10f4fe6b84b9 Merge pull request #1878 from alexander-demichev/blockdevices
8f7934c33a600090caabd528515f9250e13fd59b Add support for multiple block devices
93a49819c9867887f96ae66b3f86e186309dd26c Add webhooks for multiple block device validation
479bb9e33155970800dc265b2d1765c24f42e5a7 Add multiple block devices to API
57f6073679dbbdf5763943ce6bd450d9bcd4c298 Merge pull request #1853 from newrelic-forks/rudoi/awsmachine-scope-refactor
a0cc9033a174e66614bcd465289bcd8f7b7baffa chore: refactor AWSMachine to use scope interfaces
50b3fed57327045aa50845a9fa2a180ee23b9508 Merge pull request #1873 from alexander-demichev/spotvalidation
bbbba1b1a8b6a01ec4e230f425d3ec601efd31d6 Fix spot instance field validation
66d77f41efd8a55aef56ddf2d1e77bd3698cc86f Merge pull request #1868 from alexander-demichev/spot
77d493d6c72a3b4d9369a1afa2fa1d6693167bd7 Add logic for creating spot instances
fa8db0dfc764bdd9c0023dc4ec103fc2989b08eb Add API fields for spot instances
ab5ddd62adbd17c7024a39d0afe515f1a7a23a71 Merge pull request #1856 from richardcase/sgrefactor
29077a4f10f94ac223f84d68a3b14b215c0c4270 refactor: split security groups from network service
162b70cb36d0c9d35a230265f3ba6b626c0cbfd8 Merge pull request #1865 from gab-satchi/1799-local-zone
79729f0717fc7e07389ec05727fe03ca4a944557 Merge pull request #1848 from richardcase/tagsrefactor
f03d7f073aaea0df3e746e4a8a3b5bbf3f846ff9 Ignores local zones when fetching AZs
e46ab9168c3f97612202fe08c45c58538b0fefb0 Merge pull request #1836 from benmoss/goerr113
c1feda47f94b1ab082c2df74c6446d9670360fed Fix error handling for goerr113 linter
ee8ea85f02825e3bf05103d0a756493d62a02fce Merge pull request #1831 from randomvariable/bastion-instance-type
daf30e9951cfcff8f7c6b0e447d00b5ffd5ab125 bastion: Update default instance type and allow override
f1e08917d3e7015af2dacaa9f0266a18c5ce8bde Merge pull request #1859 from randomvariable/cloudinit-compat
f12caa4c59fe7151a4e0bd0b47d9c2f64c576e9b Workaround for https://bugs.launchpad.net/cloud-init/+bug/1888822
aa11790780db8578729a60d6268bf6fd82a41bb1 refactor: use builder with functional opts
ec33dadeeaac5886551c8ed2c07c12dba15c24d0 Merge pull request #1854 from superbrothers/fix-incorrect-comments
c6830a677fefbe543e24bfd8ce7cad9d318af85c Fix MachineScope GetInstanceState/SetInstanceState comments
ae7331e25aed5703f9c3ca613d8b2af702624dc0 Merge pull request #1849 from ashish-amarnath/move-to-emeritus
3875af81fc80b3b2ce07bd28b0b9fd5bee01a3bc 🏃‍♂️ Update owners file
6d90b15a9dd04d441c561ea2adfd451f158e58dc refactor: tags package to support other services
8549d6ed2a3dbe3e2e46f2be89ed64b87b846465 Merge pull request #1845 from justaugustus/version-markers
06ab70d8f395d58b95a6847428d3ca9d216db21f test/e2e_new: Use ci/latest version marker for retrieving cross builds
d59f6777ce348d5e2fb790b1eebd371785a58416 Merge pull request #1833 from gab-satchi/1776-subnet-filter
760cb197161d864f82cc735dba8ca80cbf1f4b43 Merge pull request #1841 from srm09/patch-1
1c0175d0f911db641dbd41317da77db5aaea4977 Update prerequisites.md to add IAM section header
675be8e35feabd889ec5ff9c14da586b8359c351 Use filters to select subnet for machines
e868fe2b2d22e6a06c92599c9295c968ce8b218b Merge pull request #1835 from benmoss/make-targets
cd53d0b51a610e03be0e6137f266d42a6c656655 Remove unused make targets
36e6c1a29583f1c87f55950c8a9920313b85436b Merge pull request #1834 from gab-satchi/update-owned-conditions
4b22d07031398a7c58ee164aafe921410a19170c Adds Ready condition to list of owned conditions
8c0c3db8af44e3c3a1db772145d96154a3d36280 Merge pull request #1798 from gab-satchi/e2e-tests
38bdd8122a960a42607cd1825a70f1bc8e49264f Waits for machines and ensures volume is created in first AZ
aa5698ddb9afc74316035af64824a626ef2d395f Update e2e tests to use clusterctl framework - Adds volumes and multi-workload tests - Adds md recovery test. - Adds infra node deletion and VPC limit tests - Adds invalid subnet and az tests - Adds more cluster name tests - Adds multi az test and test with '.' in name
45d6622f3777886f990e61fb2aa1490ab633241c Merge pull request #1823 from randomvariable/conformance-fixup-2
5ae10e4fbb5f797f660f0a5e0e2cd4b15d8db45d e2e: Move conformance template generation to go
de647f72846051371f42fb35e66e0b4cc43d39c3 Merge pull request #1825 from ncdc/capi-v0.3.7
d62b06eff18eef34441fd49c196f1e1cbdf6b7ac Merge pull request #1820 from randomvariable/restore-bootstrap-user-alpha
fe49373ee27f19b616a825f2ba33e3deb1387675 Update to cluster-api v0.3.7
f76ecb40a83eb0876c3a465d7f9725e9f087af77 Merge pull request #1810 from richardcase/scoperefactor
3cafceed8a1940a21815b6d1c6bd12c128cd8a75 clusterawsadm: Add bootstrap user back to deprecated alpha command
3ad5710c8c50f1820276b78bfe8c716d462c383e refactor: split the ClusterScoper interface and created network service
a48518f3eccd97ef98bc6604ded9c5c6d999f2b0 Merge pull request #1819 from newrelic-forks/rudoi/disable-gofumpt
9d4bd7f63d005e160d2f576d90431d4997eaf279 ci: disable gofumpt linter
a6070d1141203d0c7931b8eb5cbc2ab34e95e765 Merge pull request #1760 from randomvariable/conformance-refactor
d79e8b5f262bbd2f60ff17ce022eded042493b3e refactor: fixed bad merge and added comments
0cebc12696d0dbd05b47172654caef825ae76e33 refactor: cluster scope and service refactor for future EKS support
ac623653af46711926fd9b3c25a79aaf4ddbf1bd Merge pull request #1809 from randomvariable/golang-timeout-10m
8b6b30bc72ec38ac77e388e5dba3264089647a05 Increase golangci timeout
ca931b5d2fab0bd0d5f1a6e2628b6031a99b3cc1 e2e: Rewrite kubernetes main branch conformance to use clusterctl
aa772191e829b879c92ae615e9b6f51e9ea73b5c Merge pull request #1797 from gab-satchi/e2e-ci-script
e19d905ea5b2bbf3da5ac97e8104096ee6350082 Merge pull request #1807 from randomvariable/metric-test
a4cc6173507584b8c94a8240833704101970ac40 ✨ controllers: Capture metrics for every AWS API request
ad866d818e23763e0353d459ec94eb3318ef04cd Merge pull request #1805 from gab-satchi/1792-parallel-ng
aa61600165ce6083431406aad670ff82a1a76332 Creates NAT GWs in parallel
3a98cf396c83ec0926bc5b1385dc4a2d855fca29 Merge pull request #1801 from gab-satchi/1754-cross-zone
b4724838cce089fe893b7cb24dccf7d7b1e60181 Merge pull request #1802 from gab-satchi/1725-sg-name
bfd92f9b8138f2dac89a3de1de985cdcf8e1b348 Updates ci script to test new e2e flow
4f153e3ff788114c081ed8c2b6013d90332ff26b Allows configuring crossZoneLoadBalancing on controlPlaneLoadBalancer - removed omit empty on the field so it still shows up when set to false
ded7c7e8bc5bfe81422299ea63d138d66d1e35b1 Fixes cluster creation with names starting with 'sg-'
5ddb728174d49232feade8e1793f7c228919ecd4 Merge pull request #1803 from aaroniscode/eip_fix_batch
3940207dcebcf88badb71f95fddb5fc71af5aca0 batch create NAT gateways and EIPs
db9a69baf5b7cdb4cda4e95806310ff19955ea24 Merge pull request #1794 from benmoss/bump-linters
a7a502861fc676f53fa4fd6b7de0a20c5388dfc2 Fix import grouping
6b6dfdfd305f973fcc9e19d8c1865e0d4387d2da Update generated files
3c88e81f8a9d1bcc7d725b9d28a4c13c61e02603 Bump golangci-lint
87d629471aef012647a87518260da68ada2e0b35 Merge pull request #1783 from randomvariable/aws-sdk-0-33
f5b3ec77e4107c3b55164524665f8e21a9476bc1 Bump to AWS SDK for Go 1.33.3
0a050a72c16a328ddc8a8177337f60591ee6813c Merge pull request #1793 from benmoss/inclusive-other
eeaabc5cfb4de54711e5603bcc361ec55f82b6ca Merge pull request #1761 from aaroniscode/bastion_rules
b950729f23f1783a7d6dc6189e1781c0feb95565 Sync up with running emoji to seedling change from capi
040406e90dd5f67e840cad00b3ec01c89ffbc24c Merge pull request #1789 from gab-satchi/e2e-fix
5bb849dce29e23ee94d7265daee3db6107b6b6c6 Merge pull request #1791 from ncdc/randomvariable-maintainer
ecac4cf28bb7153d42c2e9040ca69d279a2f3d21 Add randomvariable as a maintainer
2dd0b0121ec976f5f15fa9552ff3bc29bfa19d6b Merge pull request #1790 from randomvariable/binaries-before-manifests
f45d3d092c7cd95ece746124d229b47155856877 Makefile: Build clean binaries on release
365729b3cbd31e4b8b951f20887b50c82c0f3fd6 add AllowedCIDRBlocks field to Bastion
0271970a024d9ec6ae202762069bd1aa450f19ef Restricts AZ limit to 1 in e2e tests
bfbe06045eb1bf85e9f16b0decc4f527401d5379 Merge pull request #1777 from gab-satchi/cluster-conditions
3a5cb46dd49ec5556fdc9cce96bce6feb156d6e9 Merge pull request #1788 from randomvariable/elb-ignore-not-found
1bca421da3aa8fe0373a639264ed112a3a4418e3 Adds conditions to AWSCluster - Uses OwnedConditions in patch
e4e00524dfd993858739943d69a535fe3a6a5c5e awsmachine_controller: Allow instances to be deleted if ELB is already gone
68f4c6e8ac5b97aa61bc6771cf1d3f822926c0a3 Merge pull request #1740 from gab-satchi/1739-conditions
092d7d7b2919b330dd8edbaab1b3cdfe923ced6b Adds AWSMachine conditions - ready condition uses step counter - patches machine with OwnedConditions set - predicate to reject status only updates
0574c1d140364428b47480b52ab3ee6c4706938a Merge pull request #1781 from randomvariable/seth-emeritus
569e9fc1eaaa7266f1697fc0296c3174630a6fed Merge pull request #1775 from sethp-nr/patch-3
1d4e9c81867bc893d145575f71c696a7d21eac4a Add Seth Pellegrino to emeritus
faf9258b1ea658023f5531917cb7b79cf183ea25 Merge pull request #1763 from randomvariable/clusterawsadmv2fix
b68c341ef6522f87830e3f9c560e51749d5d5f2f clusterawsadmv2: Behavioural fix
d9aafd2caef487882a5d613e6d53b4a03615f081 Remove sethp-nr from reviewers list
54ade7b8e8a97b8db2f05844a719b8da11a756ab Merge pull request #1774 from ncdc/fix-delete-bastion-byo-vpc
9ea2842cca39327908458e3295860ab9a63b931a Delete bastion regardless of VPC type
d3b36247c034bb3d358f23f9788e6fd41513c181 Merge pull request #1767 from ncdc/fix-lost-vpc-spec-fields
1d4307fe81bcf6e04821d71a1d64b46ac72cc6e0 Preserve all VPCSpec fields
bab89e839dc483082051f402633bb98f83fb9235 Merge pull request #1766 from jayunit100/minor-build-note
198a9ced7b1dcfaa331f69e37140f3a6c6266dc3 Patch build instructions/note in mkfile
4831a1d5347b00a2523cf7b02845eee56fbac1f7 Merge pull request #1737 from moensch/1736-machine-elb-harden
2933987ab708cbbde06bb0f2bacc83045c6bbee8 Ignore "not found" errors when deregistering ELB instances
bc356de31803d34a861a39651c93face848410b3 Merge pull request #1759 from evalsocket/fix-1748
f95ccbc1d1d048daa2528a2867852d593310c244 Merge pull request #1758 from ncdc/fix-elb-instance-registration-rate-limits
19cc0feaea81518c4daca1702ba2d316a9d70df3 create a bastion host if it's enabled in the spec, regardless of managed or unmanaged VPC
e71a82acae488823deafb7a72b63bbfead5dc2b4 Check before (de)registering with ELB
c718d8e8aaf2b5634cf7b233834818ff07d9d613 Merge pull request #1747 from gab-satchi/1744-cni-ports
98b4e9f809881bee15b8c85997bf153aeefa9aba Merge pull request #1749 from randomvariable/conformance-timeout
6e556c6590948882e4667db02eb014d7786851c6 Bump cluster creation timeout for conformance in multi-AZ
d25c45090eab379b146b43e84d8b4ff24b8f58f9 Merge pull request #1734 from randomvariable/clusterawsadm2
d7f9d5ca1b9b4de12b0a5c021f91987e07d84b0e Adds configurable CNISpec to AWSCluster - Adds Calico rules as defaults - Merges user defined ingress rules with defaults
e14356175f4dacdcb644b6373ef6c876aae349ca clusterawsadmv2: New API and customisability
25713cd6f2d9d880cdc1f950a789c90277fe5a43 Merge pull request #1721 from richardcase/networktopology
7933fcd71b352fca6775f8a34bec70b9eba21db7 fix: changed the default AZ selection scheme to ordered
f75813c1d186e9a83e4c9b0526e0b066300a6122 chore: updated generated conversion files
957037d1cb6822e93f1d9656fb7b3b352b068cc5 feat: exposed AZ options for default subnets
d4ade5922e04a2327f4043effd16252126dea223 Merge pull request #1716 from gab-satchi/e2e-refactor
2dcbebbbbc71d23297699c06f0ebc687b763fa21 PR updates - removes unused template
00885d99c7af9b5c77bbb9ae681b5d7bc824bae4 Merge pull request #1713 from randomvariable/credential-provider
6eaa3f7350716ee7a94185b646b756bac5124c7a PR updates
212eae6835285a130aa1688a7ab565feb529b636 Merge pull request #1735 from randomvariable/remove-spews
ee7831278fa029413ed9b0c2e9b5967937256311 Remove spews from tests
13ceee9bfe8ac582d0c4e71e9b74dfe387fddb62 Merge pull request #1730 from alexander-demichev/providerid
8fcb41c02c021fb5a50423fe0feedf1870fa5071 Merge pull request #1733 from randomvariable/aws-sdk-may-2020
02bb32961f8214a00d323360d39b666316136d16 Update NAT gateway creation against new EC2 API set tags directly on creation.
d9505ed836f8117d2701b9b0f8ad413863212f4d Bump AWS SDKs
e34750d31145490fea887ef9bb3d7511993c6063 Make machine's providerID consistent with node providerID
d3d8d2f2b505e090d0bfe517c378defb8601cffc Merge pull request #1732 from detiber/capi-v0.3.6
4e820bd5874348cdd23b86b1205e4666c8697675 Update cluster-api dependencies to v0.3.6
93f7cb06ff5d3a4623ebd078a8ecf9c3039ebfd7 Merge pull request #1695 from spectrocloud/cloudservice-events
17ebe05d990a33509b8aaa8fbac9e73843d2f188 add events for AWS cloud service failures
2f7b382b70ccbf7c2b4b56f9a14227c5b422b698 proposal: Single controller multitenancy model
f5332ce432ea588daa45452375669d778d956601 Merge pull request #1731 from randomvariable/machineaddress
0beedefe8fc56462dca25fe85037e7dc2f4f0c45 Switch to using CAPI's MachineAddress instead of corev1.NodeAddress
425e1bb337cfb76ceb38c1cce97345c26fafe08d Merge pull request #1694 from bagnaram/1644-customizable-image-lookup-format
7c422f9f361e07523f0071609c3b18d374926a1b docs: updated multi-az docs
3a2454aa3a8426bfd5ac7b1088e4b3563e80e9e3 docs: updated the existing infrastructure docs
b282d5f78210a8beb29baa56202585d577cbe9ca feat: incorporate review changes
92914ed01fc89b11a389ba947cacba898f9239f6 chore: added missing header
138314b051716b196607688d55aa520fd6bb62e7 Adds LB service test
b25c06a693d1deda33af1fc4b9b6b18a37ae63ce fix: fixed typo that caused lint failure
a05a30cb14158b05d6c130885b7278e14d31e1cf chore: removed unused function from subnets
164f84be98b9957a0c1c3db866e13228f174b758 feat: changed the logic for unmanaged cluster to not create subnets
d42df45ed300969861bb8f0ca5737062776a0e85 test: fixing tests broken by subnet changes
5ab4c7c366be51a673068d8e775436623f0cc00d feat: changes to the default subnet logic
130a4c061c9c0a95e45980a1152a44146063493d Adds capa types to scheme
11b362088b382165b03b208857e9d6a757f68bbd Merge pull request #1680 from evalsocket/fix-1678
728b29dbcce867b7a9149aecda358ed3f0eb33db Added bastion check
d150541075065c52aea4640eaafc5c47aecdbcad Merge pull request #1714 from vincepri/fix-loop
6b271ea3454eaae9d6dbc625f5d7553d86235165 Merge pull request #1710 from fabriziopandini/improve-reconcile-lb-machine
36bffcd7f7a1b407a05a9517feebb75dfed35f60 Adds boilerplate copyright info
e8f37a242058b15a7fc7699102df3d39e66d5054 Adds e2e tests which utilizes clusterctl framework from CAPI
f464b17cb56516a77bcef7c21d74a27f1b0bad0b Reconcile ELB attached machines when a Machine is being deleted
6e59e96c5ace7b04a86eaea6ca2defd820bad47a :bug: ELB should now not register subnets in the same AZ more than once
ce642e8a40a67d43810972b8fbe7a4a2223773c6 Merge pull request #1708 from vincepri/see-stopped-bastion
49057dacdb762d007621c336145c720d1ef7e4a5 docs: Add timestamps to existing proposals
8efef28fb2a255b5bd81162284a54f1224eb61cb Makefile: Add diagram rendering tasks
9d05351c4fd97c627a854d6b64f55557f689a030 Merge pull request #1709 from newrelic-forks/fix/dry-run-side-effects
3d8d5f16b74add8f3b587868c47310889a70dc8f fix: flag webhooks as side-effect free
e56d0e873a05c20265c44e30fe15f2f9ed8866b7 Merge pull request #1688 from detiber/updateRoadmap
ba264f498528da7325b572f603d74cbe84ef7966 :bug: Include stopped bastion instances when describing
08e09fc8b31974837a4876055eef804d27718a99 Merge pull request #1706 from detiber/capi-v0.3.5
0580fa23476bbd797ecb5b3d1be218077f801662 Update cluster-api dependencies to v0.3.5
32eefe16ddea72d4727e0db4ec38e68902bd99bc Merge pull request #1675 from scottslowe/issue-930
7624e5c2d9e3daa25b1ebe1536b84f5c846680bf documentation
74822cb2ef9272bc07a7e247156921533536e2f9 modules out of date
2523f8a64102d9980f52a1d0db073640f84abc19 moved gopath and reran conversion-gen
a0271e8138234839ea66fd3d99fd624c19d44dd1 go.sum
e9f771c0c7135d70b72be939caac9178e38c1667 re-generate conversion.go
e1736630736ee52d6a7c356651b333180afdc746 Merge pull request #1687 from detiber/conformanceFixes
3ada65c76f225879971389e6947c366bfd2ef096 Merge pull request #1697 from detiber/updateAMI
bc07e2bb1d15ce861cf2cbe4129f47223937d4b7 Update AMIs for latest Kubernetes versions
63e9ce29f0691a1520377ee0cb0568c27172eb56 Merge pull request #1692 from scottslowe/issue-1638
5aa713a44d66115533fdc5d5f3993892efeabb5f error handling
d75cca2b8fa2e5094430c84291eceaa55e70f6a9 re-gen manifest
2336209288326497cc6b545ff44c3830079842e8 Address feedback
aacdbd76c59ac188d95d23df4c68555890c4407a Using golang templates
6ae07d0118f1e1883546f62a5a41fb909bf37d9b Incorporate reviewer feedback
a1e4900f34b2568099f5399952d8ef484ed794e6 Incorporate feedback
618c1bb57292e04773da6bbbd05c755bd054734a Conversion to hub
166993ead16a6f599e846c80fa80bdcd9d58bbf7 gofmt run
6950b4e130c5604a4fda6784cdbdd29090346778 conversion
bfc23cb8867d5944e9cdb5348826745009a3e7a7 fix tests
0e5c4e4ca44b6c57691a248b08131b95c7c46205 API conversion
6d96862803cdda9424cbf76878c75ff022535800 Fix issue with clusterctl misinterpreting comments with env var
db7e8b7027f6e9b7f34cc7415cc68f985854fb6e include generate manifest
9a430c7fbc389d15d9bb2fde805eb4009fc2d66d Syntax
b234d73e965b5edcbdf7e8da8d3a2f8b30369d54 syntax
ae2a903177d68ed236ed51ea220a945211db5355 AMI lookup string
6799a1887ece646c2a3ba53a9a35b36a8f196c6e [ci-conformance] Fix make-based conformance tests
99349b8abeb34123b2e13d025946a2e66d6d6b40 Merge pull request #1560 from scottslowe/issue-1511
58168a6040a6d696145f382a53e1b9246a6bb11b Update docs on accessing instances
b63871f27f68ccf7a5e534493a252d0a6f17893d Merge pull request #1690 from detiber/updateAMIs
220fc5e91fb1673c8ab43a7892c44ac6dc122e47 Add AMI for k8s v1.18.1
34844c12f164d30055743776a54976b546bc4ece Update roadmap for delayed v1alpha4
e2c994bc32f43713eb983efbcfe313353b80b4b5 Merge pull request #1677 from benmoss/cluster-validation
ff52703acb1552431bb4fd701400c23bda05c6db Remove bastion validation, formatting
ca38f8ac0bbe18bf388f02e4c6b90b96c45caef0 Merge pull request #1686 from detiber/conformanceFixes
60c534b3456ad9e322182b934416f1ca3525348a [ci-conformance] Additional conformance test fixes
616ee39c2de91414a7e520d0c3778047e42ec247 Merge pull request #1684 from detiber/ConformanceFixes
7db6141e58b997dc984f57cdb8336b55202c67f6 Merge pull request #1683 from benmoss/default-ready
99f59aa7f235e28080ac047d0d73cd549d7d59ab [ci-conformance] Fix ssh-to-node to use instanceId rather than private IP address
c50f7e01848e49e838532229a7958075b5189303 Default cluster ready to false
6287ed34d5d6fd831981e3a6d1f19202f935295c Merge pull request #1682 from detiber/fixConformance
67ba7778b38b42d4ca4f7c4e6152830f5e9572f7 [ci-conformance] Increase timeout for workload cluster node availability to 15 minutes
a14a228ce6b8a548c4768c0bcfc78ed1f88f98bc [ci-conformance] Use AWS Session Manager for retrieving logs instead of tunneling through bastion
62532957e84cc8cadcb99b4d74d32620a4849796 Merge pull request #1681 from detiber/IncreaseTimeout
af6a3445100a5649503f977277e006d5e73dde52 [ci conformance] increase timeout waiting for nodes
b43dfd31e5425f1f110fa9b37b83269cd58dabcf Merge pull request #1679 from evalsocket/fix-1670
90d606bc1eb5094f56cc5faca9e860d352dd7f1c Add validation for AWSCluster
df7da8ef2be251cfb4e5555d677e2563710fe862 Added version setup log
661e28de987654e1b91db293fc2725838da46f33 Add documentation for multi-AZ control plane
22be31dd76da04409c425c77e2967db327f409a4 Merge pull request #1672 from detiber/updateCAPI
e2730c63464960eb95dd4d6dbe859c0b7a7286ff Update to latest cluster-api version
488ad18ea3159d8e1cdcb9acbfeb88969204a262 Merge pull request #1667 from detiber/LoggingPredicatesMappers
e41e84961aa0bf90efdfaf84e9cb86a7b3820cfd Merge pull request #1669 from detiber/fixE2EScript
0e65c9295b4153f10d66401ac7bc2e5bf0bb834b Update predicate handling
6cbe0c0167d7f6c021090e806d83892c768aba01 Merge pull request #1671 from detiber/fixConformanceTest
f4e0671eca64c0fa0445cf58e97cede796fed02d Update cluster-api release used for e2e/conformance tests
76ffc3d53aaee89b1052989b9f1a3bea910027f9 Fix filter argument for e2e-conformance.sh
982d2200ded3123e3803cd0d3c9197f4af5380d0 Merge pull request #1666 from detiber/conformanceScriptFixes
f5b1f488eea79240da08936ccd5149c9f30ee4db Merge pull request #1665 from detiber/updateDeps
2bb23c55447d7e621380c7c2070f960159521991 Update dependencies and latest k8s AMI
2160cf21d57c557d826f11743ffe5f6c9e93e1e8 Fixes for the conformance script
a1cf6448459c155421b041af2ac86ccdbf3cec7f Merge pull request #1663 from ncdc/rand-seed
790d80f7815f3588da8e24e67ba590246eb08ae1 Merge pull request #1662 from ncdc/init-CR-logger-earlier
506c8a226fc0ec38e903144013103923f6cba036 Seed the random number generator
efa2513d310f9c256c227c855acfd022447eb474 Initialize CR logger earlier
a33342eeb2fb0e0682ba6bf90745df1954a458c5 Merge pull request #1651 from benmoss/dns
82d8f2c0c5e3ee82e6e5ca6a84eee7cb32633425 Merge pull request #1648 from minsheng-fintech-corp-ltd/master
07ec7d90f1047a2b2740bfe6251d54a9ea1b7b02 Merge pull request #1653 from detiber/loosenImageLookup
5170c58ba70c7417c9ca90e44ad8264839a30f7c Loosen the filter used for image lookups
92508e6db9858a22cb29974d0841a4507b84a8a4 Merge pull request #1655 from ncdc/awscluster-watch-clusters
96a146b993e0b25a1c782ad5574a02316ed50b89 Watch for unpaused Clusters in AWSCluster controller
1667e3ab6c1655c4c8e151e32e4f002983f5ce31 Incorporate suggested wording changes
35ec7d2a453c10ab1ce5ddca85ccaa7744f4eb2e Add flag option for uncompressed userdata. related: #1639
38ce86029964b8639415b889b2254ca1fdaf1e22 Incorporate reviewer feedback
e6076e967fb08dca2286245c3c9ddcb36decfb44 Ensure ELB is resolvable before marking as ready
7240d095ea189681c6f92c79e14dd37853af2512 Merge pull request #1647 from cpanato/fix_typos
2fad41ccdd35de7190250c0b6e130e35e41fed05 Merge pull request #1649 from 70data/master
4055dd7df4110176bebd1c7606bee3873f01a090 Fix v0.3.0-rc.3 to v0.3.0-rc.3
e36493d2073362dc13f65167ec7d4b74f1bda79c typos: fixing typos
ceeafcbc701bae0129cd59347302e581f8ca564a Merge pull request #1645 from detiber/updateAMIs
c8b958aeb52aa796ac8981c97448220ca9b8174f Update AMIs for latest k8s releases
f873e1afca2094f12f6811b3ce7370971d738693 Merge pull request #1640 from detiber/updateAMIs
e7f975a85d7d23ce53a8c6d0f9ad9062f1463fb2 Update latest v1.16 and v1.15 AMIs
763c3ea9da37f2ad9fcb5783ec64cbe14c61a911 Merge pull request #1636 from detiber/UpdateDeps
e997afb80c6f0f76e0b6707177d65b2c5ac564cf Merge pull request #1635 from detiber/v0.5.0-docs
413b5310e9b34e469600781705408ccc7659ca06 Update docs for v0.5.0
970ff4d08f1c2ba7b9322ee16fe03d5d1be4f72c Merge pull request #1633 from randomvariable/normalise-template-vars
45b09b97076fa1c3223605f727a7987eec8621bc Update conformance testing script for updated template variable prefixes
566e1dbdf8c08d39f95172e1e231a247589a301c Update cluster-api dependency as well as k8s and sonobuoy versions for testing
04d016ee2d8f5b706c68482f054849e6022df2e6 Merge pull request #1634 from detiber/fixTests
ee921e57cf9c2de651c3da745d0e4cef9547770f Update e2e tests for SSHKeyName change to pointer
d3256ebb4b90c59f146330a60699895d1b5a0b8b Normalize vars to have AWS_ prefix
3e884c7f3823a5ac48c913c027a511dbc3aeefc4 Merge pull request #1630 from detiber/fixFailureDomains
40985d540f5805a7f52a4226c076e184465491d0 Update failureDomain support to handle it being set on the Machine rather than AWSMachine
ba0dfd656473310fb4bf45905e99579e2c6bcf13 Merge pull request #1621 from andrewmyhre/1156-allow-no-key-pair-v1alpha3-2020
b12ff806e7f801a14f0d6faa87e76a27dd183a3e Allow machines to be provisioned without SSH key pairs
500ab7a6407e123a52b120d4a672615773c2aa3b Merge pull request #1628 from jayunit100/backportGinkgoParallel2
d850d188b491307c8bf018568b7e485b5a6cb6b4 Parallelization of Ginkgo tests, combined with confirmance, combining Naadir and Jason's work and adding stateless concurrency friendly implementation , tests complete in approximately 2 hours
5645b8ac06fce23cb0d4706d73a03e69b40f042e Port E2E test automation from release-0.4 branch
0b83f06314410a9a3d628f006a647086f51736a8 Merge pull request #1626 from detiber/updateCAPIComponentsConformance
930c764b9055581ebd65d0caa5987b6a7e8b219c Update the CAPI components used for conformance testing
a130b0bd495237d3a69bb2fc2be70147b1387f31 Merge pull request #1617 from randomvariable/pause
b580dd4e98c85a2f264187804334292819dc5990 Merge pull request #1623 from ncdc/fix-calico
6569902a81c14e4e0f97b1f93e79e22484533efe Use latest Calico manifests
15da39360ff1d942b39da6fa9d93e08e517bafa1 contrtollers: Implement pause mechanism
faf51a5061f91ecdce92ee917295b9cfd40403ee Merge pull request #1600 from detiber/addRoadmap
e3759e4a1a065c4b2ba58985b4aec22c97afcd74 Merge pull request #1618 from detiber/capirc3
26ec606fccbe07122460c1ca0ec655f951cc06c5 Update CAPI dependency and set MatchPolicy=Equivalent on webhooks
0f8e8c3b03a2a25c94dc18ba0271e5791274485a Merge pull request #1612 from voor/upgrade-aws-go-sdk
e883bb2e37d285fc63cd6a3cd648d4ded6440b66 Merge pull request #1613 from randomvariable/releasing-updates
3796ff740bc1710780de910e81ad37579796be20 Update releasing process doc.
a2d2d69a50fe8a15fee83c24e17b35308dd62110 Update releasing docs for latest changes
6687035717d67c8da78f9cee225096a98ee1ac8b Merge pull request #1607 from detiber/releaseArtifacts
208a3a261044823ad40f44fe371e695ddce97e13 Prepare release artifacts for v0.5 relesae
ffea16734694510d96eccf06338ec362ff856074 make generate causing some inconsistency, need to investigate further but for now just revert this.
4b6b97d12c325ada2fb22901ebfabd9a33bf52e7 Changing AWS SDK needs more mock methods for test due to changes in AWS EC2 API.
10758950c2d68322ed0cbe99ed9cfd75842a79a6 Bring AWS SDK in-line with Kubernetes master
af07c1cf90e1291293dcb7668fa1238428405e90 Merge pull request #1606 from randomvariable/automated-cherry-pick-of-#1563-master
0913458f93405c420a159f69ce464a936cc54ebf secrets-manager: Fix error handling
f3ef8a252d9e89129624ea7b240e35dc8ecda50a Merge pull request #1599 from detiber/fixManagerFlags
6c77697168a3b6c9176918913ce7742ec2567385 Merge pull request #1593 from detiber/addSessionManagerPolicy
4787af5a3620130073e5f54e65994a6ec7ced96c Merge pull request #1601 from randomvariable/calico-1-17-fix
272c71b0b4da9445bf5b28a94e73bee37c8ad583 Add a project roadmap doc
7dc878f4a25d1f50ae106b1141a3e59229b5de3e addons: Bump Calico version to 3.12 for 1.17 compatibility
dccce0effbdc74e91194a2392c84986cdb61f30e Ensure that leader election is still enabled after applying auth proxy
04921198635ba0881299da26dd28789cd36bc080 Update node instance profile to add support for Session Manager
db0e9944ce0ab25f29307c844065ad43dd3a404a Merge pull request #1597 from voor/missing-gov-region-aka-partition
c9682181a79eb1ee21c83d5c68ff446c17b929b6 Need ARN values different in GOV regions.
6aaaea94f1f3fba0e26419de9ef7f09ba6ec0411 Finalize instructions
40ddcc9e055e34446f82966377d832a372432b5a Merge pull request #1575 from newrelic-forks/refactor-kustomize
9cb203e3ed8d9c9b2f513ccd9c4757101e8cb891 Replace config/default with config
44b7898a696a172d345d0b67cff50004b0580085 Removing role aggregation
52e840502f174ce4119449512dd07d997be3eca8 Merge pull request #1584 from fabriziopandini/fix-clusterctl-settings.json
1219e68e0d4f1657010397a6aa1760330d7c5745 Deduplicates the capa-manager-bootstrap-credentials sectret
0787d80b23ac79607ddd289015b1637183ba5f6b fix-clusterctl-settings.json
9913ac8dbb96ed9bcffa6eba75b886cd4ef8c20b Merge pull request #1567 from teaguecole/errorcheck-linter
279eaa9ed386a4ef8b5df73f570de52b64d875b1 forgot to lint check, fixed a style error
03bbc944c22d0851a6a72b9a968adacc42612a13 missing curly braces
d1af735bf438eea1faaab2b1d39b2ab03f1e4cfe Merge branch 'master' into errorcheck-linter
6f3090142dd512f07fd315d1de508f3ffbc4eef9 Register reconcilers/webhooks if and only if webhookPort ==/!= 0
ff9b7da312108b804632dc715949595139123796 Merge branch 'master' into refactor-kustomize
addae52b339b935a442e28ad65b0418deb760920 Merge pull request #1569 from ernestas2k/enable-and-fix-stylecheck-rule
ac5797cca4ee0354c2be11b9c5562cff8474f613 Merge pull request #1559 from teaguecole/enable-linters
58cd7f89f895bfdf9f03bc88143b11e727c565bf Fixes flag indentation
6cdae7f1f9ebe3ccddb69b8c21bac707d4a9d40f Merge pull request #1577 from newrelic-forks/crdv1
568be061ee90b16fc851b30a4dfbc3eb3ff42d76 Adds the contract version label to CRDs
c5a3e214a8efd5e717ae9e7ac8cc787db0cd9328 Update CRDs from v1beta1 to v1
2350a635f68580fd2101b2cb439be169658d65c2 Update to kubebuilder-tools-1.16.4
5c3058db2b151dfceb348514b74d5f4975fbbae9 enable <stylecheck> linter rule and fix related issues
e3d17e333370cc6136e1e8f4c09a3ba2c5fad66e Updates controller-gen.kubebuilder.io/version annotation
36a2a68e13386c3ff0eeea243f4998fa1ee2dfcb Update controller-tools to v0.2.5
d984d0eceba1527c24f84d900119c0eafca3e523 Merge branch 'master' into errorcheck-linter
24b7c9810471e583184f347bf662d2efffa04eef Failed test, I think I iterated incorrectly
118548d567017e728bf65c84e205bc0c59f99728 Add missing and remove unused modules
3479b0025548ea329a69a066c53ef1aa0ac7df4d Define webhook in CRD patches
f93447a23bbdfc0d5fb1d679f550c9ee529dba05 Fix kustomize build
3196214146ba8e3a46649b84e2601345538581db Sets crd:crdVersions=v1
eed4f59aa5ba72db7a213772c43d49fd9ad9ea99 Update controller-runtime to v0.5.0 (Kubernetes v1.17.2)
6d2e093f91cceb4b3f5cbeb6e9983549f0d84812 Update all dependencies to v0.16.4, which is Kubernetes v1.16.4
a9fe4f8b4065b5fb7c937a1c074fe7a7a51971fe Merge pull request #1574 from detiber/kinderEnsureKind
67f1b1c54abc452058296b81c21d6e6642e954bd Do not set xtrace in hack/ensure-kind.sh
bb316bc4498248d77830e6226c93adcafc997e2c Refactor kustomize
19dd80de9d26b40b50a42c02d96c16cc4016e2c4 Merge pull request #1570 from ernestas2k/enable-and-fix-gosimple-rule
e6f254335cb839d50104df38aa21964b39c8a41b No longer shadowing for the other changes
b5dac7a03eee2a72662ced87e857782a06cc2bd9 Fixed style for the rest of the changes according to reviewer
edd968b7173ccb9eaecb84b66d865c8d917ac813 rebasing branch on to master
046921666f9c7ed3bcac8fbc16d386f981ed80dc Enabled errorcheck linter, caught all errors
6c6919039fceef9e25ef5e38e338b53f615dc3b6 Changes to styling to accomodate review requests
5fa9f2ed8832284061074c41032a7bd9f8184135 Merge pull request #1566 from ernestas2k/enable-and-fix-unused-rule
dca5858e2ef4f951e70380cb860cc019f26bc170 enable <gosimple> linter rule and fix violations
7513c30a054f7380a002e9eb919091549900bafc Merge pull request #1568 from teaguecole/staticcheck
31aad4a2368d36b7fcc8afc82b0f84090689b513 Enabled staticcheck, replaced deprecated log pkg
488f46f646122d3b18f69920e2a568fd1817f7f9 Enabled errorcheck linter, caught all errors
ec12ecf714e3ac0f3f4d18d623022d23b9f36a72 enable <unused> linter rule and fix related issues
1809e29e0d780ecb262929a425c095619c4a1bb8 Addressing detiber's nit, no longer shadowing
28446b5f4c3aea0b76a5a8e7e21c5394c707c26d Merge pull request #1557 from newrelic-forks/rudoi/network-omitempty
c3e8cfe170c7579099ef16c53f9d3a556fb4980b Add instructions for existing AWS infrastructure
cc42b63dc96c22a64eb90595111400dcdd9e6cbe removed commented out scopelint
249e617e427358732e94b7a45052d2eda9604eea enabled scopelint and fixed reported errors with suggestions
df81babf16e955d0d4f38474807a75c68e7acd59 chore: add omitempty to networking types that may be empty
833e9ec9eda524c5c14b859a630fd583b4edadb4 Merge pull request #1558 from randomvariable/secrets-debug
b84a27c92d1175136ae20dd251bc58db08517b7c userdata-privacy: Additional troubleshooting info
aef36c6546f12379bc7a260385dddc7d7e352dbf Merge pull request #1549 from ericsmalling/gocriticfixes
b8f61b70982eea3c24d21efbfa03eb95070eeb85 Merge pull request #1551 from newrelic-forks/fix/create-sg-panic
e512c81c99ce68659d06812a5c31122cb596c29c :bug: panic in createSecurityGroup error reporting
51aeadc0cb93869010e8d71330275b64eb012f40 Merge pull request #1548 from detiber/updateAMIs
be2f025974372d257e0da47fc88a120d75fac72d Update README for latest built AMIs
0f7e2dbd4204c981beeda4d5491bb4ff564cad1b More gocritic fixes
8cffc61b6bc7f6cc2f687e1f6ba4fb7e09a8fb89 Fixing gocritic linter reports
81e5184b6902b8ffd753c738b1a91c3bdb7a7b6b Merge pull request #1498 from johnharris85/expand-disk-options
379c6c7f101fbdef61f3fc3a4fe6c1fac57c2a33 Merge pull request #1545 from hypnoglow/enable-linter-unparam
1643dd427b1737b50e1fcea2541003a59b8fd28c cleanup: enable unparam linter
80af1bc77743c28011c3416590cbe67eb74617a7 Add extra root volume options
b5b1e6b5ed20dd23fde2375c98ab8d7795f947ec Merge pull request #1535 from randomvariable/chunk-secrets
3007191b617b10681d4829c30f49960d365030d5 :running: Update golanci-lint
83b05eecdd87f4863a07d9ddc3e8005dfa3c750d Support chunking AWS secrets
aad48bd4140f10703d6f05bc83a66a284350734a Merge pull request #1525 from vincepri/use-fuzzer
2dd02273e0669b9a1c193893d56caa20862d5b5d Merge pull request #1529 from randomvariable/userdata-privacy-docs-master
7ea3b81b7868f281d15fdb29c258f977fce94482 Update docs for correctness around userdata-privacy
7d5972577a376c7b35212b5071cfb84f33b9223b Merge pull request #1527 from ncdc/readd-return-for-failed-machines
f501f3293e0090f830d48d8af67424bfb1d889fe Re-add missing return when reconciling failed machines
30df9a923449cfa50cd209518e0e28605c515a8a :running: Test conversions with object fuzzer
bd50c3be2531633d55091f08cc344f38489153d7 Merge pull request #1524 from randomvariable/secrets-additional-perms
7b9420997a6a961fc2b30a326494451700a236b9 cloudformation: Add tag permission for secretsmanager
31331d46accc7f5c83fd5c8bd7ee33ff41ed1fa1 Merge pull request #1521 from ncdc/fix-getAPIServerClassicELBSpec-panic
492ec530e6d868923eefe77899be867efaa78b7a Fix panic in getAPIServerClassicELBSpec
877217828d36912fe301238d45491da21a84f5ed Merge pull request #1518 from detiber/boskosHBTimeout
156a7b4bf988783b0c59bb75528164ce75d0083d Remove hardcoded 3h timeout from hack/heartbeat_account.py
b34e88428c07cf9d88c384a3fb830531c513fd7c Merge pull request #1490 from randomvariable/encrypted-userdata
02d50dae39254bf409b74bb8d0f371c142109cfb Support use of AWS Secrets Manager for userdata privacy
417592a6c3c7293f7b7b38cb3f4825fd97ecb1b9 Merge pull request #1514 from detiber/FixConversionGen
d75d914e874d51d774cc684381c53a70e9dce96d Update version of conversion-gen we are using
b240a09c22245e372d482641ebc7c89f6f8d5188 Merge pull request #1515 from ncdc/update-kube-ci-url
de4ac76d9e3be6e6d289c402c7a23d0cbaf9cc12 Switch Kubernetes CI URL
ef808cd721a9fe198bb44dd403cfc8319394b7ad Merge pull request #1442 from vincepri/support-cross-zone
b92a24637a2dc0f64850b0999d300a466a54efbe :sparkles: Support cross zone load balancing option
6dd034c2ba7d90abd11b48a328c490d631512eb9 Merge pull request #1509 from vincepri/remove-az
5da6bbd270df4c4c2082b23101f11c88eb5395db :running: Remove deprecated AvailabilityZone field on machine spec
f07636cc6daae362c8c1ddd1c76a3d2bb484b972 Update module dependencies
38f1b477d86e625e3342dd387e72adb899bb15a0 Update generated files
b1c6eaeaea339e344479cf7ed242f2f85ab36e23 Merge pull request #1448 from aaroniscode/machine_webhook
bb4e55c426e781a917969ef9b566809ee7e4f413 fail AWSMachine when no AMI or k8s version is specified
926c6b58443109fbed404675a675525f82dce64c Merge pull request #1507 from chuckha/failure-domain
2e2408898c7938a316e37dc52d9d31cf2d83ecbf Update Machine FailureDomain field
f1349d8098e9ad9b477d8df16a11684417184c77 Merge pull request #1504 from aveshagarwal/master-tags
fe8e4faa44f7063f9048ec808148f801fd7ff52f Add unit tests.
40fdc64dde2fc2da49099b930d07a60d20e98235 Avoid updating tags if there is no change.
03dd538cf3b71e8fa53e3a8897edc18baa9739c5 Merge pull request #1487 from cpanato/GH-1402
0280646c93e9d6d5d1f81f51aa1e317d3f2a2f66 Add liveness and readiness probes
24b2057904692380d419db6e8ab56ec35779993c Merge pull request #1502 from ncdc/update-capi-maintainers-alias
0929125ef132b3c249fa126b24bd7ee349c84125 Sync cluster-api-maintainers
00d21035bb4d0ea3fd49a77ffd5811529abeaa3b Merge pull request #1488 from wfernandes/clusterctl-labels
67067f7f8a8292ed604c14e7b50e523fc5ac0c81 Add provider label to CAPA components
83fceb011bc94bebf3f733bbc330b335c8d265b0 Merge pull request #1494 from noamran/rbac-proxy
1688ce575fd9555242f596616eb72cbb24536807 enable rbac proxy sidecar
9b2137f8139ef1f9e43d68d21fb3eccc395b7816 Merge pull request #1493 from detiber/fixLogs
65d948a09f9d664eafea28b3ca8b63a3960732ec [e2e] Add waiting for deployment and watching logs for bootstrapper and control plane deployments
501c521c6687084d3d9e7af3d4f3727c69b2eb18 Merge pull request #1492 from ncdc/e2e-do-not-fail-overall-if-pod-logs-fail
c0eae43e6b9e96be8fc49cb885e5fdae38f412d7 e2e: don't fail test if log streaming fails
7734c5c73341219a01f7ae69495c133eb7860060 Merge pull request #1455 from aaroniscode/update_clusterscope
c48dd60c132d612daa1ea6c43adad1bc676e76be update the cluster scope after adding the finalizer
9b99309494a8614907a511228120ce60b6d3fd8c Merge pull request #1445 from aaroniscode/subnet_not_available_event
644d6e1e15eb8fc1f01976baeb7665cfe60581f6 add event for no subnets available in an availability zone
1973d5e58f0f811edfd269a5c64501ba464ecb5d Merge pull request #1482 from aaroniscode/controlplane_sg
2dc6a0bc985e39a6e6ddc1a260ef9bbea0f26642 update control plane security group to remove 0.0.0.0/0 ingress CIDR
91799d7d15997bdf8f113b28da1ca99f3152b97a Merge pull request #1466 from vincepri/bastion-host-flag
36815e1d849da08cd69515586310395558b5e126 Merge pull request #1481 from aaroniscode/lb_reconcile_sg
55ba7167a3b1cb94d13735a4ab6b263f37edbc83 include security groups when reconciling load balancer
3175195b20146ea20ec00d4717e3695261b867f5 Merge pull request #1480 from cpanato/GH-1411
c27881d39902aee68b1fbf5198bc37185b9e1c80 Fix when AWS return InvalidInstanceID.NotFound with statusCode 400
a9ce8a3a0bd763a6167d2732bdaf0f8f4349ce11 Merge pull request #1456 from aaroniscode/lb_security_group
412dbb0c81f8d7bf9a241dd8719e5c9ad6802fb8 Merge pull request #1470 from fabriziopandini/add-clusterctl-settings
3190af2609f5798c804924b5c4bc04c0d2d5e075 ELB for API Server to use separate security group
c0b06ab2ffb33b41571acb3162aa6c79050300ad add clusterctl-settings.json
75271f7b51f4a1e358792754a1c890b167d62460 Merge pull request #1453 from aaroniscode/vpc_delete
54606074d22e823da6c984d89a8582f31304d6cb :sparkles: Add support to enable/disable bastion host
24798b0715c30e43b2206be5257803358bff7d76 Merge pull request #1465 from vincepri/fix-e2e-cabpk-kcp
90d5a68582e08476c056ae31b393a546af59bad2 :running: Install cabpk and kcp components in e2e tests
09bb239953cb8a7c69212377d4913bb341dad9de Merge pull request #1463 from vincepri/remove-get-rootdevicesize
938b413284b19bd256d0a5ced8127df20e603c11 :warning: Remove check for root volume size
0525403d47f547cf451d42633bfa32e42478115f fix vpc delete with vpc id is not set
9991024a9cb401e8b3366aea5b647f82790a39a1 Merge pull request #1458 from wyyxd2017/hato2
77ed7305542454ca2c7ba776abafbe7c2f0396b5 Merge pull request #1447 from aaroniscode/eip_events
84ab8e5e8b5c743fc1ede4b86236cbeb7cd1743a "url 404"
cd85264a434df83f9eee1c321a644a49e23e1e3e "url 404"
49faafe2639839756a54ea4e2e85205ba3b6fee4 Merge pull request #1444 from vincepri/fix-panic
6d5b1232d5b75325ef3c1d8dfd64a91a82f7a450 Merge pull request #1446 from aaroniscode/event_typo
f097949fce23751f2c694d37999b768de6193f6e add events for Elastic IP allocate/disassociate/release
7f25c858442228187a150a9eb70715820ef31c13 fix typo in SuccessfulTagVPC event name
771cc36739e14ca484c1ebcad90724d04f437749 :bug: Fix NPE when instance doens't have a root volume
3ac16430dc6e72343f9478b58cde11c6d4c48e00 Merge pull request #1433 from ncdc/gcb-for-tag-image-builds
6f3414023e6306ba1f22a9ef7f12cee75550aafc Merge pull request #1421 from vincepri/update-routes
bb16b638dd0a7858dcf754c4e43c0bcc6fe9e1ca Merge pull request #1434 from vincepri/exclude-pprof-sec
e2f21e5770e01896c9a914d0a7b80e46b2e7eb45 :running: Exclude pprof lint warning in golangci-lint config
6647f9915f27411f03cef1a68cce1225a6b724cd Merge pull request #1430 from vincepri/go-113
5b7375f201783f6f104ee4c0b2bf8a09a7365166 :running: Update Go 1.13
994d1d1c3debfae8e55dc52798c4361f4f7694e4 Merge pull request #1427 from aaroniscode/user_agent
6b4377c320953ed6bc554dee9080cb131b4c343a add capa version to user-agent for AWS API calls
0f6ef1f781f05da833b087181f96794453926e53 Let GCB build release images
3344c09966400f2b859de144b36e2cc5a7b64c3e Merge pull request #1432 from ncdc/tilt
0b37715bafb09bbda802fffa081f0c3ee2b4d571 Support Tilt for local development
169f72dd7835bef00e08b6c76ed194b76fcff2a1 Merge pull request #1431 from johnharris85/clusterawsadm-allow-additional-policies
73f90efdea5df74e427732857f537da7fdde02f5 Fix broken e2e test
b94a2eadf662bf444876c2059815e42f833dd8ba Merge pull request #1426 from johnharris85/clusterawsadm-allow-additional-policies
a235482b1e7933e1aaec703e80fb3c9aebc371bd :sparkles: Add support for extra AWS policies in clusterawsadm
e2a2954850f9dfc6b495cfbbd87e79d589aae290 Merge pull request #1424 from aaroniscode/elb_subnet_fix
9d71ee832a072e61d75cbdb3c5d34995b380750f fix elb subnets filter
0615db48dd815c11e3d67f5c77a2dfbcb2112b2a Merge pull request #1420 from vincepri/failure-domains
0f2b8dc5e00dd28ca19e6abb1304b1e48017aab2 ✨ Add support for failure domains
c300be4a01d7f8a928633746959d935cea9c7297 :sparkles: Add support for updating oudated managed routes
0764a5e6e5ba69f525dcebaa2832d545e045df64 Update module dependencies
e04e021940301004d6fb1bec31af6205b8872b0b Update generated files
47f89b4bfe93c34b8b4615dbdd12d2a5bbe05a45 Merge pull request #1415 from ncdc/cross-platform-base64
bbfa1e9540231f66f5a5077eb77bd2733b3884da make create-cluster: use --decode for base64 decoding
cb61f1f6bf891ac75da610f51dfa791f23c53d7e Merge pull request #1412 from vincepri/fix-e2e-imports
23f1114156c84ba76d9ef5a665089210694bd607 :bug: Fix e2e CABPK imports
e19e0e50ada52312f7c1b5decc761e0700f17d5b Merge pull request #1409 from detiber/moreCAPAFixes
fc8feda033eed3ae4e3115108929bf06e032e5ee Base64 the User Data retrieved from the bootstrap secret
25ddbc1581a9c3b05c99d407c11742beac7225e8 Merge pull request #1408 from detiber/capaFixes
c79c56e92aae1e88b685832e32252ae414fd37de Update RBAC to add getting, listing, and watching Secrets for bootstrap data
920e3de666c8de703bf3f6b6c40a35eac3d0cb25 Merge pull request #1407 from vincepri/data-secret
039240877554ca36ff09b883b1d1d8f2a7309c6b :warning: Support bootstrap data in secret
63fbc20d963bfa72cbb9cc731350bd965c4876a2 Update module dependencies
e91f9e35e847021051c7d7b5e42cfc24cb3c532f Merge pull request #1406 from vincepri/fix-cluster-name
495af19f670756c8188cf526432761235153837a Merge pull request #1405 from vincepri/hostname-fix
1dad398c4a31fe38f74fd812c8a2e6042f076b61 :running: Use variable to determine cluster name in create-cluster
493b2766238513f3dbb2eb9b21b85c12aba1926d :running: Use local_hostname in cloud-init config
9b0ce59c661d5c89cddf1b2faccc7bbd120fa00d Merge pull request #1404 from vincepri/remove-clusterctl
c38e6a743b95accb3594ec25086f9ad1dae129d4 :running: Remove clusterctl calls from create-cluster / update CAPI
7e012a803e5662e3210f0670028231ff39a79940 Merge pull request #1401 from vincepri/kind-06
bf31a14decf2add6b6eeed54637896243d71cd21 :running: Update to KIND v0.6.1
98bae8fc10002ce469cf065b73576b6330315d33 Merge pull request #1399 from vincepri/update-kubeadmconfig-v1a3
a2cf7c3d1c04ce38928776783a4e7249db841ece :bug: Update KubeadmConfig(s) to v1alpha3
69e35b2f1532380c05d165a24fb22666d9ae04ea Merge pull request #1396 from ncdc/fix-log-dump
b73742ec1992ba3cb253f1caeb978bfd6ce505a1 conformance: select correct ec2 instances
8062b54b463d9c0bb926be916f68b26f702e874a conformance: try capturing all VM logs
a33871cab0294f58435ba0a8dacbe1316ddd3809 conformance: better gsutil handling
6c77690fd211421c866f432bc8c906d06313db99 Merge pull request #1388 from ncdc/conformance/unique-cluster-name
8b343d309cc93c1302bd0ee15ac37eed34f09a06 Make conformance cluster names unique by default
46e30fd6fc12f3a11d980f16ebb9faf67df77dd0 Merge pull request #1385 from ncdc/better-cert-manager-wait
9cb44e974f110472510eb64fecbd001896691797 Correct MachineDeployment version (alpha3)
d086cfd983420d25e57c82f800015df47805b318 create-cluster: wait for capi/capa pods
8b3851de717c3c08f115cb281d1909a9b2ab8365 Merge pull request #1386 from spectrocloud/cherry-pick-elb-fix
e0ca0328e8aeaa7723dbe79d28106783d4f913e8 check for subnet nil pointer when register instance to apiserver elb
1bfd9534ba4ac3c549048dc079538ca9560ff6b2 Remove the other cert-manager sleeps/waits
ca1a311cf94d25ce296538300b56b860adfe2fc8 make create-cluster: Improve cert-manager wait
06ec59c1f788ab5ddefa6006c7a3ebc32d8d39f7 Merge pull request #1218 from tahsinrahman/validate-awsmachine
af1e8a307c47c8d5d593bd841f1f4b9eb0447364 Add validation webhook for AWSMachine
8ae81eb833e189aaac8b968765cc4e42066f320f Merge pull request #1382 from ncdc/add-elb-perms
b8a6eadf6aeb1f5462f66590ea6276e3b4f3a8aa Add new required ELB permissions
6072cbc5ba5674189538d7fdc8652db86dfcf2c0 Merge pull request #1371 from vincepri/rename-makefile
03acfaceadb8885d17228b1053801a9eac97fc69 Merge pull request #1380 from ncdc/fix-e2e-import
0cff8c9b0965619a034348c6e54f48d7abcf2628 Fix kubeadm types import
1eddbcf1de6c6d0a8a086e5ed5bc65b039f48793 Merge pull request #1372 from vincepri/cluster-spec-controlplaneendpoint
8d84ac70b6a39619b80ecb2a7df8b8ead2a43241 Merge pull request #1377 from newrelic-forks/rudoi/elb-tags-master
6ca857fb781e485d1946f687f3b5f0a95c7db15e chore: reconcile apiserver elb tags
b1cc2f6f9c68da45dd114394c4c8d65322e82891 Merge pull request #1340 from vincepri/maintainers-update
bbc9fd7667c986a69c5ea502f85cb7c08793d7e6 ⚠️ Move Status.APIEndpoints to Spec.ControlPlaneEndpoint
73e4356bb5da2c0fa3618e71b0e672d10c2b720e :running: Rename Makefile dev target to create-cluster
40a6a24f7306a04e29ea180d65e65e83f15e1503 Merge pull request #1367 from noamran/ct-0.2.3
f0e02e37b8d13009dad5500f9925edd3d449a2f8 Update controller-tools version
089e55b15a1c711f7db67212c84ce03fe60e3143 Merge pull request #1365 from ncdc/fix-releasing-doc
d908e522e2f1016b94200a70f89c5966fbd7544f Merge pull request #1366 from ncdc/remove-git-branch-from-version-info
f33b041e62fc489f4300ae23451558d46ac224cc Remove git branch from version info
fd0fa6c72039560c28df83ae3dfa95e218eaa899 Correct outdated information in releasing doc
14101ecb222301677ad0f7a1819d02b0fbbeeec9 Merge pull request #1352 from noamran/1350
21219ef8ce957f1c386216dbe4b0add5869b4c78 Merge pull request #1358 from vincepri/cherry-pick-awsmachine-updates
56e3a548be4b5ca3075822b34fa0797bb64ff915 :bug: Validate AWSMachine updates last
8475046c7fb83ea406dc54d761e30936554ecf10 Merge pull request #1356 from randomvariable/awsauth-error-global-recorder
573d7f053a9a5ccbb2ca745cb687325f814c0fc9 Add NoCredentialProviders to list of authentication errors
82a11a03f6240cd967b89085c533517cf1a25edc Rename ErrorMessage and ErrorReason to FailureMessage and FailureReason
2dc2fe8e5e968b474ee1cada99609496f0bd3af0 Merge pull request #1345 from yashbhutwala/fix-example-generate-script
6e4259c9bcb132172e96ce0d4035ff957e3cef8c point to the output dir in examples generate script
651566d34bb7ca79b90e1dc2e835c7333d7c1f80 Merge pull request #1319 from alexbrand/base-os-field
2aae9e696343cdd989fbedb58d62683c963a4e37 Merge pull request #1338 from dims/fetch-logs-from-nodes
a7bcbcbe9c0152a35f4a2cd574417931b84f68c4 Merge pull request #1256 from randomvariable/log-for-events
ff912c8959a99fe319325b9072c686e8c524ebb1 machine controller: improve EC2 state handling
00a7e702ad09cff1a8ce57210f19fbed16fcc8e7 Add conversion code to AWSMachineSpec
9881dcb154befefb22bd42c2b6e8974526e1bd81 :running: Update project maintainers and reviewers
dbe10b9b6c1deb7e3c87f8ef6407d7fe3f914f68 Expose ImageLookupBaseOS field in the AWSCluster and AWSMachine CRD
6b2a2e8af8293cef97905e4c1672e3c92d88eab2 pkg/cloud: Collapse base OS name and version into a single parameter
f02497b20f3a1149338b29de04faac6ea545f9de setup better defaults for cluster name and ssh key
3599247369fd59e76a7bb92ad2956509f6a9127e Merge pull request #1305 from alexbrand/fix-docs-readme
5a137c11ed3b497e26b0cabaa708cf313d8adc2f fix typo
ed5aba3f75b8518eb165000b60e49ede6da094f8 Fetch logs from nodes
2f6834f4ac76e9e65bb8cf511e921677a5abcb93 Merge pull request #1329 from noamran/1204
d2b508707901ef02f3e64fd75110670736b49b01 Merge pull request #1290 from randomvariable/lb-name
3ede0e1581da5203065e187568e2f67442005637 Merge pull request #1337 from ncdc/fix-examples
6a0a88d75f9ddf72cc8ad55b45260138d80404e0 Remove generate-examples as create-cluster-management prereq
a02982c452555d7f184b7ac70012657b9f7c59f5 Fix IMAGE_ID issue in examples
1a194d1d98322ed6db5e891162a61a51a162dc13 WIP:Conversion webhook
739d9d96ce4f2cb16028eb56a929c73b1e5d197d Merge pull request #1334 from detiber/e2eTempFix
28c045239b8cd7748b5366afd219a7e65ef67611 Merge pull request #1320 from vincepri/update-kubebuilder-1155
2f2c8dabbe81ffff6af5075e2c265c82577d9420 Merge pull request #1314 from rsmitty/master
9cf4eeee3b6250ebabfdf9791a18db648fe6167e :sparkles: Add addresses to machine status
4d73b0af2b2d0921754a7977da1536067024436c Merge pull request #1333 from rsmitty/issue-1332
1087b566d2fb266bbf32de35bb281633585f1f21 Temporary e2e test fix for cluster-name label not being applied for machinedeployments automatically
6e6ef94937a92e18882227c47000158a73cc4f96 :running: Remove converters.SDKToInstance references
597cd8381735ca42725b8ebf0b4bc412a7028292 Merge pull request #1324 from wfernandes/fix-generate-examples
02645d5f89a3bf1dafbaffab438b121f19c828d2 Add cert-manager to output of generate-examples
abaa8adca55de8afbb46507cb9cca08d84a7cc1d Merge pull request #1321 from detiber/moreLogging
09d19619d97495cd98e611917b77bf5197da8e6a Merge pull request #1330 from dims/fine-tune-e2e-conformance-script-1
24c8a825737175766bddf1a0cfe0f1af90edefca Fine tune e2e-conformance and ci-conformance.sh
61a6bbf653db67fb3f5da8519af81cc74ade2ef0 Address feedback
fc09c9fe74184536041bdf6e6c87abfb0743c247 Merge pull request #1326 from dims/patch-1
feaf4af0b595919fd99ebe1c2986098f7862666f Merge pull request #1325 from dims/fix-path-to-image-builder-under-pod-utils
28ac847d621452e5e392130df0ea3ef6cc6c0bdc Allow passing in parameters to ci-conformance.sh
9a90e8c97ea84f1f4c22374afa295dba2045546f Fix path to image-builder under pod utils
729b44aae9b3e536ac0465bd2a97a2d1a732ac27 [e2e] Improve logging and add event logging
f8e50a917bc79b8b575b35a0521e578ee2c1ee10 Update Kubebuilder / k8s 1.15.5
78e5ef40f9f5c863e1c2fe1f8d81bf33ccfe858d Merge pull request #1316 from dims/better-command-line-processing-in-e2e-conformance.sh
2b33e872f15c54c932d24e8caa305fab5d026144 Merge pull request #1318 from detiber/e2eFix
ea3fe4828d0197708cc531abb4b6864f45477988 [e2e] Fix up MachineDeployment for latest v1alpha3 changes
21adafdebf971a3c48de75506cb8fae8051051dc Better command line processing in e2e-conformance.sh
e88e3112bf450282f7f95a01c4238e140cd59fb2 Merge pull request #1315 from detiber/e2eFix
332f2f13d1df540788cd7f44798dfb62ea354e62 Merge pull request #1280 from dims/fix-up-e2e-conformance-tests-against-master
da64a0fcd54ca867287eddd08c8617eb976d551a [e2e] Update ClusterLabelName usage
030356c164f5763b09c2cca8aa551da74311ebd7 Fix issues for e2e conformance tests in prow
fa3ca34c5a8b06e455722fd7622e67ee21704b3a Merge pull request #1313 from detiber/e2eFix
d6b4f4b1d0a329bfeae064a752be564f1651e7d9 [e2e] Fix e2e suite
f69282c0d6af4a3a47bb60160a4076ba0e12f0fa Merge pull request #1309 from alexbrand/cluster-image-lookup-org
ff22a42fd0d650032a842eaf80e0ae561fed97a8 Merge pull request #1296 from detiber/fixe2e-master
27cd81b5393cec5021ae6ea1914a8989f3c8e83e AWSCluster: Allow setting ImageLookupOrg at the cluster level
e52b8099f21a11a60737f9951dc0091a54f0e830 Merge pull request #1312 from detiber/e2eFix
e9d5006e44dc9a34c3b96d4c941a36e24b760afe [e2e] Additional e2e tweaks
20689ae489cabe54e3a5f4301cc8eb51412fd85e Merge pull request #1304 from tahsinrahman/fix-make-mgmt-cluster
bb0dcd3b2e263ee730f016d3ff3f75861ce1fd20 Wait for cert-manager in `make create-cluster-management`
aeeae3083c48443c2fe2e15ae5450d818a783f2d Merge pull request #1311 from detiber/e2eFix
19e36f038456c158c76bc7ff92d8a869989be2a0 [e2e] Update e2e test to use upstream cert-manager
f6abb265b110adabba69c72a725f93e9df9fa1db Merge pull request #1310 from vincepri/update-certmanager
928fa22503b98b53a0f4772ff5eeaa1adc2ab647 Update cert manager / fix Makefile targets
c382ee361e414ed7c76f93b85d4c58c70e0cb274 Merge pull request #1306 from detiber/e2eHeartbeat
9e05991335ce910e805f6480aec3abf30407e5f4 Merge pull request #1308 from vincepri/bump-concurrency
0783b1734a30d6d6528abe5cbdf76cb9330e49f4 :running: Bump AWSMachine concurrency to 10, AWSCluster to 5
22f62f67aa3c3e8e104d9e2b45e4cab946b01712 [e2e] Add boskos heartbeat
db9b4821ac33377b6128071ede82660a044978ba docs/README.md: remove broken link
b235996f23152b2e2ad76d21bfcdbf7e297cd37f Merge pull request #1303 from dims/drop-cabpk-from-manager_tolerations_patch
f362414d2e27fe38c6ba33cd5cda55d90c27bff7 Drop cabpk-controller-manager from manager_tolerations_patch.yaml
eaddb1095bb2d57423b095f1eed1eeb50846fc80 Merge pull request #1302 from vincepri/fixup-examples
54205ec10aa5077e577c4ea5987c0f0a50e05429 Update generate examples to v1alpha3
d4872a5ef85572e4e5af018d695808e37b3d3260 Merge pull request #1299 from dims/return-error-when-stuff-fails
844f14811a01d0e6d83909c384f0df5eb76d8b57 We should propagate any errors during create-stack
ed567459fc086e625c769a79313a303fcf98355d Merge pull request #1298 from detiber/deleteStack
a178923290af537b8ee6a666b3edd2de0386cdc2 [e2e] delete cloudformation stack on teardown
769de6806c6193d74ab258ffaea9627fc0b4de6d [e2e] fix machinedeployment scaling comparison
b5ccf030fb8ccdae2372cf737c011936572b7d3e Update test/e2e/aws_test.go
dfb17fb1086d5c26f6dae3eb4546197a6e6eb814 Add MachineDeployment, scale up, down tests
c4e587a34bb610d00cfa766c0bf84f6568b175e7 Merge pull request #1294 from noamran/doc-release
af793df01baea95a8bb38747773a5727de2682b9 Adding make release-notes to the doc
c3b0776b3f92bc6b0a5e450bb7a3755fa6a41150 Merge pull request #1293 from randomvariable/byebye-build
7bbcd79608aa01101ffdaf5889cb320d22f36501 deleting unused /build directory
0068ee5088cefc19e9bc34d71313705d295a712f consistently hash ELB names when above 32 characters in length
52ba7f89a8a6f346c68b38989c14e208ad451e03 Merge pull request #1288 from randomvariable/cloudformation-v3
891cffed459cd65f9b7de6cd8dceb432de61076f :sparkles: Bump goformation to v3, and remove IAM hacks
938643cef9df8d41136f8e04060b47791b75b2d9 Merge pull request #1277 from randomvariable/kubectl-get-awsmachine-info
644d254fb49a2cccd1d8005a25ba2bdbe0e88cf6 api: Add printer columns
6fbf99438223907678070224106b34044e5177ef Merge pull request #1284 from randomvariable/wait-300s
46370352161810eda9b55670919f54ebec4f947b wait: Revise backoff parameters
92228c7031b2c470edb93d7e1b95a60082bb70c0 Merge pull request #1281 from detiber/e2e-junit
ba3ef043afada0bb42a95b2a713e919abcd419ef [e2e] add junit output for e2e tests
d8deb7eed0a8b9a05872ba3326c93e97796a5535 Merge pull request #1276 from randomvariable/consistent-events
30860ec01031bc2e638314955a59bbbcff26c55a services: Record events only on AWSMachine
ac1993a2f7324d6df31ca3b0a4187b3892bb35c2 Merge pull request #1273 from detiber/fixMachineReconcileDelete
afa5ca795d27970e215d457c38b72ad3ac321ea2 Fix Machine reconciliation of deletion
9237cc4c861283129e5fea04e84a9f917084dc8f Merge pull request #1271 from detiber/master-e2e
04ef30da17146305f6c7145e3854270119dfbc85 [e2e] reinitialize the kindClient after deploying the cluster api components
5d8fd5303918e32d7ec95dc33c91c699d80d5c60 Merge pull request #1267 from detiber/master-e2e
07a641bb2d7e716f34e75462a70a0285c1f7b4ea Merge pull request #1269 from detiber/updateVersions
52ed9d2109cc0cc08ae3556698948b2d83384f2f Update available AMI versions
faa2eb16a9b2ed22854e5708b86072601e4b4982 [e2e] Create access key after creating the prerequisites
1c58cd4c625bb0e716e36d0415c1db1a9fd7f1fd Merge pull request #1265 from detiber/master-e2e
856e27d566d499a516a4ee84e2f3098c92245abe [e2e] more e2e fixes
725074b691d426a96f509270d541c2f7d3c6e080 Merge pull request #1259 from detiber/master-e2e
ea1055ae8689da22b53c4ec421e9e069ed4d0e0f Merge pull request #1258 from randomvariable/disassociate-eip
3308e677b1606491358ad4e56bd77a2376a7ab67 eip.go: Disassociate Elastic IPs if still associated
6c7a7fea44264b468d6fd5921bcd1a8fd36535c1 Merge pull request #1244 from liztio/test-instance-delete
1b08dd3e04bbf3887c3bfbff0afdf824bba4f15a Merge pull request #1263 from aaroniscode/internal_elb_subnet_fix
d7806edd0d9a3f3a3b6bf9a42bb084c2a9a6c396 Merge pull request #1254 from dims/scripts-to-run-e2e-conformance-tests
1c5638c45faa6ae55dcb03c5b42d9249643ac6da choose private or public subnet for ELB based on scheme
7932bf7d29521f880a40fe2b11d8548509f89cb8 e2e-conformance.sh to be able to run e2e tests
e2d0ff39d6cf17a2473b4d283bbae49fa2f31b41 [e2e] update credentials used for controller
af5c36445248ec194db6cc79d0e1f2ee3ccb7677 Merge pull request #1257 from randomvariable/run-from-cmdline
fc2c33721a267cddb4b294e387728158ed2caef0 main.go: Add support for configuring leader election namespace via command line
7f7dc49a5cdc7299b02bff5c6d87a5832337c9b0 main.go: Allow disabling of webhook
b1903bab4121fb0ba1c921460d63ae741f389949 Merge pull request #1250 from dims/allow-injection-of-a-development-image
8eee112917483ad534671cca9e78d3e052ed822d Merge pull request #1251 from detiber/master-e2e
604b2ece3b3a056e683f115dd01ceec8dbc58710 Fix verification issues with e2e test
e7fbccb9beb4b5538760efc72aee3ef272cc057c LOAD_IMAGE to allow injecting locally built image into kind
bdbf52db29a42850272fb245538cdfe7bc9c1579 Merge pull request #1248 from detiber/master-e2e
275524305627c6a18efd3d024d41f31d7872a463 [e2e] Fix region handling for e2e tests
60a093481549c2729a5d2e42d6eee90ea99c55c1 Merge pull request #1245 from detiber/master-e2e
60db52d26daea938d1813d6f78da85ceb9c7d755 [e2e] Fetch controller logs when tearing down kind cluster
101c68eac91844ad01ba366b5f43f072888525a3 unit tests for deleting machines
aa0b18efc6accd2ae3debf1f27d1d6ceaab2f5a5 Merge pull request #1232 from aaroniscode/fix_clusterawsadm_version
9750b2c6000754413d6ed3df74a3c81b14f047f9 Merge pull request #1197 from liztio/machine-controller-test
19c6d3f7bd70b8e6929846e9ac5ea853208a1002 fix clusterawsadm version that broke with removal of bazel
1728e1d752e84ec1dbd3a525c436d0181588e1f9 Merge pull request #1234 from randomvariable/aws-sdk-oct-2019
945ef3c565f287022783d0bbc646187cb12b3401 go.mod: Bump AWS SDK to v1.25.16
172c72508a4eef74d937845329aa9e0d652dcd12 Merge pull request #1231 from detiber/master-e2e
0fb1914ec54dde049df15c948c17a1d90580d802 Additional e2e test fixes
99b5d357bc0b4b5f0396094f9a6d60506b9c9915 Merge pull request #1230 from detiber/updateWebhookName
9bc1891a995758266dc259fcd8e8ccaf237b2644 Fix AWSMachineTemplate webhook name
5507747dc630a58371e184a42706b5d30baa759a Merge pull request #1219 from detiber/updateWebhookName
eb44fa27fe69656651c3dbe368cdf4454ca08cc2 Merge pull request #1229 from detiber/master-e2e
e3ceba9bb6371ddb6392b901fb54f10f4eea7d84 Update name of AWSMachineTemplate validating webhook
25d74bd156adbd56170b85396aaec0bfa4c79ba5 Patch up e2e tests
7936a886530d07e76923ae6c6c4a982581374fb8 Finished reconcileNormal testing
20ff90a173597c140fae53d64091ae611dd7658b EC2 Machine Interface Mock
58c6b0a0ceb52e215692270d2814e602c849ea2e Some basic unit tests for the machine controller
813729a71d3ab476cb35de6e9d71140a7c8843ba Merge pull request #1226 from chuckha/cabpk-cleanup
79787e50859e02c4b37c2c540da4d46533c8ec8a Fixup code for cabpk merge into capi
ba9cd02a9c42a74d8dd03d2163ebbec60f83d5dc Merge pull request #1225 from chuckha/dev-dockerfile
bd7966f530caceeb50f6fa60935c7a38ecaab8e9 Cleanup dockerfiles
ceaebeee0a62d282bfdfd8a7086fd22e386dcfb8 Merge pull request #1224 from randomvariable/doc-update-2019-10
07aec8f16c2bbe63e80a5598294802dd288f1488 docs: Delete obsolete documents
67e862628f5f17e17c511422eafb4da7c6faf504 Merge pull request #1223 from petergardfjall/default-bastion-image-for-eu-north-1
623c6e2f27c6022a782223524742f58dd4c88701 add a default bastion AMI for the eu-north-1 (Stockholm) region
9fa23f8eee2b1d72b10a062384da0b2d25ed4cee Merge pull request #1221 from tahsinrahman/fix-retryable-error
72b6fc62fde5dd4c6f225500a11e8a57366f14f6 Merge pull request #1220 from liztio/capi-v1a3
d6cb088a47573efd1d07bd663f2279497fecad42 Cluster API v1alpha3
5477066c3bbfd63dee19b272d03aae23e2fbb3be Fix WaitForWithRetryable should return latest error
e85812c6eb63a779f47145d4ce0b8619a880c37d Merge pull request #1217 from tahsinrahman/fix-wait-err
ba17aaf4d5c53124721352d74b60c1a74e101da1 Surface inner error from WaitForWithRetryable
ccf11ac2a1812fa6efb388ef312fb459200e14d3 Merge pull request #1116 from tahsinrahman/webhook
24430fd9c01755cdfadd921a212370afb44e1de0 Add validating webhook for AWSMachineTemplate
9c2983ac66f82294f89ff6a5f05353780db1cbe9 Update config/ to match with kubebuilder 2.0.1
468f1d6110e14f51a6d4c4b129c5c583c1358e67 Merge pull request #1213 from alexbrand/fix-natgateways
34d21a0007802620fa74cd16594e6b78f2c7155c Do not attempt to log NAT gateway ID when creation fails
8c336af895ac4bb83555597eab6cebd2d13efd60 Merge pull request #1212 from ncdc/fix-v1a3-version
e68033f5673a5df51f17e04b602fbf28b366e622 Fix API version in v1alpha3
6999f6dd5d41f63e7b783d3676bd6b484a31e391 Merge pull request #1210 from tahsinrahman/add-v1alpha3
618136bc1bc409896d97a875fda6111668629e55 Add v1alpha3 types
54abebdfd9a0b4caa3fb63b2e194dc4a8db050e7 Merge pull request #1206 from tahsinrahman/remove-v1alpha1
bed0b7c341de102b9f934bcebb74c68687d35e5b Remove v1alpha1 references
3abd1936dcae8dd5165f5cbc6b3ed5e568120286 Merge pull request #1198 from tahsinrahman/sshkey-name
2aef6f7e2bc6ab30fecb0c271d4012ce3f026017 Merge pull request #1199 from detiber/updateControllerRuntime
ff4d99c22594ca6e2f68934a11cddc0b71e006db Update controller-runtime and golang versions
6d639aac5eac053f0ed92ac8d50c91e40965ef05 Merge pull request #1181 from randomvariable/instance-deletion-logs
be6d84e9061ac7851fb93e47475a0e9fed7b5b18 awsmachine_controller: Add note on how to reach bad state
e1548068c9b2b315d3838817b67c9788932320e0 Use sshKeyName from awsCluster if not set in awsMachine
6bf9d72f6039e4d037c57a9075d6b52dbb38b2c8 Merge pull request #1192 from Sn0rt/bugfix-add-tag-permission
357c69a266d2654a278dacda39e98ca94ab7f6f3 bugfix: add permission allow controller get elb by tag if delete cluster
1d717ad21861b151cd3ba1714f06b94f03fd20db Merge pull request #1196 from ncdc/routeTableID-omitempty
c123d2c26c88415e7fc54494c4cc20de71363d4b Add omitempty to RouteTableID
4981051c285fb36f0ca657fa4df252d9d7888e13 Merge pull request #1194 from vincepri/released-components
dc65b4e5dd49f08be88bff59d49ef7db4b735a6d docs: Document events
b9810524addfbed93e02ac2eaca2f68f8302f5a5 :running: Use released manifests for CAPI and CABPK in examples
7447919f85328d496b2fba3f4e4cf3d5b58c896a Merge pull request #1176 from luigi-riefolo/feature/webhook-port-flag
f6d29dd7400ac47d0c6699c9badaf4abf97f2ce1 Merge pull request #1186 from detiber/cleanupE2E
be25807d6aff62d6ebcd8effabb1eadeb90fd029 add webhook flag
df52f73b074f1042d90275eef911a15fe0b0957f Merge pull request #1188 from chuckha/dev-docker
7d6bc98fc57e4bd45f293d6504321da0fd45bb79 Add a development dockerfile
e416350a197baee3320cbc071fbbaca4573aff0a Use e2e test helpers and cleanup e2e tests
8839e6cc740ad7f3dc3c17e9e9907d02d65ded95 Merge pull request #1179 from andrewmyhre/873-add-control-plane-load-balancer-options-struct
d1f5acc16479ca64e84e9c2c1ebf23a16503de48 add an AWSControlPlaneSpec struct, attached to AWSClusterSpec (optional), with optional ELB scheme property
38a0a2579fa464ef9e186cc0444eb592bf325e3d Merge pull request #1184 from detiber/fixKustomizeScript
26930749b63e2582d5097551e768433fed5ca32c Fix hack/ensure-kustomize.sh
08306b2431a635f4ced83867e0378958ef4d441f Merge pull request #1183 from tahsinrahman/verify-codegen
9603d51acfa9aa3a7b8d5dc2cd7d334bfc1b6aa2 Run make generate
f6c34bfe49adb126abbfa15bfa35a4708ff07913 Add rule to verify generated codes and manifests
b4a936dab6ef30ce7aa6d85e1177aa0f2283fe40 Merge pull request #1168 from liztio/lb-delete
25242418c68bd1ed4c83e7fc6f71c20055ce9ee0 Merge pull request #1177 from liztio/tags
7192bb3f55455b6820f4991ca70c6e93e53d481c Delete cloud provider provisioned load balancers and security groups
c4170d4cfccd69f83f453df41124d599572370f6 Merge pull request #1182 from randomvariable/control-plane-iam-profile
7cd7b11cfa25c86ca9e83d66ff876b09b45f5134 examples: Correct IAM profile for control plane
f5b5a4b7c81423e5466c1c81f3a2504c51bc029f awsmachine_controller: Log EC2 instance ID when available
1860fc02778a4b434ebea6b337bfb53f8743d0dd awsmachine_controller: Record event when instance isn't found
28949dbe4f3f5e0f4e5e2bb8c5e1cfe14aecf9ce awsmachine_controller: Change instance not found to log-level 2 More in keeping with logging conventions https://github.com/kubernetes/community/blob/master/contributors/devel/sig-instrumentation/logging.md
0b09df056064abc14513e2cce08056bf992da90f Merge pull request #1178 from noamran/1172_uniqueID
d9ea6c068151e91ddf6fcc79715676748cfeb8c0 Merge pull request #1163 from vincepri/increase-concurrency
7f9311cb01369323beff516af10eaf32d2423beb Merge pull request #1174 from liztio/tag-subnets
b45f52763cf66ea48c49a2cf1957362ab70a04cc :sparkles: Increase AWSCluster and AWSMachine default concurrency
3f145a9192fbec8ee9b4cec0be1190cbf7c6948a Setting a unique LeaderElectionID
935f4a6656309f5bd51b69961811cde90b664f08 Actually apply explicitly specified subnet tags
3a5ffc9ca728571bea546834dbc59908ca2f1592 Apply elb-related tags to managed subnets
feb358010d79659ffdca2a5631f74454053271ac Merge pull request #1170 from andrewsykim/tolerate-manager
b20492c832d6b39d32d0aa06171238228700f84d add well-known tolerations to released CAPA manager manifest
c6b8c307095892de15b1edcf8d610967dec77750 Merge pull request #1165 from henrykhadass/docs
0551b1744cf37ee8dedda8d2fa3429a2a92715e4 fix: cleaning up readme.md
32a1c96126717349b0c27b5ae44814fb688044a8 Merge pull request #1162 from vincepri/update-utils
7a92e012ddfd973cbacefd9efba1880ca5b5b2ec :running: Align Makefile (release) and hack/tools with other repos
f16274ed1b09dc1e94026d24600405b5f80ea0cb Merge pull request #1159 from vincepri/prereq-cleanup
b41790eb526cf854eaed9fc53cf498305504f2ef Merge pull request #1122 from detiber/e2e
a9de379916ed69659939fa488f8e4e7624fba4e9 E2E test updates
8d116c5e19a36bae586eb727fcba6aaa82a25700 :book: Improve prerequisites document to be embedded in book
6c52422bad3e9f58af8a622887d61e26faf20bcf Merge pull request #1154 from yukirii/patch-1
a2c5f9ebcae13eb3818c1e1d110659417c9687db Rename link title
0dd895830ee1efa3e5e2fd6b6ecae2e3f24a4a69 Merge pull request #1153 from newrelic-forks/fix/tag-leaks
4e1622da596ef78badb34f390cc487f318d1f628 fix: incorporate review feedback
d97a8ce69fccddfe9edcc40ddc1f5cacf919b7d7 Merge pull request #1124 from liztio/disable-event-throttling
4b22bf972295b006ae3129d8395cbbb49d9f7734 Manually specify broadcaster options so events do not get discarded
dd83df886eaf1ec36bd68877354ca88ba768931b :book: Fix broken link in docs/development.md
01da761abb58b6d7ba5df784f6e9f4e96d5869f9 fix: misplaced ownership tag
958c95e3c9289ca808bc7c98e6c62f70164506c1 Merge pull request #1152 from newrelic-forks/rudoi/perms
c3a82a689f5971f25838e9f96a7c4b281b7107b1 chore: log security groups always
565f5a78a932214e049e429fc2296055a15ff3e8 fix: update comments
59dffc72955c8826cafad939f25471c496566f5b fix: use copy builtin correctly for security groups
e5a284445798de7c969a8e3ec7bbc32ad0581c1b fix: add DescribeNetworkInterfaceAttribute permission
4306de8187b64742ec045783b073ce6126f37cdc Merge pull request #1150 from detiber/fixTypo
b1ba6b5a02ed570aefea130d4f74dbcd028eab9c Fix typo in readme
ec57d028302444da734ef5f7173b8148427df4d2 Merge pull request #1149 from detiber/updateAMIs
8f733aca873ef4257ed3ef96e8bdb6756ab83cf7 Update latest AMI information
df4c6521593153641fb75dae2038adcd6d66b7e0 Merge pull request #1136 from tahsinrahman/log-name
3739742ab5e6d55618e9426a7a4aad8f64b52124 Fix log names are too verbose
32c0546a557347b36302aa637a1c9e760ba41bcb Merge pull request #1131 from tahsinrahman/check-mod
177952a51cae90043a96b067220eb4f21b2fb8d0 Update go mod files
0ccedc6bee9acc70eabcb6df35f2bd2c1aea64d8 Add go mod verification
6fdffa11c15d1c1582e31d605587b892d03ec7ce Merge pull request #1146 from newrelic-forks/rudoi/eni
c2310d09b0488a8d55283b6405b594ef39bf063e chore: fix comments and log messages
10428f06710e226d2b852f029dc752e398576797 chore: manifests generation for networkInterfaces
9e79b7d3fb29f8ea1ada9dee1696dbb2e9b9ca3d feat: add support for specifying an ENI
d64b5dad5922dfb178002899134def861f41a700 Merge pull request #1147 from newrelic-forks/rudoi/listeners
0fe80d3e3d1e73dcfc3cde3f229fa346ebd677ac chore: use scope port for API Endpoint
a667ec69795fb6c257d71ae41569e49e4b932d1a Merge pull request #1144 from sethp-nr/patch-3
841c72a1cdffb85d4ceeeb7a4b9b35ae6fed83bd fix: remove finalizer when machine is absent
256276cd93bb38d4a1d6dae98d376908689c9d5d Merge pull request #1126 from vincepri/custom-apiserver-port
da53a5dd587df80317e613f77b3ca5d126687e13 ✨ Add ability to customize APIServer LB listener port
60b1ac241411f1726e54dbdfaa37d63020c589b4 Update module dependencies
9dc57fdea283fabb49a6c16f3c13ca8d10cc67ca Merge pull request #1129 from ncdc/credentials-error
8d48e1e9454ac7ffc81923bacecf1f4056bba504 Merge pull request #1133 from codenrhoden/remove-verify-install
49aefb95e3e9860b395639e741f7e2ecbdc0aaf4 Remove hack/verify-install.sh
257c5215d85a73ccf9acce343f93f438ee510bd9 Merge pull request #1127 from vincepri/add-subnets-load-balancer
ccad13aecafc3f9ec38bd6fe306ee18ab76a5714 :running: Return an error if ELB doesn't have necessary subnets
7aae5ba02d919b72c9e206f076503b05678ce414 go mod tidy
c5768b355c9ffff8c8b0d7255216354c1b2ef728 Record events for creds/perms issues
c88205c8e4dfd0925ed315f81691536d6014c49b :bug: Register all available AZs (from public subnets) to the APIServer ELB
eb4326127c829e6df73e3648612086d0ae2552ca Merge pull request #1125 from yukirii/patch-1
6c22dcf2f55e140e4e91c4c537aa22493a8d06af Fix broken link in docs/README.md
a49e1dfc9a3180951afdc7745609d3600d978473 Merge pull request #1123 from vincepri/cloudbuild
7c7572e27fc19e7f91253d14b9d5af292f28872c :sparkles: Add prow image building
a745288a721d0509fe853ff271683f7973302914 Merge pull request #1119 from soggiest/rootdevicesize-comment-fix
31e747c609757cacf1021c82b8818b0e7409326a Specified measurement unit for rootdevicesize comment
7bef117bb70fafa6f77946f73f493c8c71657b8f Merge pull request #1113 from ncdc/wire-up-additional-tags
dcd6d564fb545723464ad7c50a3fbb433eb63eea Add .DS_Store to .gitignore
423721d074144de956f70ed95996101e3585758f instance: use AdditionalTags
e92230d5b9feb87daeba38d0cba4fa69bea152c5 elb: use AdditionalTags
cb2bd893ad7848ca64a9fe96eaafbc005a188bbf vpc: use AdditionalTags
312bcc6c616593afea1bf28b8842e0403b11ac6f subnet: use AdditionalTags
bbb864c0e79f3f9b45e6e2bbe4732c0f015996c1 security group: use AdditionalTags
59f53a34558202e669be9b21e1a7a18b9f32d7de route table: use AdditionalTags
d3c1b7f4f38d0886f142f2bcd8a97d4fe3a2904e nat gateway: use AdditionalTags
8ec631effc7d81e7cc8d39e56dd0896725fbdf44 internet gateway: use AdditionalTags
b01f61fbe28beeb4917716bfc2dd0fb15b87570d eip: use AdditionalTags
f07e90e6e1dc29d559d3e9943aa35268ecad63b9 bastion: use AdditionalTags
8ffe3b5ce2945ff4ff98ad74d16765235041f8ca Add AdditionalTags() to scopes
5ba827e29f22506d1392ed172d44b8779841faff Tags: add Merge()
4da4eeb5108ff141f0ade10868cfba29bb793c05 Merge pull request #1111 from vincepri/fixup-getting-started
b56ebfba2d20d45db23b1984b46af404f5a2a6f9 Merge pull request #1081 from liztio/conversion
18cba2754b310bfbca1a3e38bb864abf7000cef9 Get Secrets
9ad82819f9a7158ccba371f9d3ca5e8f9f5f3f16 Fancy new struct-based conversion
4c05a3ea5a1a18035d3dd6ca8064d13182c91a40 Conversion functions for v1alpha2
33dd129c4b4d3e9af7409718c217bfec2f43bc09 :book: Update getting started guide to prerequisites doc
c3bc195aaea2b8b926b92eab868551464251b638 Merge pull request #1115 from tahsinrahman/fix-gen-example
771323ac775c5cdc0beca3229f455dac828d3124 Use latest clusterawsadm for generate-example
81317248556e1f93156e7d5e425e1d98166aa6c9 Merge pull request #1112 from vincepri/update-pr-template
14a8b746b91fc5edcfbab4816d89ad1d38dee83d :running: Remove release notes from PR template
c0a8b761e36b4a425daf67f6487be653d987ca04 Merge pull request #1109 from chuckha/context-cleanup
15640f3563f46f5711e93cb30896aa659093cf71 Context cleanups
80786b684667bda336d547f01afe0fcf66ad1cbc Merge pull request #1108 from chuckha/time-error
6fab15fc65d47d62fd15ffa60e80a5cf1270c6f6 handle an unhandled error
af939037b1c29e2b039cf8b71e69fdc27758d056 Merge pull request #1107 from ncdc/additional-tags
57362442c66ee5a7bd499f48c1be101c4ff1237e make generate
7d510e8052453b7c41d9f8344d1635ef2e5c0141 Add AdditionalTags to AWSClusterSpec
97b7265950d8baaca2149786bd23bab65833a70c Merge pull request #1104 from vincepri/release-binaries
57d79f86c802bf8cc548a25c64181b89d1cbcb2e :running: Add release binaries target
3780d295fda55d3bd70edd38e8f6baf6936bfe5a Merge pull request #1103 from chuckha/fixupexamples
02e3ff9e1bebaaaca69fd106d1d650ccc97c8df2 Adds kind and apiversion to example
e7cff682f95eb314d4e3c967c7b8de837a4cbd30 Merge pull request #1098 from vincepri/update-capi-0.2.0
2b99fd7475531ff214ef924793a515521c0c20c2 :running: Release target fixes
3813e6c4c7dc01bbcfd1e315e94f7bf5bdf23581 :sparkles: Update Cluster API to v0.2.0
f748de96b7941281802d4fcbaf8581cf40fcb477 Merge pull request #1096 from vincepri/release-goodies
9889f40ef3ba8c8caaf3a846d740129e9a490016 🏃 Add release targets
cce5b9455bb20d77cb1bd436ef137f93ee4bf425 Merge pull request #1095 from vincepri/rename-ssh-field
e8b6e3393765b32cdbd2c8132cb4efc7e2811652 :warning: Rename ssh key name field
9f158d13212d63f704ccf8a949dc80cacc0b1fb7 Merge pull request #1094 from detiber/ImproveDelete
c2a64fc639e26baebfb825d5efea102be782e658 Improve handling of instance deletion
89e8ab62a6ee0de8f6644ae44cb7f224fc202f38 Merge pull request #1088 from chuckha/aws-watch
deb759191b9b81ed49f9609069a14659257a19e8 Fix bug with requeuing machines from AWSCluster requests
7990519ea525e7e3e28fcb89d610a200cd7f0fb2 Merge pull request #1090 from tahsinrahman/sync-period
8fff4a8b030e4ab2d863532d11f6c5e4a196f5e2 Merge pull request #1091 from detiber/updateMachineDeploymentExample
5048d0219087dfbf79c75932ff7ee9624a34131d Add unique label for MachineDeploymentExample
952b082f618fc21465a1ffd2c72fc8a1548d10ff make manager syncperiod configurable
b32cdae21f6848eaef0ec2731671de4d0a51a957 Merge pull request #1087 from vincepri/update-container-build
e5e696c25960757aed0f170f41aef0b09035bb73 Merge pull request #1086 from joonas/name-v1alpha2-imports
8c93b6228d8f9557490f0abad83e740baf6712f9 :sparkles: Add tag to action, update Makefile
44fe1182c6e9ab6794554c3d5214b0bf9a0b18f6 Name v1alpha2 imports
b01c4f7982a34861f0368cfca68488fc703dc07b Merge pull request #1085 from detiber/noEmbeddedObjectMeta
6e5a63852525cc9d6ebe57c884ec66b0dd1532a5 Remove embedded typemeta and objectmeta from AWSMachineTemplate
4cb93096d6650973b216902c0f07eeb02aeb6b8a Update cluster-api dependency
9ba836c040e86be8cb78e06b48ea2b6521503d29 Merge pull request #1082 from vincepri/allow-custom-goproxy
80e2429e7abf26bdd4fbaa938f37d7d1f63e15b6 Merge pull request #1083 from akutz/bugfix/update-toleration-patch
af64893bebfaa007b8bd257fc31557e59d139c8d Update tolerations patch
b2988bea1bab236ec0f394c0f38e7c2df207e9b2 :running: Allow to provide custom GOPROXY
e747dea3534a39718b7ee46fc7a5be8e2bd5f7c9 Merge pull request #1078 from vincepri/image-building
69837ee8b1ba88c1b2b22053f9e43face00cb5ec Merge pull request #1080 from detiber/fixe2e
74311a28f7245273224966c2409525f24ed4356c Fix e2e error
fa02277f59664f6e7ef153ee86a07d4ea29905b9 :sparkles: Add github action to publish images on master merge
052df7d90f6a4a21d56aa4e820ab276622908c00 Merge pull request #1079 from vincepri/remove-unused-consts
dd7ed666583cc9d221c4a3f99e74945b63930593 :running: Remove unused constants
99d7507133fcd4e62b4ed3f1d5b6472362f954df Merge pull request #1076 from vincepri/remove-vendor-bazel
45d8280206f143792b278356d6d76f4f7d4b88e3 Update files, Dockerfile and tooling to remove bazel and vendor
77dad3699896b278b2cec7a6a384a9253d6108f0 Update vendor dependencies
e65fc5ec78eb87ff3550ba7a8a646ee17403e518 Update generated files
f491b3b916a0a779e67731a71f437bdd2a2f3f5f Update Bazel
695129c30c187ffe2d0552aaacf96f3be6de8904 :sparkles: Remove vendor
09c3c213c1988b9a6d1c98c9da09ec5375184a9f Merge pull request #1075 from vincepri/reduce-factor
d0f1ca6b4eaa833e4aa4a52fb6111d32773fd80e Refactor wait package to be capped to 10m and simplify
47eff4512368f248fe5bc79f23e3127e394af212 Merge pull request #1070 from vincepri/fixups-examples
ae2a5596fcfcfcce423377c8065eeef39b644677 Fix match labels for CAPA controller manager
0b290baa372fb8d5c34d40ae25cc2bf503c68a3e Fixup examples
12ab064cd2d108ee81e69808dfd23103fbd5dbe6 Merge pull request #1073 from ncdc/concurrency
1cd5c05eaf35775496a5e2647ba071e9f762fbd2 Merge pull request #1067 from detiber/fixEvents
f3aa5286536a1e4563f0d7ce0fdb0767d23efd67 Add concurrency support
99626b22aaa70d25a5d62cf7d27a0d1ef053a13e Merge pull request #1072 from detiber/removeImageBuilding
9c332ed086e5b91b8f2ecf22972d74cc461f325d Merge pull request #1071 from detiber/updateImages
dc240e0b4b707428194f2394276eec7f943923a7 Remove image builder
be52a17a604a3c6dec13d8476fd7ad86ffbe5c5f Update AMI information and default k8s version
368ce8faf520266d001b3ba22edc95a6b9bbe935 Remove unused Makefile target
4330efe2a5985fc8e9539609d14f7ebc96ebea7b Cleanup events
a9eaeadddc5b402332babc4f6aaee974cc57db19 Merge pull request #1065 from vincepri/cleanup-makefile
9e2940f080d9a9b5b250f2df892090ebaf2ef2cd Merge pull request #1064 from detiber/sgOutput
f040c62a76583f274c82480a835dcef19f349496 :running: Cleanup Makefile targets
c2d36e0f069d22db15d99a0b1271438622cc688a Clean up some of the security group events and logs
469e8c9199efd5da48e4576964deb3a89418b627 Merge pull request #1020 from xrmzju/fix-patch
888f27105bb5af389c199c40275a66e34643eb56 make vendor
0a619fe4a6838b7ffbd59a282084ca70a7e40999 use patch helper to do the scope close
f33d16620161378356168ae8efea4773985661f3 Merge pull request #1060 from vincepri/examples-md
f07db98f825cd6d6ec33332f5543eaf51f52adcd :sparkles: Add MachineDeployment example
3e143356a394c0b32e36cd61f88b4b2e604be89f Merge pull request #1061 from vincepri/examples-tolerations
aff0474fd34d0bc53815643a5909f7105afbba18 :sparkles: Make example controlplane HA, add toleration to managers
392f823e09422548008e8022eb8a7de7b65dee08 Merge pull request #1058 from detiber/fixes
e55007b112b41b8ef60a035a7f6daea1b89bff78 Fix reconciliation issue when not specifying an ssh key
b3c5dd3edba904638c17f166022e884e74f1f268 Merge pull request #1047 from vincepri/add-examples
26378f36d519017d6f0c420b34a10f6401b42d28 Add automation examples for v1alpha2 clusters
23eb2503a2e56a197cca96fdaf0dd28cd176ba31 Update vendor dependencies
6fa2830e5e7b43b940c6b13bb065509537216ce8 Update Bazel
b3ba9e7a2903f391465e303312e012915e5ebaef Merge pull request #1053 from detiber/fixKustomizeErr
da04c8f0e3818a220fa4876d7cda37ab11485c09 Remove empty patches key in config/crd/kustomization.yaml
87331ba1900892bb04be5ef58ba993ee78ae8be6 Merge pull request #1048 from detiber/norequeue
b843f0aa8058f68aa6eab6fd4a6132331bc79fe6 Remove unnecessary requeues
43b0e22dcade545908d86457383e116c8f8cab11 Merge pull request #1042 from newrelic-forks/rudoi/rbac
3535e04b201bdc8f874fa94e16eac47302c13338 Merge pull request #1046 from newrelic-forks/capi-categories
c39a8a0aa41e02d6e36d9b62ede5675b3ad617c6 fix: add capi to scheme, small yaml fixes
fad04d5c467ae2185879d7860af6adc6e7b321c3 add capi categories
563e1d23b3d26e7c7b9ae0f935cd877bf3e77b22 Merge pull request #1045 from ncdc/delete-kubeadm-logic
6eb08ec12fb5efedcb39e9d2dc1e9f5cc9873db0 Merge pull request #1036 from vincepri/pr-template-update
a1666ff10b8a0d7a13561d6b19d8c00492f1e4a7 Remove as much kubeadm code/logic as possible
8492f942687c106d9329d89e0da381f00b0ab941 Merge pull request #1043 from joonas/verify-bazel-improvements
bf4d91073045e99d545b4e82336cfe52fdc5287f Do not exit immediately if gazelle fix finds something; address shellcheck nit
f1ae6d0021e95b6b2fab56da7210b1f3035e2fd8 Merge pull request #1040 from joonas/add-missing-partition-arg
1bd78bab3d6daa06e5587bfe0c616a11498be5e0 Add missing partition argument to ReconcileBootstrapStack call
6cd8696faa35c6bdd8918ec80d3adf40e629a318 Merge pull request #1033 from aaroniscode/service-loadbalancer-tags
944ef4a346f46413f2a1f1422da2bac4fdfce7aa Merge pull request #1039 from joonas/update-manager-image-refs
a24932c87dcfa7a526483e2795473ad356641d40 Update manager image references
80569055adc374759a67c4003be1a744baccbb20 Merge pull request #1029 from aaroniscode/aws-partition
9b9f4df2dfe08deaa7122da1fcc358a651b8a146 Merge pull request #1038 from joonas/update-cluster-api-reference
35607013367af26d638a93574e7167585a31aaef Update import paths to match latest cluster-api
b22e1b65492d4b7be3eae9d1b4160cadb2d4ef04 Update cluster-api version to latest master
38e69b81470cda48f72482e27bc58f5570a319c9 Merge pull request #1030 from vincepri/update-go
506fa1021464fef2d45d122011ae0f5355034af7 Update PR template to match CAPI
823c7f5c9aba2d50c6eb4cf0414f6b3be275dd93 Merge pull request #1028 from chuckha/port-controllers
f2e8f6d2882ea700d674fcd920f39f9e5b69d870 Standarize infrav1 import
3ee4c63877d830ce9318c31a897cb127387f4107 Port AWSMachineReconciler to kubebuilder v2
caabb0c89ff3f37ac6c74fa4b3d54c9f793bb45f Port AWSClusterReconciler to kubebuilder v2
e66ab0471d8119bec71b644d882853e168f214bf Merge pull request #1034 from newrelic-forks/rudoi/status-ready
f1beef01aca2c22b637cdef82e38dbfb1796cde4 chore: set status.ready when machine is running
77907812c7d29c8bc766ef80c15cf8eebeab27ea add tags for service of type LoadBalancer to create ELB
817190b919336e11d5afac81e41004c8ba6f500f Update Go 1.12.9
a5f620cddf00521bfece7984f8deb342586cd5aa --partition flag for clusterawsadm
1dc953b74055090c4104da402e9d3e54bb41a5ab Merge pull request #1025 from joonas/clean-up-error-message
401721df2a9dd0b0a0cf9122548582e58796e474 Do not include input object in the error message
a86ee59d81c4b1d1b3ee7114fc42231816fd9d7f Merge pull request #994 from chuckha/kubebuilderv2
1bcb9245f869742fd48a4cac70f2d5fec32e548e Fixes rbac directory and manager_image_patch
420ea0012d6cec1e1f810b54357d2c0a421837c1 capi kubebuilder v2 update
bb84ee9392ff53a2aa8979a4eef05c409ae4ea45 update vendor
2182a8a9b8ddd28a858873eeeaedae2c600fb3bf Fix imports
4380448b8e23d19be5950390e292d7da1f51abc8 Move types, controller, and manager to kubebuilder v2
d73e3c924eb5780993cc33f155e54b5565460df1 Update config/ directory
f6bbee4c575954b9dca28ca164a6595535884d05 Merge pull request #1009 from vincepri/update-deps
03e827a2a26c0c6f97c195d4fbe3224f26e245d1 Remove unused package
763434fefef7b0d35508bac5b4ae579b0a1857f2 Fixup breaking changes
c69aa524035dca2447fa1fa3b2a57ac7ba357bd5 Remove GVK hack
dc5edd6b604a5a611c81fc942e5efb36c9c269d3 Update vendor dependencies
4857549265b4599df692f0a3620929dbc52504fc Update generated files
85b7b4a43af4bdaa99f94ffe19f39faa33c43bc0 Update Bazel
df9bf5158114c74394e1a1ce47bf49547238ea80 Merge pull request #996 from newrelic-forks/rudoi/decode-bootstrap
7841d0a2b39485729b12b45e733684db605a1aa4 Merge pull request #1001 from johnharris85/change-healthcheck-ssl
0a05127734a4fb955742b27c6e326a65821851ce Merge pull request #997 from newrelic-forks/rudoi/clusterscope
f301e053058a035a91efe8835531c27d001148bd Merge pull request #995 from newrelic-forks/rudoi/fixes
c2d1aaccf79ca9e50d1b8ea0c18a939759a710c6 Merge pull request #999 from johnharris85/set-make-shell-bash
d4b54a59d2723aeb79f626110eb0af642aa9c896 Set Makefile default shell to bash
36b8d4565489544162d3062d7b757f05dfb2b1d7 Change APIServer healthcheck to SSL protocol
202a9f8a438bef7fc379036175e99a25ca0aabbf test: update test data
d7fd735377d6e0cac028544c5610ff79d4ef8e53 chore: add nil check
447343e08f4fdfa0b8645858e640509120bd04e4 fix: pass cluster into machinescope return
356c61e2530d3b7914efd42337e155411f91bedb fix: base64 decode bootstrap data
51e8de63a9592e6ddc4ea82a8d067bef3c3879a5 fix: add gvk patch workaround for clusters
1ee153eed0fcb84b41585dbfd56ae852fdddd459 fix: update rbac and status endpoint
6de25b31def9b4203a3c0a92b868a1819ea6e3e7 Merge pull request #985 from aaroniscode/doc-update
aa3dc4dabf10b47377620d4f7dcbc2abfe986769 update dev docs with move to gomod
959a9208e099a2a3d74e98f56bb997c718608a06 Merge pull request #975 from chuckha/916-to-v1a2
55d1138d8f508a89640cc3dbf0561e68d6f384a0 Merge pull request #963 from randomvariable/packer-ebs-public-option
a9d676610b36a9e863fb7b38967084702a30a75e Merge pull request #979 from aaroniscode/fix-978
61b5feb31a94c60de352117a491f8adb62dad4b9 fix for AMI build to detect Amazon Linux
187e34ee606b7c347f7e4c57e2663e00b5afdf38 Merge pull request #971 from chuckha/remove-v1alpha1
2348b76d1bfe30d04bd32273f6d2bf68002e1f4f Merge pull request #974 from chuckha/839-for-v1a2
7fdb5020c2c6e07b5a8c60c99e347f2dcd9a2086 Port #916 to v1alpha2
f8a3a3ab544c8ec6bfdaefe07cacd24cd7d32da2 Port #839 forward
2bd08d2eff6b41acdb195b9ae65e2f6775cf0fef Merge pull request #961 from ncdc/port-910
227b2404d7cf6a7d84dc0b45de0162bc56d05d0b Merge pull request #973 from ncdc/port-955
8b6d148ed1259bfcaef08225f86e3902ea507f10 Query vpc before attempting to delete
3db7078ec88945b0db07802dc2931975d4a88f1b code review
a50fd8052fa21df4bd98f29472f11f7579b91541 Remove generation from v1alpha1 types
773690f16e3a783871cc1008c043f1352f9dd10e packer: Add image permission and encryption options
d158b9c215dae7a43eb3291db512f792b7c16ffc Port 0.3 event generation code to master
78c2a633937eef502bc735ba563071276384d2fa Merge pull request #957 from detiber/updateE2EMaster
a230b5f0175b9e66b7d9bafa7e5da8604170016f Update E2E/kind testing framework
1148ea317d71ec1eb8a7910127219ce2a65526c1 bugfix: add describe-vpc-attribute to permissions (#951)
be139797dd3afaadc1d962b49ed831ca31558a35 Fix error with `make clean-bazel-mocks` when bazel-bin/pkg does not exist (#945)
e3b2ce11a8befdafc9e2067d89684686b9d576db Add AWSCluster (#942)
93afeea4d9ba39ab1bab9d3149bdb30cb687b138 Add deletion logic for AWSMachines (#935)
d33fa0ec0238b55b749d65f1dd620044655d2f45 Clean bazel mocks before generating them (#934)
99bf138a98c96fafd266ab096f209f1fd1bca7df Update releasing documentation for image-promoter (#932)
3cfea6e29a174b4123ed4321cf13b0ab3238df2a Update CAPI dependency, remove clusterctl and make examples top level (#923)
c66768e0bfacf1d00b2a175428ebe1eeb7b23a5f Switch apiGroup to cluster.x-k8s.io (#919)
25376aa086f183a13f1d50cbb23dd250c03d3137 Update CAPI and controller-tools dependencies (#915)
4ad964545b8838e240a94dbceda29dd855eb1245 Improve AWSMachine reconciliation logic (#909)
be8cbe7b339941771af2abe2d2d218445b357f35 Add AMIs for Kubernetes v1.15.1 (#911)
8b0128f8e926dbc27bcbe1b6e1b7d5237c178041 feature: support set metric address (#907)
9df39814a0ad6d37c829c137bb9ba9ec2f8beaa5 Restructure repository / cleanup (#905)
33ff3a05505242b564596de67d5a3e7f227cf97a Convert Status.Ready to plain bool (#904)
8347a46699d0871641d568bf3afdf261c83fb43d Supplemental update for v1alpha2 (#896)
85213648fb1585c9151b8f7a71a41419e88e4362 Document custom ssh key (#902)
0eab27c657498725c6153d723adc87d4e67e62ca Add optional pprof http server (#900)
d409c5809c780bd5baaf6b52990edea548622eee Update Kubernetes Versions (#897)
3268ab4a6ac862465581baadf020d6b11143078b CAPA v1alpha2 :tada: (#892)
718a38a55cf6301d5d99a2a80d40c675d47b9fdf Update Releasing docs (#895)
1032602d9380e2a1471cfc5d3cc4d633a266aa9a Don't rely on status for deleting security group ingress rules (#893)
82023f16e9b1254bde2a1b46e66e4e203f42a382 Go modules (#888)
f7144edd1aada8cca8c115ccf53009f6197b085f Fix ELB panic on deletion (#875)
d8eeecc50f70082047d011b83872f5bf424db22a Add additionalUserDataFiles to ClusterSpec (#879)
445861a9f6cdca10740f6da47a3c87df723d2442 Avoid infinite APIEndpoints (#881)
df5163df955cfb9cda8380a096db703fb97cb9bf Cleanup services/userdata package (#877)
b1e47060691af596d2d35442631906a1a5da7b5b Fix controlplane machine race (#779)
39cfa38d703c5fb1340fc1e6e979d500c7140734 Match ncdc owner alias membership with k/org (#855)
60a717deab450aa479be6d102e9423068a215a2e Rev minimum version of Bazel to match requirements (#872)
1e7225b91241a5a5a4be4e431999fbec5b76ad6c Prefix templated objects with cluster names (#868)
5f035ffcfd73bfbe46ef8e08e582fdc5f63d8e42 fix: respect cri socket if set (#863)
a180acceaa288a6fadbc21f67a4b60cd9a19828e doc: Add godoc for GetCoreSecurityGroups (#867)
86012e5d24130a0932dedf18290c54ebcf89c5a2 Add watch and list to secret rbac (#862)
311c67be294e783a14ab637018b29ffe0d1063a5 Update for Kubernetes v1.15 (#860)
f8e0517874fbcb9109ef8dd225ea81ce3fc61c1a Update to cluster-api v0.1.4 (#858)
176ae819ea09bc404341825dda7ac28ab85b16cc More bazel fixes (#854)
99bac1756771d9376fb431e588eea6bb1bcc5416 Log userdata size (#853)
1f67c7645a8c202e676ef8e0fb15aa2660e30a40 Add support for NodeRef controller (#830)
ace9cb7b1ab5b3d5ced5663e44656ac94ad78b2c Bazel fixes (#844)
ef1c8691a0dac7d644424e410322081a777fb033 Minor fixes (#843)
8e12155d0eb12deddb5e1b45558d92637c942dca Fix cross compilation issue with bazel 0.26+ (#841)
e3324c9c65ecc0151214dde4e56a55206ceb2fe4 Add logic to handle implicit route table associations to main route table (#835)
46d5f38316f5be97f90cfc882d15794a725c6534 Improve dependency graph (#833)
ab94d4b0968ffb4fd13351411cf0a4ec4e90a8fa Switch Kustomize to use bases and not resources. (#742)
00a5173c7ca53ea8f8a05a87a3c3e87b19db2f81 Add AWS_SESSION_TOKEN to the documentation (#834)
8feaa2b880d3252af8cbfe79e369d1d5e480c10e updated link to kubernetes bot commands (#832)
e6dffac908c230e963fe2e06240739f2d27bd630 Remove unused parameter (#831)
6d1684f646dbd83d56ac6daf2fd359726caa365b Ignore deleted control plane machines (#829)
2ca6185e7dabcddca22f7858a677eb64d97ace44 Update some bazel dependencies (#827)
098201ec8d6fe9c3e658ef9ee8dc09cc9f55819f Allow Nodes to talk to Kubelet API Port (#826)
f9051c978d278dd575f39dce071fe6234431b44a OWNERS_ALIASES: Remove randomvariable (#824)
b1d5924d1edb88015ea1d09ab7b0a479cff9cc4b fix: use provided NodeRegistrationOptions as base (#823)
77da568c59f4355188103987a6d8d3519847d8dd Bugfix: add ModifyVpcAttribute and DescribeVolumes  permissions (#820)
e2abf2fcf8062dd290b9f1d72441f82d04dff9c8 Add create-cluster-management to Makefile (#819)
6438073724e6d9288a59997e6be20bd058bb95c7 Update CAPI to latest release-0.1 (#818)
c11fdd37d5c9e170105c2530222d3ee466d8a69e Promote sethp-nr and rudoi to reviewers (#800)
6b455f697449d6e00eab9a02b57d3d80c8284182 Update cluster-api for v0.1.2 (#814)
910edc05c65f691276d61960e7e72b27616f75ad Update for k8s v1.13.7 (#812)
450cff8d46fa0b1cac4cee73469dc5e405bf5869 Update cluster-api dependency (#813)
75f4e3e12e40f23003140e367a993e7a1ef51db7 Add availaibilityZone to Machine Spec (#811)
4f21f2f891dd15c6f04e3588a13c15392dbb68dc Update for k8s v1.14.3 (#810)
71f72fa058ca5bfdc457dd519070ee5c7834a893 Update version compat docs for v0.3 (#807)
7a87a3058e742d8a324999113a125bba792602a3 Remove go get install instructions for binaries (#806)
c85586c59121d5a9ac89c589c919a73722b5af3f Build and update images for k8s v1.14.2 (#805)
b744f876647b02fd74b52d98c05615ab911925a0 minor documentation improvements to cluster-api-provider-aws (#804)
d12043bc5b948fd53732bb46bd9b7a8253d05ef8 Fix errant formatting (#802)
359991ec850866bc1f3451c9a942af484aa61701 Functional options for kubeadm types (#797)
b59af64ce04cb8174fac0347d0d973dcff49e4ce add gpg key dependency to docs (#798)
fc33354c7a8125367755c77725c2b74386157301 Remove retries (#796)
fcec2e0165ce077e9ac492cbea7b3bba60fe614a Copy taints to new machines (#794)
342d6bb0183ba59637d03e753b94ac008f346311 chore: append nodeRole label if additional labels provided (#790)
0ca4e7db7294a4d4608ca82555e903364eb663b6 Show where to get the cluster-api-provider-aws-exmaples.tar (#788)
b0d188ce11fb0cbd91a28e3bfb93c8f2fb8029a4 Delete broken symlinks committed by `dep` (#786)
eb236d81e6c8d9679d3766de5fbeab2dbeb79980 Split the VPC options into two aws calls (#785)
55f8f8d6d6dc41989a61f90d6af42afed28b85a1 Add unit test for security group reconciliation logic (#782)
28d328af4f4736e769082c2de6d7e5bfe55095f3 Set attributes for managed VPCs (#781)
112255a206ed65ee0aa0f15aacd753db7bdf1528 Add more troubleshooting tips (#775)
d747df6b8a34f96616756c4b941d79e84f0e4a79 Fix security group reconcile (#774)
c0a2c0f57ff2e2be1c751b7e322fed1224efb10e Update to latest cluster-api release-0.1 commit (#771)
77f6168f039bf89d7e8ff21c146e03df5035ed51 Update release tooling (#762)
5b16e56111bcfc47fdfa5e59d751a4f3a335caf3 Set cluster status api endpoints. (# 764) (#768)
2c093fd6c1409a66457354acf9c8345d4b35bf9a refactor: separate CAPA resources from cluster (#706)
74c4c9dddfae2650d3901bba5f53da3bcd1d15a6 Update dep to 0.5.2 (#770)
1f9a31c0a17d3637a570e43171c9020c9a06379e Update base image to k8s v1.13.6 (#766)
9fa76f35c28cb17d5579eb6f0ac4a857a07af54a Update to Go 1.12.5 (#765)
97c7d7f53fef64673f290937f49f711b79da986e Fix control plane node join logic (#745)
edb269f04df51a7b520a717031baae7b7ce13eef Simple cache for sessions (#757)
7e32f349f6b4bcc92c416af487e8884467edef78 Fix log message (#761)
5420c884c45cd26a012e15be80c6d2e0954ad5ba Fix up //test/e2e:manifests (#760)
9b73152f59df84ca8a851bc2327e70261cf5f777 Add machine-deployment to release artifacts (#755)
4e0112195c85b9622d4192436b6910fb81ca93a3 Reduce the number of re-reconciles (#752)
c4636dad00a17c5f2bf9ad28ab43591b4922397a Update cluster-api release-0.1 vendor (#750)
a0289c53b23bb3048d1d355e953d0b8af016f590 Update Gopkg.lock and cleanup Makefile (#751)
970144de689f92f1b7d42c34da87b218f1f01dc4 Fixes the infinite reconcile loop (#748)
f38fae51c312c3d93a47d85f222b5bf27f2afb08 Update AWS sdk, improve log in machine actuator delete (#747)
3ee1b3dde70b1874a90c796f817773b167dc18ef include machines-ha.yaml.template in release artifacts (#741)
cd4f48a3f682ec3d874dca42db0b58aee0580773 Documentation for creating a new cluster on a different AWS account  (#728)
239d386207ba138de193128b4ebbef0fb05d4a10 Fix NPE on delete bastion host (#746)
7035fb30605fa0b9a7dc0b01187045c9253f303c Scope nodeRef to workload cluster (#744)
bb35b028466172e1c368a5aca9368a0d4fee92d8 fix: Don't try to update root size when it's unset (#726)
740d384491e599b604abc5efb12ef01e935f82a8 e2e testing improvement (#743)
c56fd14510791871e96c2e304bfaa10edc49a762 Use DEFAULT_REGION as the default and REGION as the supplied (#739)
41cfbb2d87173eb1c6807ed5820b9995153cd7aa extract fmt from release tool (#738)
c9f985dad9ef37193e5b2ef4ec589263e56ba5b5 Fix markdown formatting (#736)
6b092ff657cc601116534dceb80847812d395f6d Fix the prow jobs (#735)
74aa2a84a2181bc7c0f90f538b75929cb333750b Update OWNERS_ALIASES and SECURITY_CONTACTS (#712)
2650c01775856c1e00cc5cdd7855b1b7436de450 Ensure bazel is the correct version (#731)
b35c24df4430f1879f3577adec9a41fd421842dc Add the HA machines configuration to bazel (#733)
91f1a310c6864b8353d5edddfcc025946c2092f7 Adds retry-on-conflict during updates (#725)
24a9abd3777e7f8dffdcefb4727e50b7ce856c3c Rename BUILD -> BUILD.bazel for consistency (#724)
1aa10aafd7bb2b908a13bd7cc0af55d5cb3d2ab2 feat: support customizing root device size (#718)
420d8c4337990ce37ed63e2ea75510a00b5684af Add ability to override Organization ID for image lookups (#723)
1ba422e82dc1dd55cdcda9779ed56aadb27d215f Update to Go 1.12 (#719)
182c1018408ba28e5007d706d4e54371722f09c3 Add clusterawsadm as make dependency to manifests make target. (#721)
0dc56e7905165d33f998493eee06eafc9ed8a946 Ensure `make manifests` generates machines file for HA control plane too. (#720)
9ad1cf56a84e851eb35edd93deb04a221a1340d5 Adds logr as dependency (#714)
1c287daa7c447ce104ce9b8f28d8fb3b6cded05c Switch dep to use release-0.1 branch instead of version (#715)
6b2db7616ec886633429ca6505d7e04840673aad Logging (#713)
265f3a5a3709bd748b8ddddf7b45869927430dc4 Adds tests to kubeadm defaults (#709)
c694a556e993c243326d63e38f09ee167dfdd6b8 Make sure Calico can talk IP-in-IP (#701)
a1943c6b1785f569f4e3a93a043a78aa81bbcab2 GZIP user-data (#710)
4898eda6f9ee3016cab61b338e567081fc179664 Update listed v1.14 AMIs to v1.14.1 (#708)
6795fed7f090ece6b16d64db5ce9d6c6bae813c5 Fixes a bug and adds tests for kubeadm defaults (#707)
fb3208a5632c62aea0390cbfa0ada931000b95a4 Fix: all traffic ingress rule triggers fatal nil dereference (#697)
6f304f5e2d2c51e16d608797bba790e0306b4787 Make hack/checkin_account.py executable (#703)
1653605284e83fbce6316b270a416266090678ad Fix checkout_account.py (#702)
2e978b91c42246c58201c30767ea94956c3018ce Update checkout_account.py to not reuse connections (#700)
7759225aaf46aa177372104a25dee7543fb24e98 Temporary workaround a data issue in boskos service (#699)
7899d1fab90c234cdaa3341747ff8a2d9e630fae Add error reason to output if fail to checkout an account from boskos (#698)
d84147d9b75346ab4707acb55519fb3642ecf92f Attach node security group to control plane nodes, so control plane nodes can talk to each other in HA setup. (#694)
eea53382d0f9a044b3d8e05dd19be6f3d3aedc27 Update the releasing docs (#689)
c78ce65cc61fa0c84a6ca28edb9961866a48789a Avoid nil dereference when missing cluster (#691)
e4b898551a60f6c699dd506fcb45b8fd9708a3e2 Update cluster-api to v0.1.0 (#686)
b97e610f56886355af22f8de63fa263c0af1d2cc fix doc (#688)
249884b2e1fc174c42f94a204d653ffdb017e1dc fix: update bootstrap permissions for ENI modifications (#687)
bb4beca83d05effc3d44f72c1ced86929ca7a8a0 fix: apply security groups by ENI rather than instance (#684)
9f13a377c6f4920699a8c8cbcc2bcfbe954658de Add Roles for ControlPlane and Nodes (#681)
bc84827cced55253857eba081f8b418b09e04d21 docs: Fix reference to renamed script (#683)
0450ebe4dfcf601fecdd04fc69b304a1e8c19695 Sync binary and image versions with release tool (#682)
09d44d3630f3d0a0e95f55545b7118c1a64162c7 Update AMIs (#680)
7c67a1ffb3fb3d3353ad80df76ae667821c7d13b test: Mark integration and e2e tests as external (#679)
f0e30278b277f707f525f6535bf9027acf162a03 Specify minimum Go and KIND versions in Getting Started Guide (#677)
02d33fca011814c5b5d079296b2e99a7a83e5e31 e2e: Fix-up for changes to release process (#678)
8f0c8275e77668a49b122de28e68a264b6037bbb Add version compatibility info to README (#676)
3a538eda22bed42c817034b6eb3ac8be15630955 docs: Add note on new binaries for DevX (#675)
32a5c5147684829fcd53a9787ad1474eff937469 docs: Update developer documentation for v0.1.1 (#672)
c69b9abaccb0eb17cc2c44a543b9a0c6426d06a3 Update NodeRef (#670)
3ea54b8505ba98e31635da341221fc99723edbed Update the resync interval to 10m instead of 10h (#671)
32530b5c4ce81c1dbd40f2b7f86449ba81ac5d9f Update releasing.md (#669)
e2c4b3bed5048e8f3d3f0df62ca176ce0e4e359c clean up release tool a tiny bit (#668)
fc14a274367e300b9f5238b396b06ee20fb67831 fix: add AWS ExtraArgs for ControllerManager (#664)
1101aad084486939603e3e24cdcd63939279ac61 Fixup release tool (#667)
993ca9d3394b52ab23d2b542a10895f97c36cf6c Remove more bazel defaults (#665)
19f0cba3b73221e6c307e303d4724a79dd5b9969 remove '-dev' references (#666)
e01bcd1c2275a8f8c429bfe6bdf2696896bb981b A little make & bazel cleaning (#662)
92bda1a36009653a26d46d7433020bb7fe1e7e67 e2e tests, rebase of 606 (#658)
78f45a1d83efe1bcd28eb7cf24acfb74cf19c3f4 more verbose immutable machine state errors (#649)
f04ca3a5d43466c9f0e655e22e5d01bbf2af5779 small e2e fixes (#655)
6ff9411c2828ef7e15d94f29b708b1467a6f1d00 Fix issues with `clusterctl delete` (#654)
670b95cde3a3ce199a647215cd5fa8dcaa9fff79 update ec2interface mocks (#650)
786d725ea8c914479bd6ea9b16d0dff248f1b241 fix: no longer panic when instance id is nil (#644)
83f8bad0bd6430bd186fbbff934ef84cdea8d212 Fix AWS credentials mountpoint with distroless image (#648)
45e89a31dc4cde2cb7a420e5c0710002ef32c8b3 Update Bazel WORKSPACE / use tags where appropriate (#647)
9cdfbbef40f25cf7d3e9ff23504e6736e2f20a76 Restructure Makefile (#645)
a52c4bc63ec5f9805ab540e1d1aee9db4b5ca1bd Development doc improvements (#639)
ca19555adb024cb4bfbac84c0c9485676d4bb6dd Rev cluster-api dependency (#646)
9f7f989f1cad11c8c9cd093e878a6d8f9acfbd46 Fix panic when IAM profile isn't available (#643)
0819fcb468dd5cda8b127f78ec366b0512063e58 Add ec2:DescribeAccountAttributes to bootstrap user (#630)
e8a3530e0572034f139439e0c723688fb5b9a8d3 Update cluster-api dep / pivot phase (#640)
c153cfd82bd74f7c3d688b632bc2c76015aea180 Fix bug where additional security groups and tags are not applied (#635)
1235f41ee2e23a9d602134b008c76707f168e989 Adds initial release automator (#633)
9f5518b905021127a6c7cfb24cb570a38e14cc86 Set the ProviderID if unset (#637)
fe235099c3e055624084bd227b4f7298c3300010 Fix linting issues with asm_shim (#636)
98f8b2c4b591f5449e6fd750ac324fcfd21c3942 fix: repair node joins (#634)
22f23edfce17dc3aedd87b0143080b355a50c339 Release docs update (#632)
42c8f00ac96e2b57c675d82a9940789a30f6fe7e Remove unused fetch_ext_bins.sh script (#631)
a02577c691e2629644344acb6b180e50001175c1 Rev the version of golangci-lint used (#627)
44dedbbd9bbde4f1f5f9d6895ed37a0d6736b893 build: lock golangci-lint to a version instead of commit sha (#625)
13b5457575f9de0062ab723f468e8678079b7cef Update cluster-api dep (#621)
5bf527511ce7155c7d24722d25278b4c2ec9d21b Adds ashish-amarnath as a reviewer (#616)
d994310a5f9f6422b2f641ceeb0e013c7eaec034 README: Update meeting times (#618)
389258fab9f15efc7c1d335d1ea228fd3248abba Document the 'namespace' cli flag to capa controller (#615)
6c70e25e2961b652e1ec7ac2495cd03130a4c92b update multi-node control plane document (#604)
60789ed2e2bd1aa66fd30348eec3bd39d7b66762 Add cli flag to supply namespace for capa controller to watch for capi objects (#607)
64079bfbf8278026a5fa3cc51b295f4fb1e2d248 Update cluster-api to latest master (#609)
e75d478659a2b4522a74a69928957bcf616502e9 Fix tag for cluster-api-aws-controller (#605)
e4adcc04c61b3d60d14e6be1e6d95c7f745a14b8 Fix bazel for aws examples (#602)
f1ce0646bfc18796a82b993e7db5fd3439a7ba18 Update cluster-api dep to latest / ownerRef (#596)
2b7af23e9bb0fbf326875449ccaad32fe71745e5 Separate e2e and integration scripts (#603)
bde2b144b16d60825fe8f1cad134446d03ecee1e Configurable region for e2e (#598)
d11a562d991c81292b9ba586940ed6f7bce090a4 enable deadcode linter, cleanup (#600)
325cfd6272dc01638982d666b4d2f2b26e9359b1 Remove dead code (#599)
7241c0faf147deee506e0606c0790f3be2153913 Updates release document (#597)
ffc57fbcbbd0198f6950d00572f82345363afa77 Adds documentation on releasing (#595)
605138e52b7b138da08f254565869d7ec2b874c4 Fix manifest-dev workflow with Bazel updates (#594)
ac12d29524befdc0b7fde18f874c61ff7fb24972 Revert "fixes bug in generated manifests (#589)" (#591)
1f4d4572099f9d471aa63e8c6184e901049ad859 fixes bug in generated manifests (#589)
2e996f184b2868dc90c5723b1faa30de440873eb bazel: Fixup to dev manifests (#587)
5dbb7de429177091288aa9ab6f65850f6dc41978 bazel: Expand make variables in stateful_set_patch (#586)
14a72d66751e5a643d5b1cca6e68f92b1a7c920a Fix typo (#585)
e6bb385084bc4bc067819391d2179b55d8b96e17 Release artifacts MVP (#580)
9f0fd8afcaf600dbff51a0057d6feae320575f77 More reliable public subnet detection (#560)
870d03d2d5a25a407b335d3f0b702227dfd7cd59 Kubeadm types (#575)
c10d30aa2ad0f92664f1b8786b24ccfafc4bce37 Fix return in isNodeJoin (#584)
64aa635f1610f9a9b3e951785a09d3037a307b6e Followup to #579 comments (#583)
94a3a3abc7b1ebdd88ea89889347f5e644e160cf Set NodeRef to Machines (#579)
39266b8d492046eeefb4d44abec13eb59ab03c19 Update default AMI list (#582)
de3d0fad47497aa42e6d92ad8877004fcf086338 Fix repeated error messages for clusterawsadm (#568)
699b324eff3cacfc309698742b5d0ba3d432c272 Rev versions of containerd and Kubernetes (#576)
e456e75213c7e3d231f9bb1e4f2fc580da7c59ec Real e2e (#573)
d11e7ea39ef09be37afd6b887167044e4260ce44 Use InstanceState instead of String in Machine Status (#577)
878bae8e17c8cfd38400511f3a542eafc4d50eae Document manual steps to creating a cluster with an HA controlplane (#545)
e1ea167e3a1ef3f3551a11ac8d96490af0e26b97 Add support for MachineClass (#571)
d0c4c973b010d7c084d6000a0beb451906060f54 Update cluster-api dep (#572)
294ec3ec8fd6cae1e5b9e4ed0a75c148b8919130 Update cluster-api, add cluster-name label to machines (#567)
d148b486fa4e7fd6203abcdfc46b76862f6e0ab5 Rev manager image tag (#566)
a909e8d5ad2522c5829b11e7950a33a5d8a57841 Set pathLenConstraint X509 constraint on CA certificates (#565)
27e2e7fec56549f0dd0ff41b12d113ed94b2bad1 Sorts AMIs when they are returned (#563)
4d4a16fad0009e1df861a195e2f0e881dfb2fb1d Update cluster-api (#561)
6bbcc790553475e62c59384fef732477187f5a43 Python scripts for checking in/out Boskos AWS accounts (#564)
d9e98201a79c202b63a49b1d7465bfc9dcaa2f64 Switch bash to cloud config (#510)
aacc639d8cc3f662f0e0b4e05af0ced213fed69d Update AMIs to latest builds (#556)
0b8b993e86269f2b87c55a2a8c63362aa4fe61e0 Make sure ubuntu gets proper version of cloud-init (#538)
b97293e0de18768db9b0e6f702ab26b0cf6b7c3c Bazel CRD and RBAC role generation (#543)
a3f1aeaa6e782ddc2dc515bb9c259cd096a27a8b Add gitbook link to dev docs (#555)
63e7427256d75a5812aee61853de03473dbfb86a Fix CloudFormation stack updates (#553)
65be5b49949184cad6983d41180fcb9a22fddf6a Improve user experience when generating manifests (#552)
17a835d09405923388309c29d59564a69bbc76fe Refactor cert generation into a service (#544)
c46b0c4de65b97f0043821524f876715d9a65f0c Introduce NetworkSpec to support existing infrastructure (#483)
20af206e76b72d6bbffddc6ef295011fc9e8fe34 Update bootstrapper policy for loadbalancer attributes (#547)
279b7669967f76d370f49cd81da0bf2544111a1b Reconfigure cloud-init to use ec2-user instead of centos on Amazon Linux (#541)
ead6fe0cd67f116572643f42c31edcd35933a78e Add new line while printing error (#542)
8818da08964e48f0fddd16d12265ec3b86d1e7cb Allow cluster operators to use custom cert material (#502)
a1cdde773114882ea9237223326b560b2b17d442 Updates base AMIs to v1.13.2 (#534)
c9355db4ff05a6a7c28906c294215720b2fcd8da Machine Actuator: Implement immutable state checking for Update method (#512)
438e1702ca4f2d442ab897d09e05f0238add4077 Use default credentials chain instead of environment variables (#518)
aecfb4ff12096251d4562d208d89aad67712603f Fix control plane url in token creation (#532)
73646520dbf0e0dab40a8d607268e64e348d1cb4 Bump go version to 1.11.5 (#531)
7a9f9f40a5cb8d99fec2f7a158f232e7143b5275 vendor: Update Cluster API to 9d16c16ede4ed343ba8d2335243d2cbf1fc1d87d (#530)
324eeb053468fce8e634214ee10f2d4f4c2a4a9f Fix klog init in manager (#527)
55b26b6423e7edaf62d866c5fa3e041c276ba841 Update capi version (#526)
e78b40465f19279580bcfaa06d6d228434e64ca9 Bazel: Removed unused repository (#524)
44a85be255eeea95662feb76d3d190c640f826b5 Updates getting-started documentation (#523)
7917575b0991e0261af2ee198461890ae57d7005 Bazel: Update dependencies for Bazel (#521)
03b32d9317467108d8c0f2d04cb830a0f1200545 cluster-api-dev-helper: Delete dev helper (#522)
0e543e0eb30a7065c967f5df8d6abd872aa4ff0c Update developer docs (#520)
7cadc4d6fc81cfd6b73b140758ae2aefe2f8038d Add IdleTimeout to ELB (#516)
5496b43a012c9b06ae7ad2c38493b506e0ffea58 Add documentation on how to access cluster nodes (#517)
6b1875be6c162e1969bc5ba10d629b742ac70ef1 Add permissions for ELB to create service linked roles (#489)
8fe6eb1bb2d3534a6753b762bf23e2d0eb7f0fab Return if scope/machinescope if store config errors (#515)
d43bd72f8252c4780ddbdb19686cb3fa3e988887 Small getting started fixup (#514)
c6d50ef91a6c9fc00c558041ad1c29657badac7e Update cluster-api to latest master (#509)
34a1106372d105da0aecf45c22e16bb4e9c0ba95 Makefile: Ensure out directory exists for release-binaries target (#507)
7ef2a13c025c39eacde08508741e648c5b8bcfe9 Update documentation to use KIND (#505)
0daee6fa326aa754db03fbf17a1390c1efc372e2 Update autogenerated files (#504)
e73d829a5f1c733b84ef7e3e8186f582b1871fd1 Replace glob with more strict directory matching. (#506)
2ca3a9b0834a0b7bb13e3f14f313c32ba6c08c96 update cluster-api dependency (#503)
de77b4572466eac339fe474c111d0958f8eff4ac Update aws-sdk-go dependency (#501)
45482f9edfd356e41371da3afe9aaf089dc9dda7 cloudformation: Add ec2:DescribeImages to controller policies. (#500)
5816c1814af68a3438bd5f1f1dc8db7177d41c31 Add equality for ingressrule (#499)
b8ef509599060cd594d0ae7c6123507c4c193cc9 Control plane node join (#463)
7f16b006de6bcf0f8c47dcfd62e5571871c83e95 minor cli message (#493)
9f2f4b6be15f962267d4400d5bff233c2161d277 Include owner as an AMI filter (#488)
32e87fea3314df84f1cd6e75a040a2d08b541f48 Lookup AMIs instead of hardcoding them. (#479)
ca8712c3fb9595850662a511582132cee81f2464 Ensure tags on subnets (#480)
1e4f1d91135e91c6df9e1716b3b2e6947c8c29c4 Ensure tags on routing tables (#482)
74a268e8d485c9a5d34cf9e95c178096b430c95b Ensure tags on VPC (#477)
f800315148eff0c9c5db8885c7c1b40d3422ed6e Fixes examples(-dev) makefile targets (#478)
2f4306206341fd0c42c49f871a8f46d6dae376ff Ensure tags on security groups (#475)
4465ae5f60318f7f87f46db9331258b148dddd7c Ensure tags on internet gateway (#474)
b9669ebf60df9313f7d4d1a4dcae4b3660611b12 Installs binaries to gopath even if gopath is unset (#473)
430e9872ab7c8fa132792ebe3cdd96fad7a42e3f Bump cluster-api version (#468)
8a3b421d7ce97d73ae13826ea63249e2df41eba5 Ensure tags on natgateways (#465)
0248b7522541f94a2637dff443371d9b81b41da3 Update services/elb to use tags/converters pkgs (#464)
8aded3946ab2aab9d57ac4a3438eb05690456c0c Wait for cloud-init to complete (#462)
eca27451d0478d4563e1c6803759e036aff5f46d Containerd 1.2.1 (#461)
42c08ebe2953653711b71dc4ff302131178e178f Update Bazel to Go 1.11.4 (#460)
23bb329ad01496775daf5eb04d0013844dca0374 Bump cluster-api dependency (#459)
3152b0f9f3c15d330008a4239a9a09a1ff46935f fix kubeconfig to use correct cluster name (#457)
55671b3a1f3cf6429f735e84c116775af9b79cd4 Enable stack trace error printing in actuators (#456)
41f84093cfa905ce258b669d8a99acb2e3426d97 Fix cluster/machine status updates (#452)
f370db891e1f611c36b37262b8e252149b8e0398 Rev manager image (#453)
a7557b5ffb9a667d9e7ecd979f21db09d4900393 Add ability to configure cluster name, remove generateName (#450)
5f514290e206dcef503beb9556c7f6295f09dd60 Fix manager container imagePullPolicy substitution (#449)
8cadc31e8d0ac0331de7c43ed3cca24843409786 Simplify bazel verify script (#447)
3b6715eded896b17b98b435bca00f568e11aad1e Fixes bazel 0.20 deprecated git_repository native rule (#448)
4bc7a9bd8cb07e98cdbbf04be3652dcfa909a395 Add a single, simple ginkgo test: Make sure our set comes up (#440)
da39a220ecaa02fee8c24f6923c6b576e39a1852 Add verify_boilerplate step to check for copyright header (#442)
5359842b917f998c567553c4d3b0e9a56f29effb Fix node join post-1.13 (#446)
5abecc3aeb6a90ab5004ebc304a2747f67a6134b v1.13 update (#439)
25bc6b283cfba665f20560039d90bdeb5a1fae78 Adds clusterctl documentation (#436)
14e6eadd6002c24e2cce029da2abb1c3b99b8464 Fix status update error on first run (#443)
927f5b76d62f4b0aa09a1e9f75db75ad964a0486 Implement 'version` sub-command (#433)
690b220e2fd6b44934987f9f7c59e1b26f8dd980 Add kind targets to Makefile (#437)
b9dd5967f661e461380542fdfb6db1bce4ec8d1f Update clusterapi dependency / fixup logs (#435)
587119942eb737e728be38be2d252849c7f5c468 Record basic events (#425)
0fe17bc908f15a13ea1aec840fff258acf4915c8 Remove manager binary and add to gitignore (#434)
1bbda384f91e3fda37cdac111d67ddd7e488a63f Exclude .git/bazel-* directory in verify bazel (#432)
8fee055d467f54678669e484141a9715c935189d Update Makefile for easier DX (#429)
2bf78fd5b61e41b65e824ac329e487cf46538884 Add verify-bazel script for CI (#428)
75b07276ca5a1b0cf97ea80a8f2bb1f6a58c7723 Fix possible race condition between machine and cluster actuator (#424)
d0297ffae4530dbfdd7dad5b29390f5b7773860d Fix security group duplicate rule bug (#423)
dcd74bc15077c91e43ab74966afdeafc2fb24727 Fixup logs (#421)
f8d26331254952fb067c7d779dc2f4df8013e17c Update committed mocks (#420)
796a86a3a00d9475fba018831ee1132196292e9f Update dependencies as of 2018/11/28 (#419)
7f3f0114341287a65197400dbd9311c0e3d5ecda Fix deployer initialization, update config files (#418)
2ce47bab2861e49b93521e2c3911cbc5fe92b1f1 Refactor instances around Scope/MachineScope (#411)
a9a9a7b83f11153759a7e567f5856c6df8c75985 Refactor elb package around Scope (#410)
01f252ae73a8eee38c544e54caa5fe2b1494b2dd Refactor VPC around Scope (#408)
68434b386b80187fe4a7d2631747c54a9fa6dc39 Refactor subnets around Scope (#407)
98f1b7865c40941442bfa16967dcf3533a1d471a Refactor NAT & Internet gateways around Scope (#406)
9f53e0e2412a37757347a5c15deebde4076f7697 Refactor routing tables around Scope (#405)
9ec16a0783452d477856e53de6c029f2cb97bc1c Refactor security groups around Scope (#403)
053d5d85bee74903bbe2c394e8a3270446a2cffb Refactor elastic ips around scope (#402)
2e3970a0d70eb967f4a0a143f15af8c6846ac270 Enable dep pruning (#401)
7f1f593272c700a31b5ce212b9a4b039ac6b1943 Add actuator interface tests (#400)
928469f37d7203f048ac6e5d481a3d7d45b3b4e3 Refactor bastion methods around scope and remove region from status (#399)
c3144d7b2e5143e1bcaa8cdb960d23ed7daa31b3 Refactor services around actuator scope (#398)
129f8fa1d4020bdcbbefe3086cad5b4b5d969c2b Fix ec2 subnet filter typo (#394)
f8797e99812307434b4a9363529d042f90eb45da Update getting started guide (#341)
545c32a4856ebd104865d14e53e8a079386a3788 Move filters into a package (#393)
64df039a0dffcd625a12fa0fbe7aee3bb2dd8630 Refactor actuators around a scoped struct (phase 1) (#381)
aba41e37bea88fced02825e5d69641dae544003b Add tags package (#391)
3ef866c6f7883f18c0c510a93f221dd960d1b063 Copy mocks on generate step (#389)
8cc4594527b109ed4a3304380154c5bcda4c5608 Add converters package, use awserrors pkg for all errors (#386)
a7e97cc3445245a9ebed477d7bf761be85704fef Fixed typo in cluster provider config (#387)
aac64a54ee67a3227adbdd6e26709a7b1d192aca Remove unused controller (#385)
f5899b4242b24df42a210bf45f86b469abab4bb4 Do not bail early in Machine create (#384)
eb746798f826d4976f6bdbc0d679a5c6c3f3fbeb Minor cleanup (#382)
18f571436fa7f0bdc650aee57abbcc63c883e4b0 Remove actuator mocks (#380)
9d38f64c9ed98cf96c3fc41e69dfe1d9217d2cab Move deployer tests, remove cluster actuator tests (#378)
8f47fb018f73d31e75f010fcfcb9b06c85c02972 Add build tag to e2e kind tests (#373)
d2c0a235304b43caf72aa8b42382cac8d0f6b6a1 Use klog instead of zap logger in manager (#377)
939579b3b81c41398bd9501b4ad802223c86def2 Move getters to services package (#374)
2901ae5465a3f78cb97306da2edc91cd8161f4e7 Convert to klog (#375)
64c079160a4b4c3620f8d60281d2b5a4a2e908b5 Update machines.yaml.template with TypeMeta (#370)
0f625bc4dcb6042f51e640bf59655b78026e86e4 fix 'cmd/clusterctl/examples/aws/out/' make target (#369)
1d5a033234f40baf7d8488531d0b1ae5cdb4e1ef Prefer ec2 metdata hostname (#368)
6b9de749332049a32a919a30b5bdf545ffa0ec39 Fix kubelet argumnets (#366)
d0b407a91a017c0ded1460a97e4a8f8f2c9c4b23 [DOCS] More info on minikube and aws user in the getting started doc (#364)
845b86f01b6406c8d8af46c8f96580b42932912a Add generate-iam-policy-docs command (#360)
4acdad27e2a56125ae7b182a5282787b9b576b65 Bump Go to 1.11.2 (#363)
6e9b78885d78fd98bbc83dd9fee62f49b9f78447 Node join (#355)
fc366937c26d053bdcb609539cf1d1f39e501b5b Makefile update for local Docker (#362)
bb72f44cd72ce72bb91efe0ec854f9ca0fca444f Update yaml to use official sigs.k8s.io fork (#356)
e74f4f96463735baea95869b4afaa36d878ee041 Fixes machine delete (#353)
9a43d97eba84302ecfa1ae420a48ff775311441b quick aws test fix (#354)
8cd96f3dfc28f50b17b6fb81228a5f57a56a9cc8 Don't assume compilining machine has envsubst (#352)
98c1267c09f3a3ddf3c4f5a3f18af5d752850dc2 pkg/apis/awsprovider/v1alpha1: remove blank lines (#350)
e3e52b321890b311d2f6306591a94bc5a794caa3 Basic Integration Test (#346)
e97549354fe106bb80960ff5c05bc40ab7a65726 *: fix "Kubernetes" typos (#349)
511c6d444870348c3b4ee5c693cfac521919c0d0 Improve release tooling (#340)
12306a10946a0d06e86b30b5ab055911b7737d4f Update to BUILD.bazel (#345)
b60a402c0d4d96bd1862ab4318cecb0b92a74951 fix gazelle parameters (#344)
c2837933a5d00d6d06b5889a8c54f5ab56a7d4b0 fixup vendor (#342)
54df69fc881e5d3ed77b84ddd14a1c6455b1efa1 Add copy-genmocks target to Make (#339)
d33b43a9b20dd88d5aad67824c9f6c09359b8c38 Fix Bazel image name, remove cmd directive in yaml (#338)
f5be8acd8abdd64c9a29a5a72156a871d6c4e7a1 Fix Bazel image building & Makefile GOPATH (#337)
defe6e55eaeb5a4f00952ed7af121ba25aad56a8 Add state filtering for subnets (#336)
ec1927a4958feded291c72eb2d10642d1be221a5 Adding test script to test ci credentials work for us (#325)
2d1da0d20f907e04533a83e0a1480f9baeef69aa Fix issue if no gopath is set (#334)
2cb0cfef50f04cba4bded73bed92db7b3028b940 fix check-install for empty GOPATH (#333)
8508721fbc0d6bb6e07849c0c70c01e76ea1f3f2 cleanup vendor (#332)
3ea88f5abb515beed333b3381fcc4a8481d2bf7e OWNERS_ALIASES: Add randomvariable (Naadir Jeewa) (#291)
54ab36dc4b0cee4ccc5ce2b212d119aba1d7f710 Remove hard-coded Calico install (#331)
a5f58f497dcec6a1064e2e85bcc1331ccba3508b Adds tests for serde code (#319)
0186e26d3947803182b8638b53226b587dc1df13 Add record package for events (#329)
17d8f035003c5202db9297e10bc4e8869d5bdcaa Do not install binaries to gopath (#327)
782a9d0c25af58274cfbc1ed158373a85c74495c Fix typo in Makefile (#328)
e3bd4dc8eaecd13f68d22dcdd416c4b533e384ee Fix missing vendor files (#326)
f26aaf9b11b1f16c2a6cea50813281bf4c7fceee Fix up warnings displayed to users in Gazelle (#290)
58ce37cf5a8bab888e7ce8ef9a0554f7f840ea5e Cleans up clusterctl workflow (#317)
48143735a99bcb76b0ba96aa86a200abeaa4b347 Move images to build/amis (#309)
399867968c1581e076eb7b794264f5be722e90f3 Fix up the getting started guide (#308)
da007dfea4b1d1f5fc66da7b3d9ee6905d60e10c Fixes for status updates (#307)
faa0c40c34dd18d061890daf53c01601105e0cf5 Cluster and machine actuator updates status (#304)
0253e841a5e99b6169beb78d3f7fd44591940ab0 misc post-crd fixes (#301)
c96f472a6b181325a852336f1258e5ed445dd3f8 Correct location of generate script. (#298)
ba686f17ed9a6525410ea8cd771559efa027dab9 Fixup table of contents from last commit. (#295)
f4691fcea4be1240cc24dcdab548665ab58bcbeb Correct link to CF templates. (#293)
56965c82b8460b8f05a2dcc53bdf78e8e09368d8 Commit vendor to the repo (#284)
382eed10d4af49622e5fce851c811fbf750a9582 Generate manifests with kustomize, fix RBAC (#286)
51b22b06398f69735651d48a721c7e9ff2a33440 Fix NPE in machine actuator (#289)
cac705d86bffcfac0f9edb9bee8a02dda1e418e2 Coalesce test results (#285)
ce1465720123be9f002542387e6aaa492509e7a5 Fix Bazel test scripts (#279)
e6362776ad2f685d8ae7106e14c66322a17b4e89 Updated instructions for new CRD version using Kustomize (#283)
17cbc4eda3ab7c880a9c61d15e638745bfb7e99d Adding a check-install script to the Makefile (#282)
ce2b096f6a9e3723b339a3899efcd06ed92bcd93 controller: Add RBAC annotations for kubebuilder (#265)
19274b257c2f923589879fbade2daad9ed5b9c97 fix aws credentials template for session-token (#278)
b26ae5eae586e0f109e6bdfec50a5d45773dbb10 Use Bazel for CI (#249)
4553a80b6337b4adcc378c07db943772d30fbc78 Uses kubebuilder API types (#263)
78366c21d9859924e8bda6485d59787c59e58e4e Fix looped package installation deprecation (#264)
99b4a24c6543a4c00aa77679850e7eda3d7d3740 clusterawsadm: remove ec2 command tree and ec2 console-output command (#250)
b6b58af8fdad3458bcd797b5a1b43589bcc87a6a cluster-api-dev-helper: Make compatible with CRDs (#262)
944779a1d4a86423a5e7e510b0d9f4b6981dedaf clusterawsadm: Add command to generate AWS secret (#261)
11142d2ec428eeedc3df3f97523e373794d38989 Adds kubebuilder migration types (#256)
de99ab169c2d6dde1a6807d7f2e9251f8e92853e Improve NAT logging & filtering (#258)
68dad3c4c535650ca2af8f5f805249309149cbce Cleanup certificates package (#257)
2a2fe06b51221feb84da7bdbbb77f8b3f9047846 Return a VPC only if it's available or pending. (#255)
ca9682cd9dde90d6f5448d0223794b1e6ae4a8b3 adds basic CRD to get started (#251)
c8c721351b97994307eb4552adb9d80492466cb6 clusterctl: Remove grabbing kubeconfig on start (#248)
a2018e7eb765ed9a574d45e86939289d2e924265 clusterawsadm: improve user experience (#244)
ba99b3b4ae90907b85685cf890ba58f8bb84f434 clusterctl: remove unused "NewActuator" call (#243)
60e91475363f191f3677aef399ff1c84a31832b4 Add initial Bazel support (#240)
c9d7c5b77a1fba7af780f5762d4d30799cefde98 Move some methods into more appropriate files (#232)
a4ede43ebf3f55953f5e95f60503f85b442eb784 docs: Add gettext to prereqs (#235)
9a4e3812199e589b9c952ac2c07812a1c3089acc Fix CI & Makefile with CRD refactor (#229)
da98511864fc54e0baff5678f6f6446bcd3168f4 docs: fix minor typo in "ssm put-parameter" command (#237)
8b76e7bfd59d9f5f9361d7d3488617f2506c94fe examples: AWS, not OpenStack (#238)
67bb82652553c48712632bac6db9e2ccf8f5cb11 clusterctl: fatal on empty kubeconfig (#231)
eb78482d271bdc9c4b7c15a2b43db6cdcddf1e0e docs/getting-started: fix minor typo (#230)
27ffe763e3cd5ddbbf11162c93e7ad7556353769 CRD Update (#228)
196a3b269bf28a570e0d2cc8d768410a6ee2116f CRD: remove cluster/machine actuators (#227)
4cb9802981c4ddedbc55f558cb9a2b4b16218e14 Move cloud into pkg to conform to cluster-api structure (#226)
976d9f6aa1d29baed86cef86a621273279822c12 bastion: Fix bastion code to always lookup via tags (#216)
4e1ba5decc30808464328ae0205f2e43b644c30b Refactor instance security group handling (#222)
d82f11b958ab661817afd0b935aee38aecab1263 use go env to gather GOPATH in makefile (#225)
dbde0ff45bb2b0190946421abcc0317955309f7a Use interfaces in machine actuator (#223)
f7359e75669050a93d73ad0cd019365aed2db31b Normalize/Wrap errors (#219)
3f7039c7dc1bc458a3842bad742957b7f749e54c Start docs around idempotent AWS resource management (#66)
c109050c8f88ebeb9f9081a09449811f07da6080 Normalize copy notice (#217)
4a6f4faf3941e412de08e08519dfbb67cc0d443e Comment out node machine from example (#212)
935415f97d96701572874d12190e217a175b485b Clean up ELBDescribe errors (#211)
371098411039797e9b931aa7c70bcb39b9225273 clusterctl: Get API Server endpoint from AWS (#207)
7109f812d065148a2d6afb01455579e64fb7821e Use existing machine by tag lookup (#210)
798d4ddbaa9697590b8db84dd972d4f46d05c701 Use the latest release of cluster-api (#209)
b1bd83e16b1ffebf2094e2b45651020591786796 Misc fixes for release (#199)
f6765f4228638830d38f45bd58354ac620f90848 machine_actuator: Split into separate files (#197)
ba0224477540c31eea8ad499ad548ae3c3e7493f cloudformation: Add iam::PassRole policy so machine actuator (#198)
de17ea1aeb8912ac9b3ee77548f516d2ced1dd98 Create certificates in cluster actuator instead of machine actuator (#195)
72465aa14740e69784916f2cf10bb95090c530e7 [clusterawsadm] Do not return error if stack update successful (#193)
3a3bc5f3b65ae135a8f6c5be8d29da307e3b86d7 update example and gopkg.lock (#192)
6b5cd83345fe685bd6bfe97d161d21c3bcbc09a7 cluster controller: Delete bastion first (#186)
b4bee019a6d16937b1bf45633a07808fc56c933e services/ec2/instances: Add some more glogging to methods (#183)
06a93025655871b44e145de6abd5de0d5551afc2 Dev helper additions (#185)
262e043bc096bf308adc81b9d0e089017816bfc4 Refactor clusterawsadm (#184)
34aaa092850f68aeaaa8752c48033feb7b4a5640 services/ec2/instances: Fix NPE (#182)
3abdda30f0726f5f37f974a0bcf842d586ce69f3 More getting started fixes (#181)
20d2ffcde4f5b45f57bc74e25d5b4c46287851cc Adds utilities to speed up dev process (#177)
c2566d5aa42dcfc419b762a72e01ba094ef4126f docs: Update TOC in getting started doc (#179)
1887c3147e2a5c7523904c10af6c8d028b1d6e9d Appease the linters (#178)
97c7b62c87d0f2c9e2910445ab2f47c215a90121 Use t2.medium in template (#176)
022bb8ce00dc0a41d7b788b7f38aed9eb86eb49f Misc fixes (#175)
0fde929d6e3cfbecb96a421ecaa68baedb27aece Update getting-started.md (#174)
63b2eedf8802e76e13a192223621a10e987fbf93 Set the DNSName during type conversion (#172)
3fe29c8faa59f508f855ad62ac25fb00073aeda7 Cluster actuator tests, services interfaces, other fixes (#166)
0a08d27a1dd4dd64ddf2ade64a5800bcc0ebc981 Use string for IAMInstanceProfile (#169)
6ee6e685f56ae016138e7ab61956369575b79f56 Cleanup some NPE (#171)
9b6e92dcc99a65f73b98360cad9ec712b3aac7c5 Adds generated certificates (#170)
2a5259c46f35dacee07d048fdee01728106bae51 gofmt/govet cleanup (#167)
6552b101d8818474937df95298ac731beb9b40e3 Initial user facing documentation (#161)
f2d64b476a1672862c338cbb21aed41790352980 Unify tagging and edge cases (#156)
700904156025ad8d164f2515bee612da25dcd8c0 Add CloudFormation template for bootstrap (#160)
351cd29627990240487f138e5c763c61ca1d1a84 Fix ansible temp folder directory (#164)
8815e3031b60d6de0244ab3e56d2ed6728e21328 Fixes GetIP to return ELB DNSName (#163)
e6979d98ae42d43b65b0ef6ccced95ec6101b5a3 machineactuator: Update Tags and SecurityGroups implementation (#104)
4f15a13c391956bd618344c23662a297b20f3610 Remove actuator tests (#162)
77e49593a05605d2b477e5de819d296fc7271fe7 Reconcile apiserver classic load balancer (#158)
e2782de65c24856c4808dea17399a21bcd30fde2 Refactor use of consts and minor improvements (#159)
3346c62086b4a2d82aa5cf3e85049122ab704256 Make key name configurable (#157)
bbc97c590704b05269739a253c21c5d15a564f44 cluster_actuator: Add VPC teardown (#152)
edea2adb5496e955b3a0217f9e40262efd51e75b Add bastion host (#155)
70a109873b2d4e9908279e20399ec559294585f8 Add security groups to new instances (#154)
e8351626ae783909ca655a229ab91b93d0f2e7a1 Add runInstance method & refactor (#153)
a473e99c6f2ce9faf5b184c4389a094d7a142d34 Add ELB package and mocks (#147)
8101679569f046eee7cc2b286190cdcdb30b5813 Add region cluster configuration parameter (#150)
a38efd2c1d2d6f64b1b1aa9945f3f2784a8ed98c Add Instance and InstanceState to v1alpha1 types (#149)
1ca34b2eacd2f5515fed2ba71b3a5898f32d4d3d Add security group for bastion host (#148)
bfeef5086e4c3c792a18ae6f16cd1d38d4039c22 Update README with more development instructions (#146)
aebd03f355f3ca7d6c51f584ced221ca463b821f Security groups! ControlPlane + Node (#141)
8ece4cacc094348080001c4ee6791097c5080308 Create an instance with dynamic AMI (#132)
35c3f832564012eaba3672d75c31efa84cac9322 Improve logging for NAT gateways (#139)
8bddce2e9060eead41e145dc162a6336e1f84d5d Add vincepri to cluster-api-aws-maintainers (#111)
5cd5047eb519b75d6746776b9634adb37e281f7a Makefile: Fix sourcing of env file. (#143)
4f66ebca86132c5470e388a534155916f12068ec Tag additional cluster resources (#134)
227ec809e93b36981bd5109c643cebcd13283f20 Update image generation (#133)
f31ae804e2405487ca28f78cc17a5823acab4ea8 Tag created VPC (#112)
80afae0324c38ae02354e128f68dbdda0ba6ac10 Example improvements (#100)
d63ccaeebcf9d9033da702c000181d867db49efd Fix subnet discovery, reconcile route tables, add logs (#119)
6c95a5e50e97e1d4525a5b9511821a9593612a15 do not overwrite existing envfile (#131)
1a2861d2befe1e784eaa92306c1b4e25675f0c9c Update Security Contacts (#124)
ba663951eddeb50916c587890018c104d7fbafa0 Remove the cluster service in favor of directly exposed interfaces (#117)
d87f7df86711e14684557c5393621837d7b4d362 Refresh README dev instructions (#118)
16fbee44bb4d20714a1ab493f9d11ad59819f4e9 Fix generate-yaml.sh example script so it can run from anywhere (#116)
0777cb967c63a020e7df8a56b436c1fd375bfd9d Refer to `deepcopy-gen` using explicit path names in Makefile (#113)
3427aff7b5e0e885f13827e8408595d3207bb870 minor fixes for glog and yaml (#105)
2b95e0201f2338e162cf918835596f7f02ada2df Add bug/feature issue templates (#108)
f01a7c4bcc5a26a3ab0230ea9fc20dc00088791a Use real cluster client (#110)
551dcb19db61032370d9d0dc4f96091ef4152e95 Add GitHub PR template (#107)
ab3493a6233c10c520a01ae0c9819bbe46d65348 Fix subnet create (#102)
3ba156b026d41b09c074df49c1c484e7e574efc7 Store cluster status and remove pointers (#106)
8335f8a68938d2758df2a4b4cccd16790370f408 Fix NPE when deleting not yet created machine (#101)
d014bcc5556076357cc6249a40e830a2a1d111d7 Add code to handle routing tables (#97)
2edc00001025d6a93aa141275ea49b280c8f564d machineactuator: Initial Update implementation (#91)
31276739017a6f307a9ac585db3b553049668a50 Initial NAT gateway reconciliation (#81)
bc2034c47d1d6c48e61cea7fd8c5774a108e0f12 machine actuator: Fix typo and restore tests (#93)
eb92f933b3a34fd03ec4c4cc0ca2936ee07496aa Support pushing dev images to AWS ECR (#92)
d3df0ea840bb44b0df900f1364c8fde88fa742f8 Adds simple Exists implementation to machine actuator (#67)
8c827ef5f0c7ddbeb7b0177d31165cfe94222abe machineactuator: Initial Delete implementation (#80)
0adcf20116018bc72cd18a4729f6ff3b3800d117 Add code to describe/create/associate routing tables. (#86)
869137220ffdad8ed7b9337f26137ac375e6197c Add tests for internet gateways (#90)
67535ad58f7f95d9636d12fcf698f10ddf5ef2c2 Add internet gateways (#85)
282c3d2abf8883f898b212d11edac277a42f6c47 Adds cluster api machine interface mock (#83)
27b438d5654f674129c5c5838cfa7361f5ea60b1 refactor subnet and vpc with defaults (#82)
938a356e486ff6fce6110f243dd38dc2086b99b7 refactor service, add support for vpc subnet creation and reconciliation (#77)
79f652e98c5ce92d1350022979e53d30cdeed483 refactor tests with gomock (#76)
02ee78bb9f5b680d9343033357a83c87626dceb0 Update dependencies to pull in latest cluster-api (#75)
25efe2df4f2446e9b411dbe78ee416e0b969a1de Add initial implementation for vpc (#68)
f9238a4db1ab6c592a0dd70afda585f768ce4d43 Aws client (#73)
351542502c5ca7ba75279bb6dd702cc5dc4d91bd Improve dev workflow (#72)
6b6cedd8bcf3ef0c30998224511124424cf8d3a6 Adds dev push instructions (#71)
fc27c562447b4eb179fae35e76cf37b66b98e98a Adds tests with package cleanup (#65)
f103494b072a5819119b0d9fc4fcc3dfcf096289 add base for packer and ansible (#25)
c08072a31e7ea9973e88186cd54e01508f61a8b0 Implement skeleton for Cluster Actuator (#55)
b0c888eaa27be15a384967fadf58d91b4744c1cf basic machine actuator and aws instance implmentation (#27)
346e3cb85ad347dee431f0ed0938150c93a4b33b Clusterctl (#22)
45b2ea80f5b5e51d4bc6a041a554e080bea13e70 MVP Proposal (#26)
7f794cffbb183683fbe44edafb54e76f847952af Update generate-yaml for clusterctl (#20)
858b70655680ad1ea40c61019230d83b08a3ff00 Machine Config Proposal (#4)
139cd14693a74a705a582ffcc10ce379daf0ae95 fix tests (#10)
eb36e3181f1dce882e7f56c06d024ea57e8bb641 Adds ci scripts for presubmit checks (#7)
f4e440b580c1ed1e618d00a49f2ccfa121d1c495 update design doc link (#1)
36aba70deb58b2d91146d2b1bfc0ce00440aeb83 Merge pull request #1 from enxebre/owners
c1c2b682666df9b01fd7b2b4937feb8f3dee31f8 add maintainers
dddca32ac95da8b4ee63cc86e605cd9a9c90ba7b Update Owners
91e18276b4ca414b21de9396cc7b7fea4c9143ed Update README.md
59e59db47c257d8981648192502167e5bac4e53a Initial project skeleton
98801d5c32f26229fb495ee8a3d4badb01828807 Initial commit
```

Status: Fast-forwarded successfully.
