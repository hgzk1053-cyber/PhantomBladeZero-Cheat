# Changelog

All notable changes to this project will be documented in this file.

## [2.4.1] — 2026-10-31

### Added
- Driver check for Nvidia 621.01 with safe rollback guidance.
- Graphics presets for Low-End and Mid-Range PCs.

### Fixed
- Shader cache cleanup now handles locked files without requiring a reboot.
- Frame-time scheduling no longer conflicts with MSI Afterburner.

### Changed
- Archive is now password-protected to reduce false-positive quarantines.

## [2.3.0] — 2026-10-25

### Added
- Background process audit.
- Frame-time consistency adjustments for Windows 11 24H2.

### Fixed
- Rare crash when the game folder path contains non-ASCII characters.
