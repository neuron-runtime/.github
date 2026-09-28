# .github

[![Markdown lint](https://github.com/neuron-runtime/.github/actions/workflows/markdown.yml/badge.svg)](https://github.com/neuron-runtime/.github/actions/workflows/markdown.yml)

Community health files and templates for the [Neuron](https://github.com/neuron-runtime) organization.

## About Neuron

Neuron is a language-agnostic runtime for composing and operating software capabilities.

At the center of Neuron is the **Neuron Assembly Protocol**: a language-neutral representation of
capabilities, their contracts, configuration, and composition. SDKs are language-specific frontends
that produce the protocol representation; N.O.R.E. — Neuron Operational Runtime Engine — operates
that representation through the available Capability Runtimes.

The definition language never becomes part of the runtime model, and neither does the implementation
language. The protocol is the boundary.

Read the full overview in the [organization profile](profile/README.md).

## What lives here

These files apply to every repository in this organization that does not define its own version.

| File | Applies to |
| --- | --- |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contributors to any Neuron repository |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | Everyone participating in the community |
| [SECURITY.md](SECURITY.md) | Reporting a vulnerability in any Neuron repository |
| [SUPPORT.md](SUPPORT.md) | Getting help with any Neuron repository |
| [.github/ISSUE_TEMPLATE](.github/ISSUE_TEMPLATE) | New issues in any Neuron repository |
| [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) | New pull requests in any Neuron repository |

Repository-level concerns stay in the repository. Build commands, test suites, and code layout
belong in each project's own `README.md` and `CONTRIBUTING.md`, which override the defaults here.

## Working on this repository

This repository holds only Markdown and YAML, so the only automated check is a Markdown lint:

```shell
npx markdownlint-cli2 "**/*.md"
```

Keep additions focused. If a default is wrong for the whole organization, change it here. If it is
wrong for one project, change it in that project.
