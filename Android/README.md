# FACETS Digital Toolkit - Android

## Changelog
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
- Logic – Update Existing Fragments & Activities to ButterKnife Binding
- JavaDocs & Documentation
- Rate my sleep option + Settings
- UI/UX – Full Functional Onboarding and Post-Registration
- Functionality - Activity Diary Notifications
- Logic – Reduce layout files for help and recap to 2 templates and then populate text via java not xml


## [Upcoming] (Next Release)
- UI/Functionality – View Alarm


## [Open Bugs]
See [Here](https://github.com/VersCreativeUK/FACETS/issues)

## [Unreleased] [0.1.0]
### Added
- Activity Diary Categories
- Goal Planner
    - Home, List, Swipe to Refresh and Tabbed Layouts
    - DB Logic
    - Add Logic
    - View Goal
    - Help & Recap Sections
    - Keep on Track Plan linkages
- Keep on Track Planner
    - Fatigue Factors
    - Priorities
    - Goals (inc. DB references to Goal Planner)
    - Help & Recap Sections

### Changed
- Activity Diary Reporting
- Updated Dashboard Layout

## [Unreleased] [0.0.8-rc1]
### Added
- MS Symptoms can be added to an Activity diary entry

## [0.0.7] - 2019-03-29
### Added
- Toolkit Help to Context Menu
- More UI Concept and substitute Toolbar Save action added to Add Activity [#68](https://github.com/VersCreativeUK/FACETS/issues/68)
- View RestPeriod Options Bottom Sheet (replaces outdated `Toast`)
- Admin Function Settings Fragment Added to Settings (For **Supervised Testing Version** Only)
    - Restart with Tutorial Settings Option

### Changed
- Add Activity "Activity Name" changed to "Activity Description" and Layout altered to improve flow
- Sleep/Wake Pattern Activity Title (was "Routine")
- Update Unsaved Changes Dialog wording
- Aligned Unsaved Dialog Titles, Buttons and Content Text
- Removed further references to "Alarm" when this should be "Rest Period"
- Updated Crashlytics to handle non-fatal (caught) crashes

### Fixed
- BLOCKING REGRESSION issue with `Fragment` backstack [#72](https://github.com/VersCreativeUK/FACETS/issues/72)
- Activity context dialog remaining open erroneously when deleting from said dialog
- `Fragment` `Context` attachment conflicts
- Bug when editing a rest period the app was checking for rest period overlaps including itself forcing an error
- Bug preventing a reminder tone being selected for a Rest Period
- Bug where Reminder Tone did not clear when switching Reminder Type
- Further bugs with AlarmManager request codes
- Dashboard crash on Android 6
- `RestSleepWakeReceiver` and `AlarmActivity` Crashes on `null` models
- Multiple fixes for Custom Duration Crashes
- Miscellanous Bugs found in testing

## [0.0.7-rc4] - 2019-03-20
### Added:
- **MAJOR** - Temporary Privacy Policy added to resolve Google Play Policy Violation
- Forgotten Password Option
- Summary/Explanation for Sleep/Wake Pattern timings
- `MainActivity` Tutorial and Logic
- TTS added to Toolkit Help, page 1
- Network check added to YoutubePlayer instances - [#59](https://github.com/VersCreativeUK/FACETS/issues/59) Initial Logic for Unsaved confirmation dialogs
    - Activity Diary
    - Rest Period
    - Sleep/Wake Pattern (View and Edit)

### Changed:
- [#57](https://github.com/VersCreativeUK/FACETS/issues/57) Rest & Sleep Routine updated to match user’s chosen theme.
- [#68](https://github.com/VersCreativeUK/FACETS/issues/68) Updated Save UI and Button Alignment
- Colour Scheme for Dashboard `AppBarLayout` has been amended to `appColorPrimary`
- Updated Logos
- Add Activity moved to `Activity` from `Fragment`
- Add Rest Period moved to `Activity` from `Fragment`
- Add Activity Comments Auto-Open on Add
- Updated Toolkit Help Layout
- Updated reminder logic for Sleep/Wake Pattern to include beginning/end reminders
- Updated Sleep/Wake Pattern visuals to include duration of wind up/down periods
- Updated Sleep/Wake Pattern logic to handle wind up/down period duration that overlaps midnight
- `PreferenceManager` Changes for Tutorial Management
- Minor Sleep/Wake Pattern text format change
- Notification changes to adopt new Sleep/Wake Settings
- Alarm Activity Updated to allow for Sleep/Wake alarm reminders

### Fixed:
- [#11](https://github.com/VersCreativeUK/FACETS/issues/11) Sleep Wake Pattern reminders on Device Boot 
- [#69](https://github.com/VersCreativeUK/FACETS/issues/69) Rest Period Overlap Prevention
- Rest Periods can no longer overlap another
- Sleep/Wake Pattern can no longer overlap a Rest Period
- Bug where activityName chip options did not populate field correctly
- Bug where newly created Sleep/Wake patterns where reminders were forced to be Alarms
- Reminders now default to 0 seconds on the minute (previously defaulted to set time seconds value)
    - i.e: if reminder was set up at 15:30:20 for 19:00, the reminder would set at 19:00:20 not 19:00:00
- Sleep Wake Pattern reminders have been added to fix for #11 
- Minor graphical calculation issue on Rest/Sleep/Wake timings
- Minor intermittent visualisation issues with Rest/Sleep Summary
- Crash on Device Boot Receiver and `SleepWakePattern` Receiver
- Crash on Add Activity
- Crash on FieldUtils when a null field is passed
- Bug and Clashes with `AlarmManager` request codes

### Removed: 
- `android:navigationBarColor` style item removed
- New to Toolkit Dashboard Item

## [0.0.7-rc3] – 2019-03-06
### Added
- Placeholder Video Created to fill missing video views
- Network check prior to retrieving temperature in case of no connection
- Automated Temperature retrieval to Copy Activity
- Close App confirmation dialog
- Sleep Time added to Sleep Wake Routine
- Unsaved changes dialog (part of #59) added to Sleep/Wake Routine
- [#61](https://github.com/VersCreativeUK/FACETS/issues/61) [REQUEST] Placeholder for Rest/Sleep Summary when neither element contains data.

### Changed
- MAJOR Updated Data Format for Sleep/Wake Pattern and new setup UI implemented
- MAJOR Updated YoutubePlayerView dependency version to 10.0.1 from 8.0.1
- Updated Edit Activity enjoyment rating texts
- Updated implementation based on #28
- Updated additional activity field descriptions
- Miscellaneous updates to layout files to improve spacing
- Miscellaneous text updates
- Updated Recap and Help layouts (part of #52)
- Updated miscellaneous dependencies to latest version
- Heatmap end time updated to 12AM
- Navigation Updates
- Snackbars updated to Material Guidelines 2
- [#56](https://github.com/VersCreativeUK/FACETS/issues/56) Change of Sleep/Wake Routine Icon
- [#65](https://github.com/VersCreativeUK/FACETS/issues/65) Removal of “Remind Me” option when first creating a rest period
- [#66](https://github.com/VersCreativeUK/FACETS/issues/66) Next Rest period not updating immediately in RSW Home

### Fixed
- [#N/A] Minor issue with FitChart where rest periods did not clear when Sleep/Wake pattern does not exist
- [#53](https://github.com/VersCreativeUK/FACETS/issues/53) Crash caused by a Context reference bug when creating a rest period
- [#54](https://github.com/VersCreativeUK/FACETS/issues/54) Activity Diary Fatigue level of 1 not re-populating to UI on Edit
- [#55](https://github.com/VersCreativeUK/FACETS/issues/55) [REQUEST] Color state list change for bottom navigation
- [#56](https://github.com/VersCreativeUK/FACETS/issues/56) Sleep Wake Icon Visibility
- [#60](https://github.com/VersCreativeUK/FACETS/issues/60) [REQUEST] Remove Enabled Option when first creating a Sleep/Wake routine
- [#64](https://github.com/VersCreativeUK/FACETS/issues/64) Improvements and Prevention of continued fragment backstack issues


## [0.0.7-rc2] – 2019-02-26
### Added
- Initial Logic for Sleep/Wake Routine Reminders

### Changed
- Removed Logout functionality if user is a guest

### Fixed
- [#N/A] Crash on API 23 and below caused by formatting error in Activity Diary
- [#N/A] Multiple fixes for Sleep/Wake Routine logic
- [#28](https://github.com/VersCreativeUK/FACETS/issues/28) Drawable Runtime Crash for logo

## [0.0.7-rc1] – 2019-02-25
### Added
- Swipe to Refresh Layouts to Activity Diary and Rest Period List
- Performance & Crashlytics SDK
- Updated App Icon
- Today’s Heatmap Calculation

### Changed
- Updated View Sleep Wake Routine Layout and Reminder Settings
- [#20](https://github.com/VersCreativeUK/FACETS/issues/20) REQUEST - Rest Period Reminder Option Layout
- [#27](https://github.com/VersCreativeUK/FACETS/issues/27) REQUEST – Merge Toolkit Introduction and Help into 1 section
- [#35](https://github.com/VersCreativeUK/FACETS/issues/35) REQUEST – Changes to Rest & Sleep/Wake Home and Visualisations

### Fixed
- [#10](https://github.com/VersCreativeUK/FACETS/issues/10) Missing Activities between 12AM-1AM
- **PARITAL** [#11](https://github.com/VersCreativeUK/FACETS/issues/11) Alarms not resetting on phone restart
- [#12](https://github.com/VersCreativeUK/FACETS/issues/12) Navigation Drawer current selection not showing/updating on “Up”
- [#45](https://github.com/VersCreativeUK/FACETS/issues/45) Rest Period Updates not propagating
- [#48](https://github.com/VersCreativeUK/FACETS/issues/48) Erroneous Rest Period displaying on Resume


## [0.0.6-rc4] – 2019-02-12
### Changed
- Condensed On-Boarding journey for testing users
- [#38](https://github.com/VersCreativeUK/FACETS/issues/38) Changes to Heatmap colours and design
- [#40](https://github.com/VersCreativeUK/FACETS/issues/40) Changes to custom rest period duration entry

### Fixed
- [#24](https://github.com/VersCreativeUK/FACETS/issues/24) Get Temperature GPS request hang
- [#28](https://github.com/VersCreativeUK/FACETS/issues/28) Resource Crash on API 23 and below
- [#33](https://github.com/VersCreativeUK/FACETS/issues/33) Text overlap issues in Rest & Sleep Routine
- [#34](https://github.com/VersCreativeUK/FACETS/issues/34) Fixed ability to disable individual Rest period reminders
- [#37](https://github.com/VersCreativeUK/FACETS/issues/37) Added missing icon for silent notifications
- [#39](https://github.com/VersCreativeUK/FACETS/issues/39) Updated Sleep/Wake Pattern layout for smaller devices
- [#41](https://github.com/VersCreativeUK/FACETS/issues/41) Crash on Edit Rest Period
- [#42](https://github.com/VersCreativeUK/FACETS/issues/42) Updated Add Activity Layout for smaller devices

## [0.0.6-rc3] – 2019-02-07
### Fixed
- [#26](https://github.com/VersCreativeUK/FACETS/issues/26) Versioning not Updating
- [#28](https://github.com/VersCreativeUK/FACETS/issues/28) RuntimeException for API23 and Below

## [0.0.6] – 2019-02-05
### Added
- Initial Heatmap Functionality 
- Dynamic Dashboard Items
- [#20](https://github.com/VersCreativeUK/FACETS/issues/20) – Silent Reminder Option

### Changed
- UX - Rest Period Notification Text Change (Removal of “!”)
- UX – Entry/Selection field placeholders change to “Please Choose…” or “Please Enter…” instead of “None”
- UI – Reminder Type dialog title correction from “Alarm Type” to “Reminder Type”
- UX – Dashboard “SpeedDial” FloatingActionButton items are now dynamic depending on locked content

### Fixed
- [#17](https://github.com/VersCreativeUK/FACETS/issues/17) UI – Success UI issues
- [#19](https://github.com/VersCreativeUK/FACETS/issues/19) Dashboard FloatingActionButton Erroneous Display Issue
- [#22](https://github.com/VersCreativeUK/FACETS/issues/22) Missing Rest Period Summary Items
- [#23](https://github.com/VersCreativeUK/FACETS/issues/23) Major - View Activity IllegalStateException
- [#25](https://github.com/VersCreativeUK/FACETS/issues/25) Major - NumberFormatException on Custom Duration Rest Period entry
- [#NA] Multiple issues with Heatmap display

## [0.0.5] – 2019-01-27
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
