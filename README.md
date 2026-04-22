# Sistem Antrian Pelayanan Mie Gacoan

# Link PPT
https://canva.link/93h4u5vjbdg60rs

# Identitas Kelompok:
I Wayan Ardika Putra Widnyana (2501010108) (ardikaptra)

⁠I Gede Aris Pratama Putra (2501010011) (arisspratamaa092)

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

# 3. Desain Sistem dan Implementasi
Desain Sistem (Pseudocode)
```
START

SET nomor = 1

WHILE program berjalan:
    Tampilkan menu:
        1. Ambil Nomor Antrian
        2. Panggil Antrian
        3. Lihat Antrian Depan
        4. Tampilkan Semua Antrian
        5. Keluar
   
    INPUT pilihan

    IF pilihan == 1:
        enqueue(nomor)
        tampilkan "Nomor antrian:", nomor
        nomor = nomor + 1

    ELSE IF pilihan == 2:
        dequeue()

    ELSE IF pilihan == 3:
        peek()

    ELSE IF pilihan == 4:
        display()

    ELSE IF pilihan == 5:
        STOP
END
```
Alur Sistem (Input → Proses → Output)
Input: Pelanggan mengambil nomor antrian melalui sistem
Proses: Sistem menyimpan nomor ke dalam queue menggunakan operasi enqueue, serta memproses pemanggilan dengan dequeue
Output: Nomor antrian ditampilkan dan dipanggil sesuai urutan (FIFO)
Implementasi Program

Sistem ini diimplementasikan menggunakan struktur data Queue berbasis Linked List dengan operasi minimal:

Enqueue (menambah data)

Dequeue (menghapus data)

Peek (melihat data terdepan)

Display (menampilkan seluruh data)

# 4. Kesimpulan

Sistem antrian digital yang dirancang menggunakan struktur data Queue dengan prinsip FIFO (First In First Out) terbukti efektif dalam mengelola proses pelayanan pelanggan secara lebih teratur, adil, dan efisien. Dengan konsep ini, pelanggan yang datang terlebih dahulu akan dilayani lebih dahulu sehingga dapat meminimalisir kesalahan dalam pemanggilan nomor antrian.

Implementasi menggunakan linked list membuat sistem menjadi lebih fleksibel karena tidak memiliki batasan kapasitas tetap seperti array. Hal ini memungkinkan sistem untuk menangani jumlah pelanggan yang terus bertambah, terutama pada kondisi lonjakan pengunjung.

Selain itu, sistem ini juga menyediakan informasi antrian secara real-time, sehingga pelanggan dapat mengetahui posisi mereka dalam antrian dan memperkirakan waktu tunggu. Dengan demikian, sistem ini tidak hanya meningkatkan efisiensi pelayanan, tetapi juga memberikan kenyamanan dan transparansi bagi pengguna.

Berdasarkan hasil implementasi, dapat disimpulkan bahwa seluruh rumusan masalah telah berhasil diselesaikan. Sistem yang dibangun juga telah berjalan sesuai dengan teori struktur data, khususnya dalam penerapan queue dan prinsip FIFO. Oleh karena itu, penggunaan queue pada sistem antrian pelayanan terbukti sangat bermanfaat dalam meningkatkan kualitas dan efisiensi pelayanan.
