# ReplaySwap - Android APK Project

Aplikasi Android untuk swap file replay game (Mobile Legends .battle files) menggunakan Floating Bubble Overlay langsung dari dalam layar game.

## Cara Jadikan APK (Build APK):

### Metode 1: Lewat GitHub Actions (Paling Mudah, Tanpa PC)
1. Buat repository baru di github.com.
2. Upload seluruh isi folder ini ke repository GitHub Anda.
3. Buka tab **Actions** di repo GitHub Anda.
4. Klik workflow **Build ReplaySwap APK** lalu klik **Run workflow**.
5. Tunggu ~2 menit hingga selesai centang hijau.
6. Klik hasil build, dan download file **ReplaySwap-Debug-APK** (berisi file `app-debug.apk` siap install di HP Android).

### Metode 2: Lewat Android Studio (PC / Laptop)
1. Ekstrak ZIP ini ke folder komputer.
2. Buka aplikasi Android Studio, pilih **File > Open**, dan pilih folder ReplaySwap.
3. Tunggu Gradle Sync selesai.
4. Klik menu **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Selesai! File APK ada di: `app/build/outputs/apk/debug/app-debug.apk`.

### Metode 3: Langsung di HP Android via Termux
```bash
pkg update && pkg install openjdk-17 git
chmod +x gradlew
./gradlew assembleDebug
```
