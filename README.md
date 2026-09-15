# MAD Practical 3 - Implicit & Explicit Intents in Android

A modern Android application developed using **Kotlin** demonstrating the concepts and usage of **Implicit Intents** (system app actions like Web Browsing, Dialing, Call Logs, Gallery, Camera, Alarms) and **Explicit Intents** (Activity Navigation to Login Screen with Data Passing).

---

## 📌 Student Details
* **Student Name:** Maharsh Patel
* **Enrollment No:** `24012011102`
* **Batch:** 5H-1
* **Branch:** Computer Engineering (CE)
* **Course:** Mobile Application Development (MAD)
* **Practical:** Practical Assignment 3

---

## 🚀 Features & Actions

### 1. Implicit Intents (`MainActivity`)
- 🌐 **Web Browser:** Opens any web URL in the device's default browser (`Intent.ACTION_VIEW`).
- 📞 **Phone Dialer:** Dials a target phone number using the phone dialer (`Intent.ACTION_DIAL`).
- 📋 **Call Log Viewer:** Opens system call logs (`CallLog.Calls.CONTENT_TYPE`).
- 🖼️ **Gallery:** Opens the device image gallery (`image/*`).
- 📷 **Camera:** Triggers default camera application for photo capture (`MediaStore.ACTION_IMAGE_CAPTURE`).
- ⏰ **Set Alarm:** Opens system alarm settings (`AlarmClock.ACTION_SHOW_ALARMS`).

### 2. Explicit Intents (`LoginActivity`)
- 🔑 **Activity Navigation:** Navigates directly from `MainActivity` to `LoginActivity` using explicit target class intent (`Intent(this, LoginActivity::class.java)`).
- 📦 **Data Passing:** Passes extras (`username` and `password`) to `LoginActivity` via `Intent.putExtra()`.
- 🎨 **Custom Login UI:** Displays GUNI Login interface and Toast notification receiving passed intent extras.

---

## 🛠️ Tech Stack & Requirements

* **Language:** Kotlin
* **Minimum SDK:** API 24 (Android 7.0 Nougat)
* **Compile / Target SDK:** API 35/36
* **UI Components:** `ConstraintLayout`, `AppCompatActivity`, `Button`, `EditText`

---

## 📱 Application Screenshots

<table align="center">
  <tr>
    <td align="center" valign="top" width="33%">
      <h3>1. Main Home Screen</h3>
      <p>Primary landing activity displaying options for implicit & explicit intents.</p>
      <img src="Screenshot/Screenshot_20260915_222218.png" alt="Home Screen" width="240"/>
    </td>
    <td align="center" valign="top" width="33%">
      <h3>2. Phone Dialer Action</h3>
      <p>Opens dialer with pre-filled phone number ready to dial.</p>
      <img src="Screenshot/Screenshot_20260915_222344.png" alt="Phone Dialer" width="240"/>
    </td>
    <td align="center" valign="top" width="33%">
      <h3>3. Active Phone Call</h3>
      <p>Initiates call screen via implicit phone intent.</p>
      <img src="Screenshot/Screenshot_20260915_222419.png" alt="Active Call" width="240"/>
    </td>
  </tr>
  <tr>
    <td align="center" valign="top" width="33%">
      <h3>4. Photos / Gallery</h3>
      <p>Launches Gallery / Photos app to view media files.</p>
      <img src="Screenshot/Screenshot_20260915_222516.png" alt="Gallery Action" width="240"/>
    </td>
    <td align="center" valign="top" width="33%">
      <h3>5. Camera Action</h3>
      <p>Opens camera application to capture a new photo.</p>
      <img src="Screenshot/Screenshot_20260915_222557.png" alt="Camera Action" width="240"/>
    </td>
    <td align="center" valign="top" width="33%">
      <h3>6. Alarm Clock</h3>
      <p>Opens system alarm clock screen.</p>
      <img src="Screenshot/Screenshot_20260915_222616.png" alt="Alarm Action" width="240"/>
    </td>
  </tr>
  <tr>
    <td align="center" valign="top" colspan="3">
      <h3>7. GUNI Login Activity (Explicit Intent)</h3>
      <p>Explicitly opens <code>LoginActivity</code> displaying Login UI with passed extras.</p>
      <img src="Screenshot/Screenshot_20260915_222640.png" alt="Login Activity" width="240"/>
    </td>
  </tr>
</table>

---

## 📥 How to Clone & Run

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/maharsh-patel/MAD_24012011102_Practical_3.git
   ```

2. **Open in Android Studio:**
   * Launch **Android Studio**.
   * Select **File > Open** and select the project folder (`MAD_24012011102_practical3`).

3. **Build & Run:**
   * Let Gradle sync dependencies automatically.
   * Select an Emulator or connected Physical Device (Android API 24+).
   * Click **Run (Shift + F10)**.

---

**Submitted by Maharsh Patel**  
**Enrollment No: 24012011102**  
**Branch: Computer Engineering (CE)**
