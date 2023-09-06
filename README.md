# DiveScript

Lightweight, flexible Rust dialect that compiles to its own bytecode.

> Work-in-progress

Getting started:

- [Overview](https://divescript.github.io/overview)
- [Reference](https://divescript.github.io/reference)

## Terminal usage

```sh
divescript new hello-world
divescript build
divescript run
```

## Package manager

The `divescript` terminal command is a package manager itself.

- Dependencies in the registry are qualified and organized by platform through using the scheme prefix `scheme:`. For example, `ue:com.a.lib`. The manifest of a package must always define `platform = "platform"`. Packages of different platforms cannot be used at the same time.
- Package names in the manifest may contain one or more dots typically following the convention `com.author.package`.
- Everyone can upload a package to the registry, however it must be reviewed by the team if it is the first time it is published.