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

### halaman user 
- Halaman ini adalah Data Pengguna `(User)`, dan berfungsi untuk menampilkan daftar semua pengguna yang terdaftar dalam sistem. Seperti halaman Artikel, halaman ini mewakili operasi READ dari fungsi CRUD.
- Tampilan Utama
  - Halaman ini menampilkan semua data      pengguna dalam format tabel yang        terstruktur.
- Fitur Utama `(Tombol)`
  - Tombol "Tambah User Baru": Tombol       ini digunakan untuk menjalankan         operasi CREATE `(membuat data           baru)`. Jika diklik, pengguna akan      diarahkan ke halaman form untuk         menginput detail pengguna baru.
- Struktur Tabel `(Data Pengguna)`
  - NO: Nomor urut pengguna.
  - NAMA: Nama lengkap pengguna.
  - EMAIL: Alamat email pengguna.
  - JENIS KELAMIN: Jenis kelamin            pengguna `(Laki-laki/Perempuan)`.
  - AGAMA: Informasi agama pengguna.
  - HOBY: Informasi hobi pengguna.
  - ALAMAT: Alamat fisik pengguna.
  - AKSI: Kolom ini berisi tombol-          tombol untuk mengelola data             pengguna per barisnya:
    - Edit (Hijau): Digunakan untuk           operasi UPDATE                         `(mengubah/memperbarui detail            pengguna)`
    - Delete `(Merah)`: Digunakan untuk       operasi DELETE `(menghapus data         pengguna dari sistem)`.

### halaman tambah user 
- Halaman ini adalah Form Input User `(dengan Oop Routing)` yang berfungsi untuk menjalankan operasi CREATE `(menambah data)` pada modul pengguna. Halaman ini digunakan untuk mendaftarkan pengguna baru ke dalam sistem.
- Komponen Utama `(Form Input)`
  - ID `(Internal)`
  - Nama Lengkap
  - Password `(Sandi)`
  - Jenis Kelamin
  - Agama
  - Hobi
  - Alamat Lengkap
- Navigasi & Aksi
  - "← Kembali ke Daftar": Tautan untuk     membatalkan proses dan kembali ke       halaman Daftar User.
  - Tombol "Simpan User": Tombol aksi       utama. Jika diklik, data yang           diinput akan diproses dan disimpan.

### kesimpulan 
- Ini adalah framework sederhana berbasis PHP Object-Oriented Programming '(OOP)' & `(CRUD)` yaitu Create, Read, Update & Delete


