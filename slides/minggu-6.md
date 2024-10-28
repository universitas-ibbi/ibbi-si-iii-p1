---
title: Git, GitHub dan Github Pages
version: 1.0.0
theme: react
header: Front-end Development for Web Design (Minggu 6)
footer: https://github.com/universitas-ibbi/ibbi-si-ii-p1
paginate: true
marp: true
---

<!-- _class: lead
_paginate: skip -->

# Git, GitHub dan Github Pages

---

### **Apa itu Git?**

Git adalah sistem kontrol versi terdistribusi yang memungkinkan pengembang untuk melacak perubahan dalam proyek mereka, berkolaborasi dengan orang lain, dan mengelola riwayat proyek.

---

### **Mengapa menggunakan Git?**

Git memungkinkan tim untuk bekerja secara bersamaan tanpa saling mengganggu, memudahkan rollback ke versi sebelumnya, dan menyediakan alat untuk mengelola konflik perubahan.

---

## **Konsep Dasar Git:**

---

### **Repository:** 

Tempat menyimpan semua file dan riwayat perubahan proyek.

---

### **Commit:**

Merekam perubahan yang telah dilakukan. Setiap commit memiliki ID unik dan pesan yang menjelaskan perubahan.

---

## **Instalasi Git**

---

### **Cara menginstal Git:**
- **Windows:** Unduh installer dari [git-scm.com](https://git-scm.com) dan ikuti petunjuk instalasi.
- **macOS:** Gunakan Homebrew dengan perintah `brew install git`.
- **Linux:** Gunakan manajer paket seperti `apt` atau `yum`, misalnya:

```bash
sudo apt install git
```

---

### **Konfigurasi Git:**

Setelah instalasi, atur nama pengguna dan email dengan perintah berikut:

```bash

git config --global user.name "Nama Kamu"

git config --global user.email "email@domain.com"

```

---

## **Dasar-dasar Perintah Git**

---

### **Inisialisasi Repository:**

Membuat repositori baru:

```bash

git init [nama-repo]

```

---

### **Menambahkan File:**

Menambahkan file baru ke staging area:

```bash

git add index.html

```

---

### **Menyimpan Perubahan:**

Merekam perubahan ke dalam repository:

```bash

git commit -m "Menambahkan file index.html"

```

---


### **Melihat Status:**

Mengecek status repositori:

```bash

git status

```

---

### **Melihat Riwayat Commit:**

Melihat riwayat commit:

```bash

git log

```

---

### **Menghapus File:**

Menghapus file dari repositori:

```bash

git rm index.html

```

---

## **Pengantar GitHub**

---

### **Apa itu GitHub?**

GitHub adalah platform berbasis web yang memungkinkan pengembang untuk meng-host repositori Git secara online dan berkolaborasi dengan tim.

---

### **Fitur Utama GitHub:**

GitHub menawarkan berbagai fitur seperti repository, issues untuk melacak bug, dan pull requests untuk mengusulkan perubahan.

---

### **Perbedaan antara Git dan GitHub:**

Git adalah alat kontrol versi lokal, sedangkan GitHub adalah layanan online yang menyediakan penyimpanan repositori Git dan kolaborasi.

---

## **Membuat dan Mengelola Repository di GitHub**

---

### **Membuat Repository Baru:**

Masuk ke GitHub, klik tombol "New" di halaman repositori, lalu isi nama dan deskripsi repositori.

---

### **Menghubungkan Repository Lokal dengan GitHub:**

Pertama, buat repositori di GitHub, lalu hubungkan dengan repositori lokal:

```bash

git remote add origin https://github.com/username/nama-repo.git

git push -u origin main

```

---

### **Menarik Perubahan dari GitHub:**

Untuk menarik perubahan dari repositori GitHub:

```bash

git pull origin main

```
---

### **Apa itu GitHub Pages?**

Layanan GitHub untuk menghosting halaman web statis dari repositori Git.

---

### **Membuat Halaman GitHub Pages:**

Kamu dapat membuat branch `gh-pages` dan menambahkan file HTML untuk membuat halaman:

```bash

git checkout -b gh-pages

git add index.html

git commit -m "Menambahkan halaman GitHub Pages"

git push origin gh-pages

```

---

### **Menambahkan Konten ke Halaman GitHub Pages:**

Kamu bisa menggunakan HTML, CSS, dan JavaScript untuk mengembangkan halaman web.

