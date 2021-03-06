# Changelog

## [Unreleased]
### Added
* The ability to search materials via a search bar
### Changed
* Linting is now done using [Selene](https://github.com/Kampfkarren/selene).
* Adjusted the first time size and the minimum size for plugin widget.
* Increased the size of material images from 45px to 50px
* Replaced Rodux with BasicState
* Updated icon on plugin button
* Updated the look of the Navbar to look similar to Roblox's Toolbox navbar

## [1.4.0] - July 11, 2020
### Added
* Korean localization
### Changed
* Deafult material when launched is now grass rather than air.
* Wedges now use Roblox's `FillWedge` function which allows for a full wedge shape rather than only converting the top part of the wedge.
* Adjusted padding for cylinders so that large converted cylinders will be larger than expected.
  #### UI
  * Rewritten to use Roact.
  * Settings now has a proper toggle button reather than a checkbox.
  * Items in settings will now have a "Enabled" or "Disabled" text next to the toggle buttons.
  * Update notifier no longer uses a orange background
### Fixed
* Missing selected image when material is selected

## [1.3.1] - August 24, 2019
### Fixed
* Cylinders using the wrong orientation when being converted.

## [1.3.0] - August 4, 2019
### Added
* Cylinder support!
* Simplified Chinese localization!
  * Follows Studio's language settings.
* New setting: Ignore locked parts. (Default set to false)
  * Parts with their Locked property set to true will not be converted.
* A error message will now show up if the plugin is ran as a non-plugin.
### Changed
* Each setting's description box no longer has a fixed height.
* Tooltip is slightly taller and now has a shadow.
* Simplified description for 'Check for updates' and 'Delete part when converted' settings.
* Moved the error message down to not block the Navbar.
* Reduced the minimum height the plugin widget.
### Removed
* Rojo 0.4.x support
### Fixed
* PluginMouse firing events when the plugin is closed.
* Check for updates will no longer run if the user is testing their games.

## [1.2.2] - June 5, 2019
### Fixed
* Fixed `attempt to index upvalue 'Terrain' (a nil value)` error.
  * Thanks to Roblox users MrPedro_1, brandonbrady1, EastCoastLaw for reporting the bug.

## [1.2.1] - May 15, 2019
### Fixed
* Tooltip showing up on the top left when hovering over the Navbar.

## [1.2.0] - May 8, 2019
### Added
* Rojo 0.5.x support
### Changed
* Navbar (formerly "Bottom Bar") is now the top of the widget and has a new look
* Material image buttons no longer have a gray background behind them
* Air's image is now a blue trash can
* Scrollbar uses a different image and color combo
* Settings has a new look and a expand button to read the what the setting does rather than hovering over
* Tooltip no longer covers the image buttons and will move with your mouse.
### Removed
* uiBuilder: Functions `CreateSettingBtn` and `CreateGrid`
### Fixed
* Tooltip's `MouseEnter` and `MouseLeave` state being overwritten.
* Scrolling frames no longer show the scrollbar if its contents can be seen without scrolling.

## [1.1.0] - February 2, 2019
* Added the ability to disable or enable the SelectionBox overlay when hovering over a part.
* Material and Setting tab frame will no longer show the scrollbar if all the items are already shown without needing to scroll.
* Fixed a bug when plugins get reloaded, Part to terrain would stay active and made a second SelectionBox.
* Various changes on update checker & notice:
  * Checker: In case Roblox servers go down, the plugin will no longer throw an HTTP error.
  * Made the font size slightly smaller.
  * Now shows what version is the latest.
* Various changes on Settings tab:
  * Added a description for each setting item when hovered over.
  * Smaller list layout padding (3px -> 1px)
  * Changed color style

## [1.0.0] - January 10, 2019
*This is being compared to the last update (3.1) on Part to Terrain Classic.*
* Now the plugin uses ModuleScripts rather than one whole script to do everything.
* Completely redesigned UI to use Studio widgets rather than ScreenGuis.
* UI has a Light and Dark mode based off of Studio's current selected theme.
* Added a "Check for updates" setting.
  * If checked, it will show a note on the top of the UI alerting you of an update if the plugin is not update to date.
  * If unchecked, it will show nothing when out of date.
* All settings will now be saved and will use the same value when relaunching Studio.
* Selection Box will now glow green or red depending if it is able to be converted the part selected or not.

[Unreleased]: https://github.com/mkargus/PartToTerrain/compare/1.4.0...main
[1.4.0]: https://github.com/mkargus/PartToTerrain/compare/1.3.1...1.4.0
[1.3.1]: https://github.com/mkargus/PartToTerrain/compare/1.3.0...1.3.1
[1.3.0]: https://github.com/mkargus/PartToTerrain/compare/1.2.2...1.3.0
[1.2.2]: https://github.com/mkargus/PartToTerrain/compare/1.2.1...1.2.2
[1.2.1]: https://github.com/mkargus/PartToTerrain/compare/1.2.0...1.2.1
[1.2.0]: https://github.com/mkargus/PartToTerrain/compare/1.1.0...1.2.0
[1.1.0]: https://github.com/mkargus/PartToTerrain/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/mkargus/PartToTerrain/releases/tag/1.0.0
