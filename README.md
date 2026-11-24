# SmartSplit

SmartSplit is an Android app prototype for choosing two installed apps and requesting adjacent launch, with font previews and a shortcut to the phone's display settings.

## Build the APK with GitHub

1. Create or open the GitHub repository named `Smart-split`.
2. Upload **all contents** of this project folder (not the outer ZIP) to the repository root.
3. Commit the files to the `main` branch.
4. Open the **Actions** tab.
5. Select **Build SmartSplit APK** and choose **Run workflow** (or wait for the push build).
6. Open the completed workflow run, then download the `SmartSplit-debug-apk` artifact.

## Important device limitations

- Android/HiOS controls split-screen support. SmartSplit requests adjacent launches, but the phone may still require you to open Recent apps and choose **Split screen** manually. Some apps do not support split-screen.
- Android apps cannot freely replace the system-wide font. The Fonts tab previews font families inside SmartSplit and opens the phone's display settings for system font options where available.
- The app requests `QUERY_ALL_PACKAGES` so it can list installed launchable apps. This is intended for personal sideloading/testing; app-store distribution has additional policy requirements.

## Requirements

- Android Studio with JDK 17 and Android SDK 35, or GitHub Actions workflow above.
- Minimum Android version: Android 8.0 (API 26).
