# Latihan 2 Aplikasi Penghitung Umur Atma Fathul Hadi-(2210010425)

Aplikasi **Penghitung Umur** ini ditulis dalam bahasa pemrograman Java. Aplikasi ini dapat menghitung umur berdasarkan tanggal lahir yang dimasukkan dan menampilkan event-event penting yang terjadi pada tanggal tertentu dalam sejarah.

## Fitur

1. **Penghitungan Umur**: Menghitung umur dari tanggal lahir yang dimasukkan.
2. **Pengambilan Data Event Penting**: Menampilkan daftar peristiwa penting yang terjadi pada tanggal yang sama dalam sejarah melalui API eksternal.
3. **Pembatalan Pengambilan Data**: Aplikasi memungkinkan pembatalan pengambilan data jika pengguna memilih tanggal lain saat data sedang diambil.

## Struktur File

- **PenghitungUmur.java**: Kelas utama yang menjalankan aplikasi, mengelola antarmuka, dan menerima input pengguna.
- **PenghitungUmurHelper.java**: Kelas pembantu yang bertanggung jawab untuk menghitung umur dan mengambil data event penting dari API eksternal.
- **PenghitungUmurFrame.java**: Kelas yang mengatur tampilan antarmuka pengguna dan mengelola aksi pengguna seperti memilih tanggal dan memulai perhitungan.

## Cara Kerja

1. **Pengguna memasukkan tanggal lahir** di aplikasi.
2. Aplikasi **menghitung umur pengguna** dan menampilkannya di antarmuka.
3. Pengguna dapat memilih tanggal tertentu, dan aplikasi akan **mengambil data event penting** dari API eksternal (`https://byabbe.se/on-this-day/`) untuk tanggal tersebut.
4. Jika terdapat event penting, aplikasi menampilkannya dalam area teks. Jika tidak ada event, pengguna akan melihat pesan bahwa tidak ada event untuk tanggal tersebut.

## Persyaratan Sistem

- **Java**: Pastikan Anda memiliki JDK terinstal untuk menjalankan aplikasi ini.
- **Koneksi Internet**: Diperlukan untuk mengambil data event dari API eksternal.

## Catatan

- API eksternal yang digunakan untuk pengambilan data event penting hanya menyediakan informasi dalam bahasa Inggris.
- Pastikan koneksi internet stabil saat menggunakan fitur pengambilan event penting, karena aplikasi membutuhkan koneksi untuk mengakses data.

## Contoh Tampilan

- **Input Tanggal Lahir**: Pengguna memasukkan tanggal lahir untuk menghitung umur.
- **Hasil Penghitungan Umur**: Aplikasi menampilkan hasil umur berdasarkan input.
- **Tampilan Event Penting**: Daftar event penting pada tanggal tertentu ditampilkan dalam area teks, atau pesan "Tidak ada peristiwa penting yang ditemukan pada tanggal ini" jika tidak ada data event yang tersedia.

## Penanganan Error

- Jika terdapat kesalahan saat mengakses API atau koneksi terputus, aplikasi akan menampilkan pesan "Gagal mendapatkan data peristiwa".
- Jika pengguna memilih tanggal lain saat data sedang diambil, proses pengambilan data akan dibatalkan.
