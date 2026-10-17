# Project governance and release model

## Maintainer control

The official repository is maintained by `YaoMang`. The maintainer controls
roadmap, releases, accepted contributions, and merges. A public LGPL license
protects downstream recipients' freedoms but does not confer merge access to
this official repository.

External pull requests require a separately executed broad-relicensing CLA
before merge. This requirement **does not apply to independent forks**.

## Development source and public release

Development takes place first in a **separate private source repository**.
This public repository receives selected, reviewed **content snapshots** as
new commits; it is not an automated Git mirror. The private source and any
unreleased code remain proprietary unless separately licensed.

Public releases must not contain private Git history, secrets, internal
configuration, unapproved files, or proprietary vendor SDK material.
Maintainers check license provenance and tests before each public release.

## Initial compatibility scope

FAIRINO FR5, Python SDK release `v2.2.8_robot_v3.9.8`, controller v3.9.8
are the initial engineering targets, **not yet a tested support claim**.
The interfaces should be extensible to new SDK versions/vendors as needs arise.

## Merge protection

The CODEOWNERS file requests maintainer code review. It **does not itself**
enforce required review, CLA completion, or branch protection. GitHub
rulesets / branch protections and CLA verification must be enabled separately.
