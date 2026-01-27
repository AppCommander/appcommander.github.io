# Changelog

Version format: `YEAR.WEEK.BUILD`

## 2026.05.6 (2026-01-27)

### New Features
- Built-in terminal with SwiftTerm integration (SSH auto-login, SFTP panel sync)
- Configurable parallel transfer threshold setting

## 2026.05.5 (2026-01-27)

### Security Improvements
- Migrate credential storage to macOS Keychain (replaces custom AES encryption)
- Sanitize file rename input to prevent path traversal
- Remove user email from log output (PII privacy fix)

## 2026.05.4 (2026-01-26)

### New Features
- Column resize mode setting (Preferences → Columns)
  - Horizontal Scroll: fixed column widths with horizontal scrolling
  - Fit to Panel: columns scale proportionally to panel width
  - Fit with Wrap: columns scale and text wraps to multiple lines

## 2026.05.3 (2026-01-26)

### Fixes
- Panel content alignment fixed (always starts from top-left)
- Content no longer centers when window is resized

## 2026.05.1 (2026-01-26)

### New Features
- Sparkle auto-update support
- "Check for Updates" menu item
- Licensing system (60-day trial)
- Online license validation
- Dynamic pricing from API

### Changes
- Version format: year.week.build
- Sparkle Hungarian localization
- SSH passwords stored in encrypted file
