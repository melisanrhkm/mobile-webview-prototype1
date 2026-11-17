# 🌐 Portal Kampus - Fabric WebView

Prototipe aplikasi mobile berbasis **React Native** yang digunakan untuk menampilkan website **Universitas Langlangbuana (UNLA)** (`https://www.unla.ac.id/`) langsung di dalam aplikasi menggunakan komponen WebView.

Repository ini merupakan hasil penggabungan **Tugas Sesi #2 dan Tugas Sesi #3** mata kuliah Pemrograman Mobile melalui dua siklus pengembangan dengan metode **Prototyping**.

- **Siklus 1 (Prototype Awal):** Dibuat menggunakan MIT App Inventor dengan pemrograman berbasis blok visual.
- **Siklus 2 (Implementasi):** Dikembangkan menggunakan React Native dan library `react-native-webview`.

---

## 📌 Gambaran Proyek

Proyek ini dikembangkan sebagai media pembelajaran untuk memahami penggunaan WebView dalam aplikasi mobile serta mengenal perbedaan pendekatan pengembangan menggunakan MIT App Inventor dan React Native.

- **Siklus 1:** Prototipe awal menggunakan MIT App Inventor dengan komponen `WebViewer1` untuk membuka website UNLA.
- **Siklus 2:** Implementasi aplikasi menggunakan React Native dengan `react-native-webview`, `SafeAreaView`, dan konfigurasi tampilan aplikasi.

Kedua siklus memiliki tujuan yang sama, yaitu menampilkan website UNLA melalui aplikasi mobile, tetapi menggunakan platform dan pendekatan pengembangan yang berbeda.

---

## ✨ Fitur dan Implementasi

- 🏛️ **Portal Kampus UNLA:** Menampilkan website resmi Universitas Langlangbuana.
- 🌐 **WebView Integration:** Memuat halaman website langsung di dalam aplikasi mobile.
- ⚡ **JavaScript Support:** Mengaktifkan JavaScript pada komponen WebView.
- 🔄 **Loading State:** Menggunakan `startInLoadingState` untuk menangani kondisi pemuatan halaman.
- 📱 **Safe Area:** Menggunakan `SafeAreaView` untuk membantu mengatur area tampilan aplikasi.
- 🎨 **Application Header:** Menampilkan header dengan judul Portal Kampus - Fabric WebView.
- 🔁 **Refresh pada Prototype 1:** Menggunakan tombol `REFRESH` untuk menjalankan fungsi `Reload` pada komponen `WebViewer1` di MIT App Inventor.

---

## 🔄 Metode Pengembangan — Prototyping

Pengembangan proyek dibagi menjadi dua siklus:

### 1. Prototype Awal — MIT App Inventor

Prototipe pertama dibuat menggunakan MIT App Inventor dengan pendekatan visual block-based programming.

| Komponen         | Keterangan                                         |
| ---------------- | -------------------------------------------------- |
| Nama Proyek      | `TEST`                                             |
| Screen           | `Screen1`                                          |
| Judul Aplikasi   | `UNLA APK`                                         |
| Komponen WebView | `WebViewer1`                                       |
| Website          | [https://www.unla.ac.id/](https://www.unla.ac.id/) |
| Tombol           | `REFRESH`                                          |
| Fungsi Tombol    | Menjalankan `Reload` pada `WebViewer1`             |

### 2. Implementasi — React Native

Siklus kedua dikembangkan menggunakan React Native dengan library `react-native-webview`.

Implementasi utama terdapat pada file [`App.tsx`](./App.tsx).

Beberapa bagian implementasinya meliputi:

- Menampilkan header aplikasi Portal Kampus - Fabric WebView.
- Memuat website UNLA menggunakan komponen WebView.
- Mengaktifkan JavaScript.
- Mengatur status pemuatan halaman.
- Menggunakan SafeAreaView.
- Mengatur warna status bar aplikasi.

**Catatan:** Siklus kedua merupakan implementasi menggunakan platform berbeda. Dokumentasi evaluasi atau umpan balik pengguna pada siklus pertama tidak tersedia, sehingga tidak dinyatakan sebagai hasil perbaikan berdasarkan evaluasi tersebut.

---

## 📊 Perbandingan Siklus 1 dan Siklus 2

| Aspek               | Siklus 1 (MIT App Inventor) | Siklus 2 (React Native)       |
| ------------------- | --------------------------- | ----------------------------- |
| Platform            | MIT App Inventor            | React Native                  |
| Teknologi WebView   | WebViewer                   | react-native-webview          |
| Bahasa / Pendekatan | Visual Block Programming    | JavaScript / TypeScript       |
| Website             | UNLA                        | UNLA                          |
| Refresh             | Tombol REFRESH              | Mengikuti konfigurasi WebView |
| Pengembangan        | Visual programming          | Pengembangan berbasis kode    |
| Source Proyek       | Proyek MIT App Inventor     | Source code React Native      |

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

---

## 📥 Instalasi dan Menjalankan Proyek

### Persyaratan

Pastikan perangkat pengembangan telah memiliki:

- Node.js versi 22.11.0 atau lebih baru.
- npm.
- Android Studio dan Android SDK.
- Java Development Kit (JDK) yang sesuai dengan konfigurasi Gradle.

### 1. Clone Repository

```bash
git clone https://github.com/melisanrhkm/mobile-webview-prototype1.git
```

### 2. Masuk ke Direktori Proyek

```bash
cd mobile-webview-prototype1
```

### 3. Instal Dependensi

```bash
npm install
```

### 4. Jalankan Metro Bundler

```bash
npm start
```

### 5. Jalankan Aplikasi Android

Hubungkan perangkat Android atau siapkan emulator yang sudah terdeteksi oleh Android SDK, kemudian jalankan:

```bash
npm run android
```

---

## 📦 APK Aplikasi

Repository ini menyediakan file APK pada direktori `apk/`.

[**📥 Lihat Webview.apk**](./apk/Webview.apk)

File APK disertakan sebagai bagian dari hasil proyek. Keberadaan file tersebut di repository tidak menjadi bukti pengujian pada seluruh perangkat Android.

---

## 📁 Struktur Repository

```text
mobile-webview-prototype1/
│
├── android/                  # Source dan konfigurasi Android
├── ios/                      # Source dan konfigurasi iOS
│
├── apk/
│   └── Webview.apk           # File APK aplikasi
│
├── App.tsx                   # Komponen utama aplikasi
├── app.json                  # Identitas aplikasi
├── index.js                  # Entry point React Native
│
├── package.json              # Konfigurasi dan dependensi proyek
├── package-lock.json         # Lockfile dependensi
├── babel.config.js            # Konfigurasi Babel
├── metro.config.js            # Konfigurasi Metro
├── tsconfig.json              # Konfigurasi TypeScript
├── .gitignore                 # File yang diabaikan Git
└── README.md                  # Dokumentasi proyek
```

---

## 🔗 Repository Proyek

- 🌐 **Website Universitas Langlangbuana:** [https://www.unla.ac.id/](https://www.unla.ac.id/)
- 💻 **Repository GitHub:** [mobile-webview-prototype1](https://github.com/melisanrhkm/mobile-webview-prototype1)

---


---

