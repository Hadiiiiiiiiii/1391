# Graph Studio — Android APK project

This project packages the supplied Graph Studio HTML calculator as an Android app using a local WebView. The HTML is stored at `app/src/main/assets/index.html`; it is loaded from the device and does not need a web server.

## Build the APK with GitHub Actions

1. Create a GitHub repository (for example, `Graph-Studio`).
2. Upload the **contents** of this folder to the repository's `main` branch. Keep the `.github/workflows/build-apk.yml` file in place.
3. Open the repository's **Actions** tab and select **Build Graph Studio APK**.
4. Wait for the run to finish successfully.
5. Open the completed run, scroll to **Artifacts**, and download **Graph-Studio-APK**.
6. Extract the downloaded ZIP. The installable debug APK is `app-debug.apk`.

A push to `main` also starts the build automatically.

## App details

- App name: Graph Studio
- Application ID: `com.example.calculatorgraphstudio`
- Minimum Android version: Android 6.0 (API 23)
- Build: Debug APK (suitable for testing / direct installation)
- Launcher artwork: supplied graph icon

For Google Play distribution, create a signed release build with a private upload key. Do not publish the debug APK.
