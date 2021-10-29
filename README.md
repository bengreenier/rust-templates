# rust-templates

Templates for creating rust projects with a GitHub-managed lifecycle with cargo-generate. 🏗️📃

What you get:

- PR build validation
- Automated Release PR generation using [release-please](https://github.com/googleapis/release-please)
- Automated crates.io publishing (after merging a Release PR)

## Quickstart

> First make sure you've done: `cargo install cargo-generate`.

### Prerequisites

For publishing to crates.io:

- Create an API access token [here](https://crates.io/me)
- Add it as a [GitHub repository secret](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository) named `CARGO_REGISTRY_TOKEN`
- `.github/release.yml` will use this secret when publishing a release

### single-crate

> Use this template for single crate repositories.

```
cargo generate bengreenier/rust-templates.git single-crate
```

### workspace

> Use this template for [rust workspace](https://doc.rust-lang.org/cargo/reference/workspaces.html) projects that will produce multiple crates.

```
cargo generate bengreenier/rust-templates.git workspace
```

## Favorites

If you use these templates repeatedly, be sure to [favorite them](https://crates.io/crates/cargo-generate#favorites) for quicker access!

## Supporting the project

If this project saved you some time, and you'd like to see it continue to be invested in, consider [buying me a coffee. ☕](https://www.buymeacoffee.com/bengreenier)
