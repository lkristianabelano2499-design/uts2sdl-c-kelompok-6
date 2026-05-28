https://docs.google.com/document/d/16eolUemPmEhimkGHUXqXS7ycX6XqD-_49dNV9udaBGk/edit?usp=sharing

Oleh  
Abel Y Bigail	255314112
Antonius Dwi Sukamdi	255314073
Vincentius Abimanyu Wahyono	255314106
Yudha Gustavo Manihuruk	255314110


C.	Hubungan Antar Class

1.	Class Pasien
Class Pasien digunakan untuk menyimpan seluruh informasi identitas pasien yang berada di IGD, seperti nomor rekam medis, nama, umur, dan alamat pasien. Selain menyimpan identitas, class ini juga memiliki riwayat tindakan medis pasien yang digunakan untuk mencatat setiap tindakan yang diberikan dokter. Class ini menjadi pusat data utama dalam sistem karena hampir seluruh proses berkaitan langsung dengan data pasien.

2.	Class Tindakan Medis
TindakanMedis digunakan untuk menyimpan informasi mengenai tindakan medis yang diberikan kepada pasien. Data yang disimpan meliputi nama tindakan, tanggal tindakan dilakukan, dan nama dokter yang menangani pasien. Objek dari class ini nantinya akan disimpan ke dalam riwayat tindakan medis pada class Pasien.

3.	Class NodePasien
Class NodePasien digunakan sebagai node pada struktur data linked list. Setiap node menyimpan satu objek Pasien serta referensi menuju node berikutnya. Class ini berfungsi untuk membangun hubungan antar data pasien sehingga data dapat disimpan secara dinamis menggunakan konsep linked list.

4.	Class LinkedList
Class LinkedListPasien digunakan untuk mengelola seluruh data pasien yang tersimpan dalam linked list. Class ini memiliki fungsi untuk menambahkan pasien, mencari pasien berdasarkan nomor rekam medis, mengurutkan data pasien berdasarkan umur, dan menampilkan seluruh data pasien. Dengan menggunakan linked list, proses penyimpanan data menjadi lebih fleksibel karena ukuran data dapat bertambah secara dinamis.




5.	Class Queue
Class Queue digunakan untuk mengatur antrean pasien IGD berdasarkan urutan kedatangan. Struktur data queue menerapkan konsep FIFO (First In First Out), yaitu pasien yang datang lebih dulu akan dipanggil lebih dulu untuk diperiksa dokter. Class ini memiliki fungsi untuk menambahkan pasien ke antrean, memanggil pasien berikutnya, dan menampilkan daftar antrean pasien.

Hubungan antar class pada sistem IGD ini saling terhubung untuk mendukung pengelolaan data pasien. Class Pasien memiliki hubungan dengan class TindakanMedis karena setiap pasien dapat memiliki beberapa riwayat tindakan medis yang disimpan dalam riwayat tindakan. Class NodePasien berhubungan dengan class Pasien karena setiap node menyimpan satu objek pasien pada struktur linked list. Selanjutnya, class LinkedListPasien menggunakan NodePasien untuk mengelola seluruh data pasien seperti menambah, mencari, dan menampilkan data pasien. Selain itu, class Queue juga berhubungan dengan class Pasien karena antrean digunakan untuk menyimpan pasien berdasarkan urutan kedatangan di IGD. Seluruh class tersebut bekerja sama untuk membentuk sistem pengelolaan pasien yang terstruktur dan efisien.
