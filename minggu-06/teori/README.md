BAB 8 – PENANGANAN ERROR DAN EXCEPTION

Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-06

8. Kesalahan errors dan Pengecualian exceptions

8.1. Kesalahan Sintaksis

Pengurai parser mengulangi baris yang menyinggung dan menampilkan sedikit 'arrow' yang menunjuk pada titik paling awal di baris di mana kesalahan terdeteksi

![Screenshot_1](https://user-images.githubusercontent.com/70943455/111461481-d7588180-874f-11eb-8582-bbe1ac0d7a83.png)

8.2. Pengecualian

Kesalahan yang terdeteksi selama eksekusi disebut exceptions dan pada umumnya tidak fatal. Baris terakhir dari pesan kesalahan menunjukkan apa yang terjadi. Pengecualian ada berbagai jenis yang berbeda, dan tipe dicetak sebagai bagian dari pesan: tipe dalam contoh adalah ZeroDivisionError, NameError dan TypeError.

![Screenshot_2](https://user-images.githubusercontent.com/70943455/111461485-d889ae80-874f-11eb-9fe8-76c1965152a4.png)

8.3. Menangani Pengecualian

Pernyataan try mungkin memiliki lebih dari satu klausa except, untuk menentukan penangan dari berbagai pengecualian.

Kelas dalam klausa except kompatibel dengan pengecualian jika itu adalah kelas yang sama atau kelas basisnya.

![Screenshot_3](https://user-images.githubusercontent.com/70943455/111461487-d9224500-874f-11eb-95b1-b6e62a29f5f9.png)

![Screenshot_4](https://user-images.githubusercontent.com/70943455/111461488-d9badb80-874f-11eb-92b1-f21edebf2c8b.png)

![Screenshot_5](https://user-images.githubusercontent.com/70943455/111461490-d9badb80-874f-11eb-9023-5dc014d49850.png)

![Screenshot_6](https://user-images.githubusercontent.com/70943455/111461492-da537200-874f-11eb-8dde-27d06f8dc0e4.png)

![Screenshot_7](https://user-images.githubusercontent.com/70943455/111461493-daec0880-874f-11eb-8528-e71a05320ffa.png)

![Screenshot_8](https://user-images.githubusercontent.com/70943455/111461494-daec0880-874f-11eb-9e63-889625fcd8c8.png)

![Screenshot_9](https://user-images.githubusercontent.com/70943455/111461495-db849f00-874f-11eb-8f75-e1bea160e17c.png)

8.4. Memunculkan Pengecualian

Pernyataan raise memungkinkan programmer untuk memaksa pengecualian yang ditentukan terjadi.

![Screenshot_10](https://user-images.githubusercontent.com/70943455/111461497-dc1d3580-874f-11eb-9870-d342f9475eff.png)

![Screenshot_11](https://user-images.githubusercontent.com/70943455/111461501-dc1d3580-874f-11eb-93ce-6d63dad8ecbb.png)

![Screenshot_12](https://user-images.githubusercontent.com/70943455/111461504-dcb5cc00-874f-11eb-89c6-3fa817fbb708.png)

8.5. Pengecualian yang Ditentukan Pengguna

Program dapat memberi nama pengecualian mereka sendiri dengan membuat kelas pengecualian baru, Pengecualian biasanya berasal dari kelas Exception, baik secara langsung atau tidak langsung.

![Screenshot_13](https://user-images.githubusercontent.com/70943455/111461505-dcb5cc00-874f-11eb-9490-be748ccc62e2.png)

8.6. Mendefinisikan Tindakan Pembersihan

Pernyataan try memiliki klausa opsional lain yang dimaksudkan untuk menentukan tindakan pembersihan yang harus dijalankan dalam semua keadaan. Pernyataan klausa finally akan menjalankan tugas terakhir sebelum statemen try selesai.

![Screenshot_14](https://user-images.githubusercontent.com/70943455/111461509-dd4e6280-874f-11eb-9543-c37fe0c4b7ea.png)

![Screenshot_15](https://user-images.githubusercontent.com/70943455/111461512-dde6f900-874f-11eb-8a38-3cc58fdf83fd.png)

![Screenshot_16](https://user-images.githubusercontent.com/70943455/111461514-dde6f900-874f-11eb-9d4b-87de9502c202.png)

8.7. Tindakan Pembersihan yang Sudah Ditentukan

Beberapa objek mendefinisikan tindakan pembersihan standar yang harus dilakukan ketika objek tidak lagi diperlukan, terlepas dari apakah operasi menggunakan objek berhasil atau gagal.

