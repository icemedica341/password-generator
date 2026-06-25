# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

No unreleased changes yet.

## [0.7.0] - 2026-05-15

### Added

- Terminal demo SVGs (password, passphrase, quit) with centered title bar

### Changed

- Reorganize README with screenshots in relevant sections, center title
- Simplify `.gitignore` to project-specific entries (remove template boilerplate)
- Update LICENSE for icemedica341
- Replace `random` with `secrets` for cryptographically secure password generation
- Format README title for consistency

## [0.6.0] - 2024-05-02

### Added

- Bandit security linting workflow

### Changed

- Change `WORDS` list to tuple for better constant semantics

## [0.5.0] - 2024-04-29

### Added

- Type annotations for `QUIT_COMMANDS` in `constants.py`

### Changed

- Revert type annotations for constants (not enforceable in Python)
- Indent quit statement for improved readability
- Uncomment actual password generation statement, remove debugging print

## [0.4.0] - 2024-04-28

### Added

- Ruff as the project formatter (compatible with Black)
- Brackets to distinguish functions from variables in code
- Extended docstring descriptions for `main()` entry points
- `LEARNT.md` extracted from `README.md` remarks section

### Changed

- Comprehensive refactor of input handling: simplified `my_input` wrapper, raise `QuitCommand` exception instead of breaking
- Add quotation marks to quitting options for enhanced readability
- Reorganize README: move Constants and Exceptions descriptions before Password Generator section, keep Password Generator first as the entry point
- Format all markdown files consistently
- Add spaces after function docstrings
- Improve heading formatting across documentation
- Move Tests section after Password Generator in README

### Removed

- Unnecessary `if __name__ == '__main__'` guards from `password_generation.py`

## [0.3.0] - 2024-04-23

### Changed

- Refactor `handle_quit()`: move `quit_commands` list to `constants.py` as `QUIT_COMMANDS`
- Minor code line adjustments for clarity

### Fixed

- Ignore profiling files (`.prof`, `.pyprof`) via `.gitignore`
- Ignore `.ruff_cache` directory via `.gitignore`

## [0.2.0] - 2024-04-20

### Added

- "Getting Started" section header to README for improved onboarding
- Notice on how to get started using the password generator

### Fixed

- Import error for custom exception class
- Remove incorrectly formatted "contains" words from README

## [0.1.0] - 2024-04-13

### Added

- Initial password generator implementation:
  - Password and passphrase generation via `password_generation.py`
  - CLI interface via `project.py` with menu-driven interaction
  - Custom exception hierarchy in `exceptions.py` (`QuitCommand`, `PasswordGenerationError`)
  - Constants file (`constants.py`) with word lists and configuration
  - Test suite (`test_password_generation.py`)
  - Project dependencies (`requirements.txt`)
  - README with usage documentation
  - License (MIT)
  - `.gitignore` for Python project
- Organised import sorting across all modules
- Gap spacing between constants for readability

[Unreleased]: https://github.com/icemedica341/Password-Generator/compare/v0.7.0...HEAD
[0.7.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.7.0
[0.6.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.6.0
[0.5.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.5.0
[0.4.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.4.0
[0.3.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.3.0
[0.2.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.2.0
[0.1.0]: https://github.com/icemedica341/Password-Generator/releases/tag/v0.1.0
