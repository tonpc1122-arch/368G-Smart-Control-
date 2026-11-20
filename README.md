# 368G Smart Control V1

Android prototype for Zontes 368G V1 (2025).

## Current scope
- Requests Android Bluetooth permissions.
- Scans nearby Bluetooth Low Energy (BLE) advertisements.
- Displays discovered device names, addresses, and signal strength (RSSI).
- Does **not** connect to, authenticate with, or send commands to the motorcycle.

## Build APK with GitHub Actions
1. Create a new GitHub repository.
2. Upload all files and folders from this project to the repository root.
3. Open the **Actions** tab and enable workflows if GitHub asks.
4. Select **Build 368G Smart Control APK**.
5. Press **Run workflow** (or push to `main`).
6. Open the completed run and download the artifact named `368G-Smart-Control-debug`.
7. Extract the ZIP and install `app-debug.apk` on your Samsung phone.

## Phone test
- Turn on Bluetooth.
- Open the app and grant Bluetooth permissions.
- Press **ค้นหา Bluetooth รอบตัว**.
- Keep the motorcycle powered on and close to the phone.
- Send screenshots of the discovered device list for analysis.

## Safety and compatibility
The motorcycle's BLE service UUIDs, pairing flow, authentication, and command protocol have not yet been verified. Do not send guessed commands or modify the CAN bus, immobilizer, or keyless wiring. Actual remote control requires a verified, authorized protocol and safe testing.
