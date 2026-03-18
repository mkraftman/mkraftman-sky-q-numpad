# mkraftman-sky-q-numpad

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
