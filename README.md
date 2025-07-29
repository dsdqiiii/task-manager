 Alat dan Bahan
- Flutter SDK terbaru
- Android Studio / VS Code
- Firebase Project (Authentication & Firestore)
- Emulator Android atau perangkat fisik Android
3.2 Langkah Pengerjaan
Langkah 1: Inisialisasi Proyek Flutter
- Membuat project baru dengan perintah:
flutter create task_manager

Langkah 2: Konfigurasi Firebase
- Buat project di Firebase Console.
- Tambahkan aplikasi Android dan unduh google-services.json ke folder android/app.
- Aktifkan Authentication (Email/Password) dan buat koleksi di Firestore.

Langkah 3: Tambahkan Dependency Firebase
Tambahkan pada pubspec.yaml:
firebase_core, firebase_auth, cloud_firestore

Langkah 4: Setup Gradle
- Ubah semua file .kts menjadi .gradle (Groovy DSL).
- Tambahkan classpath Firebase di build.gradle dan plugin di app/build.gradle.

Langkah 5: Implementasi Fitur
- Login Screen: form email & password, tombol login.
- Task List Screen: daftar tugas dari Firestore, fitur tambah & hapus.
