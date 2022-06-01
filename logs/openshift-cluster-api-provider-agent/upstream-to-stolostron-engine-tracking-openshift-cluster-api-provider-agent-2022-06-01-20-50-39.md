## Fast foarding of openshift/cluster-api-provider-agent into stolostron-engine/tracking-openshift-cluster-api-provider-agent.

## Status Summary:

master -> backplane-2.0: First run, created backplane-2.0.  

### Branch master -> backplane-2.0:

New commits (first branch sync):

```
195e73284964fd97d6365c99bc852c8a36f86207 NO-ISSUE: fixing some typos in the README (#46)
fe07a1a601b1eb6138fd44d9e9902435e273e76d MGMT-9946: Avoid unnecessary requeues in agent cluster controller (#45)
43fd6e0db06158ff96203a171f106dbc007b595e MGMT-9826: AgentMachine controller watches Agents (#42)
a81e915d8ead3aec82b60c8287555232ba9c8a41 MGMT-9821: Add Conditions to AgentMachines (#41)
dd6353f609dc9e7bfd0312ce4b2c8d3dac5d749e MGMT-9422: Remove choosing Agents by minimum CPU and RAM (#40)
3e97ff2910f9a92cc3497ddad84b25cd911f3f30 MGMT-9398: capi-provideer leak the agentMachineRef on the agent CR (#39)
ed7700491054e7a6ac886d7261c03901d01b7b13 Extend OWNERS file, I join the party (#33)
5547ce3c684d5f33f37efa80d7164ee76705938c MGMT-9390: Add owner ref on the ClusterDeployment (#38)
6b7a21702910032ecfe119c06ae3dfeefa3c89c4 MGMT-9278: Adding wait for control plane to be ready (#37)
8b0ef0efc693e4ce9508428018d05ef1c557d5a8 MGMT-9255 agentcluster_controller sometimes fails to update the ACI (#36)
49686348da71e04d83bfd6fdc61f8c67c93b23fd Bug 2045067: Adding clustermetadata to clusterdeployment (#34)
11db8af765258ea7b6de5588c8a038e18cb1f407 MGMT-9254 Failure to update agentCluster.Status breaks reconciliation (#35)
03d0b4a038df424872c15ac76f121d2575f8f530 MGMT-8859: Refactor agentCluster spec to hold just the ControlPlaneEnpoint (#30)
d0773900578f96aa0ea4bdca5479aa06ff6b0cfc BZ2047937: Fix Make deploy manager arguments (#31)
70b56aedb93d18fdf7b47e1f66a6e61d0cfb4b36 Update Makefile to allow setting runtime CLI (#32)
175a7788cf4abdff19100075055415c535cb9443 Updated readme with Provider ID controller info (#29)
4bf24014170091666d52e835774e0c209cfecf47 MGMT-8849: Avoid races when matching agents (#26)
1f8b4de090154570b2060dfff2cd937fe9b58d27 Add namespace scope options (#27)
2b267e259f2307bb53f78688e257b68a924ce13c MGMT-8907: Add ACI ref in CD creation (#28)
b81d5354658149b811ba67c831a1d41b7f36b4f5 MGMT-8819-list-agents-by-namespace (#25)
5c7cf44a4685c2ab62b503a9b57cb33fda6d2d75 MGMT-8821: Option to specify watch namespace (#24)
17b49facb577539aab6aa26b761983a72fef2ab9 MGMT-8668: Remove release image from AgentCluster (#17)
a04d0a7973269e7cf4d27093dca5b8005c3e1c4e Added golangci conf file and fix all current errors (#22)
21f6f0509a7a47ef5b1318c5b8caaa67be36e1f5 Mgmt 8764: agent fail to pull ignition due to expired token (#20)
13c7d124f075a60fa53aabae1ac0d6c932ae21dc Fix machineConfigPool logging (#19)
e93a02f0c7ce81a369f83c31d906ea032d51d596 Remove the 'system' suffix from the capi-provider-agent default namespace (#15)
e990a0a8e3cbb4ee702f70e3377c642c69b28a86 Add label to token secret (#16)
3bb4d79bfa4ef9df9d9da29417d892909441b532 MGMT-8706: Add secret create to AgentMachine controller rbac in order to create ignition token secret (#14)
19ae53c6fe0432cacabeceb04b4484b34cb804c9 MGMT-8679: Add lint to makefile (#13)
a308f9be047e68cf232f3e5d1247c1390bace60a Merge pull request #12 from avishayt/avishay/user-data-secret-copy
62e477a5b638d9b674aa0dd982d345a5c4ea94f1 Accept ignition token as user-data secret and copy to a new one
6ae181af926730acfac475a71c1fc6605bb1ff05 Merge pull request #11 from avishayt/avishay/MGMT-8609
cac2f59de5a91b2be3a1f0e45190c61ae5f60b1a MGMT-8609: Align provider to use secretRef for token and Ca Cert
0bfb3322e3132f1d437813ed47cc780580e48a1e Merge pull request #10 from eranco74/lint
f44243ab86d980ac7d412fb3d87d8c940aab212e Fixed formating and lint errors
b6e3a7c9b7ef74fa9b02ce3cc6b483f9ab279d10 Merge pull request #9 from eranco74/allowDeleteIfAgentIsMissing
4ed2033460d9696ff69170758f3a72ccb860ef17 Merge pull request #8 from eranco74/RequeueAfterWhileWaitingForAgent
38013f4900d335537593418bc1f2702f1980d0c3 Allow deleting AgnetMachine in case the referenced agent wasn't found
03c81a12bdb48b956c110ebe5d374d31f22c988b Added RequeueAfter 30 seconds in case there is no available Agent for the AgentMachine
46a222623aa43a13518864dd80f49762677e4d2a Merge pull request #7 from avishayt/avishay/fix-api-comments
0293b7b9f600c2599bebb2f894d49da526ece8e2 Fix comments according to guidelines
47815ccb09132a77bd96f433581c3e3c48ec785d Align dockerfile with other openshift cluster-api-providers forks The build stage in the dockerfile should use vendor
b6e397056fb6114971fccf64c165e515c682f2d3 Added vendoring of the api sub module
91e8810e2f7c703b9e089d74bb671eb666b6ee43 Updated the base image to registry.ci.openshift.org/ocp/4.10:base
1e2b4bbd1cf7e923b252a444c311733e5bd44df7 Added vendor directory
b55340fd62922484ed71834d5b69f16215e15a3e Fix go fmt
220b4fb3669502c4c62fc8544a5bfbd8bd868010 Added OWNERS file
b1cb8da87e73fa276bfa99ef5a82d81841a4df3a Reference openshift github org
8777a997068e371e76abad81f07d3a4c6bf6ca86 Simplify flow with one update per reconcile
7fa94a621a1c4efec34faac2ee359f74f5d8c4bd Rename publish image steps in build workflow
b76f5940919682780591f243376b06145484811c MGMT-8434: fix missing info in error to get secret
b633556695e5cf60ad53b00135e9267559a6d9b3 MGMT-8408: capi-provider-agent fail to create clusterdeployment Added AgentBareMetal platform to clusterdeployment spec
ed7ea7867aa3b36866d271d4edb0a2e489195e71 Updated the API Version of Cluster API (contract) to v1beta1
2ee36da80c8d001baf315e67b936406d84cc746b Added metadata.yaml
f3a1432efe4569397bff6560710b9a3f4ade77a7 Updated readme
c330a47131ff2319485de5c77370a718cec4c36c clustectl integration
17f629b16ac84bbf823e6329191d42a9fb724ef4 MGMT-8347: AgentCluster shouldn't set status.ready to true without having controlPlaneEndpoint set in the spec
60a94bdac0cd7f9198aa541159dcffdc87d32eaf Added mokegen target to makefile
b94519272255df04defac3c828fbe030ef16a41a MGMT-8311: Add ProviderID to Node This commit adds a controller that will reconcile agentMachine with status ready, the controller get a REST client to the cluster API and adds the agentMachine ProviderID to the matching node spec
f133b858f7ac1a4adad05d7c4901630756439da4 Added focus and skip flags to make test
35d8ba4c7dd89f49ebc63503e91b3cbf9fd76357 MGMT-8352: AgentMachine ignition properties fixups
e9ea5460cf023f1fd038cba0bd921b7701181293 MGMT-8339: Use hardware reqs and labels when matching agents to machines
ee92dfba2d5ea32d53b09a990696fec1b6d49819 The clusterctl integration messed up the capi integration (the versioning is wrong) and the make deploy target (can't override the image) Revert "Added clusterctl integration" Revert "Updated commonLabels to map all cluster.x-k8s.io/ versions to v1alpha1"
fe20140b9e1594aaeb952aad7b3afdfa176af472 Add filename and line number to capi-provider-agent logs
3e305fc1ac6788c1099db2973b1a80f7a474b694 AgentMachine finalizer improvements
28afd0b02641506d97a5bd2d8538581669470054 Improve unit test coverage
3b20d674d78a39ab9ac3f78aa47c1124714ba4cf Update README.md
c023d356aadffd4fe6352e2bc1eaba2da9a1be51 Convert IP from CIDR format
391b17135625d68498ff745b9d505674a48baaf4 MGMT-8320 Unbind agent upon AgentMachine deletion
feb372e547842613be50c7162bd85c809f1bddb1 Return error in case of failure to update the agentMachine
c8ca319836ddc0ea884a374140ac99495bb5f613 Add machine internal DNS to the agentmachine addresses
1db481f8c7582f67fa361c4fb7c1fdd3852577d9 Update the providerID on the agentmachine spec
9775931a93491b8131968831f15bdc1cda76a525 agentmachine_controller stop reconciling CRs once the installation starts
6527b66b354b5f8c77c8f85851445580455496c9 Generated the updated CRDs and the updated role
ce2c3f0daebdc939eb50ea3c4b1410adf96de8f9 Add CRD generation in the api directory since the api dir is a different submodule it seems that the controller-gen isn't generating the CRDs for the types in the api directory
24169822032c4c70354a7a1a59c53bd97cf94393 RBAC generation
18ccc2fa4ce5d839df52a9de149bc25a8b02af68 Add ControlPlaneEndpoint to AgentCluster Spec (#33)
19c479d66a758d664fa8e1fa245041602e11bf7c Updated commonLabels to map all cluster.x-k8s.io/ versions to v1alpha1
49abce388201dda49dbd99545333ce5b270aec7d Fix add agentmachine controller rbac for secret adding empty string as the secret apiGroups: //+kubebuilder:rbac:groups="",... without it the deploy target fail with this error: The ClusterRole "cluster-api-provider-agent-manager-role" is invalid: rules[0].apiGroups: Required value: resource rules must supply at least one api group
1c8460aa6f51ba4d5de7807e7d750e555ad603e9 Added clusterctl integration
86d71ffaa1102f136e716188a732af0694d9be0c add agentmachine controller rbac for secret
d05011f84eea4d1491fa7c93cc80804dbce85e62 Do not continue if ownerref not set on agentmachine
721daa4de07c8463721c65f98df0ae30c407f2dc Remove last component of ignition URL
61fbf441ae2dcf03ed66308343183abd5a18bca6 clusterAgent with ready=true shouldn't get skipped during reconsile since some information might change and should get synced This is relevant for the ignition endpoint that is being added to the agentCluster after it get created but can be relevant to other configurations as well
38f3fd12bfbcf4d5a874433bf6516253fc9092ef MGMT-8259: update ControlPlaneAgents in ACI to 3
362b71e960f4b008064c9abff17907e7d33c4578 Publish image with latest tag upon push to master Pull request images should expire after 1 week
4a8343f9751418b5d7c2a87494a342fdebd408a0 Fix dockerfile due to go.mod changes
4b7a132397235b5cbc91a839c5ea0d460da1b602 Add 'Publish image to registry' step to the build gitaction
286a27380039bc93b6e0916244c42d1bfb02aed8 Use plain logrus instead of assisted-installer logutil Updated go.mod
e91607aa66284f2221d1f1defff9f9a7ba5cc7af Added go.mod inside the api dir
91fb13dc709f587376109f94c3dfd7ca98e3884c Extract ignition endpoint info from user-data and set on agent
a1bba483557dd86f11191b03f839ca210154421d Add clusterDeploymentRef to ACI spec when creating it
699783e9be40885be7c949fdbc1c6d3f9d2070a5 Look for existing clusterImageSet before trying to create it
e62061c103a2c05f1942348389cf06e0d1a7e6ac Added How to install section to the readme
cfe1dd1ae897f3887c61ef87a901199f5e54b20c Not finding agents should not be an error
4bba5a8b91a63a0b49c5b16fc3b86ccba879bea2 Check if agent is approved before using
e9bd3c809a34580fdcf9b4ada121e24ed7e7b16e Added logging for updateAgentStatus
90f9ecb598707a8d2dafd20f953952791225dee9 use assisted-installer logutil in AgentMachineReconciler
308495d6218412777d895dcb6a797dbd0cb88f01 Added agent, clusters and machines to clusterrole
869918ad8fadf4be9a435e9ab1c4a5a0ec98c407 Added capi to scheme
db781b6f7e7b985af24626f457f9ac2f123ddd56 Get clusterImageSet using ImageSetRef.Name requeue when creating clusterImageSet
cfa46f08fab6cc86a4a41ff5e22bcdc69498829b Set ClusterDeploymentRef.Namespace when creating the clusterDeployment
ca074ff8f00cfc72c2a409de7a50573caf655f0e Added clusterdeployment, clusterimagesets and agents to clusterrole
9597a43df763b7b3bafccd74da9cbabe4d8197d3 Add relevant APIs to client scheme
d5c525573d904e05bb3a4f36218e8475e954a867 Initialize AgentClusterReconciler in main.go
977b7857e1ead0a4b3a4b560f58ea261b9a72629 Added commonLabels to kustomization.yaml
e5c0a233ac01cfb8337b8940d72c8d0d42a2bd06 Use plain logrus instead of assisted-installer logutil Initialize AgentMachineReconciler logger
993460b216ca21f09b252565d60588c717997155 Updated generated agentcluster crd
bf12694014e98b6b8a980dda1a9c3b2fcd3b3d1e Updated agentCluster spec to have releaseImage instead of imageSetRef The agentCluster will create or update a clusterImageSet according to the releaseImage
5a75c30cd1774c4e6e5b2c31b11cea0a2d9ae062 AgentMachine unit tests
9c9999daca61b3ee107c4e7c157fbbb28deb5fdd Added agentclusters and agentmachinetemplates to kustomization.yaml
4a34b1a543cc5c74d3ab08f796283abb414a8731 Added build workflow
1e361eadbbf7651a88ff1ec197fb4c382f49d912 Removed bin/ from git
102c303d6fa270221975489e466d27f4f783bb2b Added agentmachine_controller_test
2217d3ce3ff06c07b77973728dedb4ec1bf41552 Finish first pass of AgentMachine controller
3d850884f893f7f59c1e0c69d60f3692b3162711 Added UTs
8bfc05cdce1c5cee89bd77236ab21f4f5772d7b7 Added basic UT agentcluster_controller_test
c1ba7923a3056ed7db591dc5914b53530f01aaaa Updtaed logging
1ef5b7465a7f6c35068cd579832207fb7d7c7c43 Added basic reconcile functionality to agentcluster controller
bb26966adce0ded618d6499d02904448ad9c7b60 First pass of controllers
1a36c3eaf41d3c37ec53e3bd67ff797ef24d1a67 Merge pull request #1 from eranco74/avishay/apis-first-pass
c485b763db25bc22aee4d798c2acbda3282bccb3 First pass on API
2ab3ca6bfcbc407a969ff7ab6cd9484c9765a988 Generated code using the operator-sdk ``` operator-sdk init --domain agent-install.openshift.io --repo github.com/eranco74/cluster-api-provider-agent operator-sdk create api --group capi-provider --version v1alpha1 --kind AgentMachine --resource --controller ```
9c11535f0eaa14d8a71159ec1ba23f8f4a118646 Initial commit
```

Status: Fast-forwarded successfully.
