# Lab11Web

Praktikum 11: PHP Framework (Codeigniter)

Buatlah folder baru dengan nama “lab11_php_ci”

![image](https://user-images.githubusercontent.com/56398506/122625772-0117a080-d0d1-11eb-96e7-c8dc66d34377.png)

Sebelum memulai menggunakan Framework Codeigniter, perlu dilakukan konfigurasi pada webserver. Beberapa ekstensi PHP perlu diaktifkan untuk kebutuhan pengembangan Codeigniter 4. Untuk mengaktifkan ekstentsi tersebut, melalu XAMPP Control Panel, pada bagian Apache klik Config -> PHP.ini

![image](https://user-images.githubusercontent.com/56398506/122625793-14c30700-d0d1-11eb-8d1d-f3aca7100509.png)

Pada bagian extention, hilangkan tanda ; (titik koma) pada ekstensi yang akan diaktifkan. Kemudian simpan kembali filenya dan restart Apache web server.

![image](https://user-images.githubusercontent.com/56398506/122625808-39b77a00-d0d1-11eb-8e99-5ac2c95dff16.png)

Instalasi Codeigniter 4

Untuk melakukan instalasi Codeigniter 4 dapat dilakukan dengan dua cara, yaitu cara manual dan menggunakan composer. Pada praktikum ini kita menggunakan cara manual.

![image](https://user-images.githubusercontent.com/56398506/122625833-64093780-d0d1-11eb-8109-cf7abd10ed6b.png)

Menjalankan CLI (Command Line Interface)

Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah: ( php spark )

![image](https://user-images.githubusercontent.com/56398506/122625864-9024b880-d0d1-11eb-8512-d3c734d5eca2.png)

Mengaktifkan Mode Debugging

Ketika terjadi error pada aplikasi akan ditampilkan pesan kesalahan seperti berikut.

![image](https://user-images.githubusercontent.com/56398506/122625881-a763a600-d0d1-11eb-96cd-a29b21a1141f.png)

Ubah nama file env menjadi .env kemudian buka file tersebut dan ubah nilai variable CI_ENVIRINMENT menjadi development

![image](https://user-images.githubusercontent.com/56398506/122625896-bea29380-d0d1-11eb-8d5c-832cc610c338.png)

Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.

![image](https://user-images.githubusercontent.com/56398506/122625930-ce21dc80-d0d1-11eb-9b74-e8d7a8cdca21.png)

Routing dan Controller

Router terletak pada file app/config/Routes.php

![image](https://user-images.githubusercontent.com/56398506/122625940-ded25280-d0d1-11eb-86ba-0124cd030c06.png)

buka CLI dan jalankan perintah berikut.
yaitu php spark

![image](https://user-images.githubusercontent.com/56398506/122625947-edb90500-d0d1-11eb-953d-66718b4aaf0b.png)

Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url http://localhost:8080/about 

![image](https://user-images.githubusercontent.com/56398506/122625957-fc072100-d0d1-11eb-9ed2-c7017a65da62.png)

Membuat Controller

Selanjutnya adalah membuat Controller Page. Buat file baru dengan nama page.php pada direktori Controller kemudian isi kodenya seperti berikut.

![image](https://user-images.githubusercontent.com/56398506/122625967-09241000-d0d2-11eb-986e-77593ff03797.png)

Selanjutnya refresh Kembali browser,

![image](https://user-images.githubusercontent.com/56398506/122625975-15a86880-d0d2-11eb-829d-fcab3a47bfce.png)

Tambahkan method baru pada Controller Page seperti berikut.

![image](https://user-images.githubusercontent.com/56398506/122625986-26f17500-d0d2-11eb-9c3e-d0fa535c5dbe.png)

Method ini belum ada pada routing, sehingga cara mengaksesnya dengan menggunakan alamat: http://localhost:8080/page/tos

![image](https://user-images.githubusercontent.com/56398506/122626001-353f9100-d0d2-11eb-97fe-b133feafa3f9.png)

Buat file css pada direktori public dengan nama style.css

![image](https://user-images.githubusercontent.com/56398506/122626019-45577080-d0d2-11eb-9e6c-85384e0232bf.png)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php

![image](https://user-images.githubusercontent.com/56398506/122626033-53a58c80-d0d2-11eb-9001-7c46057bdc0f.png)

footer.php

![image](https://user-images.githubusercontent.com/56398506/122626040-5e602180-d0d2-11eb-9fe5-65572d3418f9.png)

Kemudian ubah file app/view/about.php seperti berikut

![image](https://user-images.githubusercontent.com/56398506/122626047-68822000-d0d2-11eb-84d7-5832fcc90dd1.png)

selanjutnya refresh tampilan tersebut:

![image](https://user-images.githubusercontent.com/56398506/122626054-75067880-d0d2-11eb-9d59-9e00a0701c6b.png)


