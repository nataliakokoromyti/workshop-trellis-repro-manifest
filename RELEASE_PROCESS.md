# Release Process

This repository uses a tag-triggered GitHub Actions workflow to measure the
Tinfoil manifest and create the GitHub release.

Rules:

- Push the tag only.
- Do not create the GitHub release manually.
- Keep project-specific runtime knobs and debug settings out of this public
  repository.
- Inject secrets and private runtime configuration through private deployment
  channels only.
