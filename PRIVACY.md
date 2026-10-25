<div align="center">
<img src="assets/headers/PRIVACY.svg" alt="PRIVACY" width="100%"/>
</div>

<div align="center">

<sub><a href="README.md">Home</a> &nbsp;·&nbsp; <a href="docs/FEATURES.md">Features</a> &nbsp;·&nbsp; <a href="docs/FAQ.md">FAQ</a> &nbsp;·&nbsp; <a href="docs/PERMISSIONS.md">Permissions</a> &nbsp;·&nbsp; <a href="PRIVACY.md">Privacy</a> &nbsp;·&nbsp; <a href="docs/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp; <a href="CHANGELOG.md">Changelog</a> &nbsp;·&nbsp; <a href="SECURITY.md">Security</a></sub>

</div>

> [!IMPORTANT]
> **No `INTERNET` permission. No networking code. No accounts. No ads. No analytics.**
> Battery Stats works fully in airplane mode, and you can [verify that yourself](README.md#-verify-it-yourself).

Battery Stats is designed to keep your data on your device.

## What the app reads

- Battery level, voltage, current, temperature, health, chemistry and charging status from Android's `BatteryManager` and battery broadcasts
- App screen-time statistics from `UsageStatsManager`, only after you grant *Usage access* in system settings

## Where data is stored

- Charging sessions, samples and drain samples live in a local Room (SQLite) database
- Settings and per-app limits live in local DataStore files
- Nothing is uploaded by the app. It has no `INTERNET` permission and contains no networking code

## Exports

CSV, PDF and SVG files are created on your device. They leave the device only when you pick a destination in the system share sheet.

## Android device backup

The manifest allows Android's own backup system. Depending on your phone's backup settings, Android may include the app's local database and settings in your device backup. That process is controlled by Android and your Google account, not by this app. You can turn it off in your phone's backup settings.

## Permissions

See [`docs/PERMISSIONS.md`](docs/PERMISSIONS.md) for what each permission does.

## Questions

Email yash92726@gmail.com.


<div align="center">
<img src="assets/footer-wave.svg" alt="" width="100%"/>
</div>
