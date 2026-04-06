# StartingForth

A small browser-based FORTH system with a teletype-style terminal and a virtual disk.

This FORTH system strives to be compatible with the description in Leo Brodie's book *Starting FORTH*.

## On-line version

[CRT terminal](https://pavel-krivanek.github.io/forth/crt/)

[Teletype](https://pavel-krivanek.github.io/forth/teletype)

[IDE version](https://pavel-krivanek.github.io/forth)

## Controls

- `Enter` — send the current input buffer to FORTH
- `Shift+Enter` — insert a newline into the input buffer
- `Ctrl+S` / `Cmd+S` — download the current disk image as `forth-YYMMDD-HHMMSS.img`
- drag and drop a `.img` file onto the page — replace the current virtual disk
- browser function keys such as `F5` and `F11` are left to the browser

## Disk format

The virtual disk is a 1.44 MB image stored in memory and exposed as a plain `.img` file. Internally, the FORTH side works with 1 KB blocks.

That makes it easy to:
- keep example screens and source blocks in a single image
- export your current state
- reload a previously saved image later
