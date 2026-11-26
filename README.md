# DJALIMEN MANAGER

**DJALIMEN MANAGER** adalah proyek yang dikembangkan dan dipelihara secara independen dengan identitas DJALIMEN, berlandaskan komponen open-source dari para pengembang aslinya.

## Fitur

- Aktivasi Root, Wireless ADB, TCP ADB, serta aktivasi melalui komputer, browser, dan OTG.
- Start-on-boot dan pemantauan status server.
- Pengelolaan hak akses aplikasi dan kompatibilitas Shizuku API.
- Plugin/module manager dengan WebUI.
- QuickShell, Settings Editor, Process Manager, dan pengaturan tampilan.

## Build APK

```bash
git clone --recurse-submodules https://github.com/rizal070901-dot/DJALIMEN-MANAGER.git
cd DJALIMEN-MANAGER/upstream
./gradlew :manager:assembleDebug
```

APK debug berada di `upstream/manager/build/outputs/apk/debug/`.

Build otomatis tersedia melalui tab **Actions** pada workflow **Build DJALIMEN Manager APK**. Unduh artifact `DJALIMEN-MANAGER-debug` dari run yang berhasil.

## Branding dan perubahan

Identitas DJALIMEN digunakan untuk nama aplikasi, tampilan, halaman Tentang/Dukungan, dan materi proyek. Perubahan branding dipisahkan dari implementasi fitur inti. Nama package, applicationId, protokol, izin Android, dan komponen layanan tidak diubah oleh pembaruan dokumentasi ini.

## Asal-usul dan atribusi

DJALIMEN MANAGER merupakan proyek independen yang menggunakan dan memodifikasi komponen perangkat lunak open-source. DJALIMEN bertanggung jawab atas pengembangan, pemeliharaan, serta perubahan yang dibuat khusus untuk distribusi DJALIMEN.

Pemberitahuan hak cipta, atribusi, dan ketentuan lisensi dari seluruh komponen upstream maupun pihak ketiga tetap dipertahankan sesuai lisensi masing-masing. DJALIMEN MANAGER bukan rilis resmi atau produk yang didukung oleh pengembang komponen upstream.

- [LICENSE](LICENSE) — teks lisensi dan pemberitahuan lisensi.
- [NOTICE](NOTICE) — atribusi upstream dan komponen pihak ketiga.

## Lisensi

Kode dan komponen dalam repositori ini dapat memiliki ketentuan lisensi yang berbeda. Komponen yang berlisensi Apache License 2.0 tunduk pada [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0); komponen lain tetap mengikuti lisensi masing-masing. Periksa file lisensi di direktori komponen terkait, termasuk `api/LICENSE` bila menggunakan API tersebut.
