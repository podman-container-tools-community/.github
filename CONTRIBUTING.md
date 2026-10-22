# Contributing

Thanks for helping out! This organization only maintains **build and release configuration** for
community builds of Podman, Buildah and Skopeo. Changes to the tools themselves belong
[upstream](https://github.com/podman-container-tools).

## What we accept

- Fixes and improvements to the goreleaser configuration, Dockerfiles, packaging and workflows.
- Support for new platforms or architectures.
- Documentation fixes.
- Dependency updates (most are handled by Renovate).

We don't accept patches to upstream source code, or changes that build from anything other than
the unmodified upstream release. That rule is what makes our builds verifiable.

## How to contribute

1. Open an issue first for anything larger than a small fix, so we can agree on the approach.
2. Fork the repository and create a branch.
3. Sign off every commit (`git commit -s`) to certify the [Developer Certificate of Origin](https://developercertificate.org/).
4. Keep pull requests focused. Pull requests run a dry-run build, which has to pass.
5. Explain in the pull request what you changed and how you tested it.

## Reporting problems

- A problem with our binaries, images, packages or release process: open an issue in the matching
  repository.
- A bug in the tool itself: reproduce it with an official build and report it upstream.
- A security issue: see [SECURITY.md](SECURITY.md).

## Code of Conduct

Everyone taking part is expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).
