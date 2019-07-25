# Anthos Config Management Demo Base

A repo to serve as a base for [Anthos Config
Management](https://cloud.google.com/anthos-config-management/) demo scripts
that move a git repo through a series of update. the approach is to sequence the
changes you want to demo as branches, e.g. gatekeeper-label-check-001,
gatekeeper-label-check-002, gatekeeper-label-check-003, etc. when actually doing
a demo, create a branch for the demo itself, ie osp-review-20190624, and
configure your nomos cluster to pull from it. then as you move through the
script, merge in the branches following the sequence suffix and push to your
demo branch. when your done, best practice would be to delete the demo specific
branch (ie osp-review-20190624) so it doesnt clutter the repository.

