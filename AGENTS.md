# AGENTS.md

Notes for maintainers and coding agents working on this repository.

## What this repository is

The organization's `.github` repository. GitHub uses its files as defaults for every
repository in podman-container-tools-community that has none of its own:

```
profile/README.md                    organization profile page
CONTRIBUTING.md                      contributing guide
CODE_OF_CONDUCT.md                   Code of Conduct
SECURITY.md                          security policy (private vulnerability reporting)
.github/ISSUE_TEMPLATE/              issue forms and their chooser configuration
.github/pull_request_template.md     pull request template
```

The build repositories,
[skopeo](https://github.com/podman-container-tools-community/skopeo),
[buildah](https://github.com/podman-container-tools-community/buildah) and
[podman](https://github.com/podman-container-tools-community/podman), each have their
own `AGENTS.md` with their build, tests, release workflows and rules. Nothing here is
built or released.

## Rules

- Work through pull requests; never push to `main`. Sign off every commit
  (`git commit -s`) for the DCO.
- Text here applies to all three tools. Keep it in line with the READMEs of the build
  repositories (trust model, supported platforms, where to report what), and change
  those together when the facts change.
- The organization is an independent community effort, not upstream: keep the notice
  that it is not affiliated with or supported by the upstream maintainers.
- The Code of Conduct contact is [@jkroepke](https://github.com/jkroepke).
