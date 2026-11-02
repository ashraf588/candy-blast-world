CANDY BLAST WORLD — ANDROID WRAPPER PROJECT

Yeh V15 game ko Capacitor ke zariye Android app project mein package karta hai.
Package ID: com.candyblastworld.game

MOBILE/CLOUD BUILD KA TAREEQA:
1) ZIP ko extract karein.
2) GitHub par naya PRIVATE repository banayein aur is folder ki tamam files upload karein.
3) Repository ke Actions tab mein “Candy Blast World Android Build” workflow run karein.
4) Workflow complete hone par Artifacts se app-debug.apk download karke Android phone par install/test karein.

PLAY STORE AAB:
Release AAB ke liye apni upload keystore banani aur GitHub repository Settings > Secrets and variables > Actions mein yeh secrets add karne hain:
ANDROID_KEYSTORE_BASE64, ANDROID_KEYSTORE_PASSWORD, ANDROID_KEY_ALIAS, ANDROID_KEY_PASSWORD
Keystore ko safe backup karein; ise kisi ke saath share na karein. Secrets set hone par workflow signed app-release.aab bhi banata hai.

IMPORTANT:
- Is package mein abhi AdMob SDK/Ad Unit IDs integrate nahi hain.
- APK/AAB build is waqt run nahi hua; GitHub Actions mein cloud build karna hoga.
- App ko Play Store par submit karne se pehle real Android devices par gameplay, screen sizes, offline behaviour aur privacy policy test karein.
- Google Play Console ki current target API, testing aur account verification requirements publish karte waqt check karein.
