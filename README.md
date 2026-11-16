# Lifting Plan (team)

Lorry crane lifting plan generator (EHS-14-F08A) for the team.

- **Open the app (any phone / PC):** https://rijalkhairuddin.github.io/lifting-plan/
  On a phone, use the browser menu → *Add to Home screen*.
- **Android app:** https://rijalkhairuddin.github.io/lifting-plan/LiftingPlan.apk

## Shared crane & lifting-gear register
`register.json` is the one shared register. Every copy of the app downloads it on start-up.

To update certificates for everyone:
1. In the app, open **Crane & gear register**, update the dates, then press **Export team register (register.json)**.
2. On GitHub, open this repository → **Add file → Upload files**, drop the new `register.json`, and commit.
3. About 3 minutes later the website, the APK and every user's register are updated.

(Or edit `register.json` directly on GitHub with the pencil icon and commit.)

## Updating the app
Replace `app/src/main/assets/index.html`, bump `versionCode` in `app/build.gradle`, commit. The build in the Actions tab rebuilds the APK and redeploys the website.
