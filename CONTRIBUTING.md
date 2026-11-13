# Contributing to Theoros

This guide applies to every repository unless a repository provides its own.

## Outside contributors

Thank you for your interest. Issues and discussions are welcome in every
repository. Pull requests to source-available repositories are accepted only
after you sign the [Contributor License Agreement](CLA.md). Pull requests to
`theoros-bench` follow the Apache License 2.0 inbound terms.

## Branches

- `main` is always releasable. It is protected: no direct pushes, no force pushes.
- Work happens on short-lived branches named `<type>/<short-description>`,
  for example `feat/int8-conv-kernel` or `fix/manifest-hash`.
- Rebase on `main` before asking for review. Keep branches under one week old.

## Commits

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <summary in imperative mood>
```

Types: `feat`, `fix`, `perf`, `refactor`, `test`, `docs`, `build`, `ci`, `chore`.
A breaking change adds `!` after the type and a `BREAKING CHANGE:` footer.

## Pull requests

1. Open a draft early. Mark it ready when CI is green.
2. Fill in the template, including the requirement IDs the change touches.
3. One approving review from a code owner is required. Two for anything that
   runs on a satellite (`theoros-edge`, `theoros-delivery`).
4. Squash merge. The PR title becomes the commit message.

## Versioning and releases

- Software follows [Semantic Versioning](https://semver.org/).
- Flight models are named `theorosnet-<tier>-<sensor>-v<major>.<minor>`,
  for example `theorosnet-base-sentinel2-l1c-v1.0`. Every release ships a
  model card.
- Releases are tagged `vX.Y.Z` from `main` with release notes.

## Requirements traceability

Every requirement has an ID with a repository prefix: `MOD-REQ`, `EDGE-REQ`,
`DEL-REQ`, `GND-REQ`. Reference it in the pull request and in the test that
verifies it. The traceability matrix lives in `theoros-docs`.

## Secrets and data

- Never commit credentials, keys or customer data. Use GitHub Actions secrets.
- Datasets live in object storage, not in git. Record their source and license
  in a dataset card.
- Large binaries use Git LFS.
