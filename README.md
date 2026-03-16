# Tugas Layout Part 1 - Flutter

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)

## Identitas

| | |
|---|---|
| **Nama** | Sulthonika Mahfudz Al Mujahidin |
| **NIM** | 1202230023 |
| **Mata Kuliah** | APB (Aplikasi Perangkat Bergerak) |

## Deskripsi

Tugas ini membuat halaman profil skor TOEFL. Tampilan terdiri dari header sambutan pengguna, card ringkasan hasil tes, dan daftar riwayat tes yang bisa di-scroll.

## Konsep Dasar yang Dipelajari

**StatelessWidget dan StatefulWidget**
Di Flutter ada dua jenis widget dasar. `StatelessWidget` dipakai kalau widget tersebut tidak perlu berubah setelah ditampilkan, contohnya `MyApp` yang hanya mengatur tema dan halaman awal. `StatefulWidget` dipakai kalau widget bisa berubah kondisinya, contohnya `MyHomePage` yang nantinya bisa merespons perubahan data.

**Scaffold dan SafeArea**
`Scaffold` adalah kerangka dasar halaman di Flutter, menyediakan struktur seperti body, appBar, dan lainnya. `SafeArea` dipakai supaya konten tidak tertutup notch atau status bar di bagian atas layar.

**Column dan Row**
`Column` menyusun widget secara vertikal, `Row` secara horizontal. Keduanya adalah pondasi utama menyusun layout. Di tugas ini hampir semua bagian tampilan dibangun dari kombinasi keduanya.

**Padding dan SizedBox**
`Padding` memberi jarak di sekitar widget. `SizedBox` dipakai untuk memberi jarak kosong antar widget atau membatasi ukuran. Lebih tepat dari pakai `Container` kosong yang tidak punya fungsi lain.

**Container dan BoxDecoration**
`Container` dengan `BoxDecoration` dipakai untuk membuat card bergradient pada bagian status TOEFL. Di sini belajar pakai `LinearGradient` untuk warna gradasi dan `borderRadius` untuk sudut melengkung.

**ListView.builder dan Expanded**
`ListView.builder` dipakai untuk menampilkan daftar riwayat tes. Lebih efisien karena hanya me-render item yang sedang terlihat di layar, bukan semua sekaligus. Dibungkus `Expanded` supaya list mengisi sisa ruang yang tersedia tanpa menyebabkan overflow.

**Reusable Widget**
Widget yang dipakai berulang seperti tampilan skor (Listening, Structure, Reading) dipisah menjadi class `_ScoreItem` tersendiri. Tujuannya supaya kode tidak redundan dan lebih mudah diubah kalau ada kebutuhan.


