# Alur Pengguna (User Flow) & Spesifikasi Wireframe — KawanTumbuh

Dokumen ini adalah cetak biru susunan layout dan alur interaksi untuk diimplementasikan langsung pada **Figma** (Desktop 1440px).

---

## 1. Alur Pengguna Utama (Core User Flows)

### Flow 1: Skrining Mandiri Tumbuh Kembang Balita
```
[Buka Web KawanTumbuh] 
       │
       ▼
[Pilih Rentang Usia Anak di Beranda: misal "1-3 Tahun"] 
       │
       ▼
[Masuk ke Halaman Skrining Visual]
  - Pertanyaan 1 (Wicara): "Apakah anak bisa menunjuk benda saat disebutkan namanya?" [🔊 Audio]
  - Pengguna melihat ilustrasi kartun -> Klik [✓ Sudah Bisa]
  - Pertanyaan 2 (Motorik): "Apakah anak bisa berjalan tanpa berpegangan?"
  - Pengguna klik [✕ Belum Bisa]
       │
       ▼
[Selesai 5 Pertanyaan -> Muncul Lembar Hasil Evaluasi Ramah Keluarga]
  - Motorik: Sesuai Usia (Hijau)
  - Bicara: Butuh Stimulasi Tambahan (Kuning)
       │
       ▼
[Klik "Mulai Latihan Stimulasi Hari Ini" atau "Simpan Hasil"]
```

### Flow 2: Mengakses Playbook Stimulasi Harian Mandiri di Rumah
```
[Masuk Menu "Playbook Stimulasi"] 
       │
       ▼
[Pilih Kategori: "Melatih Bicara & Bahasa"] 
       │
       ▼
[Pilih Aktivitas: "Meniup Bola Kapas (Melatih Otot Mulut & Bicara)"] 
       │
       ▼
[Buka Halaman Aktivitas]
  - Daftar alat murah di rumah (Kapas + Sedotan)
  - Video animasi 30 detik cara bermain bersama anak
  - Tombol Audio: Dengarkan instruksi suara
       │
       ▼
[Orang tua mempraktikkan langsung bersama balita di rumah]
```

---

## 2. Spesifikasi Tata Letak Wireframe (5 Layar Utama di Figma)

### Layar 1: Beranda (Home & Educational Portal)
* **Header / Navigasi Atas**:
  * Logo **KawanTumbuh** (Ikon Tunas Tumbuh & Hati) + Tagline
  * Menu: *Deteksi Dini*, *Playbook Stimulasi*, *Direktori Faskes*, *Edukasi*
  * **Accessibility Toolbar**: Tombol Ukuran Teks (`A-` / `A+`), Tombol Kontras Tinggi (`🌓`), Tombol Suara (`🔊`).
* **Hero Section**:
  * Judul Besar: *"Kenali Potensi Emas Anak Anda Sejak Dini"*
  * Subjudul: *"Skrining tumbuh kembang mandiri, deteksi anak berkebutuhan khusus, dan panduan stimulasi bermain gratis untuk keluarga Indonesia."*
  * Tombol CTA Utama: **[Mulai Deteksi Tumbuh Kembang (Gratis)]**
* **Quick Age Selector (Pemilih Usia Cepat)**:
  * 3 Kartu Ilustrasi Besar:
    1. `[👶 Bayi 0 - 12 Bulan]` (Milestone: Tengkurap, Merespons Suara)
    2. `[🧒 Balita 1 - 3 Tahun]` (Milestone: Berjalan, Kata Pertama)
    3. `[👦 Pra-Sekolah 4 - 6 Tahun]` (Milestone: Bersosialisasi, Kalimat Lengkap)
* **Pojok Edukasi (Tanda Bahaya Perkembangan)**:
  * 3 Kartu Edukasi bergambar: *Kapan harus waspada anak belum bicara?*, *Mengenal sensitivitas sensorik anak autis*, *Pentingnya protein lokal untuk otak*.

---

### Layar 2: Skrining Visual Interaktif (Assessment Screen)
* **Bar Progres Atas**:
  * Indikator Langkah: *"Pertanyaan 2 dari 5 (Kategori: Kemampuan Bicara & Bahasa)"* + Bar Progres Hijau.
* **Area Pertanyaan Utama**:
  * Kartu Putih Besar di Tengah:
    * Ilustrasi Kartun Jelas: Gambar anak sedang menunjuk gambar kucing di buku cerita.
    * Teks Pertanyaan (Besar & Jelas): *"Apakah anak dapat menunjuk gambar benda yang disebutkan oleh orang tua?"*
    * Tombol Audio: `[🔊 Dengarkan Pertanyaan Ini]`
* **Tombol Respon Biner (Super Besar 56px)**:
  * Tombol Hijau: **[✓ Sudah Bisa Mandiri]**
  * Tombol Abu/Oranye: **[✕ Belum Bisa / Jarang]**
* **Petunjuk Bawah**: *"Tidak perlu cemas jika belum bisa, setiap anak memiliki waktu tumbuh masing-masing."*

---

### Layar 3: Lembar Hasil & Rekomendasi Ramah Keluarga (Evaluation Result)
* **Header Hasil**:
  * Badge Kalimat Hangat: *"Hasil Evaluasi Tumbuh Kembang Ananda Budi (Usia 2 Tahun 3 Bulan)"*
* **Ringkasan 4 Pilar Perkembangan (Grid 4 Kartu Bersih)**:
  1. *Motorik Kasar*: 🟢 **Sesuai Usia** (Anak sudah aktif berjalan dan memanjat).
  2. *Motorik Halus*: 🟢 **Sesuai Usia** (Mampu memegang sendok dan menumpuk balok).
  3. *Bicara & Bahasa*: 🟡 **Butuh Stimulasi Tambahan** (Perlu diperbanyak interaksi tatap muka).
  4. *Sosial & Mandiri*: 🟢 **Sesuai Usia** (Mampu tersenyum dan merespons orang lain).
* **Rekomendasi Aksi Nyata**:
  * Kotak Saran Praktis: *"Lakukan stimulasi wicara 15 menit setiap hari dengan aktivitas di Playbook."*
  * 2 Tombol Aksi: **[Buka Panduan Stimulasi Wicara]** dan **[Cari Jadwal Posyandu / Faskes Terdekat]**.

---

### Layar 4: Playbook Stimulasi Harian Mandiri (Home-Therapy Activity Card)
* **Header Aktivitas**:
  * Judul: *"Aktivitas 03: Meniup Gelembung & Bola Kapas"*
  * Kategori: `Melatih Otot Wicara & Fokus Mata` | `Durasi: 10-15 Menit/Hari`
* **Alat & Bahan Sederhana di Rumah (Visual List)**:
  * [x] 1 Mangkok Air Sabun Lembut
  * [x] 1 Buah Sedotan Minum
  * [x] Beberapa Butir Bola Kapas
* **Langkah Bermain Interaktif (Step-by-step dengan Gambar Ilustrasi)**:
  * Langkah 1: Duduk berhadapan setinggi mata anak.
  * Langkah 2: Tiup bola kapas perlahan dan ajak anak menirukan gerakan bibir mencucu.
  * Tombol Suara: **[🔊 Putar Panduan Suara untuk Orang Tua]**
* **Tombol Tandai Selesai**: **[✓ Selesai Bermain Hari Ini (Dapatkan Bintang)]**.

---

### Layar 5: Showcase Mode Aksesibilitas Tinggi (High Contrast & Senior Mode)
* Menampilkan bagaimana tampilan Beranda dan Skrining berubah saat **Accessibility Toolbar** diaktifkan:
  * Latar belakang kanvas menjadi hitam pekat (`#121212`).
  * Teks dan ikon berubah menjadi kuning neon (`#FFD166`) dan putih kontras tinggi.
  * Ukuran teks membesar 130% untuk kakek/nenek pengasuh.
  * Bukti implementasi standar **WCAG 2.1 Level AAA** yang memikat juri lomba.
