# DompetKu — Premium UI Revamp

Pembaruan tampilan menyeluruh untuk DompetKu berbasis HTML, CSS, dan JavaScript murni. Logika transaksi dan penyimpanan finansial tidak dirombak.

## Cara memakai
1. Ekstrak ZIP.
2. Ganti file `index.html` dan `style.css` di repositori dengan file versi ini.
3. Pertahankan `script.js` versi proyek yang saat ini berfungsi. File `script.js` dalam paket ini disertakan sebagai pendamping dan logika keuangan tidak diubah dari versi sumber yang dipakai untuk revamp.
4. Pastikan file logo berada di folder yang sama dengan `index.html`.
5. Buka `index.html`, cari baris ini:

   `const DOMPETKU_LOGO_FILE = "logo.svg";`

   Ganti **hanya** `logo.svg` dengan nama file logo milikmu, misalnya `brand-dompetku.svg` atau `ikon.png`. Nama file harus sama persis, termasuk huruf besar/kecil. File PNG dan SVG sama-sama didukung.
6. Commit ke GitHub dan tunggu deployment Vercel selesai.

## Yang diperbarui
- Desain antarmuka premium bertema hijau-obsidian, kartu dan tipografi lebih konsisten.
- Dashboard responsif untuk HP dan desktop.
- Menu samping desktop serta menu hamburger pada HP.
- Tampilan transaksi, target tabungan, anggaran, rekening, laporan, formulir, dan dialog diperbarui.
- Logo pada layar pembuka dan identitas aplikasi diatur dari satu nama file di `index.html`.

## Fitur keuangan yang dipertahankan
- Tambah/edit/hapus, cari, dan filter transaksi.
- Saldo rekening, pemasukan, pengeluaran, dan kategori.
- Target tabungan, anggaran bulanan, rekening/dompet.
- Transaksi berulang, grafik arus kas, laporan, ekspor CSV, cetak/PDF.
- Backup JSON, pemulihan backup, profil, dan pengingat.

## Catatan
Data proyek sumber disimpan di `localStorage` browser. UI ini tidak memigrasikan atau menghapus data. Tetap simpan backup sebelum mengganti file pada situs yang sedang digunakan. Jika proyek PWA-mu memiliki `manifest.json` terpisah, ubah ikon manifest secara terpisah bila kamu juga ingin ikon di layar utama Android ikut berubah.
