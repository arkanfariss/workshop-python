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

15

10.12. Dilengkapi Baterai

Python memiliki filosofi “dilengkapi baterai”. Ini paling baik dilihat melalui kemampuan yang canggih dan kuat robust dengan dukungan paket-paket yang lebih besar.