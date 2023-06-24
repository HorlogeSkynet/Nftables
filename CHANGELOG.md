# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- `storage.type.set-element-counter.nftables` scope for set elements
- `string.unquoted.{counter,limit,quota}-unit.nftables` scopes for bytes and packets counter/limit/quota units
- nftables 1.0.7 features :
	* `destroy` script command

### Fixed
- `mbytes` pattern matching
- TCP MSS rule in syntax tests

## [v2.1.0] - 2022-10-27
### Fixed
- CHANGELOG v2.0.1 anchor link
- Windows line termination support
- Rename `storage.type.ct-expecation.nftables` to `storage.type.ct-expectation.nftables` (typo)

### Changed
- Exclude syntax test files from package
- Relax `first_line_match` REGEXP to match a wider set of shebangs
- Stop capturing end-of-lines characters in `statement-separators`
- Simplify some REGEXPs by avoiding unnecessary word-boundaries and escapes

## [v2.0.1] - 2022-04-30
### Fixed
- `ct status { ... }` usages
- Rule statements matched in `set`
- Sublime Text "All Syntaxes" build command conflict with GitHub Actions workflow

## [v2.0.0] - 2022-04-05
### Added
- CI using GitHub Actions
- `limit` objects
- Named `quota` objects
- `symhash` operator
- Network address ranges
- `devices` in `chain` objects definitions
- `add`, `update` and `delete` rule statements
- `keyword.operator.word` and `meta.path` scopes honoring
- nftables 0.9.1 features :
	* `tproxy` verdict
	* `dynamic` flag in `set`
- nftables 0.9.2 feature :
	* `ct expectation` and `ct timeout` objects
- nftables 0.9.3 feature :
	* `secmark` objects
	* `synproxy` objects
- nftables 0.9.4 features :
	* `typeof` keyword in `set`
	* `lshift` and `rshift` operators
- nftables 0.9.5 feature :
	* Elements `counter` in `set` and `flowtable`
- nftables 0.9.7 features :
	* `comment` in `set`
	* Implicit chains (using `jump`)
	* `device` assignment to constant for `ingress` hooks
- nftables 0.9.9 features :
	* Bits checking
	* Wildcard (`*`) in `set`
	* `owner` flag for `table` objects
	* `offload` flag for `flowtable` objects
- nftables 1.0.1 features :
	* `egress` hook

### Fixed
- Anonymous `quota` objects
- `devices` assignment to constant

### Changed
- `*.helper.nftables` scopes renamed to `*.ct-helper.nftables`
- `constant.numeric.integer.signed.nftables` scope renamed to `constant.numeric.integer.decimal.nftables`

### Removed
- Unquoted strings matching in `set`

## [v1.3.0] - 2021-08-30
### Added
- Explicit support for Sublime Text 4
- Chain `priority` constant keywords (nftables >= 0.9.6)

## [v1.2.3] - 2021-05-28
### Changed
- Test cases improvements

### Removed
- `remove` script command (unavailable upstream)

## [v1.2.2] - 2021-04-26
- `comment` statement for `rule`

## [v1.2.1] - 2020-11-18
### Added
- `dormant` flag for `table` objects

## [v1.2.0] - 2020-09-25
### Added
- Comment toggling through key binding

## [v1.1.1] - 2020-03-25
### Fixed
- Matching when rules contain `type` literal

## [v1.1.0] - 2020-03-16
### Added
- `ingress` hook
- IPv4 and IPv6 subnets

### Changed
- Minor optimizations

### Fixed
- Stack management issues
- Line continuation issue

## [v1.0.0] - 2020-03-01
### Added
- Extensive tests suite
- Complex named `set` declarations matching

### Changed
- Various improvements

## [v0.6.0] - 2020-02-29
### Added
- Verdicts highlighting in `set` objects

### Changed
- Various improvements

## [v0.5.0] - 2020-02-26
### Added
- Package now available through Package Control

### Changed
- Various improvements

## [v0.4.0] - 2020-02-23
### Added
- MAC addresses matching
- Network families usage in commands

### Changed
- Various improvements

### Removed
- Single-quoted strings (unsupported upstream)

## [v0.3.0] - 2020-02-22
### Added
- `+` and `-` arithmetic operators
- `handle` and `position` in rule commands
- Compatibility with new Sublime Text optimized REGEXP engine (>= 3103)

### Changed
- Various improvements

### Fixed
- Glitches related to `status [sd]nat` matching

## [v0.2.0] - 2020-02-20
### Added
- `ct helper` stateful object
- `numgen` and `jhash` operators

### Changed
- Various improvements

### Fixed
- Line continuation
- Integers range scoping
- Basic `table` declarations

## [v0.1.1] - 2020-02-20
### Changed
- Various improvements

## [v0.1.0] - 2020-02-18
### Added
- Initial version

[Unreleased]: https://github.com/HorlogeSkynet/Nftables/compare/v2.1.0...HEAD
[v2.1.0]: https://github.com/HorlogeSkynet/Nftables/compare/v2.0.1...v2.1.0
[v2.0.1]: https://github.com/HorlogeSkynet/Nftables/compare/v2.0.0...v2.0.1
[v2.0.0]: https://github.com/HorlogeSkynet/Nftables/compare/v1.3.0...v2.0.0
[v1.3.0]: https://github.com/HorlogeSkynet/Nftables/compare/v1.2.3...v1.3.0
[v1.2.3]: https://github.com/HorlogeSkynet/Nftables/compare/v1.2.2...v1.2.3
[v1.2.2]: https://github.com/HorlogeSkynet/Nftables/compare/v1.2.1...v1.2.2
[v1.2.1]: https://github.com/HorlogeSkynet/Nftables/compare/v1.2.0...v1.2.1
[v1.2.0]: https://github.com/HorlogeSkynet/Nftables/compare/v1.1.1...v1.2.0
[v1.1.1]: https://github.com/HorlogeSkynet/Nftables/compare/v1.1.0...v1.1.1
[v1.1.0]: https://github.com/HorlogeSkynet/Nftables/compare/v1.0.0...v1.1.0
[v1.0.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.6.0...v1.0.0
[v0.6.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.5.0...v0.6.0
[v0.5.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.4.0...v0.5.0
[v0.4.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.3.0...v0.4.0
[v0.3.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.2.0...v0.3.0
[v0.2.0]: https://github.com/HorlogeSkynet/Nftables/compare/v0.1.1...v0.2.0
[v0.1.1]: https://github.com/HorlogeSkynet/Nftables/compare/v0.1.0...v0.1.1
[v0.1.0]: https://github.com/HorlogeSkynet/Nftables/releases/tag/v0.1.0
