- Membangun Infrastruktur AWS

---------------------------------------------------------------------------------------------------------------

1.AKUN - Setiap pelanggan di AWS akan memiliki akun atau akun mereka sendiri untuk masalah itu. Jadi elemen pertama dalam arsitektur adalah AKUN

2.REGION - menjalankan aplikasi di wilayah pelanggan atau sedekat mungkin dengan wilayahnya untuk meminimalkan masalah latensi dan menangani kebijakan kepatuhan.  dapat melakukan semua ini menggunakan akun yang sama. Jadi elemen kedua adalah REGION

3.VPC - dapat sepenuhnya membangun komputasi, penyimpanan, dan jaringan dari awal di dalam VPC Anda. Lebih lanjut tentang VPC di bagian selanjutnya. Jadi elemen ketiga adalah VPC.

4.Availability Zone - AWS membuat beberapa zona di wilayah yang dikenal sebagai Availability Zone. Jadi elemen keempat dalam arsitektur adalah - Availability Zone

5.Subnet - VPC adalah seluruh jaringan besar kami, kami dapat membuat beberapa sub-jaringan berdasarkan persyaratan untuk membuat jaringan seefisien dan seaman mungkin. Jadi Subnet adalah elemen kelima dalam arsitektur.

6.Menghitung EC2 - EC2 adalah singkatan dari Elastic Compute Cloud. Ini adalah komponen komputasi inti di infra. Ini tidak lain adalah server sederhana tempat aplikasi dapat dihosting. Ada beberapa jenis EC2 yang tersedia dari AWS, setiap jenis memiliki tujuan yang sedikit berbeda. AWS menggunakan kata Instans EC2 yang merujuk ke server.

Hampir semua layanan AWS akan memiliki awalan yang disebut ELASTIC yang berarti layanan tersebut dapat diskalakan atau menyusut dalam hitungan detik.

- Jenis EC2:

Ada berbagai jenis instans EC2 yang masing-masing melayani tujuan yang sedikit berbeda. Katakanlah jika Anda meng-host server game, Anda mengharapkan banyak kecepatan jaringan daripada yang lain, dan jika Anda menerapkan beberapa algoritma ML, DL yang sangat rumit, Anda akan mengharapkan kekuatan komputasi super daripada yang lain, berdasarkan penggunaan Anda. bisa memilih jenisnya. Ini adalah jenis instans EC2 yang masing-masing dilambangkan dengan kombinasi karakter alfa-numerik yang berbeda -

Tujuan Umum - A1, T3, T3a, T2, M6g, M5, M5a, M5n, M4 . Jenis ini adalah keseimbangan komputasi, penyimpanan, dan jaringan yang tepat.
Hitung Dioptimalkan - C6g, C5, C5a, C5n, C4. Seperti namanya, terutama digunakan untuk aktivitas Komputasi Kinerja Tinggi seperti Server Game Khusus, Pemrosesan Batch Tinggi, dll.
Memori Dioptimalkan - R6g, R5, R5a, R5n, R4, X1e, X1, Memori Tinggi, z1d. Ideal untuk beban kerja yang memproses kumpulan data yang besar.
Komputasi Dipercepat - P3, P2, Inf1, G4, G3, F1 . Instans ini didukung oleh Akselerator Perangkat Keras dan cocok untuk Pembelajaran Mesin, beban kerja Pembelajaran Mendalam.
Penyimpanan Dioptimalkan - I3, I3en, D2, H1. Ideal saat mengerjakan kumpulan Data yang sangat besar yang akan membutuhkan akses baca dan tulis berurutan yang sangat tinggi seperti Data Warehousing, aktivitas Data Analytics.

7.Penyimpanan,TFS - Saya ingin mengklasifikasikan penyimpanan menjadi dua kategori - Sistem File Tradisional (TFS) dan Database

8.Database - Di Database, ada banyak layanan yang ditawarkan AWS, di antaranya -
- RDS (Layanan Database Relasional)
- DynamoDB
- Redshift

9.Jaringan - Komponen jaringan utama di akun Anda adalah sebagai berikut—
- IGW - Gerbang Internet
- Router Implisit (Virtual)
- Tabel Rute
- NACL - Daftar Kontrol Akses Jaringan
- Gateway NAT
- Grup Keamanan
- Semua komponen jaringan dalam daftar ini ada secara default saat kami membuat akun, di VPC kecuali untuk - Gateway NAT. Kami dapat menjalankan Gateway NAT atau instance NAT sesuai dengan kebutuhan. Lebih lanjut tentang NAT Gateway / Instance di bagian selanjutnya.

===============================================================================================================

[Link to ichi.pro](https://ichi.pro/id/dasar-dasar-aws-panduan-pemula-281381563635451)