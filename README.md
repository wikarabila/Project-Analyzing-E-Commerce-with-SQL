# Project Analyzing E-Commerce with SQL

## Background
Tak bisa dipungkiri bahwa mengukur performa bisnis dalam sebuah perusahaan adalah kunci untuk melacak, memantau, dan mengevaluasi keberhasilan atau kegagalan dari berbagai proses bisnis. Oleh karena itu, hal ini bertujuan untuk menganalisis performa bisnis sebuah perusahaan eCommerce dengan fokus pada metrik-metrik vital seperti pertumbuhan pelanggan, kualitas produk, dan jenis pembayaran.

## Objective
Mengumpulkan insight dari analisis dan dengan visualisasi berupa :
1.	Annual Customer Activity Growth
2.	Annual Product Category Quality
3.	Annual Payment Type Usage

 ## TASK 1: Data Preparation
Berikut adalah dataset yang digunakan: 
[https://drive.google.com/file/d/1rvMxaBnRSLV7CrKHcfMsH41U_R-XZI5N/view?usp=sharing](url)

Sebelumnya yang kita lakukan adalah Data Preparation. Dataset e-commerce terdiri dari 8 dataset yang akan berhubungan satu sama lain. Oleh karena itu, berikut ini adalah langkah-langkah mengolah data tersebut.
1.	Buat database baru beserta tabel-tabelnya untuk data yang telah disiapkan dengan memperhatikan tipe data dari setiap kolom. Menggunakan CREATE TABLE. 
2.	Impor data CSV ke dalam masing-masing tabel.
3.	Buat hubungan tabel-tabel berdasarkan skema hubungan data berikut:
![skema minpro1](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/a69e8edb-cc23-4a8c-ba6c-dc03ce702982)

4.	Membuat Entity Relationship Diagram (ERD) bisa secara manual, yaitu: Tools > ERD Tool, primary atau foreign key bisa juga diatur secara manual.
5.	Kemudian ekspor Entity Relationship Diagram (ERD) dalam bentuk gambar dengan mengatur tipe data dan memberi nama kolom-kolom antar tabel yang saling terhubung. 

![ERD e-commerce pgerd](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/6006ddfa-8277-4d28-a7d0-0ebf7c548655)

## TASK 2: Annual Customer Activity Growth

![ANALISIS TABEL Annual Customer Activity Growth](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/2a2171c4-7272-4385-bce5-53abc3003ed0)
Tabel tersebut menyajikan hasil analisis pertumbuhan aktivitas pelanggan tahunan, dari tahun 2016 - 2018, yang mencakup metrik penting seperti rata-rata pengguna aktif bulanan (MAU/Monthly Active User), total pelanggan baru, total pelanggan yang melakukan repeat order, dan rata-rata frekuensinya.
Berikut adalah insight yang didapat:
![AVG mau](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/91ac9575-7d1e-4feb-9d65-b5e3623cfbfe)
Pada tahun 2016, rata-rata MAU adalah 108, dengan total 326 pelanggan baru. Tahun berikutnya, 2017, menunjukkan peningkatan tajam dengan rata-rata MAU mencapai 3694 dan total 43708 pelanggan baru. Tren ini terus berlanjut pada tahun 2018, di mana rata-rata MAU meningkat menjadi 5338 dan jumlah pelanggan baru mencapai 52062. Pertumbuhan ini menunjukkan bahwa ada peningkatan minat oleh pelanggan baru dari tahun ke tahun.

![Cust repeat ord](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/2c059dcf-3b4e-4055-a1d3-d62165c6ced2)
Analisis repeat order menunjukkan tren menarik. Pada 2016, hanya ada 3 pelanggan yang melakukan repeat order. Jumlah ini melonjak menjadi 1256 pada 2017, menunjukkan lebih banyak pelanggan melihat nilai dalam pembelian berulang. Pada 2018, jumlahnya sedikit menurun menjadi 1167, tetapi tetap jauh lebih tinggi dibandingkan 2016.

![avg freq transaksi](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/f606e32c-9c9c-4970-8267-a8720ac4ff86)
Frekuensi rata-rata transaksi pelanggan juga menunjukkan perubahan yang positif. Pada tahun 2016, rata-rata frekuensi transaksi adalah 1.009. Tahun 2017 mengalami peningkatan menjadi 1.032, menunjukkan bahwa pelanggan mulai bertransaksi lebih sering. Namun, pada tahun 2018, terjadi sedikit penurunan dalam frekuensi ini, menjadi 1.024. Meskipun ada penurunan kecil, frekuensi ini tetap lebih tinggi dibandingkan dengan tahun 2016.

Secara keseluruhan pada task 2, data ini menunjukkan adanya pertumbuhan yang kuat dalam jumlah pelanggan baru dan aktivitas, meskipun ada beberapa fluktuasi dalam frekuensi transaksi dan repeat orders. Pertumbuhan yang signifikan dalam jumlah pelanggan baru dan MAU mencerminkan peningkatan kesadaran dan penerimaan layanan oleh pelanggan.




