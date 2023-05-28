# Lab7_php_ci

framework CRUD PHP code igniter

###### Nama : Muhammad Arya Dipanegara Gunawan

###### NIM : 312110396

###### Kelas : TI.21.A3

Instruksi Praktikum

1. Persiapkan text editor misalnya VSCode.

2. Buka kembali folder dengan nama lab11_php_ci pada docroot webserver (htdocs)

3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.

Langkah-langkah Praktikum

Persiapan.

Untuk memulai membuat aplikasi CRUD sederhana, yang perlu disiapkan adalah
database server menggunakan MySQL. Pastikan MySQL Server sudah dapat dijalankan
melalui XAMPP.

#### Membuat Database & Tabel

![](./IMG/image-1.png)

#### Konfigurasi koneksi database

Selanjutnya membuat konfigurasi untuk menghubungkan dengan database server.
Konfigurasi dapat dilakukan dengan du acara, yaitu pada file app/config/database.php
atau menggunakan file .env. Pada praktikum ini kita gunakan konfigurasi pada file .env.

![](./IMG/image-2.png)

#### Membuat Model

Selanjutnya adalah membuat Model untuk memproses data Artikel. Buat file baru pada
direktori app/Models dengan nama ArtikelModel.php

![](./IMG/image-3.jpg)

#### Membuat Controller

Buat Controller baru dengan nama Artikel.php pada direktori app/Controllers.

![](./IMG/image-4.png)

#### Membuat View

Buat direktori baru dengan nama artikel pada direktori app/views, kemudian buat file
baru dengan nama index.php.

![](./IMG/image-5.png)

Selanjutnya buka browser kembali, dengan mengakses url http://localhost:8080/artikeL

![](./IMG/image-6.png)

Belum ada data yang diampilkan. Kemudian coba tambahkan beberapa data pada
database agar dapat ditampilkan datanya.

![](./IMG/image-7.png)

![](img/6%20enam.jpg)

Refresh kembali browser, sehingga akan ditampilkan hasilnya.

![](./IMG/image-8.png)

#### Membuat Tampilan Detail Artikel

Tampilan pada saat judul berita di klik maka akan diarahkan ke halaman yang berbeda.
Tambahkan fungsi baru pada Controller Artikel dengan nama view().

![](./IMG/image-9.png)

#### Membuat View Detail

Buat view baru untuk halaman detail dengan nama app/views/artikel/detail.php

![](./IMG/image-10.png)

#### Membuat Routing untuk artikel detail

Buka Kembali file app/config/Routes.php, kemudian tambahkan routing untuk artikel
detail.

![](./IMG/image-11.png)

![](./IMG/image-12.png)

#### Membuat Menu Admin

Menu admin adalah untuk proses CRUD data artikel. Buat method baru pada
Controller Artikel dengan nama admin_index().

![](./IMG/image-13.png)

Selanjutnya buat view untuk tampilan admin dengan nama admin_index.php

![](./IMG/menuadmin.png)
![](./IMG/admin_index.png)

Tambahkan routing untuk menu admin seperti berikut:

![](./IMG/route_admin.png)

Akses menu admin dengan url http://localhost:8080/admin/artikel

![](./IMG/aksesadmin.png)

#### Menambah Data Artikel

Tambahkan fungsi/method baru pada Controller Artikel dengan nama add()

![](./IMG/fungsi_add.png)

Kemudian buat view untuk form tambah dengan nama form_add.php

![](./IMG/form_add.png)

hasil

![](./IMG/hasil_formadd.png)

#### Mengubah Data

Tambahkan fungsi/method baru pada Controller Artikel dengan nama edit().

![](./IMG/edit.png)

Kemudian buat view untuk form tambah dengan nama form_edit.php

![](./IMG/form_edit.png)

hasil :

![](./IMG/hasil_formedit.png)

#### Menghapus Data

Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete().

![](./IMG/hapus.png)

Hasil :

![](./IMG/hasilhapus.png)

## Pertanyaan dan Tugas

Selesaikan programnya sesuai Langkah-langkah yang ada. Anda boleh melakukan
improvisasi.

#### Laporan Praktikum

1. Melanjutkan praktikum sebelumnya pada repository dengan nama lab7web.
2. Kerjakan semua latihan yang diberikan sesuai urutannya.
3. Screenshot setiap perubahannya.
4. Update file README.md dan tuliskan penjelasan dari setiap langkah praktikum
   beserta screenshotnya.
5. Commit hasilnya pada repository masing-masing.
6. Kirim URL repository pada e-learning ecampus
