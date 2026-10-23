# BTP Screen Control

<p align="center">
  <img src="./logo.png" alt="BTP Screen Control Logo" width="160">
</p>

<h2 align="center">BTP Screen Control</h2>

<p align="center">
  <strong>Mirror and Control Your Android Phone from Windows</strong>
</p>

<p align="center">
  A dedicated Windows desktop application for discovering Android devices, mirroring phone screens, and controlling your phone directly from your PC or laptop.
</p>

<p align="center">
  <a href="https://github.com/BasicTouchPro/BTP-screen-mirror-and-control/releases/latest/download/BTP.Screen.Control_0.2.0_x64-setup.exe">
    <img src="https://img.shields.io/badge/⬇%20Download-Windows%20Installer-00C9D8?style=for-the-badge" alt="Download BTP Screen Control">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows 10 and 11">
  <img src="https://img.shields.io/badge/Architecture-x64-blue?style=flat-square" alt="64-bit">
  <img src="https://img.shields.io/badge/Version-0.2.0-00C9D8?style=flat-square" alt="Version 0.2.0">
  <img src="https://img.shields.io/badge/Connection-USB%20%7C%20Wi--Fi-64748B?style=flat-square" alt="USB and Wi-Fi">
</p>

<p align="center">
  <a href="https://www.youtube.com/@BasicTouchPro">
    <img src="https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Subscribe on YouTube">
  </a>
  &nbsp;
  <a href="https://t.me/BasicTouchPro">
    <img src="https://img.shields.io/badge/Telegram-Join%20Channel-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Join Telegram">
  </a>
</p>

---

## Overview

**BTP Screen Control** is a Windows desktop application developed by [BasicTouchPro](https://www.youtube.com/@BasicTouchPro) to make Android device connectivity, screen mirroring, and phone control accessible through a single desktop workspace.

The application helps you discover Android devices connected through USB or supported wireless connections and launch a dedicated control window powered by the official scrcpy distribution.

Whether you use a desktop computer or a laptop, BTP Screen Control provides a convenient way to interact with your Android phone from Windows.

## Features

- **Screen Mirroring** — View your Android phone's screen on your computer.
- **Phone Control from PC** — Control your Android device through a separate scrcpy window.
- **USB Connection** — Discover and manage Android devices connected through a USB data cable.
- **Wi-Fi Connection** — Pair and connect supported devices using Android Wireless Debugging.
- **QR Code Pairing** — Generate a QR code for supported wireless pairing workflows.
- **Bluetooth PAN Networking** — Attempt an ADB network connection through Bluetooth tethering when supported by your phone and network.
- **Bluetooth LE Discovery** — Scan nearby Bluetooth Low Energy advertisements and inspect available device details.
- **Device Management** — Refresh device lists and manage devices hidden from the application's list.
- **Dark and Light Themes** — Choose your preferred application appearance.
- **Resource Diagnostics** — Check the availability of required ADB and scrcpy resources.
- **Local Connection Design** — Device control is designed around local connections, without a dedicated remote-control server.

## Download

### Latest Release — v0.2.0

<p align="center">
  <a href="https://github.com/BasicTouchPro/BTP-screen-mirror-and-control/releases/latest/download/BTP.Screen.Control_0.2.0_x64-setup.exe">
    <img src="https://img.shields.io/badge/Download%20BTP%20Screen%20Control-v0.2.0-00C9D8?style=for-the-badge&logo=windows&logoColor=white" alt="Download Windows installer">
  </a>
</p>

**Installer:** `BTP.Screen.Control_0.2.0_x64-setup.exe`

- **Operating System:** Windows 10 or Windows 11
- **Architecture:** 64-bit (x64)
- **Package Type:** Windows installer (.exe)
- **Device Support:** Compatible Android phones

The application has been tested on Windows 10 and Windows 11.

For version history and other available downloads, visit the [GitHub Releases page](https://github.com/BasicTouchPro/BTP-screen-mirror-and-control/releases).

> The direct download link works when the matching installer is uploaded to a published GitHub Release. If you rename the installer, update the link accordingly.

## Screenshots

The following screenshots illustrate the main sections of BTP Screen Control.

### Overview

![BTP Screen Control Overview](./screenshots/overview.png)

### USB Devices

![USB device management](./screenshots/usb-devices.png)

### Wi-Fi Connection

![Wi-Fi connection and QR pairing](./screenshots/wifi.png)

### Bluetooth Discovery

![Bluetooth Low Energy discovery](./screenshots/bluetooth.png)

### Settings and Diagnostics

![Settings, resources and diagnostics](./screenshots/settings.png)

> To display these images, upload your screenshots to the `screenshots/` folder using the filenames specified above. You can remove this section if you do not want to publish screenshots.

## System Requirements

- Windows 10 or Windows 11, 64-bit.
- A compatible Android phone or tablet.
- A USB data cable for wired connections, or a supported wireless connection.
- Android USB debugging or Wireless Debugging configured for the selected connection method.
- The application's required ADB and scrcpy resources.

Some Android devices may require a manufacturer-specific USB driver. Wireless connectivity can depend on network configuration and Windows Firewall settings.

## Installation

1. Open the [latest release download](https://github.com/BasicTouchPro/BTP-screen-mirror-and-control/releases/latest/download/BTP.Screen.Control_0.2.0_x64-setup.exe).
2. Download `BTP.Screen.Control_0.2.0_x64-setup.exe`.
3. Run the installer and follow the on-screen instructions.
4. Launch BTP Screen Control.
5. Connect your Android device using USB or a supported wireless connection.
6. Follow the instructions shown in the application.

If Windows displays a security warning, verify that the installer came from this repository before proceeding. The project does not claim that the installer is code-signed.

## How to Connect Your Android Phone

### USB Connection

1. Open **Settings → About phone** on your Android device.
2. Enable **Developer options** and **USB debugging**.
3. Connect your phone to the PC using a data-capable USB cable.
4. Unlock the phone and approve the USB debugging authorization prompt.
5. Open BTP Screen Control and select **USB devices**.
6. Refresh the device list and launch the control window.

If the device status shows `unauthorized`, approve the debugging authorization prompt on your phone.

### Wi-Fi Connection

BTP Screen Control supports wireless connection workflows for compatible Android devices.

1. Connect your PC and Android phone to the same trusted Wi-Fi network.
2. On Android 11 or later, open **Developer options → Wireless debugging**.
3. Choose **Pair device with QR code**.
4. In BTP Screen Control, open **Wi-Fi**.
5. Select **Generate QR code for phone**.
6. Scan the displayed QR code using the phone's Wireless Debugging pairing interface.
7. Keep the pairing screen open while the application discovers and connects to the device.

#### Manual Connection

If automatic discovery does not work:

1. Open the phone's main **Wireless debugging** screen.
2. Find the current IP address and connection port.
3. Enter the endpoint in the application's connection field.
4. Select **Connect**.

**Important:** Wireless debugging pairing ports and connection ports are different. Use the connection port when connecting to an already paired device.

Network isolation, firewall rules, and unavailable mDNS discovery can affect wireless connections.

### Bluetooth PAN

Bluetooth LE discovery and Bluetooth PAN networking are different functions.

Bluetooth LE discovery scans for nearby Bluetooth Low Energy advertisements. It does not, by itself, establish an ADB connection or enable screen mirroring.

To attempt an ADB connection through Bluetooth PAN:

1. Pair your Android phone with Windows using Bluetooth settings.
2. Enable Bluetooth tethering on Android if supported.
3. Connect the PC to the phone's Bluetooth Personal Area Network (PAN).
4. Check whether Android exposes ADB and mDNS on that network.
5. If automatic discovery is unavailable, use the current connection IP address and port when supported.

Bluetooth PAN availability depends on the Android device, Windows Bluetooth adapter, and network configuration.

## Privacy and Connectivity

BTP Screen Control is designed to establish local connections between your PC and Android device.

- No account or sign-up is required by the current application design.
- The application is designed around local device connections rather than a dedicated remote-control server.
- Device discovery and control use the configured ADB connection and packaged scrcpy resources.
- Wireless connections may use your local network.
- Bluetooth discovery runs when initiated through the application.

These statements describe the intended design. Users and developers can review the source code and bundled dependencies to verify the application's behaviour.

## Troubleshooting

| Problem | Suggested solution |
|---|---|
| No USB device detected | Check the USB cable, enable USB debugging, and refresh the device list. |
| Device is unauthorized | Unlock the phone and approve the USB debugging RSA prompt. |
| Windows does not detect the phone | Try another data-capable cable or install the manufacturer's official USB driver. |
| Wi-Fi pairing fails | Keep the Wireless Debugging pairing screen open and confirm both devices use the same trusted network. |
| Wireless discovery fails | Check Windows Firewall, local network restrictions, and mDNS availability. |
| Manual Wi-Fi connection fails | Verify the current device IP address and connection port. |
| ADB or scrcpy resources are missing | Restore the complete required resource folders, including helper DLLs and the scrcpy server. |
| The control window closes unexpectedly | Check device authorization, ADB status, resource files, and Settings → Diagnostics. |
| Bluetooth PAN connection fails | Confirm Bluetooth tethering is enabled and that the phone exposes ADB connectivity through the PAN. |
| A removed device is not listed | Use the application's restore action under the removed-device list, if available. |

## Development

BTP Screen Control uses Tauri, React, Rust, and Android device connectivity tools.

### Development Prerequisites

The project documentation specifies these prerequisites:

- Node.js LTS and npm.
- Rust stable with the MSVC target.
- Microsoft C++ Build Tools with **Desktop development with C++**.
- Microsoft Edge WebView2 Runtime.
- The required Android Debug Bridge (ADB) resources.
- The complete official Windows x64 scrcpy distribution, including required DLLs, server files, and notices.

### Run in Development Mode

Open an appropriate Visual Studio developer terminal and run:

```powershell
npm ci
npm run tauri dev
```

Check the frontend and Rust components:

```powershell
npm run build
cargo check --manifest-path src-tauri/Cargo.toml
```

### Build the Windows Installer

Run:

```powershell
npm run tauri build
```

The output location depends on the project's Tauri configuration. Verify the generated installer and all bundled resources before distributing the application.

## Resources and Third-Party Licenses

BTP Screen Control uses third-party software and libraries, including scrcpy, ADB-related resources, React, and Tauri.

Third-party components remain subject to their respective licenses and notices.

- [Project LICENSE](./LICENSE)
- [Third-party license references](./THIRD_PARTY_LICENSES.txt)
- [Resource manifest](./resources/resource-manifest.json), if included in the repository

Preserve upstream license files and notices when distributing third-party binaries. Verify the applicable license terms before redistributing bundled resources.

The bundled ADB executable and helper DLLs should be distributed with their applicable upstream notices. If replacing them with a separately downloaded Android Platform Tools package, review Google's current Android SDK terms.

## Contributing and Feedback

Suggestions, bug reports, and feedback are welcome.

When reporting an issue, include the following information where possible:

- Windows version.
- Android device model and Android version.
- Connection method (USB, Wi-Fi, or Bluetooth PAN).
- Relevant error messages or diagnostic details.

Do not include passwords, private keys, or other sensitive information in issue reports.

## Developer

<p align="center">
  <strong>BasicTouchPro</strong>
</p>

<p align="center">
  <a href="https://www.youtube.com/@BasicTouchPro">
    <img src="https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Subscribe on YouTube">
  </a>
  &nbsp;
  <a href="https://t.me/BasicTouchPro">
    <img src="https://img.shields.io/badge/Telegram-Join%20Channel-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Join Telegram">
  </a>
</p>

<p align="center">
  <a href="https://www.youtube.com/@BasicTouchPro">YouTube Channel</a>
  &nbsp;•&nbsp;
  <a href="https://t.me/BasicTouchPro">Telegram</a>
  &nbsp;•&nbsp;
  <a href="https://github.com/BasicTouchPro/BTP-screen-mirror-and-control/releases">All Releases</a>
</p>

## License

The repository includes an MIT License notice for the project. See [`LICENSE`](./LICENSE) for the full text.

The MIT License does not replace or override the separate licenses governing third-party libraries and bundled resources. Review the relevant upstream notices before redistributing the application.

---

<p align="center">
  Made with care by <a href="https://www.youtube.com/@BasicTouchPro"><strong>BasicTouchPro</strong></a>
</p>
