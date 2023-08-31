# Strikethrough app

Based on https://simplepwa.com.  An experiment to see how complex it is to go straight to android via a PWA.

To run, simply load up index.html. In chrome you can run lighthouse and should get a PWA valid score.

Next step packaging.



## build for android

1. Ensure the keystore is in the repo root directory: `android.keystore`
1. Gen a new version: `bubblewrap update`
1. Build it: `bubblewrap build`
1. checkin the new versions of `twa-manifest.json` & `app/build.gradle`
1. Do something with the generated APK or the AAB (AAB is a newer form of APK, both may be generated)

## updating icons

1. Update favicon.png
1. `real-favicon generate favicon_config.json favicon_data.json .`
1. delete `favicon_data.json`
1. commit
