# Lab11Web

Praktikum 11: PHP Framework (Codeigniter)

1. konfigurasi PHP.ini :

![image](https://user-images.githubusercontent.com/81431392/121955588-ff3a8f80-cd14-11eb-857b-59d5d7bdece5.png)

2. extention, hilangkan tanda ; (titik koma) pada ekstensi yang akan diaktifkan :

![image](https://user-images.githubusercontent.com/81431392/121956150-a0294a80-cd15-11eb-95f2-40194d0e71fa.png)

3. hasil output di web server :

![image](https://user-images.githubusercontent.com/81431392/121960603-2bf1a580-cd1b-11eb-9aad-b60e3402640c.png)

4. Menjalankan CLI (Command Line Interface)
lalu jalankan syntax : 
- cd d:\xampp\htdocs\lab11_php_ci\ci4
- php spark
dan hasilnya :

![image](https://user-images.githubusercontent.com/81431392/121958040-0ca54900-cd18-11eb-9019-ab55063468cd.png)

5. Mengaktifkan Mode Debugging dan konfigurasi file env yg ada di D:\xampp\htdocs\lab11_php_ci\ci4 ubah menjadi .env dan edit nilai variable,nya :

![image](https://user-images.githubusercontent.com/81431392/121958695-cac8d280-cd18-11eb-83d7-3296ec8c4041.png)

6. contoh mengubah file home.php dengan mengahapus tanda ; (titik coma) maka akan terjadi muncul pesan Whoops! :

![image](https://user-images.githubusercontent.com/81431392/121961327-28125300-cd1c-11eb-9f2c-a0a783c88fe6.png)

7. konfigurasi Routing dan Controller yg terletak di app/config/Routes.php :

![image](https://user-images.githubusercontent.com/81431392/121962025-05346e80-cd1d-11eb-8d93-4a98959015ae.png)

menambahkan Route baru di routes.php :

![image](https://user-images.githubusercontent.com/81431392/121962512-afac9180-cd1d-11eb-9ffb-403284de1dc2.png)

 dan hasilnya pada CLI php spark routes :
 
 ![image](https://user-images.githubusercontent.com/81431392/121962643-df5b9980-cd1d-11eb-88ff-a86b878f9444.png)

hasil output di web server maka terjadi error 404 file not found karena file/page tsb tidak ada.
![image](https://user-images.githubusercontent.com/81431392/121970176-d02f1880-cd2a-11eb-9ae8-75b5b62b52f7.png)

8. membuat Controller page.php pada direktori Controller :

![image](https://user-images.githubusercontent.com/81431392/121963220-aa037b80-cd1e-11eb-83d2-ad9ea270cf02.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/121969990-6878cd80-cd2a-11eb-83b8-541bb417dc01.png)

9. auto routing :

 ![image](https://user-images.githubusercontent.com/81431392/121970833-47b17780-cd2c-11eb-8243-afddb4fc7d15.png)
 
 hasil outputnya
 
 ![image](https://user-images.githubusercontent.com/81431392/121970898-61eb5580-cd2c-11eb-8b2b-31ff5dcb1430.png)

10. membuat php.about pada direktori (app/view/about.php) :

![image](https://user-images.githubusercontent.com/81431392/121971339-606e5d00-cd2d-11eb-9ee0-baf3af7a902e.png)

11. Ubah method about pada class Controller Page :

![image](https://user-images.githubusercontent.com/81431392/121971405-8267df80-cd2d-11eb-9985-034b10edde16.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/121971466-a3303500-cd2d-11eb-87af-c3b6666c626f.png)

12. Membuat Layout Web dengan CSS header.php dan footer.php pada direktori baru app/view/template :

![image](https://user-images.githubusercontent.com/81431392/121971878-a546c380-cd2e-11eb-983c-16ef0da102b5.png)

![image](https://user-images.githubusercontent.com/81431392/121971896-b1328580-cd2e-11eb-9a72-f7495400f7b3.png)

kemudian ubah file app/view/about.php :

![image](https://user-images.githubusercontent.com/81431392/121972177-49c90580-cd2f-11eb-9d32-6459e82b7f39.png)

dan hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/121972257-7a10a400-cd2f-11eb-9184-7349bddd75e0.png)

<b>TUGAS PRATIKUM</b>

1. menu home :

![image](https://user-images.githubusercontent.com/81431392/121972436-f1dece80-cd2f-11eb-9974-bce22dfb02f4.png)

2. menu artikel :

![image](https://user-images.githubusercontent.com/81431392/121972487-15097e00-cd30-11eb-8d2a-fb8ebab8ee29.png)

3. menu about :

![image](https://user-images.githubusercontent.com/81431392/121972518-2783b780-cd30-11eb-9c2a-07fc06a3e348.png)

4. menu kontak :

![image](https://user-images.githubusercontent.com/81431392/121972555-3a968780-cd30-11eb-92df-90a65156f3c1.png)


<b>Lanjut Tugas Pratikum ke 12 </b>

1. buat database lab_ci4 :

![image](https://user-images.githubusercontent.com/81431392/122088711-dbca2000-cdba-11eb-8b7a-5e40f3eb30cb.png)

2. konfigurasi koneksi database .env :

![image](https://user-images.githubusercontent.com/81431392/122089782-f6e95f80-cdbb-11eb-9e83-b0d6042a3a7f.png)

3. membuat ArtikelModel.php pada direktori app/Models :

![image](https://user-images.githubusercontent.com/81431392/122090450-9f97bf00-cdbc-11eb-8376-8400cc996fcc.png)

4. membuat Artikel.php pada direktori app/Controllers :

![image](https://user-images.githubusercontent.com/81431392/122090572-bf2ee780-cdbc-11eb-87e2-fc0615637284.png)

5. Membuat direktori artikel pada app/view dan isi file index.php :

![image](https://user-images.githubusercontent.com/81431392/122090922-2482d880-cdbd-11eb-8a05-9a5f49a7eb8f.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/122851566-05f07600-d2c4-11eb-9aae-e1c4393bdea8.png)

6. tambahkan isi tabel database lab_ci4 :

![image](https://user-images.githubusercontent.com/81431392/122091633-d91cfa00-cdbd-11eb-9ffc-b530cc4664bf.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/122837257-a5077480-d2a8-11eb-8625-816f0ca3c5d6.png)

7. Membuat View Detail dengan nama app/views/artikel/detail.php :

![image](https://user-images.githubusercontent.com/81431392/122852982-58329680-d2c6-11eb-8994-31eb06efa7ad.png)


hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/122843259-e5b8bb00-d2b3-11eb-92a8-0c8df1febdee.png)

8. Membuat menu admin :

![image](https://user-images.githubusercontent.com/81431392/122846156-1b60a280-d2ba-11eb-89b4-b5c89238d363.png)

9. Membuat template admin_header dan admin_footer :

![image](https://user-images.githubusercontent.com/81431392/122848478-71374980-d2be-11eb-9db2-98499d753243.png)

![image](https://user-images.githubusercontent.com/81431392/122848503-801dfc00-d2be-11eb-9ddb-dc992aacd7d9.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/122848543-9461f900-d2be-11eb-8280-ea9a5ec099c7.png)

10. menambahkan controller add dan membuat form_add.php :

![image](https://user-images.githubusercontent.com/81431392/122848656-dee37580-d2be-11eb-8201-c1fe1281cfc5.png)

![image](https://user-images.githubusercontent.com/81431392/122848883-40a3df80-d2bf-11eb-9a91-0a0a59e8fca4.png)

hasil outputnya dan contoh menambahan artikel baru :

![image](https://user-images.githubusercontent.com/81431392/122849267-071fa400-d2c0-11eb-9d0b-d27aa2c7eaa4.png)

![image](https://user-images.githubusercontent.com/81431392/122849337-28809000-d2c0-11eb-9526-cd2c91488900.png)

11. membuat controler edit dan form_edit.php :

![image](https://user-images.githubusercontent.com/81431392/122850242-be68ea80-d2c1-11eb-834e-cdcc3942e36e.png)

![image](https://user-images.githubusercontent.com/81431392/122850392-fd973b80-d2c1-11eb-9af9-15ef24b73250.png)

hasil outputnya dan contoh edit :

![image](https://user-images.githubusercontent.com/81431392/122850594-549d1080-d2c2-11eb-8a91-3c48bd21d1d4.png)

![image](https://user-images.githubusercontent.com/81431392/122850642-70a0b200-d2c2-11eb-9754-50761d268f8c.png)

12. menambahkan controler untuk menghapus data :

![image](https://user-images.githubusercontent.com/81431392/122850829-bd848880-d2c2-11eb-9020-ed0d8cb35b59.png)

hasil outputnya dan contoh ketika di klik hapus maka data yg dipilih akan hilang :

![image](https://user-images.githubusercontent.com/81431392/122851005-13f1c700-d2c3-11eb-94e0-a5d197094671.png)

![image](https://user-images.githubusercontent.com/81431392/122851215-721eaa00-d2c3-11eb-8857-17e43036374f.png)

<b>Lanjut Tugas Pratikum ke 13 </b>

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

dan ketika isi email,password maka muncul pada halaman portal admin :

![image](https://user-images.githubusercontent.com/81431392/123542783-69cdd100-d700-11eb-8c1d-f8ef7f0c9e5a.png)

6. Menambahkan Auth Filter :

![image](https://user-images.githubusercontent.com/81431392/123542912-ea8ccd00-d700-11eb-926f-8b36650305a9.png)

7. Konfigurasi file app/Config/Filters.php :

![image](https://user-images.githubusercontent.com/81431392/123542978-55d69f00-d701-11eb-9797-780bcd3f0d63.png)

8. dan konfigurasi app/Config/Routes.php :

![image](https://user-images.githubusercontent.com/81431392/123543075-b9f96300-d701-11eb-9117-82d3145dd762.png)

hasil outputnya :

![image](https://user-images.githubusercontent.com/81431392/123544719-68ed6d00-d709-11eb-8829-30d641aa2f19.png)

9. Fungsi Logout :

![image](https://user-images.githubusercontent.com/81431392/123544784-b2d65300-d709-11eb-92d7-2ee02d1adcc6.png)

