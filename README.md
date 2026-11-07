# Day 1 - Workshop "Building with AI, Managing Change with GitHub"

**Nama Lengkap:** Lazwardi Aulia
**Kelompok:** 22 - Far Cry 5
**Tanggal Workshop:** 07 November 2026
**Pemateri:** Nugi Farhan (Senior Product Designer)

---

## Deskripsi Repository

Repository ini berisi dokumentasi kegiatan Day 1 workshop **"Building with AI, Managing Change with GitHub"**, mencakup rangkuman materi, poin-poin penting yang saya pelajari, dan pendapat pribadi saya tentang Day 1 Proyek Workshop.

## Tujuan Repository

- Mendokumentasikan materi dan pengetahuan baru dari workshop Day 1.
- Melatih penggunaan Git dan GitHub untuk version control.
- Memenuhi ketentuan tugas Day 1 dari panitia.

## Kegiatan Workshop yang Didokumentasikan

Workshop Day 1 membahas dua topik utama:

1. **Membuat dan mengembangkan dengan AI:** prompt engineering.
2. **Manajemen perubahan dan kolaborasi:** Git dan GitHub.

Dokumentasi lengkapnya ada di bagian-bagian berikut dalam file ini: Rangkuman Materi, Poin Penting dan Pengetahuan Baru, serta Pendapat Pribadi.

## Daftar Isi

1. [Rangkuman Materi](#1-rangkuman-materi)
2. [Poin Penting dan Pengetahuan Baru](#2-poin-penting-dan-pengetahuan-baru)
3. [Pendapat Pribadi tentang Day 1](#3-pendapat-pribadi-tentang-day-1-proyek-workshop)

---

## 1. Rangkuman Materi

### 1.1 Capaian Pembelajaran

- Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
- Membedakan Git dan GitHub.
- Mengidentifikasi repository, commit, branch, dan pull request.
- Melakukan version controlling.

### 1.2 Prompt Engineering

**Pengertian.** Prompt engineering adalah cara merancang instruksi agar AI memberikan jawaban yang tepat, relevan, dan layak digunakan. Prompt bisa berupa pertanyaan sederhana, kata kunci, instruksi rumit, atau potongan kode.

**Context is key.** Prompt tanpa konteks (misalnya "Create student task planner") memberi AI terlalu sedikit informasi. Prompt dengan konteks menjelaskan peran, tujuan, kebutuhan, dan batasan sehingga hasilnya lebih sesuai.

**Struktur prompt yang baik:**

| Komponen | Fungsi | Contoh dari workshop |
|---|---|---|
| Role | Peran yang diminta dari AI | "You are helping me build a beginner-friendly student task planner..." |
| Task | Tugas yang dikerjakan | Membuat task planner untuk mahasiswa baru |
| Context | Kebutuhan dan batasan | Daftar tugas, filter, hanya HTML, CSS, vanilla JS |
| Format | Bentuk output | Kode lengkap tiap file, cara menjalankan, cara menguji |

**Taktik menulis prompt** (sumber: Google Cloud, *What is prompt engineering*):

- Gunakan kata kerja aksi untuk menentukan tindakan yang diinginkan.
- Tentukan panjang dan format output.
- Tentukan target audiens.
- Sertakan fakta dan data yang relevan.
- Rujuk sumber atau dokumen tertentu.
- Definisikan istilah dan konsep kunci.

**Keuntungan prompt engineering:** meningkatkan performa model AI, mengurangi bias dan respons yang offensive, meningkatkan kontrol dan predictability, serta memberikan pengalaman yang lebih baik.

### 1.3 Git dan GitHub

**Git** adalah sistem version control terdistribusi (DVCS) yang melacak siapa, kapan, dan apa yang berubah dalam sebuah file. Git dibuat oleh Linus Torvalds pada tahun 2005 dan bekerja secara lokal.

**GitHub** adalah platform berbasis web untuk menyimpan repository Git secara online dan mendukung kolaborasi.

**Alur kerja Git:**

| Area | Penjelasan |
|---|---|
| Working Directory | Salinan satu versi proyek yang sedang dikerjakan di komputer |
| Staging Area (index) | Menyimpan informasi perubahan yang akan masuk ke commit berikutnya |
| Git Directory (Repository) | Tempat Git menyimpan metadata dan object database proyek; bagian ini yang disalin saat clone |

Alurnya: Working Directory → (`git add`) → Staging Area → (`git commit`) → Repository.

### 1.4 Perintah Dasar Git

| Perintah | Fungsi |
|---|---|
| `git init` | Memulai repository baru |
| `git clone "url"` | Menyalin repository dari GitHub ke komputer |
| `git add .` | Memindahkan perubahan ke staging area |
| `git commit -m "pesan"` | Menyimpan perubahan ke repository |
| `git remote add <name> <url>` | Menghubungkan repository lokal ke remote (GitHub) |
| `git push origin main` | Mengirim commit dari branch lokal ke GitHub |
| `git pull origin main` | Mengambil perubahan dari GitHub dan menggabungkannya ke branch saat ini |

### 1.5 Setup yang Dilakukan

1. Install Git, lalu cek dengan `git --version`.
2. Atur identitas Git:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```
3. Install VS Code dan aktifkan perintah `code` di terminal.
4. Buat SSH key dengan `ssh-keygen -t ed25519 -C "email@domain.com"`, tambahkan public key ke GitHub (*Settings → SSH and GPG keys*), lalu verifikasi dengan `ssh -T git@github.com`.

### 1.6 Proyek Workshop: Student Task Planner

Proyek latihan berupa aplikasi web sederhana untuk mencatat tugas dan deadline mahasiswa. Alurnya: pasang platform AI, tulis prompt untuk membuat aplikasinya, `git init`, commit dan push ke GitHub, lakukan perubahan, lalu commit dan push lagi.

---

## 2. Poin Penting dan Pengetahuan Baru

- **Prompt yang spesifik menghasilkan hasil lebih baik.** Prompt singkat seperti "Create student task planner" membuat AI menebak-nebak kebutuhan kita, sedangkan prompt yang menjelaskan tujuan, kebutuhan, dan batasan menghasilkan jawaban yang lebih sesuai.
- **Struktur Role, Task, Context, Format** membantu menyusun prompt secara runtut, sehingga tidak ada informasi penting yang terlewat saat meminta sesuatu ke AI.
- **Git dan GitHub itu berbeda.** Git melacak perubahan secara lokal, GitHub menyimpannya online untuk kolaborasi.
- **Ada staging area** di antara working directory dan repository, sehingga kita bisa memilih perubahan mana yang masuk ke commit.
- **SSH key** memungkinkan koneksi ke GitHub tanpa memasukkan password setiap kali push atau pull.
- **Pesan commit perlu jelas**, karena riwayat commit adalah catatan perubahan yang akan dibaca anggota tim lain.

---

## 3. Pendapat Pribadi tentang Day 1 Proyek Workshop

Menurut saya, workshop hari ini berjalan baik karena pemateri menyampaikan materi dengan sangat jelas, mulai dari prompt engineering sampai konsep Git dan GitHub. Penjelasan yang runtut membuat materi yang awalnya terasa teknis jadi lebih mudah dipahami.

Namun, pada sesi praktik terdapat kendala. Praktik mengharuskan peserta menginstal beberapa perangkat seperti Git, sementara sinyal di lokasi workshop sulit didapat. Kendala jaringan ini cukup menghambat proses instalasi dan membuat praktik tidak berjalan semulus penyampaian materinya.

Meski begitu, saya melihat penggunaan Git sangat penting bagi mahasiswa TIK. Git mempermudah workflow kerja sama dalam tim, karena setiap perubahan tercatat dan bisa dikelola bersama tanpa saling menimpa pekerjaan. Saya berharap pada hari-hari berikutnya instalasi bisa disiapkan lebih awal, sehingga waktu workshop bisa fokus ke praktik.