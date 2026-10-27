# Clean Calculator for Android

A minimalist, high-precision dark-themed calculator built with Android **Jetpack Compose** and Kotlin. Features standard arithmetic in portrait mode, a scientific keyboard in landscape mode, gesture-based swipe-to-delete, and fluid reactive button animations.

![Clean Calculator Banner](store_assets/feature_graphic_1024x500.jpg)

## ✨ Highlights

* **100% Native Jetpack Compose**: Modern declarative UI with fluid state-driven animations.
* **Standard & Scientific Modes**:
  * **Portrait**: Essential daily arithmetic, percentage calculations, sign flipping, and swipe backspace.
  * **Landscape**: Full scientific suite including trigonometry (`sin`, `cos`, `tan`), hyperbolic functions, logarithms (`ln`, `log10`, `log2`), powers (`xʸ`, `eˣ`, `10ˣ`, `2ˣ`), roots, and mathematical constants (`π`, `e`).
* **Active Operator State Tracking**: Highlights active operations in bright contrast, reverting smoothly upon calculation completion.
* **Haptic Feedback**: Subtle vibration on keypress for satisfying physical-like tactile confirmation.
* **Zero Tracking & Completely Offline**: No internet access required, no third-party telemetry, 100% private.

## 🚀 Building with GitHub Actions (Automated .AAB & .APK)

Every push to `main` automatically triggers the GitHub Actions workflow in `.github/workflows/build-apk.yml`:
1. Navigates to the **Actions** tab in this GitHub repository.
2. Selects the latest run of **Build Android App & Play Store Bundle**.
3. Downloads the build artifacts:
   - **`Clean-Calculator-PlayStore-AAB`**: Upload-ready `.aab` (Android App Bundle) for Google Play Console.
   - **`Clean-Calculator-Release-APK`**: Signed release `.apk` for direct sideloading.
   - **`Clean-Calculator-Debug-APK`**: Fast debug build for local development.
   - **`Release-Keystore-Backup`**: Keystore (`release-key.jks`) used to sign the build.

## 📦 Google Play Store Submission

Refer to [`PLAY_STORE_LISTING.md`](PLAY_STORE_LISTING.md) for ready-to-use copy-paste text for the Google Play Console:
- App Title, Short Description, and Full Description
- Data Safety form declarations
- IARC Content Rating answers
- Privacy Policy URL (`privacy.html` hosted on GitHub Pages)

## 🛠️ Local Build Requirements

* Android Studio Hedgehog (2023.1.1) or newer
* JDK 17
* Android SDK 34 (Android 14)
* Gradle 8.7

```bash
# Build Debug APK
./gradlew :app:assembleDebug

# Build Play Store Release AAB
./gradlew :app:bundleRelease
```

## 📜 Privacy & License

* Privacy Policy: See [`privacy.html`](privacy.html).
* License: Apache 2.0
