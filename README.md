# Portal Kampus - Fabric WebView

Prototipe aplikasi mobile berbasis React Native yang menampilkan situs Universitas Langlangbuana (UNLA) di dalam aplikasi menggunakan komponen WebView. Repository ini merupakan hasil penggabungan Tugas Sesi #2 dan Tugas Sesi #3 melalui dua siklus metode Prototyping.

## Latar Belakang

Perangkat mobile dapat digunakan untuk mengakses layanan dan informasi kampus secara lebih praktis. Salah satu penerapannya adalah penggunaan komponen WebView untuk menampilkan halaman website langsung di dalam aplikasi mobile.

Proyek ini menggabungkan dua tugas praktikum yang memiliki tujuan serupa, yaitu membuat aplikasi mobile yang dapat menampilkan website menggunakan WebView. Pengembangan dilakukan melalui dua siklus Prototyping dengan platform yang berbeda.

## Tujuan

1. Memahami penerapan komponen WebView pada aplikasi mobile.
2. Membuat aplikasi sederhana untuk mengakses website Universitas Langlangbuana.
3. Mengenal proses pengembangan aplikasi menggunakan MIT App Inventor dan React Native.
4. Menggabungkan hasil Tugas Sesi #2 dan Tugas Sesi #3 dalam satu repository GitHub.

## Metode Pengembangan

Metode yang digunakan adalah **Prototyping**, yaitu metode pengembangan perangkat lunak yang dilakukan melalui pembuatan prototype secara bertahap.

Pada proyek ini, metode Prototyping diterapkan melalui dua siklus pengembangan:

1. **Siklus 1 – Prototype Awal:** Pembuatan aplikasi WebView menggunakan MIT App Inventor.
2. **Siklus 2 – Pengembangan Prototype:** Pembuatan aplikasi WebView menggunakan React Native.

Kedua siklus merupakan implementasi menggunakan platform yang berbeda. Tidak terdapat klaim evaluasi atau perbaikan berdasarkan umpan balik pengguna karena hasil evaluasi tersebut tidak didokumentasikan.

## Siklus 1 – Prototype Awal (MIT App Inventor)

Pada siklus pertama, aplikasi dibuat menggunakan MIT App Inventor dengan memanfaatkan komponen WebViewer untuk menampilkan website.

### Implementasi

Berdasarkan berkas proyek yang tersedia, implementasi memiliki konfigurasi berikut:

| Komponen         | Keterangan                      |
| ---------------- | ------------------------------- |
| Platform         | MIT App Inventor                |
| Nama proyek      | TEST                            |
| Screen           | Screen1                         |
| Judul aplikasi   | UNLA APK                        |
| Komponen WebView | WebViewer1                      |
| Website          | https://www.unla.ac.id/         |
| Tombol           | REFRESH                         |
| Fungsi tombol    | Memuat ulang halaman WebViewer1 |

### Fitur

- Menampilkan website Universitas Langlangbuana melalui WebViewer.
- Menyediakan tombol REFRESH untuk memuat ulang halaman website.

## Siklus 2 – Pengembangan Prototype (React Native)

Pada siklus kedua, aplikasi dikembangkan menggunakan React Native dengan library `react-native-webview`.

Pengembangan ini menggunakan JavaScript/TypeScript dan lingkungan React Native untuk membuat aplikasi mobile yang menampilkan website Universitas Langlangbuana.

### Implementasi

| Komponen           | Keterangan                     |
| ------------------ | ------------------------------ |
| Framework          | React Native                   |
| Bahasa pemrograman | TypeScript                     |
| Komponen WebView   | react-native-webview           |
| Website            | https://www.unla.ac.id/        |
| File utama         | App.tsx                        |
| Tampilan header    | Portal Kampus - Fabric WebView |

### Fitur

- Menampilkan halaman website Universitas Langlangbuana.
- Menggunakan komponen WebView untuk memuat website di dalam aplikasi.
- Mengaktifkan JavaScript pada WebView.
- Menampilkan indikator proses pemuatan halaman awal.
- Menggunakan Safe Area Context untuk mendukung area aman tampilan perangkat.

### Teknologi yang Digunakan

| Teknologi                      | Versi/Keterangan |
| ------------------------------ | ---------------- |
| React Native                   | 0.88.0           |
| React                          | 19.3.0           |
| TypeScript                     | 6.0.3            |
| react-native-webview           | ^14.0.1          |
| react-native-safe-area-context | ^5.5.2           |
| Node.js                        | >=22.11.0        |
| Gradle                         | 9.4.1            |
| Android Compile SDK            | 37               |
| Android Build Tools            | 37.0.0           |
| Android Target SDK             | 36               |
| Android Minimum SDK            | 24               |
| NDK                            | 27.1.12297006    |
| Kotlin                         | 2.2.0            |

## Struktur Repository

```text
mobile-webview-prototype1/
│
├── android/
├── ios/
├── apk/
│   └── Webview.apk
│
├── App.tsx
├── index.js
├── package.json
├── package-lock.json
├── babel.config.js
├── metro.config.js
├── tsconfig.json
├── .gitignore
└── README.md
```
