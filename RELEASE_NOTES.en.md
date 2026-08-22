# Clip Float v1.0.7 2026-08-22

Version 1.0.7 adds delayed region capture, making it easier to capture the screen after preparing menus or other transient UI.

## Highlights
- Added delayed capture for Region mode. Press `D` while selecting a region, then confirm the area to capture after a countdown.
- Added `-` / `+` controls for adjusting the delay, plus a Settings default from 1 to 60 seconds.
- Shows the remaining countdown time in the menu bar and adds a status-menu action to cancel delayed capture.

# Clip Float v1.0.6 2026-08-19

Version 1.0.6 improves capture-region accuracy on built-in displays and multi-display setups.

## Improvements and Fixes
- Fixed capture output drifting away from the selected area when using scaled built-in display modes.
- Centralized capture overlay coordinate conversion, making mouse-position handling more reliable across multi-display layouts and global input monitoring.
- Adjusted the capture overlay so menu bar, Dock, and notch constraints do not desync it from the actual screen frame.
- Added tests for display scaling and coordinate conversion to catch capture-region regressions.

# Clip Float v1.0.5 2026-08-09

Version 1.0.5 expands editing workflows with OCR access from previews, canvas expansion, and richer line editing.

## Highlights
- Added OCR from the preview window gear menu. Recognition results are copied to the clipboard, and history previews can target either the full image or the current cropped area.
- Added an Expand tool for adding transparent or solid-color padding around a captured image, so annotations can be placed outside the original capture.
- Added Bezier curve support for line annotations and a Pen tool, including anchor/handle editing, point insertion/removal, and curve straightening.
- Added a bottom status bar in the editor to show line/path editing hints when a line object is selected.

## Improvements and Fixes
- Improved text annotation editing: font size now follows the image display scale, text boxes grow only when content needs more space, and click/caret behavior is more stable.
- Fixed OCR current-area targeting after multiple chained crops.
- Fixed Expand gestures adding no-op Undo entries, and ensured unfinished Pen drafts are cleared when switching tools.
- Improved curve point insertion/removal, arrow endpoint trimming, and exported arrow direction for curved lines.

# Clip Float v1.0.4 2026-05-22

- Improved Screen Recording permission flow
  - When Screen Recording permission is missing, the app now requests permission first, and only opens System Settings if permission is still not granted.

# Clip Float v1.0.3 2026-05-21

## Improvements
- Fixed an issue where range selection in History Browser could not be extended with Shift + Arrow keys.

# Clip Float v1.0.2 2026-05-20

Version 1.0.2 Released

This release improves capture and history workflows with better usability, reliability, and release/build maintenance updates.

## Highlights
- Added a fallback path for preview export drag-and-drop in environments where the previous behavior was unreliable.
- Added a way to hide capture guidance/HUD information when needed, improving visibility during selection.
- Improved gear icon visibility in dark mode for better UI clarity.

## Fixes
- Fixed a regression where the Delete shortcut did not correctly delete selected history items.
- Fixed preview export drag control behavior, including accessibility-related handling.
- Aligned Space-key HUD toggle behavior and hint wording.
- Included follow-up fixes around capture/HUD interaction and related UI behavior.

## Quality and Maintenance
- Refactored internal helper naming for clearer Delete command handling.
- Expanded and updated tests for capture session and history coordinator behavior.
- Updated release/build process assets, including Makefile/README-related maintenance and release prep commits.

# Clip Float v1.0.1 2026-05-19

Version 1.0.1 focuses on stability and usability improvements across history browsing, window behavior, and distribution readiness.

## What is improved
- Improved visibility of the document and settings icons in preview windows, especially on bright or white backgrounds.
- Refined history window frame restore and save behavior to prevent unusable or overly small window states.
- Improved internal robustness around retention cleanup and related APIs.

## Behavior and reliability fixes
- Fixed an issue where capture region size could drift by 1 pixel when restoring or moving windows.
- Improved consistency of history and trash retention cleanup when settings are updated.
- Added persistent trash sort order behavior for a more consistent browsing experience.

# Clip Float v1.0.0 2026-05-15

This is the first release of Clip Float.
You can use the basic features for screen capture, capture history management, and image editing.

## Highlights
- Screen capture
- Saving and reopening history
- Image editing
- Adding and editing annotations
