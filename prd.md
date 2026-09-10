# Product Requirement Document (PRD) — Standar Pembuatan & Publikasi Artikel Website Kontraktor Bangunan

## 1. Ikhtisar Dokumen (Overview)
Dokumen ini berfungsi sebagai panduan standar operasional dan spesifikasi teknis (PRD) dalam proses produksi, pemformatan konten, optimasi media gambar, penanaman internal link, dan publikasi artikel blog baru pada website **Kontraktor Bangunan Surabaya** (`kontraktorbangunansurabaya.web.id`). Panduan ini wajib dipatuhi untuk memastikan seluruh artikel memiliki standar SEO, AEO/GEO, performa teknis, dan keterhubungan internal link yang sempurna tanpa broken links.

---

## 2. Struktur & Penamaan File (File & URL Conventions)

### 2.1. Penamaan File HTML
- Setiap artikel baru dibuatkan file `.html` mandiri di dalam direktori `artikel/`.
- Nama file wajib mengikuti judul artikel dengan format *slug/kebab-case* (huruf kecil semua dipisahkan tanda hubung `-`) untuk menjamin URL yang rapi dan SEO-friendly.
- **Contoh**:
  - Judul: `Estimasi Biaya Renovasi Rumah di Surabaya - Panduan Lengkap & Hitungan RAB`
  - File: `artikel/estimasi-biaya-renovasi-rumah-surabaya.html`

### 2.2. Metadata, Canonical, & Schema Markup
- Wajib menyertakan tag `<title>`, `<meta name="description">`, `<meta name="keywords">`, `<meta name="robots">`.
- Tag `<link rel="canonical">`, Open Graph (`og:url`, `og:image`), serta Twitter Cards harus merujuk ke URL file dan gambar yang tepat.
- Menyertakan structured data Schema JSON-LD lengkap (*TechArticle* / *Article*, *BreadcrumbList*, dan *FAQPage*).
- Menyertakan GEO Meta Tags wilayah Surabaya & Jawa Timur (`geo.region: ID-JI`, `geo.placename: Kota Surabaya, Jawa Timur`, `geo.position: -7.2575;112.7521`).

---

## 3. Spesifikasi & Optimasi Gambar Artikel (Featured Image)

| Kriteria | Ketentuan Standar |
| :--- | :--- |
| **Format File** | `.webp` *(Wajib format WebP modern)* |
| **Ukuran Maksimal** | **Maksimal 50 KB** (terkompresi optimal, tetap tajam dan cepat dimuat) |
| **Rasio & Dimensi** | Rasio `16:9` (Standar: `800 x 450 px` hingga `1200 x 675 px`) |
| **Watermark** | Wajib memiliki watermark teks **`kontraktorbangunansurabaya.web.id`** di posisi **Tengah (Center)** gambar dengan opasitas proporsional |
| **Lokasi Penyimpanan** | `assets/img/artikel/[nama-gambar].webp` |
| **Alt Text** | Wajib deskriptif dan mengandung kata kunci utama artikel |

---

## 4. Standar Penulis & Entitas Brand (Brand & Author Standardization)

- **Identitas Penulis Resmi**:
  - **Nama Penulis**: `Tim Teknik Sipil & Arsitektur Kontraktor Bangunan Surabaya`
  - **Bio Penulis**: *Divisi Perencanaan & Pelaksanaan Konstruksi Bangunan. Berfokus pada perhitungan volume material presisi, mutu beton SNI K-300, penyusunan RAB transparan, dan pendampingan proyek di area Surabaya dan Jawa Timur.*
- **Standar Penamaan Brand**:
  - Seluruh artikel, metadata, schema markup, dan CTA **DILARANG** menggunakan sebutan badan usaha seperti **`PT.`** atau nama PT lainnya.
  - Nama Brand Resmi: **`Kontraktor Bangunan Surabaya`** / **`Kontraktor Bangunan`** (website: `kontraktorbangunansurabaya.web.id`).
- **Nomor WhatsApp & CTA Resmi**: Menggunakan link WhatsApp resmi `https://wa.me/6288989643555` dengan teks pesan konsultasi otomatis.

---

## 5. Standar AEO, GEO, dan Local SEO

### 5.1. Strategi Answer Engine Optimization (AEO)
- **Direct Answer Format**: Setiap heading `<h2>` berbentuk pertanyaan wajib diikuti oleh **1–2 kalimat jawaban ringkas, tegas, dan berbobot (direct answer)** di awal paragraf sebelum pembahasan teknis mendalam. Format ini memudahkan mesin AI (Google AI Overviews, Perplexity, dsb.) mengambil kutipan instan.

### 5.2. Strategi Generative Engine Optimization (GEO) & Local Context
- Menyebutkan entitas wilayah target secara alami di dalam konten (Kota Surabaya, Surabaya Barat/Timur/Selatan/Utara, Sidoarjo, Gresik, Malang, Jawa Timur) serta faktor aksesibilitas (gang pemukiman padat vs jalan utama).
- Mengintegrasikan standar mutu konstruksi nasional (SNI, izin PBG via SIMBG PUPR, mutu beton K-300, uji slump cone).

---

## 6. Struktur Konten & Navigasi Internal (Content Structure & SEO On-Page)

### 6.1. Format Judul Subheading (Berbentuk Pertanyaan)
- Seluruh tag `<h2>` diformat dalam bentuk kalimat tanya informatif yang sering dicari pengguna (misal: *"1. Berapa Kisaran Biaya Renovasi Rumah per Meter Persegi di Surabaya?"*, *"2. Apa Saja Komponen Penentu Anggaran Konstruksi Proyek?"*).

### 6.2. Daftar Isi (Table of Contents / TOC Collapsible)
- Setiap artikel wajib memiliki blok **Daftar Isi Buka-Tutup (Collapsible)** dengan tombol chevron interaktif (`data-bs-toggle="collapse"` target `#tocCollapse`).
- Setiap butir link terhubung melalui anchor `#id-heading` ke masing-masing subjudul section artikel.

### 6.3. Tabel Data & Transparansi Biaya
- **Minimal 1 Tabel Data per Artikel**: Wajib menyertakan minimal 1 tabel data responsif (`.article-table`) yang memuat rincian estimasi biaya per m², komparasi spesifikasi material, atau breakdown tahapan pekerjaan.

### 6.4. Strategi Internal Linking Alami (Wajib Valid & Relevan)
Setiap artikel wajib memuat dua jenis tautan internal:

1. **Contextual Internal Links (Tautan Alami di Dalam Paragraf)**:
   - Menghubungkan kata kunci kontekstual secara mengalir dan natural di dalam teks paragraf.
   - **Target Link Wajib Ada Halamannya (Dilarang Broken Link / 404)**:
     - **Layanan:** `../layanan/bangun-rumah-baru.html`, `../layanan/renovasi-bangunan.html`, `../layanan/gedung-&-komersial.html`, `../layanan/desain-arsitektur-&-RAB.html`, `../layanan/interior-&-finishing.html`, `../layanan/maintenance-bangunan.html`.
     - **Halaman Utama:** `../index.html`, `../portofolio.html`, `../tentang-kami.html`, `../kontak.html`, `../artikel.html`.
     - **Artikel Terkait:** `cara-menilai-kualitas-beton-k-300.html`, `cara-menilai-kualitas-beton-k-300-dak-rumah.html`, `strategi-menyusun-rab-bangunan.html`, `panduan-mengurus-izin-pbg-bangunan.html`, `panduan-memilih-kontraktor-rumah-surabaya.html`, `panduan-lengkap-bangun-rumah-baru-malang.html`.
   - **Anchor Text**: Harus bervariasi, natural, dan kontekstual (tidak kaku atau monoton).
   - **Styling Tautan**: Wajib **Huruf Tebal (Bold)** dan **Tanpa Garis Bawah (No Underline)** agar tampilan tetap bersih dan elegan (menggunakan kelas Bootstrap: `.fw-bold .text-decoration-none .text-navy .hover-yellow`).

2. **Inline Box "Baca Juga"**:
   - Menyisipkan box rujukan artikel (`.baca-juga-box`) di antara section paragraf untuk meningkatkan keterlibatan pembaca.

### 6.5. Section FAQ Interaktif & Banner CTA Penutup
- Accordion FAQ interaktif di akhir artikel yang mencakup 3–4 pertanyaan umum.
- Banner penutup CTA konsultasi WhatsApp dan survei lokasi gratis.

---

## 7. Prosedur Integrasi & Publikasi (Langkah Wajib Setiap Upload)

Setelah file `artikel/<slug>.html` dan gambar WebP dibuat, jalankan 2 langkah integrasi ini agar artikel langsung tampil di blog dan terindeks:

### Step 1: Daftarkan ke `assets/js/main.js` (Array `dataArtikel`)
Tambahkan objek artikel baru di urutan **paling atas (indeks 0)** pada array `dataArtikel` di [assets/js/main.js](file:///e:/Magang/boostrap/kontaktor-bangunan/assets/js/main.js):
```javascript
{
    judul: "Judul Lengkap Artikel Hari Ini",
    kategori: "manajemen", // Pilihan kategori: "bangun-rumah" | "sipil-dasar" | "manajemen" | "legalitas"
    kategoriLabel: "Manajemen Biaya", // Label: "Bangun Rumah" | "Sipil Dasar" | "Manajemen Biaya" | "Legalitas & Izin"
    tanggal: "8 Sep 2026",
    waktuBaca: "8 Menit",
    url: "artikel/nama-file-artikel.html",
    gambar: "assets/img/artikel/nama-file-gambar.webp",
    ringkasan: "Ringkasan padat 1-2 kalimat untuk preview kartu artikel di blog artikel.html..."
},
```

### Step 2: Daftarkan ke `sitemap.xml`
Tambahkan blok `<url>` baru di bagian *Detail Artikel Teknis* pada [sitemap.xml](file:///e:/Magang/boostrap/kontaktor-bangunan/sitemap.xml):
```xml
<url>
  <loc>https://kontraktorbangunansurabaya.web.id/artikel/nama-file-artikel</loc>
  <lastmod>2026-09-08</lastmod>
  <changefreq>monthly</changefreq>
  <priority>0.85</priority>
  <image:image>
    <image:loc>https://kontraktorbangunansurabaya.web.id/assets/img/artikel/nama-file-gambar.webp</image:loc>
    <image:title>Judul Lengkap Artikel</image:title>
    <image:caption>Deskripsi ringkas gambar artikel</image:caption>
  </image:image>
</url>
```

---

## 8. Checklist Publikasi QA

Sebelum artikel dinyatakan selesai, pastikan seluruh checklist berikut terpenuhi:

- [ ] **File HTML Dibuat:** Tersimpan di folder `artikel/<slug-judul>.html` dengan format relative path (`../`) yang valid.
- [ ] **Featured Image Sesuai:** Format `.webp`, ber-watermark `kontraktorbangunansurabaya.web.id` di **Center**, ukuran **≤ 50 KB**.
- [ ] **Brand Resmi:** Menggunakan nama **Kontraktor Bangunan Surabaya** tanpa penyebutan `PT.`.
- [ ] **Subheading Pertanyaan (H2):** Diformat dalam bentuk kalimat tanya informatif dengan *direct answer* di paragraf awal.
- [ ] **Daftar Isi (TOC Collapsible):** Berfungsi buka-tutup dan anchor link menuju section terkait aktif.
- [ ] **Tabel Data:** Memuat minimal 1 tabel estimasi/spesifikasi biaya.
- [ ] **Internal Linking Kontekstual:** Link tertanam alami di dalam paragraf isi (format **huruf tebal tanpa garis bawah**), aktif me-redirect, dan seluruh URL target benar-benar ada/valid.
- [ ] **Box "Baca Juga":** Terpasang rapi di sela-sela konten.
- [ ] **FAQ Accordion & CTA WA:** Berfungsi interaktif dan nomor WA valid.
- [ ] **Listing Blog Aktif:** Terdaftar di urutan teratas `dataArtikel` [assets/js/main.js](file:///e:/Magang/boostrap/kontaktor-bangunan/assets/js/main.js) dan tampil di [artikel.html](file:///e:/Magang/boostrap/kontaktor-bangunan/artikel.html).
- [ ] **Sitemap Terupdate:** Entri URL dan gambar artikel sudah ditambahkan ke [sitemap.xml](file:///e:/Magang/boostrap/kontaktor-bangunan/sitemap.xml).


nih artikel ke 3 day 4 kita. buatkan file nya sesuai nama judul, gambar harus baru, menarik, dan diminati dan tidak boleh ngambil dari gambar di halaman lain dan harus berformat .webp berwatermark dan terkompres max 50kb, lalu harus sudah tampil di blog nya

jangan lupa link internalnya minimal 2, dan juga artikelnya harus relevan dengan judulnya jangan meleset