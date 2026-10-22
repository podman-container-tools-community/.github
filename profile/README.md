# Podman Container Tools — Community Builds

> [!IMPORTANT]
> This is **not** the official [Podman Container Tools](https://github.com/podman-container-tools) project.
> It is an independent, community-run effort that repackages unmodified upstream releases.
> It is not affiliated with, endorsed by, or supported by the upstream maintainers.

We publish **static binaries, packages and container images** of
[Podman](https://github.com/podman-container-tools/podman),
[Buildah](https://github.com/podman-container-tools/buildah) and
[Skopeo](https://github.com/podman-container-tools/skopeo) for environments where distribution
packages are missing or several releases behind, such as CI runners and minimal hosts.

## 🛠️ Our builds

| Tool | Repository | Image |
| --- | --- | --- |
| **Skopeo** | [podman-container-tools-community/skopeo](https://github.com/podman-container-tools-community/skopeo) | `ghcr.io/podman-container-tools-community/skopeo` |
| **Buildah** | [podman-container-tools-community/buildah](https://github.com/podman-container-tools-community/buildah) | `ghcr.io/podman-container-tools-community/buildah` |
| **Podman** | [podman-container-tools-community/podman](https://github.com/podman-container-tools-community/podman) | `ghcr.io/podman-container-tools-community/podman` |

<!-- TODO(Joe): mark Buildah and Podman as "work in progress" or remove the rows until their first release is out. -->

Each repository's README has install instructions, the supported platforms and the known
limitations of the static builds.

## 🔐 Trust model

Our repositories contain **only build configuration**. Nothing in them can change what is compiled.

- **Upstream source only.** Each release is built from the upstream release tag, fetched from the
  Go module proxy and verified against the Go checksum database (`sum.golang.org`) with
  [goreleaser verifiable builds](https://goreleaser.com/customization/builds/verifiable_builds/).
- **Built in public CI.** Releases are built only in GitHub Actions, never on a developer machine.
- **Signed and attested.** Checksums and images are signed keyless with
  [cosign](https://github.com/sigstore/cosign) through GitHub OIDC, and every released file gets a
  GitHub build provenance attestation.
- **Reproducible.** With the same Go version, anyone can rebuild bit-for-bit identical binaries.

Each repository's README shows how to verify a binary or an image.

## 👩‍💻 Where to go

- **A problem with our binaries, packages, images or release process:** open an issue in the
  matching repository here.
- **A bug in Podman, Buildah or Skopeo itself:** check first whether it also happens with an official
  build, then report it [upstream](https://github.com/podman-container-tools). Please don't send
  upstream maintainers bugs that only occur in our builds.
- **Contributing:** see [CONTRIBUTING.md](https://github.com/podman-container-tools-community/.github/blob/main/CONTRIBUTING.md).

## 🛡️ Security

See our [Security Policy](https://github.com/podman-container-tools-community/.github/blob/main/SECURITY.md).
Vulnerabilities in the tools themselves are handled by upstream under the
[upstream Security and Disclosure Policy](https://github.com/podman-container-tools/container-libs/blob/main/SECURITY.md).

---

<sub>Podman, Buildah and Skopeo are projects of
[Podman Container Tools](https://github.com/podman-container-tools), a CNCF Sandbox project.
All names belong to their respective owners.</sub>
