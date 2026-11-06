# FPS Boost Kit for Android

An offline-friendly Android WebView app wrapping the upgraded FPS Boost Kit.

## Build an APK in the cloud (recommended)
1. Create a free GitHub account if you do not already have one.
2. Create a **new public repository** on GitHub (public repositories are the simplest way to use GitHub-hosted Actions without consuming private-repository minutes).
3. Upload the contents of this project ZIP to the repository root. Make sure `.github/workflows/android-apk.yml` is included.
4. Open the repository's **Actions** tab.
5. Select **Build FPS Boost Kit APK** and tap **Run workflow** (or push to `main` to trigger it).
6. Wait for the green check mark, open the completed workflow run, and download the artifact named **FPS-Boost-Kit-debug-apk**.
7. Extract the downloaded artifact. Install `app-debug.apk` on your Android phone. Android may ask you to allow installation from that source.

## Build locally
Open this folder in Android Studio and choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**, or run `gradle assembleDebug` after installing the Android SDK and Gradle.

## App details
- Android 6.0+ (API 23+) target.
- Local HTML asset; no internet permission, account, analytics, or paid API.
- The smoothness test measures WebView animation callback cadence. It does not unlock FPS or measure a game's true FPS.
- Checklist progress is stored locally in WebView storage.
