# DRAF PROPOSAL KONSEP DESAIN (MAKSIMAL 2 HALAMAN)
**Kompetisi**: IT - Competition AMIKOM Surakarta (IT-CAS) 2026  
**Kategori**: UI/UX Web Design (Pelajar)  
**Judul Karya**: **KawanTumbuh — Ruang Digital Edukasi & Deteksi Dini Tumbuh Kembang Anak Inklusif Menuju Indonesia Emas**  
**Link Prototipe Figma**: `[MASUKKAN_LINK_FIGMA_PROTOTYPE_VIEW_ACCESS_DI_SINI]`  

---

## HALAMAN 1: LATAR BELAKANG, KONSEP EDU-HEALTH & FITUR UTAMA

### 1. Latar Belakang Masalah
Masa depan **Indonesia Emas 2045** ditentukan pada periode usia emas (*Golden Age*, 0–6 tahun), di mana 80% perkembangan otak manusia terbentuk. Namun, di Indonesia jutaan anak mengalami gangguan tumbuh kembang—mulai dari keterlambatan bicara (*speech delay*), gangguan sensorik-motorik, autisme, ADHD, hingga stunting—yang **terlambat dideteksi dan ditangani**. 

Masyarakat di daerah pelosok, keluarga prasejahtera, dan pengasuh lansia (kakek/nenek) kerap terhalang oleh:
1. **Minimnya Literasi Pola Asuh**: Gejala awal disabilitas kognitif/perkembangan sering dianggap hal biasa ("nanti juga bisa bicara sendiri") atau anak diberi cap "nakal/bodoh".
2. **Mahalnya Biaya Konsultasi & Ketiadaan Dokter Spesialis**: Layanan dokter spesialis tumbuh kembang anak hanya terpusat di kota besar dengan biaya terapi yang tidak terjangkau warga miskin.
3. **Sistem Kesehatan yang Kaku**: Informasi medis yang ada dipenuhi istilah klinis latin yang membingungkan dan tidak menyertakan panduan stimulasi praktis sehari-hari di rumah.

### 2. Deskripsi Konsep: Edu-Health Inklusif
**KawanTumbuh** adalah platform web responsif yang menggabungkan pilar **Pendidikan (*Education*)** dan **Kesehatan Anak (*Healthcare*)**. Dirancang dengan standar aksesibilitas **WCAG 2.1 Level AAA**, KawanTumbuh mendemokratisasi deteksi dini tumbuh kembang balita dan membekali orang tua dengan panduan stimulasi bermain mandiri di rumah (*Home-Therapy Playbook*) secara gratis, bebas jargon medis, dan ramah bagi warga berliterasi rendah.

### 3. Fitur Utama Solusi
1. **Interactive Visual Milestone Screening (Deteksi Dini Bergambar)**: Kuesioner skrining perkembangan anak (KPSP yang disederhanakan) menggunakan animasi visual nyata per rentang usia (0–12 bulan, 1–3 tahun, 4–6 tahun) untuk mengevaluasi 4 pilar: Motorik Kasar, Motorik Halus, Bicara & Bahasa, serta Kemandirian.
2. **Home-Therapy Playbook (Panduan Stimulasi Mandiri di Rumah)**: Kurikulum aktivitas bermain harian yang melatih wicara dan saraf sensorik anak menggunakan benda-benda sederhana di rumah (spons air, sedotan, kancing baju) dilengkapi video panduan 30 detik.
3. **Voice Guidance & Low-Literacy Support**: Setiap teks pertanyaan dan panduan aktivitas dilengkapi pembaca suara otomatis (*Text-to-Speech*) untuk orang tua yang memiliki keterbatasan membaca atau lansia.
4. **Red Flags Alert & Direktori Faskes Rujukan**: Peringatan tanda bahaya medis yang memerlukan rujukan dokter spesialis serta pemetaan faskes BPJS/Posyandu pendamping terdekat.
5. **Adaptive UI Engine**: Tombol pengubah kontras tinggi (*High Contrast Mode*) dan pembesar teks dinamis di bilah atas (*header*).

---

## HALAMAN 2: ARSITEKTUR INFORMASI, ALUR PENGGUNA & IMPACT INDONESIA EMAS

### 4. Struktur Informasi (Sitemap)
Arsitektur informasi disusun bertingkat dan bebas hambatan kognitif guna memudahkan navigasi pengguna awam (memenuhi bobot struktur informasi 15%):
* **Beranda (Portal Utama)**: Hero Edukasi Golden Age, Pemilih Usia Cepat (3 Kategori), Kartu Tanda Bahaya (*Red Flags*), Bilah Aksesibilitas Global.
* **Modul Skrining Tumbuh Kembang**: Pemilihan Profil Anak, Kuis Visual Bergambar (Langkah 1–5), Lembar Hasil Evaluasi 4 Pilar.
* **Modul Playbook Stimulasi Harian**: Kategori Latihan (Wicara, Motorik, Sensorik), Detail Aktivitas Rumah, Tombol Putar Suara & Checklist Harian.
* **Direktori Faskes & Posyandu**: Peta Lokasi Faskes Ramah Anak & Kontak Kader Kesehatan Desa.
* **Panel Pengaturan Aksesibilitas**: Skala Font Dinamis, Mode Gelap Kontras Tinggi, Pembaca Layar.

### 5. Alur Pengguna (User Flow)
```
[Buka Web KawanTumbuh] ──> [Pilih Rentang Usia Balita: 1-3 Tahun]
                                       │
                                       ▼
                     [Jawab 5 Pertanyaan Skrining Visual]
                     (Dilengkapi Ilustrasi Gambar & Tombol Suara)
                                       │
                                       ▼
                   [Lembar Hasil Evaluasi 4 Pilar Perkembangan]
           ┌───────────────────────────┴───────────────────────────┐
           ▼                                                       ▼
[Kondisi Sesuai Usia (Hijau)]                          [Butuh Stimulasi Tambahan (Kuning/Merah)]
           │                                                       │
           ▼                                                       ▼
[Jaga Perkembangan dengan                          [Buka Home-Therapy Playbook & Praktikkan
 Aktivitas Bermain Harian]                          Stimulasi Wicara/Motorik Mandiri di Rumah]
                                                                   │
                                                                   ▼ (Jika Terdapat Tanda Bahaya)
                                                   [Cek Faskes & Rujukan Dokter Terdekat]
```

### 6. Kebermanfaatan Jangka Panjang & Kontribusi Menuju Indonesia Emas 2045
* **Pencegahan Disabilitas Permanen**: Intervensi tumbuh kembang pada 1.000 Hari Pertama Kehidupan (HPK) terbukti secara klinis mampu memulihkan fungsi saraf dan bicara hingga 80%, mencegah disabilitas permanen sejak balita.
* **Membangun Generasi Bebas Stunting & Cerdas**: Edukasi literasi gizi dan stimulasi otak anak sejak dini menciptakan generasi dengan kapasitas kognitif (IQ) optimal untuk menyongsong Indonesia Emas.
* **Prinsip Inklusivitas Sejati (*Leave No Child Behind*)**: Menghilangkan stigma terhadap anak berkebutuhan khusus (ABK), memanusiakan keluarga miskin desa, dan membangun ruang digital yang memberdayakan masyarakat secara berkelanjutan.
