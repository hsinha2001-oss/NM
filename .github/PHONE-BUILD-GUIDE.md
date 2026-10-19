# Build Nearme APK using only your Android phone (free)

This project includes a GitHub Actions workflow that builds a debug APK in the cloud.

## Steps
1. Download and extract `Nearme-Android-Cloud-Build.zip` on your phone, or upload the ZIP contents directly to a new GitHub repository.
2. Open https://github.com in Chrome and sign in/create a free account.
3. Create a new repository named `Nearme` (public is simplest for free Actions) and create it.
4. Upload the project files and folders from this ZIP into the repository root. Ensure `.github/workflows/build-apk.yml` is included; on Android, hidden folders can be easy to miss.
5. Open the repository's **Actions** tab and select **Build Nearme APK**. Tap **Run workflow** if it has not started automatically.
6. Wait for the workflow run to finish with a green check.
7. Open the completed run, scroll to **Artifacts**, and tap **Nearme-debug-apk** to download the ZIP artifact.
8. Extract that downloaded ZIP. It contains `app-debug.apk`. Tap the APK to install. Android may ask you to allow installation from Chrome/Files; only enable it for the app you used to download the APK, then turn it off again if desired.

## Notes
- This creates a debug/test APK, not a Play Store release-signed APK.
- GitHub Actions may require confirming your email/account or enabling Actions.
- The app is a WebView wrapper around the Nearme prototype and uses internet-hosted assets. Some demo actions and payment are simulations, not a production backend or real payment processing.
