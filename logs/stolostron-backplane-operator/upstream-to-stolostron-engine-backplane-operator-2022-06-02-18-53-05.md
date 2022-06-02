## Fast foarding of stolostron/backplane-operator into stolostron-engine/backplane-operator.

## Status Summary:

backplane-2.1 -> backplane-2.1: First run, created backplane-2.1.  
backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  
main -> main: First run, created main.  

### Branch backplane-2.1 -> backplane-2.1:

New commits (first branch sync):

```
691c802a8c41cff91360f89c70e2f6fdb4ad42f9 Add HostedCluster and NodePool CRD's. This is so ServiceDelivery can use the ObjectRef capability! (#203)
1f3cbd21905e0bb5e468e59e92b26f269dd69f61 Update hypershift deployment crd (#198)
37a586c8d7d1b9f310853522d84c3994c3644a4e Add HostedCluster and NodePool obj references (#197)
6154ba205c861a8d0ff1b2ffddf84980a966f36e Add permission for nmstateconfigs for agent-install.openshift.io (#194)
732d4774dfbf578a881314745c6a773a1ce86d22 Regenerate Charts using inclusion (#195)
bfc7ea3545e705aae0851fd854618b8b6bb076ad adding conditional addition of global pull secret to EDIT environment variable (#191)
5fe67dcc6000fdf63396138c4492c93be1e50fea [create-pull-request] automated change (#192)
d6b404b9af987856caad911b679226ad478f234d add test for service monitor deletion (#190)
abc2f33f726d10909fcb2d9834f67be193357788 Update README.md (#189)
0a64096ab7c8249b73af574233f6330b01d20470 Picking up latest CRD from hypershift-deployment-controller. (#188)
ea9b9d1cef7ee2ac1c42109b093a6d64f5fb414d [create-pull-request] automated change (#187)
9d04f2dd496644ba9ecdad45110529fe2e89f2a0 [create-pull-request] automated change (#185)
b40cb45a6d98de1eaffee954029b29b75ba758bf watch servicemonitor resource (#186)
72c48e9060f1001b7d522298383c328a413b1b75 Add image override configmap support (#182)
134a9845a130dd644e13cccc9c7624a495354b89 Enable mce plugin when console is toggled on (#184)
975787031c10847bf01148d5efe3d3f8ea329e61 Add rbac requirements for consolequickstarts resource (#183)
4900dfc3eb9243069e89c268d6ae501be6e75e62 Create Quick Start for multicluster switcher (#151)
94f1f5b57a61717842513767c912cbbb5be5a8c8 Add managedclusteraddon deletecollection permission for import controller (#181)
9c46ea716bfecc1147215c8402b477a554da8892 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 99cfc43a28bd758a66bcfe195d48099746fbb212 Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/2204100020
1c8c5107b5c43a89745af46631825ac077a25653 update rbac of import-controller to fix 21838 (#180)
338f2df9aad2327be11a51dc91a78b0c13ad179d update command of cluster curator (#179)
5949b5c12a636829c5c97187b6bee7cbfaa02e12 update imageregistry crd to fix issue 21706 (#178)
ca312ef6349ed526650d9a7d019eb141942f9b48 [create-pull-request] automated change (#177)
a83ff2c0515cb3f72dfb50f66dfa86958f3341a6 Add support for spec.serviceAccountSigningKey. Issue 21690 (#176)
2bb312245a9eba5cfa958b2e24112ecb0062ac81 Apply new HypershiftDeployment printcolumns (#175)
7efd11035f30910b468a7b139eb734fae7b3284a New objectRef, resulted from final hypershift:release-4.10 vendoring (#174)
6336a083e89cba74ab71f769a57d80dcecf7ae2a add update rbac for managed cluster (#173)
ca4362ea1090f77b7e79171febb280b6126a402f Name ManagedServiceAccount as preview (#172)
0113ca8bf7b438b9ca769fe74f6cc6badac56abc [create-pull-request] automated change (#171)
cb4ed767befd4c1cada8ec44f2e2e1233460e9c2 update the renamed fields (#170)
9b2bc4b05643486efd173dd8b3d2f88c09eebcb9 [create-pull-request] automated change (#169)
90fe6c4039aa8fef7db45a04667f41b7e868b498 Update README.md (#168)
cffe77ecc61b941f4c17dbde7162065fd51a4f9e add lease permission (#167)
42600ee516c35d1370ae0b9a37a106bc17cbbb93 Added missing HOSTING print column for HypershiftDeployment (#166)
fdf13e3fab40ec88cdb6415c19ab658652dbb8ff [create-pull-request] automated change (#164)
d858822c201cd6266e42555cae6ea2cd3da60ab9 add lease rbac for work-manger addon agent in ocp 311 case (#165)
213a98649ee80c40ada3e292be7ea5fe969c4eea Rename ConfigMap (#163)
9645c89a35a85810f4a19ce3882d688e98a05223 Add new printer column and update CRD with hypershift:release-4.10 (#162)
1ff5135ec15327c4e7f32110ef687d5970ac9d84 Change ReplicaCount to 1 (#159)
d8a4b60659af10b8d13b1b7e512a4ae1520f5fad Add static override to change assisted installer namespace (#158)
d63200de8a69ee75826cda6e1eeb805765779e1a Proceed with deploying other components if one fails (#157)
1004517ed3a755a32102c0bd4ae2257c6b474672 Fix hypershift yaml format error and render test (#156)
34cc6eae651aad131d623b4bd1fba9d600b3d94e Collapse repeat components in spec to one (#154)
284d5522fac0cf53a540fe3e4fbdf3095d73cdde [create-pull-request] automated change (#155)
c68bddac39d8d244181cefaf314e9fa6373346ee [create-pull-request] automated change (#153)
4e504c321adf0fa2c5665c6684562e7aea1825ff Require no AgentServiceConfigs to delete MCE (#152)
dc667ed11a0287479606042e27c8fdc738de7384 No-op (#150)
49692834676c21874d8760dcddd6188ef5a9f828 Onboard HyperShift Configmap (#149)
6458171446ec1eccb1c7eadb0b0d7de686eee264 Add subscription.operators.coreos.com to console-clusterrole (#148)
9285bfd96d97ae15674e0a1de754682c7058c175 Merge pull request #147 from stolostron/zkayyali812-patch-1
bcc8cbf1f21352d002337e0878d3c8bda09a91a0 No-op
d295c8603bd90f1864490b72519aaff8321e4ebf Ensure ReplicaCount of 1 (#146)
363b1102077954c8287635da49b9c68dc4b9c1e0 Move component list to overrides and remove restrictions (#145)
dd14a1ec3f5058f84631b40955a55ca36d7c0137 Ensures bundled CSV is up to date (#144)
1fe7ddbb5923e12444402f620fd9ac517387c3b0 Merge pull request #142 from stolostron/zkayyali812-patch-1
edac57d9fcb93238f198c17145b5589c6f3ba60d No-op
474d5a3f4944b2d7df402c40b1a7dc426aa9331d Onboard Hypershift (#126)
c00a2425ba6aec046f8284b58d84f9f72de4e3d6 Pin Hive to mce-2.0 (#141)
90a2586264f5b91c0bc205d91ba3cf17fbe6906c Merge pull request #140 from stolostron/zkayyali812-patch-1
9b51ab7117495769c368ab9812c265875649edbd no-op
c9de7c4b74ee5d1ad212ffdb741d1ccb34a814f0 [create-pull-request] automated change (#139)
1bedc45e5991f3ee3c31c026a8faa683b3f6c643 Allow console-mce to be toggled off in 4.10 (#138)
b44481feae429ecffd0936effbec307d1dc88ea7 [create-pull-request] automated change (#137)
529ad00f36b37b53bc4395915c52ede27accd698 removing clusterrole and binding tests, updating cr & b naming to not duplicate (#136)
aa4da6ecdcbcf7b9d30ba97b5fa1174e77357fdd Add cluster-proxy-addon CRD (#133)
4e8e44fc39882f3a2e3c2b607c4a3b2b4104c11f [create-pull-request] automated change (#134)
3b54f8fcd343bc93205f2d8acb58bb61603bee74 update rbac for addonplacementscores and import controller (#132)
325c8f165fd5c88d0eb7c2cb95ba153ce46915bd updating script to run with python3 (#130)
5f4a84d0283c6fc7320e4025d6f64d245fbc9af7 redoing chart link to use https instead of ssh (#129)
61aa4ffe1f1f16f7571842bdca4f79c7cfe65b75 Chart polling (managed service account) (#128)
256a58ce391e2a349b323cdbef7681a0b458196f update go dependencies (#127)
6d734f2a290d48ce31c6154ae72db13b4e1c8f0c [create-pull-request] automated change (#122)
9bb3bd740f546fbdf1e8645d647b8d32c1b99153 Correct official MCE component name (#125)
85fb406de76b4c019d2668055d86d11700bad424 Allow components to be toggled on or off (#124)
63b46e9d23546e1f0a42930f792bec1e4ac1d459 adding agg roles for managed serviceaccount (#121)
e7d01d81b6f41f8f68a8c5bca93a6c5326994b7f Add PlacementDecisions to console-clusterrole (#123)
326edc0bcc7d6151e343463fb990c37c082ecc78 Latest Operator Bundle Updates (#119)
497e60f6f4da324e4a1cbe4da68982eb9ce390a9 Onboard Console-MCE (#118)
fdefc0f6529fca1b755de01d84b72e322c0461f0 Onboard AI to MCE (#112)
54b9b4b15be143c9fccd3f5fa08c9215bfe5c703 [create-pull-request] automated change (#117)
37603a75abe1a8c04aca20e00c2e8e6c97a8fef0 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - fcf3027d804c0f36e1b85a3fa1aec27dd184f46e Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1882088305
ff5c849da4c1078a7719c8c23e0df2597b825a60 set default targetNamespace to multicluster-engine (#116)
423e889a570f51bde991152f4193f1842814d9a8 Merge pull request #115 from zkayyali812/fix-sample
01cf6c79160ca72bf92e989ba50cbf21601dd505 Fix Sample
5c0202582466ed67c0b7681d35981c3ff21c138a Refactor License test (#114)
2ac44649a63c1d37c5cbe33d60aa01923e205339 match clc-state-metrics ClusterRoleBinding to correct ClusterRole (#113)
92f2afb9301a019928958b461a7e8b81b0478e33 No-op (#111)
c6057493924d093bbc0f78c80acfcd8b5cb9d987 Automate Discovery (#108)
308c7cb1fb147e52624b7639523f8292ec64e562 update foundation clusterrole (#109)
62d32258f05898aeead5a84c090cf520eab5c845 Nweather managed serviceaccount support (#4) (#105)
051c8ee1dbbb257a68b0cecb4e71a6855d686f1e  Canary fix (#107)
8eeb800764f27cfaea95c522b9f21141e297764d Update Discovery CRDs (#106)
3d616c4417369f15ded7b58db9c081a6589c64e1 add discovery (#96)
90bc805dc42e4802c9e33906943182c5265b83f1 Add arm64 for MCE (#104)
55de156c0cae55dfdb3d8e39a1a0a7f6f0318991 Update README.md
6674a04b150573a1e3aecdf928b2349577d95e43 Onboard CLC (#100)
3b0826089509d912c3f41680d1f81c0b18323618 Update registration bundle automation (#101)
cd134b9c29003543bc0150b28e2b02f2356f5492 Configure webhook for mce v1 (#99)
5d702a49d2cd326da899a572e4b44ccd64bb1da7 No-op PR (#95)
66e2ad2fa49bf7e378460833b0757a60ae2f64fb No-op PR (#94)
1603260fa040656178e079df77d15cb92af80efc Update to v1 (#93)
9704892826b5bf9ea20b12c94663681512e02971  add back pod namespace (#92)
b41bfae5a5e3292e6b1fa03b6a0a0b60fddbd593 change default image pull policy to always and add override (#91)
cc86c9e0d2b1e2a7d0fd105fea8858f20b433db8 [create-pull-request] automated change (#86)
22ac530acb53c04ea71c75cb6ce678a94fb6f3d6 Label adopted subcomponents (#88)
e2d4aefe0abd5f55f8a6219dd2628cfa6c00b759  add availability configuration (#87)
803834a696b7bad29e76d7d45dd4fc38af74113b Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 9edbc5ff4293a0d1c46fb56c7bd719a3b1cb44cf Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1684452233
41d9d602b5123f33462a3424ec9a15a069ee245f rename update (#84)
9232af7f64d5bb1a6f17793a805f90315b63937c Update functional test suite (#83)
f08a30f1074d73530b619cafb0ed7804c17f1dcf Allow installation with existing MCH (#82)
013a778a07aa1aad3472ffae84064dd83fb80f88 Update COMPONENT_VERSION to 2.0.0 (#81)
29fb30d35688408afff802f91f636a70f9c6d7b6 No-op change (#80)
c6ba0a203b87a1dcc74a66f79070757545f9f256 Adds OCM webhook definitions (#79)
369e6f836a615380df1cecdb6ed038f25e80f00e Manual manifests refresh (#78)
a0b4faa612f5bd60277fc03badff1384c9e8674a [create-pull-request] automated change (#77)
0ba0fea0723a3dd176855c3b1752990095f2bb56 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 425b5ba413fafae825a735c0511dbb36691ecf41 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1346958202
be8277514e763926e215fe9504ddbe1c60550020 Install ClusterManagementAddon (#76)
1511a69bfc4fe6288f9b51a216fc0f25093828ca  bundle fix (#75)
2b9c6f8131358319e0df80c701d80b965a0ba4cb Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 8381b82c22103d820d16b5d4eae53d98f6c365ed Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1317639471
765505d4924d65b64f1d7d53846b7350fc0d01bd Prepare global (#73)
a949ac2eb161933e0dbf197c66ad95ccc563166a Remove MCO from MCE Webhook (#72)
c92dda938a1cae7898405796df945daab0dc1723 Track UID in status manager (#71)
bf9af1eb748e5fab7b8e48ce87ab8dc399c765ff Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 717a30350c872334abfea1dc39f85de6b9848c3b Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1309498819
aebfb3ba8ce771aa78f5d76da647cfde8acab5fa [create-pull-request] automated change (#70)
e516a298c7b95fe3e574991ceede8f14fa28694d  add default tolerations to the cluster manager resource (#67)
463bea09c2d144057b33f17d1e8a6f8eca98a11b Operator Bundle Update (#66)
2718b17653c4e899982f32d2fd85e773bedd3d36 Annotations (#64)
91c6b57ac0df3eaeeb378d5f8b0cb5cb0863e7e3 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ff366feb12c4bc67a39541e6c9d75cabe521edbf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1285727449
b9681bdbb6cad525c3ef605389d54d67e0fb21e1 Report status while mce uninstalls (#62)
f0dc7d3d12f5272536a31a0580986246e4643867 Update managedclusterimport controller RBAC (#61)
de757769be40d6e11863fed21008c059552f5374 Operator Bundle Update (#60)
586c90c63ebb1c6f9208eb93ec095da166dbf6f8 Fetch images from backplane pipeline (#59)
5a040f639c2f74519683cd3db9a35388f9496d8d Install foundation agent automatically (#56)
5e132032b4e1adc5e7ac5bc638889bdba1fafcf2 Mods (#58)
ad2642b6a675baa7c9aa8d9d1648ff13f5335a9f Remove unused code (#57)
8e2aa7caa097f40d0a0d02aec100586f79a9bee4 Refactor reconciler (#53)
eee5f5f9e6cb0512f66a68bc70e5a57034046484 Update .gitignore (#55)
2319a0cd3ca5d453401f291d9177c333c99ee8db Lint Operator Bundles (#52)
4b258cfff1fab2df325fc708e8cd2d2e7b0c8ead Remove foo field from CRD (#51)
1694fa6ff28ee1de18bea397ef3ca4ae658faf58 15635 Automation to update templates (#50)
32c61535143c588a38857a19c40a807676b513eb Update Go and modules (#48)
5ededbae8649e84ddd6a34f12f0445afe138907e Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 5e9ebe1c9a97c21817701a5aa04185ad1bf4229d Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1242267934
eedff1f9c3ad5231083faf93ed16530f754515b1 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - f7d413a5804f0506d4324334170a339e4ff13856 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1240134327
24395f26ad8b5c4f44cb99c9e5e3d6776dc3c6c7 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 4a913e3222c708c33eebddf9be9f41345501bebf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1235193835
77e35de24c03b44d01352f84d47e2164ceea9ce2 onboard managedclusterimport-controller (#47)
1c9da1f0d21e2bbdf56734b0472705a90b8a8391 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 0867b07d045c305e26d8d2bc5bd66f10e8b6255f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1221968356
ad265f1a885d53747e603e1c4d784d61e8a9405d update cluster manager (#45)
31de3d0a847e04efe23f878e8dc4b4248c63c041 Use ownerreferences to handle cleanup (#46)
75fde901382e61da1e4b4192368700802a33e43e Add role to backplane (#44)
8055fbca7e8e6e86447deed72b6cfbd4a6d96cbf Use server-side apply to deploy (#41)
f3353ad40e54181031846f4a907cd1ae014380a9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ae67ba475e56280ba24cf1d77ec462f918f538b8 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1213388914
bb14c4ef9d81dbdb9be7edda8c525fc63e9a7a49 14976 proxy configs (#40)
37cee07444f3a7b95740a6a0d02c7dabe48e18ac  propagate proxy variables (#39)
57780768a70134f63e0eb23b38dc3e80b54e5aac  add toleration to spec (#38)
919deafd1216961cd6d69b5ebb21ff33fab39130 add image pull secret (#37)
59f388f455dc6d82476dbf2342056190cd4ef352 Watch subcomponents (#36)
b7c927600d0979ef185bef42ba4607ada9a4a596 14869 spec node selector (#34)
87dd0a0c93937eea680d4d336c12111bfbd1c99b rename csv to multicluster-engine (#35)
fdbfd10d2448619101b2dadd03589f5869ad2265 add clusterpool/claim permission in cluster admin (#32)
0756a71641dda98b1f2fe47b50ca7556f3eba6ad 15632-multiclusterengine-rename (#33)
d335d09863c117681a54625a479075e6ab0e8816 Expand Webhook Logic (#31)
a924b5ef358267bdd75815dd94e19c373d41c962 fix the different labels of ocm deployment and service (#30)
79761f7b3f050d6652abc54c4d04424fee382ecb Update clusterrole-foundation.yaml (#29)
20851b4a48e422657229cfe3eb9b40dc2c36f737 Update foundation roles (#28)
feb5e9779192a0f0ba159c7b7d994d3dd1fab937 auto-update-crds (#27)
e8b53c49d498d7b703e40803b478a515c62a2dfd Expand status (#25)
2a195e0ba85cb44c86a9e288f449e78c540de57f change config scope and related code (#24)
5d07faf017a20e0aa74088629869b18c38f60858 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 17bbf4a5958ba90a8be9200b0a97dec2b7d091a4 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1166508714
bb49db228d703c20ef3702ecfd21df6710dc0532 update channel (#23)
a96db35ae342ce17843989eabe1471a9bd1f58d0 Install Clustermanager and Hive Operator bundles (#22)
a29c95aff842e5cdea417884d28baba9dccc2caa Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 7f9ddf9af3aeb71003159083885592db73c7d66f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1158084680
8f7ee173f61c0ef7a0b18a36ce96f1e74e03187c Quick fix (#21)
afdda4a9e5d29f7eaf202a9c72f2e4fa7458cb44 Redesign server foundation installation (#19)
5e1e2ee441da387167d7255f36be3fd6223b3cfd 14546 installation guidance (#18)
b161e12e234343c44db22f44d458e44aeacfe0bf adding basic functional tests (#17)
f2aae328e7dae5fae38a3b03ef06c944f7ffd1c0  add files (#16)
8a055a298df3c4dd9798688ddd72c21657e2cf1c  fix image and sonar tests (#14)
638614610e5427f137ebf8a7fc82df8e092f89c6 Merge pull request #12 from zkayyali812/14710-webhook
7c038906069f4df146fe12edbbeae0063e202e5f Refactor Validatingwebhook
c0bfdf1deebb96ee26b4d1e86308ffb68603d9bc Run locally
a9abea9413a99c107eabf285164bf4e7967a51da Enable ValidatingWebhookConfiguration
796e3a8068e50319673fe479c8e43eeba72ce86c Merge pull request #11 from cameronmwall/setup-prow
47bb77ea5d1c153743689c7fd6a4767d6cbc8af4 setup prow
760d560cd23691dc7f632a143ff5deda590579e9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/main Chart SHA - 1e5712716d56b1641e7e28406d0a31b70b83486e Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1090944233
93d1454cfc4da589cfdd35e3c6d4e4ec0c5bf939 Merge pull request #10 from JakobGray/crd-auto-update
241d894b3b03005a67c5eb4036e0983e272abc63 Auto update CRDs from the hub-crds repo
5f2de4d6916e912cb882f56807b13039ebc3f2f2 Merge pull request #9 from zkayyali812/14711-add-finalizer-logic
c78b21e501b9e0b76972327d6c77d40c50909add Unit tests
a1a05dc180fcaa165275fa3b3a91f960bfec7d1c Merge branch 'main' of github.com:open-cluster-management/backplane-operator into 14711-add-finalizer-logic
fb6d52dccf5b315bb7c0640d90e7b23bb7118d69 Add Finalization Logic
03685c56181a5df4958d1c0c619e7b892c331f3e Merge pull request #8 from JakobGray/status
1073f32371b70cda733d61b545fbcb5022848b8f Add phase status to api
b7c901296d1fb06c83700fea5126bd0b992eb1a6 Merge pull request #7 from zkayyali812/14549-server-foundation
13d5a536482eda83cc2eb5e977177e9e8b627ea4 Add descriptions and update license test
9bc57fd1ce9e35eaffd5a12b1db081771cbed6d6 Install Server Foundation Components
47ee4a59cefb1841dcfb5c2b9fa3909d00d583aa Merge pull request #6 from open-cluster-management/JakobGray-patch-1
64f79176127069ac45f765f0c7f78f775cf83ab0 Update README.md
0108861937c167c4627082d35e01c3035bc7c597 Merge pull request #5 from JakobGray/license
00bd8dd658ad83358edc6940405c6160e0c3fcca Add files for contributing
2d320b259c3bc0b630fa46903e80c1db3c8d56ed Add OWNERS file for openshift-ci
68297ea458a022de70e4562a08f5ce94a9b4bcd4 Add Open Cluster Management license header and check
3ec3d4283b180895bcd6965a2d94a5d64ac3fa58 Merge pull request #4 from open-cluster-management/backplane-operator-mark1
777e9fbe1372f1ed5c6003d81c7e59344f21205c Add Hive RBAC
fd8817da9500c80e2d6ce47437da91100a2e4ecb Rebundle
79779c8384eccca583bbc63c5c8e02e6d7558b91 Add Unit Tests
abbfb2b3a79614434833ed0dfd42aaf33b7c51e9 Backplane-Operator Mark v1
339cddd2b48a1b2f681466179aae5b7add3300e9 Remove metrics mservice from bundle manifest (#2)
da69d07c831ec077eea219181acff3bf38cd25a5 Generate OLM bundle (#1)
278b7ef3037cad60f129d7353d30cd36e5563df1 Initial commit
```

Status: Fast-forwarded successfully.

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
49d8211c07f3a9014a1c18645bdc5783385e222e Update hypershift deployment crd (#199)
37a586c8d7d1b9f310853522d84c3994c3644a4e Add HostedCluster and NodePool obj references (#197)
6154ba205c861a8d0ff1b2ffddf84980a966f36e Add permission for nmstateconfigs for agent-install.openshift.io (#194)
732d4774dfbf578a881314745c6a773a1ce86d22 Regenerate Charts using inclusion (#195)
bfc7ea3545e705aae0851fd854618b8b6bb076ad adding conditional addition of global pull secret to EDIT environment variable (#191)
5fe67dcc6000fdf63396138c4492c93be1e50fea [create-pull-request] automated change (#192)
d6b404b9af987856caad911b679226ad478f234d add test for service monitor deletion (#190)
abc2f33f726d10909fcb2d9834f67be193357788 Update README.md (#189)
0a64096ab7c8249b73af574233f6330b01d20470 Picking up latest CRD from hypershift-deployment-controller. (#188)
ea9b9d1cef7ee2ac1c42109b093a6d64f5fb414d [create-pull-request] automated change (#187)
9d04f2dd496644ba9ecdad45110529fe2e89f2a0 [create-pull-request] automated change (#185)
b40cb45a6d98de1eaffee954029b29b75ba758bf watch servicemonitor resource (#186)
72c48e9060f1001b7d522298383c328a413b1b75 Add image override configmap support (#182)
134a9845a130dd644e13cccc9c7624a495354b89 Enable mce plugin when console is toggled on (#184)
975787031c10847bf01148d5efe3d3f8ea329e61 Add rbac requirements for consolequickstarts resource (#183)
4900dfc3eb9243069e89c268d6ae501be6e75e62 Create Quick Start for multicluster switcher (#151)
94f1f5b57a61717842513767c912cbbb5be5a8c8 Add managedclusteraddon deletecollection permission for import controller (#181)
9c46ea716bfecc1147215c8402b477a554da8892 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 99cfc43a28bd758a66bcfe195d48099746fbb212 Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/2204100020
1c8c5107b5c43a89745af46631825ac077a25653 update rbac of import-controller to fix 21838 (#180)
338f2df9aad2327be11a51dc91a78b0c13ad179d update command of cluster curator (#179)
5949b5c12a636829c5c97187b6bee7cbfaa02e12 update imageregistry crd to fix issue 21706 (#178)
ca312ef6349ed526650d9a7d019eb141942f9b48 [create-pull-request] automated change (#177)
a83ff2c0515cb3f72dfb50f66dfa86958f3341a6 Add support for spec.serviceAccountSigningKey. Issue 21690 (#176)
2bb312245a9eba5cfa958b2e24112ecb0062ac81 Apply new HypershiftDeployment printcolumns (#175)
7efd11035f30910b468a7b139eb734fae7b3284a New objectRef, resulted from final hypershift:release-4.10 vendoring (#174)
6336a083e89cba74ab71f769a57d80dcecf7ae2a add update rbac for managed cluster (#173)
ca4362ea1090f77b7e79171febb280b6126a402f Name ManagedServiceAccount as preview (#172)
0113ca8bf7b438b9ca769fe74f6cc6badac56abc [create-pull-request] automated change (#171)
cb4ed767befd4c1cada8ec44f2e2e1233460e9c2 update the renamed fields (#170)
9b2bc4b05643486efd173dd8b3d2f88c09eebcb9 [create-pull-request] automated change (#169)
90fe6c4039aa8fef7db45a04667f41b7e868b498 Update README.md (#168)
cffe77ecc61b941f4c17dbde7162065fd51a4f9e add lease permission (#167)
42600ee516c35d1370ae0b9a37a106bc17cbbb93 Added missing HOSTING print column for HypershiftDeployment (#166)
fdf13e3fab40ec88cdb6415c19ab658652dbb8ff [create-pull-request] automated change (#164)
d858822c201cd6266e42555cae6ea2cd3da60ab9 add lease rbac for work-manger addon agent in ocp 311 case (#165)
213a98649ee80c40ada3e292be7ea5fe969c4eea Rename ConfigMap (#163)
9645c89a35a85810f4a19ce3882d688e98a05223 Add new printer column and update CRD with hypershift:release-4.10 (#162)
1ff5135ec15327c4e7f32110ef687d5970ac9d84 Change ReplicaCount to 1 (#159)
d8a4b60659af10b8d13b1b7e512a4ae1520f5fad Add static override to change assisted installer namespace (#158)
d63200de8a69ee75826cda6e1eeb805765779e1a Proceed with deploying other components if one fails (#157)
1004517ed3a755a32102c0bd4ae2257c6b474672 Fix hypershift yaml format error and render test (#156)
34cc6eae651aad131d623b4bd1fba9d600b3d94e Collapse repeat components in spec to one (#154)
284d5522fac0cf53a540fe3e4fbdf3095d73cdde [create-pull-request] automated change (#155)
c68bddac39d8d244181cefaf314e9fa6373346ee [create-pull-request] automated change (#153)
4e504c321adf0fa2c5665c6684562e7aea1825ff Require no AgentServiceConfigs to delete MCE (#152)
dc667ed11a0287479606042e27c8fdc738de7384 No-op (#150)
49692834676c21874d8760dcddd6188ef5a9f828 Onboard HyperShift Configmap (#149)
6458171446ec1eccb1c7eadb0b0d7de686eee264 Add subscription.operators.coreos.com to console-clusterrole (#148)
9285bfd96d97ae15674e0a1de754682c7058c175 Merge pull request #147 from stolostron/zkayyali812-patch-1
bcc8cbf1f21352d002337e0878d3c8bda09a91a0 No-op
d295c8603bd90f1864490b72519aaff8321e4ebf Ensure ReplicaCount of 1 (#146)
363b1102077954c8287635da49b9c68dc4b9c1e0 Move component list to overrides and remove restrictions (#145)
dd14a1ec3f5058f84631b40955a55ca36d7c0137 Ensures bundled CSV is up to date (#144)
1fe7ddbb5923e12444402f620fd9ac517387c3b0 Merge pull request #142 from stolostron/zkayyali812-patch-1
edac57d9fcb93238f198c17145b5589c6f3ba60d No-op
474d5a3f4944b2d7df402c40b1a7dc426aa9331d Onboard Hypershift (#126)
c00a2425ba6aec046f8284b58d84f9f72de4e3d6 Pin Hive to mce-2.0 (#141)
90a2586264f5b91c0bc205d91ba3cf17fbe6906c Merge pull request #140 from stolostron/zkayyali812-patch-1
9b51ab7117495769c368ab9812c265875649edbd no-op
c9de7c4b74ee5d1ad212ffdb741d1ccb34a814f0 [create-pull-request] automated change (#139)
1bedc45e5991f3ee3c31c026a8faa683b3f6c643 Allow console-mce to be toggled off in 4.10 (#138)
b44481feae429ecffd0936effbec307d1dc88ea7 [create-pull-request] automated change (#137)
529ad00f36b37b53bc4395915c52ede27accd698 removing clusterrole and binding tests, updating cr & b naming to not duplicate (#136)
aa4da6ecdcbcf7b9d30ba97b5fa1174e77357fdd Add cluster-proxy-addon CRD (#133)
4e8e44fc39882f3a2e3c2b607c4a3b2b4104c11f [create-pull-request] automated change (#134)
3b54f8fcd343bc93205f2d8acb58bb61603bee74 update rbac for addonplacementscores and import controller (#132)
325c8f165fd5c88d0eb7c2cb95ba153ce46915bd updating script to run with python3 (#130)
5f4a84d0283c6fc7320e4025d6f64d245fbc9af7 redoing chart link to use https instead of ssh (#129)
61aa4ffe1f1f16f7571842bdca4f79c7cfe65b75 Chart polling (managed service account) (#128)
256a58ce391e2a349b323cdbef7681a0b458196f update go dependencies (#127)
6d734f2a290d48ce31c6154ae72db13b4e1c8f0c [create-pull-request] automated change (#122)
9bb3bd740f546fbdf1e8645d647b8d32c1b99153 Correct official MCE component name (#125)
85fb406de76b4c019d2668055d86d11700bad424 Allow components to be toggled on or off (#124)
63b46e9d23546e1f0a42930f792bec1e4ac1d459 adding agg roles for managed serviceaccount (#121)
e7d01d81b6f41f8f68a8c5bca93a6c5326994b7f Add PlacementDecisions to console-clusterrole (#123)
326edc0bcc7d6151e343463fb990c37c082ecc78 Latest Operator Bundle Updates (#119)
497e60f6f4da324e4a1cbe4da68982eb9ce390a9 Onboard Console-MCE (#118)
fdefc0f6529fca1b755de01d84b72e322c0461f0 Onboard AI to MCE (#112)
54b9b4b15be143c9fccd3f5fa08c9215bfe5c703 [create-pull-request] automated change (#117)
37603a75abe1a8c04aca20e00c2e8e6c97a8fef0 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - fcf3027d804c0f36e1b85a3fa1aec27dd184f46e Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1882088305
ff5c849da4c1078a7719c8c23e0df2597b825a60 set default targetNamespace to multicluster-engine (#116)
423e889a570f51bde991152f4193f1842814d9a8 Merge pull request #115 from zkayyali812/fix-sample
01cf6c79160ca72bf92e989ba50cbf21601dd505 Fix Sample
5c0202582466ed67c0b7681d35981c3ff21c138a Refactor License test (#114)
2ac44649a63c1d37c5cbe33d60aa01923e205339 match clc-state-metrics ClusterRoleBinding to correct ClusterRole (#113)
92f2afb9301a019928958b461a7e8b81b0478e33 No-op (#111)
c6057493924d093bbc0f78c80acfcd8b5cb9d987 Automate Discovery (#108)
308c7cb1fb147e52624b7639523f8292ec64e562 update foundation clusterrole (#109)
62d32258f05898aeead5a84c090cf520eab5c845 Nweather managed serviceaccount support (#4) (#105)
051c8ee1dbbb257a68b0cecb4e71a6855d686f1e  Canary fix (#107)
8eeb800764f27cfaea95c522b9f21141e297764d Update Discovery CRDs (#106)
3d616c4417369f15ded7b58db9c081a6589c64e1 add discovery (#96)
90bc805dc42e4802c9e33906943182c5265b83f1 Add arm64 for MCE (#104)
55de156c0cae55dfdb3d8e39a1a0a7f6f0318991 Update README.md
6674a04b150573a1e3aecdf928b2349577d95e43 Onboard CLC (#100)
3b0826089509d912c3f41680d1f81c0b18323618 Update registration bundle automation (#101)
cd134b9c29003543bc0150b28e2b02f2356f5492 Configure webhook for mce v1 (#99)
5d702a49d2cd326da899a572e4b44ccd64bb1da7 No-op PR (#95)
66e2ad2fa49bf7e378460833b0757a60ae2f64fb No-op PR (#94)
1603260fa040656178e079df77d15cb92af80efc Update to v1 (#93)
9704892826b5bf9ea20b12c94663681512e02971  add back pod namespace (#92)
b41bfae5a5e3292e6b1fa03b6a0a0b60fddbd593 change default image pull policy to always and add override (#91)
cc86c9e0d2b1e2a7d0fd105fea8858f20b433db8 [create-pull-request] automated change (#86)
22ac530acb53c04ea71c75cb6ce678a94fb6f3d6 Label adopted subcomponents (#88)
e2d4aefe0abd5f55f8a6219dd2628cfa6c00b759  add availability configuration (#87)
803834a696b7bad29e76d7d45dd4fc38af74113b Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 9edbc5ff4293a0d1c46fb56c7bd719a3b1cb44cf Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1684452233
41d9d602b5123f33462a3424ec9a15a069ee245f rename update (#84)
9232af7f64d5bb1a6f17793a805f90315b63937c Update functional test suite (#83)
f08a30f1074d73530b619cafb0ed7804c17f1dcf Allow installation with existing MCH (#82)
013a778a07aa1aad3472ffae84064dd83fb80f88 Update COMPONENT_VERSION to 2.0.0 (#81)
29fb30d35688408afff802f91f636a70f9c6d7b6 No-op change (#80)
c6ba0a203b87a1dcc74a66f79070757545f9f256 Adds OCM webhook definitions (#79)
369e6f836a615380df1cecdb6ed038f25e80f00e Manual manifests refresh (#78)
a0b4faa612f5bd60277fc03badff1384c9e8674a [create-pull-request] automated change (#77)
0ba0fea0723a3dd176855c3b1752990095f2bb56 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 425b5ba413fafae825a735c0511dbb36691ecf41 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1346958202
be8277514e763926e215fe9504ddbe1c60550020 Install ClusterManagementAddon (#76)
1511a69bfc4fe6288f9b51a216fc0f25093828ca  bundle fix (#75)
2b9c6f8131358319e0df80c701d80b965a0ba4cb Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 8381b82c22103d820d16b5d4eae53d98f6c365ed Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1317639471
765505d4924d65b64f1d7d53846b7350fc0d01bd Prepare global (#73)
a949ac2eb161933e0dbf197c66ad95ccc563166a Remove MCO from MCE Webhook (#72)
c92dda938a1cae7898405796df945daab0dc1723 Track UID in status manager (#71)
bf9af1eb748e5fab7b8e48ce87ab8dc399c765ff Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 717a30350c872334abfea1dc39f85de6b9848c3b Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1309498819
aebfb3ba8ce771aa78f5d76da647cfde8acab5fa [create-pull-request] automated change (#70)
e516a298c7b95fe3e574991ceede8f14fa28694d  add default tolerations to the cluster manager resource (#67)
463bea09c2d144057b33f17d1e8a6f8eca98a11b Operator Bundle Update (#66)
2718b17653c4e899982f32d2fd85e773bedd3d36 Annotations (#64)
91c6b57ac0df3eaeeb378d5f8b0cb5cb0863e7e3 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ff366feb12c4bc67a39541e6c9d75cabe521edbf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1285727449
b9681bdbb6cad525c3ef605389d54d67e0fb21e1 Report status while mce uninstalls (#62)
f0dc7d3d12f5272536a31a0580986246e4643867 Update managedclusterimport controller RBAC (#61)
de757769be40d6e11863fed21008c059552f5374 Operator Bundle Update (#60)
586c90c63ebb1c6f9208eb93ec095da166dbf6f8 Fetch images from backplane pipeline (#59)
5a040f639c2f74519683cd3db9a35388f9496d8d Install foundation agent automatically (#56)
5e132032b4e1adc5e7ac5bc638889bdba1fafcf2 Mods (#58)
ad2642b6a675baa7c9aa8d9d1648ff13f5335a9f Remove unused code (#57)
8e2aa7caa097f40d0a0d02aec100586f79a9bee4 Refactor reconciler (#53)
eee5f5f9e6cb0512f66a68bc70e5a57034046484 Update .gitignore (#55)
2319a0cd3ca5d453401f291d9177c333c99ee8db Lint Operator Bundles (#52)
4b258cfff1fab2df325fc708e8cd2d2e7b0c8ead Remove foo field from CRD (#51)
1694fa6ff28ee1de18bea397ef3ca4ae658faf58 15635 Automation to update templates (#50)
32c61535143c588a38857a19c40a807676b513eb Update Go and modules (#48)
5ededbae8649e84ddd6a34f12f0445afe138907e Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 5e9ebe1c9a97c21817701a5aa04185ad1bf4229d Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1242267934
eedff1f9c3ad5231083faf93ed16530f754515b1 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - f7d413a5804f0506d4324334170a339e4ff13856 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1240134327
24395f26ad8b5c4f44cb99c9e5e3d6776dc3c6c7 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 4a913e3222c708c33eebddf9be9f41345501bebf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1235193835
77e35de24c03b44d01352f84d47e2164ceea9ce2 onboard managedclusterimport-controller (#47)
1c9da1f0d21e2bbdf56734b0472705a90b8a8391 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 0867b07d045c305e26d8d2bc5bd66f10e8b6255f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1221968356
ad265f1a885d53747e603e1c4d784d61e8a9405d update cluster manager (#45)
31de3d0a847e04efe23f878e8dc4b4248c63c041 Use ownerreferences to handle cleanup (#46)
75fde901382e61da1e4b4192368700802a33e43e Add role to backplane (#44)
8055fbca7e8e6e86447deed72b6cfbd4a6d96cbf Use server-side apply to deploy (#41)
f3353ad40e54181031846f4a907cd1ae014380a9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ae67ba475e56280ba24cf1d77ec462f918f538b8 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1213388914
bb14c4ef9d81dbdb9be7edda8c525fc63e9a7a49 14976 proxy configs (#40)
37cee07444f3a7b95740a6a0d02c7dabe48e18ac  propagate proxy variables (#39)
57780768a70134f63e0eb23b38dc3e80b54e5aac  add toleration to spec (#38)
919deafd1216961cd6d69b5ebb21ff33fab39130 add image pull secret (#37)
59f388f455dc6d82476dbf2342056190cd4ef352 Watch subcomponents (#36)
b7c927600d0979ef185bef42ba4607ada9a4a596 14869 spec node selector (#34)
87dd0a0c93937eea680d4d336c12111bfbd1c99b rename csv to multicluster-engine (#35)
fdbfd10d2448619101b2dadd03589f5869ad2265 add clusterpool/claim permission in cluster admin (#32)
0756a71641dda98b1f2fe47b50ca7556f3eba6ad 15632-multiclusterengine-rename (#33)
d335d09863c117681a54625a479075e6ab0e8816 Expand Webhook Logic (#31)
a924b5ef358267bdd75815dd94e19c373d41c962 fix the different labels of ocm deployment and service (#30)
79761f7b3f050d6652abc54c4d04424fee382ecb Update clusterrole-foundation.yaml (#29)
20851b4a48e422657229cfe3eb9b40dc2c36f737 Update foundation roles (#28)
feb5e9779192a0f0ba159c7b7d994d3dd1fab937 auto-update-crds (#27)
e8b53c49d498d7b703e40803b478a515c62a2dfd Expand status (#25)
2a195e0ba85cb44c86a9e288f449e78c540de57f change config scope and related code (#24)
5d07faf017a20e0aa74088629869b18c38f60858 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 17bbf4a5958ba90a8be9200b0a97dec2b7d091a4 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1166508714
bb49db228d703c20ef3702ecfd21df6710dc0532 update channel (#23)
a96db35ae342ce17843989eabe1471a9bd1f58d0 Install Clustermanager and Hive Operator bundles (#22)
a29c95aff842e5cdea417884d28baba9dccc2caa Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 7f9ddf9af3aeb71003159083885592db73c7d66f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1158084680
8f7ee173f61c0ef7a0b18a36ce96f1e74e03187c Quick fix (#21)
afdda4a9e5d29f7eaf202a9c72f2e4fa7458cb44 Redesign server foundation installation (#19)
5e1e2ee441da387167d7255f36be3fd6223b3cfd 14546 installation guidance (#18)
b161e12e234343c44db22f44d458e44aeacfe0bf adding basic functional tests (#17)
f2aae328e7dae5fae38a3b03ef06c944f7ffd1c0  add files (#16)
8a055a298df3c4dd9798688ddd72c21657e2cf1c  fix image and sonar tests (#14)
638614610e5427f137ebf8a7fc82df8e092f89c6 Merge pull request #12 from zkayyali812/14710-webhook
7c038906069f4df146fe12edbbeae0063e202e5f Refactor Validatingwebhook
c0bfdf1deebb96ee26b4d1e86308ffb68603d9bc Run locally
a9abea9413a99c107eabf285164bf4e7967a51da Enable ValidatingWebhookConfiguration
796e3a8068e50319673fe479c8e43eeba72ce86c Merge pull request #11 from cameronmwall/setup-prow
47bb77ea5d1c153743689c7fd6a4767d6cbc8af4 setup prow
760d560cd23691dc7f632a143ff5deda590579e9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/main Chart SHA - 1e5712716d56b1641e7e28406d0a31b70b83486e Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1090944233
93d1454cfc4da589cfdd35e3c6d4e4ec0c5bf939 Merge pull request #10 from JakobGray/crd-auto-update
241d894b3b03005a67c5eb4036e0983e272abc63 Auto update CRDs from the hub-crds repo
5f2de4d6916e912cb882f56807b13039ebc3f2f2 Merge pull request #9 from zkayyali812/14711-add-finalizer-logic
c78b21e501b9e0b76972327d6c77d40c50909add Unit tests
a1a05dc180fcaa165275fa3b3a91f960bfec7d1c Merge branch 'main' of github.com:open-cluster-management/backplane-operator into 14711-add-finalizer-logic
fb6d52dccf5b315bb7c0640d90e7b23bb7118d69 Add Finalization Logic
03685c56181a5df4958d1c0c619e7b892c331f3e Merge pull request #8 from JakobGray/status
1073f32371b70cda733d61b545fbcb5022848b8f Add phase status to api
b7c901296d1fb06c83700fea5126bd0b992eb1a6 Merge pull request #7 from zkayyali812/14549-server-foundation
13d5a536482eda83cc2eb5e977177e9e8b627ea4 Add descriptions and update license test
9bc57fd1ce9e35eaffd5a12b1db081771cbed6d6 Install Server Foundation Components
47ee4a59cefb1841dcfb5c2b9fa3909d00d583aa Merge pull request #6 from open-cluster-management/JakobGray-patch-1
64f79176127069ac45f765f0c7f78f775cf83ab0 Update README.md
0108861937c167c4627082d35e01c3035bc7c597 Merge pull request #5 from JakobGray/license
00bd8dd658ad83358edc6940405c6160e0c3fcca Add files for contributing
2d320b259c3bc0b630fa46903e80c1db3c8d56ed Add OWNERS file for openshift-ci
68297ea458a022de70e4562a08f5ce94a9b4bcd4 Add Open Cluster Management license header and check
3ec3d4283b180895bcd6965a2d94a5d64ac3fa58 Merge pull request #4 from open-cluster-management/backplane-operator-mark1
777e9fbe1372f1ed5c6003d81c7e59344f21205c Add Hive RBAC
fd8817da9500c80e2d6ce47437da91100a2e4ecb Rebundle
79779c8384eccca583bbc63c5c8e02e6d7558b91 Add Unit Tests
abbfb2b3a79614434833ed0dfd42aaf33b7c51e9 Backplane-Operator Mark v1
339cddd2b48a1b2f681466179aae5b7add3300e9 Remove metrics mservice from bundle manifest (#2)
da69d07c831ec077eea219181acff3bf38cd25a5 Generate OLM bundle (#1)
278b7ef3037cad60f129d7353d30cd36e5563df1 Initial commit
```

Status: Fast-forwarded successfully.

### Branch main -> main:

New commits (first branch sync):

```
691c802a8c41cff91360f89c70e2f6fdb4ad42f9 Add HostedCluster and NodePool CRD's. This is so ServiceDelivery can use the ObjectRef capability! (#203)
1f3cbd21905e0bb5e468e59e92b26f269dd69f61 Update hypershift deployment crd (#198)
37a586c8d7d1b9f310853522d84c3994c3644a4e Add HostedCluster and NodePool obj references (#197)
6154ba205c861a8d0ff1b2ffddf84980a966f36e Add permission for nmstateconfigs for agent-install.openshift.io (#194)
732d4774dfbf578a881314745c6a773a1ce86d22 Regenerate Charts using inclusion (#195)
bfc7ea3545e705aae0851fd854618b8b6bb076ad adding conditional addition of global pull secret to EDIT environment variable (#191)
5fe67dcc6000fdf63396138c4492c93be1e50fea [create-pull-request] automated change (#192)
d6b404b9af987856caad911b679226ad478f234d add test for service monitor deletion (#190)
abc2f33f726d10909fcb2d9834f67be193357788 Update README.md (#189)
0a64096ab7c8249b73af574233f6330b01d20470 Picking up latest CRD from hypershift-deployment-controller. (#188)
ea9b9d1cef7ee2ac1c42109b093a6d64f5fb414d [create-pull-request] automated change (#187)
9d04f2dd496644ba9ecdad45110529fe2e89f2a0 [create-pull-request] automated change (#185)
b40cb45a6d98de1eaffee954029b29b75ba758bf watch servicemonitor resource (#186)
72c48e9060f1001b7d522298383c328a413b1b75 Add image override configmap support (#182)
134a9845a130dd644e13cccc9c7624a495354b89 Enable mce plugin when console is toggled on (#184)
975787031c10847bf01148d5efe3d3f8ea329e61 Add rbac requirements for consolequickstarts resource (#183)
4900dfc3eb9243069e89c268d6ae501be6e75e62 Create Quick Start for multicluster switcher (#151)
94f1f5b57a61717842513767c912cbbb5be5a8c8 Add managedclusteraddon deletecollection permission for import controller (#181)
9c46ea716bfecc1147215c8402b477a554da8892 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 99cfc43a28bd758a66bcfe195d48099746fbb212 Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/2204100020
1c8c5107b5c43a89745af46631825ac077a25653 update rbac of import-controller to fix 21838 (#180)
338f2df9aad2327be11a51dc91a78b0c13ad179d update command of cluster curator (#179)
5949b5c12a636829c5c97187b6bee7cbfaa02e12 update imageregistry crd to fix issue 21706 (#178)
ca312ef6349ed526650d9a7d019eb141942f9b48 [create-pull-request] automated change (#177)
a83ff2c0515cb3f72dfb50f66dfa86958f3341a6 Add support for spec.serviceAccountSigningKey. Issue 21690 (#176)
2bb312245a9eba5cfa958b2e24112ecb0062ac81 Apply new HypershiftDeployment printcolumns (#175)
7efd11035f30910b468a7b139eb734fae7b3284a New objectRef, resulted from final hypershift:release-4.10 vendoring (#174)
6336a083e89cba74ab71f769a57d80dcecf7ae2a add update rbac for managed cluster (#173)
ca4362ea1090f77b7e79171febb280b6126a402f Name ManagedServiceAccount as preview (#172)
0113ca8bf7b438b9ca769fe74f6cc6badac56abc [create-pull-request] automated change (#171)
cb4ed767befd4c1cada8ec44f2e2e1233460e9c2 update the renamed fields (#170)
9b2bc4b05643486efd173dd8b3d2f88c09eebcb9 [create-pull-request] automated change (#169)
90fe6c4039aa8fef7db45a04667f41b7e868b498 Update README.md (#168)
cffe77ecc61b941f4c17dbde7162065fd51a4f9e add lease permission (#167)
42600ee516c35d1370ae0b9a37a106bc17cbbb93 Added missing HOSTING print column for HypershiftDeployment (#166)
fdf13e3fab40ec88cdb6415c19ab658652dbb8ff [create-pull-request] automated change (#164)
d858822c201cd6266e42555cae6ea2cd3da60ab9 add lease rbac for work-manger addon agent in ocp 311 case (#165)
213a98649ee80c40ada3e292be7ea5fe969c4eea Rename ConfigMap (#163)
9645c89a35a85810f4a19ce3882d688e98a05223 Add new printer column and update CRD with hypershift:release-4.10 (#162)
1ff5135ec15327c4e7f32110ef687d5970ac9d84 Change ReplicaCount to 1 (#159)
d8a4b60659af10b8d13b1b7e512a4ae1520f5fad Add static override to change assisted installer namespace (#158)
d63200de8a69ee75826cda6e1eeb805765779e1a Proceed with deploying other components if one fails (#157)
1004517ed3a755a32102c0bd4ae2257c6b474672 Fix hypershift yaml format error and render test (#156)
34cc6eae651aad131d623b4bd1fba9d600b3d94e Collapse repeat components in spec to one (#154)
284d5522fac0cf53a540fe3e4fbdf3095d73cdde [create-pull-request] automated change (#155)
c68bddac39d8d244181cefaf314e9fa6373346ee [create-pull-request] automated change (#153)
4e504c321adf0fa2c5665c6684562e7aea1825ff Require no AgentServiceConfigs to delete MCE (#152)
dc667ed11a0287479606042e27c8fdc738de7384 No-op (#150)
49692834676c21874d8760dcddd6188ef5a9f828 Onboard HyperShift Configmap (#149)
6458171446ec1eccb1c7eadb0b0d7de686eee264 Add subscription.operators.coreos.com to console-clusterrole (#148)
9285bfd96d97ae15674e0a1de754682c7058c175 Merge pull request #147 from stolostron/zkayyali812-patch-1
bcc8cbf1f21352d002337e0878d3c8bda09a91a0 No-op
d295c8603bd90f1864490b72519aaff8321e4ebf Ensure ReplicaCount of 1 (#146)
363b1102077954c8287635da49b9c68dc4b9c1e0 Move component list to overrides and remove restrictions (#145)
dd14a1ec3f5058f84631b40955a55ca36d7c0137 Ensures bundled CSV is up to date (#144)
1fe7ddbb5923e12444402f620fd9ac517387c3b0 Merge pull request #142 from stolostron/zkayyali812-patch-1
edac57d9fcb93238f198c17145b5589c6f3ba60d No-op
474d5a3f4944b2d7df402c40b1a7dc426aa9331d Onboard Hypershift (#126)
c00a2425ba6aec046f8284b58d84f9f72de4e3d6 Pin Hive to mce-2.0 (#141)
90a2586264f5b91c0bc205d91ba3cf17fbe6906c Merge pull request #140 from stolostron/zkayyali812-patch-1
9b51ab7117495769c368ab9812c265875649edbd no-op
c9de7c4b74ee5d1ad212ffdb741d1ccb34a814f0 [create-pull-request] automated change (#139)
1bedc45e5991f3ee3c31c026a8faa683b3f6c643 Allow console-mce to be toggled off in 4.10 (#138)
b44481feae429ecffd0936effbec307d1dc88ea7 [create-pull-request] automated change (#137)
529ad00f36b37b53bc4395915c52ede27accd698 removing clusterrole and binding tests, updating cr & b naming to not duplicate (#136)
aa4da6ecdcbcf7b9d30ba97b5fa1174e77357fdd Add cluster-proxy-addon CRD (#133)
4e8e44fc39882f3a2e3c2b607c4a3b2b4104c11f [create-pull-request] automated change (#134)
3b54f8fcd343bc93205f2d8acb58bb61603bee74 update rbac for addonplacementscores and import controller (#132)
325c8f165fd5c88d0eb7c2cb95ba153ce46915bd updating script to run with python3 (#130)
5f4a84d0283c6fc7320e4025d6f64d245fbc9af7 redoing chart link to use https instead of ssh (#129)
61aa4ffe1f1f16f7571842bdca4f79c7cfe65b75 Chart polling (managed service account) (#128)
256a58ce391e2a349b323cdbef7681a0b458196f update go dependencies (#127)
6d734f2a290d48ce31c6154ae72db13b4e1c8f0c [create-pull-request] automated change (#122)
9bb3bd740f546fbdf1e8645d647b8d32c1b99153 Correct official MCE component name (#125)
85fb406de76b4c019d2668055d86d11700bad424 Allow components to be toggled on or off (#124)
63b46e9d23546e1f0a42930f792bec1e4ac1d459 adding agg roles for managed serviceaccount (#121)
e7d01d81b6f41f8f68a8c5bca93a6c5326994b7f Add PlacementDecisions to console-clusterrole (#123)
326edc0bcc7d6151e343463fb990c37c082ecc78 Latest Operator Bundle Updates (#119)
497e60f6f4da324e4a1cbe4da68982eb9ce390a9 Onboard Console-MCE (#118)
fdefc0f6529fca1b755de01d84b72e322c0461f0 Onboard AI to MCE (#112)
54b9b4b15be143c9fccd3f5fa08c9215bfe5c703 [create-pull-request] automated change (#117)
37603a75abe1a8c04aca20e00c2e8e6c97a8fef0 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - fcf3027d804c0f36e1b85a3fa1aec27dd184f46e Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1882088305
ff5c849da4c1078a7719c8c23e0df2597b825a60 set default targetNamespace to multicluster-engine (#116)
423e889a570f51bde991152f4193f1842814d9a8 Merge pull request #115 from zkayyali812/fix-sample
01cf6c79160ca72bf92e989ba50cbf21601dd505 Fix Sample
5c0202582466ed67c0b7681d35981c3ff21c138a Refactor License test (#114)
2ac44649a63c1d37c5cbe33d60aa01923e205339 match clc-state-metrics ClusterRoleBinding to correct ClusterRole (#113)
92f2afb9301a019928958b461a7e8b81b0478e33 No-op (#111)
c6057493924d093bbc0f78c80acfcd8b5cb9d987 Automate Discovery (#108)
308c7cb1fb147e52624b7639523f8292ec64e562 update foundation clusterrole (#109)
62d32258f05898aeead5a84c090cf520eab5c845 Nweather managed serviceaccount support (#4) (#105)
051c8ee1dbbb257a68b0cecb4e71a6855d686f1e  Canary fix (#107)
8eeb800764f27cfaea95c522b9f21141e297764d Update Discovery CRDs (#106)
3d616c4417369f15ded7b58db9c081a6589c64e1 add discovery (#96)
90bc805dc42e4802c9e33906943182c5265b83f1 Add arm64 for MCE (#104)
55de156c0cae55dfdb3d8e39a1a0a7f6f0318991 Update README.md
6674a04b150573a1e3aecdf928b2349577d95e43 Onboard CLC (#100)
3b0826089509d912c3f41680d1f81c0b18323618 Update registration bundle automation (#101)
cd134b9c29003543bc0150b28e2b02f2356f5492 Configure webhook for mce v1 (#99)
5d702a49d2cd326da899a572e4b44ccd64bb1da7 No-op PR (#95)
66e2ad2fa49bf7e378460833b0757a60ae2f64fb No-op PR (#94)
1603260fa040656178e079df77d15cb92af80efc Update to v1 (#93)
9704892826b5bf9ea20b12c94663681512e02971  add back pod namespace (#92)
b41bfae5a5e3292e6b1fa03b6a0a0b60fddbd593 change default image pull policy to always and add override (#91)
cc86c9e0d2b1e2a7d0fd105fea8858f20b433db8 [create-pull-request] automated change (#86)
22ac530acb53c04ea71c75cb6ce678a94fb6f3d6 Label adopted subcomponents (#88)
e2d4aefe0abd5f55f8a6219dd2628cfa6c00b759  add availability configuration (#87)
803834a696b7bad29e76d7d45dd4fc38af74113b Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - stolostron/hub-crds Chart Branch - refs/heads/release-2.5 Chart SHA - 9edbc5ff4293a0d1c46fb56c7bd719a3b1cb44cf Workflow URL - https://github.com/stolostron/backplane-operator/actions/runs/1684452233
41d9d602b5123f33462a3424ec9a15a069ee245f rename update (#84)
9232af7f64d5bb1a6f17793a805f90315b63937c Update functional test suite (#83)
f08a30f1074d73530b619cafb0ed7804c17f1dcf Allow installation with existing MCH (#82)
013a778a07aa1aad3472ffae84064dd83fb80f88 Update COMPONENT_VERSION to 2.0.0 (#81)
29fb30d35688408afff802f91f636a70f9c6d7b6 No-op change (#80)
c6ba0a203b87a1dcc74a66f79070757545f9f256 Adds OCM webhook definitions (#79)
369e6f836a615380df1cecdb6ed038f25e80f00e Manual manifests refresh (#78)
a0b4faa612f5bd60277fc03badff1384c9e8674a [create-pull-request] automated change (#77)
0ba0fea0723a3dd176855c3b1752990095f2bb56 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 425b5ba413fafae825a735c0511dbb36691ecf41 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1346958202
be8277514e763926e215fe9504ddbe1c60550020 Install ClusterManagementAddon (#76)
1511a69bfc4fe6288f9b51a216fc0f25093828ca  bundle fix (#75)
2b9c6f8131358319e0df80c701d80b965a0ba4cb Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 8381b82c22103d820d16b5d4eae53d98f6c365ed Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1317639471
765505d4924d65b64f1d7d53846b7350fc0d01bd Prepare global (#73)
a949ac2eb161933e0dbf197c66ad95ccc563166a Remove MCO from MCE Webhook (#72)
c92dda938a1cae7898405796df945daab0dc1723 Track UID in status manager (#71)
bf9af1eb748e5fab7b8e48ce87ab8dc399c765ff Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 717a30350c872334abfea1dc39f85de6b9848c3b Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1309498819
aebfb3ba8ce771aa78f5d76da647cfde8acab5fa [create-pull-request] automated change (#70)
e516a298c7b95fe3e574991ceede8f14fa28694d  add default tolerations to the cluster manager resource (#67)
463bea09c2d144057b33f17d1e8a6f8eca98a11b Operator Bundle Update (#66)
2718b17653c4e899982f32d2fd85e773bedd3d36 Annotations (#64)
91c6b57ac0df3eaeeb378d5f8b0cb5cb0863e7e3 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ff366feb12c4bc67a39541e6c9d75cabe521edbf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1285727449
b9681bdbb6cad525c3ef605389d54d67e0fb21e1 Report status while mce uninstalls (#62)
f0dc7d3d12f5272536a31a0580986246e4643867 Update managedclusterimport controller RBAC (#61)
de757769be40d6e11863fed21008c059552f5374 Operator Bundle Update (#60)
586c90c63ebb1c6f9208eb93ec095da166dbf6f8 Fetch images from backplane pipeline (#59)
5a040f639c2f74519683cd3db9a35388f9496d8d Install foundation agent automatically (#56)
5e132032b4e1adc5e7ac5bc638889bdba1fafcf2 Mods (#58)
ad2642b6a675baa7c9aa8d9d1648ff13f5335a9f Remove unused code (#57)
8e2aa7caa097f40d0a0d02aec100586f79a9bee4 Refactor reconciler (#53)
eee5f5f9e6cb0512f66a68bc70e5a57034046484 Update .gitignore (#55)
2319a0cd3ca5d453401f291d9177c333c99ee8db Lint Operator Bundles (#52)
4b258cfff1fab2df325fc708e8cd2d2e7b0c8ead Remove foo field from CRD (#51)
1694fa6ff28ee1de18bea397ef3ca4ae658faf58 15635 Automation to update templates (#50)
32c61535143c588a38857a19c40a807676b513eb Update Go and modules (#48)
5ededbae8649e84ddd6a34f12f0445afe138907e Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 5e9ebe1c9a97c21817701a5aa04185ad1bf4229d Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1242267934
eedff1f9c3ad5231083faf93ed16530f754515b1 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - f7d413a5804f0506d4324334170a339e4ff13856 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1240134327
24395f26ad8b5c4f44cb99c9e5e3d6776dc3c6c7 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 4a913e3222c708c33eebddf9be9f41345501bebf Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1235193835
77e35de24c03b44d01352f84d47e2164ceea9ce2 onboard managedclusterimport-controller (#47)
1c9da1f0d21e2bbdf56734b0472705a90b8a8391 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 0867b07d045c305e26d8d2bc5bd66f10e8b6255f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1221968356
ad265f1a885d53747e603e1c4d784d61e8a9405d update cluster manager (#45)
31de3d0a847e04efe23f878e8dc4b4248c63c041 Use ownerreferences to handle cleanup (#46)
75fde901382e61da1e4b4192368700802a33e43e Add role to backplane (#44)
8055fbca7e8e6e86447deed72b6cfbd4a6d96cbf Use server-side apply to deploy (#41)
f3353ad40e54181031846f4a907cd1ae014380a9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - ae67ba475e56280ba24cf1d77ec462f918f538b8 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1213388914
bb14c4ef9d81dbdb9be7edda8c525fc63e9a7a49 14976 proxy configs (#40)
37cee07444f3a7b95740a6a0d02c7dabe48e18ac  propagate proxy variables (#39)
57780768a70134f63e0eb23b38dc3e80b54e5aac  add toleration to spec (#38)
919deafd1216961cd6d69b5ebb21ff33fab39130 add image pull secret (#37)
59f388f455dc6d82476dbf2342056190cd4ef352 Watch subcomponents (#36)
b7c927600d0979ef185bef42ba4607ada9a4a596 14869 spec node selector (#34)
87dd0a0c93937eea680d4d336c12111bfbd1c99b rename csv to multicluster-engine (#35)
fdbfd10d2448619101b2dadd03589f5869ad2265 add clusterpool/claim permission in cluster admin (#32)
0756a71641dda98b1f2fe47b50ca7556f3eba6ad 15632-multiclusterengine-rename (#33)
d335d09863c117681a54625a479075e6ab0e8816 Expand Webhook Logic (#31)
a924b5ef358267bdd75815dd94e19c373d41c962 fix the different labels of ocm deployment and service (#30)
79761f7b3f050d6652abc54c4d04424fee382ecb Update clusterrole-foundation.yaml (#29)
20851b4a48e422657229cfe3eb9b40dc2c36f737 Update foundation roles (#28)
feb5e9779192a0f0ba159c7b7d994d3dd1fab937 auto-update-crds (#27)
e8b53c49d498d7b703e40803b478a515c62a2dfd Expand status (#25)
2a195e0ba85cb44c86a9e288f449e78c540de57f change config scope and related code (#24)
5d07faf017a20e0aa74088629869b18c38f60858 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 17bbf4a5958ba90a8be9200b0a97dec2b7d091a4 Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1166508714
bb49db228d703c20ef3702ecfd21df6710dc0532 update channel (#23)
a96db35ae342ce17843989eabe1471a9bd1f58d0 Install Clustermanager and Hive Operator bundles (#22)
a29c95aff842e5cdea417884d28baba9dccc2caa Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/release-2.4 Chart SHA - 7f9ddf9af3aeb71003159083885592db73c7d66f Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1158084680
8f7ee173f61c0ef7a0b18a36ce96f1e74e03187c Quick fix (#21)
afdda4a9e5d29f7eaf202a9c72f2e4fa7458cb44 Redesign server foundation installation (#19)
5e1e2ee441da387167d7255f36be3fd6223b3cfd 14546 installation guidance (#18)
b161e12e234343c44db22f44d458e44aeacfe0bf adding basic functional tests (#17)
f2aae328e7dae5fae38a3b03ef06c944f7ffd1c0  add files (#16)
8a055a298df3c4dd9798688ddd72c21657e2cf1c  fix image and sonar tests (#14)
638614610e5427f137ebf8a7fc82df8e092f89c6 Merge pull request #12 from zkayyali812/14710-webhook
7c038906069f4df146fe12edbbeae0063e202e5f Refactor Validatingwebhook
c0bfdf1deebb96ee26b4d1e86308ffb68603d9bc Run locally
a9abea9413a99c107eabf285164bf4e7967a51da Enable ValidatingWebhookConfiguration
796e3a8068e50319673fe479c8e43eeba72ce86c Merge pull request #11 from cameronmwall/setup-prow
47bb77ea5d1c153743689c7fd6a4767d6cbc8af4 setup prow
760d560cd23691dc7f632a143ff5deda590579e9 Chart update run automatically via repository_dispatch Initiated by - acm-installer-team Chart Repo - open-cluster-management/hub-crds Chart Branch - refs/heads/main Chart SHA - 1e5712716d56b1641e7e28406d0a31b70b83486e Workflow URL - https://github.com/open-cluster-management/backplane-operator/actions/runs/1090944233
93d1454cfc4da589cfdd35e3c6d4e4ec0c5bf939 Merge pull request #10 from JakobGray/crd-auto-update
241d894b3b03005a67c5eb4036e0983e272abc63 Auto update CRDs from the hub-crds repo
5f2de4d6916e912cb882f56807b13039ebc3f2f2 Merge pull request #9 from zkayyali812/14711-add-finalizer-logic
c78b21e501b9e0b76972327d6c77d40c50909add Unit tests
a1a05dc180fcaa165275fa3b3a91f960bfec7d1c Merge branch 'main' of github.com:open-cluster-management/backplane-operator into 14711-add-finalizer-logic
fb6d52dccf5b315bb7c0640d90e7b23bb7118d69 Add Finalization Logic
03685c56181a5df4958d1c0c619e7b892c331f3e Merge pull request #8 from JakobGray/status
1073f32371b70cda733d61b545fbcb5022848b8f Add phase status to api
b7c901296d1fb06c83700fea5126bd0b992eb1a6 Merge pull request #7 from zkayyali812/14549-server-foundation
13d5a536482eda83cc2eb5e977177e9e8b627ea4 Add descriptions and update license test
9bc57fd1ce9e35eaffd5a12b1db081771cbed6d6 Install Server Foundation Components
47ee4a59cefb1841dcfb5c2b9fa3909d00d583aa Merge pull request #6 from open-cluster-management/JakobGray-patch-1
64f79176127069ac45f765f0c7f78f775cf83ab0 Update README.md
0108861937c167c4627082d35e01c3035bc7c597 Merge pull request #5 from JakobGray/license
00bd8dd658ad83358edc6940405c6160e0c3fcca Add files for contributing
2d320b259c3bc0b630fa46903e80c1db3c8d56ed Add OWNERS file for openshift-ci
68297ea458a022de70e4562a08f5ce94a9b4bcd4 Add Open Cluster Management license header and check
3ec3d4283b180895bcd6965a2d94a5d64ac3fa58 Merge pull request #4 from open-cluster-management/backplane-operator-mark1
777e9fbe1372f1ed5c6003d81c7e59344f21205c Add Hive RBAC
fd8817da9500c80e2d6ce47437da91100a2e4ecb Rebundle
79779c8384eccca583bbc63c5c8e02e6d7558b91 Add Unit Tests
abbfb2b3a79614434833ed0dfd42aaf33b7c51e9 Backplane-Operator Mark v1
339cddd2b48a1b2f681466179aae5b7add3300e9 Remove metrics mservice from bundle manifest (#2)
da69d07c831ec077eea219181acff3bf38cd25a5 Generate OLM bundle (#1)
278b7ef3037cad60f129d7353d30cd36e5563df1 Initial commit
```

Status: Fast-forwarded successfully.
