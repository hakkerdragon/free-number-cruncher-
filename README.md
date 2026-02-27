# 🧮 Free Number Cruncher

[![Android Engine](https://img.shields.io/badge/Engine-WebView-green.svg)](https://developer.android.com/reference/android/webkit/WebView)
[![UI Framework](https://img.shields.io/badge/UI-Jetpack%20Compose-orange.svg)](https://developer.android.com/jetpack/compose)
[![Material Design](https://img.shields.io/badge/Design-Material%203-blue.svg)](https://m3.material.io/)
[![Security](https://img.shields.io/badge/Security-Biometric-red.svg)](https://developer.android.com/training/sign-in/biometric-auth)

**Free Number Cruncher** is a sophisticated, Material 3-style calculator for Android that serves as a stealth gateway to a private web browser. On the surface, it is a fully functional calculator; underneath, it contains a biometric-locked browsing experience designed to leave zero trace on your device.

---

## ✨ Features

### 🧮 The "Cruncher" (Calculator)
*   **Modern UI:** Built with **Jetpack Compose** and **Material 3** for a clean, responsive interface.
*   **Dynamic Theming:** Seamless support for Light and Dark modes via the `CalculatorViewModel`.
*   **Tactile Feedback:** Integrated haptic feedback for a premium physical feel.
*   **Secret Trigger:** Use a custom mathematical expression (secret combination) as the "key" to unlock the hidden browser.

### 🕵️ Stealth Browser
*   **Biometric Security:** Access is guarded by the Android Biometric API (Fingerprint/Face Unlock/Device Credential).
*   **Auto-Wipe Technology:** Exiting the browser or double-tapping triggers an immediate wipe of:
    *   Cookies & Cache
    *   Web Storage & Form Data
    *   Browser History
*   **Reader Mode:** A custom JavaScript-injected mode that strips ads and clutter for a distraction-free reading experience.
*   **Efficiency Mode:** Ability to "freeze" the WebView process to conserve battery and data when not in active use.
*   **Multi-Engine Support:** Built-in support for switching between search providers.
*   **Panic Exit:** Double-tap gesture support to instantly close the browser and return to the calculator.

---

## 🛠 Tech Stack

*   **Language:** [Kotlin](https://kotlinlang.org/)
*   **UI Framework:** [Jetpack Compose](https://developer.android.com/jetpack/compose)
*   **Design:** Material Design 3 (M3)
*   **Architecture:** MVVM (Model-View-ViewModel)
*   **Security:** AndroidX Biometric Library
*   **Web Engine:** Android WebView with custom `WebViewClient` and `WebChromeClient` implementations

---

## 🔒 Privacy & Security

Privacy is the core principle of this application:
1.  **Two-Factor Entry:** Requires both a "Secret Combination" entered into the calculator AND a successful Biometric scan.
2.  **No Persistence:** Once the session is closed via the `closeAndClear` function, the app invokes:
    
!!!!!!!!!THE DEFAULT CODE IS 1234= YOU CAN CHANGE THIS LATER IN THE APP!!!!!!!
