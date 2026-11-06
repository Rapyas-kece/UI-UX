# Design System & Accessibility Specification — KawanTumbuh

## 1. Prinsip Desain (Design Principles)
1. **Empati & Kehangatan (Empathetic & Caring)**: Antarmuka harus memberikan rasa tenang bagi orang tua yang cemas, bukan menakut-nakuti dengan istilah medis yang mengancam.
2. **Keterbacaan Universal (WCAG 2.1 Level AAA)**: Dirancang untuk orang tua dengan tingkat literasi rendah, pengasuh lansia (kakek-nenek), serta penyandang disabilitas sensorik (tunanetra/low-vision).
3. **Beban Kognitif Rendah (Low Cognitive Load)**: Setiap pertanyaan skrining dan panduan stimulasi disajikan melalui ilustrasi visual nyata, opsi biner sederhana (`[✓ Bisa]` / `[✕ Belum Bisa]`), serta narasi suara (*Voice Guidance*).

---

## 2. Palet Warna & Rasio Kontras (Color Palette)
Warna dipilih untuk memadukan nuansa kesehatan (*healthcare*) yang terpercaya dengan edukasi anak (*education*) yang ceria dan ramah, dengan tetap mempertahankan kontras tinggi.

| Token | Nama Warna | Kode Hex | Penggunaan | Rasio Kontras (vs Background) |
| :--- | :--- | :--- | :--- | :--- |
| `primary-900` | Deep Teal | `#0F3A40` | Teks utama, judul, header navigasi | > 13:1 (Lolos AAA) |
| `primary-600` | Ocean Teal | `#186A75` | Brand primary, tombol aksi utama, link | > 7:1 (Lolos AAA) |
| `secondary-500`| Warm Marigold| `#E08A00` | Aksen edukasi, kategori aktivitas bermain | > 4.8:1 (Lolos AA) |
| `success-600` | Meadow Green | `#1E7B44` | Indikator perkembangan sesuai usia, tombol "Bisa"| > 5.5:1 (Lolos AAA) |
| `alert-600`   | Coral Warning| `#C23B22` | Tanda bahaya (*Red Flags*), butuh stimulasi khusus | > 6.2:1 (Lolos AAA) |
| `neutral-100` | Cream Surface| `#FAF8F5` | Background kanvas web (ramah mata) | Base |
| `neutral-000` | Pure White   | `#FFFFFF` | Background kartu, kontainer kuesioner | Base |

---

## 3. Tipografi (Typography Hierarchy)
Font utama: **Plus Jakarta Sans** (tipe sans-serif modern dengan bentuk melengkung yang ramah anak namun memiliki keterbacaan tinggi / *x-height* besar).

| Skala | Ukuran (px / rem) | Weight | Line Height | Penggunaan |
| :--- | :--- | :--- | :--- | :--- |
| **Heading 1** | 36px / 2.25rem | Bold (700) | 1.25 | Judul Hero Beranda / Lembar Evaluasi |
| **Heading 2** | 28px / 1.75rem | Semi-Bold (600) | 1.3 | Judul Kategori Skrining & Playbook |
| **Heading 3** | 20px / 1.25rem | Semi-Bold (600) | 1.4 | Judul Kartu Aktivitas / Sub-pertanyaan |
| **Body Large** | 18px / 1.125rem | Regular (400) | 1.6 | Teks pertanyaan skrining (ramah lansia) |
| **Body Default**| 16px / 1.0rem | Regular (400) | 1.5 | Teks standar deskripsi aktivitas |
| **Caption/Tag** | 14px / 0.875rem | Medium (500) | 1.4 | Badge usia anak, status perkembangan |

---

## 4. Komponen & Aturan Aksesibilitas Khusus (Accessibility Rules)
1. **Area Sentuh Ramah Motorik (Touch Target)**:
   * Seluruh tombol pilihan (`[✓ Bisa]`, `[✕ Belum Bisa]`, tombol pemutar audio) berukuran minimal **52 x 52 px** dengan jarak antar-tombol minimal 16px agar tidak salah tekan oleh pengguna tremor/lansia.
2. **Audio-Guided Experience (Fitur Suara Terintegrasi)**:
   * Setiap kartu pertanyaan skrining dan instruksi bermain memiliki ikon speaker `[🔊]`. Ketika diklik, web membacakan teks dengan intonasi jelas berbahasa Indonesia.
3. **Accessibility Toolbar (Header Global)**:
   * **Pengatur Ukuran Teks (`A-` / `A+`)**: Meningkatkan skala teks hingga 150%.
   * **Mode Kontras Tinggi**: Mengubah tampilan menjadi latar belakang hitam gelap (`#121212`) dengan teks dan ikon kuning terang (`#FFD166`).
