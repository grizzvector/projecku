Penggunaan Cuckoo
=================


Menajalankan Cuckoo
^^^^^^^^^^^^^^^^^^^

Untuk penggunaa cuckoo, jalankan cuckoo, rooter, dan web interface cuckoo pada terminal yang berbeda.

1. Pada terminal 1, dilakukan untuk menjalankan perintah agar rooter dapat digunakan oleh group PSSN. 

$ cuckoo rooter –sudo –group pssn

.. image:: 1.PNG

2. Selanjutnya, Pada terminal 2, jalankan virtual environment yang telah dibuat pada langkah sebelumnya. 

$virtualenv -p python2.7 cuckoo-test

.. image:: 2.PNG

3. Pada terminal 3, jalankan web interface cuckoo untuk mempermudah dalam melihat analisis dan memonitor  cuckoo.

$cuckoo web –host 0.0.0.0 –port 8000

.. image:: 3.PNG

4. Setelah semua terminal telah dijalankan, berikut merupakan tampilan pada ketiga terminal dalam menjalankan cuckoo.

.. image:: 4.PNG

Cuckoo Interface
^^^^^^^^^^^^^^^^
Setelah menjalankan ketiga perintah diatas, buka engine browser dan akses alamat IP cuckoo dengan port yang telah di konfigurasikan.

.. image:: 5.PNG

Selanjutnya, Lakukan pengambilan binaries dari server Dionaea dan Cowrie, kemudia import ke cuckoo untuk melakukan analisis.

.. image:: 6.PNG

.. image:: 7.PNG

Setelah binaries berhasil di import, lakukan analisi dengan menjalankan binaries pada sandbox yang telah dibuat. Proses analisis yang sedang berjalan akan di-tag dengan “running” sedangakn proses yang telah selesai akan di-tag dengan “reported”.

.. image:: 8.PNG

.. image:: 9.PNG

Pada menu recent, dapat dilihat proses analisis yang telah dilakukan. Pada menu ini akan di perlihatkan kapan malware itu di analisis serta memberikan nilai hash.

.. image:: 10.PNG

Cuckoo tidak hanya menilai score dari binaries dan memberikan summary analisis saja, tetapi cuckoo memberikan hasil analisis pada berbagai bagian. Pada dashboard Cuckoo akan diberi pilihan, fitur apa saja yang tersedia pada Cuckoo.

.. image:: 11.PNG

1. Summary Analysis

Pada analisis ini akan memberikan informasi umum terkait malware yang dianalisis seperti ukuran file, tipe, serta nilai hash.

.. image:: 12.PNG
.. image:: 13.PNG
.. image:: 14.png

2. Static Analysis

.. image:: 15.PNG

3. Network Analysis

.. image:: 16.PNG

4. Behavioral Analysis

.. image:: 17.PNG

5. Dropped File

.. image:: 18.PNG

6. Dropped Buffers

.. image:: 19.PNG

7. Process Memory

.. image:: 20.PNG

8. Compare

.. image:: 21.PNG

9. Export Analysis

.. image:: 22.PNG

 
