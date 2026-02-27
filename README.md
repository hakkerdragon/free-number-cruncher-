Free Number Cruncher
Free Number Cruncher is a sophisticated, Material 3-style calculator for Android that serves as a gateway to a secure, private web browser. On the surface, it is a fully functional calculator; underneath, it contains a biometric-locked private browsing experience designed to leave zero trace on your device.
🚀 Features
🧮 The "Cruncher" (Calculator)
•
Modern UI: Built with Jetpack Compose and Material 3 for a clean, responsive interface.
•
Dynamic Theming: Full support for Light and Dark modes.
•
Tactile Experience: Integrated haptic feedback for button presses.
•
Secret Trigger: Use a custom mathematical expression as the "key" to unlock the hidden browser.
🕵️ Stealth Browser
•
Biometric Security: Access is guarded by the Android Biometric API (Fingerprint/Face Unlock/Device Credential).
•
Auto-Wipe Technology: Exiting the browser triggers an immediate wipe of:
◦
Cookies & Cache
◦
Web Storage & Form Data
◦
Browser History
•
Reader Mode: A custom JavaScript-injected mode that strips clutter and ads for a clean reading experience.
•
Efficient Mode: Ability to "freeze" the WebView process to conserve battery and data.
•
Multi-Engine Support: Choose your preferred search engine (Google, DuckDuckGo, etc.).
•
Panic Exit: Double-tap gesture support to instantly close the browser and return to the calculator.
🛠 Tech Stack
•
Language: Kotlin
•
UI Framework: Jetpack Compose
•
Design: Material Design 3
•
Architecture: MVVM (Model-View-ViewModel)
•
Security: AndroidX Biometric Library
•
Web Engine: Android WebView with custom WebViewClient and WebChromeClient implementations
🔒 Security & Privacy
Privacy is the core principle of this application.
1.
Two-Factor Entry: Requires both a "Secret Combination" entered into the calculator AND a successful Biometric scan.
2.
No Persistence: Once the session is closed via closeAndClear, the app invokes WebStorage.deleteAllData() and CookieManager.removeAllCookies() to ensure no data persists on the hardware.
3.
Back-Handler Safety: The system back button is overridden to ensure users don't accidentally exit the browser without triggering the data wipe, or to navigate the browser history safely.
📸 How to Use
1.
Calculate: Use it as your daily calculator for basic math.
2.
Unlock: Enter your unique secret expression (defined in the ViewModel) and press the equals button.
3.
Authenticate: Confirm your identity via the system biometric prompt.
4.
Browse: Search and navigate freely.
5.
Vanish: Double-tap the screen or use the back button to wipe all session data and return to the calculator.
!!!!!!!!!THE DEFAULT CODE IS 1234= YOU CAN CHANGE THIS LATER IN THE APP!!!!!!!
