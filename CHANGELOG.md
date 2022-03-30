# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.2] - 2021-03-30
### Added
- deploy script to push the project to the `upm` branch, allowing for easy import to unity
- namespaces
- checkbox to config to allow the tilde keyboard key to toggle the terminal visibility
- function to show the terminal by script

### Changed
- Only add to don't destroy on load scene if the terminal is outside of this scene
- Restructure project so a Unity project can be opened and run from the repo root
- updated the readme to describe new installation and deploy procedures
- replaced deprecated WWW class
- make the toggle function public
- change the order of default commands

### Fixed
- Null error when pressing tab with an empty input field


## [1.0.1] - 2021-03-29
### Added
- Added font size to config file and set a default font size

### Changed
- Do not attempt to execute empty commands

## [1.0.0] - 2021-03-29
### Changed
- Reworked repo structure to adhere to [Unity's custom package structure](https://docs.unity3d.com/Manual/CustomPackages.html)
