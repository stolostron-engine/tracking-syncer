## Syncing stolostron/managed-serviceaccount with stolostron-engine/managed-serviceaccount

## Status Summary:

backplane-2.1 -> backplane-2.1: Already in sync.  
backplane-2.0 -> backplane-2.0: Already in sync.  
main -> main: Picked up 65 new commits.  

### Branch backplane-2.1 -> backplane-2.1:

Branches are already in sync, nothing to do.

### Branch backplane-2.0 -> backplane-2.0:

Branches are already in sync, nothing to do.

### Branch main -> main:

New commits:

```
9b3eb46728d8d41a7f521500dae33b6e5058a417 Merge branch 'open-cluster-management-io:main' into main
01b32ef2ae558592dbd315d4d1d20a15b1d673ad update addon-framework (#58)
2a662f319bc2e2981fcba3d6178199dac6d47f45 use fine grained rbac for addon (#57)
2ebb47b67877d57b8bbaac99bf17db4334c09087 Fix: Quick restart container when hubconfig changed. (#55)
0d31ce1cf0f99d92b73c6fb030922b1f5c38d52f support addon deployment config (#54)
95bb35c8efa813976e10d895ad0699204649ee06 using addonfactory to build addon agent (#53)
9b3090d03d630bc2579854096d70bd19f0cd7c96 Bump go version to 1.19 (#51)
0a31bf857ac79eac6c1066840c05c5d293f9ad3e add more unit test cases (#50)
cc352f573aea1cfcdb38913f18c338082b623882 refreh token until remaining lifetime < 20% validity (#49)
0c4c772260a772d5f11ff929dc742b971c3f4ad0 upgrade golang to 1.18 and upgrade go modules (#48)
68f9c0ad942e1dca5afc91a8272f3575befd4400 homogenize chart version (#46)
a7b99d48783b31745c865c60781a2653a28bd437 fixes: makefile variable s/IMG_TAG/IMAGE_TAG/ (#45)
3dd454ef997904ac4efd394dad2ee81f721398bb remove microdnf directives (#44)
441d5a67f6d12192d3a576190e76c8ae360da446 fixes release workflow yaml format (#43)
76335cfe4da643d90a007c1c40b72203a173ae69 chore: update ocm helm chart registry in README (#42)
daca956e0cda056f2bf2b3a40283aaa08b070db5 s/image/images/ in Makefile (#41)
b3c5e6cdd3b7d394924a005fb034170cacc921f6 add agent-image-pull-secret param to manager (#40)
c9d0ea9f474f9b7d556b0e8efb38eed99fd15cdf fix minior go-staticcheck issue (#39)
de6a7b7b5be89d6a05cc2fd4f5c855e543cbbc29 generated client (#38)
42c2a4c7a04fe4c75d5a8aa9f4e9793a9b36489c Replace dockerfile image (#37)
803375e3e0603bfc22774727c505834dfcff428b workflow: image multi-arch (#35)
1deea963b8c418b7f5e527fc62fd54a0dd984aca update chart version to v0.2.0 (#34)
30952e0201202e49cebdf7aa193d3e9f07d72293 Bump golang & addon framework: csr beta compatibility (#33)
c5c6a4113f4cd1cd8e3bc666457b4fb05f4dda90 fail fast if token-request no fonud in api-discovery (#32)
d6e2852f6c0fe64222e0a35d3ee689a12f7dec71 chart package action (#29)
b8d1b0bff9ef3d4a8c568069b93410a3b4917afe typo fix and description review (#31)
6c25aaf3c72c086b0cbeb170eabab3c124cb15df add error catches (#30)
1bab3a51ebf7d6d25510dd3363df2953bad41ca6 renaming crd and adding make target line to copy generated crd every time (#28)
55aaf9c83b18974b5affcb3ce6f4910e14a09d09 feat: fail fast if managed SA CRD absent in the hub (#27)
03bd185a05443c6e1c33a034849d0a1f7139b4cc add test to validate deletion of managedserviceaccount (#21)
f3a35bdfb48f8de0a8cd18832770b792558e10c5 add demo script for ephemeral-identity feature (#25)
a25e1e4793cfb22c911572733e53c262bee83b66 chore: converge on klog (#26)
162fc97b11f6b23d3be61928792cf55c774f8d24 fixes chart image tag to v0.1.1 (#24)
87f3aaaf9b673d889a4b58a028555fab56532c5d bump chart v0.1.1 (#23)
3dc5f97f99b71d4d7c079eee4e87ab8a597d06c8 add e2e for ephemeral-identity (#22)
f34e26e55344a2771f170c2faddbc3059ff905e9 validate generated token via TokenReview (#20)
eea6c2bed16c07349ce2c10d3af345cd60cb5893 update default value of agent-image-name org to open-cluster-management (#12)
e13a23f404a1f657fa45acef886d771b55856023 adding permission for deleting of managed-serviceaccount (#19)
62d6d396f604f8813a9dbc47ae62e4ab6907bd4a e2e: follow-up (#13)
8aa2ad025a4b7e9166c5236bb5405e0c5f1f7985 add EphemeralIdentity alpha feature (#18)
1f8d3a37c8e2689c44c5e67dece08590b120e594 delete serviceaccount when managed-serviceaccount is deleted (#17)
dae0a61acf8793bf58122ae84963309ffa005036 switch health lease to primarily managed cluster side (#16)
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

Status: Syncing successful
