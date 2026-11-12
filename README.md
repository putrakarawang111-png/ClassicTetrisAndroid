# Classic Tetris - Android project

- App name: Classic Tetris
- Package/application ID: `com.mangdede.tetris`
- Minimum Android: Android 6.0 (API 23)
- Gameplay runs locally in an Android WebView from `app/src/main/assets/index.html`.
- No internet permission or backend is required. High score uses browser local storage.

## Build an installable APK with Android Studio

1. Install Android Studio and the Android SDK Platform 35 (or let Android Studio install it).
2. Open this folder (`ClassicTetrisAndroid`) in Android Studio.
3. Use JDK 17 when prompted and wait for Gradle sync to finish.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. The debug APK will be at `app/build/outputs/apk/debug/app-debug.apk`.
6. Copy that APK to the Android phone and install it. If prompted, allow installing apps from that file manager/browser.

For a release APK, use **Build > Generate Signed Bundle / APK > APK**, create a signing key, then follow the wizard.

This source project is ready to open in Android Studio. The APK itself is not prebuilt in this environment because Android SDK/Gradle build tools are not installed here.

## Build online with GitHub Actions (no Android Studio needed on the phone)

1. Create a GitHub repository and upload the contents of this project.
2. Open the repository's **Actions** tab.
3. Choose **Build Classic Tetris APK** and tap **Run workflow**.
4. When the workflow finishes, open its run page and download the `Classic-Tetris-APK` artifact.
5. Extract the downloaded artifact ZIP; it contains `app-debug.apk`.
6. Transfer the APK to the Android phone and install it.
