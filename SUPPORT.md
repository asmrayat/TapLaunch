# Support

This guide covers installation, compatibility, and common troubleshooting steps for TapLaunch.

## Contact

For help not covered here, email [info@asmlab.agency](mailto:info@asmlab.agency).

Please include:

- TapLaunch version (for example, `v1.0.0`)
- macOS version (for example, `macOS 14.5`)
- MacBook model (for example, `MacBook Air M2`)
- A short description of the issue and steps to reproduce it

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

TapLaunch detects gentle physical taps on the MacBook itself. If your Mac is not in the supported list above, TapLaunch may not work as expected.

---

## Installation

1. Download `TapLaunch.dmg` from the [latest GitHub Release](https://github.com/asmrayat/TapLaunch/releases/latest).
2. Open the downloaded `.dmg` file.
3. Drag **TapLaunch** into your **Applications** folder.
4. Eject the disk image.
5. Open **TapLaunch** from Applications.
6. If macOS blocks the app on first launch, go to **System Settings → Privacy & Security** and choose **Open Anyway**.
7. When TapLaunch prompts you to install the sensor helper, approve the installation. macOS will ask for your administrator password.
8. Open TapLaunch settings from the menu bar and choose apps for double tap and triple tap.

---

## Troubleshooting

### Taps are not detected

1. Confirm your Mac is a supported Apple Silicon MacBook running macOS 14 or later.
2. Make sure TapLaunch is running and detection is not paused in the menu bar.
3. Open settings and use the **tap test tool** to verify whether taps are being recognized.
4. Try increasing sensitivity (Low → Medium → High) or adjusting the manual threshold.
5. Use **gentle taps** on the MacBook body or lid area. Hard hits are not required and may reduce reliability.
6. Verify the sensor helper is installed. If needed, reinstall it from TapLaunch settings.
7. Quit and relaunch TapLaunch after changing sensitivity or helper settings.

### macOS blocks TapLaunch or shows a security warning

1. Open **System Settings → Privacy & Security**.
2. Scroll to the security section and click **Open Anyway** if TapLaunch is listed.
3. If the app was downloaded from the browser and macOS quarantined it, you can remove the quarantine attribute from Terminal:

   ```bash
   xattr -d com.apple.quarantine /Applications/TapLaunch.app
   ```

   Only run this command if you downloaded TapLaunch from the official GitHub Releases page.

4. Make sure you are using a release build distributed through [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases), not an unsigned copy from an unknown source.

### Helper installation fails or taps stop working after an update

1. Open TapLaunch settings and reinstall the sensor helper.
2. Enter your administrator password when macOS prompts you.
3. Restart TapLaunch after installation completes.
4. If problems continue, quit TapLaunch, restart your Mac, and launch TapLaunch again.

### The wrong app opens, or no app opens

1. Open TapLaunch settings and confirm the correct apps are assigned to double tap and triple tap.
2. Use the test buttons in settings to verify each assignment.
3. Make sure the target app is installed and available in `/Applications` or your user Applications folder.
4. If the selected app is already running, TapLaunch should bring it to the front rather than launching a new instance.

### TapLaunch does not appear in the menu bar

1. Check whether TapLaunch is running in Activity Monitor.
2. Relaunch TapLaunch from Applications.
3. If you enabled **Launch at login**, log out and back in, then check the menu bar again.

---

## Uninstall

1. Quit TapLaunch from the menu bar.
2. Remove `TapLaunch.app` from your Applications folder.
3. If you installed the sensor helper, remove it using the uninstall option in TapLaunch settings before deleting the app, or follow the helper removal steps shown in the app.

---

## Release Notes and Downloads

- [CHANGELOG.md](CHANGELOG.md)
- [GitHub Releases](https://github.com/asmrayat/TapLaunch/releases)
- [README.md](README.md)
