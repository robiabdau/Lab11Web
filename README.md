# Lab11Web
```bash
Nama      : Robi Abda'u
NIM       : 311910563
Kelas     : TI.19.B1
M. Kuliah : Pemograman Web
Dosen     : Agung Nugroho,S.Kom.,M.Kom
```
# Tugas Praktikum 11
Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga 
semua link pada navigasi header dapat menampilkan tampilan dengan layout yang 
sama <br>

1. Menambah route untuk menu home

![image](https://user-images.githubusercontent.com/81253746/121814600-2012ce80-cc9c-11eb-9184-9dd94326bb8d.png)

2. Menambahkan function pada file page.php

![image](https://user-images.githubusercontent.com/81253746/121814624-45074180-cc9c-11eb-92d7-c0a44d7260b6.png)

3. Menambahkan file home.php pada direktori view

![image](https://user-images.githubusercontent.com/81253746/121814674-7e3fb180-cc9c-11eb-88a2-77015051f35f.png)

4. Menambahkan file artikel.php pada direktori view

![image](https://user-images.githubusercontent.com/81253746/121814701-97e0f900-cc9c-11eb-991c-3522f2121bbf.png)

5. Menambahkan file contact.php pada direktori view

![image](https://user-images.githubusercontent.com/81253746/121814727-bc3cd580-cc9c-11eb-9341-105ff4af23b6.png)

6. Hasil menu home

![image](https://user-images.githubusercontent.com/81253746/121814814-2e151f00-cc9d-11eb-968d-8882aa14b3f5.png)

7. Hasil menu artikel

![image](https://user-images.githubusercontent.com/81253746/121815157-2c4c5b00-cc9f-11eb-900f-946712149e30.png)

8. Hasil menu about

![image](https://user-images.githubusercontent.com/81253746/121815186-4be38380-cc9f-11eb-8b2c-c2ef22dbe01a.png)

9. Hasil menu kontak

![image](https://user-images.githubusercontent.com/81253746/121815208-6fa6c980-cc9f-11eb-8901-c5a51177cfdb.png)


# Praktikum 11
1. Installasi & konfigurasi CodeIgneter

2. Membuat route baru pada file Routes.php

![image](https://user-images.githubusercontent.com/81253746/121798955-8cb5ab00-cc53-11eb-8fbb-811c430351f3.png)

Cek routes pada CLI

![image](https://user-images.githubusercontent.com/81253746/121799193-e66aa500-cc54-11eb-967f-8093c94d31b2.png)

Hasil masih error sbb :

![image](https://user-images.githubusercontent.com/81253746/121799321-9d672080-cc55-11eb-9b07-d5bce5d4751e.png)

3. Membuat Controller (page.php)

![image](https://user-images.githubusercontent.com/81253746/121813068-b511c980-cc94-11eb-9964-34cb66a12a3d.png)

Hasil :

![image](https://user-images.githubusercontent.com/81253746/121813033-885db200-cc94-11eb-9da7-2bb857bae51a.png)

4. Auto Routing

![image](https://user-images.githubusercontent.com/81253746/121813155-edb1a300-cc94-11eb-859e-572a450261f2.png)

Hasil :

![image](https://user-images.githubusercontent.com/81253746/121813163-f99d6500-cc94-11eb-9de0-79a2c5e01f4e.png)

5. Membuat View

a. Membuat file about.php

![image](https://user-images.githubusercontent.com/81253746/121813231-56991b00-cc95-11eb-97a3-8bde4cf81436.png)

b. Mengubah method about pada class Controller Page

![image](https://user-images.githubusercontent.com/81253746/121813289-a5df4b80-cc95-11eb-8169-58b1af06be1d.png)

c. Hasil

![image](https://user-images.githubusercontent.com/81253746/121813314-b8f21b80-cc95-11eb-9ea4-ea320b934506.png)

6. Membuat Layout Web dengan CSS

a. Membuat file header.php

![image](https://user-images.githubusercontent.com/81253746/121813555-acba8e00-cc96-11eb-9a96-ab9a3d890427.png)

b. Membuat file footer.php

![image](https://user-images.githubusercontent.com/81253746/121813574-bfcd5e00-cc96-11eb-82af-19ceb9fd44b0.png)

c. mengubah file app/view/about.php

![image](https://user-images.githubusercontent.com/81253746/121813614-00c57280-cc97-11eb-8268-5f5d5fe1348b.png)

d. Hasil:

![image](https://user-images.githubusercontent.com/81253746/121813696-6dd90800-cc97-11eb-8487-c2679bde9a31.png)


<b></b>
# Praktikum 12 - Lanjutan Codeigniter - Pemrograman Web
```bash
Nama      : Robi Abda'u
NIM       : 311910563
Kelas     : TI.19.B1
M. Kuliah : Pemograman Web
Dosen     : Agung Nugroho,S.Kom.,M.Kom
```

## Persiapan
### Buat Database
```
CREATE DATABASE lab_ci4;
```
### Buat Tabel
```
CREATE TABLE artikel (
 id INT(11) auto_increment,
 judul VARCHAR(200) NOT NULL,
 isi TEXT,
 gambar VARCHAR(200),
 status TINYINT(1) DEFAULT 0,
 slug VARCHAR(200),
 PRIMARY KEY(id)
);
```
![1](https://user-images.githubusercontent.com/56241285/122758596-2e2ba500-d2c3-11eb-986c-75c26c2f496e.png)
![2](https://user-images.githubusercontent.com/56241285/122758603-31269580-d2c3-11eb-9c72-7b499ac51c6b.png)
## Langkah 1 - Konfigurasi Koneksi Database
### Konfigurasi dapat dilakukan dengan cara mengubah beberapa kode pada file htdocs\lab11_php_ci\ci4\.env.

- Cari pada line DATABASE
- Ubah seperti berikut ini
```
# database.default.hostname = localhost
# database.default.database = lab_ci4
# database.default.username = root
# database.default.password = 
# database.default.DBDriver = MySQLi
# database.default.DBPrefix =
```
- Hilangkan tanda pagar # didepan. Maka jadi seperti dibawah ini.
```
database.default.hostname = localhost
database.default.database = lab_ci4
database.default.username = root
database.default.password = 
database.default.DBDriver = MySQLi
database.default.DBPrefix =
```
![3](https://user-images.githubusercontent.com/56241285/122759157-d3467d80-d2c3-11eb-9527-6ac74d2f2041.png)
## Langkah 2 - Membuat Model
Selanjutnya adalah membuat Model untuk memproses data Artikel. Buat file baru pada folder app/Models dengan nama ArtikelModel.php

![4](https://user-images.githubusercontent.com/56241285/122760400-46042880-d2c5-11eb-81b0-f2675ab3388f.png)
## Langkah 3 - Membuat Controller
Buat Controller baru dengan nama Artikel.php pada folder app/Controllers

![5](https://user-images.githubusercontent.com/56241285/122760857-ca56ab80-d2c5-11eb-9636-cb899f8969c6.png)
## Langkah 4 - Membuat View
Buat folder baru dengan nama artikel pada folder app/views, kemudian buat file baru dengan nama index.php

![6](https://user-images.githubusercontent.com/56241285/122761299-481ab700-d2c6-11eb-8f6f-18a6e3b1bc6d.png)

Selanjutnya buka browser kembali, dengan mengakses url http://localhost:8080/artikel

![7](https://user-images.githubusercontent.com/56241285/122762592-adbb7300-d2c7-11eb-8479-0dc9c5b2ceb2.png)

Kemudian tambahkan beberapa data pada database agar dapat ditampilkan datanya

## Langkah 5 - Membuat Tampilan Detail Artikel
Tampilan pada saat judul berita di klik maka akan diarahkan ke halaman yang berbeda. Tambahkan fungsi baru pada Controller Artike dengan nama view()

![10](https://user-images.githubusercontent.com/56241285/122862655-ab9af800-d34b-11eb-8c18-ac373389922a.png)
## Langkah 6 - Membuat View Detail
Buat view baru untuk halaman detail dengan nama app/views/artikel/detail.php

![12](https://user-images.githubusercontent.com/56241285/122863107-6cb97200-d34c-11eb-8542-7070e48bdf9a.png)

##  Langkah 7 - Membuat Routing untuk artikel detail
Buka Kembali file app/config/Routes.php, kemudian tambahkan routing untuk artikel detail

![13](https://user-images.githubusercontent.com/56241285/122863432-ed786e00-d34c-11eb-899f-18bf398269ad.png)
![14](https://user-images.githubusercontent.com/56241285/122865172-1ea66d80-d350-11eb-83c1-d1f6d9e7428b.png)

## Langkah 8 - Membuat Menu Admin
- Buat method baru pada Controller Artikel dengan nama admin_index()

![15](https://user-images.githubusercontent.com/56241285/122865584-d50a5280-d350-11eb-82c8-665e8aa1694e.png)
- Kemudian buat view untuk tampilan admin dengan nama admin_index.php

![16](https://user-images.githubusercontent.com/56241285/122866073-95903600-d351-11eb-8a23-365b926cc03a.png)
![17](https://user-images.githubusercontent.com/56241285/122866086-99bc5380-d351-11eb-881f-30f8af01e977.png)

- Tambahkan routing untuk menu admin seperti berikut:

![18](https://user-images.githubusercontent.com/56241285/122866265-d9833b00-d351-11eb-887a-4cbceed73f38.png)

- Setelah itu buat template header dan footer baru untuk Halaman Admin. Buat file baru dengan nama admin_header.php pada direktori app/view/template

![19](https://user-images.githubusercontent.com/56241285/122866572-629a7200-d352-11eb-8b94-3bf825cdf483.png)

- Dan Buat file baru lagi dengan nama admin_footer.php pada direktori app/view/template

![20](https://user-images.githubusercontent.com/56241285/122866773-bad17400-d352-11eb-9e32-3a0733af7292.png)

- Kemudian buat file baru lagi dengan nama admin.css pada direktori ci4/public untuk mempercantik tampilan Halaman Admin

![21](https://user-images.githubusercontent.com/56241285/122867285-71355900-d353-11eb-9750-466e998c7acc.png)
![22](https://user-images.githubusercontent.com/56241285/122867302-785c6700-d353-11eb-87f2-913e8aece8d8.png)

- Akses menu admin dengan url http://localhost:8080/admin/artikel

![23](https://user-images.githubusercontent.com/56241285/122867496-cbceb500-d353-11eb-8ccb-96292eacad8b.png)

## Langkah 9 - Menambah Data Artikel
Tambahkan fungsi/method baru pada Controller Artikel dengan nama add()

![24](https://user-images.githubusercontent.com/56241285/122867840-56afaf80-d354-11eb-9478-975c9bbbec3d.png)

- Kemudian buat view untuk form tambah dengan nama form_add.php

![25](https://user-images.githubusercontent.com/56241285/122868197-d8074200-d354-11eb-84a1-3bddbcee4848.png)

- Klik menu Tambah Artikel dan inilah hasilnya
 
![26](https://user-images.githubusercontent.com/56241285/122869487-8d86c500-d356-11eb-973c-5ecab87e422a.png)

## Langkah 10 - Mengubah Data
- Tambahkan fungsi/method baru pada Controller Artikel dengan nama edit()

![27](https://user-images.githubusercontent.com/56241285/122869816-fff7a500-d356-11eb-8301-8b9fedea1646.png)

- Kemudian buat view untuk form tambah dengan nama form_edit.php

![28](https://user-images.githubusercontent.com/56241285/122870076-6a104a00-d357-11eb-9196-2d568a907f30.png)

- Klik ubah pada salah satu artikel dan inilah hasilnya

![29](https://user-images.githubusercontent.com/56241285/122870363-c2dfe280-d357-11eb-8c9f-7965c02528ca.png)

## Langkah 11 - Menghapus Data
- Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete()

![30](https://user-images.githubusercontent.com/56241285/122870562-05a1ba80-d358-11eb-8835-b67b2ae83f3b.png)

<b></b>
# Praktikum 13 - Lanjutan Praktikum sebelumnya - Pemrograman Web
```bash
Nama      : Robi Abda'u
NIM       : 311910563
Kelas     : TI.19.B1
M. Kuliah : Pemograman Web
Dosen     : Agung Nugroho,S.Kom.,M.Kom
```


1. Membuat Tabel User :

![image](https://user-images.githubusercontent.com/81431392/123540098-20768500-d6f2-11eb-93a6-cb00911e3180.png)

2. Membuat Model User :

![image](https://user-images.githubusercontent.com/81431392/123540179-937ffb80-d6f2-11eb-818b-482d350a93f9.png)

3. Membuat Controller User :

![image](https://user-images.githubusercontent.com/81431392/123540385-87486e00-d6f3-11eb-99f1-458b33b7e5fc.png)

4. Membuat View Login :

![image](https://user-images.githubusercontent.com/81431392/123542712-004dc280-d700-11eb-9d92-211abb9beffd.png)

5. Membuat Database Seeder :

- jalankan pada CLI php spark make:seeder UserSeeder 
- edit file Database/Seeds/UserSeeder.php : 

 ![image](https://user-images.githubusercontent.com/81431392/123540730-59642900-d6f5-11eb-9a43-32677bb79179.png)


- lalu jalankan lagi CLI php spark db:seed UserSeeder

hasil outputnya : 

![image](https://user-images.githubusercontent.com/81431392/123542761-43a83100-d700-11eb-9594-c250764b7d7c.png)


ketika isi email,password maka muncul pada halaman portal admin :

![image](https://user-images.githubusercontent.com/81431392/123542783-69cdd100-d700-11eb-8c1d-f8ef7f0c9e5a.png)

6. Menambahkan Auth Filter : 

![image](https://user-images.githubusercontent.com/81431392/123542912-ea8ccd00-d700-11eb-926f-8b36650305a9.png) 
 
 7. Konfigurasi file app/Config/Filters.php : 
 
![image](https://user-images.githubusercontent.com/81431392/123542978-55d69f00-d701-11eb-9797-780bcd3f0d63.png) 

8. dan konfigurasi app/Config/Routes.php : 

![image](https://user-images.githubusercontent.com/81431392/123543075-b9f96300-d701-11eb-9117-82d3145dd762.png) 

hasil outputnya : 

![image](https://user-images.githubusercontent.com/81431392/123544719-68ed6d00-d709-11eb-8829-30d641aa2f19.png) 

Fungsi Logout : 

![image](https://user-images.githubusercontent.com/81431392/123544784-b2d65300-d709-11eb-92d7-2ee02d1adcc6.png) 



























                         
