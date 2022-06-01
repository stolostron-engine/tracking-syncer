## Fast foarding of openshift/aws-encryption-provider into stolostron-engine/tracking-openshift-aws-encryption-provider.

## Status Summary:

backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
02fca6c24ee5c55327cbabf08f1e96acb8e64e7a Merge pull request #3 from csrwng/fix_lint
ce1cb506e40c869874e75053f6590518c2535d8c Fix lint errors
22e71fec40199d05d158a7046314833bc64d03d2 Merge pull request #2 from csrwng/openshift_dockerfile
84430c8b15333d84ab80a8cc57c50e03fdc32a87 Add OpenShift specific Dockerfile
a96718230665623012af665473a5015e8ad922df Merge pull request #1 from csrwng/ocp_owners
32d55b1a0ee377d6e9859a4a5a292c658a2ca68f Update OWNERS file for OpenShift
c4abcb30b4c1ab1961369e1e50a98da2cedb765d Merge pull request #77 from gyuho/error
e1ae850152c7097aaf47374b507e44663d4b2846 *: use named testing.T.Run
670ee14f117daa054a6592b9501267ad6f1d0ad2 hack/golint: pin golangci-lint@v1.41.1
150ab6793c3c94a36cec2fa301f8f96b5a575619 pkg/*: clean up tests, wrap errors, update types
9366918ddcc8f0752abc5c004a3f986f1e7c73ce "/livez" endpoint: initial commit
3b753805908e18734abda2482363fef6fa7e9a42 plugin: add "Check" API to discard user-induced errors
e1e9ad2ff45d4cdc567d782f3adadc74bcd59c2d Merge pull request #75 from bhks/fix_cabundle
2b6225806e25c4f6d3b71acab896150e25644f11 Updating AWS Session creation to be able to use AWS_CA_BUNDLE environment varibale
959eca3a6354703db2529219bedeebee35599026 Merge pull request #72 from syncier/goreleaser
ccec2f83c714b830aa0e04b9272938244a781d7e manage golangci-lint via go.mod
69d30c0e57c08c46e884007d610175b836c0ba85 update go.mod to golang 1.15
bee5673b035276d58386d51f5e411ba5be454934 Update go version in Dockerfile
20b037c1c11005c1b5de1c836b34ab813b18a305 go mod tidy and gofmt as part of linting
124b65989f8642fb649a89ffa4aeab7f4b997175 Address review comments
53b86edd67f97a0c84dc072c7b7b61ff3d3bea79 Configure goreleaser to build client and server
01a3b6dbc137a9f9d57cb63a8ab2c9b4b4c5f203 Merge pull request #69 from elordahl/fix/docsdash
8be72332c999257544db0354a19e0e45e37c4efa Double-dash(--) args in example commands
bed12e4c3bdca596330823b7988a310901c14f59 Merge pull request #68 from nckturner/update-aws-sdk
5c192463e5f1bce7b1f91c612994e0054659aaaa Update vendor
b8a6534e3cd3c52360cd5e222a88bd59245bc5c9 Update aws-sdk-go to v1.31.7
6c2b3d01151c90be65de9ed21d51a1d212e16bbb Merge pull request #65 from bhagwat070919/testimprove
3c26e5243c51d99b4c5bf978a6ac070416eb0868 Improving the unit tests for client_test.go
03bbda0ed6c2f8adcc30f9e57c6817c8436fe805 Merge pull request #64 from gyuho/deep-healthz
277f295ba26c392d8f7ce184ac660bd351c93446 *: separate healthz package, check KMS API availability, add throttle failure metrics
c295741f8e321864e0aa716f31ff353801ce6f97 Merge pull request #63 from gyuho/logging
c5dcd7e68836579db75f9deb714bb9932fb7b616 cmd/server: add kms server start logging
ea3276c175184c486f514e3007d30dd6a0bfdf35 Merge pull request #62 from gyuho/flaky
982ec9798fbe73a62b299033689dbc6b29bcd3e5 pkg/httputil: mask "dial i/o timeout" error in "TestNewRateLimitedClient"
ffe55e1b83b98f3b477682945dcafdbf4881b7e2 Merge pull request #60 from gyuho/encryption-ctx
1e93e662f251e576fd208c200cbad878ed4c51d7 vendor: add "spf13/pflag" to replace "flag" package
58121022582c6d2b08d10a4c1f433c5658b4beae cmd/server: add "encryption-context"
c58333c7415a8580c3c5fc7ddb2fb20611d45798 test/integration: pass nil encryption context
dab0b25e70cff1e0d63d2a0d23ee49997426ad22 pkg/plugin: pass encryption context if configured
1186f4be0d5dc3b5a2a7503cf5890f4944e1318c Merge pull request #59 from gyuho/rate-limit
3f15e30cf5b7a8d6a82631b05957b2a45ef97def *: add "qps/burst" limits for rate limits
953c5b4a45d3933ba5a81f58b8b6179ab6a2d115 pkg/httputil: add "NewRateLimitedClient"
c6406ffb7816b67554f203388e3544af7e776ccf vendor: add "golang.org/x/time/rate"
1a969db6ed1230a9f1fcd41f4b74f351801fbc34 Merge pull request #58 from rajatjindal/add-logging
c15e0659c3118d3792244b709ad6a2cc6efe558e add logging to encrypt/decrypt operations
088ae784c8bb81d13fdc62e5241a701947b225d2 allow debug level logging
2e47c0ac41741ff50bd851fc6f54a35c8a22e8a3 Merge pull request #57 from rajatjindal/remove-cat
32b7cb0c5a6b20943c8ab4549d8f87b27e82502e Merge pull request #44 from gyuho/dockerfile-shell
bcd895a7a896e256ceff4b26d52f55ebde65bccb remove cat statement that was added for debugging test failure
063f5fbeee53782ae36403caf010701520e4b575 Dockerfile: build from "busybox" to include "/bin/sh"
3ece52888343a257533b210234047e9615f63ef9 Merge pull request #55 from micahhausler/gyuho-owners
be4187ed25aac541124edd5780a1f874f0c79593 Added Gyuho Lee as owner
efd26959af668525cded07f004675df73891c4bf Merge pull request #54 from rajatjindal/replace-glog
446fb46238bcbc2bdf95a436bdb7a74ef556056a display whats diff
6b20beef653288eb4620a2bf40ce93bfa60cf20e replace glog with zap
a55fa7f341f0ec930b5a82dc5818ee890a358d81 Merge pull request #52 from rajatjindal/update-makefile
4c155d90cfc18c2ba39585337ecc2619cceb4201 make use of vendor directory consistent
434773b1105194d4cd622739b20149e9213da19b Merge pull request #53 from rajatjindal/update-ldflags
78d9b5bf7d0d1b6667273c514f1a955e5535cbef remove installsuffix and add -w -s ldflags
cbef4a6d522c65ee34665afd157e98fd9d7e26c5 Merge pull request #51 from rajatjindal/override-kms-endpoint
88549a12d23a1dab5971e229e76b3e7fb2c7ad74 Merge pull request #48 from rajatjindal/update-go-version
9771081488e9b70ffda3b04b0f4d69113d1d6c32 update go version in go.mod
3e893c425b7cbcbcbac2afa97e4bb40a5547a882 Merge pull request #50 from rajatjindal/update-copyright
48753ba6b0ac96821a6ca6cacbcff415d94412d4 allow user to override kms endpoint
0d7f09ac3e39641ec6dffad66ae432ddad3ac95f Merge pull request #49 from rajatjindal/use-vendor
ffa7fc7f5c66dfbbdec1c438b1f6e463e8d9defb update go version in travis config
67e87bb971447beeab2f5c791fb191b1008ad4e2 update copyright year to 2020
8b1f7df232e5601eb70bf72658f067f48772f8d7 use vendor directory to build
d88a1ee02614afea516d19fd60ab1bcfb058371c update go version
fa467e978cb699aa09dec37f210bb8d0648127b4 Merge pull request #38 from vvbogdanov87/fix-kops-doc
89e1097a9e511c997c7f076758ae4194c926a74a Fix kops docs remove imagePullPolicy and tolerations
b279a11c11779a7be334a3d232659f68885319e6 Fix specs
cc11fdcce05195078d377e24127bbe56a09aaf1f Merge pull request #41 from kasured/doc/encryption-provider-config-flag
9cf3dfc928ee27d061fd51a53297c2e3112d3ee1 Fixes wrong name of the kube-apiserver flag
93b557b9c7fe44192b5665ed6c09341bd3b51297 Merge pull request #42 from micahhausler/module-pinning
df3090c2038acbede4a1e67a7beb209e739c492f Updated vendored modules
8962e22f3fd6fd9eb9e1243d86a894ffb62eb533 Pinned more modules
c99f1eed40b9e1d87a65a52cf15a6e6d73bd5a94 Merge pull request #37 from micahhausler/badge-fix
27a673666c16fc5adfe48e95c98a5e865ff40a07 Fixed build badge
fd4e308954e9a3e7f52bcb26bc0a9d21bfb756bf Merge pull request #35 from micahhausler/aws-sdk-go-bump
917b3c6e3a8b00ac2b6f9e33e6021758c25ae8d5 Updated aws-sdk-go to v1.23.11
94605f99769197c6dc1915d8e0a978547c62aef4 Merge pull request #34 from micahhausler/vendor-commit
5595bd6a222644141373726b49c27d5394d94d01 Added vendor folder
3bbfed049948a5c21fb6ef5d6ed05e81be7ac8df Merge pull request #33 from micahhausler/pkg-path-update
7281053211ad2955aaa2ba700ea1d0d0a05e247c Merge pull request #31 from rajatjindal/add-duration
3d7981554a0f7e94b2a52057969e94b481828e61 add latency metrics
20fe4a294bd8e73ede624f6da0f5d34823d90d2b Renamed go import path
04fbc46feabbbeabd3e6913cf9e50520d9d14448 Merge pull request #30 from TajMahPaul/add-additional-docs-kops
0468159167c0c5f7b7179666e4ed45cbb6debb65 Issue#29: Added additional docs for kops bootstrap
315f12f61b650e624877464d2ab2a676be5d1700 Merge pull request #20 from rajatjindal/update-readme
eaca32b95a89b8bb15d002aa5e14c094629ab895 Merge pull request #23 from rajatjindal/add-metrics
8bfde4f32b18d9687cc5bc7d85d3d94819e8da58 add very basic metrics
8fec0a87d1fac9bae76d679b573ad95e5e30f4e1 update documentation for bootstrap cluster time requirements
d5d7ff20016f9212b558d4456c317098e3aac50c Merge pull request #21 from rajatjindal/fix-dockerfile
9fcf14ab4ddf582662eb2d096876a7fcf9a93286 enable gomodules to fix docker image creation
a5cafb03873d2cbf286a3b4c9162d77787644cec Merge pull request #19 from jvassev/use-alias
bd0fa691703267ec6650764cac45d7a1eff6ad02 Use the key alias in README
b5aa5366c8d9b35617aa7909973a9080a39c38a2 Merge pull request #17 from micahhausler/docs
dfe02f2650c5a785904cc496be94a30252b6c47f Added user guide to README
9095cc91a35d639d793064686489c3c482308a5c Merge pull request #16 from micahhausler/security-contacts
645c9e5645cd556695744f4cc4eaf67ab9a382c0 Updated security contacts
a2ba8c6713610d08993f6651336cb2ab5c94c653 Merge pull request #15 from micahhausler/godoc
6d6025f47a26b8b0c2a2e6a4cfad974406fa98e9 Added godoc comments
99527cb24c9142cdc1d55650b31d0a0a210806b9 Merge pull request #12 from sethpollack/flaky_tests
d365cce669724ac71d3772551c80f069fb416a93 add KeyManagementServiceServer type assertion
5c31345be7b726d64cbbd716eea1269aa9f042a4 Merge pull request #14 from micahhausler/micahhausler-maintainer
1ec081dbd0a8fcbe33864124a73f906f82c7587d Added micahhausler as maintainer
37cb120b551844687e2a94ae375200ab0a167416 fix flaky tests
19d360e2a8b9641a25ad3ce45d12df75e41a9f0d Merge pull request #10 from dsexton/feature/linting
778ed119e2e66b7001186d4d3b600b920dd61082 Merge pull request #11 from micahhausler/updates
61496c032f791f61d6fc39fa846aff079da7f8ae Updated Go, AWS SDK, added go modules, moved code to pkg
1ffddb91ff44bff7dd077f5ad92d59bc308403e6 Fixed linter warnings
9d28416e9d992b382b29d33156cc2fc91b6634b9 Added lint target
a29167c58a3a1cf98b9b18611c27a873abe54658 Merge pull request #8 from sethpollack/master
4e093479b1fa75fda6b1ed1b5587dfb141d48b4b update owners file
7f6b7464ca5f6ea1d7c1cf3d77df80a2c2eaff53 Merge pull request #5 from sethpollack/security_contacts
b200926968cd6c71d57b3280b51dd35e8048b04d Merge pull request #3 from sethpollack/updates
a637a350946c649de6eb94ffb3ea40e8b8dc2d94 add SECURITY_CONTACTS file
18162c63eb0b265e60d1ee5f78ff7bf33813680e add StorageVersion
3e5fc9b1512334e6a40306249948643fa9fb9bce add link to docs
9c02fd17ac19d0e899b6e00bc7448751ad8f4e3a set CredentialsChainVerboseErrors
de64e295f45a6efa3197f2bfc444e10954cfc0d6 update defaults
1dd80022c1910f4de84b6d4f19eb9bed4fd03615 Merge pull request #2 from sethpollack/imports
235a76c10de202511e709e3bf4421b20d1f4bbc0 update imports
6dabbcd0af8bde5f0a8c939f7a3bcf867344a9f4 Merge pull request #1 from sethpollack/init
f881fb5fabbf05338f906e4e075e052998998bee refactor and add healthcheck
5b04d7ca87c1acce2a64934efb65c177b9a214b3 init
a3a1798f53d5d6c4396cf2392130be1d3d45418f Merge pull request #14 from spiffxp/rm-incubator-wording
c7a74bf55d0a03627783ffeb9d1dc06d3a8321fe Remove incubator content, touchup existing requirements
f6fc3f39b8e6e244cdc57077e2548ea2d3f9d23a Merge pull request #13 from spiffxp/use-kubernetes-community-coc
1f2f089f4df94a573ecdd00609a8174f6697905d Use git.k8s.io uri
e92bceda18cc411425c329a3ee84468b19831b83 Use kubernetes/community as source of truth for code of conduct
6eec07f1947ea0f4d9af1c947e09d1e29c468453 Merge pull request #12 from dankohn/patch-1
c16b58564af18f8554a0065e2a37c21d3d58d66a Change code-of-conduct to call by reference
27ddd7d5dfbd390208793a70796d7d75eec8adf8 Merge pull request #5 from mbssaiakhil/patch-1
3885f042bc7460ee4afed532a327b790cf95b1a5 Merge pull request #6 from krishna-mk/patch-1
e56f3814c2184bcb42a3226d95852ca62bff752f Merge pull request #7 from munnerz/patch-1
1a92ed9c6ea4d8bc8e03842f1815122e2704be83 Fix typo
d886dc7d6788ec0fe27cb5334b981534159f6c59 Add steering-committe as approvers for this repo
b5f61105b43dfb341faf38b85b06c5d6988a4d44 They are effectively the same, assignees is deprecated
baccff40abdfd3b8acb698c3c13d51915aa8fb47 Set correct project start date
0a62c067a72dac65d612dc4df4c80fc5cdf3de80 Update README.md
96e590562928ee9b25a32df8ec9d25330148b130 Fix typo
f8a2f3a870eb9bebfc06bcc204a2759ed30d972a Merge pull request #4 from mbohlool/patch-2
c50561e797f8080fb031fc5ac1081e7a7a8aafa5 Update CONTRIBUTING.md with CNCF CLAs link
98749d6b8efc612fe05d1bc42b0e0bff89f30e0a code-of-conduct: provide concrete points of contact
7bbf806ba23a838b07b12668e902bb73f0172815 Merge pull request #1 from philips/incubator-boilerplate
96198ace5ec9e558ff0b61642758389268b28d87 README: add some incubator boilerplate
25ead97bebdff65bfc177908ac79d4f00dd90bb6 Initial commit
```

Status: Fast-forwarded successfully.
