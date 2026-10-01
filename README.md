# QR Codex

QR Codex is a beginner-friendly Flutter/Dart mobile app for scanning, creating and storing QR/barcode data.

## Features

- QR and barcode scanning
- Flashlight
- Switch front/back camera
- Scan history
- Delete one scan or all scans
- Share scan results
- Create QR codes for:
  - Text
  - Website URL
  - Wi-Fi
  - Contact / vCard
  - Email
  - Phone
  - SMS
- Light / dark / system theme
- Local history using SharedPreferences
- No login
- No backend
- No paid API

## Run in VS Code

1. Install Flutter and the Flutter/Dart extensions.
2. Open this project folder in VS Code.
3. Open the terminal.
4. Run:

```bash
flutter pub get
```

5. Connect your Android phone with USB debugging enabled.
6. Check the device:

```bash
flutter devices
```

7. Run:

```bash
flutter run
```

## Android camera permission

Open:

`android/app/src/main/AndroidManifest.xml`

Add this line directly inside `<manifest>` and before `<application>`:

```xml
<uses-permission android:name="android.permission.CAMERA"/>
```

Also set the application label to:

```xml
android:label="QR Codex"
```

## Project structure

```text
lib/
├── main.dart
├── home_page.dart
├── scanner_page.dart
├── generator_page.dart
├── history_page.dart
└── storage.dart
```

## What each Dart file does

- `main.dart` — starts QR Codex and controls the theme.
- `home_page.dart` — home screen, bottom navigation and settings.
- `scanner_page.dart` — camera scanner and scan result.
- `generator_page.dart` — creates different QR formats.
- `history_page.dart` — displays and manages scan history.
- `storage.dart` — saves/loads history on the phone.

## Build APK

```bash
flutter build apk --release
```

The release APK will be created under:

`build/app/outputs/flutter-apk/app-release.apk`
