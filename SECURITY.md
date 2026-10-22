# Security Policy

This organization builds and distributes community releases of Podman, Buildah and Skopeo.
It is **not** the upstream project, so where you report depends on what is affected.

## Vulnerabilities in Podman, Buildah or Skopeo

If the issue is in the tools' source code, it affects official builds too. Report it to upstream
following the [upstream Security and Disclosure Policy](https://github.com/podman-container-tools/container-libs/blob/main/SECURITY.md).
We pick up the fix automatically once upstream publishes a release.

## Vulnerabilities in our builds

Report it to us if the issue is specific to our distribution, for example:

- our build configuration, GitHub Actions workflows or release process,
- the signing or attestation of our releases,
- the base image or packaging of our container images, deb and rpm packages,
- a Go toolchain or dependency issue that only affects our builds.

Please report it privately through
**[GitHub private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)**
in the affected repository (Security → Report a vulnerability). Do not open a public issue.

<!-- TODO(Joe): enable private vulnerability reporting on skopeo, buildah and podman
     (Settings → Code security), and optionally add an e-mail contact here. -->

This is a volunteer effort. We aim to acknowledge reports within a week, but cannot promise
response times.

## Supported versions

We build every upstream release covered by each repository's README. Fixes are delivered by
rebuilding the affected releases; we do not patch upstream source.
