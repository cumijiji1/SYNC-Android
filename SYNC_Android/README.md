# SYNC Android App Starter

Starter project Android Studio untuk aplikasi SYNC Recruitment Center.

## Build APK
1. Install Android Studio (versi terbaru yang mendukung Android Gradle Plugin 8.7.x).
2. Buka folder `SYNC_Android` melalui Android Studio.
3. Tunggu Gradle Sync.
4. Untuk menghubungkan dashboard online, edit `app/src/main/java/com/sync/recruitment/MainActivity.java` dan ubah `DASHBOARD_URL` menjadi URL HTTPS dashboard Anda.
5. Atau letakkan file dashboard lokal dan aset terkait di `app/src/main/assets/`, ganti `index.html` dengan dashboard utama.
6. Pilih **Build > Build APK(s)**.
7. APK hasil build biasanya ada di `app/build/outputs/apk/debug/app-debug.apk`.

## Catatan
- Project ini adalah starter Android wrapper; APK belum dibuild di lingkungan ini.
- WebView mendukung JavaScript, penyimpanan web, navigasi kembali, dan upload file dasar.
- Untuk dashboard yang menggunakan login, pastikan cookie/session dan endpoint backend mengizinkan akses dari WebView.
- Gunakan HTTPS untuk dashboard online.
