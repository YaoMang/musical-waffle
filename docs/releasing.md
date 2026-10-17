# Public release checklist

1. Receive a **selected content-only snapshot** from the private development
   source; never copy the private Git history.
2. Review the exact public diff and all provenance, third-party licenses,
   notices, secrets, device-specific configuration, and internal paths.
3. Confirm release code can build and function without unreleased proprietary
   source. Verify tests and document any hardware verification limitations.
4. Verify all external contributions have been properly licensed and accepted
   with the required CLA before incorporation into the private source.
5. Update CHANGELOG/release notes and choose version/tag only when functionality
   is ready; avoid implying FR5 hardware validation without real tests.
6. Review through a maintainer-controlled PR before merging to protected main.
7. Record cross-repository provenance in internal records, without exposing
   sensitive private revision details unnecessarily.

This file establishes a policy, not an automated release pipeline.
