# DJALIMEN MANAGER

**DJALIMEN MANAGER** adalah distribusi komunitas dengan identitas visual DJALIMEN yang dibangun di atas fondasi open-source AxManager.

## Fitur fondasi

- Aktivasi Root, Wireless ADB, TCP ADB, aktivasi melalui komputer/browser/OTG.
- Start-on-boot dan pemantauan status server.
- Pengelolaan hak akses per aplikasi dan kompatibilitas Shizuku API.
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

Identitas DJALIMEN diterapkan pada nama aplikasi, teks UI, halaman Tentang/Dukungan, tautan proyek, dan aksen warna. Perubahan branding tidak mengubah applicationId, protokol, izin Android, maupun implementasi fitur inti.

## Lisensi dan atribusi

Fondasi kode berasal dari [AxManager](https://github.com/fahrez182/AxManager) oleh FahrezRB. Proyek ini mempertahankan Apache License 2.0, pemberitahuan hak cipta, dan NOTICE upstream. Komponen pihak ketiga tetap mengikuti lisensinya masing-masing. Lihat [LICENSE](LICENSE) dan [NOTICE](NOTICE).

DJALIMEN MANAGER merupakan distribusi komunitas dan bukan proyek resmi dari pengembang upstream.
