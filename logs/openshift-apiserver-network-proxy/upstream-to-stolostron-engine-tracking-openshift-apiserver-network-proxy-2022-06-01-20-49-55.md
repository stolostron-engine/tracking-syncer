## Fast foarding of openshift/apiserver-network-proxy into stolostron-engine/tracking-openshift-apiserver-network-proxy.

## Status Summary:

master -> backplane-2.0: First run, created backplane-2.0.  

### Branch master -> backplane-2.0:

New commits (first branch sync):

```
4da513df08b8af0d87ef029cb221bdcb35d92d01 Merge pull request #18 from openshift-bot/art-consistency-openshift-4.11-ose-apiserver-network-proxy
95e06b4fc2851a4e52a9c85f908dab829a74d7db Updating ose-apiserver-network-proxy images to be consistent with ART Reconciling with https://github.com/openshift/ocp-build-data/tree/5bdff8f034891d949f702da1c194719005a2df3a/images/ose-apiserver-network-proxy.yml
c1f0d79554b857754e2ce06b47b63bf009d44b62 Merge pull request #17 from csrwng/update_owners
a79c1e9348721b9ebfbe7d11771b94806e4dbdd5 Update OWNERS file
e5509dfb75f5f582160465f9ec42d814ec4b98e6 Merge pull request #16 from Basavaraju-G/add-label-dockerfile
6b31048a1f3a431560a0543e97b2dcbd69d2e34d Add apiserver-network-proxy image to OCP payload
c6374b0dd2afc0c709833213004cfcc62d4a4daf Merge pull request #15 from openshift-bot/art-consistency-openshift-4.11-ose-apiserver-network-proxy
01f86983911d9497776c78ae0d48d52e4284c9d7 Updating ose-apiserver-network-proxy images to be consistent with ART Reconciling with https://github.com/openshift/ocp-build-data/tree/bda003f7da37004310548850f710d3ff0597acc9/images/ose-apiserver-network-proxy.yml
ba74ca29f6cead6c103a109024adc83d4fe6096f Merge pull request #13 from mihivagyok/sync-upstream-20220215
447353321e2f10876043125b225b64d3aece3cb5 Merge pull request #317 from mainred/reduce-annoying-error-msg
d156a8c437d0c043aa0d33fa6712e88c57378e96 ignore the log only when the connection is not mormally closed
26e0efc2d5a8c8784a02f2088c335749fbc8a931 reduce annoying error message
0eb91a1ebf9f1af6e2e99fc15b19d57aceb63c6c Merge pull request #11 from relyt0925/sync-comm-20220211
da4dc903e77d7cadcebe4641fb5df2f5a40c9b39 Merge branch 'master' of https://github.com/kubernetes-sigs/apiserver-network-proxy into sync-comm-20220211
078a683a8f5e07fb97f4e0feb5f12daf710cb2e7 Merge pull request #323 from mihivagyok/add-http-concurrent-test
c29f9ca7ea0e94ba4cedc6ef3759728a23604a7a use Lock instead of RLock to fix read-write race condition on http concurrent test
5a3d857863774c357b740bd002f121688d422cc4 Merge pull request #305 from mihivagyok/rework-async-dial-request
98c9562f0fbd8a01fc3640c3404147624b194f9b Merge pull request #313 from alvaroaleman/health-addr
8b71e6f0fb653b402757f120a7adaaa7f0fb974c Agent: Add flag for health server listn address
230801892fff04ff1f49fd1670307c5f8e19763a adding concurrency test for HTTP mode
c99240bdb6cd5570b89794d33a313a80e1176369 rename ctx to connCtx to be more self explanatory add connCtx to connManager once we get the connection for the remote
f6866f4a1100338409c07b3881aa633f8713b1f1 Merge pull request #320 from rastislavs/arm64
3c911ffec387577455ea38ca1327a8cca3b43ea2 Merge pull request #10 from relyt0925/async-dialing
80a1c7fe01ebc467e5016ae54f6a68ccae9b6dba make dail request handling async in the agent
5f5d931d6367cc162959f3655161dc1ec4dae89b Merge pull request #9 from relyt0925/community-sync-20220128
780a61a8b7e42295cbe435efa5a6de469ee4fcfa Merge branch 'master' of https://github.com/kubernetes-sigs/apiserver-network-proxy into community-sync-20220128
4afbf38003e6ec7e67d8b872c11c12bd1babaea5 add missing conn.Close() - do not leak connections
3bfad816057016b2fff7f29486af64031f978744 revert infoln -> infoS changes
2e284cdd1a2ad05e3705e0e383571a2ccbbf4fd8 Add arm64 into RELEASE_ARCH_LIST
462dd0a533fa404a9068b59d20d3a5236b0a696f fix review comments: - log when ctx.conn is nil - handle connection inside the go func()
31f6ed8cbb08a2d16cc80eb3f4344db6354b84fb Merge pull request #308 from Jefftree/reduce-pushed-images
b9bf6c51031b435180466a6ccf2c7e9a531f12c6 Merge pull request #314 from jkh52/one-seventeen-five
cf9e99d529bec59e3064bfe702d288d6f77784e1 Update go from 1.17.2 to 1.17.5.
eac94c1f839a84a7b09146e858f3725503b64cfd Avoid pushing docker images for proxy-test-client and http-test-server
c526bb07ab88066acba16c4943b241ddcf9b71de Merge pull request #304 from Jefftree/amd64
1fdbe51bdb37ceae248185696f82b0e79ed71f1e - make dial request handling async - use infoS instead of infoln
1c2dcc7aa58de993b79637d943d1878f7de9c000 Only publish image for amd64
2ebe8a7a5f2057f709b4dedee9251e16e3fe6a81 Merge pull request #303 from Jefftree/patch-8
3fb3bd706d715de4741f63ca702b8fb0f6d8fb7c Increase cloudbuild timeout
ca97e2c7aa9d215c5f0804e49f13fa0c0cceef25 Merge pull request #302 from Jefftree/patch-5
0a47abfa6595de8bebdb1e65d11995b50e8f24bc Update cloudbuild.yaml add auth step
a8c54abeda0c5398407ef37cd0274075541b1a69 Merge pull request #301 from Jefftree/patch-4
5d18abd8500d71b50f0dc259535c0698199c5676 Update cloudbuild.yaml to support docker buildx
a6a7c13f359f046d1b360f1c711b2436cd105222 Merge pull request #300 from irozzo-1A/fix-test-race-condition
d4d4c618db95a09cf20511a4f35d2d976bcdb512 Defer sending close response after having cleaned connection manager to avoid race condition in unit test
7831f453429d1fdb2989e05328ed4469c8c49894 Merge pull request #299 from jkh52/client-grpc
084136e6f2db15be07928d3e5e92a2a5eaac7e39 Lower konnectivity-client/go.mod requires to 1.21 compatible.
4ca180256f05cfa04e7c11b58d9af961f547988e Merge pull request #8 from relyt0925/community-backport-20211128
c864ffb41c69fcec3b815ab4ed1915ea90a34933 Merge pull request #298 from spiffxp/fix-gcb-image
057ba64f8ea6a6e207c2b094a68ef4ccb6164dfd images: fix invalid k8s-staging-test-infra/gcb-docker-gcloud tag
3d175adc372d7c137bddccc34720a2a2d045258b Merge pull request #297 from spiffxp/use-k8s-infra-for-gcb-image
9237f0cec06325defb56664742ee5acc94bf05b1 images: use k8s-staging-test-infra/gcb-docker-gcloud
24529d92a20a88ee05a4bfae018b3002a56ce6a6 Merge pull request #274 from mainred/qinhao/docker-buildx
baf5431d8d221215e6dc96e2b97ee57beba361ea update vendor dir
c2df8b9e8032dcb89d12d9418bc72789ef93f637 Merge branch 'master' of https://github.com/kubernetes-sigs/apiserver-network-proxy into community-backport-20211128
ae256620eb3d841d2dc92d33ca5bc011d4f7b7af Merge pull request #285 from jkh52/agent-server-count
b40bc697af90ef0e5d08e3146c60bc9960bf55de proxy-agent: support new SyncForever mode.
5944ae0ba9ebf5ae14a3cc412a337d29794ccb50 Merge pull request #290 from kinvolk/rata/client-leaks
93f5a7d314b170b8920546041a428c6ee5d48669 konn-client: Stop goroutine if DialResp is not recognized
d171965cedeb428f7c27f4d628519b2569ad1eb1 Merge pull request #289 from jkh52/kas-logs
a67f5f743e8bd5332768e789f4cfb39d0e287350 Merge pull request #291 from kinvolk/rata/update-grpc
84bab2f997f3a616a7e8376300fdfbe6afba0c4c split all-arch into separate archs
cb613f13fb2e6508636860b4b052fbf0c52a33a1 Merge pull request #7 from relyt0925/community-backport
ebe18eb12192c8dbfb98dc2701a9b59b1ed099ae Merge branch 'master' of https://github.com/kubernetes-sigs/apiserver-network-proxy into community-backport
40710634290fc930807f816dae58f4c6a3c49b5c Update to grpc 1.42.0
d7eca6e9622e4bc09d0a01bb5b8acf740f890b93 Merge pull request #6 from relyt0925/randomize-redundant-backends
6bf6fefee2274982e542737110c662e0ad5bc7bd konnectivity-client: improve logs for DIAL_RSP not recognized case.
7c05e8a391b7048645c7a279ad34334d956c4654 load balance traffic across redundant backends
ae5b857b5b02d924626836835a45d675a5d9c17c Merge pull request #5 from relyt0925/openshift-comm-merge
fc56f4ba47a3da62519f93743830f13abf962492 Merge pull request #282 from Tamas-Biro1/add-ciphersuite-option
2a7e07eec588a5de1524d6f9fe3a4e314a901388 Merge pull request #288 from jkh52/no-limit
cb5906d8a009919676e64257e88e45ff0cb4b1ee Remove cpu limit from example agent pod.
9e52504107076d226563725be6134666fc585273 Merge pull request #287 from cheftako/release
f92efd82760a4d1f8f5339982279e4a24084345c Make sure deps are clean prior to running update vendor.
793abbac6a19c9881fbde57f44b336376c5001fe add option to change cipher suites
a29aa2a8911da926d61c997d522e7801d807cb16 Merge pull request #284 from cheftako/gomod
bc49a880a763b977a5bdd78ca8298627d5f1df56 Ran go mod tidy
39c3498ff1cc90840ab36017addd9cb6f73c2ba9 add phony target for buildx-setup
cddca435c6f35a222a2bd6e19a9c665c82e2af3a Merge pull request #277 from cheftako/xferChannel
3a2c63dbfa54a0f0f2bf85da10dd27f03d12c8c0 Merge pull request #281 from kinvolk/rata/bubble-up-errors
896acb7c8b7714836ffa4c15b17c8b67df58e2d1 Bubble up errors on grpc connections.
2fdfa66186b1b35c139e20e1d0d0d1a246e70d9e Added block check to agent xfer channel.
a007c42f6c9d06ff869da5b93c428546658c414e Merge pull request #280 from jkh52/uds-keepalive
60b7403590d977a30ed2ccb96087b9f997b5a36a proxy-server: in gRPC mode, set same keepalive for UDS and mTLS.
adbe995d9221914136d536dfbb92f313e5fba62c Merge pull request #279 from cheftako/grpcv
5635507690bc74a2f6257fed11a007f43f9945df Add an agent side keep alive.
08077b9daa148920ac3c5ea902119b2ee54c20a8 update vendor
def7eaf4dbcf786df7d5980fe305c7ba367e7856 Merge branch 'master' of https://github.com/kubernetes-sigs/apiserver-network-proxy into openshift-comm-merge
d6bb29a778a92a8d3fcc9cee52985777b7323114 Merge pull request #278 from cheftako/grpcv
361ec7531a03773c56f533e02781837ade2d24cf Update to a recent version of GRPC.
c9ee282a6906469c858e2ea4dd52b4788cfe904a Merge pull request #275 from soorena776/golang_update
ba0318873551cc04de6e4ad960a00841efcd8a0b Updating golang version to fix  a few vulnerabilities
4e54721623664c0df7fa154bd9249ed7a8ff181c use docker buildx to build multi-arch image
4e8b12d2cd77db7ae5acecb5b706d5ecb3bf93e3 Merge pull request #270 from jveski/fix-failed-conn-leak
8b141c70196437b13a9560000183fcb653b46b38 Only close tunnel once
37161720707bcc97ed8c73ea1cac97a8ec00b47d Merge pull request #271 from Sh4d1/remove_Sh4d1_reviewers
e44532fecafaea60f19fb6646d0709dac906d39e Move Sh4d1 from reviewer to emeritus_approvers
58e06413201a31fbc0e04ba156dd7b3847898efd Add HTTP CONNECT connection gauge
f3f6bb08a4c06aa3efe9693c06ca98dc2c3eecc7 Add type conversion and comment
c747eafa58cafdb9d96977cedfec4a6b0d0dffb4 Fix failed connection leak
57df1484a81a85c6984436e35f50003e7cccea3e Merge pull request #269 from cheftako/agent-log
edf4d8f45954e9990b23b861e424b044cd640d99 Add a flag to "hide" the channel full check race condition. The check now has to be explicitly turned on.
daed7d0822779621cbbf9277d4bd0c946d44a3ec Merge pull request #263 from mainred/refine-local-build-slightly
b5e4ac18ab48320f11afcc9e070ed764aa670f51 Instrumenting connection issues on Proxy Server
f690ecaba4700e0d1a86cb15b31c83b4a7b84a3f Merge pull request #212 from jkh52/owner
93029f4ff548c0af61bbb340a55e1b65fb352797 Merge pull request #265 from cheftako/agent-log
6da21fcece82c8961e9b12078ad5a9ea6fb5e14b Improve logging around agent stream read/write.
d999f5fc613660785355af6d40f705cb1f2e1444 refine local build code slightly
47a9234435b115cc764d76c8336057ea27ed0db6 Merge pull request #258 from cheftako/deps
9edf441402225c7b6cfc4394d413f496c07f41a5 Merge pull request #257 from PratikDeoghare/add-after-auth
e90ddb06fa6d62231dbb4de4beda91ea06c3fcff add agent to backend after it is authenticated
ac0f2f72ab4f6dd260f75978f028d05130cc1e73 Updates K8s dependency from v0.19.10 to v0.20.10.
da800daed6eb7fa4b505c2ac5a67136da6b4c7d8 Merge pull request #248 from relyt0925/enable-http2-health-checking
3bde8ef6ba32433f926f1e15768e9e7393cfa73c Merge pull request #254 from jdnurme/pending-dial-metrics
d0eec6a6be457c876a552d30f9d987ad56d9d5da Updated server.go to include metrics for pending dial requests
36d83bc05317cf03a5bc63c05fccffb29f455402 Merge pull request #253 from cheftako/master
8cad10ac53862fa479f28681a5e775db896fc887 Fix cleanup of timeout on dial request.
4155932b9ff1a5919a78a7706d6d4194c0e36c3d Merge pull request #251 from cheftako/agentClose
4054f2b85bfcc7f3e9c280167451a5a2a4900d1b Fixed race condition writing to closed channel
d964a216f8298931dc1745a3a24bb0292d465397 Merge pull request #179 from ScheererJ/master
913d074fe5da8d9ebc509f378e06099d230f0a9a Add timeout to dial request processing
e08b1c1ea7282f1ca146898b0ffe65d97c155307 enable http2 healthchecking to recover from dead connections
a5ef259da4e413ac9398b0577ae125d5f72d827e Merge pull request #246 from relyt0925/update-to-latest-go
c1e7677cc5b434b13947c67898d2e0fee6d5a58a Merge pull request #3 from sjenning/fix-ocp-dockerfile
3d8fa39832faa16cb0319cc36fc4ae0256317b42 fix OCP dockerfile
6eb779ec370631d2f6a8b1b7bae9ede77730ffde Merge pull request #1 from sjenning/add-dockerfile
c26c26f8f4a52c51b36f1b5f7201c3e74cea5170 override OWNERS for OCP
d9e5833dc3c39b682e268d3db33f478766fce4b5 Fixed potential resource leak in race between dial and close.
4811e98a5b266a77e8df74eb426821471bb95f9f Make dial request processing asynchonous.
17944c23169b4be429813fcad5a9e3dfb3c1b84e add Dockerfile
ee17a1314dc4edd8c3b160c752c3664084cf066b include vendor tree
1cf3d2e7be2d05da1e235510175b63e38c22bd23 update to latest go to pickup critical http2 connection fixes
ad45346e68ab4757cdfad420a8623756be7b9569 Merge pull request #243 from aojea/deadcode
8b006e8ca734f2d0c03a15ac8d7b773b245820c2 Merge pull request #238 from jkh52/context
89eb6ca8c58f2085f1de5e7e699cc0a75d9cd4dc Add context to CreateSingleUseGrpcTunnel.
570ba69f1b7179130bc5592a22906aaa6a84e36e Merge pull request #245 from sjenning/fix-default-route-validation
2aeb531ff0e6894b6fc6970d555187d44c45ddad add DefaultRoute strategy to validation
b29b965c4ceb5358e4b0a0b442dee524d0a5f937 remove unused code in server
178138ced5f0761bd6c9615f624777e026f16254 Merge pull request #241 from aojea/client_wait
a418bd1eabbe49f0c9dd72a3bdfaeb9e3bfd0d48 Merge pull request #242 from aojea/client_concurrent
58e92164393811e33344e1808d7a156fc9a006c8 enable govet linter to detect loopclosure issues on CI
2917a4312beda4b9f4d9ae83f211f3fc4a559a8a proxy-test-client record number of failed request
684c2b969033a354583f899414cfb67d2e3d9283 capture the loop variable in the proxy-test-client
5d2b5126a2f0c9640ca0394a0b3b5039fb96210b Merge pull request #235 from SataQiu/update-readme
36f149d83f4b6ff3d70d1c9f6488890d355e7261 fix the wrong command in readme
93c0a7742a689bb0a7c6baef1c954b7f316d7458 Merge pull request #234 from cheftako/metrics
925c618b443d5d5367639a5a709796f969d416bd Merge pull request #233 from cheftako/inclusive
6b74d5e0abe921c56b39538f8f214e658cf264ce First pass at fixing non-inclusive verbage.
8d7660f1cc481d64da991a65551f04b432f65fb5 Added histogram metric for send to frontend.
144711265d3d996e39a98a694ebea496dd758742 Merge pull request #215 from jdnurme/keep-alive-konnectivity-server
554a60b5bacec1e3c27f218d10ec004a244b1719 Merge pull request #228 from relyt0925/default-backend-specification
482479612d9e28f52376ef774089f9d12d6b54fb updated flag names
a88a7044a47f94c228acb5014e4a9d8457fd6163 updated to make flag names distinct
e32d71d78c75245bf9bd079771a5731903835a21 Updated flags for master server timeout
bbc5a527681552ce5c2d0aeb3e9ad930e50c58b5 Merge pull request #231 from cheftako/readyz
9fbd6bbc7acd6ada32d91d06663d77386a6f3517 Fixed readiness url path to be /readyz
cef0aece32fdc74fc1e5b9e957bfcb6e72a8fe39 add new defaultRoute strategy to allow agents to advertise they serve default route
22d911a1253dc2741a30be1e741db46a31929013 Merge pull request #227 from liufen90/refine_main_pkg
56275d63a550204471328d4ae93c839639c15733 Merge pull request #225 from yan-lgtm/master
b6c54eee6acc9294407b26b10116b3782c0d1387 Bug fix
f7dcc1aef81d3caceb1e9eab6770e8fb263916e3 Merge branch 'master' of github.com:yan-lgtm/apiserver-network-proxy
5a9701eafda1c8c0222e991c80900fbe68cd7fd9 fix build error
8d827f62ec30f3007b77c2bcca016edc1641f7f7 fix build error
1ec0e0d4640f6c55c8ae7a0264cfa103d1c83609 Merge branch 'master' into master
74ef7682300969c9999d3966bac3d309a35baec0 Merge pull request #230 from cheftako/linter
8be63d2b666bd7adf69a36241114a359e27f8882 Fix lint errors. Fix the label to be backward compatible
6f3de56514e8b56b99da7d537026245b314d259b Merge pull request #205 from liufen90/master_makefile
ceffc62a84a5921866ca4a2ae9d1d1ed4b3bd144 refine cmd/agent/main.go and cmd/server/main.go
10f9476bb138496ad6a9a56e207d2089cfb1900a Address comments
67469e3f8b70cc7fbd4951dabc73d49aa715854f Add metrics for showing the number of backend agents connected to the server
603aa670ea3d1e8449dfc7ddd9a303a07a53b904 Merge pull request #221 from cheftako/nonblockingWrite
9f0e43ed18be28c1d7759c8be3e1034dff88dc3e Improve handling of repeated dial response.
115c2e2e6ede60ec57d863d8b43d31c7646688f0 Merge pull request #220 from jkh52/timer
b70bf97571ac08998c9ec2735a54fdd1df1055bd Use more efficient timer pattern.
1af1023e48811876046a4b45022487fb7c864f15 Merge pull request #216 from liufen90/master_upgradeclient-go
a818c7b9af186cb5dcfdca1d7c53d29f8dd3aa20 Merge pull request #218 from caesarxuchao/fix-block
9bbe1fc5fac157b660fc8a47e10d57c0ff29573c Add a timeout to prevent the tunnel in the grpc client lib indefinitely blocks on sending data.
8cb411eef4f230ac0aa3c35548e0b711924c9e73 Merge pull request #213 from silenceper/patch-1
92728fc4de9a47f828593e8c318457e6b8630d10 upgrade client-go package from v0.17.1 to v0.19.10
467b94d5c26b3e9d3f09a112ebd7c9f1bb664684 Update backend_manager.go
70e111dcc31e8591c783fad9dafb2f24347711e7 Merge pull request #211 from cheftako/master
5416db20d02ed49ad1ec0d43c71e7c39a2bad4dd Clean up client testing.
609f7f4c67052cfc169da4df96a9528c8225d215 Update backend_manager.go
faa76d334816fb02d20d3364e46d66d2f78955db fix error msg
c88d89a0e32f949706f614207556cee8298b8234 Merge pull request #203 from jveski/always-remove-client
987db026bd235b66abe38a298297a1a89e86f23d Add myself to ANP reviewers.
e8ff21084f4d9e02642b35326c8a864b3c2b816a Re-introduce call to RemoveClient from Send
6dd6bf28780550b57986f7cbd4e73090d5c8b586 Merge pull request #204 from jkh52/metrics
951614123f11e86f72c4177ba4cce7deaf9b58a5 replace 127.0.0.1 by PROXY_SERVER_IP in agent and server-proxy's certs
2de52858f4c1d0954a2b2be8ea8056fcc88c9d14 Add proxy-server current connections metric.
0df5151025ca82ea7b2cd85f7e1de65b263e9ae1 Always remove client when loop returns
847b98331f17962157ed3b56acf095e1d297d045 Merge pull request #201 from cheftako/master
98f2a4ad28ed51f85fd3c6ca544b345d9a11ffdd Added pprof support to the Proxy Agent.
17ec9af1d263506058cd0cb78c36a165daa5ecd4 Merge pull request #199 from jkh52/master
f00b94039560c28d099000cd11430b0ad261202f Trivial: make agent log level more consistent with server.
c744a6b77b95cd4cf7d5b42cedffc43d46e90ff6 Merge pull request #197 from jveski/custom-alpn
cd722638477f519f3c9ca5cef49cbf07d0e84d80 Only set NextProtos if protos are given
cff3667149b7871eb02c06008bb56ea06bc015c6 Add agent flag for custom ALPN proto
89ec41592480a526f9d758cc4a4a1702e508c8af Merge pull request #172 from Jefftree/steps
3b1d2efdd4c49aee481e2d96fb0008e45b1e6b9b Fix bug around low steps for exponential backoff
01a5ca04c985042831bb687dde5030ed4796c6b0 Merge pull request #192 from jkh52/master
b8be7d515ae230157b5024fbc404c3a9e2282968 Add flags to allow tuning k8s client throttling.
63f2c4d590c3e85199e0da7f8024278249348c74 Merge pull request #185 from MaxRenaud/mrbranch
3d8ebcb865bad73c150b8d46b5f9ee1d0db91acf Improve Makefile and README.md for new users
a04e5641db659a8fe7ffb19949593848079c8af8 Merge pull request #184 from MaxRenaud/easyrsa
ed989c7ab40d41c0024b1bdbee8a20fa5bf7ebf3 Update EasyRSA to 3.0.8
a84ec40e4b72be27fd7e0d943035715f2d627e5e Merge pull request #183 from MaxRenaud/make
046b238ac131a2e758d01e7939b4367b39710eb3 Use the latest version of CFSSL.
0b09bccc9905e4d790e2290c16577dae1265e53b Merge pull request #178 from irozzo-1A/fix-dest-host
fc92bc6bcd8f73522c9b946f8040cb7f43a3b4ab Fix destHost context key
9a777b9ebb1dd0145d5323a1e4563cffeb5a14e7 Merge pull request #173 from irozzo-1A/add-feature-gate
4fd09d01b7db1ecab38d4f9389565d5bf98b5d81 Rename Cluster to Node in feature gate name
9b2a77dbb63a22a57066e6b53b1597afffabc00f Merge pull request #174 from toumorokoshi/add-kep-link
9ec023c76ceed4761ba8922ce6f13e2f1e2c4b7a address feedback
b0f77310aa8addf8117271fa11d78caddedab537 Include KEP in the readme
0d534d3ecfbcff74f48087b341b6831d74cc9b2b Add feature gate to enable master to cluster traffic
e4f869941b507b8e1b7789f2a2e922343fbc595e Merge pull request #163 from rambohe-ch/cleanup-agent-conn-contexts
70bc72cfab28b595f32c27676448253e73b93b3c cleanup all of conn contexts when agent client exits to prevent conn contexts leakage
c84318766b305ffd2035990270e8b4e541c8e302 Merge pull request #170 from Tamas-Biro1/add_go_linter
745d8654a688069c894243c10195d2722c585aff Merge pull request #162 from rambohe-ch/send-close-req
6ef51fde6220523cc7ec104aff8dca65082f5680 introduce lint target
0a52211bc9ab47021eb0deb2dbcac9ccedb6c41b Merge pull request #169 from Jefftree/release-doc
28d28a7439fba22965cf0712e090776baf54e7aa Add instructions for releasing new version
7665074252b5d181c85c76b2209bab6063d3b500 Merge pull request #168 from jkh52/master
1869c4f10f53a28d5c865f2933474a990715add3 Fix a memory leak that can happen when the initial dial fails.
20d8f7aaecc1771ac3c84064329b515c22599340 Merge pull request #144 from charleszheng44/feature/destIP-bm
682693c65f196bbee952804264dd68c4d15ea8e3 add the default proxy strategy
1ffc0f0e4d3432029f81c7d5b222bfe877a76ee8 the agent identifiers pass to the proxy agent must be URL encoded
a1f54197ea92c5ebce16a4f3d54bf2ff3b6eb137 send PacketType_CLOSE_REQ to agent when tunnel serve exits to prevent conn between agent and remote leakage.
2fdb1a46954b1e99af989b037e543751eae49fe0 Merge pull request #160 from daixiang0/slack
54646c2abc8229e59b8aea65189752830f49351e Merge pull request #159 from daixiang0/patch-1
d484628e842d7fefded561018610b5dad340d04e README: update slack link
013fe964dffbefc87cbab9925ca3bb59ea54123e Update README.md
dbce01fe7e6559cb6fc291c645e8c2e37fa32f97 Merge pull request #157 from Jefftree/default-logging
43c884f8666c69a0227f9186d9ab5633fd0816a3 Set default logging to v4
0a13b9f2c92f45a61acb6f5fd65f089f34bb91d3 fix typo
da08f7fe4a497126a6a0e4222fade8a701560683 remove FailureZone for now retrigger checks
dc930106e79e5ae7205fe1c02e1d1d8a99fdfc76 1. change agentAddress to agentIdentifiers 2. pass the identifier type into the BackendStorage
2c91c1e17354df45184476a8f6526cf9a7ff4752 implements the BackendManager list mechanism, which allows the proxy server to have multiple backend manager(BM). To use this feature, one can start the proxy server with the option `--proxy-strategies "destHost,default"`, and the agent with the option `--agent-addresses="host=foo,cidr=127.0.0.1/16,ipv6=:::::,failure-zone=us-central1-b"`
408d5bb273118211d4dd87be996666c9cacaf34c Merge pull request #153 from Jefftree/multiple-grpc-options
ba87710a25f3133658d83cd776ff7b87cefcab2b Support multiple grpc dial options for agent
806811f25d4a6a18ad10d7450ee2665e03be1906 Merge pull request #154 from Avatat/server-keepalive
b6536887ea8e8d31e7d7329bab46d46f8f0e6c86 Add keepalive option to agent server
3cf58829c4f429fd038b7a5797d112979878060b Merge pull request #151 from cheftako/conflict
425f280dd41a563dab5dcc68a38e820d0bdcda6a Fix conflicting port 8093, problem on local testing.
727b66f2fe755f921dcd563f8d198ee7a562ad55 Merge pull request #150 from cheftako/test
7749a54f018fc66b8daf394c9d28efd4c156716e Defaulted test client log level to 4.
43045367f3839b00653198b932123e4c8fecedbc Merge pull request #148 from vinayakankugoyal/umask
42458c2489abd50142517e6476db30acf4ac10d5 konnectivity-server should make the socket group readable and writeable when it listens on the socket. Most systems have a default umask of 022, meaning when konnectivity-server creates the socket only the user that it is running as will have read-write permissions to the socket. This means that any other process that needs to read-write to the socket needs to be run as the same user as konnectivity-server.
a2242e427bff1e484e9f30c2d6c91bfdea7008c0 Merge pull request #112 from mvladev/add-log-verbosity-levels
7ce64dc6cd99f7b6f8043bac94b2f2a3e5f7a0db Fix typos and log level for empty packets
2e0ca71784246c1b72a3f42afcf7e714fd7c0f8d Add verbosity levels and structured logs
9e6944a352493d11bc5302db36efc88862490ebf Merge pull request #143 from charleszheng44/designating-bm
0f3d541108225f5f0e030bda79deda67ae374a25 Decouple the Backend method from the other methods of the BackendManager
ea6f33562405c10156a300c4fd1f4194477bcb45 Merge pull request #139 from Jefftree/patch-3
8634d39cd99619e35eeb201a81a49afe5572fa8d Move metrics handler from admin to health server
3a3da81ac237c5823e6fb2e487058c21801846bf Merge pull request #136 from Jefftree/optimize-cloudbuild
6856dca3b78ec213f1a911ad3007b6be127e20fc Remove docker build from release staging
04716f75f9ef5ca9ddf6c4f9192a885800b46b42 Merge pull request #138 from Jefftree/stream-for-frontend
bf56118733a0f66621a0311eb2b0433bec456270 Fix race condition with frontend cleanup
5136fd4d13014203252f36c42c82e117e5167618 Merge pull request #131 from Jefftree/netproxy-fix-client-test
dda78c5a97bafae59568c03703dd07fc9f60b765 Merge pull request #129 from yue9944882/chore/var-typo
60275bcbdd4cf03bf03a499cfe7e92d18a1dff02 Merge pull request #135 from Jefftree/docker-push
7832111d6765e30a6b73b93903ea503aec0deffb Merge pull request #134 from Sh4d1/patch-4
41675952b7ca0d692623485f614e0b5cd9369d4d Increase cloudbuild timeout
b62efe2314888dc23271a802700f0778efc54a31 fix typo with docker push
769bef1115e5a42279f8953022bbd88776fed0f9 Fix konnectivity-client test
b184b608e9f24a50c95eb0a344ec9b858d43c60f Merge pull request #128 from jieyu/fix_makefile
ab43d56985f3032edcd134c73946d0ada5690921 fixes minor interface assertion
1887e2e683f37d7bc5732720542ff500eb9a606f Merge pull request #125 from Jefftree/fix-agent-reconnect
9d269717a1049630791939978a1bf5b5e73a1daf Add test for agent disconnect
5689c0ea5fe7dd04f4fd36581c0eeb3a1d0271da Make certs gen work on macOS Catalina
3faec2750541599eb811bc54acd326073f73599c Merge pull request #121 from caesarxuchao/close-uds
0fd0b932ca684ce7faa296805ca9252381909da5 Disconnect frontend if backend drops
687b682306b3a0ca3a95fa56b9a0ea0ec6cc5cf4 Add an option to delete existing UDS file before listening on it.
81cb3f4e6855a1f8e5a5b94fa02d9c2ebcb1b06b Merge pull request #122 from caesarxuchao/add-server-pprof
5afb5f2ac3e934484097208baee832b246c9577c Merge pull request #124 from cheftako/test
afa2a6326937b929fc90e1db9a0457eb6e6e32ab Added controllable test http server.
d8eb7a25c66f7024c88533d12e36fe3f900fe872 enable pprof
c9cec5ca1ad40aa668f8d9c1e594ce1cea666608 Merge pull request #119 from caesarxuchao/more-metrics
20e36da5038b7d15afa40440e9b199ba9e6c5acf Merge pull request #120 from caesarxuchao/server-metrics
8488f48e8d44d772a073433306812d72cbd1dad9 add agent dial latency metrics
21f1fa7b097421349e04447e7705451530c5db7c Include the latency of sending DIAL_REQ in the dial latency in case of http-connect mode.
ae471b1e14ac0f4fdc06f3a2fc0f31d286db315c add proxy server metrics
de6fcbd363c088f224a3689d390862229aadcdc1 Merge pull request #118 from caesarxuchao/metrics
153d78f92fa775106844bfd902484bcca95b3700 Add metrics to the proxy agent.
5726ff46c345edceb49a5b7bcb019e4cc84a1a7f Merge pull request #115 from charleszheng44/dns-localhost
c005aeecd78e6abb2fffaad5944645124da360d3 add DNS:localhost to certificate
b202c6e0d79055b7f6dc0a87d8fb203097417f57 Merge pull request #108 from caesarxuchao/remove-retry
7d3dd7f1e3262492f91e2630d05c9d4d34914a20 Remove the proxy agent retry logic to simplify the code.
8c608e708f561e75e9db23edfb0b5acd0c5708ec Merge pull request #102 from caesarxuchao/readiness
6a8e2426cb8273702ded19172fbfce064d893a24 Implement the readiness check of the proxy server
f8dece94a03dc9a90bf37ad50f8d7804bb5f1a92 Merge pull request #110 from Jefftree/protoc
b135cd5cd3acdde7ed1f5f56251aa57346324532 Update README to include protoc
554ed405179653d3f137cf67d6a53b323740e338 Downgrade protoc-gen-go
9667f2ddea24ac50a22531484bbfbe84e39485ca Merge pull request #106 from cheftako/race
09de8a3e34c11a2119c1d1c71cb9fef8809d8103 Turn on race for tests and correct code.
33b997865007d1f12f57d8c2f0d61cd031372bab Merge pull request #93 from Jefftree/grpc-close-conn
35518283193be0c4cc1a44e66f7600dd6b0c27eb Single Use GRPC Tunnel
3e53817abb70e069120534a5b7106ff5bbb108bc Close UDS socket connection on completion in GRPC mode
5ab9684eaacf3d97cd2359a54143f0060a001b58 Merge pull request #104 from zanetworker/fix.sa-auth-mode
99b10f830627b1b55bf074295634784eeac401e1 Improve validation to when using SA authentication
e6e9418c08fd6619bccfdbd0345384fc1c554509 Merge pull request #94 from Jefftree/dial_rsp
e22230a8c2a5fe9070d7bb9e253dcfb80f8607c0 Close HTTP connection if DIAL_RSP contains error
42e9699576b77d2d6e0cca3621917d10aa34e2f2 Merge pull request #96 from Sh4d1/health_proxy
402679da43f8e4981e0dd2f8174f58146543689e Merge pull request #99 from Jefftree/propagate-caller
cce063183570f8b68b476584cabbdbcd1e7af310 Merge pull request #100 from tanjunchen/patch-01
bd8983c15198c2199b53638cbcbd53f47285485d Log user agent info in proxy server
e8fdaa81344a2d3618781ebcfa51823e36c78ec9 Switch to klog v2
be6b06dba50ad4b81529d4ab23a76c41cc2064b9 invert health and admin ports
33265276daba4eab3aa1d3d24f002c2c45c96c0a add port in example
70a5a5a7376cf3a7686dd452e971a4cfb1aa2927 Merge pull request #98 from Sh4d1/fix_panic_no_backend
4ef1b60316a77ec10e2678625d2af4c9d405dc74 add a missing return on error
38b74f928a2c4e60e4bb88cf4135d2200db1534d add health server for proxy
a2f5197100239475b57cba43f95c55b6101e26ec Handle case where DIAL_RSP contains error
ff5e07c4048701a7d19acbc70e634e108d05bd0c Merge pull request #57 from Jefftree/doc
c9359490a03d6e550bdafd7091e271a89a9e5553 Merge pull request #91 from caesarxuchao/refactor
b752d631decaf4f6562b1bc57d259f171be63c07 Restructure the directories
e429016415c1f885518f494a2116b97bab69369f update docs to remove vendor
92d98b013dd42035b5dfa93b06761f85543a1af9 Merge pull request #90 from caesarxuchao/quick-return
67e354888f355397b7a5ec1414a5e342d8099926 Merge pull request #75 from Jefftree/patch-2
6c65e12808de2c2ac66b06ff58ed99cc719fa602 Fix warning message if agent disconnects
211900313620435cc3a1004bf95bb1dce0e82e23 return early if backend is broken
c967cb0d1f680d39945e3175b122f8f89759491a protect agent connContext
4ad355b74e558161e26a71e5cf0514ecbdff7e2f Merge pull request #78 from caesarxuchao/add-packet-size
2ee6177e6b3dc40dc0f3f59b525c7e6d0ccb8e4f Add more logging.
d7a881650b1a40ba116082e5baee75b27f37f1b8 Merge pull request #82 from caesarxuchao/use-bufrw
35d320d5a84c4987f2613cf15632254798cd44b8 Use the bufrw
da0186e6db180d4ff153be228cc7465bfe44425f Merge pull request #68 from Jefftree/admin-port-dont-use-localhost
7c9c74f9b4e35df569aab3b724458605396566fc Merge pull request #58 from caesarxuchao/concurrency-test
645b8cdf49efa406ccd9d99e1afebe8b6a83178d Distinguish connID of different agents.
6755b429a7d29a2b4e0a193831772c232f5a60f5 Add separate port for health server
5ee6c06c9135d0398f72771d96c8227df541e380 Don't listen on localhost for admin server
02dcfc2ed56fdd4b79ec35bdd33ee00ff6d2c8e1 Merge pull request #67 from Jefftree/client-proxy-separation-readme
5a1d08f9e7fb2a53b0a181bb00c194be4d674442 Merge pull request #71 from Jefftree/reduce-log
1169cd6b06802698efcfbc8fe0485708f5ca9552 Change req to req.Type
8910850965a3307007830a3bb69b3b12017eaaec Add note about importing
ef0d8904d40440b21965704d715902ccbe7a836e Merge pull request #65 from Jefftree/fix-docker-build
818303774674bec490cbb5b121f0ac39c9acaf1a Fix client proto name
599e184e191a30b0d0f1a801e0a8131b59787418 Add konnectivity-client copy to docker build
8bf6a95b2312c8f09b01f86b4950fde735990a0c Merge pull request #59 from Jefftree/split-stuff
08d981c5e420052d8e2786044f237640a925f4b3 Merge pull request #53 from caesarxuchao/exponential-backoff
2a115c2ff31644651f4004ff1b4ac39cdff76c37 do exponential backoff in clientset sync function
a43037a6c65af0914025f9daf2013aea90ebd271 Undo dependency upgrades for konnectivity-client
56a50af9700614de76c520bcfaba60e280bedf10 agent and client proto split
65cfdedc7aab3381b56ee5ae34a222a51f53e0e7 Merge pull request #60 from caesarxuchao/add-owner-reviewer
2a864f67ee3e70af73aa41a7cf3562ec8638ea13 Move client libraries into separate module
65263a9fd4e810f76bfe586164b33c7ff12df437 Merge pull request #51 from dberkov/token
32635eda76b8d209168d0fcc354eb76360eb5be7 Adding support for server to authenticate agent
098b812d5f66806475442eb90494585a3b601a85 add an owner and a reviewer
850364616771cfbca9ca505a49ca4db1be838ef0 Merge pull request #52 from caesarxuchao/minor-fixes
f1baef75de587bb6dba8187541f36318907e331b Merge pull request #54 from caesarxuchao/fix-makefile
7b74f53ffe79166afcd9aaea0a703a7e16194215 fix typo in the makefile
c1639234bdddecdece84386dffda7c8ef5acb1f8 minor fixes
233625485a9484b788623c7b11e5ccbb780a80f2 Merge pull request #46 from caesarxuchao/agent-connect-to-all-servers
1aa2e5fa5ce5c827d5717a00950e5389e362a064 addressing comments
8be49268890b74b5909c4f3ce71aa702da72e9ed remove duplicate fields in ac and rac. Only rac has a copy now
26b4ab08ec9816ee25d6c02cdb563c8912b8a30b Add a unit test for ha proxy server
f330515da9b27e0ebca8ce949112bf418f506d49 update mod and vender
e2a8b6fa87b3002b6280ac3a3eef9f19c6e5a5fd fixing tests
57d5d3e64aced724ded9a20c3bdccbbb0204c028 Updates the proxy server to interact with the ClientSet.
0af05b173519bcf65789231489b3758119d81f00 Add ClientSet to handle HA proxy servers behind a proxy.
edfd3417ecf1a9332cc2c8c51172d156a7195034 Merge pull request #49 from Jefftree/patch-1
47b3ebfae2034ad64660003d8f8ecb36d5fcb77c Merge pull request #48 from cheftako/master
b8db36eb7e634a877715652128a28d2113a0efd0 Merge pull request #50 from dberkov/uds-name
024f3bff99b627688f3d61ad18b0d23ea6710c22 update to go 1.13 since k8s requires 1.13
4c672e3f3c41e87c790c7fe710c2bb9cedeba647 fix for go 1.12
5216b6b8b31d9b2405df11e24fdc62f143669f49 go 1.13 should solve CI error without flag
df8f8dac622d83a9c70303fe5dcfc6d1c96304a3 Fix CI
ccece5d0391790a948883d32f56486ec68fbd588 remove vendor
132eb8fd7265af761313f31d7d1a8effa1660499 update go mod
e045cdeb13598628513f7ba9c7e60227738fe549 update Dockerfile to use go.mod
2359a0771866e945ae1ad3d91241c047bacbd47d Align proxy/main.go's flags naming convention with rest of the project
7c9384b8aa5a2c15e424c6eba0a44c44f347e2fb Change grpc.WithDialer to WithContextDialer
b03c1980e62adf37c7f9d72ebc411788c4e9c359 Merge pull request #47 from dberkov/auth
166faaf15fec6fc5887ecd02559cd42ab46a385f Adding support for agent authenticate server by using kubeapi-server ca certificate.
20b729910d7196c7ae8c39ec67c9e65663cf13fb Update reviewers to reflect current contributors.
a03ea77aa169a6beedd040749b32fa30ed4b5a6d Merge pull request #44 from Sh4d1/clean_ci
2260a7e53da3bc48f8fe86dabf9383ff7a56f203 Merge pull request #45 from cheftako/uds
e5412e08bf59d07d8b243d52a0c8a1bceee90618 Adding support for UDS.
fea45dc0de46cdab62f2b07029cc481f5b71282d Merge pull request #42 from caesarxuchao/minor
ad4a57595ac2ff40930444a080a601d158a39cd4 remove uneeded travis ci and golangci
6ee3f3e417a0a8db78bdae0137f0f5a52aa52ac3 remove duplicate log message
8100da112f1cac73fe08562f29d603d89181cd0d Merge pull request #35 from anfernee/concurrent-test
9028280085a0da933d9b591fa072c3aeee0c6701 Merge pull request #41 from Sh4d1/patch-2
e8dc46a5df164c282e4b64978e29cb553bc871b1 Fix missing docker experimental env
09738b1b5315c9e35c1c84436ce9d14bece1b7f8 Merge pull request #40 from Sh4d1/patch-1
f3ac3a86f6c37c8bb17113c5e7d785acbc77f8db Add tcp echo server test
66155b9c357d19c8c04789a914e68d9c567659c4 Add concurrency test
0783a3b4880ec2bcac4582fbeb33aa8b3dc2c09d Fix build makefile
acfe94e9db7c1ebc2848a9981e10ba635dbc74d1 Merge pull request #39 from Sh4d1/fix_makefile
4a4249518ec8890557479dde8f384c5d21d0d0b4 fix Makefile commands
71f9d2867e55c0f688ece9dce55718450e25ebb1 Merge pull request #38 from Sh4d1/multi_stage_cloudbuild
a1d5e4d8d8c5751f411e4f0887cbd6dd4563e614 change place for docker experimental env
a0fa98fd8567fb2fcef25557e9c1d4d6c3588b84 Merge pull request #37 from bysph/master
96e724fc67157e18806a1f36e8b54b5aad2eb1ac add multisarch and cloudbuild
5b4ede7e8f6ed3ef2f10f3cc9d4d412e1a34efed fix golint errors
3b44a3df95555c2bde19f626a21fc3825543a0e2 Merge pull request #32 from Sh4d1/add_ci
a1a1a1ba3b1b12a55b638acd0f603cd2e9171815 fix error message
80039096d6ecb59a8000a5d0c0adc7814467d327 continue on error in server tunnel
0220dc7fe54dd7857f757b150bcd9091efa4e289 fix to pass test
fbe17788b47f5489d846274292d45d617437694a add CI and fix code to pass linting
72862c0d791296a2789bd9c1a4827e8656f0c915 Merge pull request #31 from anfernee/agent
ae0fa93afaf8deb5da7b07d4025a0de275569059 agentclient handles multiple waiters for reconnect
e846112b23a2a2c751a775d7574c6ab7b02fbc90 Add integration test for basic proxy functionality
dfa7cd1277b120bd63ad4379002164a25270876d Agent supports reconnect
8ebdad54073fe690c81d21dc9f54f6b698472eb8 Merge pull request #29 from cheftako/master
43452412877e5078c13a57f1c5abdc3cc003037c Fix error on DIAL_RSP for http-connect.
a3b4aa976bfa3c90e44c054c6381a2c805d9c5d7 Merge pull request #25 from cheftako/master
82d0998a142b68d651b671a7b3fc811640062981 apiserver-network-proxy flags should use kebab-case not camelCase
b82dffb75655efc9a2f9ac48347f42b55ed00359 Merge pull request #22 from anfernee/improve
1d53e53c14681499223331a354bb271d7e728d78 Several improvements: unit test, logging, comments
856ad2a1cd203d12018833b4b1d18c392d258284 Merge pull request #23 from mvladev/move-to-go-modules
4fee70a46769fb856c700a513cf2d4e9ebe2b051 migrate to go modules
41c12edb6b3f3aab387460a58551c40b947151bb Merge pull request #16 from cheftako/master
35c008ab0144e4e937e896a603d4e1b07a66483c Merge pull request #14 from anfernee/close
83e81a0523df9258066872345441cba7feb66b67 Implement Close
3cb6b96790788fdb54e93e7a7e300a36aaaa79ea Added code to get http-connect to work with the test client. Unified the logic for client grpc and http-connect. Introduced a getDialer method. Moved all logic for grpc & http-connect to getDialer. Made both paths return a dialer and swtiched to using standard http client.
1eb6f70777a28fa842415fc38a95ac7ec9954a32 Merge pull request #13 from cheftako/image
1e5f502852483339f98211ad8f030e495c07c61c Allow proxy agent to connect to non local server.
cff3efc9e5e96a544184a397b384665a6acca5a7 Merge pull request #12 from cheftako/image
2c64549df27af42d809b716af0389e49599a394d Added target to allow image push.
150a047893577aeda7d64b970122608ad84f34e3 Merge pull request #11 from cheftako/license
fab277e3d93ea47be253004db95641a927b2858c Adding basic image generation targets. Factored in feedback from mcrute.
328aa99376dc0c082036272cde0e981c45e1bbdb Merge pull request #10 from anfernee/master
890e17953882b3ae54167075a3334ab483e6e27e Code cleanup
2610aeb382ae22fe308ca3d7762b41ad2e3e1307 Add agentclient unit test
a43a9e3559bcc64e96408d3b8213674b28a26574 Fixed license header on proto.
5791bad289a08dd8661048c4438d95a61dd42767 Merge pull request #9 from cheftako/license
9f9e74aa68fb664dc3914b9b7db523f3207e7055 Fixed license header on proto.
2b1aecf1751291db8455dd3bd7d80cb5b5d6b02e Merge pull request #8 from cheftako/license
1b575d817056baa52964b84f14592cf26f04423c Fix incorrect references to old repo.
453d26180018724c22e7e71c574bac374ff30566 Merge pull request #6 from mcrute/add-headers
3052da9cbad21fd9b0144e45c4ad32f1e04b0f9a Merge pull request #7 from mcrute/gofmt
65a61e9be3b559c2c3162ab022c8bbb62577c16e Run gofmt on all go files
ec6b80f87bbd98fcd2a1665286848de434604f36 Add standard header to files
7d26b9f77bb9a7b5dac18c255035e3c475000247 Merge pull request #1 from cheftako/setup
35fcdb848e3d9d0cc5bc9631bdadea901fc0b73a Fixed issue with grpc client. Added README for using curl as a client.
a83aee42ce2f9957c6815094c5474b59d730cd0b Fixed sleep to be a connected channel. Fixed logging feedback from anfernee
5f6c12940ccb47adc86690d6d6a9674cc16a644b [WIP] Adding mTLS changes.
f8d5c2c90d41dc4355e8a2630fe5475340347dc1 Move proxy-to-remote traffic into a goroutine
3e0cc006cffa7368d7a4232031ad11db4e61e794 Revert "Add new proto interface for proxy2"
d0da4f218fa10f3c54338427bff8ef54b49846f3 Add new proto interface for proxy2
dc4e184f1cdca3d98003fedda0aa86ea1c3c7c99 Added proper metrics endpoint.
b12387b93a7f347a2dcba6e25c48f48ef3ef8871 Added rudimentary healthz endpoints to proxy server and agent.
0e8c8fcf3622f486871819e128ca3bb32c7ed8b6 Updated code to handle mTLS between proxy and agent.
d4e551229cca33246a26315a9515942aa2182965 Update vendors by dep init
6351d63022ea1a7345cf62595b9027acee80a2ba Added support for mTLS.
94324367715fdf3081e922a756d103b014c11b6c Switching standard executables to live in cmd.
f5965776fba7d563e3d69cce6bd234477cdca3c3 Made build slightly cleaner.
3b5f1162a8dd5cd1edbcf29fc70ed91632235b7c Update README.md
7dc2206685e485745919cd1bf4c771c3fca6e3d5 Move cmd into examples
4c4d37f2cab9d6696e8af9dbfd54f58ce94d2dc9 basic agent service
275166d99d5887c839d1c12bcaac7429051bbef2 basic support
bf83efc52627221735edaecb3d3539014bacddaa wip
942dbb06b9703a2021416b85b9905c350410f84a clean up
c2626a9ebbdc4f966bf81865d768060d08ea1d64 comments
7dda23beec606c024f1fa91b20fe8c7546923449 Implement basic proxy
57e090ce2f3179bc6013880a01d9bcfa6eaf7366 Update template files to include repo-specific info
5371813d346ce7cbcd3cf1fd239d230d5f445bf5 Initial commit from the kubernetes-template-project
```

Status: Fast-forwarded successfully.
