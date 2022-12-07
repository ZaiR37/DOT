Quiz DOT

1) Buat RDBMS dengan Skema
- id
- title
- harga

= Masuk data host, port, username dan password database seperti yang ada pada .env
= Lakukan "Test Connection" untuk memastikan bahwa kita terhubung dengan Database.
= Buat skema baru dengan nama bebas atau gunakan skema yang ada.
= Masuk ke query lalu gunakan comamand ini untuk membuat table dengan field yang ada sepeti diatas.
CREATE TABLE `product_table` (
	`id` INT,
	`title` VARCHAR(255),
	`harga` INT,
	PRIMARY KEY (`id`)
);

= Jalankan query dan pastikan bahwa tabel telah tertambahkan dan tidak ada yang error.
= Balik ke terminal lalu jalankan "composer create-project --prefer-dist laravel/lumen ."
= Buka file ".env" nya lalu ubah ip wsl nya menurut IP WSL yang ada pada ifconfig
= Buat controller dan model pada php artisan dengan 
"php artisan make:controller UserController"
"php artisan make:model UserModel"
= locate models lalu buat model user dengan skema database pertama
= locate router/web.php
= buat route atau endpoint mengarah userController dengan metoda http get dan post
= locate htttp/controllers/UserController
= buat fungsi CRUD untuk mengecheck
= buka postman lalu masukanlah url dengan [ip vEthernet wsl:port]/[endpoint]

2. Buatlah Skema dengan MongoDB
- _id
- category

= masuklah kedalam mongodb dengan menggunakan docker exec -it mongo mongosh --username root --password p455w0rd
= masukan command "use category" untuk masuk kepada category
= buat db dengan menggunakan db.createCollection("barang")
= masukan juga data barang sebagai berikut :
category> db.barang.insert([{"id": "1", "title": "Yamaha", "harga": "100000"}, {"id": "2", "title": "Supra", "harga": "150000"}, {"id": "3", "title": "Subaru", "harga": "250000"}, {"id": "4", "title": "Kijang", "harga": "75000"}])
= cek data dengan menggunakan db.barang.find()
