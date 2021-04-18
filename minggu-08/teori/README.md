BAB 10 dan 11 – PUSTAKA STANDAR

Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-08

10. Tur Singkat Pustaka Standar

10.1. Antarmuka Sistem Operasi

Modul os menyediakan puluhan fungsi untuk berinteraksi dengan sistem operasi
 
![Screenshot_1](https://user-images.githubusercontent.com/70943455/115139214-dcfcfc00-a05a-11eb-9d91-1e4afedf384e.png)

Fungsi bawaan dir() dan help() berguna sebagai alat bantu interaktif untuk bekerja dengan modul besar seperti os

![Screenshot_2](https://user-images.githubusercontent.com/70943455/115139215-de2e2900-a05a-11eb-84bc-760f3dfaeb22.png)

![Screenshot_3](https://user-images.githubusercontent.com/70943455/115139216-dec6bf80-a05a-11eb-9c71-b34cf2de3c46.png)
 
10.2. Berkas Wildcard

Modul glob menyediakan fungsi untuk membuat daftar berkas dari pencarian wildcard di direktori

![Screenshot_4](https://user-images.githubusercontent.com/70943455/115139217-df5f5600-a05a-11eb-94ee-8f134f9d0218.png)

10.3. Baris Perintah Berargumen

Skrip utilitas umum seringkali perlu memproses argumen baris perintah. Argumen-argumen ini disimpan dalam atribut argv dari modul sys sebagai daftar

![Screenshot_5](https://user-images.githubusercontent.com/70943455/115139218-dff7ec80-a05a-11eb-987f-e5bd3cced5dc.png)

10.4. Pengalihan Output Kesalahan dan Pengakhiran Program

Modul sys juga memiliki atribut untuk stdin, stdout, dan stderr. Yang terakhir berguna untuk mengirimkan peringatan dan pesan kesalahan untuk membuatnya terlihat bahkan ketika stdout telah dialihkan

![Screenshot_6](https://user-images.githubusercontent.com/70943455/115139219-e0908300-a05a-11eb-8704-e89d8043eed7.png)

10.5. Pencocokan Pola String

Modul re menyediakan alat ekspresi reguler untuk pemrosesan string lanjutan. Untuk pencocokan dan manipulasi yang kompleks, ekspresi reguler menawarkan solusi yang ringkas dan dioptimalkan

![Screenshot_7](https://user-images.githubusercontent.com/70943455/115139220-e1291980-a05a-11eb-90de-e1e806aeddba.png)

![Screenshot_8](https://user-images.githubusercontent.com/70943455/115139221-e1291980-a05a-11eb-9973-66d64645a8b2.png)

10.6. Matematika

Modul math memberikan akses ke fungsi-fungsi pustaka C yang mendasari untuk matematika angka pecahan floating point

![Screenshot_9](https://user-images.githubusercontent.com/70943455/115139222-e1c1b000-a05a-11eb-8b9a-8a3e64d44077.png)

Modul random menyediakan alat untuk membuat pilihan acak

![Screenshot_10](https://user-images.githubusercontent.com/70943455/115139223-e25a4680-a05a-11eb-9678-521a1060b931.png)

Modul statistics menghitung sifat statistik dasar (rata-rata, median, varian, dll.) dari data numerik

![Screenshot_11](https://user-images.githubusercontent.com/70943455/115139224-e2f2dd00-a05a-11eb-9c50-8a89147dafd1.png)

10.7. Akses Internet

Modul untuk mengakses internet dan memproses protokol internet. Dua yang paling sederhana adalah urllib.request untuk mengambil data dari URL dan smtplib untuk mengirim email

10.8. Tanggal dan Waktu

Modul datetime menyediakan kelas untuk memanipulasi tanggal dan waktu dengan cara yang sederhana dan kompleks

![Screenshot_12](https://user-images.githubusercontent.com/70943455/115139225-e38b7380-a05a-11eb-8110-5fb5d3546cd9.png)

10.9. Kompresi Data

Format pengarsipan dan kompresi data umum didukung langsung oleh modul-modul yang ada antara lain :mod: zlib, gzip, bz2, lzma, zipfile dan tarfile

![Screenshot_13](https://user-images.githubusercontent.com/70943455/115139226-e38b7380-a05a-11eb-976a-ce15c53ee960.png)

10.10. Pengukuran Kinerja

Modul profile dan pstats menyediakan alat untuk mengidentifikasi bagian kritis waktu dalam blok kode yang lebih besar

![Screenshot_14](https://user-images.githubusercontent.com/70943455/115139227-e4240a00-a05a-11eb-8215-4d72decac0ba.png)

10.11. Kontrol Kualitas

Modul doctest untuk memastikan kode tetap benar untuk dokumentasi

![Screenshot_15](https://user-images.githubusercontent.com/70943455/115139760-fd7a8580-a05d-11eb-801f-bacdd650a151.png)

10.12. Dilengkapi Baterai

Python memiliki filosofi “dilengkapi baterai”. Ini paling baik dilihat melalui kemampuan yang canggih dan kuat robust dengan dukungan paket-paket yang lebih besar.

.....

11. Tur Singkat Pustaka Standar --- Bagian II

11.1. Pemformatan Output

Modul reprlib menyediakan versi repr() yang disesuaikan untuk tampilan yang disingkat dari wadah containers yang besar atau sangat bersarang

![Screenshot_16](https://user-images.githubusercontent.com/70943455/115140545-1127eb00-a062-11eb-8946-5f164e500b5d.png)

Modul pprint menawarkan kontrol yang lebih canggih atas pencetakan objek bawaan dan yang ditentukan pengguna dengan cara yang dapat dibaca oleh interpreter

![Screenshot_17](https://user-images.githubusercontent.com/70943455/115140547-12f1ae80-a062-11eb-8936-c07b749ae9e4.png)

Modul textwrap memformat paragraf teks agar sesuai dengan lebar layar yang diberikan

![Screenshot_18](https://user-images.githubusercontent.com/70943455/115140551-138a4500-a062-11eb-9a5d-f345357ebbec.png)

Modul locale mengakses basis data format data kultur khusus. Atribut pengelompokan fungsi format lokal locale menyediakan cara langsung memformat angka dengan pemisah grup

![Screenshot_19](https://user-images.githubusercontent.com/70943455/115140552-138a4500-a062-11eb-8d9f-1aa8d5de2490.png)

11.2. Templating

Modul string menyertakan kelas serbaguna Template dengan sintaks yang disederhanakan yang cocok untuk diedit oleh pengguna

![Screenshot_20](https://user-images.githubusercontent.com/70943455/115140553-1422db80-a062-11eb-8089-084392ed8f21.png)

Metode substitute() memunculkan KeyError saat placeholder tidak disertakan dalam dictionary atau argumen kata kunci keyword argument

![Screenshot_21](https://user-images.githubusercontent.com/70943455/115140554-14bb7200-a062-11eb-9614-1c7d7a0c8aff.png)

Utilitas penggantian nama batch untuk browser foto dapat memilih untuk menggunakan tanda persen untuk penampung seperti tanggal saat ini, nomor urut gambar, atau format berkas

![Screenshot_22](https://user-images.githubusercontent.com/70943455/115140556-15540880-a062-11eb-8810-13444c1c0aca.png)

11.3. Bekerja dengan Tata Letak Rekam Data Biner

Modul struct menyediakan pack() dan unpack() berfungsi untuk bekerja dengan format rekaman biner yang memiliki panjang variabel

11.4. Multi-threading

Threading adalah teknik untuk memisahkan tugas yang tidak tergantung secara berurutan. Utas threads dapat digunakan untuk meningkatkan responsif aplikasi yang menerima masukan pengguna saat tugas lain beroperasi di latar belakang

![Screenshot_23](https://user-images.githubusercontent.com/70943455/115140557-15540880-a062-11eb-9999-47271769af7a.png)

![Screenshot_24](https://user-images.githubusercontent.com/70943455/115140559-15ec9f00-a062-11eb-8ddb-9aa2fc8b84c6.png)

11.5. Pencatatan

Modul logging menawarkan sistem pencatatan logging yang lengkap dan fleksibel. Paling sederhana, catatan log pesan dikirim ke berkas atau ke sys.stderr

![Screenshot_25](https://user-images.githubusercontent.com/70943455/115140560-16853580-a062-11eb-9f9a-91beca5914c9.png)

11.6. Referensi yang Lemah

Modul weakref menyediakan alat untuk melacak objek tanpa membuat referensi. Ketika objek tidak lagi diperlukan, itu secara otomatis dihapus dari tabel weakref dan panggilan balik callback dipicu untuk weakref

![Screenshot_26](https://user-images.githubusercontent.com/70943455/115140561-171dcc00-a062-11eb-9228-90e019d1d012.png)

11.7. Alat untuk Bekerja dengan Daftar Lists

Modul array menyediakan objek array() yang seperti daftar list dimana hanya menyimpan data homogen dan menyimpannya dengan lebih kompak

![Screenshot_27](https://user-images.githubusercontent.com/70943455/115140562-171dcc00-a062-11eb-8e3f-fc29cfeab1be.png)

Modul collections menyediakan objek deque() yang seperti daftar list dengan tambahan yang lebih cepat dan muncul dari sisi kiri tetapi pencarian yang lebih lambat di tengah

![Screenshot_28](https://user-images.githubusercontent.com/70943455/115140563-17b66280-a062-11eb-998f-f11c9a3b2665.png)

Modul bisect dengan fungsi untuk memanipulasi daftar list yang diurutkan

![Screenshot_29](https://user-images.githubusercontent.com/70943455/115140564-184ef900-a062-11eb-887f-740b2e48c303.png)

Modul heapq menyediakan fungsi untuk mengimplementasikan heaps berdasarkan daftar list reguler

![Screenshot_30](https://user-images.githubusercontent.com/70943455/115140566-18e78f80-a062-11eb-81f5-1f703f76f11c.png)

11.8. Aritmatika Pecahan Floating Point Desimal

Hasil Decimal menjaga akhiran trailing nol, secara otomatis menyimpulkan empat tempat signifikansi dari multiplicands dengan dua tempat signifikansi

![Screenshot_31](https://user-images.githubusercontent.com/70943455/115140567-18e78f80-a062-11eb-85eb-ae1dd47394b5.png)

Representasi yang tepat memungkinkan kelas Decimal untuk melakukan perhitungan modulo dan tes persamaan yang tidak cocok untuk angka pecahan floating point biner

![Screenshot_32](https://user-images.githubusercontent.com/70943455/115140568-19802600-a062-11eb-8076-6a099c464a5c.png)

Modul decimal menyediakan aritmatika dengan ketelitian sebanyak yang dibutuhkan

![Screenshot_33](https://user-images.githubusercontent.com/70943455/115140569-1a18bc80-a062-11eb-9a75-2363d79a7104.png)
