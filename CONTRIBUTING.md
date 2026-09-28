# Contributing to Neuron

Thank you for your interest in Neuron. This guide applies to every repository in the
[neuron-runtime](https://github.com/neuron-runtime) organization.

Neuron is a language-agnostic runtime. Contributions that strengthen the Neuron Assembly Protocol, the
N.O.R.E. runtime, or the SDKs are all in scope, regardless of the language they are written in.

## Before you start

- **Search first.** Check the repository's issues and discussions, and linked issues, to see whether
  the work is already planned or in progress.
- **Open an issue first** for anything beyond a small fix. Design discussion is much cheaper before
  code is written, especially for protocol-level changes.
- **For a significant protocol change**, describe the change and its compatibility impact in an issue
  before you start. Protocol changes are expensive to unwind.

## Reporting bugs

Use the **Bug report** issue template. A good report includes the repository, the version or commit,
the SDK and language, the runtime in use, and steps to reproduce.

Do not use public issues for security vulnerabilities. Follow [SECURITY.md](SECURITY.md).

## Development workflow

1. Fork the repository and create a branch off the default branch.
2. Make your change. Keep it focused: one logical change per pull request.
3. Add or update tests for the behaviour you changed.
4. Update documentation when you change a public API, a configuration option, or a protocol field.
5. Open a pull request using the [pull request template](.github/PULL_REQUEST_TEMPLATE.md).

### Branch naming

Use a short, descriptive name prefixed by the kind of change:

```text
feat/assembly-composition
fix/process-runtime-cleanup
docs/protocol-overview
refactor/capability-registry
chore/ci-dependencies
```

### Commit messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```text
<type>(<optional scope>): <short summary>
```

Common types: `feat`, `fix`, `docs`, `refactor`, `test`, `perf`, `chore`.

```text
feat(sdk): add version constraint validation to capability manifests
fix(core): resolve capability runtime before container teardown
docs(protocol): document composition conflict rules
```

Use the imperative mood in the summary. Explain the reasoning in the body when it is not obvious.

### Sign-off

Sign off every commit so the Developer Certificate of Origin applies:

```shell
git commit -s -m "fix(sdk): validate capability name against the reserved prefix list"
```

## Pull requests

- Target the default branch unless the maintainers have asked otherwise.
- Link the issue the pull request resolves, using `Fixes #123` when it fully resolves it.
- Explain what changed and why. Reviewers read for the reason first.
- Fill in the checklist in the pull request template.
- Keep unrelated cleanups, formatting, and renames out of the pull request. They make the review
  harder and slow down the merge.
- CI must pass before a review. Push follow-up commits rather than force-pushing during review, so
  reviewers can see what changed.
- Respond to review comments. A pull request is a conversation, not a handoff.

## Code style

Follow the conventions already in the repository you are working in. Consistency with the surrounding
code matters more than a personal preference.

General expectations across Neuron:

- Match the existing formatting configuration rather than introducing a new formatter.
- Public APIs, protocol fields, and configuration keys are documented. Comments explain why, not what.
- Error messages say what failed and what the caller can do next.
- Do not add a dependency to solve a problem that plain code already solves.
- Avoid unrelated refactors in a change that is meant to be small.

## Licensing

Contributions are accepted under the license of the repository you contribute to. By submitting a
pull request you confirm that you have the right to license your contribution, and that it is your
original work or properly attributed.

## Code of Conduct

Participation in this project is governed by [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md). By
contributing you agree to uphold it, and you are expected to help enforce it.
