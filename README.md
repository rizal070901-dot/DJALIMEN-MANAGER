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

# DJALIMEN MANAGER

**Copyright © 2026 DJALIMEN.**

DJALIMEN MANAGER is an independently maintained and modified software project.

This project incorporates and modifies open-source components originally developed by their respective authors, including AxManager by FahrezRB.

All upstream copyright notices, attribution requirements, and applicable open-source licenses are retained in accordance with their respective license terms.

DJALIMEN is responsible for its own modifications, development, maintenance, and branding.

**License:** Apache License 2.0 (including applicable upstream components).

See [LICENSE](https://github.com/rizal070901-dot/DJALIMEN-MANAGER/blob/main/LICENSE) and [NOTICE](https://github.com/rizal070901-dot/DJALIMEN-MANAGER/blob/main/NOTICE).
DJALIMEN MANAGER merupakan distribusi komunitas dan bukan proyek resmi dari pengembang upstream.
