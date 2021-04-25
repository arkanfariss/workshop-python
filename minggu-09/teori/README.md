BAB 12 – Virtual Environment dan Package Manager

Conda

Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-09

12. Lingkungan dan Paket Virtual

12.1. Pengantar

Aplikasi Python akan sering menggunakan paket dan modul yang tidak datang sebagai bagian dari pustaka standar. Aplikasi kadang-kadang membutuhkan versi pustaka tertentu, karena aplikasi mungkin mensyaratkan bug tertentu telah diperbaiki atau aplikasi dapat ditulis menggunakan versi usang dari antarmuka pustaka.

12.2. Menciptakan Lingkungan Virtual

Modul yang digunakan untuk membuat dan mengelola lingkungan virtual disebut venv. venv biasanya akan menginstal versi Python terbaru yang dimiliki.

![1](https://user-images.githubusercontent.com/70943455/116000133-3051ea00-a619-11eb-9136-17990a74ef34.png)

![2](https://user-images.githubusercontent.com/70943455/116000135-321bad80-a619-11eb-92bb-35bb0554435e.png)

12.3. Mengelola Paket dengan pip

pip dapat menginstal, mengupgrade, dan menghapus. Secara default pip akan menginstal paket dari Python Package Index

pip juga dapat menginstal versi spesifik suatu paket dengan memberikan nama paket diikuti dengan == dan nomor versi

![3](https://user-images.githubusercontent.com/70943455/116000136-32b44400-a619-11eb-8c70-84268f2074e2.png)

menjalankan pip install --upgrade untuk meningkatkan paket ke versi terbaru

![4](https://user-images.githubusercontent.com/70943455/116000137-334cda80-a619-11eb-9538-881a48ffe8da.png)

pip uninstall diikuti oleh satu atau beberapa nama paket akan menghapus paket-paket dari lingkungan virtual

pip show akan menampilkan informasi tentang paket tertentu

![5](https://user-images.githubusercontent.com/70943455/116000140-33e57100-a619-11eb-92bc-1c8a54cbef8a.png)

pip list akan menampilkan semua paket yang diinstal di lingkungan virtual

![6](https://user-images.githubusercontent.com/70943455/116000141-33e57100-a619-11eb-8375-904a43afa971.png)

pip freeze akan menghasilkan daftar yang sama dari paket yang diinstal, tetapi keluarannya menggunakan format yang diharapkan oleh pip install

![7](https://user-images.githubusercontent.com/70943455/116000142-347e0780-a619-11eb-900c-6f2d600d8ad1.png)

requirements.txt kemudian dapat dikirimkan atau commit ke sistem kontrol versi dan dikirim sebagai bagian dari aplikasi. Pengguna kemudian dapat menginstal semua paket yang diperlukan dengan install –r

![8](https://user-images.githubusercontent.com/70943455/116000144-35169e00-a619-11eb-8356-b452ab462704.png)

Conda

Mengelola conda

Verifikasi bahwa conda diinstal dan berjalan di sistem

![9](https://user-images.githubusercontent.com/70943455/116000145-35af3480-a619-11eb-8c50-649be33442a2.png)

Perbarui conda ke versi saat ini

![10](https://user-images.githubusercontent.com/70943455/116000146-35af3480-a619-11eb-92af-187d5b0f9e95.png)

Mengelola lingkungan

Buat lingkungan baru dan instal paket di dalamnya

![11](https://user-images.githubusercontent.com/70943455/116000148-3647cb00-a619-11eb-8730-119ca3992702.png)

Untuk menggunakan, atau "activate" lingkungan baru

![12](https://user-images.githubusercontent.com/70943455/116000149-36e06180-a619-11eb-8e90-a4796ef04f67.png)

Untuk melihat daftar semua lingkungan

![13](https://user-images.githubusercontent.com/70943455/116000150-3778f800-a619-11eb-9d51-7882deebe407.png)

Ubah lingkungan Anda saat ini kembali ke default

![14](https://user-images.githubusercontent.com/70943455/116000151-3778f800-a619-11eb-8744-5594f303ae1e.png)

Mengelola Python

Buat lingkungan baru bernama "snakes" yang berisi Python 3.5

![15](https://user-images.githubusercontent.com/70943455/116000152-38118e80-a619-11eb-83d7-dc6910a830bc.png)

Aktifkan lingkungan baru dan verifikasi bahwa lingkungan snakes telah ditambahkan dan aktif

![16](https://user-images.githubusercontent.com/70943455/116000153-38aa2500-a619-11eb-9cd2-89d8f1b634dc.png)

Verifikasi versi Python mana yang ada di lingkungan Anda saat ini

![17](https://user-images.githubusercontent.com/70943455/116000154-3942bb80-a619-11eb-9498-2cc716f681e3.png)

Nonaktifkan lingkungan ular dan kembali ke lingkungan default

![18](https://user-images.githubusercontent.com/70943455/116000155-3942bb80-a619-11eb-8c75-d7ee72191f02.png)

Mengelola paket

Untuk menemukan paket yang telah diinstal, aktifkan lingkungan yang ingin dicari

![19](https://user-images.githubusercontent.com/70943455/116000156-39db5200-a619-11eb-8f4f-0ef0e43e6063.png)

Periksa apakah paket yang belum diinstal bernama "beautifulsoup4" tersedia dari gudang Anaconda (harus terhubung ke Internet)

![20](https://user-images.githubusercontent.com/70943455/116000158-3a73e880-a619-11eb-9c8c-bacf3b056a57.png)

Instal paket beautifulsoup4 ke lingkungan saat ini

![21](https://user-images.githubusercontent.com/70943455/116000161-3b0c7f00-a619-11eb-8a44-13213a2a4610.png)

Periksa untuk melihat apakah program yang baru diinstal ada di lingkungan ini

![22](https://user-images.githubusercontent.com/70943455/116000162-3b0c7f00-a619-11eb-94e7-13bcd149680e.png)
