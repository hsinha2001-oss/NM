# Nearme Android Studio wrapper

This is a minimal Android WebView wrapper around the Nearme HTML prototype.

## Build an APK (free)
1. Install Android Studio: https://developer.android.com/studio
2. Extract the ZIP.
3. In Android Studio choose **Open** and select the `Nearme-Android` folder.
4. Allow Gradle sync and install any requested Android SDK Platform 35 / build tools.
5. For a test APK, select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. Android Studio will show a notification with a link to the APK. Usually it is at `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfer the APK to your phone and install it. You may need to allow installation from that file manager.

## Notes
- Internet permission is included because Tailwind/Lucide and demo images load from CDNs.
- The prototype is not a production backend. Login is local demo state; data is stored on the device; payment is simulated only. No real payment is collected.
- The current location flow may need runtime permission handling added for Android versions that require it. Test on your device.
- The generated project has not been compiled or device-tested in this environment. Gradle/Android SDK installation is required to produce the APK.
