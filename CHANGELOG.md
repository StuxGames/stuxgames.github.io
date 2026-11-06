# Changelog

All notable changes to the Stux.Games GitHub Pages Redirect (stuxgames.github.io) are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Date Versioning](https://datevers.ing) since v26.10.23 (`YY.MM.DD`, the UTC release date, with `-1`, `-2`… for later releases the same day); earlier releases used [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v26.11.06-1

### Added

- A `test` branch: work happens on `test` (or a branch off it), and reaches `main` only through a pull request from
  `test` that Leo reviews and merges. Release commits and tags are made on `test`. CONTRIBUTING has a Branches section
  and the README's Versioning section says so

### Changed

- `commit.sh` and `commit.bat` suggest `git push origin test --tags`

## v26.11.06

### Changed

- The README describes this repo rather than the generic template: it says where stuxgames.github.io redirects
  (github.com/StuxGames), how the Actions deploy works, and points to StuxGroup/GitHubPagesRedirect for anyone wanting
  their own. It's titled **Stux.Games GitHub Pages Redirect**, with the standard footer
- The logos on the README and CONTRIBUTING use the light/dark `<picture>` form

### Fixed

- The README no longer tells you to replace `example.com`, says to use this repo as a template (it isn't one) or
  grants reuse; it now carries the Stux Group Ltd copyright

## v26.10.23

### Added

- `tests/version.sh`, which checks that `VERSION.md` is a valid Date Version, a real calendar date not in the future, and the same as the newest entry in this changelog

### Changed

- Switched from Semantic Versioning to [Date Versioning](https://datevers.ing): releases are numbered by their UTC release date as `YY.MM.DD`, with `-1`, `-2`… for later releases the same day. This release follows v2.0.0
- `commit.sh` and `commit.bat` refuse a `VERSION.md` that isn't a valid Date Version or is dated in the future (UTC), and warn when it's dated before today
- `README.md` and `CONTRIBUTING.md` describe Date Versioning and the release steps

## v2.0.0

### Changed
- Brought the repo up to the standard used across the other Stux.Group brand redirect repos: it now redirects to [github.com/StuxGames](https://github.com/StuxGames) instead of `www.stux.games`, and the README is the shared redirect README with the Stux.Games logo and footer.
- GitHub Pages now deploys through GitHub Actions (`.github/workflows/pages.yml`) instead of the legacy branch build, so every deploy is an observable CI run.

### Added
- `VERSION.md`, `CHANGELOG.md`, `CONTRIBUTING.md`, `commit.sh`/`commit.bat` and `.gitignore`, following the standard release flow. The untagged 2022 redirect counts as v1.
