# 💊 Medication Reminder App  
## Smart Medication Scheduling & Daily Reminder System

<div align="center">

### A Modern Flutter Application for Managing Daily Medication Schedules with Local Notifications

Never miss a dose again with an elegant, lightweight, and fully offline medication reminder system built using Flutter.

<br>

![Flutter](https://img.shields.io/badge/Flutter-3.22+-02569B?style=for-the-badge&logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=for-the-badge&logo=dart)
![Android](https://img.shields.io/badge/Android-Supported-3DDC84?style=for-the-badge&logo=android)
![iOS](https://img.shields.io/badge/iOS-Supported-black?style=for-the-badge&logo=apple)
![Notifications](https://img.shields.io/badge/Notifications-Local%20Alerts-orange?style=for-the-badge)
![Material 3](https://img.shields.io/badge/UI-Material%203-purple?style=for-the-badge)

</div>

---

# 📌 Overview

The **Medication Reminder App** is a cross-platform Flutter application designed to help users manage daily medication schedules efficiently and reliably.

The app enables users to:

- Create medication reminders
- Set multiple daily schedules
- Receive local notifications even when the app is closed
- Manage recurring medications
- Automatically remove expired reminders
- Persist medication data locally

This project focuses on building a clean, modern, and practical healthcare utility application with reliable notification scheduling and lightweight local storage architecture.

---

# 🎯 Core Objectives

The application was designed to:

- Improve medication adherence
- Reduce missed doses
- Simplify medication scheduling
- Provide persistent offline reminders
- Deliver a lightweight and responsive experience
- Support both Android and iOS platforms

---

# ✨ Features

# 💊 Medication Management

## Add Medications
Create medication reminders with:

- Medication name
- Dosage instructions
- Reminder times
- Frequency settings
- End date configuration

---

## Edit Existing Medications
Quickly update:

- Dosage
- Reminder schedules
- Notification settings
- Medication duration

---

## Swipe-to-Delete Support
Remove medications instantly using intuitive swipe gestures.

---

# ⏰ Smart Reminder System

## Multiple Reminder Times
Set multiple reminders for a single medication.

Example:

```text
Morning → 8:00 AM
Afternoon → 2:00 PM
Night → 9:00 PM
```

---

## Flexible Frequency Scheduling

Supported reminder frequencies include:

- Daily
- Every X hours
- Ongoing reminders
- Fixed-duration schedules

---

## Background Notifications

The app sends notifications even when:

- The app is closed
- The app is minimized
- The device is idle

powered by:

```text
flutter_local_notifications
```

---

# 🔔 Notification Features

## Exact Alarm Scheduling
Supports highly accurate medication reminders.

## Daily Repeating Notifications
Automatically repeats reminders based on schedule.

## Permission Handling
Requests:

- Notification permissions
- Exact alarm permissions
- Platform-specific alert access

---

# 🧹 Automatic Reminder Cleanup

Expired reminders are automatically removed when the app launches.

This helps:

- Reduce outdated reminders
- Keep schedules organized
- Improve user experience

---

# 🎨 UI & User Experience

The application follows modern **Material 3** design principles.

## UI Highlights

- Clean teal-themed interface
- Responsive layouts
- Smooth navigation
- Minimalistic reminder cards
- Intuitive scheduling flow
- Mobile-first design

---

# 🏗️ System Architecture

```text
User Input
     ↓
Reminder Scheduler
     ↓
Local Storage (Shared Preferences)
     ↓
Notification Engine
     ↓
Background Local Notifications
```

---

# ⚙️ Tech Stack

## Frontend

| Technology | Purpose |
|---|---|
| Flutter | Cross-platform development |
| Dart | Programming language |
| Material 3 | UI design system |

---

## Notifications & Scheduling

| Package | Purpose |
|---|---|
| flutter_local_notifications | Local notifications |
| timezone | Timezone management |
| permission_handler | Runtime permissions |

---

## Local Storage

| Package | Purpose |
|---|---|
| shared_preferences | Persistent local storage |

---

# 📂 Project Structure

```text
lib/
│
├── main.dart
│
└── screens/
    ├── addmed.dart
    ├── reminders.dart
    └── remindersettings.dart
```

---

# 🚀 Getting Started

# 📋 Prerequisites

Before running the project, ensure the following are installed:

- Flutter SDK 3.22+
- Dart SDK
- Android Studio / VS Code
- Xcode (for iOS)
- Android Emulator / Physical Device

---

# 📥 Installation

## Clone Repository

```bash
git clone <your-repository-url>
cd medication-reminder-app
```

---

## Install Dependencies

```bash
flutter pub get
```

---

## Run the Application

```bash
flutter run
```

---

# 📦 Required Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter

  flutter_local_notifications: ^17.2.3
  timezone: ^0.9.4
  shared_preferences: ^2.3.2
  permission_handler: ^11.3.1
```

---

# ⚙️ Android Configuration

# 🔔 Exact Alarm Permission

Add the following permission inside:

```text
android/app/src/main/AndroidManifest.xml
```

```xml
<uses-permission android:name="android.permission.SCHEDULE_EXACT_ALARM" />
```

---

# ⚡ Gradle Configuration

Update:

```text
android/app/build.gradle.kts
```

with:

```kotlin
compileOptions {
    sourceCompatibility = JavaVersion.VERSION_17
    targetCompatibility = JavaVersion.VERSION_17
    isCoreLibraryDesugaringEnabled = true
}

dependencies {
    coreLibraryDesugaring("com.android.tools:desugar_jdk_libs:2.1.5")
}
```

---

# 📱 Application Workflow

```text
Launch App
      ↓
Create Medication
      ↓
Configure Reminder Time
      ↓
Grant Notification Permissions
      ↓
Save Reminder
      ↓
Background Notification Trigger
```

---

# 📌 Usage Guide

## Step 1
Launch the application.

---

## Step 2
Navigate to the **Reminders** screen.

---

## Step 3
Tap the **+ Add Medication** button.

---

## Step 4
Configure:

- Medication name
- Dosage
- Reminder times
- Frequency
- Duration

---

## Step 5
Save the reminder.

Notifications will continue working even if the app is closed.

---

# 🧪 Testing Notifications

## Recommended Testing Method

- Schedule reminder 1–2 minutes ahead
- Background the application
- Wait for notification trigger

---

# ⚠️ Troubleshooting

# 🔕 Notifications Not Showing?

## Check the Following

- Notification permissions granted
- Exact alarms enabled (Android 12+)
- Physical device testing preferred
- App battery optimization disabled if necessary

---

# 🛠️ Build Errors

Run:

```bash
flutter clean
flutter pub get
```

---

# 🍎 iOS Notes

Ensure required notification permissions are configured properly inside:

```text
Info.plist
```

---

# 📜 Logs & Debugging

Verbose logging:

```bash
flutter run -v
```

---

# 🔐 Privacy & Offline Support

## Privacy-Focused Design

The application:

- Stores all data locally
- Requires no internet connection
- Uses no external servers
- Does not collect personal health data

---

# 📈 Key Technical Highlights

## Major Features Implemented

- Exact local notification scheduling
- Persistent reminder storage
- Multi-reminder support
- Automatic cleanup system
- Permission management
- Cross-platform Flutter architecture
- Material 3 UI implementation

---

# 🌍 Supported Platforms

| Platform | Status |
|---|---|
| Android | ✅ Supported |
| iOS | ✅ Supported |

---

# 🔮 Future Improvements

Future enhancements may include:

- Cloud synchronization
- Medication history tracking
- Smart dosage analytics
- Caregiver sharing system
- Voice reminders
- Wearable device integration
- AI-based medication insights
- Dark mode support

---

# 📄 License

MIT License

Feel free to use, modify, and distribute this project.


# ⭐ Final Note

The Medication Reminder App demonstrates how Flutter can be used to create reliable, user-friendly healthcare utility applications with persistent background functionality and modern mobile UI design.

The project combines:

- Mobile health utilities
- Local notification systems
- Persistent offline storage
- Clean cross-platform architecture

into a lightweight and practical daily healthcare assistant.

---
