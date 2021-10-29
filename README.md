# rust-templates

[![CI](https://github.com/bengreenier/rust-templates/actions/workflows/ci.yml/badge.svg)](https://github.com/bengreenier/rust-templates/actions/workflows/ci.yml)

Templates for creating rust projects with a GitHub-managed lifecycle with cargo-generate. 🏗️📃

What you get:

- PR build validation using `cargo`. ⚙️
- Automated Release PR generation using [release-please](https://github.com/googleapis/release-please). 🚢
- Automated crates.io publishing (after merging a Release PR). 🦀
- [Dependabot](https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/about-dependabot-version-updates) automated dependency update PR generation. 🎁
- A [toolchain file](https://rust-lang.github.io/rustup/overrides.html#the-toolchain-file) for automatic rust toolchain configuration. 🏗️
- A `justfile` for common developer actions - for use with the excellent [just command runner](https://github.com/casey/just). 🧑‍💻
- The [MIT License](https://mit-license.org/). 📝

## Quickstart

> First make sure you've done: `cargo install cargo-generate`.

### basic

> Use this template for basic rust projects. E.g. A single crate binary or lib, a workspace with a root crate.

```
cargo generate bengreenier/rust-templates.git basic
```

### Others

Coming soon - [Suggest a template](https://github.com/bengreenier/rust-templates/issues/new).

## Configuration

### For publishing to crates.io:

- Create an API access token [here](https://crates.io/me).
- Add it as a [GitHub repository secret](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository) named `CARGO_REGISTRY_TOKEN`.
- `.github/release.yml` will use this secret when publishing a release.

### Favorites

If you use these templates repeatedly, be sure to [favorite them](https://crates.io/crates/cargo-generate#favorites) for quicker access!

## Supporting the project

If this project saved you some time, and you'd like to see it continue to be invested in, consider [buying me a coffee. ☕](https://www.buymeacoffee.com/bengreenier)

Also, the setup here is largely inspired by [Amos' post: My ideal Rust workflow](https://fasterthanli.me/articles/my-ideal-rust-workflow) consider [supporting them too](https://www.patreon.com/fasterthanlime).
