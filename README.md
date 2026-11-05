# Contoh Kotlin Android + GitHub Actions

Aplikasi contoh penghitung angka (counter) menggunakan Kotlin dan Jetpack Compose.
APK dibuat di cloud menggunakan GitHub Actions, sehingga tidak perlu build di HP.

## Cara menggunakan dari HP Android

1. Unduh dan ekstrak ZIP proyek ini.
2. Buat repository baru di GitHub, misalnya `ContohKotlin`.
3. Unggah seluruh isi folder proyek ke repository (bukan folder ZIP-nya).
4. Pastikan file `.github/workflows/build-apk.yml` ikut terunggah.
5. Buka repository GitHub → tab **Actions**.
6. Pilih workflow **Build Android APK**.
7. Jika workflow belum berjalan otomatis, tekan **Run workflow**.
8. Tunggu sampai proses selesai dengan status hijau.
9. Buka hasil run workflow, cari bagian **Artifacts**, lalu unduh `Contoh-Kotlin-debug`.
10. Ekstrak file ZIP artifact dan instal `app-debug.apk` di HP.

## Menjalankan build manual

Workflow juga otomatis berjalan setiap kali ada push ke branch `main`.

## Catatan

- Ini adalah APK debug untuk pengujian, bukan APK release siap Play Store.
- Jika GitHub meminta izin Actions, aktifkan Actions untuk repository tersebut.
- Jangan mengunggah folder `.gradle` atau `build` lokal.
- Proyek menggunakan Android Gradle Plugin 8.7.3, Gradle 8.9, Kotlin 2.0.21, dan JDK 17.
