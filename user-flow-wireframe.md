# Alur Pengguna (User Flow) & Spesifikasi Wireframe — AksesWarga

Dokumen ini adalah cetak biru susunan layout dan alur interaksi untuk diimplementasikan langsung pada **Figma**.

---

## 1. Alur Pengguna Utama (Core User Flows)

### Flow 1: Menemukan Rute Aman Mobilitas (Kursi Roda / Lansia)
```
[Buka Web AksesWarga] 
       │
       ▼
[Ketik Lokasi Tujuan di Search Box] 
       │
       ▼
[Pilih Filter Kebutuhan Khusus: "Kursi Roda / Tanpa Tangga"] 
       │
       ▼
[Sistem Menampilkan 2 Pilihan Rute di Peta]
  - Rute A (Rekomendasi Inklusif: Landai, ada ramp, trotoar mulus)
  - Rute B (Jalur Cepat tapi Ada Hambatan Tangga)
       │
       ▼
[Klik "Mulai Navigasi Aman" / Dengarkan Panduan Suara]
```

### Flow 2: Mengecek Aksesibilitas Fasilitas Publik (Contoh: Puskesmas / Stasiun)
```
[Buka Tab "Direktori Fasilitas"] 
       │
       ▼
[Pilih Kategori: "Fasilitas Kesehatan"] 
       │
       ▼
[Pilih "Puskesmas Kecamatan Melati"] 
       │
       ▼
[Lihat Kartu Indeks Aksesibilitas: Ramp (Ada), Toilet Disabilitas (Ada), Lift (Tidak)]
       │
       ▼
[Klik "Panduan Menuju Lokasi" atau "Hubungi Petugas Prioritas"]
```

### Flow 3: Lapor Hambatan Akses Trotoar / Fasilitas Rusak (Inklusif & Tanpa Login)
```
[Klik Tombol Mengambang "Lapor Hambatan Jalan"] 
       │
       ▼
[Langkah 1: Ambil / Upload Foto Trotoar Rusak] 
       │
       ▼
[Langkah 2: Rekam Suara (atau Tulis): "Ubin pemandu tunanetra terputus dekat halte"] 
       │
       ▼
[GPS Mendeteksi Titik Otomatis -> Klik "Kirim Laporan"] 
       │
       ▼
[Muncul Kartu Tiket Laporan & Status Terkirim ke Dinas Terkait]
```

---

## 2. Spesifikasi Tata Letak Wireframe (5 Layar Utama di Figma)

### Layar 1: Beranda (Home & Interactive Map Explorer)
* **Header / Navigasi Atas**:
  * Logo **AksesWarga** + Tagline
  * Menu: *Peta Rute*, *Fasilitas Publik*, *Lapor Hambatan*, *Panduan*
  * **Accessibility Toolbar**: Tombol Ukuran Font (A- / A+), Tombol Kontras Tinggi, Tombol Suara.
* **Hero Search Area**:
  * Judul: *"Mau Menuju ke Mana Hari Ini?"*
  * Input Form: [Pilih Titik Berangkat] ke [Pilih Titik Tujuan]
  * Kancing Filter Cepat: `[♿ Pengguna Kursi Roda]` `[🦯 Tunanetra]` `[👵 Lansia/Tongkat]` `[👶 Kereta Bayi]`
  * Tombol CTA: **[Cari Rute Aksesibel]**
* **Kontainer Peta Interaktif**:
  * Peta live menampilkan jalur hijau (ramah), titik oranye (waspada), titik merah (rusak/tangga).
  * Panel ringkasan fasilitas ramah terdekat.

---

### Layar 2: Hasil Navigasi Rute Ramah Mobilitas (Navigation View)
* **Sidebar Kiri (Panel Rute)**:
  * Detail Rute Terpilih: "Rute Landai via Jl. Pemuda (15 Menit - 850m)"
  * Badge Status: `100% Bebas Tangga` `Tersedia Ramp Landai` `Trotoar Lebar > 1.8m`
  * Petunjuk Langkah-demi-Langkah (*Step-by-step cue*):
    * Titik 01: Mulai dari Stasiun Timur -> Belok Kiri melewati Ramp Landai.
    * Titik 02: Peringatan: 50 meter ke depan ada perbaikan paving (disarankan menyeberang via Pelican Crossing).
  * Tombol CTA: **[Dengarkan Petunjuk Suara]** & **[Bagikan Rute]**
* **Sisi Kanan**: Peta dengan garis jalur hijau terang yang jelas.

---

### Layar 3: Detail Direktori Fasilitas Publik (Place Accessibility Card)
* **Header Tempat**: Nama Faskes / Gedung ("Puskesmas Melati Sejahtera") + Foto Tampak Depan.
* **Badge Skor Aksesibilitas**: Skor Lingkaran Besar **88/100 (Sangat Inklusif)**.
* **Daftar Fasilitas Riil (Grid Checklist dengan Ikon Jelas)**:
  * [x] *Ramp Pintu Masuk (Kemiringan < 8 derajat)*
  * [x] *Toilet Khusus Kursi Roda (Pintu geser, ada pegangan besi)*
  * [x] *Guiding Block Kuning untuk Tunanetra*
  * [!] *Loket Khusus Lansia & Prioritas*
  * [-] *Lift Braille (Tidak Tersedia / Gedung 1 Lantai)*
* **Ulasan Komunitas & Catatan Riil Pengguna Disabilitas**.

---

### Layar 4: Modal Lapor Hambatan Akses (Quick Report Dialog)
* **Header**: "Lapor Fasilitas / Trotoar yang Menghambat Mobilitas"
* **Area 1 — Foto Bukti**: Kotak besar untuk drop foto atau tombol kamera instan.
* **Area 2 — Deskripsi Suara (Voice First)**: Tombol Mikrofon Raksasa dengan teks: *"Tekan dan tahan untuk merekam suara Anda"*. (Tersedia opsi ketik manual jika tidak ingin bicara).
* **Area 3 — Lokasi**: Peta kecil dengan pin otomatis lokasi saat ini (bisa digeser jika perlu).
* **Tombol Aksi**: **[Kirim Laporan Sekarang]** (Besar, kontras tinggi).

---

### Layar 5: Tampilan Mode Kontras Tinggi / Senior Mode (Design Showcase)
* Menampilkan bagaimana tampilan Beranda berubah ketika **Accessibility Toolbar** diaktifkan:
  * Latar belakang menjadi hitam `#121212`, teks dan ikon kuning menyala `#FFD166`.
  * Ukuran font diperbesar 150%.
  * Tombol menjadi blok tebal dengan pembatas kontras untuk membuktikan kesiapan penilaian aksesibilitas WCAG kepada juri.
