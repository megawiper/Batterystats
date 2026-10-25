<div align="center">
<img src="../assets/headers/PERMISSIONS.svg" alt="PERMISSIONS" width="100%"/>
</div>

<div align="center">

<sub><a href="../README.md">Home</a> &nbsp;·&nbsp; <a href="../docs/FEATURES.md">Features</a> &nbsp;·&nbsp; <a href="../docs/FAQ.md">FAQ</a> &nbsp;·&nbsp; <a href="../docs/PERMISSIONS.md">Permissions</a> &nbsp;·&nbsp; <a href="../PRIVACY.md">Privacy</a> &nbsp;·&nbsp; <a href="../docs/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp; <a href="../CHANGELOG.md">Changelog</a> &nbsp;·&nbsp; <a href="../SECURITY.md">Security</a></sub>

</div>

> [!NOTE]
> Only six permissions, none of them for networking, location, camera, microphone, contacts or storage.

Battery Stats declares the following permissions in `AndroidManifest.xml`.

| Permission | Type | Used for |
|---|---|---|
| `POST_NOTIFICATIONS` | Runtime (Android 13+) | Charging alerts and the monitoring notification |
| `FOREGROUND_SERVICE` | Normal | Running the Always-On Charging Monitor |
| `FOREGROUND_SERVICE_DATA_SYNC` | Normal | Foreground service type for the monitor |
| `RECEIVE_BOOT_COMPLETED` | Normal | Restarting monitoring after reboot |
| `REQUEST_IGNORE_BATTERY_OPTIMIZATIONS` | Normal | Lets the app ask to be exempt from battery optimization so monitoring survives in the background |
| `PACKAGE_USAGE_STATS` | Special access | Screen time and per-app usage. You enable it in *Settings → Apps → Special access → Usage access* |

## Not requested

- `INTERNET`: the app has no network access
- Location, contacts, camera, microphone, storage or phone permissions

## Why the monitor needs a notification

Android requires a foreground service to show a persistent notification while it runs. You can turn the Always-On Charging Monitor off in Settings.

## Revoking access

Usage access can be revoked at any time in system settings. The Usage screen will then stop showing per-app data; the rest of the app keeps working.


<div align="center">
<img src="../assets/footer-wave.svg" alt="" width="100%"/>
</div>
