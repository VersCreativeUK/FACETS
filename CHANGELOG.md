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
- Logic – Migrate existing “guest” entries to user on login/register
- UI – Heatmaps
- Logic – Update Existing Fragments & Activities to ButterKnife Binding
- JavaDocs & Documentation
- UI/Functionality - Activity Diary Add Additional Information
    - Symptoms (Shopping List)
- Rate my sleep option + Settings
- UI/Functionality – Full Functional Activity Diary Reporting
- UI/UX – Full Functional Onboarding and Post-Registration
- Functionality – Dashboard
- Functionality - Activity Diary Notifications


## [Upcoming] (Next Release)
- UI/Functionality – View Alarm


## [Open Bugs]
- [#10](https://github.com/VersCreativeUK/FACETS/issues/10) Functionality – Activities added between 12AM – 1AM are not displayed
- [#11](https://github.com/VersCreativeUK/FACETS/issues/11) Functionality – Issues with Alarms being removed when device is rebooted
- [#12](https://github.com/VersCreativeUK/FACETS/issues/12) UI – Navigation is not updated correctly when navigating “up” (back)
- [#17](https://github.com/VersCreativeUK/FACETS/issues/17) UI – Success UI issues
- [#N/A] Logic – Rest Periods updates do not propagate unless deleted and recreated


## [0.0.5]
### Added
- UI – Sleep Wake Pattern
- UI/UX/Functionality - App Theming
- UI – New/Alternative Colour Schemes
- Functionality – DarkSky Weather API
- UI – Initial Sleep Wake Pattern Setup
- UI – New custom font implemented [Krub]( https://fonts.google.com/specimen/Krub)
- UI – New “Quick View” dialog when long clicking an Activity
- UX – Notification Logic

### Changed
- **BREAKING CHANGE** Logic – Updated Rest/Sleep & Wake Routine
    - Updated Database, Adapter & Model Definitions
        - RestSleepAlarm – Changed to RestPeriod
        - SleepWakePattern – Added
- UI – Rest/Sleep/Wake Routine Database Accesses
- UI – Updated Activity Diary Home
    - Updated Calendar view implemented to reduce thread load
    - Updated Activity name view implemented to marquee (scroll) if a name overlaps

### Removed
- Logic – Redundant Classes
 
### Fixed
- Minor - UI – Font Consistency
- Minor – UX - App Theming inconsistency
- Minor – UX – Activity List Custom Date Picker now has future dates disabled

## [0.0.4a] – 2018-12-21
### Fixed
- Minor UI - Analog Clock Sizing Ratio

## [0.0.4]
### Added
- UX - Improved error management when accessing database
- UX - New Routing for “undeveloped” areas
- UI/Functionality – Copy Activity

### Changed
- **BREAKING CHANGE** UI/Logic - Updated Rest/Sleep & Wake Routine
    - New List Activity
    - Updated Database Definition
    - Updated RSW Home Layout
- UI/Functionality – Initial Activity Diary Reporting Layout
- Miscellaneous text changes
- Numeric value added to Enjoyment Level
- Dashboard updates for Alpha
- Two step confirmation for “long-click” delete option on Alarms and Activities
- Updated Add Activity Layout
- Updated Dashboard Hero
- Updated Activity List Layout
- Updated View Activity Layout
- Misc. descriptive changes

### Fixed
- [#14](https://github.com/VersCreativeUK/FACETS/issues/14) Functionality – ChipGroup Selection issues
- Minor – Scrolling content display bug for recap and help sections

 
## [0.0.3]
### Added
- Functionality/UI – New Dashboard FloatingActionButton and Add Menu
- Logic – Added ButterKnife
- UI – TextToSpeech UI
- UI/Functionality – Edit Alarm
- UI/UX – Basic Onboarding and Post-Registration
- UI/UX – Coming Soon Activity to hold un-developed areas cleanly
 
 
### Changed
- UI – Updated View Activity Layout
- UI – Updated Login Design and Layout
- UI – Updated AlarmActivity Layout
- UI – Dynamic Dashboard “Welcome Icon”
- UX/UI – Updated navigation layout
 
 
### Fixed
- [#9](https://github.com/VersCreativeUK/FACETS/issues/9) Functionality – Issues with Alarms duplicating when being created and overlapping
- [#13](https://github.com/VersCreativeUK/FACETS/issues/13) UI/Functionality – Missing Username on “admin” signup
- Minor UI – Status Bar colouring to match current fragment’s theme
 
 
## [0.0.2a] – 2018-11-21
### Added
- Functionality/UX – TextToSpeech
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

