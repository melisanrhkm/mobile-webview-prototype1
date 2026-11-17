# Portal Kampus - Fabric WebView

Prototipe aplikasi mobile untuk membuka website Universitas Langlangbuana (UNLA) langsung di dalam aplikasi menggunakan WebView. Repository ini merangkum dua tugas praktikum dalam dua siklus Prototyping:

> **Siklus 1:** MIT App Inventor · **Siklus 2:** React Native

## Tentang Proyek

WebView memungkinkan halaman website ditampilkan dari dalam aplikasi mobile. Kedua siklus pada proyek ini memiliki tujuan yang sama, tetapi menggunakan platform berbeda. Siklus 1 dibuat dengan MIT App Inventor, sedangkan Siklus 2 dikembangkan dengan React Native dan `react-native-webview`.

## Tujuan

- Memahami penggunaan komponen WebView pada aplikasi mobile.
- Membuat aplikasi sederhana untuk membuka website Universitas Langlangbuana.
- Mengenal pengembangan aplikasi menggunakan MIT App Inventor dan React Native.
- Menggabungkan Tugas Sesi #2 dan Tugas Sesi #3 dalam satu repository.

## Metode Prototyping

Pengembangan dilakukan dalam dua siklus dengan tujuan menampilkan website melalui WebView. Perbedaan platform menjadikan cara pembuatannya berbeda, tetapi tidak menjadi bukti bahwa Siklus 2 merupakan perbaikan berdasarkan evaluasi Siklus 1. Hasil evaluasi atau umpan balik pengguna tidak didokumentasikan.

| Siklus | Tugas dan platform | Ringkasan |
| --- | --- | --- |
| 1 | Tugas Sesi #2 — MIT App Inventor | Proyek `TEST` pada `Screen1`, dengan judul aplikasi `UNLA APK`, komponen `WebViewer1`, dan tombol `REFRESH` untuk menjalankan fungsi `Reload` pada WebViewer1. |
| 2 | Tugas Sesi #3 — React Native | Menggunakan `react-native-webview` untuk memuat website UNLA. Lihat [App.tsx](./App.tsx). |

## Siklus 1 — MIT App Inventor

Instruksi Tugas Sesi #2 meminta pembuatan prototipe sederhana yang langsung memuat website kampus atau website berita teknologi menggunakan WebView. Data proyek yang tersedia:

| Bagian | Detail |
| --- | --- |
| Platform | MIT App Inventor |
| Nama proyek | `TEST` |
| Screen | `Screen1` |
| Judul aplikasi | `UNLA APK` |
| Komponen WebView | `WebViewer1` |
| Website | [https://www.unla.ac.id/](https://www.unla.ac.id/) |
| Tombol | `REFRESH` |
| Aksi tombol | Menjalankan fungsi `Reload` pada `WebViewer1` |

Rincian tampilan lain, konfigurasi komponen yang tidak tercantum di atas, hasil pengujian, dan evaluasi tidak tersedia. Karena itu, README ini tidak menyimpulkan detail-detail tersebut.

## Siklus 2 — React Native

Siklus 2 menggunakan React Native dan `react-native-webview`. Berdasarkan implementasi di [App.tsx](./App.tsx), aplikasi:

- Menampilkan header “Portal Kampus - Fabric WebView”.
- Langsung memuat website Universitas Langlangbuana ([https://www.unla.ac.id](https://www.unla.ac.id)) di dalam WebView.
- Mengaktifkan JavaScript dan menggunakan `startInLoadingState`.
- Menggunakan `SafeAreaView` serta mengatur warna status bar.

Kedua siklus sama-sama bertujuan menampilkan website UNLA melalui WebView, dengan pendekatan platform yang berbeda. Tidak ada klaim bahwa Siklus 2 dibuat sebagai perbaikan berdasarkan umpan balik Siklus 1 karena bukti evaluasinya tidak tersedia.

## Teknologi

Versi dan konfigurasi berikut merujuk pada `package.json`, `package-lock.json`, dan konfigurasi Gradle proyek:

| Teknologi | Versi atau konfigurasi |
| --- | --- |
| React Native | 0.88.0 |
| React | 19.3.0 |
| TypeScript | 6.0.3 |
| `react-native-webview` | `^14.0.1` |
| `react-native-safe-area-context` | `^5.5.2` |
| Node.js | `>= 22.11.0` |
| Gradle wrapper | 9.4.1 |
| Android Compile SDK | 37 |
| Android Build Tools | 37.0.0 |
| Android Target SDK | 36 |
| Android Minimum SDK | 24 |
| NDK | 27.1.12297006 |
| Kotlin | 2.2.0 |

## Struktur Repository

Berikut ringkasan berkas utama dan folder proyek:

```text
mobile-webview-prototype1/
├── android/
├── ios/
├── apk/
│   └── Webview.apk
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

APK tersedia di [apk/Webview.apk](./apk/Webview.apk).
