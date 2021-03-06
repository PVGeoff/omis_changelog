# OMiS Changelog

All notable changes to this project will be documented in this file.

## [v-1.4.0 - 2022-05-17]

Infrastructure for user groups, total hours for days & improvements

### Changed

- Delete functionality now works off of milestone ID rather than milestone name.
- Users flagged as "interns" should no longer show up on timesheet excel reports for admins.
- When adding a new milestone to a project that has the status "not started" will automatically convert it to "in progress"
- When completing all milestones on a project the status will automatically be changed to complete

### Added

- Total hours for the current day selected will show above the tab switcher component
- The ability to assign multiple roles to users as well as custom groups if user is classified as "admin"

### Fixed

- Milestone duplication

## [v-1.3.2 - 2022-05-17]

Client directory & some nice-to-haves

### Changed

- Fields should clear after a client is succesfully created and will no longer reroute

### Added

- Success message when adding a new client
- Autosave timesheet [^1]
- Client directory
- Edit existing clients with autosave feature [^2]

### Fixed

- CLients not saving properly upon creation

[^1] only when editing an existing sheet the autosave will trigger when adding a new milestone
[^2] Editing can be done by clicking on any client within the client directory. Once you click to another client, the previous one will be automatically saved.

## [v-1.3.1 - 2022-05-17]

Milestone query optimization

### Changed

- Only the milestone and field you are currently editing will be altered in the database [^1]

### Added

### Fixed

[^1] Previously altering a single milestone would force delete and recreate all milestones associated with the project

## [v-1.3.0 - 2022-05-17]

Multiple Users Per Milestone

### Changed

- Temporarily removed users assigned to milestone on project breakdown page
- Temporarily removed Donut graphs on project breakdown page

### Added

- Can now assign multiple users per milestone on the project details page
- Added functionality for displaying all users for the completed milestones page
- New Theme & Icon
- Fish (go find it)

### Fixed

- Fixed a bug where token expiration would not automatically return a user to the login page

## [v-1.2.6 - 2022-05-09]

Project Breakdown and Fixes

### Changed

### Added

- Project breakdown tab to track hours spent on each milestone
- Graph to show top 5 Milestones by hour
- Various additional themes & Logos

### Fixed

- Fixed a bug where users could submit a time without assigning a milestone when creating a new timesheet

## [v-1.2.5 - 2022-05-09]

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
