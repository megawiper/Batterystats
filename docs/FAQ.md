<div align="center">
<img src="../assets/headers/FAQ.svg" alt="FAQ" width="100%"/>
</div>

<div align="center">

<sub><a href="../README.md">Home</a> &nbsp;·&nbsp; <a href="../docs/FEATURES.md">Features</a> &nbsp;·&nbsp; <a href="../docs/FAQ.md">FAQ</a> &nbsp;·&nbsp; <a href="../docs/PERMISSIONS.md">Permissions</a> &nbsp;·&nbsp; <a href="../PRIVACY.md">Privacy</a> &nbsp;·&nbsp; <a href="../docs/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp; <a href="../CHANGELOG.md">Changelog</a> &nbsp;·&nbsp; <a href="../SECURITY.md">Security</a></sub>

</div>

> [!TIP]
> Tap a question to open the answer.

<details>
<summary><b>Why is the wattage different from my charger's label?</b></summary>

The app shows power flowing into the battery (voltage multiplied by current). That is lower than what the charger delivers at the wall, and no Android phone can measure the wall-side figure.

</details>

<details>
<summary><b>Why does a value say "Not available on this device"?</b></summary>

Android only exposes some fields on some devices and versions. Cycle count needs Android 14 or newer, and most phones do not report design capacity. The app shows that plainly instead of guessing.

</details>

<details>
<summary><b>Why is my charging speed "TRICKLE"?</b></summary>

Power below 2.5 W is always classed as trickle. Common causes are a nearly full battery, a weak charger or cable, or a phone that is using a lot of power while the screen is on.

</details>

<details>
<summary><b>Can the app stop charging at 80%?</b></summary>

No. Android does not allow apps to stop charging. The stop-charging reminder alerts you to unplug at the level you choose.

</details>

<details>
<summary><b>The Usage screen is empty.</b></summary>

Grant *Usage access* to the app in system settings. See [`PERMISSIONS.md`](PERMISSIONS.md).

</details>

<details>
<summary><b>Statistics say 0 sessions.</b></summary>

Sessions are recorded while charging with monitoring active. Turn on *Auto-start monitoring on charge* in Settings and plug in your charger.

</details>

<details>
<summary><b>Why does the app show a notification?</b></summary>

The Always-On Charging Monitor runs as a foreground service, and Android requires a visible notification for it. Turn it off in Settings if you do not want it.

</details>

<details>
<summary><b>Does it work on an emulator?</b></summary>

It installs, but emulators simulate a static battery, so numbers will not be meaningful. Use a physical phone.

</details>

<details>
<summary><b>Does the app send my data anywhere?</b></summary>

No. It has no internet permission. See [`PRIVACY.md`](../PRIVACY.md).

</details>

<details>
<summary><b>Can I reuse the code or design?</b></summary>

No. All rights are reserved. See [`LICENSE`](../LICENSE).

</details>


<div align="center">
<img src="../assets/footer-wave.svg" alt="" width="100%"/>
</div>
