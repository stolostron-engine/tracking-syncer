## Syncing stolostron/managed-serviceaccount with stolostron-engine/managed-serviceaccount

## Status Summary:

backplane-2.1 -> backplane-2.1: Synced commits but not tags.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Synced commits but not tags.  

### Branch backplane-2.1 -> backplane-2.1:

New commits (first branch sync):

```
d33100a327e7b5a36516fcdec30aacf1b2cc82c4 Merge pull request #14 from nathanweatherly/cherry-pick-manager-image-pull-secret
e45ef863ea13c2580ab66674613a58da56849906 removing unused import
b3af2977d419e93569ae22fdf72b3bcceb24a42e Signed-off-by: Nathan Weatherly nweather@redhat.com
88b085dab99d1f779f401b16b9e44f7c9d5b9f3e Update OWNERS (#13)
06614707d035296693dd4c6730793243f21e471c typo fix and description review (#31) (#11)
24b8fe33e8bd663fb2378f862382cbe39ffd485f Merge pull request #10 from nathanweatherly/cherry-pick-mar-10
6641ce202566139a6b0bd9e7084751ad40401a6b renaming crd and adding make target line to copy generated crd every time (#28)
90251d309ff6ab2660c34dbb369195bc725869ab feat: fail fast if managed SA CRD absent in the hub (#27)
8729e6c4514c842003b5efd8ecc4059489a0c619 Merge pull request #9 from hanqiuzh/cherry-pick-03-09
8db4c9e9cb3b65bd2f99c5bb23f516fc38607ba6 add test to validate deletion of managedserviceaccount (#21)
211ae4be62a84401a058e1a51f20d8d3a119527e add demo script for ephemeral-identity feature (#25)
be6aafdcdb620bd80365a3281158179810c7e99e chore: converge on klog (#26)
375e42235a3b5c8a4165c7b9d37ac6c225b7f69e fixes chart image tag to v0.1.1 (#24)
40cab598d53a50d98f493fb782f1a88c66e99b49 bump chart v0.1.1 (#23)
a068b4f6911ce35dfa859d143a71b673ff51353f add e2e for ephemeral-identity (#22)
c9f415ff1b5ff15c0ba73d41d9ee31e5dc296026 validate generated token via TokenReview (#20)
7581621573b062da41d637ce36020b178322d99e update default value of agent-image-name org to open-cluster-management (#12)
0d01c1091c447b040072e504be275f982b72178f adding permission for deleting of managed-serviceaccount (#19)
0122922236c56d30507803045e247b695c79d6e9 e2e: follow-up (#13)
3403be59664e2561045bc49e4a83c38239e29800 update owners (#7)
8af9699e8a41c8cf557df915d1ad030c389f5984 Merge pull request #6 from hanqiuzh/cherry-pick-branch
1cc1cb2948b662ae544f683a8f80a9404eaa68b8 add EphemeralIdentity alpha feature (#18)
605c87989a17a89a87e2d77b4819004dd28a5bf9 delete serviceaccount when managed-serviceaccount is deleted (#17)
de3ecc2884e9c29ae85be580ab3f42ff9153eafb switch health lease to primarily managed cluster side (#16)
9860a33e0dd869246a2fa4b4ae10d79d7874639d update owners
a5e95f8951063bb9b045519555aca22d82ce7bdb provide option to configure agent install strategy (#10)
d890d518692213c2743cb93c6b73deef7935cb9e e2e: init (#7)
741d9c369e6822c98591c91b9fe86e571d44a5e5 update Dockerfile to use UBI based image (#11)
e13224eea41553a21b0ae3954a24bae7f889901a adding managedclusteraddons/finalizers to clusterrole (#8)
1b7b95842be561d1521584cfcf3cd7b21a7a5cd2 bump v0.1.0 for helm charts (#6)
120d39f927b0e42bd3f3e735ed41b18af37d1468 fixes gh action release (#5)
04dbb2ce4bb1b194c379d387128d376bf15db2fe gh-action: release (#4)
aee5d643e8b11bc3795cf241670868b16de4d951 makefile: fixes image registry (#3)
cc5279928b8157eb7587907874efaf5de3aef7d3 gh-action: post submit (#2)
75324b5575e04aee469fa6b0e44d2a3af51a1754 Chore: gh-action pre-submit (#1)
a625686761e0c3ca253e13ad6e636a02c649d97a chore: convering manager/agent image
2af08f464fb4034bd8baeaa217ea2d62c4385f32 doc: adding prerequisite
730e259c9be1c2af9a6e9c9e8cf794d0c1cecf19 chore: filling README doc
f1e5b430a132f9a4e182afe86e3032c66fe7d0c7 persisting tokens to secrets
42c4aa4147123978b85d31bda6c1044cfd636c42 updates helm charts
4054c45146ce8cbbf67246206acc726bec78bcd0 minor fixes
04bf4dfd3be1e1a62d9d0e8ec1a93ed488111754 minor fixes
37e6b98d75e8de46a736a5369e939804b5d7d3e9 healthiness updater
54da82689ff29ae829cde2334644e4c56e01c536 bump v0.0.24
b16ffbc48d056a2efc575861748d0b2c6a117d46 initial implementation
81af19cf105b26e46961ac7c9e4d5d348c2f664c adding dockerfiles
66070b49587130ecb7ad03b8a5f2d6d9e6f98ef8 init implmentation
31e30f6ad5e0fee146e299ea74d9d6861e2d0d79 Initial commit
```

Status: Synced commits but not tags

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits (first branch sync):

```
d33100a327e7b5a36516fcdec30aacf1b2cc82c4 Merge pull request #14 from nathanweatherly/cherry-pick-manager-image-pull-secret
e45ef863ea13c2580ab66674613a58da56849906 removing unused import
b3af2977d419e93569ae22fdf72b3bcceb24a42e Signed-off-by: Nathan Weatherly nweather@redhat.com
88b085dab99d1f779f401b16b9e44f7c9d5b9f3e Update OWNERS (#13)
06614707d035296693dd4c6730793243f21e471c typo fix and description review (#31) (#11)
24b8fe33e8bd663fb2378f862382cbe39ffd485f Merge pull request #10 from nathanweatherly/cherry-pick-mar-10
6641ce202566139a6b0bd9e7084751ad40401a6b renaming crd and adding make target line to copy generated crd every time (#28)
90251d309ff6ab2660c34dbb369195bc725869ab feat: fail fast if managed SA CRD absent in the hub (#27)
8729e6c4514c842003b5efd8ecc4059489a0c619 Merge pull request #9 from hanqiuzh/cherry-pick-03-09
8db4c9e9cb3b65bd2f99c5bb23f516fc38607ba6 add test to validate deletion of managedserviceaccount (#21)
211ae4be62a84401a058e1a51f20d8d3a119527e add demo script for ephemeral-identity feature (#25)
be6aafdcdb620bd80365a3281158179810c7e99e chore: converge on klog (#26)
375e42235a3b5c8a4165c7b9d37ac6c225b7f69e fixes chart image tag to v0.1.1 (#24)
40cab598d53a50d98f493fb782f1a88c66e99b49 bump chart v0.1.1 (#23)
a068b4f6911ce35dfa859d143a71b673ff51353f add e2e for ephemeral-identity (#22)
c9f415ff1b5ff15c0ba73d41d9ee31e5dc296026 validate generated token via TokenReview (#20)
7581621573b062da41d637ce36020b178322d99e update default value of agent-image-name org to open-cluster-management (#12)
0d01c1091c447b040072e504be275f982b72178f adding permission for deleting of managed-serviceaccount (#19)
0122922236c56d30507803045e247b695c79d6e9 e2e: follow-up (#13)
3403be59664e2561045bc49e4a83c38239e29800 update owners (#7)
8af9699e8a41c8cf557df915d1ad030c389f5984 Merge pull request #6 from hanqiuzh/cherry-pick-branch
1cc1cb2948b662ae544f683a8f80a9404eaa68b8 add EphemeralIdentity alpha feature (#18)
605c87989a17a89a87e2d77b4819004dd28a5bf9 delete serviceaccount when managed-serviceaccount is deleted (#17)
de3ecc2884e9c29ae85be580ab3f42ff9153eafb switch health lease to primarily managed cluster side (#16)
9860a33e0dd869246a2fa4b4ae10d79d7874639d update owners
a5e95f8951063bb9b045519555aca22d82ce7bdb provide option to configure agent install strategy (#10)
d890d518692213c2743cb93c6b73deef7935cb9e e2e: init (#7)
741d9c369e6822c98591c91b9fe86e571d44a5e5 update Dockerfile to use UBI based image (#11)
e13224eea41553a21b0ae3954a24bae7f889901a adding managedclusteraddons/finalizers to clusterrole (#8)
1b7b95842be561d1521584cfcf3cd7b21a7a5cd2 bump v0.1.0 for helm charts (#6)
120d39f927b0e42bd3f3e735ed41b18af37d1468 fixes gh action release (#5)
04dbb2ce4bb1b194c379d387128d376bf15db2fe gh-action: release (#4)
aee5d643e8b11bc3795cf241670868b16de4d951 makefile: fixes image registry (#3)
cc5279928b8157eb7587907874efaf5de3aef7d3 gh-action: post submit (#2)
75324b5575e04aee469fa6b0e44d2a3af51a1754 Chore: gh-action pre-submit (#1)
a625686761e0c3ca253e13ad6e636a02c649d97a chore: convering manager/agent image
2af08f464fb4034bd8baeaa217ea2d62c4385f32 doc: adding prerequisite
730e259c9be1c2af9a6e9c9e8cf794d0c1cecf19 chore: filling README doc
f1e5b430a132f9a4e182afe86e3032c66fe7d0c7 persisting tokens to secrets
42c4aa4147123978b85d31bda6c1044cfd636c42 updates helm charts
4054c45146ce8cbbf67246206acc726bec78bcd0 minor fixes
04bf4dfd3be1e1a62d9d0e8ec1a93ed488111754 minor fixes
37e6b98d75e8de46a736a5369e939804b5d7d3e9 healthiness updater
54da82689ff29ae829cde2334644e4c56e01c536 bump v0.0.24
b16ffbc48d056a2efc575861748d0b2c6a117d46 initial implementation
81af19cf105b26e46961ac7c9e4d5d348c2f664c adding dockerfiles
66070b49587130ecb7ad03b8a5f2d6d9e6f98ef8 init implmentation
31e30f6ad5e0fee146e299ea74d9d6861e2d0d79 Initial commit
```

Status: Synced commits but not tags
