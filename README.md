# 🌐 Portal Kampus — Fabric WebView

\<p align="center">   \<strong>Aplikasi mobile untuk mengakses website Universitas Langlangbuana (UNLA) langsung dari dalam aplikasi.\</strong> \</p>

\<p align="center">   \<img src="[https://img.shields.io/badge/React_Native-0.88.0-61DAFB?style=for-the-badge&logo=react&logoColor=white](https://img.shields.io/badge/React_Native-0.88.0-61DAFB?style=for-the-badge\&logo=react\&logoColor=white)" alt="React Native">   \<img src="[https://img.shields.io/badge/WebView-14.0.1-4285F4?style=for-the-badge](https://img.shields.io/badge/WebView-14.0.1-4285F4?style=for-the-badge)" alt="WebView">   \<img src="[https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge\&logo=android\&logoColor=white)" alt="Android">   \<img src="[https://img.shields.io/badge/Project-UTS-orange?style=for-the-badge](https://img.shields.io/badge/Project-UTS-orange?style=for-the-badge)" alt="UTS"> \</p>

---

## 📌 Tentang Proyek

**Portal Kampus — Fabric WebView** merupakan prototipe aplikasi mobile yang dikembangkan untuk menampilkan website Universitas Langlangbuana (UNLA) melalui komponen WebView.

Repository ini menggabungkan dua tugas praktikum Pemrograman Mobile, yaitu Tugas Sesi #2 dan Tugas Sesi #3, yang dikembangkan menggunakan dua platform berbeda melalui pendekatan **Prototyping**.

| Siklus | Platform         | Implementasi                                           |
| :----: | ---------------- | ------------------------------------------------------ |
|   01   | MIT App Inventor | Prototipe awal menggunakan komponen WebViewer          |
|   02   | React Native     | Pengembangan aplikasi menggunakan react-native-webview |

Kedua siklus memiliki tujuan yang sama, yaitu mengakses website UNLA melalui aplikasi mobile. Siklus kedua merupakan implementasi menggunakan platform berbeda, bukan klaim perbaikan berdasarkan evaluasi siklus pertama.

## ✨ Fitur Utama

- 🌐 **Website Integration** — Menampilkan website Universitas Langlangbuana di dalam aplikasi.
- 📱 **Mobile Application** — Mengakses website melalui aplikasi Android.
- ⚡ **JavaScript Support** — Mengaktifkan JavaScript pada WebView.
- 🔄 **Loading State** — Menampilkan status ketika halaman sedang dimuat.
- 🛡️ **Safe Area** — Menggunakan SafeAreaView untuk membantu mengatur area tampilan aplikasi.
- 🔁 **Refresh Website** — Tersedia pada prototipe awal MIT App Inventor melalui tombol REFRESH.

## 🎯 Tujuan Pengembangan

1. Memahami konsep dan penggunaan komponen WebView pada aplikasi mobile.
2. Membuat aplikasi sederhana untuk mengakses website Universitas Langlangbuana.
3. Mengenal pengembangan aplikasi mobile menggunakan MIT App Inventor dan React Native.
4. Menggabungkan hasil Tugas Sesi #2 dan Tugas Sesi #3 dalam satu repository GitHub.

---

## 🔄 Metode Pengembangan — Prototyping

Pengembangan proyek dilakukan melalui dua siklus dengan pendekatan platform yang berbeda.

### 01 — Prototype Awal: MIT App Inventor

Prototipe pertama dibuat menggunakan MIT App Inventor dengan konfigurasi berikut:

| Komponen         | Keterangan                                           |
| ---------------- | ---------------------------------------------------- |
| Nama proyek      | `TEST`                                               |
| Screen           | `Screen1`                                            |
| Judul aplikasi   | `UNLA APK`                                           |
| Komponen WebView | `WebViewer1`                                         |
| Website          | [Universitas Langlangbuana](https://www.unla.ac.id/) |
| Tombol           | `REFRESH`                                            |
| Aksi tombol      | Menjalankan fungsi `Reload` pada `WebViewer1`        |

Prototipe ini merupakan implementasi awal penggunaan WebView untuk menampilkan website kampus.

### 02 — Implementasi: React Native

Pengembangan berikutnya dilakukan menggunakan React Native dengan library `react-native-webview`.

Implementasi utama terdapat pada file [`App.tsx`](./App.tsx), dengan karakteristik:

- Menampilkan header **Portal Kampus - Fabric WebView**.
- Memuat website UNLA secara langsung melalui WebView.
- Mengaktifkan JavaScript.
- Menggunakan `startInLoadingState` untuk status pemuatan halaman.
- Menggunakan `SafeAreaView` untuk pengaturan area tampilan.
- Mengatur warna status bar aplikasi.

### 📊 Perbandingan Kedua Siklus

| Aspek      | Siklus 1           | Siklus 2                                   |
| ---------- | ------------------ | ------------------------------------------ |
| Platform   | MIT App Inventor   | React Native                               |
| Komponen   | WebViewer          | react-native-webview                       |
| Website    | UNLA               | UNLA                                       |
| Refresh    | Tombol REFRESH     | Implementasi mengikuti konfigurasi WebView |
| Pendekatan | Visual programming | JavaScript / TypeScript                    |

**Catatan:** Dokumentasi hasil pengujian dan evaluasi pengguna pada siklus pertama tidak tersedia. Oleh karena itu, perbandingan ini berfokus pada platform dan implementasi, bukan pada klaim peningkatan berdasarkan umpan balik.

---

## 🛠️ Teknologi yang Digunakan

| Teknologi                      | Versi / Konfigurasi |
| ------------------------------ | ------------------- |
| React Native                   | 0.88.0              |
| React                          | 19.3.0              |
| TypeScript                     | 6.0.3               |
| react-native-webview           | ^14.0.1             |
| react-native-safe-area-context | ^5.5.2              |
| Node.js                        | >= 22.11.0          |
| Gradle Wrapper                 | 9.4.1               |
| Android Compile SDK            | 37                  |
| Android Build Tools            | 37.0.0              |
| Android Target SDK             | 36                  |
| Android Minimum SDK            | 24                  |
| NDK                            | 27.1.12297006       |
| Kotlin                         | 2.2.0               |

## 📂 Struktur Repository

```text
mobile-webview-prototype1/
│
├── android/                  # Konfigurasi dan source Android
├── ios/                      # Konfigurasi dan source iOS
├── apk/
│   └── Webview.apk           # File APK
│
├── App.tsx                   # Komponen utama aplikasi
├── app.json                  # Identitas aplikasi
├── index.js                  # Entry point React Native
│
├── package.json              # Dependensi dan scripts
├── package-lock.json         # Lockfile dependensi
├── babel.config.js           # Konfigurasi Babel
├── metro.config.js           # Konfigurasi Metro
├── tsconfig.json             # Konfigurasi TypeScript
├── .gitignore                # Daftar file yang diabaikan Git
└── README.md                 # Dokumentasi proyek
```

## 🚀 Instalasi dan Menjalankan Proyek

### Prasyarat

Pastikan perangkat pengembangan sudah memiliki:

- Node.js versi 22.11.0 atau lebih baru.
- npm.
- Android Studio dan Android SDK.
- Java Development Kit (JDK) yang sesuai dengan konfigurasi Gradle.

### 1. Clone Repository

```bash
git clone https://github.com/melisanrhkm/mobile-webview-prototype1.git
```

### 2. Masuk ke Folder Proyek

```bash
cd mobile-webview-prototype1
```

### 3. Instal Dependensi

```bash
npm install
```

### 4. Jalankan Metro

```bash
npm start
```

### 5. Jalankan Aplikasi Android

Pastikan emulator atau perangkat Android sudah terhubung dan terdeteksi.

```bash
npm run android
```

---

## 📦 APK Aplikasi

File APK yang tersedia di repository:

[**`apk/Webview.apk`**](./apk/Webview.apk)

APK disertakan sebagai berkas hasil proyek. Ketersediaannya di repository tidak dengan sendirinya menjadi bukti bahwa aplikasi telah diuji pada seluruh perangkat Android.

---

## 🎓 Informasi Akademik

| Keterangan             | Detail                            |
| ---------------------- | --------------------------------- |
| Mata Kuliah            | Pemrograman Mobile                |
| Universitas            | Universitas Langlangbuana         |
| Jenis Proyek           | Ujian Tengah Semester (UTS)       |
| Tugas yang Digabungkan | Sesi #2 dan Sesi #3               |
| Metode Pengembangan    | Prototyping                       |
| Platform               | MIT App Inventor dan React Native |

## 👩‍💻 Author

**Melisa Nurhakim**

\<p>   \<a href="[https://github.com/melisanrhkm](https://github.com/melisanrhkm)">     \<img src="[https://img.shields.io/badge/GitHub-melisanrhkm-181717?style=for-the-badge&logo=github](https://img.shields.io/badge/GitHub-melisanrhkm-181717?style=for-the-badge\&logo=github)" alt="GitHub">   \</a> \</p>

---

\<p align="center">
&#x20; \<strong>Portal Kampus — Fabric WebView\</strong>\<br>
&#x20; \<sub>Universitas Langlangbuana · Pemrograman Mobile · 2026\</sub>
\</p>
