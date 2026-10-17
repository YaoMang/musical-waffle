# Governance and release provenance

## Official repository control

The `YaoMang` maintainer determines roadmap, accepted contributions,
licensing of its own code, and official public releases. LGPL licenses allow
others to use, modify, and fork public code; they do not confer a right
to merge into the official repository.

## Three-stage repository model

1. **Primary private development source**: code development and proprietary
   internals; private history and unreleased modules stay private.
2. **Private pre-public gate**: only explicitly selected, publishable source
   content is staged; provenance, license, security, tests, and safety claims
   are reviewed.
3. **Official public distribution**: only an approved pre-public content
   snapshot is imported into a promotion branch, reviewed through a public
   PR, and merged into `main`.

No private repository history, vendor SDK bundles, or confidential files
should be present in public releases. Pre-public is an approval source,
not an automatic synchronization mirror.

A direct public fork PR is not merged as-is, even after signing a CLA.
Approved external contributions first enter the private development
source under sufficient additional licensing rights, then pass through
pre-public and the normal release process.

## Technical enforcement state

`CODEOWNERS` and written policies do **not** prevent direct pushes,
unreviewed merges, or unapproved PR sources. GitHub branch protection /
rulesets and **required trusted promotion-provenance validation** must
be added and tested separately. The intended validation must compare
approved source identity and content hashes, not only branch names or
a self-declared provenance file. Public GitHub Actions tokens do not
automatically have read access to a separate private pre-public repo.

Until enforcement is activated, maintainers must enforce this policy
manually and must not claim that source gating is automated.

## Initial technical scope

FAIRINO FR5 / SDK `v2.2.8_robot_v3.9.8` / controller v3.9.8.
Support is planned, not yet physically tested.
