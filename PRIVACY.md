# Privacy Policy

**Last updated:** June 17, 2026

TapLaunch is a native macOS menu bar utility that detects gentle physical taps on supported Apple Silicon MacBooks and opens user-selected apps. This policy explains what TapLaunch does and does not collect.

## Summary

TapLaunch is designed to work locally on your Mac. It does not use a cloud account, does not include analytics, and does not send motion or tap data to a server.

## What TapLaunch Does Not Collect

TapLaunch does **not** collect, store, or transmit:

- Personal information or account data
- Usage analytics or behavioral tracking data
- Microphone audio
- Camera images or video
- Keyboard input or keystrokes
- Trackpad clicks or pointer input
- Motion sensor data sent to a remote server
- Location data
- Advertising identifiers

There is no TapLaunch account, no cloud sync, and no third-party analytics SDKs in the app.

## How Tap Detection Works

On supported Apple Silicon MacBooks, TapLaunch uses the MacBook's built-in motion sensor path to detect gentle physical taps. All tap detection and gesture processing happens **locally on your Mac**.

Motion data used for tap detection is processed on-device to recognize double-tap and triple-tap patterns. It is not uploaded, shared, or stored on external servers.

## Local Helper Architecture

macOS does not provide a simple public tap-sensor API for MacBooks. To access motion sensor reports reliably in the background, TapLaunch uses a small **local helper** that runs on your Mac.

The helper:

- Reads local motion sensor reports on your device
- Sends only clean tap event signals (for example, double tap or triple tap) back to the TapLaunch menu bar app through local inter-process communication

The helper does **not**:

- Open applications directly
- Run scripts or shell commands
- Connect to the internet
- Send motion data to external servers
- Access your microphone, camera, keyboard, or trackpad

Only the main TapLaunch app opens the apps you select in settings.

## Settings and Preferences

Your app selections, sensitivity settings, and other preferences are stored locally on your Mac. TapLaunch does not sync these settings to the cloud.

## Internet Access

TapLaunch is not designed to require an internet connection for core functionality. The app and its local helper do not connect to TapLaunch servers for tap detection, analytics, or account services.

## Children's Privacy

TapLaunch does not knowingly collect personal information from anyone, including children.

## Changes to This Policy

If this privacy policy changes, the updated version will be published in this repository. Material changes will be reflected in release notes when appropriate.

## Contact

If you have questions about this privacy policy, contact [info@asmlab.agency](mailto:info@asmlab.agency).
