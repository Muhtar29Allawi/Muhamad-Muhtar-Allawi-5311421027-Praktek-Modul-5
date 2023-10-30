# Muhamad-Muhtar-Allawi-5311421027-Praktek-Modul-5
Teknik Pencarian Heuristic Search

Nama : Muhamad Muhtar Allawi
Nim : 5311421027
Prodi : Teknik Elektro

MODUL 5
TEKNIK HEURISTIC SEARCH

1.	Pada source code yang saya buat akan menghasilkan sebagai berikut:

![Screenshot 2023-10-30 065831](https://github.com/Muhtar29Allawi/Muhamad-Muhtar-Allawi-5311421027-Praktek-Modul-5/assets/148027728/fd599e85-cfdb-46ce-a67f-f5f1b6fb131a)

 
-	Root: 3 1 2 4 7 5 6 8 0: Ini adalah keadaan awal (root node) dari permainan Puzzle dengan keadaan ubin seperti yang dinyatakan dalam urutan angka.
-	Setelah melakukan pencarian, program menemukan solusi, dan kemudian mencetak "Solution found" untuk memberi tahu bahwa solusi telah ditemukan.
-	Kemudian program mencetak langkah-langkah yang diperlukan untuk mencapai solusi. Setiap baris dalam output mewakili keadaan ubin pada langkah-langkah tertentu. Misalnya, 3 1 2 4 7 5 6 0 8 adalah langkah awal, dan 0 1 2 3 4 5 6 7 8 adalah langkah terakhir yang mencapai tujuan (keadaan yang benar).
Hasil output menunjukkan urutan langkah-langkah yang diperlukan untuk memindahkan ubin-ubin ke keadaan yang benar, sehingga ubin-ubin terurut dengan benar sesuai dengan tujuan "Eight Puzzle".
Jadi, program berhasil menemukan solusi dari Eight Puzzle dan mencetak langkah-langkahnya. Solusi tersebut adalah perubahan keadaan ubin-ubin dari keadaan awal ke keadaan tujuan.

	EightPuzzleSearch Class:
•	EightPuzzleSearch adalah kelas utama dalam program ini. Ini mengatur alur utama dari pencarian solusi untuk masalah "Eight Puzzle".
•	Di dalam kelas ini, Anda akan menemukan fungsi run(), yang melakukan algoritma pencarian A* untuk menemukan solusi. Ini juga mengelola open list, closed list, dan fungsi-fungsi heuristik.
•	Fungsi main() adalah fungsi utama yang dijalankan saat program dimulai. Ini membuat instance EightPuzzleSearch dan memanggil run() untuk memulai pencarian solusi. 
EightPuzzleSpace Class: 
•	EightPuzzleSpace digunakan untuk mengatur informasi tentang keadaan awal dan tujuan dalam permainan Eight Puzzle.
•	Fungsi getRoot() mengembalikan node keadaan awal dari permainan, yang disimpan dalam bentuk array.
•	Fungsi getGoal() mengembalikan node keadaan tujuan yang benar.
•	Fungsi getSuccessors() menghasilkan semua kemungkinan langkah (successors) yang dapat diambil dari keadaan tertentu dalam permainan. 
Node Class: 
•	Node mewakili node dalam pohon pencarian yang digunakan oleh algoritma A* untuk mencari solusi.
•	Setiap Node memiliki atribut yang mencakup state (keadaan), biaya, parent (node yang sebelumnya), dan successors (anak-anak).
•	Fungsi equals() memeriksa apakah dua node memiliki keadaan yang sama.
•	Fungsi getPath() digunakan untuk mendapatkan path dari root node ke node tertentu dalam pohon pencarian.
•	Heuristik yang digunakan dalam pencarian, seperti h1Cost() dan h2Cost(), digunakan untuk menghitung perkiraan biaya yang diperlukan untuk mencapai tujuan dari suatu keadaan.
•	Fungsi transformState() menghasilkan keadaan yang dihasilkan dari mengganti posisi dua ubin dalam papan permainan. 
Ketiga kelas ini bekerja sama untuk melaksanakan pencarian solusi dalam masalah Eight Puzzle menggunakan algoritma A* dengan fungsi heuristik untuk menginformasikan pencarian. EightPuzzleSearch mengatur logika pencarian, EightPuzzleSpace menyediakan informasi tentang keadaan awal dan tujuan, sementara Node mewakili setiap keadaan dalam pencarian dan menghitung biaya serta jalur yang ditempuh.

2.	Pada soal kedua setelah mengubah initial dan goal state maka akan menjadi sebuah program yang akan menjalankan puzzle sesuai keadaan awal dan goals yang dituju. Sehingga akan menhasilkan program sebagai berikut:

![Screenshot 2023-10-30 222751](https://github.com/Muhtar29Allawi/Muhamad-Muhtar-Allawi-5311421027-Praktek-Modul-5/assets/148027728/73d51f42-4a23-4063-9799-19ac9b210545)

 


4.	Ubahlah initial dan goal state dari program  di atas sehingga bentuk initial dan goal statenya Gambar 5.9. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state.  Analisa dan bedakan dengan solusi pada point 1 dan 2.
Mendapatkan hasil Program sebagai berikut:
 
![Screenshot 2023-10-30 222808](https://github.com/Muhtar29Allawi/Muhamad-Muhtar-Allawi-5311421027-Praktek-Modul-5/assets/148027728/7f1ccfec-2c51-499e-b418-21b1e45f4d9e)



5.	Setelah initial dan goal state diubah sesuai pada soal maka akan menghasilkan puzzle sebagai berikut:
 
![Screenshot 2023-10-30 220448](https://github.com/Muhtar29Allawi/Muhamad-Muhtar-Allawi-5311421027-Praktek-Modul-5/assets/148027728/b2f9854d-f69d-4026-9aeb-30637b9fba6f)

Hasil yang didapatkan adalah solusi dari permainan 8-Puzzle. Permainan 8-Puzzle adalah permainan teka-teki di mana memiliki kotak berukuran 3x3 yang berisi angka 1 hingga 8, serta satu tempat kosong yang digunakan untuk memindahkan angka-angka tersebut. Tujuan dari permainan ini adalah mengatur angka-angka tersebut sehingga membentuk urutan yang benar dari 1 hingga 8.  Dalam hasil yang didapatkan, program mencetak urutan langkah-langkah yang harus diambil dari keadaan awal (Root) untuk mencapai keadaan tujuan (Solution found). Setiap langkah mencakup pemindahan angka dari satu kotak ke kotak lainnya atau memindahkan kotak kosong. Solusi ini adalah solusi optimal, yang berarti jumlah langkah yang diambil adalah yang paling sedikit.

5.	Pada soal ini memiliki sedikit perbedaan dengan soal sebelumnya yaitu puzzle menggunakan huruf sehingga kita dapat menggantikan huruf tersebut dengan angka terlebih dahulu.
A = 1
B = 2 
C = 3
D = 4
E = 5
F = 6 
G = 7
H = 8
-	=  9
Sehingga menghasilkan sebagai berikut:
4 2 5 1 0 7 8 3 6
4 2 5 0 1 7 8 3 6
4 2 5 1 0 7 8 6 3
4 2 5 1 4 7 8 6 3
4 2 5 1 7 0 8 6 3
4 2 5 1 7 8 0 6 3
4 2 5 1 0 8 7 6 3
4 2 5 0 1 8 7 6 3
4 2 5 6 0 8 7 1 3
4 2 5 6 8 0 7 1 3
4 2 5 6 8 1 7 0 3
4 2 5 6 8 1 0 7 3
4 2 5 6 8 1 3 7 0
4 2 5 6 8 1 3 0 7
4 2 5 6 1 8 3 0 7
4 2 5 6 1 3 8 0 7
4 2 5 6 1 3 8 7 0






