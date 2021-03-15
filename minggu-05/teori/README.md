BAB 7 – INPUT OUTPUT
Github : https://github.com/arkanfrs/workshop-python/tree/master/minggu-05

7. Masukan dan Keluaran

7.1. Pemformatan Keluaran yang Lebih Menarik

Sejauh ini kami telah menemukan dua cara penulisan nilai: expression statements dan fungsi print(). (Cara ketiga menggunakan write() metode objek berkas; berkas standar keluaran dapat dirujuk sebagai sys.stdout.

Fungsi str() dimaksudkan untuk mengembalikan representasi nilai-nilai yang terbaca oleh manusia, sementara repr() dimaksudkan untuk menghasilkan representasi yang dapat dibaca oleh penerjemah (atau akan memaksa SyntaxError jika tidak ada sintaks yang setara).

![Screenshot_1](https://user-images.githubusercontent.com/70943455/111104492-71b79a00-8583-11eb-9391-5f53d4fd0f67.png)
 
![Screenshot_2](https://user-images.githubusercontent.com/70943455/111104495-72e8c700-8583-11eb-9931-abcc56902fc0.png)

7.1.1. Literal String Terformat

f-string memungkinkan untuk menyertakan nilai ekspresi Python di dalam string dengan mengawali string dengan f atau F dan menulis ekspresi sebagai {expression}.
 
![Screenshot_3](https://user-images.githubusercontent.com/70943455/111104496-73815d80-8583-11eb-96db-a52ce8d04ed4.png)

7.1.2. Metode String format()

Metode str.format() pada tanda kurung dan karakter di dalamnya (disebut fields format) diganti dengan objek yang diteruskan ke metode str.format(). Angka dalam tanda kurung dapat digunakan untuk merujuk ke posisi objek yang dilewatkan ke dalam metode str.format().
 
![Screenshot_4](https://user-images.githubusercontent.com/70943455/111104499-7419f400-8583-11eb-978c-dba7452d3052.png)

![Screenshot_5](https://user-images.githubusercontent.com/70943455/111104500-7419f400-8583-11eb-8aff-27fbbd0e035d.png)

7.1.3. Pemformatan String Manual

Metode str.rjust() dari objek string merata-kanan-kan sebuah string dalam bidang dengan lebar tertentu dengan menambahkannya dengan spasi di sebelah kiri. Ada metode serupa str.ljust() dan str.center(). Metode ini tidak menulis apa pun, mereka hanya mengembalikan string baru.
 
![Screenshot_6](https://user-images.githubusercontent.com/70943455/111104501-74b28a80-8583-11eb-8cdd-ee8893cbdd43.png)

7.1.4. Pemformatan string lama

Operator % (modulo) juga dapat digunakan untuk pemformatan string. Diberikan 'string' % values % dalam string diganti nol atau elemen pada values . Operasi ini umumnya dikenal sebagai interpolasi string
 
![Screenshot_7](https://user-images.githubusercontent.com/70943455/111104502-754b2100-8583-11eb-8b99-0c38790043bb.png)

7.2. Membaca dan Menulis Berkas

open() mengembalikan sebuah file object, dan paling umum digunakan dengan dua argumen: open(filename, mode). Argumen pertama adalah string yang berisi nama file. Argumen kedua adalah string lain yang berisi beberapa karakter yang menggambarkan cara berkas akan digunakan.
 
![Screenshot_8](https://user-images.githubusercontent.com/70943455/111104504-75e3b780-8583-11eb-9023-4fffad2d7b9a.png)

7.2.2. Menyimpan data terstruktur dengan json

Format JSON umumnya digunakan oleh aplikasi modern untuk memungkinkan pertukaran data
 
![Screenshot_9](https://user-images.githubusercontent.com/70943455/111104506-75e3b780-8583-11eb-88e9-4a3c83eed083.png)
