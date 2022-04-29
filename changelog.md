# OMiS Changelog

All notable changes to this project will be documented in this file.

## [v-1.2.4 - 2022-04-29]

User themes version-1 and excel exports

### Changed

### Added

- Themes added under the account page. To activate a theme, click one of the available themes and hit save.
- Backend support for easily adding more themes
- Export table to excel button. Currently only supports admin timesheet selection.

### Fixed

- Milestone stats should no longer show as NaN%
- Fixed Issue where completed milestones wouldn't move to completed section
- Code cleanup for themes.

## [v-1.2.3] - 2022-04-28

User Directory

### Changed

### Added

- A directory for everyone signed up through OMiS accessible through the navigation bar

### Fixed

## [v-1.2.2] - 2022-04-27

Consolidating project / milestone editing

### Changed

- Admin timesheet table striped
- Removed edit button from project view
- Project name column in project view now clickable. Goes to new project detail pages
- Milestones, completed milestones, and edit project all moved to Project details page
- Moved the ability to change project status into project details page

### Added

- Project detail page
- Milestone overview stats to project details page
- Success message when updating project
- Autosave when altering milestones

### Fixed

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
