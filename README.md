# Robot Motion Control — public edition

A Python robot-motion control library under development. This repository hosts **selected open-source releases** from a private development source; it is **not** an automatic mirror.

## Status and scope

**Pre-implementation / initial repository setup.** No robot hardware control functionality has been released or verified yet.

The first planned target is the **FAIRINO FR5** with **FAIRINO Python SDK v2.2.8** (robot controller **v3.9.8**). We intend to keep the architecture open to other SDK versions and robot vendors, without claiming support before it has been implemented and tested.

Applications (including sar-acq) should be able to depend on this library without importing a vendor SDK directly. The precise public control API is not yet finalized.

## Licensing

Our original code **published in this repository** is licensed under **GNU LGPL version 3 or later**; see [LICENSE](LICENSE). Source code not published here is **not** made available or licensed by this repository.

The FAIRINO Python SDK is a separate upstream project under **Apache-2.0**; it is not bundled here. Obtain and license it separately if needed. See [third-party dependencies](THIRD_PARTY.md).

## Contributions

External pull requests require an executed, project-accepted **Contributor License Agreement** with broad outbound relicensing permissions, based on **Harmony CLA — Option Five**, before merge. **CLA signing and automated checks have not yet been configured**, so maintainers will not merge external PRs until that process is operational. Contributors retain their copyrights; third-party forks remain free to operate under the LGPL.

See [CONTRIBUTING.md](CONTRIBUTING.md) and [project governance](docs/governance.md). Maintainers decide whether to accept contributions into the official repository.

## Safety

Robot movement can cause injury or property damage. Examples and libraries here are not substitutes for manufacturer safety guidance, risk assessment, protective equipment, or a functional emergency stop. No hardware functionality has been validated at this initial stage.
