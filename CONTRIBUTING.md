# Contributing

Thanks for helping. This is the default guide for Compeller.ai repositories. A repo's own `README`, `CONTRIBUTING.md`, and `CLAUDE.md` take precedence over this file.

## Issues

- Search existing issues first.
- Use the bug report or feature request form and fill in every field that applies.
- One problem per issue.
- Security problems do not go in issues. See [SECURITY.md](SECURITY.md).

## Discuss large changes first

Open an issue before starting anything large: a new feature, a public API change, a new dependency, or a refactor across modules. Agreeing on the approach first saves a rejected pull request. Small fixes and docs changes can go straight to a pull request.

## Fork and branch

1. Fork the repo and create a branch from `main`.
2. Keep the branch focused on one change.
3. Rebase on `main` before opening the pull request if it has moved.

## Pull requests

- Fill in the pull request template.
- Say what changed, why, and how you tested it. For hardware features, name what you tested against (CDJs, mixer, DMX fixtures, Hue, WLED, NDI receivers).
- Update docs and the README when behavior changes.
- Add or update tests for the code you touch.
- Never commit secrets, private keys, private hostnames, or signing and notarization material.

## Rust repositories

These must pass before review:

```bash
cargo fmt --all -- --check
```

```bash
cargo clippy -- -D warnings
```

```bash
cargo test
```

Use the latest stable release of any crate you add or update, and do not call deprecated APIs.

## License

Contributions are licensed under the license of the repo you contribute to. That is MIT, Apache-2.0, or both, depending on the repo. Check its `LICENSE` file.
