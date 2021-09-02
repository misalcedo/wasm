# WASM
[![Build](https://github.com/misalcedo/wasm-ast/actions/workflows/build.yml/badge.svg)](https://github.com/misalcedo/wasm-ast/actions/workflows/build.yml)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
[![Crates.io Version](https://img.shields.io/crates/v/wasm-ast.svg)](https://crates.io/crates/wasm-ast)
[![Docs.rs Version](https://docs.rs/wasm-ast/badge.svg)](https://docs.rs/wasm-ast)

A Rust-native WebAssembly syntax model useful for generating, parsing, and emitting WebAssembly code.

## Design
WASM-AST is designed with minimal validation. The goal is to closely model the WASM syntax specification in order to allow valid and invalid abstract syntax trees.

## Usage
To use `wasm-ast`, first add this to your `Cargo.toml`:

```toml
[dependencies]
wasm-ast = "0.0.1"
```

Then, add this to your crate:

```rust
use wasm_ast::model::Module;

fn main() {
    // ...
}
```

## Examples

Create an empty WASM module:

```rust
use wasm_ast::model::Module;

fn main() {
    let builder = Module.builder();
    let module = builder.build();
}
```

# License

Licensed under Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or http://apache.org/licenses/LICENSE-2.0)

# Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be 
licensed as above, without any additional terms or conditions.
