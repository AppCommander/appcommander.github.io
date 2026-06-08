# Changelog

Version format: `YEAR.WEEK.BUILD`

## 2026.24 (2026-06-08)

### SFTP
- **Recursive folder transfers** — copy and move entire folders over SFTP, including nested subfolders.
- **Data-loss hardening** — a transfer is verified complete before the source is removed, and overwrites are crash-safe.

### Performance
- Smoother browsing of large folders: icon caching plus cached sorting and filtering reduce stutter.

### Fixes
- Clicking a panel restores keyboard navigation after you've used the Filter field.

### Other
- Refined app icon that follows the macOS icon grid.
- During the free trial, the app reports anonymous, pseudonymous usage analytics (no personal data, files, or hostnames; no third-party trackers) to help improve it. Licensed copies never send this; there's a first-run notice and an opt-out in Preferences ▸ License.

## 2026.23.1 (2026-06-05)

### Reliability
- **Safer file overwrites** — copying or moving a file onto an existing one no longer risks losing the original if the operation is interrupted. The existing file is kept until the new copy completes successfully.
- **Remote operations report failures correctly** — over SFTP, a failed sudo delete/move/copy is no longer silently treated as success.

### Improvements
- Pressing Enter in the search field opens the focused item and clears the filter
- The first matching item is auto-focused as you type, and its panel is activated
- Smoother focus restoration when navigating with the arrow keys
- Disk usage dialog shows a detailed per-folder breakdown

## 2026.11.10 (2026-03-09)

### New Features
- **Disk usage dialog** - Click free space in status bar to see a donut chart of disk usage
- **Open in Finder** button in Path and Go to Folder dialogs
- **Finder-style arrow key navigation** - Left arrow goes to parent directory, right arrow enters focused directory (list view)

### Improvements
- Hide tab bar when only one tab is open to reduce visual clutter
- Fix shift+click range selection with filtered items

## 2026.06.1 (2026-02-02)

### New Features
- **Flat view mode** (⌘B) - Show all files from subfolders in a single list
- **Batch rename** (⇧⌘R) - Rename multiple files at once
  - Find & replace text
  - Add prefix or suffix
  - Sequential numbering
  - Change case (upper/lower/title)
  - Live preview before applying
- Automatic update check on app launch

### Security
- Enhanced license validation with improved offline support
- Improved archive extraction security

### Fixes
- Fix dragging multiple files to external applications
- Fix zip file handling for special characters in filenames

## 2026.05.8 (2026-01-29)

### New Features
- Slow double-click to rename files inline (like Finder)
- Permanent delete with ⇧⌘⌫ keyboard shortcut (bypass Trash)
- Swap panels with ⌘U keyboard shortcut
- Clickable path display for both panels in status bar

### Improvements
- Increased max font scale to 300%
- Preferences window widened to fit all tabs

## 2026.05.7 (2026-01-27)

### Fixes
- Fix same-panel drag-and-drop creating unwanted file copies

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