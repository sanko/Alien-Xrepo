# Changelog

All notable changes to Alien::Xrepo will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- `Alien::Xrepo::MB` and `Alien::Xrepo::MM`, generic Module::Build and ExtUtils::MakeMaker integrations for Alien distributions
- Build engine `share_dir` option: per-package installs land under `<share>/<pkg>` via `installdir`, and the snapshot records share-relative paths so an installed dist resolves packages after relocation to the site sharedir.
- Example distributions demonstrating the three recipe shapes:
  - `Exotic-SDL3` (shared libraries for FFI consumers (FFI::Platypus and Affix), and Inline::C),
  - `Exotic-Ninja`: binary tool shipped in `bin_dir`
  - `Exotic-Zlib`: static library for `cc_lib_flags` consumers (Inline::C)
  - `Exotic-Zstandard` and `Exotic-Lsquic` demonstrate `Alien::Xrepo::MB`
  - `Exotic-Raylib6` example distribution on the MM harness
  -`Exotic-SQLite3` example (currently not working...)
- Recipe `version` pinning

## [v1.0.0] - 2026-09-07

Splitting this out of the `Alien::Xmake` dist and repo

### Changed

- It exists? Check the Alien::Xmake changelog, I guess

[Unreleased]: https://github.com/sanko/Alien-Xrepo/compare/v1.0.0...HEAD
[v1.0.0]: https://github.com/sanko/Alien-Xrepo/releases/tag/v1.0.0
