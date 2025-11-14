# rust_ci_experiments

[![crates.io](https://img.shields.io/crates/v/experimental_do_nothing_crate_please_look_away.svg)](https://crates.io/crates/experimental_do_nothing_crate_please_look_away)
[![ci](https://github.com/AlexAegis/rust_ci_experiments/actions/workflows/ci.yml/badge.svg)](https://github.com/AlexAegis/rust_ci_experiments/actions/workflows/ci.yml)

## Usage

## Development of this repository

This repository is using `cargo-make`, it will take care of installing all
required cargo extensions and rustup components used in this repository.

1. Run `scripts/setup.sh` (Or run `cargo install cargo-make`)
2. (Optional) Install the rest of the tooling/cargo extensions using
   `cargo make setup`

### Requirements

- [Git LFS](https://git-lfs.github.com/)
- [Latest Rust Stable](https://rustup.rs/)

### `cargo-make` tasks

- `cargo make all` to run everything that could make ci fail (Everything below)
- `cargo make build` to build all crates
- `cargo make test` to test all crates
- `cargo make format` to format all crates
- `cargo make lint` to lint all crates using `clippy` and `rustfmt`
- `cargo make book-build` to build the documentation boo
