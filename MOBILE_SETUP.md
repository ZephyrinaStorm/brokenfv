# Native Android and iOS builds

This repository includes Capacitor configuration to wrap the same website as native Android/iOS applications. Native platform folders and compiled APK/IPA files are **not** included; generate them on a machine with Android Studio / Xcode.

1. Install Node.js 20+ and run `npm install`.
2. Run `npm run build`.
3. Android: `npx cap add android`, `npm run mobile:sync`, `npm run android:open`. In Android Studio, build APK or AAB and test playback.
4. iOS (macOS only): `npx cap add ios`, `npm run mobile:sync`, `npm run ios:open`. In Xcode, configure signing and build/test on device.
5. After web changes run `npm run mobile:sync` again.

## Important constraints
- Third-party HTTP-only radio URLs can be blocked by HTTPS web pages or mobile app security. Prefer HTTPS streams; obtain permission and station-specific metadata endpoints where available.
- Native background audio and lock-screen playback require platform-specific testing and possibly additional native plugins/configuration. Browser Media Session support is included but does not guarantee background playback on all devices.
- Listening history currently records station tune-ins, not verified individual song titles. ICY metadata needs station APIs or a compliant server-side adapter; the app never fabricates track names or cover art.
- Stream diagnostics are device-local and not continuous server-side uptime checks.
- Respect station licensing and terms; do not rebroadcast or cache copyrighted music without permission.
