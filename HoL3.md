
# Hands-on Lab: Hello World Branching dengan Git

Lab ini akan mengajarkan Anda dasar-dasar branching dan merging menggunakan Git, memungkinkan Anda untuk bekerja pada berbagai fitur atau perbaikan secara paralel dengan kode utama. Ini adalah keterampilan penting dalam workflow pengembangan perangkat lunak.

## Persyaratan
- Git terinstal pada komputer Anda.
- Sebuah repository Git lokal dengan beberapa commit. Jika belum, silakan ikuti lab "Hello World dengan Git" untuk memulai.

## Mengenal Branching di Git

Branch di Git memungkinkan Anda untuk diverge dari development line utama dan terus bekerja tanpa mengganggu line tersebut. Setiap branch merupakan salinan dari kode pada waktu tertentu, yang bisa dikembangkan secara independen.

## Membuat Branch Baru

1. Buka terminal atau command prompt.
2. Pastikan Anda berada di direktori project Git Anda.
3. Buat branch baru dengan perintah:
   ```bash
   git branch nama-branch
   ```
4. Ganti ke branch yang baru dibuat:
   ```bash
   git checkout nama-branch
   ```
   Atau gunakan perintah singkat untuk membuat dan ganti ke branch baru:
   ```bash
   git checkout -b nama-branch
   ```

## Menambahkan Perubahan pada Branch Baru

1. Buat atau modifikasi file dalam project Anda. Contoh, tambahkan file baru:
   ```bash
   touch greetings.txt
   echo "Hello from nama-branch!" > greetings.txt
   ```
2. Tambahkan file ke staging area dan commit perubahan:
   ```bash
   git add greetings.txt
   git commit -m "Add greetings from nama-branch"
   ```

## Kembali ke Main Branch dan Merging

1. Ganti kembali ke main/master branch:
   ```bash
   git checkout main
   ```
2. Gabungkan perubahan dari branch yang Anda buat ke main branch:
   ```bash
   git merge nama-branch
   ```
   Pastikan tidak ada konflik merge. Jika ada, selesaikan terlebih dahulu.

## Membersihkan Branch

Setelah berhasil menggabungkan branch dan semua perubahan sudah aman di main branch, Anda bisa menghapus branch yang tidak lagi dibutuhkan:
```bash
git branch -d nama-branch
```

## Rangkuman

Dalam lab ini, Anda telah belajar:
- Cara membuat branch baru di Git.
- Cara melakukan perubahan pada branch baru dan commit perubahan tersebut.
- Cara mengganti branch.
- Cara menggabungkan perubahan dari satu branch ke branch lain.
- Cara menghapus branch yang tidak lagi dibutuhkan.

Branching adalah fitur penting Git yang mendukung workflow pengembangan paralel, memungkinkan tim untuk bekerja lebih efisien.

Teruslah eksplorasi lebih lanjut tentang Git untuk meningkatkan keterampilan kolaborasi dan pengelolaan kode Anda.
