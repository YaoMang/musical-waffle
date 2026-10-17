## Promotion-only PR

**Public main accepts only approved content from the private pre-public gate.**
Direct external/fork PRs are proposals only and cannot merge as-is.

### Approved pre-public source

- Pre-public approved commit SHA:
- Candidate / review record:
- Approved file allowlist and SHA-256/Git blob hashes:
- Public branch diff review:

### Required release checks

- [ ] Maintainer has verified approval of this exact pre-public snapshot
- [ ] Export contains only approved content; private history was not copied
- [ ] Public content digests match the approved candidate
- [ ] LGPL/third-party license notices and external contribution CLA verified
- [ ] Secret/privacy scan and standalone build/tests completed or exceptions documented
- [ ] Hardware-motion safety claims are supported by real test evidence
- [ ] Maintainer review and repository protections satisfied

**These self-declarations are not technical verification.** Required trusted
provenance CI and public-main protections remain to be implemented.
