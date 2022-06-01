# tracking-syncer

Perhaps one way to describe the Stolostron Engine project is that it represents 
an aggregation and integration effort. It brings togther a collection of foundational
cluster-management-related projects, plus some Stolostron-Engine provided added
goodness to produce a singe integrated and easy-to-install offering 
from these pieces.

In that context, this repo exists to host aautomation that facilitates this aggregation.
It hosts GitHub ACtion-based automtion that periodically synhronizes a set of those external-to,
and thus upstream-of, Stolostron Engine source repos with Stolostron Engine's downstream 
tracking counterparts that live within the `solostron-engine` GitHub organization.
This is done to "stage" the contributions from the upstream repos for assembly into the 
oerall Stolostron Engine offering.

To make it easier to identify these tracking repos as such,  we have established the convention
of using names of the form `tracking-<upstream-repo>` where the `<upstream-repo>` part indicates
the upstream repo's GitHub orgnzization and repo name.
To further reinforce the intended purpose of these repos in `stolostron-engine`, they will not
have  a `main` or `master` branch to hopefully discourage any PRs or commits directly to them.
All updates to these tracking repos should occur only as a result of automated syncing with
their upstrem counterparts.

The tooling that this repo's workflows use lives in the `stolostron/tracking-tools` repo.

