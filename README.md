# Ping Pong — Android APK

Professional mobile Ping Pong game packaged as a lightweight Android WebView app.

## Login
- Admin: `Neelam`
- Password: `Neelam143`

## Important build fix
This project intentionally uses **no Kotlin or AndroidX dependencies**. The previous build failed because different Kotlin stdlib versions were being resolved together, producing duplicate-class errors such as `kotlin.text.jdk8.*` and `kotlin.time.*`.

The app only uses Android platform APIs, so there is no need for Kotlin stdlib, AppCompat, or AndroidX WebKit.

## GitHub Actions
Push the complete folder to GitHub, then open **Actions → Build Android APK**. The workflow builds `app-debug.apk` and uploads it as the `Ping-Pong-APK` artifact.
