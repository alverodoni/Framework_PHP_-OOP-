# Framework_PHP_-OOP-
Nama: Doni Alvero <p>
Nim: 312410663 <P>
Kelas: TI.24.A.5 <P>
Jurusan: Teknik Informatika <p>
Mata Kuliah: Pemograman Web 1 <p>

### halaman home 
- Halaman home adalah halaman sambutan  dari sebuah Framework PHP OOP sederhana. Halaman ini berfungsi sebagai pengantar dan perkenalan fitur utama dari framework yang dibuat.
- Cara Menggunakannya dengan diarahkan untuk menggunakan menu navigasi di atas `(Artikel dan User)` untuk mencoba fitur CRUD `(mengelola data artikel atau pengguna)`.
- Judul Utama Aplikasi: "Framework PHP OOP - Praktikum 11". `(header)`
- Navigasi/Menu: Kumpulan link penting agar pengguna bisa berpindah antar halaman/modul. Pada gambar, menunya adalah `home)` `(artikel)` `(tambah artikel)` `(user)` `(tambah user)`
- "© 2024 Framework PHP OOP - Praktikum 11 | Universitas Pelita Bangsa". `(footer)` & Menyediakan informasi branding juga hak cipta.

### halaman artikel 
- Halaman ini adalah implementasi dari fungsi READ dalam operasi CRUD `(Create, Read, Update, Delete)`. Tujuannya adalah untuk menampilkan semua data artikel yang tersimpan dalam database dan menyediakan akses untuk mengelola data tersebut.
  1. Tampilan Utama
     Halaman ini menampilkan semua           artikel dalam format tabel agar         mudah dibaca dan diorganisir.
  2. Fitur Utama `(Tombol)`
     Tombol "Tambah Artikel Baru":           Tombol ini digunakan untuk              menjalankan operasi CREATE             `(membuat data baru)`. Jika diklik,      pengguna akan diarahkan ke halaman      form untuk menginput data artikel       baru.
  3. Struktur Tabel
     - NO: Nomor urut artikel (biasanya        dihitung dari baris).
     - JUDUL: Judul utama dari artikel.
     - ISI: ringkasan singkat dari             konten artikel.
     - TANGGAL: Tanggal artikel                tersebut dibuat atau diperbarui.
     - AKSI: Kolom ini berisi tombol-          tombol untuk mengelola artikel          per barisnya:
         - Edit (Hijau): Digunakan                 untuk operasi UPDATE                    `(mengubah/memperbarui data             artikel)`.
         - Delete (Merah): Digunakan               untuk operasi DELETE                    `(menghapus data artikel)`.

### halaman tambah artikel
- Halaman ini adalah form yang digunakan untuk menjalankan operasi CREATE `(membuat/menambah data baru)` dalam modul Artikel. Tujuannya adalah mengumpulkan informasi yang diperlukan untuk menyimpan satu entri artikel baru ke dalam database.
- Komponen Utama
  - ID `(Internal)`
  - Judul Artikel
  - Tanggal
  - Isi Artikel
- Navigasi & Aksi
  - "← Kembali ke Daftar": Tautan ini       memungkinkan pengguna kembali ke        halaman Daftar Artikel tanpa            menyimpan data yang sedang diinput.
  - Tombol "Simpan Artikel": Tombol         aksi utama. Jika diklik, sistem         akan mencoba menyimpan data yang        telah diinput ke dalam database         kemudian datanya kesimpan ke            halaman artikel yaitu ditabel           artikel

