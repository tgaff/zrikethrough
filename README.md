# Strikethrough app

Based on https://simplepwa.com.  An experiment to see how complex it is to go straight to android via a PWA.

To run, simply load up index.html. In chrome you can run lighthouse and should get a PWA valid score.

Next step packaging.



## build for android

1. Ensure the keystore is in the repo root directory: `android.keystore`
1. Gen a new version: `bubblewrap update`
1. Build it: `bubblewrap build`
1. checkin the new version of `twa-manifest.json`
1. Do something with the generated APK