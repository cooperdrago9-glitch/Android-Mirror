# AndroidMirror

A Windows 11 ARM64 desktop app for mirroring Android devices over USB with ADB and scrcpy.

## Features

- Auto-detects Android devices over USB
- Mirrors multiple devices simultaneously, each in their own window
- 120fps, 8Mbps streaming with audio by default
- Configurable bitrate, FPS, resolution, and audio via settings
- Always on top option per session
- System tray support
- Installs system-wide to Program Files

## Requirements

- Windows 11 ARM64
- Android device with USB debugging enabled

## How to enable USB debugging

1. Go to Settings → About Phone
2. Tap Build Number 7 times
3. Go to Settings → Developer Options
4. Enable USB Debugging
5. Plug in via USB and tap Allow on the prompt that appears

## Installation

Download the latest installer from the releases page and run it. Admin privileges are required.

## Building from source

### Prerequisites

- Node.js (ARM64)
- Visual Studio Build Tools with Desktop development with C++
- Python 3

### Steps
```bash
git clone https://github.com/yourusername/android-mirror
cd android-mirror
npm install
npm run dev
```

To package:
```bash
npm run dist
```

The installer will be output to `release/`.

## Tech stack

- Electron
- React
- TypeScript
- Vite
- @devicefarmer/adbkit
- scrcpy

## License

MIT
