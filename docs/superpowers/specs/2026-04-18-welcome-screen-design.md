# Welcome Screen Design

**Date:** 2026-04-18
**Status:** Approved

## Goal

Add a minimal welcome screen that appears before the home screen on every page load. The user clicks anywhere to proceed to the main screen.

## Behaviour

- Shown on every page load (no persistence, no localStorage).
- Clicking anywhere on the screen calls `showScreen('screen-home')`.
- Does not replace the home screen — it sits in front of it.

## Visual design

- Layout: centered, full card area
- Icon: 📖 (64px)
- Title: "Language Learning" (existing app title, 28px bold)
- Hint text: "Tap anywhere to begin" (14px, muted colour)
- No buttons — entire screen is the click target
- Theme toggle visible in topbar (existing behaviour preserved)

## Technical changes

| File | Change |
|---|---|
| `index.html` | Add `<div id="screen-welcome">` with `class="screen active"` |
| `index.html` | Remove `active` from `screen-home` on initial load |
| `index.html` | Add CSS for `.welcome-wrapper` (centered flex layout) |
| `index.html` | Add `screen-welcome` to `HIDE_INDICATOR_ON` set |
| `index.html` | Add `onclick="showScreen('screen-home')"` on welcome div |

## Constraints

- No new libraries.
- Must work with existing dark mode (uses CSS custom properties).
- Must be keyboard accessible: `role="button"`, `tabindex="0"`, Enter key support.
- No changes to any other screen or flow.
