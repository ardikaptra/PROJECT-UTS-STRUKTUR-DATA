# Sistem Antrian Pelayanan Mie Gacoan

# Identitas Kelompok:
I Wayan Ardika Putra Widnyana (2501010108) (ardikaptra)

⁠I Gede Aris Pratama Putra (2501010011)

Putu Intan Cahyanti Putri (2501010046) (intancahyanti341-hue)


# 1. Rumusan Masalah dan Solusi
Rumusan Masalah:

1. Bagaimana merancang sistem antrian digital yang mampu menangani lonjakan pelanggan pada jam sibuk?
2. Bagaimana penerapan struktur data queue dapat meminimalisir kesalahan dalam pemanggilan nomor antrian?
3. Bagaimana sistem antrian dapat memberikan informasi posisi antrian secara real-time kepada pelanggan?
   
Solusi:

Sistem ini dirancang menggunakan struktur data Queue dengan prinsip FIFO (First In First Out), di mana pelanggan yang datang lebih dahulu akan dilayani terlebih dahulu.

Implementasi menggunakan linked list memungkinkan sistem untuk:

- Menyimpan data antrian secara dinamis
- Menghindari batasan kapasitas seperti pada array
- Mempermudah proses penambahan dan penghapusan data

Fitur utama sistem:

- Pengambilan nomor antrian
- Pemanggilan nomor antrian
- Melihat antrian terdepan
- Menampilkan seluruh antrian

# 2. Landasan Teori

Struktur data merupakan cara untuk mengorganisasi, menyimpan, dan mengelola data agar dapat diakses dan diproses secara efisien. Pemilihan struktur data yang tepat sangat berpengaruh terhadap performa suatu sistem, terutama dalam hal kecepatan akses, penggunaan memori, dan kemudahan manipulasi data. Struktur data banyak digunakan dalam pengembangan perangkat lunak untuk meningkatkan efisiensi algoritma.

Queue dan stack merupakan dua jenis struktur data linear yang sering digunakan dalam pemrograman. Queue bekerja dengan prinsip antrian, sedangkan stack bekerja seperti tumpukan. Keduanya memiliki aturan tersendiri dalam proses penambahan dan penghapusan data, sehingga penggunaannya disesuaikan dengan kebutuhan sistem yang dibangun.

Konsep FIFO (First In First Out) digunakan pada queue, di mana data yang pertama kali masuk akan menjadi data pertama yang keluar. Sebaliknya, stack menggunakan konsep LIFO (Last In First Out), yaitu data terakhir yang masuk akan menjadi data pertama yang keluar. Kedua konsep ini sangat penting dalam berbagai aplikasi, seperti sistem antrian pelanggan, pengolahan data, serta manajemen memori.

Implementasi queue dan stack dapat dilakukan menggunakan array maupun linked list. Array memiliki ukuran tetap sehingga lebih sederhana, namun kurang fleksibel jika terjadi penambahan data secara dinamis. Sementara itu, linked list memungkinkan alokasi memori yang dinamis karena setiap elemen dihubungkan melalui pointer, sehingga lebih fleksibel dan efisien dalam menangani data yang berubah-ubah.

Referensi:

- Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2009). Introduction to Algorithms. MIT Press.
- Goodrich, M. T., Tamassia, R., & Goldwasser, M. H. (2014). Data Structures and Algorithms in Java. Wiley.
- Weiss, M. A. (2013). Data Structures and Algorithm Analysis in Java. Pearson.
- Sedgewick, R., & Wayne, K. (2011). Algorithms. Addison-Wesley.
