# Jamf Scripts

[![Buy me a coffee](https://img.buymeacoffee.com/button-api/?text=Buy%20me%20a%20coffee&emoji=&slug=russcollis&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff)](https://www.buymeacoffee.com/russcollis)

Useful scripts for managing Macs with Jamf Pro.

**Owner:** Russell Collis

## Scripts

| Script | What it does |
|---|---|
| [Deploy Blocked Binary Notifier](Deploy%20Blocked%20Binary%20Notifier) | Installs a LaunchDaemon that watches for apps blocked by a managed binary execution control policy and shows the user a swiftDialog notification explaining what was blocked. Also installs a watchdog that keeps the notifier protected and running. See the [deployment readme](Blocked%20Binary%20Notifier%20Deployment%20Readme) for details. |
| [Bundle ID Scanner.sh](Bundle%20ID%20Scanner.sh) | Interactive lookup of app identifiers and code-signing information, with CSV export. Originally by Anthony Darlow (CantScript), with additions by Russell Collis. |
| [extract_mac_app_icons.sh](extract_mac_app_icons.sh) | Extracts icons from `.app` bundles, `.pkg` installers and `.dmg` disk images into PNG files, and writes a summary of what was extracted, skipped or missing. |

## Usage

Upload a script to Jamf Pro under **Settings → Computer Management → Scripts** and run it from a policy, or run it locally on a Mac:

```bash
sudo bash "<script name>"
```

The Blocked Binary Notifier needs [swiftDialog](https://github.com/swiftDialog/swiftDialog) installed to show notifications.
