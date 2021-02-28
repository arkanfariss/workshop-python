BAB 5

Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-03

5. Data Structures

5.1. More on Lists

list.append (x)

Tambahkan item ke akhir daftar list.

list.extend (iterable)

Perpanjang daftar list dengan menambahkan semua item dari iterable

list.insert (i, x)

Masukkan item pada posisi tertentu. Argumen pertama adalah indeks elemen sebelum memasukkan, jadi a.insert (0, x) memasukkan di bagian depan daftar list, dan a.insert (len(a), x) sama dengan a.append(x).

list.remove (x)

Hapus item pertama dari daftar list yang nilainya sama dengan x. Ini memunculkan ValueError jika tidak ada item seperti itu.

list.pop ([i])

Hapus item pada posisi yang diberikan dalam daftar, dan kembalikan.

list.clear ()

Hapus semua item dari daftar list.

list.index (x[,start[,end]])

Kembalikan indeks berbasis nol dalam daftar item pertama yang nilainya sama dengan x. Menimbulkan ValueError jika tidak ada item seperti itu..

list.count (x)

Kembalikan berapa kali x muncul dalam daftar.

list.sort (*, key=None, reverse=False)

Urutkan item daftar di tempat (argumen dapat digunakan untuk mengurutkan ubah suaian customization, lihat sorted() untuk penjelasannya).

list.reverse ()

Membalikan elemen daftar list di tempatnya.

list.copy ()

Kembalikan salinan daftar list yang dangkal.

 ![Screenshot_1](https://user-images.githubusercontent.com/70943455/109427566-94936b80-7a25-11eb-84b1-2749e56fca0d.png)

5.1.1. Using Lists as Stacks

Metode list sangat mudah untuk menggunakan list sebagai tumpukan stack, di mana elemen terakhir yang ditambahkan adalah elemen pertama yang diambil ("last-in, first-out").

![Screenshot_2](https://user-images.githubusercontent.com/70943455/109427568-95c49880-7a25-11eb-88f5-9ec3565e3e60.png)

5.1.2. Using Lists as Queues

Menggunakan list sebagai antrian, di mana elemen pertama yang ditambahkan adalah elemen pertama yang diambil ("first-in, first-out")

 ![Screenshot_3](https://user-images.githubusercontent.com/70943455/109427570-965d2f00-7a25-11eb-9c83-b9cc7521f623.png)

5.1.3. List Comprehensions

list comprehensions adalah cara singkat untuk membuat list

 ![Screenshot_4](https://user-images.githubusercontent.com/70943455/109427571-965d2f00-7a25-11eb-9b15-fcb55e2150af.png)

Pemahaman daftar list comprehension terdiri dari tanda kurung yang berisi ekspresi diikuti oleh klausa for, lalu nol atau lebih klausa for atau if.

 ![Screenshot_5](https://user-images.githubusercontent.com/70943455/109427572-96f5c580-7a25-11eb-89cd-3adfa01366b1.png)

 ![Screenshot_6](https://user-images.githubusercontent.com/70943455/109427573-978e5c00-7a25-11eb-8d59-b97d28fb6adf.png)

5.1.4. Nested List Comprehensions

matriks 3x4 berikut yang diimplementasikan sebagai daftar list 3 dari daftar list panjang 4

 ![Screenshot_6_1](https://user-images.githubusercontent.com/70943455/109427575-978e5c00-7a25-11eb-9ba3-aec163987e66.png)

listcomp bersarang dievaluasi dalam konteks for yang mengikutinya

 ![Screenshot_6_2](https://user-images.githubusercontent.com/70943455/109427576-9826f280-7a25-11eb-8be0-196bc6f2e01b.png)

 ![Screenshot_7](https://user-images.githubusercontent.com/70943455/109427577-98bf8900-7a25-11eb-976a-4968243217ac.png)

5.2. The del statement

menghapus item dari daftar yang diberikan indeksnya

 ![Screenshot_8](https://user-images.githubusercontent.com/70943455/109427579-98bf8900-7a25-11eb-9243-556845835957.png)

5.3. Tuples and Sequences

Tupel adalah urutan, seperti daftar. Perbedaan utama antara tupel dan daftarnya adalah bahwa tupel tidak dapat diubah tidak seperti List Python. Tupel menggunakan tanda kurung, sedangkan List Python menggunakan tanda kurung siku.

 ![Screenshot_9](https://user-images.githubusercontent.com/70943455/109427581-99581f80-7a25-11eb-87a2-954f9806e104.png)

 ![Screenshot_10](https://user-images.githubusercontent.com/70943455/109427583-99f0b600-7a25-11eb-9540-fdb75ebb1acc.png)

5.4. Sets

Python juga menyertakan tipe data untuk sets. Himpunan atau Set adalah koleksi yang tidak terurut tanpa elemen duplikat. fungsi set() dapat digunakan untuk membuat himpunan

 ![Screenshot_11](https://user-images.githubusercontent.com/70943455/109427584-99f0b600-7a25-11eb-80b2-25833208403e.png)

 ![Screenshot_12](https://user-images.githubusercontent.com/70943455/109427585-9a894c80-7a25-11eb-9c64-cac41970901c.png)

5.5. Dictionaries

dictionary diindeks oleh keys, yang dapat berupa jenis apa pun yang tidak dapat diubah immutable type; string dan angka selalu bisa menjadi kunci key

 ![Screenshot_13](https://user-images.githubusercontent.com/70943455/109427586-9b21e300-7a25-11eb-96e5-420c15c10cc3.png)

 ![Screenshot_14](https://user-images.githubusercontent.com/70943455/109427587-9b21e300-7a25-11eb-876e-7aacfb6b073c.png)

![Screenshot_14_1](https://user-images.githubusercontent.com/70943455/109427808-b04b4180-7a26-11eb-9ccb-7a512150cd8d.png)

5.6. Looping Techniques

Saat mengulang kamus dictionaries, kunci key dan nilai value terkait dapat diambil pada saat yang sama menggunakan metode items()

Saat mengulang melalui urutan, indeks posisi dan nilai terkait dapat diambil pada saat yang sama menggunakan fungsi enumerate()

Untuk mengulang dua urutan atau lebih secara bersamaan, entri dapat dipasangkan dengan fungsi zip()

Untuk mengulang urutan secara terbalik, pertama tentukan urutan dalam arah maju dan kemudian panggil fungsi reversed()

 ![Screenshot_15](https://user-images.githubusercontent.com/70943455/109427588-9bba7980-7a25-11eb-81bd-e6f07132b504.png)

Untuk mengulangi sebuah urutan sequence dalam susunan yang diurutkan, gunakan fungsi sort() yang mengembalikan daftar terurut baru dengan membiarkan sumber tidak diubah

 ![Screenshot_16](https://user-images.githubusercontent.com/70943455/109427590-9c531000-7a25-11eb-9c2b-f5009a265248.png)

5.7. More on Conditions

Kondisi yang digunakan dalam pernyataan while dan if dapat berisi operator apa pun, bukan hanya perbandingan. Operator perbandingan in dan not in memeriksa apakah suatu nilai terjadi (tidak terjadi) secara berurutan. Operator is dan is not membandingkan apakah dua objek benar-benar objek yang sama; ini hanya penting untuk objek yang dapat diubah seperti daftar list.
 
![Screenshot_17](https://user-images.githubusercontent.com/70943455/109427591-9c531000-7a25-11eb-9306-36f4dae3e398.png)