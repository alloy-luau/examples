# Alloy examples

One `.aly` file per feature of [Alloy](https://github.com/alloy-luau/alloy),
numbered in reading order, plus `test`, a small project with `alloy.toml`,
packages, and a Rojo layout.

The compiler's tests build every file here, so a change to the language
lands with an example, and an example that stops compiling fails CI in
the `alloy` repository. Check this repository out beside that one:

```sh
git clone https://github.com/alloy-luau/alloy crates
git clone https://github.com/alloy-luau/examples examples
cd crates && cargo test
```

`alloy build` in the `alloy` repository compiles these into its `build`
folder; `alloy fmt --check ../examples` holds them to the formatter.
