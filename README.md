# Commit Message Validation

This repository enforces Conventional Commit Messages using a GitHub Actions workflow. All commits pushed to the `main` branch are checked for compliance.

## Conventional Commit Format

Valid commit messages must follow this format:

```
<type>(<optional-scope>): <description>

```

Where:
- `<type>` is one of: `feat`, `fix`, `chore`, `docs`, `style`, `refactor`, `test`, `perf`
- `<optional-scope>` is optional and should be in parentheses, e.g., `(api)`
- There must be a colon `:` followed by a space
- `<description>` is a brief summary of the change

## Examples of Valid Commit Messages

- `feat: add user authentication`
- `fix(api): handle null values`
- `docs: update README`
- `refactor(core): simplify logic`
- `test: add unit tests for validator`
- `perf: improve query performance`

Commits that do not match this pattern will fail the workflow check.
