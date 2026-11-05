# DRAF PROPOSAL KONSEP DESAIN (MAKSIMAL 2 HALAMAN)
**Kompetisi**: IT - Competition AMIKOM Surakarta (IT-CAS) 2026  
**Kategori**: UI/UX Web Design (Pelajar)  
**Judul Karya**: **AksesWarga — Ruang Digital Navigasi & Direktori Fasilitas Publik Inklusif Menuju Indonesia Emas**  
**Link Prototipe Figma**: `[MASUKKAN_LINK_FIGMA_PROTOTYPE_VIEW_ACCESS_DI_SINI]`  

---

## HALAMAN 1: LATAR BELAKANG, KONSEP & FITUR UTAMA

### 1. Latar Belakang Masalah
Visi **Indonesia Emas 2045** menuntut pembangunan manusia yang setara dan berkeadilan. Namun, dalam kehidupan sehari-hari, jutaan penyandang disabilitas fisik (kursi roda, kruk), disabilitas sensorik (tunanetra), serta kaum lansia mengalami **isolasi sosial dan hambatan mobilitas**. Trotoar yang terputus, jembatan penyeberangan tanpa bidang miring (*ramp*), serta gedung fasilitas publik yang tidak memiliki toilet aksesibel membuat kelompok rentan kesulitan beraktivitas mandiri untuk bekerja, bersekolah, maupun berobat ke puskesmas.

Ketiadaan informasi terpadu mengenai aksesibilitas ruang publik memaksa mereka bergantung pada orang lain atau memilih mengurung diri di rumah. Di sisi lain, masyarakat yang ingin melaporkan fasilitas publik yang rusak kerap terbentur alur birokrasi aplikasi pemerintah yang rumit, mewajibkan pendaftaran NIK, dan tidak ramah bagi warga dengan literasi digital rendah.

### 2. Deskripsi Konsep & Nilai Inklusivitas
**AksesWarga** adalah platform web responsif yang dirancang sebagai ruang digital kolaboratif untuk memetakan, menavigasi, dan memantau fasilitas publik yang ramah disabilitas dan lansia. Mengusung prinsip **WCAG 2.1 Level AAA**, AksesWarga hadir dengan antarmuka yang adaptif, beban kognitif rendah, serta mendukung interaksi multimodal (layar sentuh, navigasi keyboard penuh, dan perintah suara).

### 3. Fitur Utama Solusi
1. **Accessible Route Finder (Navigasi Rute Ramah Mobilitas)**: Menyajikan rekomendasi rute perjalanan harian yang 100% bebas hambatan tangga, memiliki ramp landai, trotoar rata, serta panduan suara langkah-demi-langkah.
2. **Public Places Accessibility Index (Direktori Fasilitas Inklusif)**: Informasi terverifikasi mengenai kelengkapan fasilitas ramah disabilitas pada fasilitas kesehatan, transportasi publik, dan pasar tradisional dengan skor keterbukaan (0–100%).
3. **One-Click Voice Crowdsourced Report (Lapor Hambatan Tanpa Ketik)**: Memungkinkan seluruh lapisan masyarakat, termasuk lansia dan warga awam teknologi, melaporkan jalan rusak/terhalang cukup dengan mengunggah foto dan merekam pesan suara (*voice note*).
4. **Adaptive UI Engine**: Tombol pengubah kontras tinggi (*High Contrast Mode*), pembesar teks dinamis, dan pembaca layar terintegrasi langsung di bilah atas (*header*).

---

## HALAMAN 2: ARSITEKTUR INFORMASI, ALUR DESAIN & POTENSI IMPLEMENTASI

### 4. Struktur Informasi (Sitemap)
Sistem informasi AksesWarga disusun secara hierarkis dan intuitif guna memudahkan penemuan informasi (menjawab kriteria struktur informasi 15%):
* **Beranda**: Hero Search Rute Inklusif, Filter Kategori Kebutuhan, Peta Sebaran Jalur Aman Terdekat, dan Bilah Aksesibilitas Cepat.
* **Halaman Navigasi Rute**: Detail Langkah Perjalanan, Titik Peringatan Hambatan, Peta Interaktif Rute Hijau.
* **Halaman Direktori Fasilitas**: Profil Fasilitas, Checklist Aksesibilitas Terverifikasi, Ulasan Komunitas Disabilitas.
* **Modal Lapor Hambatan**: Input Multimodal (Foto + Voice Note), Deteksi Geotagging Otomatis, Kartu Pelacakan Status Penanganan.

### 5. Alur Pengguna (User Flow)
```
[Pengguna Membuka Web] ──> [Pilih Kebutuhan: Kursi Roda/Lansia/Tunanetra]
                                        │
                                        ▼
             ┌──────────────────────────┴──────────────────────────┐
             ▼                                                     ▼
 [Ketik Tujuan & Dapatkan Rute Aman]                  [Cek Indeks Aksesibilitas Faskes]
             │                                                     │
             ▼                                                     ▼
 [Navigasi Rute & Audio Guidance]                     [Rekomendasi Jalur & Petugas Prioritas]
             │
             ▼ (Jika Menemui Hambatan Jalan)
 [Lapor Cepat via Foto + Voice Note] ──> [Tiket Terkirim ke Dashboard Publik & Dinas]
```

### 6. Kebermanfaatan Jangka Panjang & Potensi Implementasi
AksesWarga memberikan dampak keberlanjutan nyata:
* **Sosial & Ekonomi**: Mendorong kemandirian ekonomi penyandang disabilitas dan lansia untuk bekerja dan beraktivitas sehari-hari tanpa rasa takut.
* **Kebijakan Publik Berbasis Data**: Laporan *crowdsourcing* dari warga menjadi data spasial valid bagi pemerintah daerah dan Dinas PUPR/Perhubungan dalam memprioritaskan perbaikan fasilitas trotoar dan gedung umum.
* **Pondasi Indonesia Emas 2045**: Menjadi jembatan terwujudnya *Smart and Inclusive Cities* di seluruh Indonesia, di mana tidak ada satu pun warga negara yang tertinggal (*Leave No One Behind*).
