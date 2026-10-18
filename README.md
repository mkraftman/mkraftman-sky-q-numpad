# Mkraftman Sky Q Numpad

Custom HACS Lovelace card for Sky Q numeric channel entry via `remote.send_command`.

## Features

- Dialpad icon that opens a custom numpad overlay
- Sends digits 0-9 as individual commands to the Sky Q box
- Auto-closes after 3 digits (Sky Q changes channel automatically)
- Backspace sends "left" command to keep box in sync
- Tap outside numpad to dismiss
- iOS-style keyboard appearance with rounded corners

## Installation

1. Add this repository to HACS as a custom repository
2. Install the card
3. Add to your dashboard

## Configuration

```yaml
type: custom:mkraftman-sky-q-numpad
entity: remote.sky_q_living_room
```

## Releasing

Bump the version in `VERSION` (e.g. `1.0.1`) and push to `main`. The release workflow creates the matching `vX.Y.Z` tag and GitHub release with `dist/mkraftman-sky-q-numpad.js` attached. Pushing a `vX.Y.Z` tag directly also still works.
