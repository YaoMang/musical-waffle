# Robot Motion Control — public edition

A Python robot-motion control library under development. The official public
repository contains only source snapshots that have passed a separate,
maintainer-controlled pre-public review process.

## Status and scope

**Pre-implementation.** No hardware-control functionality has been released
or verified yet. Initial planned target: **FAIRINO FR5**, **FAIRINO Python
SDK v2.2.8**, controller **v3.9.8**. Interfaces may later support other
SDK versions and robot vendors, without committing to implementations now.

The future library will be usable independently of sar-acq, which is only
one potential downstream application.

## Publication model

```text
Private development → Private pre-public review → Public release PR → Public main
```

**Only exact snapshots approved by the pre-public review gate may be merged
into public main.** The maintainers do not directly merge external/fork PRs to
public main. External proposals can be considered for inclusion through
the private development and pre-public review process.

The public PR uses an internal promotion branch carrying source *contents*
from the approved private pre-public snapshot; private commit history is
never published. GitHub branch protections and automated verification are
not yet configured, so this is presently a documented maintainer policy.

See [governance](docs/governance.md), [releasing](docs/releasing.md),
and [contributing](CONTRIBUTING.md).

## License

Original published code is **GNU LGPL-3.0-or-later**; see [LICENSE](LICENSE).
The LGPL license does not automatically cover unpublished proprietary source.
The FAIRINO SDK is a separate project licensed under **Apache-2.0**, and is
not bundled here; see [THIRD_PARTY.md](THIRD_PARTY.md).

## Safety

Physical robot motion can injure people or damage equipment. Follow manufacturer
instructions, qualified risk assessment, hardware protective measures and
emergency-stop procedures. No real-world motion control has been validated in
this initial repository state.
