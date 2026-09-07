# Minimal Calendar — Android APK

A GitHub-ready Capacitor Android project based on the supplied Minimal Calendar HTML.

## Features
- Mobile-friendly calendar UI
- Current date is initialized automatically
- Previous/next month navigation
- Date selection
- Notes saved locally with `localStorage`
- Android APK build through GitHub Actions
- No backend required

## Build APK on GitHub

1. Create a new GitHub repository.
2. Upload all files from this folder to the repository.
3. Commit to the `main` branch.
4. Open **Actions**.
5. Select **Build Android APK**.
6. Click **Run workflow** if needed.
7. After the workflow finishes, open the workflow run and download the artifact:
   `minimal-calendar-debug-apk`

The downloaded artifact contains `app-debug.apk`.

## Local build

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```

APK output:

`android/app/build/outputs/apk/debug/app-debug.apk`

## App ID

`com.bhimmondal.minimalcalendar`

Change the app name or App ID in `capacitor.config.json` before publishing a separate app.
