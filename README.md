# Hirarki Sistem

Aplikasi web untuk mengelola hirarki atau pohon struktur organisasi, proyek, maupun data bertingkat lainnya. Semua fitur tersimpan dalam satu file HTML (`index.html`) sehingga mudah dibawa dan dijalankan tanpa server — cukup buka di peramban.

> **Demo video:** https://youtu.be/cBe0hN7ZHIM

## Fitur

- **Treeview interaktif** — lihat, perluas, dan ciutkan seluruh hirarki dengan garis penghubung antar node.
- **Manajemen node** — buat node baru, tambah child, ubah nama (klik ganda atau `F2`), dan hapus node beserta seluruh turunannya (menu titik-3 atau tombol `Delete`).
- **Seret & letakkan** — atur ulang posisi node (sebelum, sesudah, atau sebagai child) dengan validasi agar tidak membentuk siklus.
- **Panel detail** — isi dan lihat detail per node: nama, deskripsi, ditugaskan kepada, status selesai (checkbox), dan tanggal selesai (format `dd/mm/yyyy`, terisi otomatis saat dicentang).
- **Tanda selesai** — node yang sudah dicentang selesai ditampilkan dengan ikon check hijau langsung di tree.
- **Panel dapat diatur ukurannya** — tarik pembatas untuk menyesuaikan lebar panel kiri dan kanan.
- **Pencarian** — cari node berdasarkan nama atau deskripsi.
- **Simpan di perangkat** — dokumen disimpan sebagai file `.hirarki` (format JSON), termasuk pemulihan dokumen saat membuka ulang.
- **Pintasan keyboard** — `Ctrl+N`, `Ctrl+O`, `Ctrl+S`, `Ctrl+Shift+S`, `F2` (rename), `Delete` (hapus).
- **Responsif** — pada layar kecil panel otomatis bertumpuk.

## Cara Penggunaan

1. Buka `index.html` di peramban (Chrome/Edge/Firefox modern).
2. Gunakan menu **Berkas → Baru** untuk memulai dokumen kosong, atau **Berkas → Buka** untuk memuat file `.hirarki` yang sudah ada.
3. Klik **Berkas → Simpan / Simpan Sebagai** untuk menyimpan dokumen ke perangkat Anda.
4. Setiap perubahan ditandai dengan titik kuning di samping nama dokumen.

## Format File

- Ekstensi: `.hirarki`
- Isi: JSON dengan struktur `{ app, version, savedAt, roots }`, tempat seluruh node hirarki (termasuk detailnya) disimpan secara rekursif.

## Teknologi

- HTML, CSS (Bootstrap 5.3.3), JavaScript murni (tanpa framework)
- Bootstrap Icons untuk ikon
- File System Access API dengan penggantian otomatis ke unduhan biasa

## Kredit

Dirancang oleh **Emanuel Setio Dewo**.

Repository: https://github.com/setiodewo/hirarki-sistem