## Fast foarding of stolostron/hypershift-deployment-controller into stolostron-engine/hypershift-deployment-controller.

## Status Summary:

backplane-2.0 -> backplane-2.0: First run, created backplane-2.0.  

### Branch backplane-2.0 -> backplane-2.0:

New commits (first branch sync):

```
16c7885a3c1c8559e323628dd3a6fd8cb4511a30 Use replicas to config the desired number of nodes the pool should maintain (#97)
6a24f89ef78559fb9041ba92269b2e1eb85abd1d Add details on using the Agent platform (#93)
b905f82a93fb7c3265db1a4b4134bb9e61f520ca Update all the libraries to 1.18: (#95)
b0e650777cb702fc3e0296f269dd0270f46439e8 Set infra and iam status condition to NA for configure=F (#94)
d3ecd1a7fdf2fcee3c7bcf173feebd32505e5e76 Bump golang to 1.18 (#92)
a3e13c103b51c73719ff1d9e1de13c765953ef56 Change where we set the conditions (#91)
cf434e4b182f6a4bb8cb1aad58dd8809534a6ed9 doc update to add the backup label to secrets (#89)
87bf7307f28e0815ce6debe41b595cbb5a9e36a8 Support hosted cluster obj ref in hypershift deployment CRD (#86)
9b3e02a4cdd32ff266f1ebe96641a7e853a0ee11 update hypershift provision doc in mce (#90)
95994a32e1335f134c2f470dd033ae64cc3e8802 Update pull_request_template.md
c3d8e20328541f5eaf2d14e29ee537e4d2890f82 Sonar gosec fix (#88)
0838702288d410f18268f2669a0e5cc2746520f1 Update README.md
aa18414f1a92a85b481d1a521c18e9b403df1d01 Update README.md
2bf49fcd27882fc3a7669897ba179f0f1b34fb31 Create pull_request_template.md
57a919adb6909ae8e3ea3be8f88f306ccb3c7bd8 Update hypershift main (#87)
67b4290e97cf6e8250f678e2c9245d254f9f5185 Aws & Azure infrastructure mock tests (#85)
9c43442f4a541a91f1e98aa6f7c2934576491889 Do not create HC configuration items in hosting cluster (#84)
7853f833498ca44e71ec7ef75277294bb890cf3e Update content.md
e681acb2caa0f1b1a7d032857a28bae33ea7cc53 Set reason for condition IAMConfigured to NA (#81)
2cfcbbbc293ce82723bc670a203616d9d8361521 Generate etcd encryption secret for Configure=T path (#79)
f165cac9a4dddfeddced1e9392ee76d9a861ea0a Add infra-id label to HypershiftDeployment and update constants (#80)
619056b334c443778f667e2e91b4bba9d70e5aa0 Add integration tests (#76)
9775f77ef0d0be5105303597718d258e71f31b4c Add support for Spec.ServiceAccountSigningKey (#78)
835c10b4dd34c72b979a3a2f9a4f2b515cbda580 Update print column conditions: (#77)
6b862a4bcae1003ce0e2c5f1efdd939456c0c096 Support for Additional Trust Bundles (#75)
39abb5b0100c5f5df952f7fe81fba66cf79789af Update owners (#73)
9cdba194f3f6a90a6c938b75de060e5d87a6756c Vendorize with final branch for ACM2.5, OCP 4.10, using hypershift:release-4.10 (#74)
d0867c0189e486f3c1bc270aa41c455eb1431b71 Set delete option foreground when need to delete namespace (#71)
929b6379baa811deed7624de707e03c9f1be786c Add scripts to test sd case (#72)
973d4603dd5592e95d785d097cacfcb9b6cc36c2 delete the hosted cluster after the managed cluster is deleted (#69)
31670a096cd388cdc0aad749bbc09b719bfa896f Add vendor and cloud label for managed cluster (#70)
0bef047674e00366d6532630e87e1359699395ce Remove oidc service def. Not required (#68)
ae9d04519eb773db58911fcade86c50c163b1972 Keep hc and np in hostingCluster for Orphan override option (#65)
2385e7fa06ec4fcd4f9144fd4d570efc79600e82 Quickstart (#66)
cf6a2e1bbd88943e9f1812f340ab85ce25abd8aa Make ManifestWork the default, remove the override for Manifestwork, and remove the code that creates local resources. (#64)
f353d89779d73bff657248ee4423ed1bd641095d Set default values for hosted cluster (#63)
4911843a848aaa2b645f069e878c3caddf74ee00 Origin/default manifest (#62)
3e37670d29e4cc79e72dddc2b4e272f00f177ae9 trigger image build on CI (#61)
bfc56e3d3d322e4d6b57842014917c26ee41a5b4 rename target to hosting (#60)
61b0dca9375b3122795ee43382c9008e7810eabf Rename management cluster to hosting cluster (#58)
4c0c8d1b069dc023a1cad763e98add37041d1406 Totally applied the map wrong... (#57)
f462f07afe67951c92eed82db88c830cdf8761fb * Add printcolumn HOSTING column, that will show Partial, or Completed on the HypershiftDeployment (#56)
3cbc2b997eb92ff36ee42d245c555499b58836af Bug: Found that extra secrets were being created on the Hub when over… (#55)
ad0cf235aab8422ff774876b6d1f44bce9ffe157 20607 sync status (#54)
446e07d45acf061fb7f4e98b374efaf361231c42 Allow the ObjectRef.Name value that is present in the HostedClusterSpec to be used when generating the secrets inside the ManifestWork. Includes tests for the default names and for custom names (#53)
1fca34c744813c97629327623a8ad4f579481381 Add document around HypershiftDeployment and extra-config-resources (#29)
d9e734e70eb73e90e34497169b39e50953b3e7a7 Add ssh key v1 (#52)
89d4b60dc06ad1bfdd7f00e7f1acc634ba411689 Bug fixes: (#50)
42838a97899b48ca9c7b8fdaf3071c01c46136fc Ensure the target namespace existes on the management cluster (#48)
6458bdc8fea79332420eee28147ac369462d8f1d make sure the default release image string is used (#49)
6854f9392e269f907676b584593af127fc048cf0 Use patch to set finalizer for hypershift deployment (#47)
3e7b0b7e3de1221a315631cf5080808cdaa13cb5 Get oidc info from secret when using manifestwork (#45)
4529aa530ea83a840fae6f88fe7748f620bb0279 Pass the control plane operator image annotation to hosted cluster (#46)
584da59c4688f8273a34a0d40ca0c070e73caa84 Doc for enable hypershift in MCE (#43)
713f2768f454ff6dbb494bf624b8c061491e2f5b Fix for issue 20823 (#44)
3da972ded44181e8361c3bcb84b5cda6060a02a6 Add provisioner annotation for managed cluster (#42)
8a4335d332fecbe07f2336870b0c48e55a16349d Update Detached mode to Hosted (#41)
ef82457b0b381df50e3b09abe17ec8702b7cb420 doc: quick start for MCE/ACM users (#40)
53e8c424ab9a095255b8985c1e9365e8773797a7 Add an auto import controller to import the hosted cluster (#32)
4f65896a48296fc98ab0649fcc304b702630a170 use infraID as manifestwork name (#38)
714a4d554de36d0247608fbfd436502c4d1b66ab Add Azure unit tests to match AWS Scaffolding tests (#37)
725ee08c3fc60f77a6bb80de87edcbb7bd19295a Add Azure ManifestWork support (#36)
0107134cbe70af79894ac5cdad3b6f78f296825b #20243 configurations (#35)
1d11d54513409d9c64dbbade4e2b6200290bf7b5 Add Azure support to HypershiftDeployment (#31)
9d27484f822c393fcbaa918d5d2598e3b8b2350c Add hypershift deployment annotation to hosted cluster (#34)
f622642e10f31c13a45b397c389362725a127917 make sure the update of manifestwork is working (#28)
14ba28db50ee33abd547744e091ec24ad98422c5 Change user for the Dockerfile (#27)
bbdf9befc5b073bf108cb348e11ed049af368cdc Move the ARN's that are stored in secrets over to the HypershiftDeployment (#26)
05e7094ede34c272287340c48b6296bf790a3cdd Remove generate from make build (#24)
a3ffd195dceaf653d4eef606b0706dac215b332a make sure the manifestwork can be create and delete properly from hypershiftDeployment controller (#25)
06cfb54f5ef71bad321795da9cc329616345668a address manifestwork related issues (#23)
4e2723ac8739334ddd9b69f292b3b1ea1baa54f3 Fix for subnet error (#22)
644c81691ad43151870f0da72336a1e3e6b26de0 Subnet update hypershift (#21)
1cc36a875d7db2fc4aaf559b679fd7db75b300f9 Bump the hypershift module version: v0.0.0-20220218003034-93ea4702f952 (#20)
060d58845ddc62689f4bfe04ad988c73ce1284f1 remove vendor from build target in makefile (#19)
d2085a549caa65b3f5aae4b1631446aa0082144e Target namespace enable (#17)
5835c161dcc17515a21309d1bc89230b1b85a2ab Add ManifestWork rules (#18)
0233fea3f51ec0e39d4ee97bef4d6e74095869c0 Basic tests (#16)
d1423c6a8e04181183df8f7e047d1738a12e320a Wrap hostedcluster and nodepool in Manifestwork after the infra is created (#14)
aa533b585322c9a74e5355b2668846f36da0bcde Clean up duplicate import (#13)
17222788a93765bd0c6de2096bc4d4c39d7d63a1 Async delete (#12)
1e5c17870a139e098877bec44272efab8895f19a Add support for ZoneID's from infrastructur (#10)
af7f704e305c00d593e35b13a3125679fb6e5b83 Add Provider Secret Condition (#9)
a705c6602f150122a4e648f037de932d42e063a6 Intro infra override (#8)
c9e68b60ce3e4d7fbba2711ae7af00b5d7dc012d Make sure that make manifests, correctly creates the roles.yaml (#5)
6504784300035a58a1d648e065a80f5da7fbc108 Fix make manifests to not include webhook (#6)
0199ef24ff7e88d7df19aa0787aeb13133ce98dd Fit and finish (#4)
0d84ad1bda17b127b71276458da785706e82cbd6 Merge pull request #2 from jnpacker/update-readme
4ae5a92a3ec1e3f4e535156da18633621121eaa9 Update README.md
bf3c8e6658ef6c43ce665c745bf6361686d23946 Merge pull request #1 from jnpacker/initial-license
c039c8c54550bed4cde8ebaf6d078b24de3e6a63 Add licensing and ownership information
a429334636b64430ddd89e3512d8d64497a0b5e3 Initial commit
3a0530fcd8cf83baaf6ae1f40c0d925743c45d55 Initial commit
```

Status: Fast-forwarded successfully.
