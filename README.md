# Khet Majdur Hisab (Android, Kotlin + Jetpack Compose)

A simple offline app for farm labor records:
- Add majdur entries per pickup (weight + rate) — automatic total.
- Date-wise view, total amount for the day.
- Export a date-wise PDF (saves to Downloads).

## Build (Android Studio)
1. Open this folder in **Android Studio (Giraffe+ recommended)**.
2. Let Gradle sync.
3. Run on device (debug) **or** Build > Generate Signed Bundle/APK… (release).

## Build (CLI)
```bash
./gradlew :app:assembleDebug
# APK will be at app/build/outputs/apk/debug/app-debug.apk
```

## Notes
- Uses Room for local storage.
- Uses MediaStore to save PDF in Downloads (no legacy storage permissions required on Android 10+).
