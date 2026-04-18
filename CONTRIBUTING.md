# Contributing to ask

## Ground Rules

- Keep dependencies to `curl` and `jq` only.
- Preserve POSIX-friendly Bash where possible.
- One focused change per pull request.

## Workflow

1. Fork the repository and clone your fork.
2. Create a feature branch: `git checkout -b my-feature`
3. Make your changes. Keep commits small and descriptive.
4. Test manually with at least one OpenAI-compatible provider.
5. Run `shellcheck ask` if you have it installed.
6. Push to your fork and open a pull request against `main`.

## Code Style

- Indent with 4 spaces.
- Use `set -euo pipefail` at the top of any new scripts.
- Quote all variable expansions: `"$var"`, not `$var`.
- Prefer `jq` over manual string manipulation for JSON.

## Commit Messages

Short imperative subject line, optional body:

Add support for custom temperature

Reads ASK_TEMPERATURE and passes it to the payload when set.

## Reporting Issues

Include: OS, Bash version (`bash --version`), exact command, and the error output (redact your API key).

