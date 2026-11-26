TIN-TIN: build the Android APK
================================
You need: Node.js (nodejs.org) and Android Studio (developer.android.com/studio).

1. Open a terminal in this folder and run:
     npm install
     npx cap add android
     npx cap sync android
2. Build the APK, either way:
   A) Android Studio:  npx cap open android
      then Build > Build App Bundle(s) / APK(s) > Build APK(s)
   B) Command line:    cd android && ./gradlew assembleDebug   (Windows: gradlew.bat assembleDebug)
3. Your APK is at: android/app/build/outputs/apk/debug/app-debug.apk
4. Copy it to your phone, open it, and allow "Install unknown apps" when asked.

NO-INSTALL OPTION (works like an app):
Upload the www folder to any web host (e.g. Netlify Drop), open the link in Chrome on your phone,
then menu > Add to Home screen. It runs full screen and offline.
