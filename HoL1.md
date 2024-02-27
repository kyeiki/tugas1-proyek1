
# Hands-on Lab: Hello World dengan Git

Selamat datang di Hands-on Lab "Hello World dengan Git". Lab ini dirancang untuk membantu pemula memahami dasar-dasar penggunaan Git, sebuah sistem kontrol versi terdistribusi yang memungkinkan Anda untuk melacak perubahan dalam file dan berkolaborasi dengan pengembang lain.

## Persyaratan
- Git terinstal di komputer Anda. Anda bisa mengunduhnya dari [situs resmi Git](https://git-scm.com/downloads).
- Akun GitHub (opsional, jika Anda ingin mempelajari cara push ke remote repository).

## Konfigurasi Git

Sebelum memulai, konfigurasikan identitas Anda yang akan digunakan dalam setiap commit Git.

```bash
git config --global user.name "Nama Anda"
git config --global user.email "email@anda.com"
```

## Membuat Repository Lokal

1. Buka terminal atau command prompt.
2. Buat sebuah direktori baru, lalu masuk ke dalamnya:
   ```bash
   mkdir hello-world
   cd hello-world
   ```
3. Inisialisasi direktori tersebut sebagai repository Git:
   ```bash
   git init
   ```

## Menambahkan File README.md

1. Buat file baru dengan nama `README.md`:
   ```bash
   touch README.md
   ```
2. Buka file tersebut menggunakan editor teks pilihan Anda, lalu tambahkan teks berikut:
   ```markdown
   # Hello World Project
   Ini adalah proyek pertama saya menggunakan Git.
   ```
3. Simpan perubahan.

## Melakukan Commit Pertama

1. Tambahkan file `README.md` ke staging area:
   ```bash
   git add README.md
   ```
2. Lakukan commit dengan pesan yang menjelaskan perubahan Anda:
   ```bash
   git commit -m "Tambahkan README.md"
   ```

## Membuat Repository di GitHub (Opsional)

1. Masuk ke [GitHub](https://github.com/) dan buat repository baru dengan nama `hello-world-3digitnim`.
2. Masuk ke [Github Setting key](https://github.com/settings/keys), tambahkan ssh key / value id_rsa.pub ke Github setting Key, cara generate ssh-key [Tutorial SSH Key](https://www.cs.utexas.edu/facilities-documentation/ssh-keys-csres-windows-10)
3. Ikuti instruksi GitHub untuk "…or push an existing repository from the command line" yang mencakup perintah `git remote add origin` dan `git push -u origin main`.

## Push Ke GitHub

1. Push perubahan Anda ke GitHub dengan perintah berikut:
   ```bash
   git push -u origin main
   ```

Selamat! Anda telah berhasil membuat proyek Hello World pertama Anda dengan Git dan, jika memilih, telah mempushnya ke GitHub.

## Rangkuman

Dalam lab ini, Anda telah belajar bagaimana:
- Mengkonfigurasi Git
- Membuat repository lokal
- Menambahkan file dan melakukan commit
- Membuat repository di GitHub dan push perubahan ke repository remote (opsional)

Teruslah belajar dan eksplorasi lebih lanjut tentang Git untuk meningkatkan keterampilan kolaborasi dan pengelolaan kode Anda.
