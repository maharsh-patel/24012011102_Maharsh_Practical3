# Practical 3: Implementation of Explicit and Implicit Intents in Android

[![Kotlin](https://img.shields.io/badge/Kotlin-1.9-purple.svg?style=flat&logo=kotlin)](https://kotlinlang.org)
[![Android](https://img.shields.io/badge/Platform-Android-green.svg?style=flat&logo=android)](https://developer.android.com)
[![Gradle](https://img.shields.io/badge/Build-Gradle-blue.svg?style=flat&logo=gradle)](https://gradle.org)

## 👤 Student Information

| Key | Details |
| --- | --- |
| **Student Name** | Maharsh Patel |
| **Enrollment No.** | 24012011102 |
| **Batch** | 5H-1 |
| **Branch** | Computer Engineering (CE) |
| **Course** | Mobile Application Development (MAD) |
| **Practical No.** | Practical 3 |

---

## 📌 Practical Overview

This project demonstrates the core Android concept of **Intents** (both **Explicit Intents** and **Implicit Intents**). An Intent is a messaging object used to request an action from another app component (like an activity).

### 🎯 Key Objectives:
1. **Explicit Intent**:
   - Navigate from `MainActivity` to `LoginActivity`.
   - Pass data (`username` and `password`) across activities using `Intent.putExtra()`.
2. **Implicit Intent**:
   - **Browse Web**: Open an external web page (`https://www.google.com`) using `Intent.ACTION_VIEW`.
   - **Phone Dialer**: Open the phone dialer with a given phone number using `Intent.ACTION_DIAL`.
   - **Call Log**: Open system Call Logs using `Intent.ACTION_VIEW` and `CallLog.Calls.CONTENT_TYPE`.
   - **Gallery**: Open system Gallery/Media viewer using `Intent.ACTION_VIEW` and MIME type `image/*`.
   - **Camera**: Launch system Camera app to capture images using `MediaStore.ACTION_IMAGE_CAPTURE`.
   - **Alarm Clock**: Display system Alarm settings using `AlarmClock.ACTION_SHOW_ALARMS`.

---

## 📸 Screenshots

| Main Dashboard (Implicit & Explicit Intents) | Login Activity (Explicit Intent Target) |
| :---: | :---: |
| ![Main Screen](./dee7aa31-80a1-4ef6-a90c-4cd272834e8e.jpg) | ![Login Screen](./134398e1-4862-456f-bb9e-5e364b2b7001.jpg) |

---

## 🛠 Project Structure

```
MAD_24012011102_practical3/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/mad_24012011102_practical3/
│   │       │   ├── MainActivity.kt      # Handles Explicit and Implicit Intents
│   │       │   └── LoginActivity.kt     # Receives Intent extras & displays login UI
│   │       └── res/
│   │           └── layout/
│   │               ├── activity_main.xml  # Layout with intent control buttons
│   │               └── activity_login.xml # Layout for login screen
├── build.gradle.kts
└── README.md
```

---

## ⚙ Code Highlights

### Explicit Intent (Data Passing)
```kotlin
val intent = Intent(this, LoginActivity::class.java)
intent.putExtra("username", "maharsh")
intent.putExtra("password", "123")
startActivity(intent)
```

### Implicit Intents Implementation
```kotlin
// Browse Website
val browseIntent = Intent(Intent.ACTION_VIEW, Uri.parse("https://www.google.com"))
startActivity(browseIntent)

// Phone Dialer
val dialIntent = Intent(Intent.ACTION_DIAL, Uri.parse("tel:$number"))
startActivity(dialIntent)

// Camera
val cameraIntent = Intent(MediaStore.ACTION_IMAGE_CAPTURE)
startActivity(cameraIntent)
```

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/maharsh-patel/MAD_24012011102_Practical_3.git
   ```
2. Open the project in **Android Studio** (Giraffe / Hedgehog or newer).
3. Sync Gradle dependencies.
4. Run on an Emulator or a physical Android Device (API 24+ recommended).

---

## 🔗 Repository Links
- GitHub Repo: [https://github.com/maharsh-patel/MAD_24012011102_Practical_3](https://github.com/maharsh-patel/MAD_24012011102_Practical_3)
