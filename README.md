# Spur Gear Calculator Mobile App

This package contains the mobile-ready app version of the HTML spur gear calculator.

## What is included

- `www/index.html` — mobile app UI and calculator logic
- local PDF engine: `www/vendor/jspdf.umd.min.js`
- PWA manifest and service worker for installable/offline use
- Capacitor configuration for Android/iOS packaging
- embedded PDF preview section before download

## Run as a local web app

```bash
npm install
npm run serve
```

Then open the shown local URL on your phone or desktop browser.

## Build as Android app

```bash
npm install
npx cap add android
npx cap sync android
npx cap open android
```

Android Studio will open the project. From Android Studio, build the APK/AAB.

## Build as iOS app

```bash
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```

Requires macOS and Xcode.

## PDF behavior

Tap **Generate PDF Preview**. The generated report appears inside the app first, then you can open full screen or download it.
