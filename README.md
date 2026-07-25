# Kin Form

> [!WARNING]
> This project is deprecated and no longer maintained. The "Kin Form" name
> and logo now belong to a new, framework-agnostic successor at
> [github.com/jolleekin/kin-form](https://github.com/jolleekin/kin-form).
> This repository will remain available, read-only, as `kin-form-lit`.

<p align="center">
<img src="website/src/favicon.svg" width="128" height="128" alt="Kin Form" />
</p>

A fast, flexible, and type-safe form management library for [Lit].

## Monorepo

This monorepo contains three packages

| Package                | Description                                                 |
| ---------------------- | ----------------------------------------------------------- |
| [form](./form)         | The primary user-facing package                             |
| [examples](./examples) | Example applications that demonstrate the power of Kin Form |
| [website](./website)   | The documentation website                                   |

## Developer setup: Git hooks

This repository includes a `.githooks/pre-commit` hook that runs the test suite for the `form` package (`deno test` in `form/`). Git doesn't enable custom hooks automatically; to enable them locally run:

```sh
git config core.hooksPath .githooks
```

Once configured, each commit will run the `form` tests and abort the commit if tests fail. This helps prevent regressions from being committed.

[Lit]: https://lit.dev
[Lume]: https://lume.land/
