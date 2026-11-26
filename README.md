# DJALIMEN MANAGER

Project Android berbasis Axeron Manager (AxManager), dengan target branding dan pengembangan DJALIMEN.

## Status saat ini

- Fondasi upstream AxManager dipatok sebagai Git submodule pada folder `upstream/` agar kode inti, modul, dan riwayat sumber aslinya tidak disalin secara parsial.
- Submodule API upstream tetap dipertahankan secara rekursif.
- GitHub Actions disiapkan untuk membangun APK debug dan mengunggahnya sebagai artifact.
- Branding aplikasi, identitas paket, aset, serta pengujian kompatibilitas masih menjadi pekerjaan lanjutan. Build awal akan tetap mengikuti konfigurasi upstream sampai perubahan branding diverifikasi.

## Fitur fondasi upstream

Aktivasi Root, Wireless ADB, TCP ADB, aktivasi dari komputer/browser/OTG, start-on-boot, status server, kontrol privilege per aplikasi, kompatibilitas Shizuku API, plugin/module manager dengan WebUI, QuickShell, Settings Editor, pengaturan server, dan pengaturan tampilan.

## Build lokal

```bash
git clone --recurse-submodules https://github.com/rizal070901-dot/DJALIMEN-MANAGER.git
cd DJALIMEN-MANAGER/upstream
./gradlew :manager:assembleDebug
```

APK debug berada di `upstream/manager/build/outputs/apk/debug/`.

## Build otomatis

Buka tab **Actions** lalu jalankan workflow **Build DJALIMEN Manager APK**. APK debug akan tersedia pada bagian Artifacts dari workflow run.

## Lisensi dan atribusi

Kode fondasi berasal dari [AxManager](https://github.com/fahrez182/AxManager) oleh FahrezRB. Hak cipta dan lisensi upstream tetap berlaku. Lihat `upstream/LICENSE` dan `upstream/NOTICE`. API upstream dipertahankan sebagai submodule terpisah sesuai lisensinya.