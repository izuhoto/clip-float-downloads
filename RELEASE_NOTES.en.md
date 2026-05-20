# Clip Float v1.0.2

2026-05-20

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

# Clip Float v1.0.1

2026-05-19

Version 1.0.1 focuses on stability and usability improvements across history browsing, window behavior, and distribution readiness.

## What is improved
- Improved visibility of the document and settings icons in preview windows, especially on bright or white backgrounds.
- Refined history window frame restore and save behavior to prevent unusable or overly small window states.
- Improved internal robustness around retention cleanup and related APIs.

## Behavior and reliability fixes
- Fixed an issue where capture region size could drift by 1 pixel when restoring or moving windows.
- Improved consistency of history and trash retention cleanup when settings are updated.
- Added persistent trash sort order behavior for a more consistent browsing experience.

# Clip Float v1.0.0

2026-05-15

This is the first release of Clip Float.  
You can use the basic features for screen capture, capture history management, and image editing.

## Highlights
- Screen capture
- Saving and reopening history
- Image editing
- Adding and editing annotations

