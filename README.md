# Git Workflow untuk Pengembangan Fitur

Dokumen ini menjelaskan langkah-langkah untuk mengelola branch, mengambil update, dan mengirim perubahan ke dalam proyek Git secara kolaboratif.

## 1. Ambil Pembaruan Terbaru

Sebelum memulai pekerjaan, selalu periksa pembaruan terbaru dari repository remote.

```bash
git fetch
```

## 2. Tarik Perubahan jika ada
```bash
git pull
```
## 3. Buat Branch Baru untuk Setiap Fitur
Untuk setiap fitur atau tugas yang sedang kamu kerjakan, buat branch baru untuk menjaga perubahan tetap terisolasi. Gunakan konvensi penamaan: feature/nama-fitur.
```bash
git branch feature/nama-fitur
```
Contoh jika kamu mengerjakan halaman home
```bash
git branch feature/halaman_home
```
## 4. Pindah ke Branch Baru
Setelah branch baru dibuat, pindah ke branch tersebut dengan perintah berikut:
```bash
git checkout feature/nama-fitur
```
Contoh
```bash
git checkout feature/halaman_home
```
## 5. Kerjakan Fitur yang Diperlukan
Sekarang kamu siap untuk mulai bekerja pada fitur baru tersebut. Lakukan perubahan yang diperlukan dan uji kode kamu.
## 6. Stage Perubahan Kamu
Setelah fitur selesai dan diuji, stage perubahan dengan menggunakan git add:
```bash
git add .
```
Perintah ini akan menandai semua file yang dimodifikasi untuk siap di-commit.
## 7. Commit Perubahan Kamu
Commit perubahan yang telah di-stage dengan pesan commit yang deskriptif. Pastikan untuk menggunakan pesan yang menjelaskan fitur atau perbaikan yang telah kamu kerjakan.
```bash
git commit -m "feat: menyelesaikan fitur halaman_home"
```
## 8. Push Branch Kamu ke Repository Remote
Push branch lokalmu ke repository remote dengan perintah berikut:
```bash
git push -u origin feature/nama-fitur
```
Contoh
```bash
git push -u origin feature/halaman_home
```
## 9. Buat Pull Request
Setelah branch-mu berhasil dipush, kamu bisa membuka pull request di repository remote (misal, GitHub, GitLab) untuk menggabungkan perubahanmu ke branch utama.

