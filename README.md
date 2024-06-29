# Project Analyzing E-Commerce with SQL

## Background
Tak bisa dipungkiri bahwa mengukur performa bisnis dalam sebuah perusahaan adalah kunci untuk melacak, memantau, dan mengevaluasi keberhasilan atau kegagalan dari berbagai proses bisnis. Oleh karena itu, hal ini bertujuan untuk menganalisis performa bisnis sebuah perusahaan eCommerce dengan fokus pada metrik-metrik vital seperti pertumbuhan pelanggan, kualitas produk, dan jenis pembayaran.

## Objective
Mengumpulkan insight dari analisis dan dengan visualisasi berupa :
1.	Annual Customer Activity Growth
2.	Annual Product Category Quality
3.	Annual Payment Type Usage

## Tools : SQL & Microsoft Excel

 ## TASK 1: Data Preparation
Berikut adalah dataset yang digunakan: 
[https://drive.google.com/file/d/1rvMxaBnRSLV7CrKHcfMsH41U_R-XZI5N/view?usp=sharing](url)

Sebelumnya yang kita lakukan adalah Data Preparation. Dataset e-commerce terdiri dari 8 dataset yang akan berhubungan satu sama lain. Oleh karena itu, berikut ini adalah langkah-langkah mengolah data tersebut.
1.	Buat database baru beserta tabel-tabelnya untuk data yang telah disiapkan dengan memperhatikan tipe data dari setiap kolom. Menggunakan CREATE TABLE. Query: [QUERY TASK 1 DATA PREPARATION.txt](https://github.com/user-attachments/files/16040368/QUERY.TASK.1.DATA.PREPARATION.txt)
2.	Impor data CSV ke dalam masing-masing tabel.
3.	Buat hubungan tabel-tabel berdasarkan skema hubungan data berikut:
![skema minpro1](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/a69e8edb-cc23-4a8c-ba6c-dc03ce702982)

4.	Membuat Entity Relationship Diagram (ERD) bisa secara manual, yaitu: Tools > ERD Tool, primary atau foreign key bisa juga diatur secara manual.
5.	Kemudian ekspor Entity Relationship Diagram (ERD) dalam bentuk gambar dengan mengatur tipe data dan memberi nama kolom-kolom antar tabel yang saling terhubung. 

![ERD e-commerce pgerd](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/6006ddfa-8277-4d28-a7d0-0ebf7c548655)

## TASK 2: Annual Customer Activity Growth

Query: [QUERY TASK 2 Annual Customer Activi.txt](https://github.com/user-attachments/files/16040400/QUERY.TASK.2.Annual.Customer.Activi.txt)

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

## TASK 3: Annual Product Category Quality

Query: [QUERY TASK 3 Annual Product Categor.txt](https://github.com/user-attachments/files/16040420/QUERY.TASK.3.Annual.Product.Categor.txt)

![tabel analisis Annual Product Category Quality](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/8b248d8b-2de3-40e9-bc68-b62c98329b60)
Tabel tersebut menyajikan hasil analisis kualitas kategori produk dari tahun 2016 - 2018, dengan fokus pada total pendapatan, pendapatan dari produk teratas, dan jumlah pembatalan produk teratas.

![revenue per year](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/ea55a0f2-e4f9-4511-8df5-741dcef0ea6a)
Pada tahun 2016, total pendapatan perusahaan mencapai 46,653.74. Pendapatan ini meningkat tajam pada tahun 2017 menjadi 6,921,535.24, menunjukkan pertumbuhan yang luar biasa. Tahun 2018 terus menunjukkan tren positif dengan total pendapatan yang lebih tinggi lagi, mencapai 8,451,584.77. Pertumbuhan yang signifikan dari tahun ke tahun ini menunjukkan adanya peningkatan yang kuat dalam aktivitas bisnis dan penerimaan pasar terhadap produk perusahaan.

![top revenue product](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/f987255e-3976-45a1-9215-fae548ba3efb)
Produk yang memberikan pendapatan tertinggi bervariasi setiap tahunnya. Pada tahun 2016, kategori produk "furniture_decor" memberikan kontribusi terbesar dengan pendapatan sebesar 6,899.35. Tahun 2017 melihat perubahan, di mana kategori "bed_bath_table" menjadi produk teratas dengan pendapatan sebesar 580,949.20. Pada tahun 2018, kategori "health_beauty" mencatat pendapatan tertinggi dengan angka 866,810.34. Variasi ini menunjukkan perubahan preferensi pelanggan terhadap kategori produk tertentu dari tahun ke tahun.

![Top canceled product](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/67f93fed-37c4-421c-adf9-cb6a61d8aef0)
Jumlah produk teratas yang dibatalkan juga bervariasi. Pada tahun 2016, kategori "toys" mengalami 3 pembatalan, sementara pada tahun 2017, kategori "sports_leisure" mencatat 25 pembatalan, yang merupakan angka tertinggi dalam periode tersebut. Tahun 2018 melihat kategori "health_beauty" mengalami 27 pembatalan, yang merupakan jumlah tertinggi untuk tahun itu. Meskipun jumlah pembatalan meningkat seiring dengan total pendapatan yang meningkat, ini mungkin menunjukkan tantangan dalam menjaga kualitas dan kepuasan pelanggan untuk produk-produk populer.

Secara keseluruhan, data ini menunjukkan pertumbuhan yang kuat dalam pendapatan perusahaan dari tahun ke tahun, dengan kategori produk teratas yang bervariasi. Namun, peningkatan jumlah pembatalan produk teratas juga menandakan perlunya peningkatan dalam pengelolaan kualitas dan kepuasan pelanggan.

## TASK 4: Annual Payment Type Usage

Query: [TASK 4 Annual Payment Type Usage.txt](https://github.com/user-attachments/files/16040524/TASK.4.Annual.Payment.Type.Usage.txt)

![tabel ananlsiis Annual Payment Type Usage](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/ae40dbb5-4a8e-4c4a-9d57-27680c879fb0)
Tabel tersebut menyajikan hasil analisis penggunaan berbagai jenis metode pembayaran dari tahun 2016 hingga 2018, mencakup penggunaan kartu kredit, boleto, voucher, kartu debit, dan metode pembayaran yang tidak terdefinisikan. Data ini memberikan gambaran tentang preferensi pelanggan dalam memilih metode pembayaran dan bagaimana tren ini berkembang selama periode yang dianalisis.

![Grafik type payment](https://github.com/wikarabila/Project-Analyzing-E-Commerce-with-SQL/assets/160766477/6c3b3f57-5a12-4173-9a1f-1a4b1a33b340)
Berdasarkan data dari tahun 2016 hingga 2018, kartu kredit adalah metode pembayaran yang paling dominan dan terus meningkat, dari 258 transaksi pada 2016, menjadi 34,568 pada 2017, dan 41,969 pada 2018. Penggunaan boleto juga meningkat dari 63 transaksi pada 2016, menjadi 9,508 pada 2017, dan 10,213 pada 2018. Voucher digunakan 23 kali pada 2016, meningkat menjadi 3,027 pada 2017, namun sedikit menurun menjadi 2,725 pada 2018. Penggunaan kartu debit meningkat secara konsisten dari 2 transaksi pada 2016, menjadi 422 pada 2017, dan 1,105 pada 2018. Metode pembayaran tidak terdefinisikan hanya muncul pada 2018 dengan 3 transaksi. Secara keseluruhan, kartu kredit adalah metode yang paling disukai, dengan penggunaan yang terus meningkat setiap tahun.

## SUMMARY
### Data Preparation
Data disusun dari aktivitas pelanggan, kualitas kategori produk, dan penggunaan jenis pembayaran untuk analisis strategis.
### Annual Customer Activity Growth
Peningkatan signifikan terlihat dalam jumlah pengguna aktif bulanan, pelanggan baru, dan pelanggan yang melakukan repeat order dari tahun ke tahun. Frekuensi rata-rata pesanan juga menunjukkan tren peningkatan yang stabil.
### Annual Product Category Quality
Pendapatan perusahaan menunjukkan pertumbuhan yang kuat setiap tahun. Kategori produk yang memberikan pendapatan tertinggi bervariasi tiap tahun, menunjukkan perubahan preferensi pelanggan. Kategori produk yang paling banyak dibatalkan juga bervariasi, mengindikasikan area yang memerlukan perhatian lebih dalam pengelolaan kualitas.
### Annual Payment Type Usage
Kartu kredit tetap menjadi metode pembayaran yang paling dominan dan meningkat setiap tahun. Metode pembayaran lainnya seperti boleto, voucher, dan kartu debit juga menunjukkan peningkatan, meskipun dalam jumlah yang lebih kecil. Metode pembayaran yang tidak terdefinisikan sangat sedikit digunakan.

