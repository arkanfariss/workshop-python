BAB 9 – OOP DI PYTHON

Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-07

9. Classes

Classes atau kelas-kelas menyediakan sarana untuk menggabungkan data dan fungsionalitas bersama. Membuat sebuah class baru menghasilkan objek dengan type baru, memungkinkan dibuat instance baru dari tipe itu. Setiap instance dari class dapat memiliki atribut yang melekat padanya untuk mempertahankan kondisinya. Instance dari sebuah class juga dapat memiliki metode (ditentukan oleh class) untuk memodifikasi kondisinya.

9.1. Sepatah Kata Tentang Nama dan Objek

Objek memiliki individualitas, dan banyak nama (dalam berbagai lingkup) dapat terikat ke objek yang sama. Ini dikenal sebagai aliasing dalam bahasa lain.

9.2. Lingkup Python dan Namespaces

Sebuah namespace adalah pemetaan dari nama ke objek. Contoh ruang nama namespace adalah: himpunan nama bawaan (berisi fungsi seperti abs(), dan nama pengecualian bawaan), nama-nama global dalam sebuah modul; dan nama-nama lokal dalam pemanggilan fungsi. Dalam arti himpunan atribut suatu objek juga membentuk namespace.

9.2.1. Contoh Lingkup Scopes dan Ruang Nama Namespaces

Ini adalah contoh yang menunjukkan cara mereferensikan lingkup scopes dan ruang nama namespaces yang berbeda, dan bagaimana global dan nonlocal memengaruhi pengikatan variable.

![1](https://user-images.githubusercontent.com/70943455/112710748-1f1c9d00-8ef6-11eb-8916-a9b56f611f14.png)

9.3. Pandangan Pertama tentang Kelas

9.3.1. Sintaks Definisi Kelas

Definisi kelas, seperti definisi fungsi (pernyataan def) harus dieksekusi sebelum mereka memiliki efek. (Anda dapat menempatkan definisi kelas di cabang dari pernyataan if, atau di dalam suatu fungsi)

9.3.2. Objek Kelas Class Objects

Objek kelas mendukung dua jenis operasi yaitu referensi atribut dan instansiasi.

Attribute references menggunakan sintaks standar yang digunakan untuk semua referensi atribut dalam Python yaitu obj.name. Nama atribut yang valid adalah semua nama yang ada di namespace kelas saat objek kelas dibuat.

![2](https://user-images.githubusercontent.com/70943455/112710752-204dca00-8ef6-11eb-8ab2-8da91f1f4b08.png)

instantiation kelas menggunakan notasi fungsi. Hanya berpura-pura bahwa objek kelas adalah fungsi tanpa parameter yang mengembalikan instance baru dari kelas.

![3](https://user-images.githubusercontent.com/70943455/112710753-20e66080-8ef6-11eb-85c7-332e8d7af70b.png)

9.3.3. Objek Instance

Data attributes sesuai dengan "variabel instan" di Smalltalk, dan "data members" di C++. Atribut data tidak perlu dinyatakan seperti variabel lokal, mereka muncul ketika mereka pertama kali ditugaskan.

![4](https://user-images.githubusercontent.com/70943455/112710754-20e66080-8ef6-11eb-870f-ed968dc1a211.png)

Metode adalah fungsi yang "milik" suatu objek. (Dalam Python, istilah metode tidak unik untuk instance kelas: tipe objek lain dapat memiliki metode juga.

9.3.5. Variabel Kelas dan Instance

Variabel instance adalah untuk data unik untuk setiap instance dan variabel kelas adalah untuk atribut dan metode yang dibagikan oleh semua instance kelas.

![5](https://user-images.githubusercontent.com/70943455/112710755-217ef700-8ef6-11eb-86fc-5ce2e72304bd.png)

Daftar tricks dalam kode berikut tidak boleh digunakan sebagai variabel kelas karena hanya satu daftar yang akan dibagikan oleh semua Dog instance.

![6](https://user-images.githubusercontent.com/70943455/112710757-217ef700-8ef6-11eb-963d-1f331fe4c328.png)

Desain kelas yang benar harus menggunakan variabel instance

![7](https://user-images.githubusercontent.com/70943455/112710758-22178d80-8ef6-11eb-9dab-0f605bde35b2.png)

9.4. Keterangan Acak

Jika nama atribut yang sama muncul di kedua instance dan di kelas, maka pencarian atribut memprioritaskan instance

![8](https://user-images.githubusercontent.com/70943455/112710759-22b02400-8ef6-11eb-86ae-9d73a26574ee.png)

![9](https://user-images.githubusercontent.com/70943455/112710761-22b02400-8ef6-11eb-86da-72e82f42c069.png)

9.6. Variabel Private

Variabel instance "Private" yang tidak dapat diakses kecuali dari dalam suatu objek tidak ada dalam Python. Namun, ada konvensi yang diikuti oleh sebagian besar kode Python: nama diawali dengan garis bawah (misalnya _spam) harus diperlakukan sebagai bagian non-publik dari API (apakah itu fungsi, metode atau anggota data)

![10](https://user-images.githubusercontent.com/70943455/112710762-2348ba80-8ef6-11eb-8983-23102b7cdca8.png)

9.7. Barang Sisa Odds and Ends

Sepotong kode Python yang mengharapkan tipe data abstrak tertentu sering dapat dilewatkan kelas yang mengemulasi metode tipe data itu sebagai gantinya

![11](https://user-images.githubusercontent.com/70943455/112710763-2348ba80-8ef6-11eb-8dc9-25d2711e650c.png)

9.8. Iterators

Sebagian besar objek penampung container dapat dibuat perulangan menggunakan pernyataan for

![12](https://user-images.githubusercontent.com/70943455/112710764-23e15100-8ef6-11eb-9c72-cd4694fcdfce.png)

Di belakang layar, pernyataan for memanggil iter() pada objek penampung container. Fungsi mengembalikan objek iterator yang mendefinisikan metode __next__() yang mengakses elemen dalam penampung container satu per satu. Ketika tidak ada lagi elemen, __next__() memunculkan pengecualian StopIteration yang memberi tahu perulangan for untuk mengakhiri. Anda dapat memanggil metode __next__() menggunakan next() fungsi bawaan

![13](https://user-images.githubusercontent.com/70943455/112710766-2479e780-8ef6-11eb-9860-d78a1ef46dfd.png)

Mendefinisikan metode __iter__() yang mengembalikan objek dengan metode __next__(). Jika kelas mendefinisikan __next__(), maka __iter__() bisa langsung mengembalikan self

![14](https://user-images.githubusercontent.com/70943455/112710767-2479e780-8ef6-11eb-8f4c-2b6cec48f4c8.png)

9.9. Pembangkit Generator

Fitur utama generator adalah variabel lokal dan status eksekusi secara otomatis disimpan di antara pemanggilan. Ini membuat fungsi lebih mudah untuk ditulis dan jauh lebih jelas daripada pendekatan menggunakan variabel instan seperti self.index dan self.data

![15](https://user-images.githubusercontent.com/70943455/112710768-25127e00-8ef6-11eb-862e-031808b0e764.png)

9.10. Ekspresi Pembangkit Generator

Beberapa pembangkit generators sederhana dapat dikodekan secara ringkas sebagai ekspresi menggunakan sintaksis yang mirip dengan pemahaman daftar list comprehensions tetapi dengan tanda kurung bukan dengan tanda kurung siku

![16](https://user-images.githubusercontent.com/70943455/112710770-25ab1480-8ef6-11eb-9f27-fed6282ef8dc.png)

![17](https://user-images.githubusercontent.com/70943455/112710771-25ab1480-8ef6-11eb-9ba1-d43204ce9061.png)
