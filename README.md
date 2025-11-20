# Lab8Web

## Nama   : Elisabeth Erni Banjarnahor
## Nim    : 312410525
## Matkul :Pemograman Web1
## Kls    :Ti.24.A5

## Tujuan Praktikum

Praktikum ini bertujuan untuk mempelajari:

    Menghubungkan PHP dengan database MySQL menggunakan mysqli
    Melakukan operasi CRUD (Create, Read, Update, Delete)
    Menggunakan form HTML untuk input data
    Upload file (gambar) menggunakan enctype="multipart/form-data"
    Menampilkan data dalam bentuk tabel
    Mengatur struktur folder pada XAMPP (htdocs)

## 🗄️ 1. Membuat Database & Tabel
Database dibuat melalui phpMyA

```CREATE DATABASE latihan1;
USE latihan1;

CREATE TABLE data_barang (
  id_barang INT(10) AUTO_INCREMENT PRIMARY KEY,
  kategori VARCHAR(30),
  nama VARCHAR(30),
  gambar VARCHAR(100),
  harga_beli DECIMAL(10,0),
  harga_jual DECIMAL(10,0),
  stok INT(4)
);
```

##    2. Membuat Koneksi Database (koneksi.php)
Koneksi menggunakan mysqli_connect:
```
<?php
$host = "localhost";
$user = "root";
$pass = "";
$db   = "latihan1";

$conn = mysqli_connect($host, $user, $pass, $db);
if (!$conn) {
    echo "Koneksi gagal: " . mysqli_connect_error();
    die();
}
?>
```

## 📄 3. Menampilkan Data (index.php)
Halaman utama menampilkan semua data dari tabel data_barang dalam bentuk tabel.

Fitur pada halaman ini:

Menampilkan data lengkap

Menampilkan gambar

Tombol Ubah

Tombol Hapus

Tombol Tambah Barang

## ➕ 4. Menambah Data Barang (tambah.php)

Pada bagian ini, user bisa menambahkan:

Nama barang

Kategori

Harga jual

Harga beli

Stok

Upload Gambar

Data yang diinput akan disimpan dalam database.


## ✏️ 5. Mengubah Data (ubah.php)

User bisa meng-update data barang yang sudah ada. Termasuk mengganti:

Nama barang

Kategori

Harga

Stok

Gambar (opsional)

Jika user tidak memilih gambar baru, gambar lama tetap digunakan.


## ❌ 6. Menghapus Data (hapus.php)
Menghapus data barang berdasarkan ID. Setelah dihapus, halaman akan langsung kembali ke index.php.



  


