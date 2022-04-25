# OMiS Changelog

All notable changes to this project will be documented in this file.

## [v-1.2.1] - 2022-04-25

Timesheet redesign, logo change, and framework for theming.

### Changed

- OMiS Logo
- Can no longer alter project once timesheet is submitted (can delete and recreate)
- Various table background colors

### Added

- Company selection on each individual milestone. This selection will default to the project's company but can be changed
- Required milestone selection when entering in times on timesheet page. Milestone must have associated company in order to show up on the timesheet page.
- Added framework for new theme colors for individual profiles
- Enter key to submit a new milestone

### Fixed

- Clearing milestone input once added
- Should now be able to delete all timesheet records (previously couldn't delete if ther was only one entry)
- Code refactoring and cleanup
