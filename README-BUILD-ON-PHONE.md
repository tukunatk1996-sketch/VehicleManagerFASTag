# Vehicle Manager FASTag — Build APK online from Android phone

This project contains a GitHub Actions workflow that builds the Android APK online.

## Steps
1. Download and unzip this project on your Android phone.
2. In a browser, sign in/create a GitHub account and create a **public** repository named `VehicleManagerFASTag` (public is needed for free Actions on a free account in many cases; GitHub's current limits may vary).
3. Open the new repository and use **Add file → Upload files**. Upload the extracted project files/folders, including the `.github/workflows/build-apk.yml` workflow. Do not upload the ZIP itself.
4. Commit/upload the files to the `main` branch.
5. Open the repository's **Actions** tab. Select **Build Android APK**, then press **Run workflow** if it has not started automatically. If it is not listed, check that `.github/workflows/build-apk.yml` was uploaded correctly.
6. Wait for the run to finish successfully (green check). Open that run and download the artifact named **VehicleManagerFASTag-APK**.
7. Extract the downloaded artifact ZIP. Install `app-debug.apk` on your phone. If Android asks, allow installing apps from that browser/files app.

The debug APK is unsigned for Play Store release but can be installed for testing. Hotlist removal is only a local request record; real FASTag hotlisting/unhotlisting needs authorized issuer integration.
