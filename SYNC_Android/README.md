# SYNC Android API Upgrade (Pelamar & Validasi)

Project Android WebView untuk SYNC Recruitment Center.

## Perubahan
- Hub & GAP tetap membaca endpoint utama Google Apps Script.
- Menu Pelamar mencoba action `applicants`, `pelamar`, `pendaftar`, `data_pelamar`.
- Menu Validasi mencoba action `validation`, `validasi`, `data_validasi`, `validations`, lalu mencocokkan nama + hub dengan data pelamar.
- Respons API dikenali jika array berada di `data`, `rows`, `results`, `items`, `applicants`, `pelamar`, `pendaftar`, `validation`, `validasi`, atau `records`.
- Jika action belum tersedia, aplikasi menampilkan status/error yang jelas, bukan data palsu.
- WebView diizinkan mengakses API HTTPS dari asset lokal.

**Catatan:** Action pelamar/validasi masih harus cocok dengan Apps Script API. Endpoint utama yang dikonfirmasi pengguna saat ini menampilkan sheet `needs hub`; action pelamar/validasi belum dapat diverifikasi dari respons tersebut.

Build: GitHub Actions / `gradle assembleDebug`.
