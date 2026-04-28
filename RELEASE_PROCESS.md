# Release Process

This repository uses a tag-triggered GitHub Actions workflow to build the attestation and create the GitHub release.

Important rule:

- Push the tag only.
- Do not run `gh release create` manually.
- The workflow itself creates the release and attestation.

Why:

- Manually creating the release first causes the workflow to fail with:
  - `a release with the same tag name already exists`

Current examples:

- `v0.3.66` was pushed as a tag only.
- The workflow then created the release for that tag.
