# Security Policy

Neuron is under active development. We take reports of security vulnerabilities seriously and
respond to them.

## Reporting a vulnerability

**Do not open a public issue for a security vulnerability.**

Report it through GitHub Security Advisories instead. On any repository in this organization, use
**Security** in the repository menu, then **Report a vulnerability**. If the repository does not
offer the form, use the organization's advisory page at
<https://github.com/neuron-runtime/.github/security/advisories/new>.

If private reporting is not enabled on a repository and you cannot open an advisory, open an issue
that contains only the repository name and a one-line summary with no technical detail, then wait
for a maintainer to contact you.

## What to include

- The repository and, where relevant, the component such as the Neuron Assembly Protocol, N.O.R.E.,
  or a specific SDK.
- A description of the issue and its impact.
- Steps to reproduce, or a proof of concept.
- Any suggested mitigation.

## Response expectations

These are targets, not guarantees.

| Stage | Target |
| --- | --- |
| Acknowledgement | 3 business days |
| Triage and severity assessment | 10 business days |
| Fix or mitigation plan | Agreed with the reporter |

We will keep you informed as the report progresses and will credit you in the advisory if you would
like to be credited.

## Supported versions

Security fixes land on the default branch. Older lines receive fixes only when the affected
component is still actively used and no replacement exists.

| Version | Supported |
| --- | --- |
| Default branch | Yes |
| Latest tagged release | Yes |
| Older tags | No |

## Scope

In scope: Neuron repositories, the Neuron Assembly Protocol and its reference implementations, and
N.O.R.E.

Out of scope: vulnerabilities in third-party dependencies, which should be reported to the
maintainer of that project. If you are unsure, report it anyway and we will route it.
