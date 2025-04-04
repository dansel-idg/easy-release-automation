# Changelog

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Known Errors

### Added

### Changed

### Removed

### Fixed

- Use pinned image version ubuntu-22.04 otherwise latest version is used which leads to
  errors.

## [0.1.0] - 2024-10-03

### Added

- #1: Added CI testing pipeline.
- #13: Optimize Readme and add end-user guide
  - Add end-user guide
  - Add simple getting-started `getting-started-release-config-simple`
  - Add Github bug report template
- #7: Added CI-ERA-Self-Release pipeline
- Added daily CI scheduler
- Added pull request template

### Changed

- #4: add "./src/core" sub-folder for ERA-specific flow control to improve the overview of
  the ERA-module
- #13: Optimize Readme and add end-user guide
  - Rename getting_started to getting_started_developer
- #15: Cleanup and improve code quality
  - Use 'graphlib' module for the topological sort algorithm.
  - Add editable option for installing ERA via setup-era.sh script.
  - Add return codes to the command line interface.
- Prepare ERA for deploying to pypi
  - Fix MIT license identifier
  - Loose fixed dependencies in pyproject.toml otherwise dependencies issue might be occur if installed via pip install

### Fixed

- #2: add error handling for plugins, that are referenced in the release-config.yml, but are
  not installed (+ tests).
- #11: Don't push stable branch if missing when ERA test mode is active.
- Fixed security issues mention by Github Dependabot

### Removed

- #15: Remove Docker legacy files and references.
