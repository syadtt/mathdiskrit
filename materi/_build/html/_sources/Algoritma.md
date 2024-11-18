---
title: Algoritma

---

# Algoritma
## Definisi Algoritma
Pengertian algoritma berdasarkan Microsoft Press Computer and Internet Dictionary (1998) merupakan deretan dari sekumpulan rangkaian tindakan tertentu yang pastinya logis dalam menyelesaikan persoalan. Logis di sini memiliki arti bahwa tindakan yang dilakukan harus sesuai dengan urutan dan tersusun secara runtut serta langkah tersebut harus diketahui dengan pasti agar algoritma yang dipakai dapat berjalan semestinya.

Sjukani (2005) berpandangan bahwa algoritma merupakan jalan pikiran yang digunakan saat penyelesaian sebuah operasi yang dijabarkan dalam bentuk tertulis. Alur pikir disini mengisyaratkan bahwa jalan pikiran seseorang dapat berbeda dengan yang lainnya. Sementara itu makna tertulis berbentuk kalimat, tabel, atupun gambar tertentu yang dapat ditulis.

Dalam pandangan Gunadarma (1988) definisi algoritma merupakan gabungan dari sekumpulan perintah yang menjabarkan langkah-langkah yang jelas saat prosedur pelaksanaan memecahkan sebuah permasalahan, dengan tuntutan himpunan bersifat mekanik.

Dapat disimpulkan definisi algoritma adalah ilmu yang membahas cara-cara penyelesaian sebuah persoalan dengan deretan langkah tertentu kemudian tersusun dengan sistematis dan memakai bahasa logis serta memiliki sebuah tujuan .

### Algoritma Sequential Search
Sequential search adalah teknik pencarian data dimana data dicari secara urut dari depan ke belakang atau dari awal sampai akhir berdasarkan key yang dicari (C, Antonius Rachmat dan M, Aditya Wikan, 2016). Kelebihan dari proses pencarian secara sequential search jika data yang dicari terletak di depan, maka data akan ditemukan dengan cepat. Tetapi dibalik kelebihannya ini, teknik ini juga memiliki kekurangan jika data yang dicari terletak di belakang atau paling akhir, maka akan membutuhkan waktu yang lama dalam proses pencariannya. Algoritma sequential search termasuk kedalam algoritma pencarian yang paling sederhana. Sequential search disebut juga pencarian lurus (linear search). Pada dasarnya, algoritma pencarian beruntun adalah proses membandingkan setiap elemen larik secara beruntun satu persatu, mulai dari 14 elemen pertama, sampai elemen yang dicari ditemukan, atau seluruh elemen sudah diperiksa. Atau singkatnya algoritma sequential search ini mencari data dari awal sampai ditemukan, setelah data ditemukan pencarian berhenti.

**Algoritma Sequential Search**
* Cara kerja : Membandingkan data satu per satu secara berurutan, mulai dari elemen pertama sampai elemen yang dicari ditemukan
* Kelebihan : Jika data yang dicari terletak di depan, maka data akan ditemukan dengan cepat
* Kekurangan : Jika data yang dicari terletak di belakang atau paling akhir, maka akan membutuhkan waktu yang lama dalam proses pencariannya
* Nama lain : Pencarian linier (linear search)

### Algoritma Binary Search
Binary Search adalah algoritma pencarian yang efisien untuk menemukan elemen di dalam daftar yang sudah diurutkan. Algoritma ini bekerja dengan membagi daftar menjadi dua bagian secara rekursif hingga menemukan elemen yang dicari atau memastikan bahwa elemen tersebut tidak ada.
## Pseudocode
### Pengertian
Pseudocode adalah representasi sederhana dari algoritma atau langkah-langkah pemrograman yang ditulis dalam bahasa yang mirip dengan bahasa manusia. Pseudocode tidak mengikuti sintaks bahasa pemrograman tertentu, tetapi ditulis dengan cara yang cukup mirip agar mudah dipahami dan diubah menjadi kode nyata.

### Tujuan Pseudocode
* **Mempermudah Pemahaman Algoritma**: Pseudocode membantu dalam memahami algoritma tanpa terjebak pada detail teknis bahasa pemrograman tertentu.
* **Komunikasi**: Membantu programmer, desainer, atau siapa pun yang bekerja pada proyek untuk berkomunikasi dengan lebih baik.
* **Perencanaan**: Digunakan untuk merencanakan struktur program sebelum mulai menulis kode sebenarnya.

### Contoh Pseudocode
Berikut adalah contoh pseudocode untuk Binary Search:
1. Tentukan low sebagai indeks awal (0) dan high sebagai indeks akhir (panjang array - 1).
2. Selama low lebih kecil atau sama dengan high:
    * Hitung mid sebagai indeks tengah dari (low + high) // 2.
    * Jika elemen pada mid adalah elemen yang dicari (target):
        * Kembalikan mid.
    * Jika elemen pada mid lebih besar dari target:
        * Atur high ke mid - 1.
    * Jika elemen pada mid lebih kecil dari target:
        * Atur low ke mid + 1.
3. Kembalikan -1 jika elemen tidak ditemukan.

### Ciri-Ciri Pseudocode
* **Bahasa Umum**: Ditulis dalam bahasa yang mudah dimengerti oleh manusia.
* **Detail yang Cukup**: Mengandung langkah-langkah utama tanpa terlalu terperinci tentang implementasi.
* **Struktur Logis**: Menggunakan struktur kontrol umum seperti "jika", "selama", atau "untuk" untuk mengorganisir langkah-langkah.

Pseudocode bertindak sebagai perantara antara pemikiran logis manusia dan penerjemahan logika tersebut ke dalam kode nyata dalam bahasa pemrograman.
## Big O Algoritma
Big O Notation adalah cara untuk mengukur efisiensi algoritma, terutama dalam hal waktu atau ruang (memori) yang dibutuhkan. Notasi Big O berfokus pada perilaku algoritma saat ukuran input (n) tumbuh sangat besar, dan menggambarkan seberapa cepat waktu eksekusi atau penggunaan memori algoritma meningkat relatif terhadap ukuran input.

### Tujuan Big O Notation
* **Mengukur Efisiensi Algoritma**: Mengetahui seberapa baik algoritma akan berperforma saat ukuran data besar.
* **Membandingkan Algoritma**: Big O Notation memungkinkan kita membandingkan efisiensi beberapa algoritma untuk memilih yang terbaik untuk kasus tertentu.
* **Memahami Skala Algoritma**: Dengan Big O, kita bisa memahami seberapa baik algoritma beradaptasi dengan pertumbuhan data.

### Jenis Kompleksitas dalam Big O
1. **Kompleksitas Waktu (Time Complexity)**: Menunjukkan seberapa cepat waktu eksekusi algoritma bertambah dengan peningkatan ukuran input.
2. **Kompleksitas Ruang (Space Complexity)**: Menunjukkan seberapa besar penggunaan memori bertambah dengan peningkatan ukuran input.

### Notasi Umum Big O
1. **O(1) - Konstan**: Waktu eksekusi tidak berubah terlepas dari ukuran input. Contoh: Mengakses elemen dalam array dengan indeks tertentu.

2. **O(log n) - Logaritmik**: Waktu eksekusi tumbuh secara logaritmik seiring dengan pertumbuhan input. Contoh: Binary Search, yang membagi masalah menjadi dua setiap langkah.

3. **O(n) - Linear**: Waktu eksekusi bertambah seiring dengan pertumbuhan input secara langsung. Contoh: Linear Search, yang memeriksa setiap elemen dalam daftar.

4. **O(n log n) - Linear Logaritmik**: Kombinasi antara linear dan logaritmik, umumnya ditemukan pada algoritma pengurutan yang efisien, seperti Merge Sort dan Quick Sort.

5. **O(n²) - Kuadrat**: Waktu eksekusi meningkat dengan kuadrat dari input. Contoh: Bubble Sort atau algoritma nested loop (dua lapisan).

6. **O(2^n) - Eksponensial**: Waktu eksekusi meningkat secara eksponensial dengan pertumbuhan input. Algoritma ini biasanya tidak praktis untuk input besar. Contoh: Algoritma rekursif yang menyelesaikan masalah subset atau kombinasi.

7. **O(n!) - Faktorial**: Waktu eksekusi meningkat secara faktorial, biasanya untuk masalah yang melibatkan semua kemungkinan urutan, seperti Permutasi.

### Contoh Penggunaan Big O
**Binary Search (O(log n))**
Binary Search pada daftar yang diurutkan secara logaritmik, membagi daftar menjadi dua setiap langkah, dan hanya membutuhkan beberapa langkah untuk menyelesaikan masalah meskipun ukuran input besar.

**Bubble Sort (O(n²))**
Bubble Sort adalah algoritma pengurutan sederhana yang membandingkan setiap elemen berpasangan, membutuhkan dua lapisan loop untuk memeriksa semua kombinasi, sehingga kompleksitas waktu adalah kuadrat.

### Mengapa Big O Penting?
Big O memberikan panduan mengenai skala algoritma. Ketika ukuran data kecil, perbedaan antara O(n) dan O(n²) mungkin tidak terasa. Namun, saat data tumbuh besar, algoritma dengan kompleksitas yang lebih rendah (seperti O(log n) atau O(n)) akan jauh lebih efisien dibandingkan dengan algoritma dengan kompleksitas lebih tinggi (seperti O(n²) atau O(2^n)).
## Hitung Big O dari Algoritma Sequrntial Search
* **Waktu Kompleksitas (Time Complexity**
    Algoritma Sequential Search memiliki kompleksitas waktu sebagai berikut:
    * **Best Case (Kasus Terbaik): 𝑂(1)**
        Terjadi ketika elemen yang dicari berada di awal daftar. Dalam hal ini, hanya satu perbandingan yang diperlukan.
    * **Worst Case (Kasus Terburuk): 𝑂(𝑛)**
        Terjadi ketika elemen yang dicari berada di akhir daftar atau tidak ada di dalam daftar sama sekali. Dalam kasus ini, algoritma harus memeriksa semua elemen dalam daftar.
    * **Average Case (Kasus Rata-rata): 𝑂(𝑛)**
        Jika kita asumsikan elemen yang dicari dapat berada di posisi mana pun dengan peluang yang sama, rata-rata waktu yang diperlukan adalah sekitar separuh dari panjang daftar, yaitu 𝑂(𝑛/2). Namun, dalam notasi Big O, 𝑂(𝑛/2) disederhanakan menjadi 𝑂(𝑛).
        
* **Ruang Kompleksitas (Space Complexity)**
     * **Ruang Tetap (Constant Space)**: Algoritma Sequential Search hanya membutuhkan sejumlah variabel tetap untuk menyimpan indeks saat iterasi dan elemen target yang dicari.

        Misalnya, jika kita menggunakan variabel index untuk menyimpan posisi saat ini dan target untuk menyimpan nilai yang dicari, ruang yang dibutuhkan oleh algoritma ini tidak bergantung pada ukuran input (list/array). Karena hanya membutuhkan beberapa variabel tambahan, ruang yang diperlukan adalah konstan.

    * **Ruang Kompleksitas**: Karena tidak ada struktur data tambahan yang digunakan yang bergantung pada jumlah elemen dalam daftar, ruang kompleksitasnya adalah:

                                    **O(1)**
        Ini berarti bahwa algoritma Sequential Search memiliki ruang kompleksitas sebesar 𝑂(1), atau disebut juga sebagai Constant Space Complexity. Algoritma ini hanya memerlukan ruang tetap yang tidak bertambah dengan meningkatnya jumlah elemen dalam daftar.
        
        Secara umum, Sequential Search sangat efisien dari segi penggunaan memori karena tidak memerlukan ruang tambahan yang signifikan, selain dari variabel untuk iterasi dan menyimpan elemen target.
## Referensi
1. https://osf.io/preprints/osf/agnzm
2. https://media.neliti.com/media/publications/360919-none-b992c0d2.pdf
