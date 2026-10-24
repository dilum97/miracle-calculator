# Miracle Calculator – Android APK

## APK එක හදාගන්න විදිය (GitHub Actions – Android Studio ඕන නැහැ)
1. GitHub එකේ අලුත් **private** repo එකක් හදන්න (උදා: miracle-calculator-app).
2. මේ folder එකේ ඔක්කොම (hidden `.github` folder එකත් එක්ක) push කරන්න:
   git init && git add -A && git commit -m "init" && git branch -M main
   git remote add origin <repo-url> && git push -u origin main
3. Repo → **Actions** tab → "Build APK" run එක ඉවර වෙනකම් ඉන්න (විනාඩි 5–8).
4. Run එක open කරලා පහළ **Artifacts** → `miracle-calculator-apk` download කරන්න (zip එක, ඇතුලේ app-debug.apk).
5. Phone එකට APK එක දාලා install කරන්න ("Install unknown apps" allow කරන්න ඕන වෙයි).

## Icon මාරු කරන්න
`assets/icon-only.png` replace කරන්න (1024 x 1024 PNG, හතරැස්). ඊට පස්සේ push කරන්න, APK එක ආයෙ build වෙනවා.
දැනට තියෙන්නේ calculator එකේ logo එකෙන් හදපු placeholder එකක්.

## Calculator එක update කරන්න
`www/index.html` replace කරලා push කරන්න.

## App name / package
`capacitor.config.json` → appName, appId
