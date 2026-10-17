# Public-only-from-pre-public release checklist

No public `main` merge may bypass the pre-public approval gate.

1. Obtain an **approved** pre-public candidate commit SHA, allowlisted file
   inventory, rights/attribution review, test output, and file hashes.
2. Confirm candidate changes contain no confidential proprietary code,
   secrets, vendor SDK bundles, device secrets, sensitive logs, or private
   Git history. Check independent buildability and honest safety claims.
3. Create a **new branch inside this public repository** from current
   public `main`, populated by a **content-only export** of that exact
   pre-public candidate; a separate private repository cannot usually
   be a direct public PR head.
4. Match exported content hashes against the approved pre-public snapshot.
   Review deletions and renames as well as added and changed files.
5. Open a maintainer-controlled PR. Record pre-public commit SHA and
   release review identifier; apply required approval, provenance and CI
   checks **once configured**. Do not merge directly from a fork PR or by
   unreviewed direct pushes.
6. After successful review, merge PR, then tag/release from public `main`.
7. Retain provenance and public SHA in the private internal release log.

No production promotion credentials, required checks, or protected-branch
rules are configured by this document alone.
