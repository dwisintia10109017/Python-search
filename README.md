# Sequential-search-dan-binary-seacrh
Percobaan 10 Binary Search_Rotation,
Menemukan rotasi terkecil dalam sebuah list yang sudah dirotasi. Kita mulai dengan menentukan low (indeks pertama dalam daftar) dan high
(indeks terakhir dalam daftar).
Dalam loop while, kita menghitung indeks tengah (mid) dengan menggunakan operator floor division // pada penjumlahan low dan high.
Kita membandingkan elemen yang berada di indeks mid dengan elemen yang berada di indeks high.
Jika data[mid] lebih besar dari data[high], itu berarti titik rotasi berada di sebelah kanan mid. 
Oleh karena itu, kita perbarui low = mid + 1 untuk mencari di sebelah kanan mid. Jika data[mid] tidak lebih besar dari data[high], itu berarti titik rotasi berada di sebelah kiri mid atau mid itu sendiri adalah indeks rotasi terkecil.
Dalam kasus ini, kita perbarui high = mid untuk mencari di sebelah kiri mid. Loop akan terus berlanjut selama low kurang dari high. 
Setelah loop selesai, nilai low akan menjadi indeks rotasi terkecil.
Kita mengembalikan nilai low sebagai indeks rotasi terkecil dan mencetaknya.

Percobaan 11 Binary Search_Most Frequent,
Menemukan elemen yang sering muncul paling banyak dalam sebuah list yang sudah diurutkan. Variabel max_count digunakan untuk melacak jumlah kemunculan maksimum dari elemen yang paling sering muncul.
Variabel most_frequent digunakan untuk menyimpan elemen yang paling sering muncul.Kita mulai dengan menentukan low (indeks pertama dalam daftar) dan high (indeks terakhir dalam daftar).
Dalam loop while, kita menghitung indeks tengah (mid) dengan menggunakan operator floor division // pada penjumlahan low dan high.Kita inisialisasi count dengan 1 untuk menghitung jumlah kemunculan elemen di indeks mid.
Kita periksa elemen-elemen di sebelah kiri dan kanan mid untuk menghitung jumlah kemunculan yang sama.
Dalam loop while, kita menginkrementasikan count dan memperbarui indeks left ke sebelah kiri dan indeks right ke sebelah kanan hingga elemen yang berdekatan masih sama dengan elemen di indeks mid.
Selama count lebih besar dari max_count, kita memperbarui max_count dengan count dan most_frequent dengan elemen di indeks mid.
Jika count sama dengan 1, itu berarti elemen di indeks mid tidak memiliki kemunculan lain dalam daftar, maka kita keluar dari loop.
Jika masih terdapat kemungkinan elemen yang sama di sebelah kiri, kita perbarui high menjadi indeks left. Jika masih terdapat kemungkinan elemen yang sama di sebelah kanan, kita perbarui low menjadi indeks right.
Loop while akan terus berlanjut selama low kurang dari atau sama dengan high.Setelah loop selesai, nilai most_frequent akan berisi elemen yang paling sering muncul dalam daftar.
Kita mengembalikan most_frequent sebagai hasil dan mencetaknya.

Percobaan 12 Binary Search_Name List,
Mencari data dalam list terurut. Pertama, kita menentukan low sebagai indeks pertama dalam daftar dan high sebagai indeks terakhir dalam daftar.
Dalam loop while, kita menghitung indeks tengah (mid) dengan menggunakan operator floor division // pada penjumlahan low dan high.Jika elemen di indeks mid sama dengan target yang dicari, maka kita langsung mengembalikan nilai mid sebagai indeks yang sesuai.Jika elemen di indeks mid lebih kecil dari target, artinya target berada di sebelah kanan mid. Oleh karena itu, kita perbarui low = mid + 1 untuk mencari di sebelah kanan mid.
Jika elemen di indeks mid lebih besar dari target, artinya target berada di sebelah kiri mid. Dalam kasus ini, kita perbarui high = mid - 1 untuk mencari di sebelah kiri mid.Loop while akan terus berlanjut selama low kurang dari atau sama dengan high.Jika loop selesai dan kita belum menemukan target, maka kita mengembalikan nilai -1 sebagai tanda bahwa target tidak ditemukan dalam daftar.Setelah keluar dari loop, kita mencetak pesan yang sesuai berdasarkan hasil pencarian.
