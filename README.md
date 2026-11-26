# PP-KELOMPOK-6-ASDOS
# 🔑 Find The Key in Maze — C++ Ncurses Implementation

> *Tugas Akhir / Final Project Pemrograman C++*
> Game petualangan labirin berbasis terminal menggunakan bahasa C dan library ncurses dengan kontrol keyboard, sistem kunci & pintu keluar, serta tampilan berwarna.

---

## 📋 Daftar Isi
1. [Latar Belakang & Studi Kasus](#-latar-belakang--studi-kasus)
2. [Fitur Utama](#-fitur-utama)
3. [Struktur Kode & Arsitektur](#-struktur-kode--arsitektur)
4. [Prasyarat & Instalasi](#-prasyarat--instalasi)
5. [Cara Kompilasi](#-cara-kompilasi)
6. [Kontrol Permainan](#-kontrol-permainan)
7. [Pembagian Tugas & Progres](#-pembagian-tugas--progres)
8. [Credits](#-credits)

---
## 📖 Latar Belakang & Studi Kasus

Proyek ini dikembangkan sebagai Proyek Akhir (Final Project) untuk mata kuliah *Pengenalan Pemrograman*. Tujuan utamanya adalah merancang dan membangun game interaktif berbasis teks/terminal yang mengimplementasikan materi dasar pemrograman:

- *Modularisasi Fungsi (Function):* Memisahkan alur program ke dalam fungsi-fungsi yang jelas dan terstruktur.
- *Struktur Data Array (Array):* Menggunakan array 2D untuk merepresentasikan tata letak peta labirin dan array 1D untuk menyimpan informasi/petunjuk.
- *Perulangan (Looping):* Menggunakan while dan for untuk game loop, pembacaan peta, serta pemrosesan logika permainan.
- *Percabangan (Conditional):* Menggunakan if-else dan switch-case untuk validasi gerak, deteksi dinding, pengambilan kunci, serta kondisi menang/kalah.
- *Terminal UI (ncurses):* Menampilkan antarmuka teks interaktif, warna, serta membaca input keyboard secara langsung.

---

## ✨ Fitur Utama
- *Navigasi Labirin Berbasis Grid:* Peta labirin 2D dengan dinding (#), jalur kosong (` ), kunci (`K), dan pintu keluar (E).
- *Mekanik Kunci & Pintu Keluar:* Pemain (@) harus menemukan kunci K terlebih dahulu sebelum dapat membuka pintu keluar E.
- *Deteksi Tabrakan (Collision Detection):* Mencegah pemain menembus dinding # dan memberikan informasi status secara langsung.
- *Tampilan Berwarna ncurses:* Membedakan karakter pemain, dinding, kunci, dan pintu keluar menggunakan pasangan warna terminal.

---

## 🏗️ Struktur Kode & Arsitektur

Struktur repositori proyek *Find The Key in Maze*:

📦 Find-The-Key-In-Maze
┣ 📜 main.c
┣ 📜 README.md
┗ 📂 docs/

*Ringkasan Fungsi Utama:*
- init_ui() — Menginisialisasi mode ncurses, input keyboard, dan pasangan warna.
- draw_maze() — Menggambar peta labirin, kunci/pintu, karakter pemain, dan status permainan ke layar terminal.
- show_win_screen() — Menampilkan layar kemenangan saat pemain berhasil keluar melewati E.
- main() — Mengatur game loop, input arah pemain, serta logika pengambilan kunci dan pintu keluar.

---

## ⚙️ Prasyarat & Instalasi
Pastikan lingkungan pengembangan memiliki:

- *Compiler C++:* gcc (di Linux, macOS, WSL, atau MSYS2/MinGW).
- *Library ncurses:* Terinstal di sistem (contoh di Ubuntu/Debian: sudo apt install libncurses5-dev libncursesw5-dev).
- *Terminal:* Mendukung ANSI/warna ncurses.

---

## 🛠️ Cara Kompilasi

Buka terminal di direktori proyek, lalu jalankan:

```bash
gcc main.c -o find_the_key_in_maze -lncurses
````

---

## 🎮 Kontrol Permainan

| Aksi        | Tombol Keyboard       |
| ----------- | ----------------      |
| Gerak Atas  | W atau Panah Atas (↑) |
| Gerak Bawah | S atau Panah Bawah (↓)|  
| Gerak Kanan | D atau Panah Kanan (→)|
| Gerak Kiri | A atau Panah Kiri   (←)|
| Keluar Game | Q (Saat bermain)      |

---

## 📅 Pembagian Tugas & Progres

Progres 1 (Kamis, 26 November 2026): 
Pembuatan repositori GitHub, draf README.md, kerangka kode awal ncurses, peta dasar, flowchart dan pengumpulan dokumen progres pertama.

---

## 👨‍💻 Credits

Universitas Lampung

| Nama                       | NPM        |
| -----------------------    | ---------- |
| Vincentius Evelyn Dovan T. | 2617051026 |
| Intan Citra Nabila         | 2617051019 |
| Ratu Fiona Tsaqifah        | 2617051028 |

---

