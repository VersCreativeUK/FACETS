# Changelog
All notable changes to this project will be documented in this file.
Added for new features.
Changed for changes in existing functionality.
Deprecated for soon-to-be removed features.
Removed for now removed features.
Fixed for any bug fixes.
Security in case of vulnerabilities.

## [Scoped]
- Functionality - Dynamic content locking based on FACETS commencement date
- UI/UX/Functionality - First time setup flows
- UI/Functionality - Activity Diary Reporting
- Logic – Migrate existing “guest” entries to user on login/register
- UI – Heatmaps
- Functionality - DarkSky API (Retrofit)
- Logic/Functionality – Alarms vs. Notifications (Rest/Sleep/Wake Planner)
- UI – New/Alternative Colour Scheme


## [Upcoming] (Next Release)
- Functionality - Activity Diary Notifications
- UI/Functionality - Activity Diary Add Additional Information
    - Symptoms (Shopping List)
- UI – Add app icon to AlarmActivity
- UI/Functionality – Copy Activity
- UI/Functionality – View Alarm
- UI/Functionality – Edit Alarm
- UI – Dynamic Dashboard “Welcome Icon”
- Functionality – Develop Dashboard Items


## [Open Bugs]
- [#9](https://github.com/VersCreativeUK/FACETS/issues/9) Functionality – Issues with Alarms duplicating when being created and overlapping
- [#10](https://github.com/VersCreativeUK/FACETS/issues/10) Functionality – Activities added between 12AM – 1AM are not displayed
- [#11](https://github.com/VersCreativeUK/FACETS/issues/11) Functionality – Issues with Alarms being removed when device is rebooted
- [#12](https://github.com/VersCreativeUK/FACETS/issues/12) UI – Navigation is not updated correctly when navigating “up” (back)
- [#13](https://github.com/VersCreativeUK/FACETS/issues/13) UI/Functionality – Missing Username on “admin” signup

## [Unreleased] [0.0.3] (Due 2018-11-29)
### Added
- Functionality/UI – New Dashboard FloatingActionButton and Add Menu

### Changed
- UI – Updated View Activity Layout

## [0.0.2a] – 2018-11-21
### Added
- Functionality/UX – Text to Speech
- UX – Add Alarm Validation

### Changed
- UI – Rest/Sleep Planner has been renamed to Rest/Sleep/Wake Routine
- UI – Rest/Sleep/Wake Routine Layout is now tabular in order to separate new rest and sleep/wake
- UI/UX – Section help moved to align with Section Title
- UI – Activity List – Updated Colour Codes to filled squares


### Fixed
- Minor – App Crash if alarm tone is not selected
- Minor – App Crash when opening intro video 2


## [0.0.2] – 2018-11-16
### Added
- Functionality - Rest/Sleep Planner
    - Add Alarm
    - Visual Reporting
    - FACETS Week 2 Recap
    - Planner Help
- Functionality - Alarm Receiver & Activity
- UI - Test Video Added
- Functionality - Guest User
    - User vs. Guest logic
- UI/Functionality - "Empty" list UI added to Activity Diary
- UI - App Launcher Icon
- UI/Functionality - Activity Diary Add Additional Information
    - Comments
    - Temperature
- UI/Functionality – Selectable options for Activity Name
- UI/Functionality – Basic View Activity
- Functionality – Basic Notifications
- UI/Functionality – Edit Activity


### Changed
- UI - Application base fonts
- UI - Activity Diary item layout
- UI/Functionality – Updated Dashboard
- UI – Updated Add Alarm Layout
- UI - Updated Splash Screen
- UX – Add Activity Validation


### Fixed
- [#1](https://github.com/VersCreativeUK/FACETS/issues/1) - UI - Available date issues with ActivityDiary and CollapsibleCalendarView
- [#2](https://github.com/VersCreativeUK/FACETS/issues/2) UI - Navigation Logic when switching between homework elements
- [#3](https://github.com/VersCreativeUK/FACETS/issues/3) UX - Issues with Ringtone preview & selection on certain devices
- [#4](https://github.com/VersCreativeUK/FACETS/issues/4) UX - Interaction issues with Activity List and Navigation Drawer
- [#5](https://github.com/VersCreativeUK/FACETS/issues/5) Functionality/UX - Data integrity & portability breaking UI when device is offline
- [#6](https://github.com/VersCreativeUK/FACETS/issues/6) UI - Locked Item Functionality not displaying in menu & items dialog notification display
- [#7](https://github.com/VersCreativeUK/FACETS/issues/7) UX - Scrolling Issues with SmileyRating implementation
- [#8](https://github.com/VersCreativeUK/FACETS/issues/8) UI – Incorrect Theming for Snackbar

## [0.0.1] - 2018-10-31 (Initial Version)
### Added
- Initial Activity Diary
- Initial Navigation

