# 🛡️ SiDul BPS - Sistem Informasi Pengaduan Layanan

<div align="center">
  <img src="logo_sidulApp.jpeg" alt="Logo SiDul" width="120" height="120" style="border-radius: 50%;">
  <p><b>Aplikasi Layanan Pengaduan & Aspirasi Masyarakat Berbasis Web</b></p>
  <p><i>BPS Provinsi Kepulauan Bangka Belitung</i></p>
</div>

---

## 📋 Tentang Project
**SiDul (Sistem Informasi Pengaduan Layanan)** adalah platform web interaktif yang dikembangkan untuk memfasilitasi masyarakat, mitra statistik, maupun pegawai internal dalam menyampaikan pengaduan, laporan indikasi *fraud*, masalah kepegawaian, atau ketidakpuasan layanan di lingkungan **BPS Provinsi Kepulauan Bangka Belitung**. 

Aplikasi ini dirancang untuk memberikan transparansi penuh dengan alur penanganan yang terstruktur sesuai Standar Operasional Prosedur (SOP) serta fitur pelacakan tiket secara *real-time*.

---

## 🚀 Fitur Utama
* **Formulir Pengaduan Interaktif**: Dilengkapi pilihan pelaporan secara **Anonim** (samarkan identitas), validasi nomor HP, penghitung karakter uraian, serta fitur unggah bukti dokumen/foto (maksimal 5MB).
* **Fitur Download Tiket Otomatis**: Setiap laporan yang berhasil dikirim akan menghasilkan nomor tiket unik dengan tombol unduh kartu bukti aduan berbasis gambar (`html2canvas`).
* **Lacak Status Pengaduan**: Pengguna dapat memantau status penanganan aduan (Menunggu, Proses, Selesai) secara mandiri hanya dengan memasukkan nomor tiket.
* **Panel Admin Dashboard (`adminnew.html`)**: 
  * Autentikasi sesi admin yang aman dengan batas waktu (*session timeout*).
  * Statistik ringkasan data pengaduan secara *real-time*.
  * Manajemen ubah status laporan & entri catatan tindak lanjut.
  * Fitur publikasi pengumuman/berita beranda secara dinamis.
  * Fitur **Export data ke format CSV** untuk keperluan pelaporan instansi.
* **Floating WhatsApp Center**: Integrasi widget chat langsung dengan petugas Pelayanan Statistik Terpadu (PST).

---

## 🛠️ Teknologi yang Digunakan
Project ini dibangun tanpa *framework* backend yang berat, mengandalkan arsitektur modern berbasis web frontend dan serverless:
* **Frontend**: 
  * HTML5 & CSS3
  * **Bootstrap 5** (Desain UI yang responsif dan elegan)
  * **Font Awesome** (Ikon pendukung antarmuka)
  * **JavaScript (ES6+)** (Logika aplikasi, manajemen DOM, dan *asynchronous fetch*)
* **Library Tambahan**: `html2canvas` (Untuk render dan unduh kartu tiket aduan)
* **Backend & Database**: **Google Apps Script (GAS)** & **Google Sheets** (Berfungsi sebagai database *serverless* dan REST API sederhana).

---

## 📁 Struktur File Repository
```text
webSidulBPSBabel/
│
├── index.html          # Halaman utama (Beranda, Form Aduan, Lacak Status, Kanal, FAQ)
├── adminnew.html       # Halaman Dashboard Admin untuk pengelolaan data & pengumuman
├── logo_sidulApp.jpeg  # Aset logo resmi aplikasi SiDul
└── logo_bps.webp       # Aset logo resmi Badan Pusat Statistik
