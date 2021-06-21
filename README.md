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

























                         
