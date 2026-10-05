# Changelog

All notable changes to stuxgames.github.io are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v2.0.0

### Changed
- Brought the repo up to the standard used across the other Stux.Group brand redirect repos: it now redirects to [github.com/StuxGames](https://github.com/StuxGames) instead of `www.stux.games`, and the README is the shared redirect README with the Stux.Games logo and footer.
- GitHub Pages now deploys through GitHub Actions (`.github/workflows/pages.yml`) instead of the legacy branch build, so every deploy is an observable CI run.

### Added
- `VERSION.md`, `CHANGELOG.md`, `CONTRIBUTING.md`, `commit.sh`/`commit.bat` and `.gitignore`, following the standard release flow. The untagged 2022 redirect counts as v1.
