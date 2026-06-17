# TapLaunch

**Tap your MacBook. Launch your apps.**

TapLaunch is a native macOS menu bar utility that lets you open selected Mac apps using gentle physical double taps and triple taps on supported Apple Silicon MacBooks.

This repository provides downloads, documentation, and release notes for TapLaunch. It does not contain application source code.

---

## Download

**[Download TapLaunch for macOS](https://github.com/asmrayat/TapLaunch/releases/latest/download/TapLaunch.dmg)**

Direct link:

```
https://github.com/asmrayat/TapLaunch/releases/latest/download/TapLaunch.dmg
```

Browse all releases: [github.com/asmrayat/TapLaunch/releases](https://github.com/asmrayat/TapLaunch/releases)

The app is distributed as a `.dmg` file attached to [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases). The installer is not stored in this repository.

---

## What TapLaunch Does

TapLaunch runs quietly from your menu bar and listens for gentle MacBook motion taps. Assign one app to double tap and another to triple tap, then bring your most-used tools to the front without reaching for the Dock, Spotlight, or keyboard shortcuts.

- Double tap to open or bring forward one selected app
- Triple tap to open or bring forward a second selected app
- Adjustable sensitivity and a built-in tap test tool
- Launch at login support
- Local-only settings and on-device tap detection

---

## Compatibility

### Supported

- Apple Silicon MacBook Air
- Apple Silicon MacBook Pro
- macOS 14 (Sonoma) or later

### Not Supported

- Intel MacBooks
- Mac mini
- Mac Studio
- iMac
- External keyboards
- External trackpads

TapLaunch detects gentle physical taps on the MacBook itself. It is designed for built-in motion sensor paths available on supported Apple Silicon MacBooks.

---

## How to Install

1. Download `TapLaunch.dmg` from the [latest release](https://github.com/asmrayat/TapLaunch/releases/latest).
2. Open the downloaded `.dmg` file.
3. Drag **TapLaunch** into your **Applications** folder.
4. Launch TapLaunch from Applications.
5. If macOS shows a security prompt, open **System Settings → Privacy & Security** and choose **Open Anyway** for TapLaunch.
6. When prompted, install the local sensor helper. macOS will ask for your administrator password because the helper runs as a system service for reliable background sensor access.
7. Choose your double-tap and triple-tap apps from the menu bar or settings window.

For detailed troubleshooting, see [SUPPORT.md](SUPPORT.md).

---

## How It Works

1. Choose an app for double tap.
2. Choose an app for triple tap.
3. Keep TapLaunch listening in the menu bar.
4. Gently double tap or triple tap your MacBook.
5. TapLaunch opens the selected app or brings it to the front if it is already running.

### Why a Local Helper Is Needed

macOS does not provide a simple public tap-sensor API for MacBooks. On supported Apple Silicon MacBooks, TapLaunch uses a small **local helper** to access motion sensor reports reliably in the background.

The helper only reads local motion data and sends clean tap events back to TapLaunch. It does not open apps directly, run scripts, or connect to the internet. See [PRIVACY.md](PRIVACY.md) for details.

---

## Privacy Summary

TapLaunch is designed to stay local and private:

- No microphone
- No camera
- No keyboard input tracking
- No trackpad click tracking
- No analytics
- No cloud account
- No motion data sent to a server
- Tap detection happens locally on your Mac

Full details: [PRIVACY.md](PRIVACY.md)

---

## Safety Note

Use **gentle taps only**. TapLaunch is designed for light physical gestures on your MacBook, not hard hits or slaps. Excessive force is unnecessary and may affect detection reliability.

---

## FAQ

### Does TapLaunch use the microphone?

No. TapLaunch does not listen to sound. It uses supported MacBook motion sensor data processed locally on your device.

### Does it work with external keyboards or trackpads?

No. TapLaunch detects gentle physical taps on the MacBook itself. External keyboards and trackpads are not supported.

### Why does TapLaunch need a helper?

The helper gives TapLaunch reliable background access to the MacBook motion sensor path. The helper is local-only and does not open apps, run commands, or connect to the internet.

### What happens if the selected app is already open?

TapLaunch brings it to the front.

### Can I pause detection?

Yes. Detection can be paused from the menu bar or settings window.

### Does TapLaunch work on Intel MacBooks?

No. TapLaunch is designed for Apple Silicon MacBook Air and MacBook Pro models running macOS 14 or later.

---

## Support

- Documentation: [SUPPORT.md](SUPPORT.md)
- Email: [info@asmlab.agency](mailto:info@asmlab.agency)

---

## Release Notes

- [CHANGELOG.md](CHANGELOG.md)
- [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases)

---

## Legal

- [Privacy Policy](PRIVACY.md)
- [End User License Agreement](EULA.md)
- [License](LICENSE.md)
- [Security Policy](SECURITY.md)

---

## About This Repository

This is a **public product and download repository** for TapLaunch users. It contains documentation, legal policies, and links to signed release downloads. Application source code, build tooling, and private implementation files are not published here.
