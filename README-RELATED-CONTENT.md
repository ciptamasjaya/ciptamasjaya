# Related Content Feature - Dokumentasi

## Fitur Related Content Sudah Aktif! ✅

Related content block sekarang otomatis muncul **di dalam konten artikel**, bukan di sidebar atau footer - persis seperti di WordPress!

## Cara Kerja

Related content mencari artikel terkait berdasarkan:

1. **Category** (prioritas pertama): Artikel dengan `category` yang sama
2. **Equipment** (prioritas kedua): Artikel dengan `equipment` yang sama

Maksimal menampilkan **4 artikel terkait**.

## Cara Menggunakan

### 1. Gunakan Layout "article" untuk Artikel

Pada front matter artikel, gunakan layout `article`:

```yaml
---
layout: article
title: "Judul Artikel Anda"
date: 2024-10-30
category: pesawat-angkat-angkut
equipment: overhead-crane
author: PT. Cipta Mas Jaya
description: "Deskripsi artikel"
---
```

### 2. Set Category dan Equipment yang Tepat

**Category**: Kategori layanan utama
- `pesawat-angkat-angkut`
- `pesawat-uap-bejana-tekan`
- `instalasi-listrik-penyalur-petir`
- `instalasi-pemadam-kebakaran`
- `elevator-eskalator`
- `pesawat-tenaga-produksi`

**Equipment**: Jenis peralatan spesifik
- `overhead-crane`
- `gantry-crane`
- `hoist`
- `boiler`
- `pressure-vessel`
- dll.

### 3. Related Content Otomatis Muncul

Related content block akan muncul di **akhir artikel** (sebelum footer) dengan:
- Judul artikel terkait (clickable link)
- Deskripsi artikel
- Tanggal publikasi
- Styling menarik dengan gradient background

## Styling

Related content menggunakan:
- **Background**: Gradient purple-blue yang eye-catching
- **Responsive**: Otomatis adjust untuk mobile
- **Hover effect**: Card terangkat saat di-hover
- **Grid layout**: Rapi dan terorganisir

## Contoh

Artikel "Overview Overhead Crane" menampilkan "Riksa Uji Crane" sebagai related content karena:
- Sama-sama category: `pesawat-angkat-angkut`
- Sama-sama equipment: `overhead-crane`

## Tips

1. **Gunakan category konsisten**: Pastikan artikel dalam satu topik menggunakan category yang sama
2. **Set equipment spesifik**: Equipment yang lebih spesifik membuat related content lebih relevan
3. **Tulis description**: Description ditampilkan di related content card
4. **Set date**: Tanggal publikasi ditampilkan untuk memberikan konteks

## File yang Terlibat

- `_layouts/article.html`: Layout artikel dengan related content
- `_includes/related-content.html`: Component related content
- Front matter artikel: `category` dan `equipment`

## Refresh Browser

Setelah rebuild, refresh browser di:
http://ciptamasjaya-githubpages.local/pesawat-angkat-angkut/overhead-crane/overview-overhead-crane.html

Scroll ke bawah untuk melihat related content block!
