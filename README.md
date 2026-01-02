# Reading Guide v1.0.0
A lightweight, tactical focus tool designed for students and researchers. This utility provides a horizontal "reading shelf" that stays pinned to your cursor, making it easier to track lines of text in dense academic papers or long code files.

## Features
- The ruler's bottom edge is anchored to your mouse tip.
- Minimalist interface that stays out of your way. The ruler is a "ghost window" - it won't clutter your taskbar or Alt-Tab menu.
- Uses pre-multiplied alpha blending to ensure the highlighter transparency easy modification.

## Dynamic Customization:
- Adjust thickness for different font sizes.
- Change opacity for light or dark mode environments.
- Custom ARGB color picker to find your most comfortable focus shade.
- Persistent Settings: Automatically saves your preferences to ~/.reading_guide_config.

## Installation (Debian/Ubuntu)

- Download the reading-guide.deb file from the assets below.
- Open your terminal in the download folder and run:
`sudo apt install ./reading-guide.deb`
- Launch Reading Guide from your application menu.

## Technical info
Language: C

**Graphics:** X11 (Xlib) with XShape extensions
**UI:** GTK+ 3.0
**Threading**: POSIX Threads (pthreads) for decoupled UI and ruler rendering.
