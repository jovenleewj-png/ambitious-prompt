# Maintaining Ambitious Prompt

For significant changes to skill behavior, capabilities, approval flow, compatibility, or rights notices:

- Add a user-facing entry under `Unreleased` in CHANGELOG.md, explaining the change and any migration or reinstallation needed.
- Preserve existing release entries. Group minor copy edits rather than releasing for every commit.
- Before a release, move the pending notes into a dated version section and set `metadata.version` in SKILL.md to the same version.
- Use MAJOR for incompatible workflow changes, MINOR for compatible capabilities, and PATCH for fixes.
- Validate the skill and verify the changed behavior as appropriate. Keep the tag and notes tied to the actual shipped commit.
- When publishing a release is authorized, push an annotated `vMAJOR.MINOR.PATCH` tag. The release workflow publishes that section of CHANGELOG.md and an installable ZIP on GitHub Releases. Verify the workflow succeeds before reporting a release as published.

Keep biography and licensing changes grounded in Joven’s instructions. Do not restore the removed MIT license or invent a reuse grant.

Use LinkedIn for creator and contact links. Keep personal website references out of the skill, documentation, release notes, and downloadable packages.
