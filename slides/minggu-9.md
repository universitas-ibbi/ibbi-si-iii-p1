---
title: Bootstrap CSS Framework (Part 2) 
version: 1.0.0
theme: react
header: Bootstrap CSS Framework (Part 2)
footer: https://github.com/universitas-ibbi/ibbi-si-ii-p1
paginate: true
marp: true
---

<!-- 
_class: lead
_paginate: skip 
_footer: https://getbootstrap.com

-->
# Bootstrap CSS Framework (Part 2)

![bg contain right](./images/minggu-7-1.png)

---

## Container

Container adalah elemen dasar dalam Bootstrap yang digunakan untuk membungkus elemen-elemen lain agar tata letak menjadi lebih terorganisir. Container membantu dalam membatasi lebar konten sesuai dengan breakpoint atau kebutuhan desain.

---

# Jenis-Jenis Container:

---

## `.container`

Menggunakan lebar tetap yang berubah sesuai breakpoint.

```html
<div class="container">
    Konten dalam container dengan lebar tetap.
</div>
```

---

## `.container-fluid`

Memiliki lebar penuh (100%) di semua ukuran layar.

```html
<div class="container-fluid">
    Konten dalam container penuh.
</div>
```

---

## Grid

- Sistem grid di Bootstrap membantu dalam membuat tata letak yang fleksibel dan responsif. 
- Grid menggunakan baris (`.row`) dan kolom (`.col`) untuk membagi tata letak menjadi 12 kolom.

---

Struktur Dasar Grid:
```html
<div class="container">
    <div class="row">
        <div class="col">Kolom 1</div>
        <div class="col">Kolom 2</div>
    </div>
</div>
```

---

## Auto Layout

Kolom akan menyesuaikan ukuran otomatis.

```html
<div class="row">
    <div class="col">Auto</div>
    <div class="col">Auto</div>
</div>
```

---

## Breakpoints

Breakpoint adalah ukuran layar tertentu yang digunakan oleh Bootstrap untuk membuat desain responsif. Dengan breakpoints, tata letak dapat berubah sesuai ukuran layar.

---

Daftar Breakpoints Default:
- `xs` (Extra small): <576px
- `sm` (Small): ≥576px
- `md` (Medium): ≥768px
- `lg` (Large): ≥992px
- `xl` (Extra large): ≥1200px
- `xxl` (Extra extra large): ≥1400px

---

Penggunaan Contoh pada Kelas Grid:
```html
<div class="row">
    <div class="col-sm-6 col-lg-4">
        Kolom ini menyesuaikan ukuran layar dengan breakpoint.
    </div>
</div>
```

---

## Spesifikasi Lebar Kolom

Tentukan jumlah kolom yang diambil (1-12).

```html
<div class="row">
    <div class="col-4">4 kolom</div>
    <div class="col-8">8 kolom</div>
</div>
```

---

## Breakpoints pada Grid

Kolom akan berubah berdasarkan ukuran layar.

```html
<div class="row">
    <div class="col-sm-6 col-md-4">Responsif</div>
    <div class="col-sm-6 col-md-8">Responsif</div>
</div>
```

---

## Typography Headings

Bootstrap menyediakan gaya default untuk heading (`<h1>` hingga `<h6>`) agar terlihat konsisten.

Contoh Heading Default:
```html
<p class="h1">h1. Bootstrap heading</p>
<p class="h2">h2. Bootstrap heading</p>
<p class="h3">h3. Bootstrap heading</p>
<p class="h4">h4. Bootstrap heading</p>
<p class="h5">h5. Bootstrap heading</p>
<p class="h6">h6. Bootstrap heading</p>
```

---

## Heading dengan Subtitle

Gunakan elemen `<small>` untuk memberikan subtitle pada heading.

```html
<h1>Heading Besar <small class="text-muted">Subtitle</small></h1>
```

---

## Colors  

Bootstrap menyediakan berbagai kelas warna bawaan yang dapat digunakan untuk teks, background, border, atau elemen lainnya. Warna ini dirancang untuk aksesibilitas dan estetika yang konsisten.  

---

## Warna Dasar:

Bootstrap memiliki palet warna utama:  
- Primary: `text-primary`, `bg-primary`  
- Secondary: `text-secondary`, `bg-secondary`  
- Success: `text-success`, `bg-success`  
- Danger: `text-danger`, `bg-danger`  
- Warning: `text-warning`, `bg-warning`  
- Info: `text-info`, `bg-info`  
- Light: `text-light`, `bg-light`  
- Dark: `text-dark`, `bg-dark`  

---


Contoh Penggunaan Warna pada Teks:  
```html
<p class="text-primary">Teks dengan warna biru (primary).</p>
<p class="text-danger">Teks dengan warna merah (danger).</p>
<p class="text-success">Teks dengan warna hijau (success).</p>
```

---


Contoh Penggunaan Warna pada Background:  
```html
<div class="bg-warning text-dark p-3">Background kuning dengan teks gelap.</div>
<div class="bg-info text-white p-3">Background biru muda dengan teks putih.</div>
```

---

## Grayscale Colors:  

Bootstrap juga menyediakan kelas untuk warna abu-abu skala gradasi:  
- `text-muted`: Warna abu-abu untuk teks yang lebih redup.  
- `bg-body`: Warna background default yang netral.  
- `bg-light` dan `bg-dark`: Warna abu-abu terang dan gelap.  

---

Contoh:  
```html
<p class="text-muted">Teks ini menggunakan warna abu-abu yang lembut.</p>
<div class="bg-dark text-light p-3">Background gelap dengan teks terang.</div>
```

---

## Border Colors:  

Bootstrap mendukung warna untuk border:  

```html
<div class="border border-primary">Border biru (primary).</div>
<div class="border border-danger">Border merah (danger).</div>
<div class="border border-warning">Border kuning (warning).</div>
```

---

## Margin dan Padding  

Bootstrap menyediakan utilitas spasi untuk mengatur margin (jarak luar elemen) dan padding (jarak dalam elemen) dengan menggunakan kelas-kelas bawaan. Kelas ini menggunakan pendekatan yang konsisten untuk mengatur jarak pada elemen.

---

## Sintaks Kelas Spasi
Kelas untuk margin dan padding mengikuti pola:  

```plaintext
{property}-{sides}-{size}
```

---

- `property`:  
  - `m`: untuk margin.  
  - `p`: untuk padding.  

- `sides` (opsional):  
  - `t`: top (atas).  
  - `b`: bottom (bawah).  
  - `l`: left (kiri).  
  - `r`: right (kanan).  
  - `x`: horizontal (kiri & kanan).  
  - `y`: vertical (atas & bawah).  
  - (tanpa sisi): berlaku untuk semua sisi.  

---

- `size`:  
  - `0`: untuk jarak 0.  
  - `1`: jarak kecil (~0.25rem).  
  - `2`: jarak sedang (~0.5rem).  
  - `3`: jarak besar (~1rem).  
  - `4`: jarak ekstra besar (~1.5rem).  
  - `5`: jarak super besar (~3rem).  
  - `auto`: untuk pengaturan otomatis (hanya untuk margin).  

---

## Margin

Margin digunakan untuk memberi jarak antara elemen dengan elemen lain.  

Contoh:  
```html
<div class="m-3">Margin di semua sisi dengan ukuran 3.</div>
<div class="mt-5">Margin atas dengan ukuran 5.</div>
<div class="mx-auto">Margin horizontal otomatis (pusat).</div>
```

---

## Padding
Padding digunakan untuk memberi jarak di dalam elemen, antara konten dan batas elemen.  

Contoh:  
```html
<div class="p-3">Padding di semua sisi dengan ukuran 3.</div>
<div class="py-4">Padding vertikal (atas & bawah) dengan ukuran 4.</div>
<div class="px-2">Padding horizontal (kiri & kanan) dengan ukuran 2.</div>
```

---

## Pengaturan Kombinasi
Anda bisa menggabungkan kelas margin dan padding sesuai kebutuhan.  

Contoh:  
```html
<div class="m-3 p-4">
  Elemen ini memiliki margin 3 di semua sisi dan padding 4 di semua sisi.
</div>
```

---

## Menghapus Margin dan Padding

Gunakan `0` untuk menghapus jarak.  

Contoh:  
```html
<div class="m-0 p-0">
  Elemen ini tidak memiliki margin atau padding.
</div>
```
