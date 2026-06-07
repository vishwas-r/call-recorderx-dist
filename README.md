# 🎙️ Call RecorderX

**Call RecorderX** is a secure, offline, local-first automatic two-way call logging application for Android. Engineered with privacy as the core priority, the app runs entirely on your device with zero cloud dependencies, zero analytics trackers, and zero internet permissions.

---

## ✨ Features

*   **🔒 Privacy-First Architecture**: Audio encoding, processing, and storage are done entirely on-device. The app does not send any telemetry or voice data to any remote servers.
*   **⚙️ Automatic Recording**: Automatically starts recording when a two-way phone call is established.
*   **🛡️ VOIP Call Recording**: Automatically detects and records audio from 13 popular VOIP apps: WhatsApp, WhatsApp Business, Telegram, Telegram X, Facebook Messenger, Messenger Lite, Signal, Viber, WeChat, Imo, Zoom, Microsoft Teams, Google Meet (Google Chat), Slack, Skype, and Discord for both voice and video calls.
*   **☁️ Scoped Cloud Backup & Two-Way Restore**: Securely backup your recordings to personal Google Drive or Box cloud folders using direct HTTPS transfer. Browse and restore synced cloud recordings back to your device local storage at any time.
*   **🎯 Filter by Caller Type**: Choose to record:
    *   **All Numbers**: Record every call.
    *   **Unknown Only**: Record only callers not in your contact list.
    *   **Known Only**: Record only saved contacts.
*   **🎨 Custom Accent Themes**: Customize the application interface with premium accent colors (Bootstrap Blue, Secondary Grey, Success Green, Danger Red, Warning Yellow, Info Cyan, or Purple) in both Dark Mode and Light Mode.
*   **🔊 Two-Way Audio Optimization**:
    *   **Automatic Speakerphone**: Toggle forcing speakerphone during active calls to guarantee clear capture of the remote caller's voice.
    *   **Audio Gain**: Select sound amplification factors (from `1.0x` up to `4.0x`) to boost distant caller voices.
*   **📂 Multi-Format & Custom Storage**:
    *   Formats: **AMR** (super lightweight, recommended), **AAC** (high quality compression), **MP3** (universal compatibility), or **WAV** (uncompressed raw PCM).
    *   Storage Locations: Save inside the app's secure private directory or export directly to a public folder (e.g. `/Documents/CallRecordings`) for easy transfers to your PC.
*   **🔍 Smart Audio Player & Organizer**:
    *   Instantly search recordings by phone number or contact name.
    *   Filter your library by call direction (Incoming/Outgoing), Starred favorites, or Unknown callers.
    *   Play, favorite, delete, or share audio files directly to external apps via the Android System Share sheet.

---

## 📲 Installation

1.  **Download the APK**: Download the precompiled [call-recorderx.apk](dist/call-recorderx.apk) directly from this repository.
2.  **Allow Unknown Sources**: If prompted by your browser or file manager, toggle the setting to allow installation from unknown sources.
3.  **Install the App**: Tap the APK file to initiate installation.
4.  *(Optional)* **Play Protect Bypass**: Since Call RecorderX uses native Accessibility APIs to extract phone numbers during calls, Google Play Protect might warn you. You can bypass this warning during installation and proceed securely.

---

## 🛠️ Step-by-Step Configuration

To ensure background services operate reliably on modern Android versions, the following permissions and settings must be configured during initial startup:

### 1. Enable Accessibility Connector (Crucial for Caller ID)
Call RecorderX requires the Accessibility service permission to detect caller information dynamically in the background:
1.  Open **Call RecorderX** and tap **Enable Service** on the warning banner.
2.  Find and tap **Call RecorderX Connector**.
3.  Toggle the switch to **On**.

#### 💡 Android 13+ "Restricted Setting" Bypass Steps:
If you are running Android 13 or newer, Google might grey out the Accessibility toggle and show a *"Restricted setting"* dialogue. To bypass this restriction:
1.  Close the accessibility window and go to your phone's main **Settings**.
2.  Go to **Apps** ➔ **All Apps** ➔ **Call RecorderX**.
3.  Tap the **three vertical dots (⋮)** in the top-right corner of the App Info page.
4.  Tap **"Allow restricted settings"** and confirm your device PIN, pattern, or fingerprint.
5.  Re-open Call RecorderX, tap **Enable Service**, and you will now be able to toggle the **Call RecorderX Connector** service successfully!

### 2. Grant Device Permissions
Upon launching, allow the following system prompt permissions:
*   **Microphone**: Required to capture call audio.
*   **Phone/Call Logs**: Needed to detect incoming and outgoing phone calls.
*   **Contacts**: Needed to resolve phone numbers to contact names.

### 3. All Files Storage Access (For Custom Storage Folder)
If you switch the storage location to *Public Documents* or a *Custom Path*:
*   Click the **Grant Storage Access** warning card in Settings.
*   Toggle the switch for Call RecorderX to allow it to create and manage files in public directories.

### 4. Battery Optimization Bypass
To prevent Android's battery-saving engine from terminating the background recorder:
1.  Go to **Settings** ➔ **Battery Optimization** (or search "Battery Optimization").
2.  Select **All Apps** and locate **Call RecorderX**.
3.  Change the preference to **Don't Optimize** or **Unrestricted**.

---

## 🤝 Support and Contact

Developed by **Vishwas R**. Visit [vishwas.me](https://vishwas.me/).