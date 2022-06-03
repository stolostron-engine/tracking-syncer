## Syncing stolostron/clusterclaims-controller with stolostron-engine/clusterclaims-controller

## Status Summary:

backplane-2.1 -> backplane-2.1: Synced commits but not tags.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Synced commits but not tags.  

### Branch backplane-2.1 -> backplane-2.1:

New commits (first branch sync):

```
7652834aa6a6258307468cbad59c642d7d05bb28 trigger new build (#43)
113df5955c44756d2b8831c468568254df7cd590 add update rbac for managed cluster (#42)
5ad46f4689a5d002b41d33219b7dd606dcc39f1c use kubeclient to replace controller runtime (#40)
c49c8ff14468d4bab2876f08ba197175782d3033 add lease permission (#39)
4656e6c89724dd1d84f5fc06404bce4869ff9856 upgrade go lib (#38)
c4881bfe0880f4070a4c54ccb708434c766a6205 fix the missing annotation if claim is not in cluster ns (#37)
6c87c2cbaa8c3d96ed21770d74ccab3be893803d should not depend on klusterlet addon config in MCE (#35)
e8af08e8578a29a98848877c3d0083aa54681215 add provisioner annotation (#34)
3d735eb2b6a82de8b981f398ea9d7ebfae5cdb63 upgrade hive api (#32)
f3cd3e96365ab47a4537fedd1a5f7c165fdf1c14 maintain the cluster name label by import controller (#27)
3f70e595c73ac88fd18917a8fe9714370844a2f2 No-Op PR (#26)
5b082ae259bcc503761e93637d980a63e4450c10 fix go 17 (#24)
26452f724b0bdc2a724e0d32bc452c6b31f1395f upgrade go to 1.17 (#22)
bef7efe572cce8b6dec5c93026f1ee15edde7a83 rename org (#20)
4009b16ddb7c3d1bca9fb156caf87ed4a665d3e0 update owners (#17)
d9a95e93ef2a17a06137a5ba5fa2be36966351c9 do not delete pool namespace (#15)
a6368354a1d5f9fc4523858c7b3a9f3a9c338fbc Make sure we only import once and then leave the rest to the Console (#16)
11a318c9d7eab8e582e9bc2b94d1e7d3b6ad57f7 Fix incorrect domain (#14)
23f36f78e55f1f540404e2a3c5a0fae40c619414 Fix when secrets are nil or missing (#13)
ac662d5655e2f825f109f8b99ce095343d4eda81 add clusterset when create managedcluster (#12)
7e402dc601aa5fcd64fa66e6d99f0f946cecbc10 Add region label to ManagedCluster when available (#9)
0e603fb56e7ff843620f2325c4c9a5d6ab3c0241 add cloud label for managedcluster (#10)
b3bf191953bcd7b28efd6ab35e4b3696b26cf0e6 fix invalid memory address (#11)
317f2b8802056d5330904500b8f91b97c93f7abb Add annotation open-cluster-management.io/createmanagedcluster: true/… (#8)
280a2e731edf955020ce4e8806c3c237f8a30a2e rebuild (#7)
6049fd8bd7031ccc54a9f8735ee6a8f52a3b1b29 Add additional role verbs, enhanced log messages, and extra instructi… (#6)
fc4b4c9108f1cd85fedb28016697ee73065b4710 Two more small Sonar vulnerabilities (#5)
7b3a8a9c17663ae2c0e6413306c0d5e8cfe3a92b Clean up the sonar code smells (#4)
f0acdf906dfbc57c96f9bfff74c77cfd367dba69 Update rebuild.md
712c4b8403de353c7152463b787cdf4b033ffd35 Update rebuild.md
0b76e19206cd11a9a212e13627c4423dcb7cf959 Create rebuild.md
4032773c85f3f568a767be916177444b425256bf Update OWNERS
927f729be8e5b18c2183d53523cf15dd0a3227f8 Update OWNERS
9b5112486de24e7cdeb2b05fd23a99483ac13cb5 Improve how labels are copied. Include vendor & name (#3)
94bb354a462c708415ed42dbb1b2a736d8259aa1 Add a clusterPools delete controller (#2)
1faeac696b064598d6e0a3c5389528946aac3ba2 Add label transfer from clusterClaims to managedClusters
dff792be76e6fe28afb330625685ffd2b5bd9bab Update readme with better example steps
38466ca98068b8ce2ad587529c2df8ac8549ed33 Update readme with better example steps
87a099b2f3e3f3f1f2963c2e34fbc32c004bcf7e Improve the log messaging around finalizers as this takes a couple of loops to complete the delete
e28bc3074b0aa19ccb9ba1572cb730588e1b70a5 Skip delete, when already deleting
7651288a18044365dca6efd2b7adf29bbd764486 Final tweaks to get the controller working
adc6aebe81589ccee5968efb7e4bbf2991585110 Update package
8b06e45eb3a741d3cfcdb10f1f49fa3ee7b9ceaf Initial commit
48434be1a3f8545ff019433b8db696f7dc87d2b9 Initial commit
```

Status: Synced commits but not tags

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits (first branch sync):

```
7652834aa6a6258307468cbad59c642d7d05bb28 trigger new build (#43)
113df5955c44756d2b8831c468568254df7cd590 add update rbac for managed cluster (#42)
5ad46f4689a5d002b41d33219b7dd606dcc39f1c use kubeclient to replace controller runtime (#40)
c49c8ff14468d4bab2876f08ba197175782d3033 add lease permission (#39)
4656e6c89724dd1d84f5fc06404bce4869ff9856 upgrade go lib (#38)
c4881bfe0880f4070a4c54ccb708434c766a6205 fix the missing annotation if claim is not in cluster ns (#37)
6c87c2cbaa8c3d96ed21770d74ccab3be893803d should not depend on klusterlet addon config in MCE (#35)
e8af08e8578a29a98848877c3d0083aa54681215 add provisioner annotation (#34)
3d735eb2b6a82de8b981f398ea9d7ebfae5cdb63 upgrade hive api (#32)
f3cd3e96365ab47a4537fedd1a5f7c165fdf1c14 maintain the cluster name label by import controller (#27)
3f70e595c73ac88fd18917a8fe9714370844a2f2 No-Op PR (#26)
5b082ae259bcc503761e93637d980a63e4450c10 fix go 17 (#24)
26452f724b0bdc2a724e0d32bc452c6b31f1395f upgrade go to 1.17 (#22)
bef7efe572cce8b6dec5c93026f1ee15edde7a83 rename org (#20)
4009b16ddb7c3d1bca9fb156caf87ed4a665d3e0 update owners (#17)
d9a95e93ef2a17a06137a5ba5fa2be36966351c9 do not delete pool namespace (#15)
a6368354a1d5f9fc4523858c7b3a9f3a9c338fbc Make sure we only import once and then leave the rest to the Console (#16)
11a318c9d7eab8e582e9bc2b94d1e7d3b6ad57f7 Fix incorrect domain (#14)
23f36f78e55f1f540404e2a3c5a0fae40c619414 Fix when secrets are nil or missing (#13)
ac662d5655e2f825f109f8b99ce095343d4eda81 add clusterset when create managedcluster (#12)
7e402dc601aa5fcd64fa66e6d99f0f946cecbc10 Add region label to ManagedCluster when available (#9)
0e603fb56e7ff843620f2325c4c9a5d6ab3c0241 add cloud label for managedcluster (#10)
b3bf191953bcd7b28efd6ab35e4b3696b26cf0e6 fix invalid memory address (#11)
317f2b8802056d5330904500b8f91b97c93f7abb Add annotation open-cluster-management.io/createmanagedcluster: true/… (#8)
280a2e731edf955020ce4e8806c3c237f8a30a2e rebuild (#7)
6049fd8bd7031ccc54a9f8735ee6a8f52a3b1b29 Add additional role verbs, enhanced log messages, and extra instructi… (#6)
fc4b4c9108f1cd85fedb28016697ee73065b4710 Two more small Sonar vulnerabilities (#5)
7b3a8a9c17663ae2c0e6413306c0d5e8cfe3a92b Clean up the sonar code smells (#4)
f0acdf906dfbc57c96f9bfff74c77cfd367dba69 Update rebuild.md
712c4b8403de353c7152463b787cdf4b033ffd35 Update rebuild.md
0b76e19206cd11a9a212e13627c4423dcb7cf959 Create rebuild.md
4032773c85f3f568a767be916177444b425256bf Update OWNERS
927f729be8e5b18c2183d53523cf15dd0a3227f8 Update OWNERS
9b5112486de24e7cdeb2b05fd23a99483ac13cb5 Improve how labels are copied. Include vendor & name (#3)
94bb354a462c708415ed42dbb1b2a736d8259aa1 Add a clusterPools delete controller (#2)
1faeac696b064598d6e0a3c5389528946aac3ba2 Add label transfer from clusterClaims to managedClusters
dff792be76e6fe28afb330625685ffd2b5bd9bab Update readme with better example steps
38466ca98068b8ce2ad587529c2df8ac8549ed33 Update readme with better example steps
87a099b2f3e3f3f1f2963c2e34fbc32c004bcf7e Improve the log messaging around finalizers as this takes a couple of loops to complete the delete
e28bc3074b0aa19ccb9ba1572cb730588e1b70a5 Skip delete, when already deleting
7651288a18044365dca6efd2b7adf29bbd764486 Final tweaks to get the controller working
adc6aebe81589ccee5968efb7e4bbf2991585110 Update package
8b06e45eb3a741d3cfcdb10f1f49fa3ee7b9ceaf Initial commit
48434be1a3f8545ff019433b8db696f7dc87d2b9 Initial commit
```

Status: Synced commits but not tags
