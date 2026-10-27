# Google Play Store Listing & Setup Kit for Clean Calculator

Use this guide to copy-paste all required fields directly into your **Google Play Console** (https://play.google.com/console).

---

## 1. App Details & Store Listing

* **App Name (Title - Max 30 chars):**
  ```text
  Clean Calculator: Dark Math
  ```
  *(Alternative: `Clean Dark Calculator`)*

* **Short Description (Max 80 chars):**
  ```text
  Minimalist, dark-themed standard & scientific calculator with smooth gestures.
  ```

* **Full Description (Max 4000 chars):**
  ```text
  Clean Calculator delivers an elegant, distraction-free calculation experience built with modern Android Jetpack Compose. Enjoy a sleek obsidian dark theme, fluid color transitions, and an instant scientific keyboard in landscape mode.

  FEATURES:
  • Standard Mode: Fast everyday math, clean percentage logic, sign flipping (+/-), and swipe-to-delete.
  • Scientific Mode: Simply rotate your phone to landscape to unlock trigonometry (sin, cos, tan, sinh, cosh, tanh), logarithms (ln, log10, log2), powers (xʸ, eˣ, 10ˣ, 2ˣ), roots, factorials, and constants (π, e).
  • Degree / Radian Toggle: Seamlessly switch between degrees and radians for precise engineering and trigonometry.
  • Smooth Reactive Animations: Responsive haptic feedback and dynamic operator button highlighting that accurately tracks current calculations.
  • Swipe to Backspace: Made a typo? Simply swipe left or right across the display digits to erase numbers one by one.
  • 100% Offline & Private: No ads, no background trackers, no internet connection required. Your calculations stay strictly on your device.

  Designed with attention to every pixel and sound for mathematicians, students, engineers, and everyday users who appreciate clean design.
  ```

---

## 2. Policy & App Content Questionnaire Answers

### A. Privacy Policy
* **Privacy Policy URL:**
  Paste the link to your hosted `privacy.html`:
  ```text
  https://erfansvsh.github.io/ios-calculator-android/privacy.html
  ```
  *(Or your custom domain/applet URL: `/privacy.html`)*

### B. Data Safety Questionnaire
* **Does your app collect or share any of the required user data types?**
  Select: **No**
* **Does your app share data with third parties?**
  Select: **No**
* **Is all of the user data collected by your app encrypted in transit?**
  Select: **Not applicable (no data collected)**
* **Do you provide a way for users to request that their data be deleted?**
  Select: **Not applicable (no data collected)**

### C. Advertising ID
* **Does your app use advertising ID?**
  Select: **No**

### D. App Access
* **All functionality is available without special access?**
  Select: **Yes, all functionality is available without special access**

### E. Content Rating (IARC)
* **Category:** Utility, Productivity, Communication, or Other
* **Violence, sexual content, profanity, drugs:** Select **No** to all questions.
* **Result:** Rating: **Everyone (3+) / PEGI 3**.

### F. Target Audience
* **Target age:** 13 and older (or All ages).
* **Could this app appeal to children?** Select **No** (unless you want "Designed for Families", which requires extra verification).

---

## 3. GitHub Actions Artifacts
When you push code to your repository `erfansvsh/ios-calculator-android`:
1. Go to the **Actions** tab on GitHub.
2. Click on the latest workflow run: **Build Android App & Play Store Bundle**.
3. Under **Artifacts**, download:
   * **`Clean-Calculator-PlayStore-AAB`**: This `.aab` file is what you drag-and-drop into Google Play Console's **Production** or **Closed Testing** release track!
   * **`Clean-Calculator-Release-APK`**: Standalone APK if you want to test install directly on your phone.
   * **`Release-Keystore-Backup`**: Keep this `release-key.jks` saved securely on your computer or cloud storage! You will need the same key to sign future app updates.
