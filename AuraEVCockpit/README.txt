BUILD THE APK
1. Install Android Studio (https://developer.android.com/studio).
2. File > Open > select this AuraEVCockpit folder. Let Gradle sync finish.
3. Build > Build Bundle(s) / APK(s) > Build APK(s).
4. APK appears at app/build/outputs/apk/debug/app-debug.apk
   Copy to your phone and install (allow "install unknown apps").

Command line (with Android SDK + Gradle installed):
   gradle assembleDebug

NOTE: The dashboard loads Tailwind from a CDN (gstatic.com). The phone needs
internet on first launch. For fully offline use, download that script, save it
as app/src/main/assets/tailwind.min.js and change the <script src=...> in
app/src/main/assets/index.html to src="tailwind.min.js".
