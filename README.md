# LPJ Keuangan App 📊

Aplikasi berbasis web sederhana untuk mengelola Laporan Pertanggungjawaban (LPJ) keuangan kepanitiaan atau organisasi per komisi/seksi.

## 🚀 Fitur Utama
- **Manajemen Komisi/Seksi:** Pencatatan alokasi anggaran khusus untuk tiap divisi.
- **Pencatatan Transaksi:** Input pengeluaran dan pemasukan dengan pemformatan mata uang otomatis.
- **Laporan & Rekapitulasi:** Pemantauan sisa saldo/kas secara real-time.
- **Export Data:** Ekspor riwayat transaksi ke format CSV/Excel.
- **Fitur Cetak:** Ekspor rekapitulasi ke format PDF/cetak langsung via browser.
- **Penyimpanan Lokal:** Menggunakan `localStorage` sehingga data tersimpan otomatis di browser tanpa memerlukan database tambahan.

## 🛠️ Teknologi yang Digunakan
- HTML5 & JavaScript (ES6)
- Tailwind CSS (via CDN)
- FontAwesome (Ikon)

## 📖 Cara Penggunaan
1. Buka berkas `index.html` langsung di browser favoritmu, atau kunjungi tautan demo (jika diaktifkan di GitHub Pages).
2. Pilih komisi/seksi dari dropdown di header.
3. Masukkan alokasi anggaran awal di tab **Anggaran**.
4. Catat transaksi pemasukan atau pengeluaran di tab **Transaksi**.
5. Lihat ringkasan dan cetak laporan melalui tab **Laporan**.

## 📄 Lisensi
[MIT License](LICENSE)
# Sistem Aplikasi LPJ Keuangan Kepanitiaan 💰

Aplikasi web berbasis **Google Apps Script** dan **Tailwind CSS** untuk membantu panitia acara mengelola anggaran serta merekapitulasi laporan transaksi pertanggungjawaban (LPJ) per divisi/seksi secara real-time ke Google Sheets.

## 🚀 Fitur Utama
- **Multi Komisi / Seksi**: Mengakomodasi pencatatan terpisah untuk 8 divisi/seksi kepanitiaan.
- **Pencatatan Real-Time**: Terhubung langsung ke Google Sheets sebagai database utama.
- **Ringkasan Laporan & Cetak**: Rekapitulasi otomatis dengan visualisasi saldo dan fitur cetak/PDF bawaan.
- **Export Data**: Unduh laporan transaksi ke file Excel/CSV.

## 🛠️ Struktur Repositori
- `Code.gs` — Backend script yang menangani komunikasi data ke Google Sheets.
- `Index.html` — Antarmuka pengguna (Frontend UI).

## 📋 Cara Setup & Deployment

1. **Buat Google Sheets Baru**
   - Buat file Google Sheets baru.
   - Buat 2 lembar (sheet) bernama `Anggaran` dan `Transaksi`.

2. **Setup Google Apps Script**
   - Buka menu **Extensions (Ekstensi)** > **Apps Script**.
   - Salin kode dari `Code.gs` dan paste ke file `Code.gs` di editor.
   - Ubah variabel `URL_SHEET` dengan ID Google Sheets kamu.
   - Buat file HTML baru bernama `Index.html` dan paste isi dari file `Index.html`.

3. **Deploy sebagai Web App**
   - Klik tombol **Deploy** > **New deployment**.
   - Pilih tipe **Web app**.
   - Set *Execute as*: **Me**.
   - Set *Who has access*: **Anyone** (atau atur sesuai preferensi organisasi).
   - Klik **Deploy** dan jalankan URL yang dihasilkan.
