MONEYMAP v3.3 - Android project
================================

APP KA VERSION KAISE PATA CHALE
-------------------------------
Naya app kholne par upar "MoneyMap" ke saamne ek chhota "v3.3" badge dikhta hai.
More tab ke neeche bhi "MoneyMap v3.3" likha hota hai.
Agar ye badge nahi dikh raha, to aap PURANA app chala rahe hain.

NAYA APP BANANE KE STEPS (sabse saaf tareeka: NAYI repository)
--------------------------------------------------------------
Purani repository mein purani files ya extra folders reh jaate hain, aur
build galti se purani copy utha sakta hai. Isliye nayi repository sabse safe hai.

1. Is zip ko unzip karein. "mera-hisaab-app" folder kholein.
2. github.com par "+" > "New repository". Naam: moneymap. PRIVATE chunein. Create dabayein.
3. Repository mein "uploading an existing file" par click karein.
4. Folder ke ANDAR ki SABHI cheezein drag karein: www, assets, package.json,
   capacitor.config.json, debug.keystore, .gitignore, README.txt.
   (Bahar wala "mera-hisaab-app" folder khud mat daalein.)
   Commit changes dabayein.
5. ".github" folder aksar upload nahi hota. Isliye: Add file > Create new file.
   Naam mein type karein:  .github/workflows/build.yml
   Zip ki .github/workflows/build.yml ka poora text paste karein. Commit changes.
6. Actions tab > "Build Android APK". Run ke andar pehle step
   "Find app folder and check version" kholein. Wahan likha dikhega:
       USING APP FOLDER: .
       APP VERSION IN www/index.html: class="ver">v3.3
   Agar yahan "NONE" ya error aaye, to www/index.html purani hai.
7. Hara tick aane par neeche Artifacts > moneymap-apk-v3-3 download karein.
   Isme app-debug.apk hogi.

PHONE PAR INSTALL (is baar purani app hatani padegi)
----------------------------------------------------
Nayi repository ki signing key purani app se alag hai, isliye pehle:
1. Purani app kholein > Backup tab > text copy karke WhatsApp/Notes mein save karein.
2. Purani app uninstall karein.
3. Nayi app-debug.apk install karein.
4. More > Backup > "Restore data from a backup" mein text paste karke "Restore data" dabayein.
Iske baad se har naya build isi key se banega aur purani app ke UPAR install hoga.

AUTO BACKUP: App > More > Backup > "First-time setup steps".
