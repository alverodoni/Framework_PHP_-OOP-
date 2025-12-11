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
     Halaman ini menampilkan semua artikel dalam format tabel agar mudah dibaca dan diorganisir.
  2. Fitur Utama `(Tombol)`
     Tombol "Tambah Artikel Baru": Tombol ini digunakan untuk menjalankan operasi CREATE `(membuat data baru)`. Jika diklik, pengguna akan diarahkan ke halaman form untuk menginput data artikel baru.
  3. Struktur Tabel
     - NO: Nomor urut artikel (biasanya dihitung dari baris).
     - JUDUL: Judul utama dari artikel.
     - ISI: ringkasan singkat dari konten artikel.
     - TANGGAL: Tanggal artikel tersebut dibuat atau diperbarui.
     - AKSI: Kolom ini berisi tombol-tombol untuk mengelola artikel perbarisnya:
         - Edit (Hijau): Digunakan untuk operasi UPDATE `(mengubah/memperbarui data artikel)`.
         - Delete (Merah): Digunakan untuk operasi DELETE `(menghapus data artikel)`.

### halaman tambah artikel
- Halaman ini adalah form yang digunakan untuk menjalankan operasi CREATE `(membuat/menambah data baru)` dalam modul Artikel. Tujuannya adalah mengumpulkan informasi yang diperlukan untuk menyimpan satu entri artikel baru ke dalam database.
- Komponen Utama
  - ID `(Internal)`
  - Judul Artikel
  - Tanggal
  - Isi Artikel
- Navigasi & Aksi
  - "← Kembali ke Daftar": Tautan ini memungkinkan pengguna kembali ke halaman Daftar Artikel tanpa menyimpan data yang sedang diinput.
  - Tombol "Simpan Artikel": Tombol aksi utama. Jika diklik, sistem akan mencoba menyimpan data yang telah diinput ke dalam database kemudian datanya kesimpan ke halaman artikel yaitu ditabel artikel

### halaman user 
- Halaman ini adalah Data Pengguna `(User)`, dan berfungsi untuk menampilkan daftar semua pengguna yang terdaftar dalam sistem. Seperti halaman Artikel, halaman ini mewakili operasi READ dari fungsi CRUD.
- Tampilan Utama
  - Halaman ini menampilkan semua data pengguna dalam format tabel yang terstruktur.
- Fitur Utama `(Tombol)`
  - Tombol "Tambah User Baru": Tombol ini digunakan untuk menjalankan operasi CREATE `(membuat data baru)`. Jika diklik, pengguna akan diarahkan ke halaman form untuk menginput detail pengguna baru.
- Struktur Tabel `(Data Pengguna)`
  - NO: Nomor urut pengguna.
  - NAMA: Nama lengkap pengguna.
  - EMAIL: Alamat email pengguna.
  - JENIS KELAMIN: Jenis kelamin pengguna `(Laki-laki/Perempuan)`.
  - AGAMA: Informasi agama pengguna.
  - HOBY: Informasi hobi pengguna.
  - ALAMAT: Alamat fisik pengguna.
  - AKSI: Kolom ini berisi tombol-tombol untuk mengelola data pengguna per barisnya:
    - Edit (Hijau): Digunakan untuk operasi UPDATE `(mengubah/memperbarui detail pengguna)`
    - Delete `(Merah)`: Digunakan untuk       operasi DELETE `(menghapus data         pengguna dari sistem)`.

### halaman tambah user
- Halaman ini adalah Form Input User `(dengan Oop Routing)` yang berfungsi untuk menjalankan operasi CREATE `(menambah data)` pada modul pengguna. Halaman ini digunakan untuk mendaftarkan pengguna baru ke dalam    sistem.
- Komponen Utama `(Form Input)`
  - ID `(Internal)`
  - Nama Lengkap
  - Password `(Sandi)`
  - Jenis Kelamin
  - Agama
  - Hobi
  - Alamat Lengkap
- Navigasi & Aksi
  - "← Kembali ke Daftar": Tautan untuk membatalkan proses dan kembali ke halaman Daftar User.
  - Tombol "Simpan User": Tombol aksi utama. Jika diklik, data yang diinput akan diproses dan disimpan.

### kesimpulan 
- Ini adalah framework sederhana berbasis PHP Object-Oriented Programming `(OOP)` & `(CRUD)` yaitu Create, Read, Update & Delete

### Image Halaman home 
<img width="1918" height="970" alt="halaman home" src="https://github.com/user-attachments/assets/fc874872-75ee-4bb3-98c3-eeeed0468676" />
### Image Halaman artikel 
<img width="1918" height="971" alt="halaman artikel " src="https://github.com/user-attachments/assets/e2b30c71-3a03-441f-92b5-5e6926323bfd" />
### Image Halaman tambah artikel
<img width="1918" height="973" alt="halaman tambah artikel " src="https://github.com/user-attachments/assets/46cacf5c-032c-4c95-990c-060d90a3157f" />
### Image Halaman user 
<img width="1918" height="972" alt="halaman user " src="https://github.com/user-attachments/assets/cab702bd-31cc-4264-bc0b-02c7ae94fb82" />
### Image Halaman tambah user  
<img width="1918" height="973" alt="halaman tambah user " src="https://github.com/user-attachments/assets/8475c657-6115-4eb8-af3d-b13861c65c59" />

### codingan keseluruhan 
```php
<?php
// --- INISIASI SESI ---
session_start();

// --- DATA AWAL (DEFAULT) ---
$default_artikel_data = [
    [
        'id' => 1,
        'judul' => 'Pengenalan PHP OOP',
        'isi' => 'Object-Oriented Programming (OOP) adalah sebuah pendekatan atau paradigma pemrograman di PHP yang mengorganisasi kode berdasarkan konsep "objek". Berbeda dengan pemrograman prosedural yang fokus pada urutan fungsi, OOP mengemas data (properti) dan fungsi (metode) yang relevan ke dalam satu unit yang disebut objek.',
        'tanggal' => '10-11-2025'
    ],
    [
        'id' => 2,
        'judul' => 'Framework PHP',
        'isi' => 'Framework PHP adalah kerangka kerja atau struktur dasar yang menyediakan kumpulan kode (library, fungsi, kelas) siap pakai untuk mempercepat dan mempermudah pengembangan aplikasi web berbasis PHP.',
        'tanggal' => '09-11-2025'
    ],
    [
        'id' => 3,
        'judul' => 'Routing di PHP',
        'isi' => 'Routing di PHP adalah proses mengarahkan permintaan URL dari pengguna ke script atau controller kode yang tepat di dalam aplikasi web Anda, sehingga URL yang kompleks menjadi lebih rapi (URL friendly) dan mudah dikelola.',
        'tanggal' => '08-11-2025'
    ]
];

$default_user_data = [
    [
        'id' => 1,
        'nama' => 'Alvero',
        'email' => 'alvero@gmail.com',
        'jk' => 'Laki-laki',
        'agama' => 'Islam',
        'alamat' => 'Jl. Sandrise No. 8',
        'hobi' => 'Travelling' 
    ],
    [
        'id' => 2,
        'nama' => 'Deceng',
        'email' => 'deceng@gmail.com',
        'jk' => 'Laki-laki',
        'agama' => 'Islam',
        'alamat' => 'Jl. Danser No. 5',
        'hobi' => 'Olahraga'
    ],
    [
        'id' => 3,
        'nama' => 'Mela',
        'email' => 'mela@gmail.com',
        'jk' => 'Laki-laki',
        'agama' => 'Islam',
        'alamat' => 'Jl. Cikaleng No. 3',
        'hobi' => 'Memasak'
    ]
];

// Inisiasi data di $_SESSION jika belum ada
if (!isset($_SESSION['artikel_data'])) {
    $_SESSION['artikel_data'] = $default_artikel_data;
}
if (!isset($_SESSION['user_data'])) {
    $_SESSION['user_data'] = $default_user_data;
}

// Ambil data dari SESSION
$artikel_data = $_SESSION['artikel_data'];
$user_data = $_SESSION['user_data'];

// --- SIMULASI ROUTING Sederhana ---
$page = isset($_GET['page']) ? $_GET['page'] : 'home';
$action = isset($_GET['action']) ? $_GET['action'] : '';


// --- LOGIKA CRUD: ARTIKEL ---
if ($page == 'tambah_artikel' && $_SERVER['REQUEST_METHOD'] == 'POST') {
    $id = $_POST['id'] ?? null;
    $judul = $_POST['judul'] ?? '';
    $isi = $_POST['isi'] ?? '';
    // Menggunakan input tanggal dari form (format D-M-Y)
    $tanggal_input = $_POST['tanggal'] ?? date('Y-m-d');
    $tanggal_format = date('d-m-Y', strtotime($tanggal_input)); 

    if ($judul && $isi) {
        $is_found = false;
        
        // Cek apakah ini edit (jika ID sudah ada)
        foreach ($_SESSION['artikel_data'] as $key => $artikel) {
            if ((string)$artikel['id'] === (string)$id && $id !== null && $id !== '') {
                $_SESSION['artikel_data'][$key]['judul'] = $judul;
                $_SESSION['artikel_data'][$key]['isi'] = $isi;
                $_SESSION['artikel_data'][$key]['tanggal'] = $tanggal_format; // Update tanggal
                $is_found = true;
                break;
            }
        }

        // Jika tidak ditemukan, ini adalah Tambah baru
        if (!$is_found) {
            // Tentukan ID baru (maksimum ID + 1)
            $new_id = 1;
            if (!empty($_SESSION['artikel_data'])) {
                 $new_id = max(array_column($_SESSION['artikel_data'], 'id')) + 1;
            }

            $new_artikel = [
                'id' => $new_id,
                'judul' => $judul,
                'isi' => $isi,
                'tanggal' => $tanggal_format
            ];
            $_SESSION['artikel_data'][] = $new_artikel;
        }
        
        // Redirect setelah simpan
        header('Location: ?page=artikel');
        exit;
    }

} elseif ($page == 'artikel' && $action == 'delete' && isset($_GET['id'])) {
    // Aksi Delete Artikel
    $id_to_delete = (int)$_GET['id'];
    foreach ($_SESSION['artikel_data'] as $key => $artikel) {
        if ($artikel['id'] == $id_to_delete) {
            unset($_SESSION['artikel_data'][$key]);
            $_SESSION['artikel_data'] = array_values($_SESSION['artikel_data']); // Re-index array
            break;
        }
    }
    // Redirect setelah delete
    header('Location: ?page=artikel');
    exit;
}

// --- LOGIKA CRUD: USER ---
if ($page == 'tambah_user' && $_SERVER['REQUEST_METHOD'] == 'POST') {
    $id = $_POST['id'] ?? null;
    $nama = $_POST['nama'] ?? '';
    $email = $_POST['email'] ?? '';
    $jk = $_POST['jk'] ?? '';
    $agama = $_POST['agama'] ?? '';
    // Hobi adalah array, perlu diubah jadi string untuk penyimpanan
    $hobi = isset($_POST['hobi']) ? implode(', ', $_POST['hobi']) : '';
    $alamat = $_POST['alamat'] ?? '';

    if ($nama && $email) {
        $is_found = false;
        
        // Cek apakah ini edit (jika ID sudah ada)
        foreach ($_SESSION['user_data'] as $key => $user) {
            if ((string)$user['id'] === (string)$id && $id !== null && $id !== '') {
                $_SESSION['user_data'][$key]['nama'] = $nama;
                $_SESSION['user_data'][$key]['email'] = $email;
                $_SESSION['user_data'][$key]['jk'] = $jk;
                $_SESSION['user_data'][$key]['agama'] = $agama;
                $_SESSION['user_data'][$key]['hobi'] = $hobi;
                $_SESSION['user_data'][$key]['alamat'] = $alamat;
                $is_found = true;
                break;
            }
        }

        // Jika tidak ditemukan, ini adalah Tambah baru
        if (!$is_found) {
            // Tentukan ID baru
            $new_id = 1;
            if (!empty($_SESSION['user_data'])) {
                 $new_id = max(array_column($_SESSION['user_data'], 'id')) + 1;
            }

            $new_user = [
                'id' => $new_id,
                'nama' => $nama,
                'email' => $email,
                'jk' => $jk,
                'agama' => $agama,
                'hobi' => $hobi,
                'alamat' => $alamat
            ];
            $_SESSION['user_data'][] = $new_user;
        }
        
        // Redirect setelah simpan
        header('Location: ?page=user');
        exit;
    }

} elseif ($page == 'user' && $action == 'delete' && isset($_GET['id'])) {
    // Aksi Delete User
    $id_to_delete = (int)$_GET['id'];
    foreach ($_SESSION['user_data'] as $key => $user) {
        if ($user['id'] == $id_to_delete) {
            unset($_SESSION['user_data'][$key]);
            $_SESSION['user_data'] = array_values($_SESSION['user_data']); // Re-index array
            break;
        }
    }
    // Redirect setelah delete
    header('Location: ?page=user');
    exit;
}

// Perbarui data yang akan ditampilkan setelah operasi CRUD
$artikel_data = $_SESSION['artikel_data'];
$user_data = $_SESSION['user_data'];


?>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Framework PHP OOP - Praktikum 11</title>
    <style>
        /* Gaya Aesthetic/Menarik (CSS tidak berubah dari sebelumnya) */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        /* HEADER (Hitam) */
        header {
            background-color: #1a1a1a;
            color: #ffffff;
            padding: 20px 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 1.8em;
            letter-spacing: 1px;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0 0;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: #ccc;
            text-decoration: none;
            font-weight: bold;
            padding: 8px 15px;
            transition: color 0.3s, background-color 0.3s;
            border-radius: 5px;
        }

        /* Efek Hover untuk Navigasi */
        nav ul li a:hover {
            color: #ffffff;
            background-color: #333333;
        }

        /* CONTAINER (Dashboard Putih) */
        .container {
            width: 85%;
            margin: 30px auto;
            background-color: #ffffff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            min-height: 60vh;
        }

        h2 {
            color: #0056b3;
            border-bottom: 2px solid #007bff;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        
        /* Tabel (Biru Muda) */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        table th, table td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        /* Warna Biru Muda untuk Header Tabel */
        table th {
            background-color: #b0e0e6; /* Biru Muda */
            color: #333;
            font-weight: bold;
            text-transform: uppercase;
        }

        /* Efek Hover untuk Baris Tabel */
        table tr:hover {
            background-color: #e6f7ff;
        }

        .action-btn {
            padding: 6px 10px;
            margin: 2px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            text-decoration: none;
            color: #fff;
            display: inline-block;
        }

        .btn-edit { background-color: #28a745; }
        .btn-delete { background-color: #dc3545; }
        .btn-add {
            background-color: #007bff;
            color: #fff;
            padding: 8px 15px;
            border-radius: 5px;
            text-decoration: none;
            display: inline-block;
            margin-bottom: 15px;
            transition: background-color 0.3s;
        }
        .btn-add:hover { background-color: #0056b3; }

        /* Form Styling */
        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }

        .form-group input[type="text"],
        .form-group input[type="email"],
        .form-group input[type="password"],
        .form-group input[type="date"], /* Tambahkan input date */
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }

        .form-group textarea {
            resize: vertical;
        }
        
        .radio-group label, .checkbox-group label {
            margin-right: 15px;
        }

        .btn-submit {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .btn-submit:hover {
            background-color: #0056b3;
        }

        /* FOOTER (Hitam) */
        footer {
            background-color: #1a1a1a;
            color: #ffffff;
            text-align: center;
            padding: 15px 0;
            position: relative;
            bottom: 0;
            width: 100%;
            margin-top: 20px;
        }
        
        /* Box Info Home */
        .info-box {
            border-left: 5px solid #007bff;
            padding: 15px;
            background-color: #e9f7ff;
            margin-top: 20px;
            border-radius: 5px;
        }
        .info-box h4 { margin-top: 0; color: #0056b3; }
        .info-box ul { list-style-type: none; padding-left: 0; }
        .info-box li::before { content: "•"; color: #007bff; font-weight: bold; display: inline-block; width: 1em; margin-left: -1em; }
    </style>
</head>
<body>

<header>
    <h1>Framework PHP OOP - Praktikum 11</h1>
    <nav>
        <ul>
            <li><a href="?page=home">Home</a></li>
            <li><a href="?page=artikel">Artikel</a></li>
            <li><a href="?page=tambah_artikel">Tambah Artikel</a></li>
            <li><a href="?page=user">User</a></li>
            <li><a href="?page=tambah_user">Tambah User</a></li>
        </ul>
    </nav>
</header>

<div class="container">
    <?php
    // --- KONTEN DINAMIS BERDASARKAN $page ---
    switch ($page) {
        case 'home':
            // 1. Bagian Home
            ?>
            <h2>Selamat Datang di Framework PHP OOP</h2>
            <p>Ini adalah halaman home dari framework modular sederhana menggunakan PHP OOP.</p>

            <h3>Fitur Framework:</h3>
            <ul>
                <li>Routing dengan URL Rewriting</li>
                <li>Database Class untuk CRUD Operations</li>
                <li>Form Class untuk Dynamic Form Generation</li>
                <li>Struktur Modular yang Terorganisir</li>
                <li>Template System (Header & Footer)</li>
            </ul>
            
            <div class="info-box">
                <h4>Cara Menggunakan:</h4>
                <p>Navigasi ke menu untuk mencoba fitur CRUD pada modul Artikel dan User.</p>
            </div>
            <?php
            break;

        case 'artikel':
            // 2. Bagian Artikel
            ?>
            <h2>Daftar Artikel</h2>
            <a href="?page=tambah_artikel" class="btn-add">+ Tambah Artikel Baru</a>
            <table>
                <thead>
                    <tr>
                        <th>No</th>
                        <th>Judul</th>
                        <th>Isi</th>
                        <th>Tanggal</th>
                        <th>Aksi</th>
                    </tr>
                </thead>
                <tbody>
                    <?php 
                    $row_number = 1;
                    foreach ($artikel_data as $artikel): 
                    ?>
                    <tr>
                        <td><?= $row_number++ ?></td> 
                        <td><?= htmlspecialchars($artikel['judul']) ?></td>
                        <td><?= substr(htmlspecialchars($artikel['isi']), 0, 100) . '...' ?></td>
                        <td><?= $artikel['tanggal'] ?></td>
                        <td>
                            <a href="?page=tambah_artikel&action=edit&id=<?= $artikel['id'] ?>" class="action-btn btn-edit">Edit</a>
                            <a href="?page=artikel&action=delete&id=<?= $artikel['id'] ?>" class="action-btn btn-delete" onclick="return confirm('Yakin ingin menghapus artikel ID <?= $artikel['id'] ?>?')">Delete</a>
                        </td>
                    </tr>
                    <?php endforeach; ?>
                </tbody>
            </table>
            <?php
            break;

        case 'tambah_artikel':
            // 3. Bagian Tambah Artikel (Berlaku juga untuk Edit)
            $is_edit = $action == 'edit' && isset($_GET['id']);
            $form_title = $is_edit ? 'Edit Artikel' : 'Tambah Artikel Baru';
            
            // Default nilai kosong untuk Tambah Baru
            $artikel_edit = ['id' => '', 'judul' => '', 'isi' => '', 'tanggal' => date('Y-m-d')];

            if ($is_edit) {
                $id_edit = (int)$_GET['id'];
                // Cari data artikel dari SESSION
                foreach ($artikel_data as $item) {
                    if ($item['id'] == $id_edit) {
                        $artikel_edit = $item;
                        // Ubah format tanggal dari d-m-Y (tampilan) ke Y-m-d (input date)
                        $artikel_edit['tanggal'] = date('Y-m-d', strtotime($item['tanggal']));
                        break;
                    }
                }
            }
            ?>
            <h2><?= $form_title ?></h2>
            <a href="?page=artikel" style="margin-bottom: 15px; display: inline-block;">&larr; Kembali ke Daftar</a>
            <form action="?page=tambah_artikel" method="POST">
                <div class="form-group">
                    <label for="id">ID (Internal):</label>
                    <input type="text" id="id" name="id" value="<?= htmlspecialchars($artikel_edit['id']) ?>" required <?= $is_edit ? 'readonly' : '' ?>>
                    <?php if (!$is_edit): ?>
                    <small style="color: gray;">*ID akan diisi otomatis, abaikan field ini untuk tambah baru.</small>
                    <?php endif; ?>
                </div>
                <div class="form-group">
                    <label for="judul">Judul Artikel:</label>
                    <input type="text" id="judul" name="judul" value="<?= htmlspecialchars($artikel_edit['judul']) ?>" required>
                </div>
                
                <div class="form-group">
                    <label for="tanggal">Tanggal:</label>
                    <input type="date" id="tanggal" name="tanggal" value="<?= htmlspecialchars($artikel_edit['tanggal']) ?>" required>
                </div>

                <div class="form-group">
                    <label for="isi">Isi Artikel:</label>
                    <textarea id="isi" name="isi" rows="10" required><?= htmlspecialchars($artikel_edit['isi']) ?></textarea>
                </div>
                <button type="submit" class="btn-submit">Simpan Artikel</button>
                <p style="margin-top: 15px; color: green;">**Data akan disimpan ke Session (tidak permanen).**</p>
            </form>
            <?php
            break;

        case 'user':
            // 4. Bagian User
            ?>
            <h2>Daftar User</h2>
            <a href="?page=tambah_user" class="btn-add">+ Tambah User Baru</a>
            <table>
                <thead>
                    <tr>
                        <th>No</th>
                        <th>Nama</th>
                        <th>Email</th>
                        <th>Jenis Kelamin</th>
                        <th>Agama</th>
                        <th>Hobi</th> 
                        <th>Alamat</th>
                        <th>Aksi</th>
                    </tr>
                </thead>
                <tbody>
                    <?php 
                    $row_number = 1;
                    foreach ($user_data as $user): ?>
                    <tr>
                        <td><?= $row_number++ ?></td> 
                        <td><?= htmlspecialchars($user['nama']) ?></td>
                        <td><?= htmlspecialchars($user['email']) ?></td>
                        <td><?= htmlspecialchars($user['jk']) ?></td>
                        <td><?= htmlspecialchars($user['agama']) ?></td>
                        <td><?= htmlspecialchars($user['hobi']) ?></td>
                        <td><?= htmlspecialchars($user['alamat']) ?></td>
                        <td>
                            <a href="?page=tambah_user&action=edit&id=<?= $user['id'] ?>" class="action-btn btn-edit">Edit</a>
                            <a href="?page=user&action=delete&id=<?= $user['id'] ?>" class="action-btn btn-delete" onclick="return confirm('Yakin ingin menghapus user ID <?= $user['id'] ?>?')">Delete</a>
                        </td>
                    </tr>
                    <?php endforeach; ?>
                </tbody>
            </table>
            <?php
            break;

        case 'tambah_user':
            // 5. Bagian Tambah User
            $is_edit = $action == 'edit' && isset($_GET['id']);
            $form_title = $is_edit ? 'Form Edit User' : 'Form Input User (OOP dengan Routing)';
            
            $user_edit = [
                'id' => '', 'nama' => '', 'email' => '', 'jk' => '', 'agama' => '', 'hobi' => '', 'alamat' => ''
            ];

            if ($is_edit) {
                $id_edit = (int)$_GET['id'];
                // Cari data user dari SESSION
                foreach ($user_data as $item) {
                    if ($item['id'] == $id_edit) {
                        $user_edit = $item;
                        break;
                    }
                }
            }

            $list_agama = ['Islam', 'Protestan', 'Katolik', 'Buddha', 'Hindu', 'Konghucu'];
            $list_hobi = ['Membaca', 'Coding', 'Travelling', 'Olahraga', 'Memasak'];
            ?>
            <h2><?= $form_title ?></h2>
            <a href="?page=user" style="margin-bottom: 15px; display: inline-block;">&larr; Kembali ke Daftar</a>
            <form action="?page=tambah_user" method="POST">
                
                <div class="form-group">
                    <label for="id">ID (Internal):</label>
                    <input type="text" id="id" name="id" value="<?= htmlspecialchars($user_edit['id']) ?>" required <?= $is_edit ? 'readonly' : '' ?>>
                    <?php if (!$is_edit): ?>
                    <small style="color: gray;">*ID akan diisi otomatis, abaikan field ini untuk tambah baru.</small>
                    <?php endif; ?>
                </div>

                <div class="form-group">
                    <label for="nama">Nama Lengkap:</label>
                    <input type="text" id="nama" name="nama" value="<?= htmlspecialchars($user_edit['nama']) ?>" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" value="<?= htmlspecialchars($user_edit['email']) ?>" required>
                </div>
                <div class="form-group">
                    <label for="password">Password (Simulasi):</label>
                    <input type="password" id="password" name="password" value="*****" <?= $is_edit ? 'readonly' : '' ?> required>
                </div>
                
                <div class="form-group">
                    <label>Jenis Kelamin:</label>
                    <div class="radio-group">
                        <label><input type="radio" name="jk" value="Laki-laki" <?= $user_edit['jk'] == 'Laki-laki' ? 'checked' : '' ?> required> Laki-laki</label>
                        <label><input type="radio" name="jk" value="Perempuan" <?= $user_edit['jk'] == 'Perempuan' ? 'checked' : '' ?>> Perempuan</label>
                    </div>
                </div>

                <div class="form-group">
                    <label for="agama">Agama:</label>
                    <select id="agama" name="agama" required>
                        <?php foreach ($list_agama as $agama): ?>
                        <option value="<?= $agama ?>" <?= $user_edit['agama'] == $agama ? 'selected' : '' ?>><?= $agama ?></option>
                        <?php endforeach; ?>
                    </select>
                </div>

                <div class="form-group">
                    <label>Hobi:</label>
                    <div class="checkbox-group">
                        <?php 
                        // Pisahkan string hobi menjadi array untuk mengecek checkbox
                        $selected_hobi = explode(', ', $user_edit['hobi']); 
                        foreach ($list_hobi as $hobi): ?>
                        <label>
                            <input type="checkbox" name="hobi[]" value="<?= $hobi ?>" <?= in_array($hobi, $selected_hobi) ? 'checked' : '' ?>> <?= $hobi ?>
                        </label>
                        <?php endforeach; ?>
                    </div>
                </div>

                <div class="form-group">
                    <label for="alamat">Alamat Lengkap:</label>
                    <textarea id="alamat" name="alamat" rows="5" required><?= htmlspecialchars($user_edit['alamat']) ?></textarea>
                </div>
                
                <button type="submit" class="btn-submit">Simpan User</button>
                <p style="margin-top: 15px; color: green;">**Data akan disimpan ke Session (tidak permanen).**</p>
            </form>
            <?php
            break;
            
        default:
            // Kembali ke Home jika halaman tidak terdefinisi
            header('Location: ?page=home');
            exit;
    }
    ?>
</div>

<footer>
    &copy; 2024 Framework PHP OOP - Praktikum 11 | Universitas Pelita Bangsa
</footer>

</body>
</html>
```



