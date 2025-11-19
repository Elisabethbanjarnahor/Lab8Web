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


##    2. Membuat Koneksi Database (koneksi.php)
Koneksi menggunakan mysqli_connect:


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



  


