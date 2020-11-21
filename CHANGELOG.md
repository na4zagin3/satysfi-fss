# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- Style keyword `font-set` to set a font set

### Removed
- `\font-set(<font-set>){ ... }` and `+font-set(<font-set>)< ... >` are removed in favor of 
  `\font-style[font-set <font-set>]{ ... }` and `+font-style[font-set <font-set>]< ... >`.

## [0.1.0]
### Added
- Style keywords `font-size` and `with-font-size`

### Changed
- Semantics of commands nested `+font-set` and `\font-set` are now undefined

## [0.0.1]
### Added
- Basic functionalities as a font selection scheme
- Japanese documentation

[Unreleased]: https://github.com/na4zagin3/satysfi-fss/compare/v0.0.1...HEAD
[0.0.1]: https://github.com/na4zagin3/satysfi-fss/tag/v0.0.1
[0.1.0]: https://github.com/na4zagin3/satysfi-fss/tag/v0.1.0

