# CheckIT Changelog

## [Unreleased]

## [3.4.1] - 2018-07-11

### Fixed

- User not authenticated immediately upon login.
- Typeahead results when no results are found.
- Mobile application now has proper Google scopes.
- Flag is now returned to indicate when there is more than the max number of users returned from the Google API.

## [3.4.0] - 2018-03-29

### Changed

- Typeahead (user lookup) functionality now uses current user's authentication to authenticate with Google Directory API.
- User directory data will be cached for small organizations and filtered from Google API for large organizations.
- Setup scripts updated for typeahead changes.

### Deprecated

- Use of service account to authenticate with Google Directory API.

## [3.3.1] - 2018-03-22

### Security

- Address potential securiity vulnerability in moment dependency.

## [3.3.0] - 2018-01-03

### Added

- Book category to asset types.

## [3.2.0] - 2017-08-11

### Added

- App icons and splash screens to Cordova config.
- Predefined return dates to checkout flow.
- Software category to asset types.

### Changed

- Cordova files tracked in source control.

### Fixed

- Back button functionality when viewing device history.
- Back button functionality when editing a device.

## [3.1.1] - 2017-08-04

### Removed

- Ability to select content.

### Fixed

- Bug where icons where selectable.
- Scanner crash on Android 6.x.

## [3.1.0] - 2017-08-03

### Added

- Notification support for checking in and out, adding editing and removing an asset.
- Integrated with HipChat to send notifications to a HipChat room.
- Chronological asset history view.

### Changed

- Asset schema now sets devices to retired.
- Record schema now contains 'adminID' field.
- History view to correctly reflect when an asset is checked in by an admin on behalf of a user.

### Removed

- Calendar setup in config.

### Fixed

- Bug that prevented deletion modal from closing.
- Bug that would not update a user's reservations when an admin checked in the asset on behalf of the user.

## [3.0.0] - 2017-07-24

### Added

- CHANGELOG.md. Content backdated to version 2.0.0.
- Setup and build scripts.
- Google Directory API endpoint and Google Directory User List endpoint.
- User lookup when checking out a device as an admin.

### Changed

- Content in README to now includes general project information and installation instructions.
- Resized history content so user's with long names are visible on the page.
- Wiki provides additional information about the application and a User Guide.
- Validation is now integrated into the page rather than use a popup modal.

### Removed

- The scan button from the webpage view.
- Unnecessary files from certs folder.
- Calendar event functionality and plugin.

### Fixed

- Invalid ID modal now displays a single Okay button.
- "checkedouts" list page title now displays as "checked out".
- Fix styling errors in code noted by `gulp build-spa`.

## [2.0.0] - 2016-08-12

Initial public release for CheckIT.

### Added

- Check out and check in assets.
- Quick scan feature on home page to navigate to asset details.
- Admin users can add, edit, and remove devices.
- Admin users can check out and check in assets for someone else.

[Unreleased]: https://github.com/PointSource/checkit-blueoak/compare/v3.4.1...master
[3.4.1]: https://github.com/PointSource/checkit-blueoak/compare/v3.4.0...v3.4.1
[3.4.0]: https://github.com/PointSource/checkit-blueoak/compare/v3.3.1...v3.4.0
[3.3.1]: https://github.com/PointSource/checkit-blueoak/compare/v3.3.0...v3.3.1
[3.3.0]: https://github.com/PointSource/checkit-blueoak/compare/v3.2.0...v3.3.0
[3.2.0]: https://github.com/PointSource/checkit-blueoak/compare/v3.1.1...v3.2.0
[3.1.1]: https://github.com/PointSource/checkit-blueoak/compare/v3.1.0...v3.1.1
[3.1.0]: https://github.com/PointSource/checkit-blueoak/compare/v3.0.0...v3.1.0
[3.0.0]: https://github.com/PointSource/checkit-blueoak/compare/v2.0.0...v3.0.0
[2.0.0]: https://github.com/PointSource/checkit-blueoak/tree/v2.0.0
