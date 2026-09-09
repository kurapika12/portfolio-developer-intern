# M. Aslam Hidayat - Developer Portfolio

## About
Hi, saya M. Aslam Hidayat! Saya seorang Developer dengan pengalaman membangun aplikasi web full-stack menggunakan **Laravel**, serta aplikasi mobile menggunakan **Flutter**. Saya terbiasa merancang database, membuat REST API (CRUD, validasi dasar), melakukan integrasi API pada aplikasi mobile (fetch data, submit data, handle error), serta bekerja menggunakan Git & GitHub (branching, commit, pull request).

Repository ini dibuat sebagai portofolio untuk mendukung lamaran **Developer Intern (Laravel + React Native) di Fun Teacher Private**, sekaligus menampilkan skill dan progres saya di bidang Software Development.

**Ketertarikan:** Web + mobile development, REST API, dan pembelajaran praktik industri melalui bimbingan developer senior (mentoring & code review).

> Catatan: pengalaman mobile saya saat ini menggunakan Flutter, dengan pemahaman konsep yang serupa dengan React Native (state management, integrasi API, komponen UI). Saya siap dan cepat beradaptasi untuk mengembangkan project menggunakan React Native.

## Table of Contents
- [About](#about)
- [Portfolio Projects](#portfolio-projects)
  - [MiniCommerce - Laravel E-Commerce](#minicommerce---laravel-e-commerce)
  - [Inventory Management System - Laravel](#inventory-management-system---laravel)
  - [Finance Tracker - Flutter App](#finance-tracker---flutter-app)
  - [Todo & Notes App - Flutter](#todo--notes-app---flutter)
  - [Kelurahan Bawasalo - Website Profil Desa](#kelurahan-bawasalo---website-profil-desa)
  - [Aplikasi Web Absensi - QR Code](#aplikasi-web-absensi---qr-code)
  - [Server Dashboard - React & FastAPI](#server-dashboard---react--fastapi)
  - [MRT Schedules - REST API](#mrt-schedules---rest-api)
  - [Stegano Tool - Python GUI](#stegano-tool---python-gui)
  - [WiFi Password Generator](#wifi-password-generator)
- [Tools & Skills](#tools--skills)
- [Contact](#contact)

## Portfolio Projects

### MiniCommerce - Laravel E-Commerce

**Role:** Full-Stack Developer (Portfolio Project)

**Tools:** Laravel, Tailwind CSS v4 (via `@tailwindcss/vite`), Vite, Blade, Xendit Payment Gateway (Sandbox)

**Goal:** Membangun aplikasi web e-commerce sederhana yang memungkinkan pengguna membeli produk dan mensimulasikan alur pembayaran menggunakan payment gateway.

**Description:** MiniCommerce adalah aplikasi web e-commerce yang memungkinkan pengguna melakukan pembelian produk sederhana menggunakan Xendit Payment Gateway (Sandbox). Aplikasi ini mensimulasikan alur pembayaran yang digunakan pada sistem e-commerce nyata. UI Blade didesain ulang pada lima halaman utama (katalog, detail produk, tambah produk, riwayat pesanan, dan detail pesanan) menggunakan palet warna indigo/slate/emerald, hover effect, sticky navbar, dan status badge.

**Skills:** Backend development dengan Laravel, integrasi payment gateway, UI/UX design dengan Tailwind, build tooling dengan Vite.

**Repository:** [`minicommerce`](https://github.com/kurapika12/minicommerce)

---

### Inventory Management System - Laravel

**Role:** Backend Developer (Portfolio Project)

**Tools:** Laravel, MySQL, Blade, Chart.js

**Goal:** Membangun sistem manajemen inventaris untuk pencatatan stok barang masuk dan keluar dengan validasi otomatis dan dashboard statistik interaktif.

**Description:** Sistem manajemen inventaris berbasis Laravel dengan operasi CRUD untuk barang, kategori, dan supplier. Dilengkapi pencatatan stok masuk-keluar dengan validasi otomatis, dashboard statistik interaktif menggunakan Chart.js, serta role-based access control untuk membedakan hak akses admin dan staff.

**Skills:** Database design (MySQL), role-based access control, data visualization dengan Chart.js, CRUD application development.

**Repository:** [`inventory-management-system`](https://github.com/kurapika12/inventory-management-system)

---

### Finance Tracker - Flutter App

**Role:** Mobile Developer (Portfolio Project)

**Tools:** Flutter, Isar (local database), Riverpod, Google Apps Script, http package, connectivity_plus

**Goal:** Membangun aplikasi pencatatan keuangan pribadi yang tetap dapat digunakan tanpa koneksi internet (offline-first) dengan sinkronisasi otomatis ke Google Spreadsheet untuk backup dan analisis data.

**Description:** Aplikasi ini menggunakan Isar sebagai local database (source of truth) dan Google Apps Script sebagai backend untuk sinkronisasi data ke Google Spreadsheet. Arsitektur aplikasi dirancang agar setiap transaksi selalu tersimpan ke database lokal terlebih dahulu; jika perangkat online maka data langsung dikirim ke Spreadsheet, dan jika offline maka data ditandai pending untuk disinkronkan otomatis saat koneksi kembali tersedia. Setiap transaksi menggunakan UUID sebagai primary key untuk menghindari duplikasi data saat proses sinkronisasi.

**Skills:** State management (Riverpod), local database design, offline-first architecture, API integration, sync mechanism design.

**Key Features:**
- Tambah, edit, dan hapus transaksi (income/expense)
- Riwayat transaksi dan ringkasan saldo
- Kategori transaksi
- Sinkronisasi otomatis ke Google Sheets dengan retry otomatis saat sinkronisasi gagal
- Status sinkronisasi per transaksi

**Repository:** [`finance-tracker-offline-first`](https://github.com/kurapika12/finance-tracker-offline-first)
---

### Todo & Notes App - Flutter

**Role:** Mobile Developer (Portfolio Project)

**Tools:** Flutter, Provider, sqflite, Google Fonts (Poppins), flutter_slidable, uuid, intl

**Goal:** Membangun aplikasi produktivitas yang menggabungkan fitur to-do list dan catatan dalam satu aplikasi dengan tema clean black & white.

**Description:** Aplikasi ini menggabungkan fungsi todo list dan catatan dalam satu aplikasi dual-function dengan dukungan dark/light mode. Fitur pencarian real-time, label warna untuk kategori catatan (dengan migrasi skema SQLite), tema monokrom hitam-putih, bottom sheet editor dengan drag handle, dialog konfirmasi hapus melalui reusable helper, serta timestamp yang tersimpan otomatis.

**Skills:** State management dengan Provider, local database (SQLite) dengan migrasi skema, UI/UX theming, penanganan bug keyboard-overlap dan API yang deprecated.

**Repository:** [`todo_notes_app_with_flutter`](https://github.com/kurapika12/todo_notes_app_with_flutter)

---

### Kelurahan Bawasalo - Website Profil Desa

**Role:** Web Developer (Portfolio Project)

**Tools:** HTML

**Goal:** Membangun website profil kelurahan yang menampilkan informasi publik secara modern dan mudah diakses masyarakat.

**Description:** Website profil Kelurahan Bawasalo yang menampilkan informasi profil, layanan publik, potensi daerah, UMKM, berita, dan kontak dalam tampilan modern, responsif, dan mudah digunakan oleh masyarakat umum.

**Skills:** Web development, responsive design, information architecture.

**Repository:** [`Kelurahan-Bawasalo`](https://github.com/kurapika12/Kelurahan-Bawasalo)

---

### Aplikasi Web Absensi - QR Code

**Role:** Full-Stack Developer (Portfolio Project)

**Tools:** Python (Flask), MySQL

**Goal:** Membangun sistem absensi sederhana berbasis QR Code untuk memudahkan manajemen data siswa dan pencatatan kehadiran.

**Description:** Aplikasi web absensi berbasis QR Code yang dibangun menggunakan Python Flask untuk backend dan MySQL sebagai database, dirancang untuk memudahkan manajemen data siswa dan pencatatan kehadiran secara efisien.

**Skills:** Backend development dengan Flask, integrasi QR Code, database design dengan MySQL.

**Repository:** [`Aplikasi-web-absensi`](https://github.com/kurapika12/Aplikasi-web-absensi)

---

### Server Dashboard - React & FastAPI

**Role:** Full-Stack Developer (Portfolio Project)

**Tools:** Python (FastAPI), React

**Goal:** Membangun dashboard monitoring server secara real-time untuk memantau kondisi CPU, RAM, storage, dan uptime.

**Description:** Dashboard monitoring server modern berbasis React dan FastAPI yang memantau CPU, RAM, storage, uptime, dan informasi sistem lainnya secara real-time melalui antarmuka web yang bersih dan responsif.

**Skills:** REST API development dengan FastAPI, real-time data monitoring, frontend development dengan React.

**Repository:** [`server-dashboard`](https://github.com/kurapika12/server-dashboard)

---

### MRT Schedules - REST API

**Role:** Backend Developer (Portfolio Project)

**Tools:** Go (Golang)

**Goal:** Menyediakan REST API sederhana untuk informasi jadwal dan stasiun MRT Jakarta.

**Description:** mrt-schedules adalah REST API sederhana berbasis Golang yang menyediakan informasi seputar jadwal dan stasiun MRT Jakarta.

**Skills:** REST API development dengan Go, backend architecture.

**Repository:** [`mrt-schedules`](https://github.com/kurapika12/mrt-schedules)

---

### Stegano Tool - Python GUI

**Role:** Developer (Portfolio Project)

**Tools:** Python

**Goal:** Membangun tool steganografi dengan GUI modern untuk menyembunyikan dan mengekstraksi pesan rahasia di dalam gambar secara aman.

**Description:** Stegano Tool - Secure Key Edition adalah aplikasi Python dengan GUI modern untuk menyembunyikan dan menampilkan pesan rahasia di dalam gambar menggunakan teknik steganografi dan enkripsi kunci unik (Fernet).

**Skills:** Steganografi, enkripsi data, GUI development dengan Python.

**Repository:** [`stegano-tool`](https://github.com/kurapika12/stegano-tool)

---

### WiFi Password Generator

**Role:** Developer (Portfolio Project)

**Tools:** HTML, JavaScript

**Goal:** Membuat tool web untuk menghasilkan password default router FiberHome secara otomatis.

**Description:** FiberHome WiFi Password Generator adalah tool web khusus untuk menghasilkan password default router FiberHome menggunakan metode konversi SSID, dengan mapping huruf-angka dan ekstraksi bagian hex dari SSID.

**Skills:** Client-side scripting, algorithm design, web tool development.

**Repository:** [`WiFi-Password-Generator`](https://github.com/kurapika12/WiFi-Password-Generator)

---

## Tools & Skills
- **Web Development:** Laravel, Blade, PHP, MySQL, Tailwind CSS, Vite, Flask
- **Mobile Development:** Flutter, Dart, Provider, Riverpod, sqflite, Isar
- **Programming Languages:** Python, Go, JavaScript, HTML
- **Tools:** Git & GitHub (branching, commit, pull request), Postman, Chart.js, FastAPI, React, Xendit Payment Gateway
- **Concepts:** REST API development (CRUD, validasi), integrasi API pada aplikasi mobile, CRUD application, role-based access control, offline-first architecture, data synchronization

## Contact
- LinkedIn: [@muhammadaslamhidayat](https://www.linkedin.com/in/muhammadaslamhidayat/)
- Email: alam090206@gmail.com
