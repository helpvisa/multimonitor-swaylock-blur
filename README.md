## Multi-Monitor Blurred Lockscreen with SwayLock and Bash

This script uses libvips (or alternatively ImageMagick) to blur the screen with regular old swaylock.
It uses swaymsg to gather information about your active outputs, takes screenshots of those outputs, blurs them, and displays them per-output when the screen is locked.
All screenshots are stored in /tmp.

Uncomment the "convert" line if you'd rather use ImageMagick than libvips (the latter is, however, *significantly* faster!)

Simply execute the script using a keybind and/or use it with swayidle!

Requirements:
- sway
- swaylock
- grim
- libvips *or* ImageMagick
