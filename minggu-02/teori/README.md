BAB 4

source code program python dibawah ada pada link berikut : https://github.com/arkanfrs/workshop-python/tree/master/minggu-02/src

4. Pengendali Aliran Program

4.1 perintah if

Kata kunci elif adalah kependekan dari else if. Sebuah if... elif... elif... urutan pengganti switch case.

 ![1](https://user-images.githubusercontent.com/70943455/108685516-d3598b00-7526-11eb-950a-6766c9677d63.png)
 
4.2. perintah for

For oada Python mengulang item dari urutan (daftar atau string), dalam urutan kemunculannya
 
 ![2](https://user-images.githubusercontent.com/70943455/108685520-d3f22180-7526-11eb-8551-642d191d949a.png)
 
4.3. fungsi range()

Jika Anda memang perlu mengulang urutan angka, fungsi range() akan berguna

![3](https://user-images.githubusercontent.com/70943455/108685521-d3f22180-7526-11eb-9fb8-a2b1abf68dbf.png)
 
Untuk mengulangi indeks suatu urutan, dapat dengan menggabungkan range() dan len()
 
 ![4](https://user-images.githubusercontent.com/70943455/108685523-d48ab800-7526-11eb-8c35-b7fb2ccbb09b.png)

![5](https://user-images.githubusercontent.com/70943455/108685526-d48ab800-7526-11eb-9e62-8447ec5c45f1.png)

![6](https://user-images.githubusercontent.com/70943455/108685527-d5234e80-7526-11eb-894d-e35d5fe30a68.png)
 
4.4. perintah break and continue, dan Clauses pada Loops

Break menjalankan perintah keluar dari for atau while

![7](https://user-images.githubusercontent.com/70943455/108685529-d5bbe500-7526-11eb-8e74-68c19a581e18.png)

![8](https://user-images.githubusercontent.com/70943455/108685531-d5bbe500-7526-11eb-9712-973a012cdd89.png)
 
4.5. perintah pass

Pass ini dapat digunakan ketika pernyataan diperlukan secara sintaksis tetapi program tidak memerlukan tindakan, untuk menghentikan proses ketik Ctrl+C

![9](https://user-images.githubusercontent.com/70943455/108685534-d6547b80-7526-11eb-857a-623ba8af6617.png)
 
4.6. mendefinisi fungsi

Def menjelaskan definisi fungsi. Ini harus diikuti dengan nama fungsi dan daftar parameter formal dalam tanda kurung

 ![10](https://user-images.githubusercontent.com/70943455/108685537-d6ed1200-7526-11eb-90fd-34b6d58c0cb9.png)

Definisi fungsi mengaitkan nama fungsi dengan objek fungsi dalam tabel simbol
 
 ![11](https://user-images.githubusercontent.com/70943455/108685539-d6ed1200-7526-11eb-9bee-9f70b9d7c81e.png)

4.7. menjelaskan lebih tentang fungsi

mendefinisikan fungsi dengan sejumlah variabel argumen

4.7.1. nilai argumen default

menentukan nilai default untuk satu atau lebih argument membuat fungsi yang bisa dipanggil dengan lebih sedikit
 
 ![12](https://user-images.githubusercontent.com/70943455/108685543-d81e3f00-7526-11eb-8a0d-16a05e8f32e0.png)
 
 ![13](https://user-images.githubusercontent.com/70943455/108685545-d81e3f00-7526-11eb-8380-72e011c9a121.png)

![14](https://user-images.githubusercontent.com/70943455/108685548-d8b6d580-7526-11eb-98b4-13c6b700e0d2.png)

4.7.2. argumen keyword

Fungsi juga bisa disebut menggunakan argumen kata kunci dari formulir kwarg=value
 
 ![15](https://user-images.githubusercontent.com/70943455/108685551-d8b6d580-7526-11eb-9537-91a6d4c6abc7.png)

![16](https://user-images.githubusercontent.com/70943455/108685553-d94f6c00-7526-11eb-8d78-326a46a8aae5.png)

4.7.3. contoh fungsi

contoh definisi fungsi dengan tanda / dan *

standard_arg fungsi yang paling dikenal, tidak ada batasan pada pemanggil dan argumen dapat diteruskan oleh kata kunci
 
 ![17](https://user-images.githubusercontent.com/70943455/108685554-d9e80280-7526-11eb-9574-6c03aae19add.png)
 
pos_only_args fungsi yang dibatasi hanya untuk menggunakan parameter kata kunci / dalam definisi fungsi

kwd_only_args fungsi hanya mengizinkan argumen kata kunci seperti yang ditunjukkan oleh  * dalam definisi fungsi

Dan yang terakhir menggunakan ketiga fungsi pemanggilan dalam definisi yang sama
 
 ![18](https://user-images.githubusercontent.com/70943455/108685556-d9e80280-7526-11eb-911e-d573c49d8d37.png)

![19](https://user-images.githubusercontent.com/70943455/108685557-da809900-7526-11eb-8107-82aebf20a249.png)

![20](https://user-images.githubusercontent.com/70943455/108685559-db192f80-7526-11eb-898a-6bace1660fc7.png)
 
4.7.4. arbitrasi argumen list

menentukan bahwa suatu fungsi dapat dipanggil dengan sejumlah argumen yang berubah-ubah

![21](https://user-images.githubusercontent.com/70943455/108685561-db192f80-7526-11eb-86a6-80a4d0712d9b.png)
 
4.7.5. argumen list

ketika argumen sudah ada dalam daftar tetapi perlu dibuka paketnya untuk panggilan fungsi yang memerlukan argumen terpisah
 
![22](https://user-images.githubusercontent.com/70943455/108685563-dbb1c600-7526-11eb-9ffd-c35ccb6ddbb8.png)

4.7.6. ekspresi lambda

Fungsi ini mengembalikan jumlah dari dua argumen. Fungsi lambda dapat digunakan di mana pun objek fungsi diperlukan
 
 ![23](https://user-images.githubusercontent.com/70943455/108685567-dc4a5c80-7526-11eb-8c64-eaa2db8fe7a5.png)

4.7.7. string

contoh docstring multi-baris
 
 ![24](https://user-images.githubusercontent.com/70943455/108685508-d18fc780-7526-11eb-8226-cc03ff41cd20.png)

4.7.8. fungsi anotasi

Fungsi anotasi adalah informasi metadata yang sepenuhnya opsional tentang tipe yang digunakan oleh fungsi yang ditentukan pengguna

![25](https://user-images.githubusercontent.com/70943455/108685514-d2c0f480-7526-11eb-94a7-7523d88f2d86.png)

