# 📱 QR Codex

**QR Codex** is a beginner-friendly Flutter/Dart Android app for **scanning, creating, and managing QR codes and barcodes** — with a clean interface, local scan history, and multiple QR generation options.

> 🔐 **No login • No backend • No paid API**

## 📥 Download

**Get the latest Android APK:**

👉 https://github.com/sami-mirza2005/QR-Codex/releases

Download the latest release and install **QR Codex** directly on your Android device.

---

## ✨ Features

### 📷 QR & Barcode Scanner

* Scan QR codes and barcodes
* Real-time camera scanning
* Front / back camera switching
* Flashlight support
* View scan results
* Open URLs directly
* Share scan results

### 🧾 QR Code Generator

Create QR codes for:

* 📝 Text
* 🌐 Website URL
* 📶 Wi-Fi
* 👤 Contact / vCard
* 📧 Email
* 📞 Phone
* 💬 SMS

### 🕘 Scan History

* Automatically save scan history locally
* View previous scans
* Delete individual scans
* Clear all scan history
* Share saved results

### 🎨 Themes

Choose between:

* ☀️ Light mode
* 🌙 Dark mode
* 🖥️ System default

### 🔒 Privacy & Architecture

* No account or login required
* No backend server
* No paid APIs
* Scan history stored locally on the device
* Uses `SharedPreferences` for local storage

---

## 🛠️ Tech Stack

| Technology            | Purpose              |
| --------------------- | -------------------- |
| **Flutter**           | Mobile app framework |
| **Dart**              | Programming language |
| **SharedPreferences** | Local scan history   |
| **Android**           | Target platform      |

---

## 📂 Project Structure

```text
lib/
├── main.dart
├── home_page.dart
├── scanner_page.dart
├── generator_page.dart
├── history_page.dart
└── storage.dart
```

### 📄 File Responsibilities

* `main.dart` — App entry point and theme management
* `home_page.dart` — Home screen, bottom navigation, and settings
* `scanner_page.dart` — Camera scanning and scan results
* `generator_page.dart` — QR code generation
* `history_page.dart` — Scan history management
* `storage.dart` — Local history storage and retrieval

---

## 🚀 Run Locally

### 1. Prerequisites

Install:

* Flutter SDK
* Dart SDK
* VS Code
* Flutter & Dart extensions for VS Code
* Android device or emulator

### 2. Clone the Repository

```bash
git clone https://github.com/sami-mirza2005/QR-Codex.git
```

Open the project folder in VS Code.

### 3. Install Dependencies

Open the VS Code terminal and run:

```bash
flutter pub get
```

### 4. Connect an Android Device

Connect your Android phone using USB and enable **USB Debugging**.

Check whether Flutter detects your device:

```bash
flutter devices
```

### 5. Run the App

```bash
flutter run
```

---

## 📷 Android Camera Permission

QR Codex requires camera access for QR and barcode scanning.

Open:

```text
android/app/src/main/AndroidManifest.xml
```

Add the following permission directly inside `<manifest>` and before `<application>`:

```xml
<uses-permission android:name="android.permission.CAMERA"/>
```

Make sure the application label is:

```xml
android:label="QR Codex"
```

---

## 📦 Build APK

To create a release APK:

```bash
flutter build apk --release
```

The generated APK will be available at:

```text
build/app/outputs/flutter-apk/app-release.apk
```

You can then install the APK on an Android device or upload it to the GitHub Releases page.

---

## 🎯 Supported QR Formats

| Type            | Supported |
| --------------- | :-------: |
| Text            |     ✅     |
| Website URL     |     ✅     |
| Wi-Fi           |     ✅     |
| Contact / vCard |     ✅     |
| Email           |     ✅     |
| Phone           |     ✅     |
| SMS             |     ✅     |

---

## 🔐 Privacy

QR Codex does not require an account and does not use a backend server.

Scan history is stored locally on the user's device using `SharedPreferences`.

---

## 👨‍💻 Developer

**Sami Mirza**

Built with **Flutter & Dart** as a learning and development project focused on mobile application development.

---

## ⭐ Support

If you find **QR Codex** useful, consider giving the repository a ⭐ on GitHub.

Your support is appreciated! 🚀

---

### 📱 QR Codex

**Scan. Create. Store. Share.**

Built with ❤️ using Flutter & Dart.
