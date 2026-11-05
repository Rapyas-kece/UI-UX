# Design System & Accessibility Specification — AksesWarga

## 1. Prinsip Desain (Design Principles)
1. **Inklusivitas Radikal (Radical Inclusivity)**: Dirancang untuk pengguna kursi roda, tunanetra, gangguan motorik, lansia, dan warga dengan literasi digital rendah. Mematuhi standar **WCAG 2.1 Level AAA**.
2. **Kejelasan Tanpa Beban Kognitif (Cognitive Ease)**: Antarmuka berbasis kartu visual, ikon yang familiar, label teks eksplisit, dan tanpa jargon teknis yang membingungkan.
3. **Kesiapan Multimodal (Multimodal Interaction)**: Setiap aksi utama dapat dilakukan melalui visual, navigasi keyboard (Tab + Enter), serta asisten suara (*Voice Input & Screen Reader*).

---

## 2. Palet Warna & Rasio Kontras (Color Palette)
Warna dipilih dengan kontras tinggi untuk memastikan keterbacaan oleh pengguna dengan *low vision* maupun di bawah terik sinar matahari (*outdoor visibility*).

| Token | Nama Warna | Kode Hex | Penggunaan | Rasio Kontras (vs Background) |
| :--- | :--- | :--- | :--- | :--- |
| `primary-900` | Deep Navy | `#0B2545` | Teks utama, judul, header navigasi | > 12:1 (Lolos AAA) |
| `primary-600` | Royal Blue | `#134074` | Brand primary, status aktif, link | > 7:1 (Lolos AAA) |
| `accent-500` | Safety Amber | `#E07A5F` | Aksen aksi penting, peringatan trotoar | > 4.5:1 (Lolos AA) |
| `success-600` | Emerald Safe | `#1B7A43` | Rute ramah, fasilitas terverifikasi aksesibel | > 5:1 (Lolos AAA) |
| `danger-600` | Signal Red | `#C1121F` | Hambatan jalan kritis, tangga curam, trotoar putus | > 6:1 (Lolos AAA) |
| `neutral-100` | Soft Surface | `#F8F9FA` | Background kanvas web | Base |
| `neutral-000` | Pure White | `#FFFFFF` | Background kartu, kontainer pop-up | Base |

---

## 3. Tipografi (Typography Hierarchy)
Font utama: **Plus Jakarta Sans** atau **Inter** (tipe sans-serif modern dengan keterbacaan tinggi / *x-height* besar).

| Skala | Ukuran (px / rem) | Weight | Line Height | Penggunaan |
| :--- | :--- | :--- | :--- | :--- |
| **Heading 1** | 36px / 2.25rem | Bold (700) | 1.2 | Judul Halaman Utama / Hero Title |
| **Heading 2** | 28px / 1.75rem | Semi-Bold (600) | 1.3 | Judul Bagian / Nama Fasilitas |
| **Heading 3** | 20px / 1.25rem | Semi-Bold (600) | 1.4 | Judul Kartu Rute / Sub-bagian |
| **Body Large** | 18px / 1.125rem | Regular (400) | 1.6 | Teks utama (Default ramah lansia) |
| **Body Default**| 16px / 1.0rem | Regular (400) | 1.5 | Teks standar deskripsi |
| **Caption/Tag** | 14px / 0.875rem | Medium (500) | 1.4 | Label status aksesibilitas, badge |

---

## 4. Komponen & Aturan Aksesibilitas Khusus (Accessibility Rules)
1. **Target Sentuh Minimum (Touch Target Size)**:
   * Seluruh tombol utama, input pencarian, dan ikon aksi memiliki ukuran area klik **minimum 48 x 48 px** dengan *padding* longgar untuk pengguna dengan tremor tangan atau lansia.
2. **Fokus State Terlihat (Visible Focus Indicator)**:
   * Garis batas luar (*outline focus*) berukuran 3px berwarna kontras (`#134074`) saat berpindah menggunakan tombol `Tab`.
3. **Accessibility Toolbar (Fitur Khusus UI Switcher)**:
   * **Tombol Cepat di Header**:
     - *Perbesar Teks (A- / A+)*: Mengubah ukuran teks dasar dari 16px ke 20px / 24px.
     - *Mode Kontras Tinggi*: Mengubah tema menjadi latar hitam pekat teks kuning terang `#FFFF00` (High Contrast Mode).
     - *Mode Suara*: Mengaktifkan pembacaan teks otomatis saat elemen disentuh/diklik.
