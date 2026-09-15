# TRA CELL — APK chay doc lap

App khong con mo trang web tren GitHub nua. Toan bo trang nam san trong APK,
nen mo len **khong co thanh dia chi trinh duyet**, va khong phu thuoc GitHub Pages.

Van can mang cho 2 viec: tai anh nen ban do (OpenStreetMap) va goi API tra cell.
Danh sach BTS 4 nha mang nam san trong may, khong can mang.

## Upload gi len repo

    settings.gradle
    build.gradle
    gradle.properties
    app/build.gradle
    app/src/main/AndroidManifest.xml
    app/src/main/java/io/github/minhcell/tracell/MainActivity.java
    app/src/main/res/values/strings.xml
    app/src/main/res/values/colors.xml
    app/src/main/res/values/styles.xml
    app/src/main/res/drawable/splash_screen.xml
    app/src/main/res/xml/file_paths.xml
    web/index.html
    .github/workflows/build-android.yml

Tat ca deu la file van ban, khong co file anh, nen upload khong bi hong.

Thu muc `app/src/main/res/mipmap-*` va `app/src/main/assets/` **khong can upload** —
may build tu tao ra luc chay.

Neu repo con thu muc `android/` cu thi xoa di cho khoi lan.

## Secret van giu nguyen 4 cai

`KEYSTORE_BASE64`, `KEYSTORE_PASSWORD`, `KEY_ALIAS`, `KEY_PASSWORD`.

## Build

Actions -> Build APK TRA CELL -> Run workflow. Vao Releases tai `TRA_CELL.apk`.

**Phai go app cu ra truoc khi cai ban nay** — app cu la vo TWA, ban nay la app
thuong, Android khong cho cai de len nhau.

## Sau nay muon sua giao dien

Sua file `web/index.html` trong repo roi push. May tu build lai APK moi.
Cac file thu vien (Leaflet, JSZip, XLSX, Mammoth) va 4 file du lieu BTS
duoc may build tu tai ve luc build, khong phai upload.

Muon du lieu BTS nam han trong repo thi bo 4 file
`mobifone_bts.js`, `vinaphone_bts.js`, `viettel_bts.js`, `vietnamobile_bts.js`
vao thu muc `web/`, may build se uu tien dung ban trong repo.

## Doi voi trang web tren GitHub Pages

Repo `tracellmoi` van chay doc lap nhu cu, khong lien quan. Neu muon trang web
do cung het loi va nut cung mau xam thi upload ban da sua o goi truoc.
