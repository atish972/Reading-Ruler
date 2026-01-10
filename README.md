<img width="64" height="64" alt="reading-guide" src="https://github.com/user-attachments/assets/a98c197a-44de-4f28-a513-806e44fb40d6" />

# Reading Guide v1.1.0
**The Stability & Persistence Update**

A high-performance focus engine designed for deep reading. This utility provides a horizontal reading ruler anchored to your cursor, now featuring a decoupled multi-threaded architecture to ensure zero-lag performance even during real-time customization.

## What's New in v1.1.0
- **Total Stability Architecture**: Re-engineered using independent X11 display connections for the HUD and Control Panel. This eliminates UI deadlocks and ensures the settings window never freezes.
- **Advanced Masking Modes**: Beyond the standard strip, you can now toggle "Above," "Below," or "Full Focus" modes to dim the rest of your screen with overlay and isolate the text you are reading.
- **Surgical Precision**: The ruler's bottom edge is mathematically locked to the exact pixel of your mouse tip for seamless tracking.
- **Under-Shadow Rendering**: Optional smooth gradient shadow to provide better visual depth against complex backgrounds.

## Key Features
- **Ghost Window Technology**: The ruler remains non-interactive and invisible to your taskbar and Alt-Tab menu.
- **Persistent Settings**: Automatically saves and restores your thickness, color, and opacity preferences from `~/.reading_guide_config`.
- **Dynamic Customization**: Real-time GTK sliders for thickness and alpha-blending.

## Installation (Debian/Ubuntu)
1. Download the `reading-guide-pkg.deb` file from the assets below.
2. Open your terminal in the download folder and run:
   `sudo apt install ./reading-guide-pkg.deb`
3. Launch **Reading Guide** from your application menu.

## Technical info
- **Language:** C
- **Graphics:** X11 (Xlib) with XShape extensions & Cairo for high-quality rendering.
- **UI:** GTK+ 3.0.
- **Threading:** POSIX Threads (pthreads) with dedicated Display connections for thread-safe UI stability.
