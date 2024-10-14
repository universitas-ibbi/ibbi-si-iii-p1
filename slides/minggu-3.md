---
title: Pendahuluan CSS
version: 1.0.0
theme: react
header: Front-end Development for Web Design (Minggu 3)
footer: https://github.com/universitas-ibbi/ibbi-si-ii-p1
paginate: true
marp: true
---

<!-- _class: lead
_paginate: skip -->

# Pendahuluan CSS

--- 

## Apa itu CSS

CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mendesain tampilan halaman web. Dengan CSS, kita bisa mengontrol tata letak, warna, ukuran teks, margin, padding, dan elemen visual lainnya pada halaman web.

```css
<style>
   body {
      background-color: lightblue;
   }
</style>
```

---

## Contoh Perintah CSS

Berikut contoh perintah CSS yang mengubah warna teks menjadi merah:

```css
p {
   color: red;
}
```

---

## Syntax CSS
Syntax dasar CSS terdiri dari selector (misalnya elemen HTML yang akan diatur), diikuti oleh blok deklarasi yang diapit oleh kurung kurawal {}. Di dalamnya ada properti dan nilainya:

```css
selector {
   property: value;
}
```
Contoh : 
```css
h1 {
   color: blue;
   font-size: 20px;
}
```

---

## How to Insert CSS

Ada tiga cara untuk memasukkan CSS:

- Inline CSS: Langsung di dalam tag HTML.
- Internal CSS: Di dalam elemen `<style>` di dalam tag `<head>`.
- External CSS: Di dalam file CSS terpisah yang di-link dari HTML.

---

## Inline CSS

CSS ini langsung ditulis pada atribut elemen HTML. 

```css
<h1 style="color: blue;">Hello World</h1>
```

---

## Internal CSS

Ditulis di dalam elemen `<style>` pada bagian `<head>` dokumen HTML. 

```css
<style>
   body {
      background-color: lightgreen;
   }
</style>
```

---

## External CSS

CSS ditulis dalam file .css terpisah dan dihubungkan ke file HTML dengan tag `<link>`. 

```css
<link rel="stylesheet" href="styles.css">
```

---

## Multiple Style Sheets

File CSS berbeda bisa digunakan bersamaan. Jika ada konflik aturan, CSS dengan prioritas lebih tinggi akan diterapkan sesuai dengan urutan atau aturan cascading.

---

## Cascading Order

CSS menerapkan aturan dari beberapa sumber (inline, internal, external) berdasarkan prioritas. Urutan prioritasnya:

- Inline CSS
- Internal CSS
- External CSS

---

## CSS Selector

Selector digunakan untuk memilih elemen HTML yang ingin diatur.

```css
h1 {
   color: green;
}
```

---

## CSS Element Selector

Selector yang memilih elemen berdasarkan nama tag HTML. 

```css
p {
   color: blue;
}
```

---

## CSS ID Selector

Selector yang memilih elemen berdasarkan ID yang unik untuk setiap elemen.

```css
#header {
   background-color: yellow;
}
```

---

## CSS Class Selector

Selector yang memilih elemen berdasarkan kelas yang dapat digunakan oleh banyak elemen.

```css
.important {
   font-weight: bold;
}
```

---

## CSS Universal Selector

Selector yang memilih semua elemen pada halaman.

```css
* {
   margin: 0;
   padding: 0;
}
```

---

##  CSS Grouping Selector

Selector yang mengelompokkan beberapa elemen untuk diberi gaya yang sama.

```css
h1, h2, h3 {
   color: red;
}
```

---

## CSS Unit

Satuan yang digunakan dalam CSS untuk mengatur ukuran elemen, seperti px, em, rem, vw, dan

```css
p {
   font-size: 16px;
}
```

---

## CSS Combinators

Digunakan untuk mengkombinasikan selector. Ada beberapa kombinator seperti descendant ( ), child (>), sibling (~), dan adjacent (+).

---

## Descendent Selector

Memilih semua elemen di dalam elemen lainnya. 

```css
div p {
   color: blue;
}
```

---

##  Child Selector

Memilih elemen yang merupakan anak langsung dari elemen tertentu. 

```css
div > p {
   color: orange;
}
```

---

## CSS Box Model

Setiap elemen di HTML dianggap sebagai sebuah kotak, dan box model ini menjelaskan elemen dengan margin, border, padding, dan konten.

```css
div {
   margin: 20px;
   padding: 10px;
   border: 2px solid black;
}
```

---

## CSS Margin

Menentukan jarak di luar border elemen. 

```
p {
   margin: 10px;
}
```

---

## CSS Padding

Menentukan jarak di dalam border antara konten dan border elemen. 

```css
div {
   padding: 15px;
}
```

---

## CSS Height and Width

Menentukan tinggi dan lebar elemen. 

```css
div {
   height: 200px;
   width: 300px;
}
```

---

## CSS Border

Menentukan garis di sekitar elemen. 

```css
p {
   border: 1px solid black;
}
```

---

## CSS Color 

Menentukan warna teks elemen. 

```css
h1 {
   color: green;
}
```

---

##  CSS Background

Mengatur latar belakang elemen. 

```css
body {
   background-color: lightgray;
}
```

---

## CSS Text

Mengatur teks elemen seperti warna, ukuran, perataan, dan dekorasi. 

```css
p {
   text-align: center;
   text-decoration: underline;
}
```

---

## CSS Fonts

Mengatur jenis font, ukuran, dan gaya. 

```css
p {
   font-family: Arial, sans-serif;
   font-size: 14px;
}
```

---

## CSS Display

Mengontrol tampilan elemen, seperti block, inline, none.

```css
div {
   display: none;
}
```

---

## CSS Attribute Selector

Memilih elemen berdasarkan atribut tertentu.

```css
input[type="text"] {
   background-color: lightblue;
}
```