# cargo-make-coverage-grcov

'cargo-make' makefile for grcov coverage.

## Install

get the file.

```shell
wget https://raw.githubusercontent.com/kazuk/cargo-make-coverage-grcov/main/coverage_grcov.makefile.toml
```

add `extend` for your top of `Makefile.toml` as bellow.

```toml
extend= [
  { path = "coverage_grcov.makefile.toml" }
]

[tasks.coverage]
alias="coverage_grcov"

```

## Usage

```shell
cargo make coverage
```

 coverage result placed on `target/lcov.info`
