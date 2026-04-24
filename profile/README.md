## 🎮 Mod Loaders

| Repository                | Description                                                    | Language |
| ------------------------- | -------------------------------------------------------------- | -------- |
| [Reloaded-II]             | Universal .NET modding framework for native x86/x64 games      | C#       |
| [Reloaded3][Reloaded-III] | [WIP] Design specification for the next generation of Reloaded | Rust     |

## 📦 Core Libraries / C#

Reusable libraries for hooking, injection, memory manipulation, and more. Used by Reloaded-II and standalone projects.

| Repository                | Description                                                                                               |
| ------------------------- | --------------------------------------------------------------------------------------------------------- |
| [Reloaded.Hooks]          | Advanced native function hooks for x86/x64: detours and API hooking                                       |
| [Reloaded.Injector]       | DLL injection: inject x86 DLLs into x86 processes from an x64 host                                        |
| [Reloaded.Memory.SigScan] | High-performance byte pattern / PE signature scanner (5000+ MB/s/core, 30000+ with AVX)                   |
| [Reloaded.Memory]         | Managed, high-performance memory manipulation with an easy-to-use API                                     |
| [Reloaded.Assembler]      | .NET wrapper around Flat Assembler (FASM) for x86/x64                                                     |
| [Reloaded.Memory.Buffers] | Efficient shared concurrent unmanaged memory storage with fixed, stable addresses across runs (C# & Rust) |

## 🦀 Core Libraries / Rust

Next-generation Rust rewrites and new libraries.

| Repository          | Description                                   |
| ------------------- | --------------------------------------------- |
| [Reloaded.Hooks-rs] | [WIP] `no_std` Rust rewrite of Reloaded.Hooks |

## 🔌 Reloaded-II Mods & Extensions

Mods bundled with Reloaded-II.

| Repository                                 | Description                                                                          |
| ------------------------------------------ | ------------------------------------------------------------------------------------ |
| [reloaded.universal.redirector]            | Redirects game file reads to mod files, replacing assets without modifying originals |
| [Reloaded.Universal.DInputPleaseCooperate] | Fix DirectInput blocking screenshots                                                 |

## ⚙️ DevOps & CI Actions

Reusable GitHub Actions for Rust, .NET, and docs. Not specific to Reloaded. All MIT licensed.

| Repository                          | Description                                                                                     |
| ----------------------------------- | ----------------------------------------------------------------------------------------------- |
| [devops-mkdocs]                     | Build & publish MkDocs Material sites                                                           |
| [devops-publish-action]             | Publish artifacts to GitHub Releases & package repos                                            |
| [devops-changelog]                  | Build & publish automated changelogs                                                            |
| [devops-rust-test-and-coverage]     | Rust test + coverage with cross-compilation support                                             |
| [devops-rust-test-in-latest-wine]   | Test Rust projects using Wine                                                                   |
| [devops-rust-lightweight-binary]    | Build & cross-compile lightweight `no_std` Rust binaries with Profile-Guided Optimization (PGO) |
| [devops-rust-cbindgen]              | Generate C/C++ bindings from Rust via `cbindgen`                                                |
| [devops-rust-c-library-to-dotnet]   | Build C# wrapper for Rust library via `csbindgen`                                               |
| [devops-cargo-semver-checks-action] | Cargo semver checks with built-in checkout, caching & filtering                                 |

## 🏗️ Infrastructure

Shared data and supporting services for Reloaded-II.

| Repository           | Description                                           |
| -------------------- | ----------------------------------------------------- |
| [Reloaded-II.Index]  | Mod search index and backup source for mod updates    |
| [Reloaded.Community] | Community sourced game configurations for Reloaded-II |

## 🛠️ Config & Templates

Shared configs, templates, and style resources.

| Repository                          | Description                                                                      |
| ----------------------------------- | -------------------------------------------------------------------------------- |
| [Reloaded.MkDocsMaterial.Themes.R2] | MkDocs Material theme matching Reloaded-II & Reloaded3's style                   |
| [reloaded-templates-rust]           | Common project configs for cross-platform Rust development                       |
| [Reloaded.Project.Configurations]   | .NET project template: editor configs, NuGet settings, code style, license files |
| [License]                           | License documentation for the project                                            |

## 🔧 Misc & Examples

Demos, examples, and smaller utilities.

| Repository                | Description                                                      |
| ------------------------- | ---------------------------------------------------------------- |
| [Reloaded.Core.Bootstrap] | Demo: inject CoreCLR (.NET runtime) into unmanaged processes     |
| [Reloaded.Messaging]      | Extensible event-like messaging over LiteNetLib (local & remote) |

## 📁 Archived

These repos are no longer maintained but preserved for reference.

| Repository                     | Description                                                 | Superseded By                     |
| ------------------------------ | ----------------------------------------------------------- | --------------------------------- |
| [reloaded.universal.steamhook] | Prevent Steam from restarting game when launched externally | Built into Reloaded-II            | - |
| [devops-rust-test-in-wine]     | Test Rust in Wine on Linux                                  | [devops-rust-test-in-latest-wine] |

---

## 🤝 Contributing

Each repository has its own contribution guidelines; check its issue tracker or `CONTRIBUTING.md` for details.

## 📄 Licensing

Licensing varies by repository:

- **Mod loaders** (Reloaded-II): [GPL-3.0][Reloaded-II-license]
- **Core libraries**: [LGPL-3.0][Reloaded.Hooks-license] or MIT (see individual repos)
- **DevOps actions & config**: MIT

See the [License] repo for full details.

[Reloaded-II]: https://github.com/Reloaded-Project/Reloaded-II
[Reloaded-III]: https://github.com/Reloaded-Project/Reloaded-III
[Reloaded.Hooks]: https://github.com/Reloaded-Project/Reloaded.Hooks
[Reloaded.Injector]: https://github.com/Reloaded-Project/Reloaded.Injector
[Reloaded.Memory.SigScan]: https://github.com/Reloaded-Project/Reloaded.Memory.SigScan
[Reloaded.Memory]: https://github.com/Reloaded-Project/Reloaded.Memory
[Reloaded.Assembler]: https://github.com/Reloaded-Project/Reloaded.Assembler
[Reloaded.Memory.Buffers]: https://github.com/Reloaded-Project/Reloaded.Memory.Buffers
[Reloaded.Hooks-rs]: https://github.com/Reloaded-Project/Reloaded.Hooks-rs
[reloaded.universal.redirector]: https://github.com/Reloaded-Project/reloaded.universal.redirector
[Reloaded.Universal.DInputPleaseCooperate]: https://github.com/Reloaded-Project/Reloaded.Universal.DInputPleaseCooperate
[devops-mkdocs]: https://github.com/Reloaded-Project/devops-mkdocs
[devops-publish-action]: https://github.com/Reloaded-Project/devops-publish-action
[devops-changelog]: https://github.com/Reloaded-Project/devops-changelog
[devops-rust-test-and-coverage]: https://github.com/Reloaded-Project/devops-rust-test-and-coverage
[devops-rust-test-in-latest-wine]: https://github.com/Reloaded-Project/devops-rust-test-in-latest-wine
[devops-rust-lightweight-binary]: https://github.com/Reloaded-Project/devops-rust-lightweight-binary
[devops-rust-cbindgen]: https://github.com/Reloaded-Project/devops-rust-cbindgen
[devops-rust-c-library-to-dotnet]: https://github.com/Reloaded-Project/devops-rust-c-library-to-dotnet
[devops-cargo-semver-checks-action]: https://github.com/Reloaded-Project/devops-cargo-semver-checks-action
[Reloaded-II.Index]: https://github.com/Reloaded-Project/Reloaded-II.Index
[Reloaded.Community]: https://github.com/Reloaded-Project/Reloaded.Community
[Reloaded.MkDocsMaterial.Themes.R2]: https://github.com/Reloaded-Project/Reloaded.MkDocsMaterial.Themes.R2
[reloaded-templates-rust]: https://github.com/Reloaded-Project/reloaded-templates-rust
[Reloaded.Project.Configurations]: https://github.com/Reloaded-Project/Reloaded.Project.Configurations
[License]: https://github.com/Reloaded-Project/License
[Reloaded.Core.Bootstrap]: https://github.com/Reloaded-Project/Reloaded.Core.Bootstrap
[Reloaded.Messaging]: https://github.com/Reloaded-Project/Reloaded.Messaging
[reloaded.universal.steamhook]: https://github.com/Reloaded-Project/reloaded.universal.steamhook
[devops-rust-test-in-wine]: https://github.com/Reloaded-Project/devops-rust-test-in-wine
[Reloaded-II-license]: https://github.com/Reloaded-Project/Reloaded-II/blob/master/LICENSE
[Reloaded.Hooks-license]: https://github.com/Reloaded-Project/Reloaded.Hooks/blob/master/LICENSE.md
