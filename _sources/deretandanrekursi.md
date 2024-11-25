---
title: deretandanrekursi

---

# Deretan dan Rekursi
## 1. Deretan (sequence)
**Deretan** adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu.

***Definisi :*** Sebuah **deretan** adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya **N** atau **P**) ke sebuah himpunan S.

N = {1, 2, 3, 4, … }
S misalnya {2, 4, 6, 8, …}, {1/3, 1/5, 1/7, …}, dan lain sebagainya.

**Notasi deretan:** {$a_n$}

Deretan umumnya dinyatakan dalam suatu formula, misalnya:
$a_n$ = 2n
$a_n$ = 1/n
$a_n$ = 7 – 3n

Dalam konteks matematika, **deretan** sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.
Misalnya:
1. Deretan bilangan ganjil: **1,3,5,7,…**
2. Deretan bilangan genap: **2,4,6,8,…**
3. Deretan bilangan yang membentuk deret aritmetika: **3,6,9,12....**

### Contoh-contoh Deretan dan Formulanya:
#### 1. Barisan Aritmatika
**Barisan Aritmatika** adalah baris yang nilai setiap sukunya didapatkan dari suku sebelumnya melalui **penjumlahan** atau **pengurangan** dengan suatu bilangan.

Untuk mengetahui nilai suku ke-n dari suatu barisan arimatika dapat dihitung dengan rumus berikut.

$$
U_n = 𝑎+(n-1)b
$$

***Keterangan :***
$U_n$ = Suku ke-n

𝑎 = Suku pertama

*b* = Beda(Selisih antar suku)

*n* = Nomor suku yang dicari

**Contoh Soal :**

Suku ke-40 dari barisan 7, 5, 3, 1, … adalah …

**Pembahasan:**

Diketahui:

𝑎 = 7

b = –2

ditanya $U_{40}$ ?

**Jawab:**

$U_n$ = 𝑎+(𝑛−1)𝑏

$U_{40}$ = 7+(40−1)(−2)

= 7 + 39 . (-2)

= 7 + (-78)

= – 71

Jadi, suku ke-40 barisan aritmatika tersebut adalah –71.

#### 2. Deret Aritmatika
**Deret Aritmatika** adalah penjumlahan suku-suku dari barisan aritmatika.

Penjumlahan dari suku pertama sampai suku ke-n barisan aritmatika dapat dihitung dengan rumus berikut.

$$
S_n = \frac{n}{2} (a + U_n)
$$

Jika kita substitusikan $U_n = a + (n - 1)b$, maka:

$$
S_n = \frac{n}{2} \big(a + U_n\big)
$$

Substitusi $U_n$ ke dalam rumus:

$$
S_n = \frac{n}{2} \big(a + (a + (n - 1)b)\big)
$$

Sederhanakan ekspresi:

$$
S_n = \frac{n}{2} \big(2a + (n - 1)b\big)
$$

**Contoh Soal :**

Rumus jumlah n suku pertama deret bilangan 2 + 4 + 6 + … + $U_n$ adalah …

**Pembahasan:**

Diketahui:

𝑎 = 2

b = 2

Ditanya: rumus jumlah n suku pertama deret aritmatika tersebut ?

**Jawab:**

$S_n = \frac{n}{2} \big(2a + (n - 1)b\big)$

$S_n = \frac{n}{2} \big(2 \cdot 2 + (n - 1) \cdot 2\big)$

$S_n = \frac{n}{2} \big(4 + 2n - 2\big)$

$S_n = \frac{n}{2} \big(2 + 2n\big)$

$S_n = \frac{n}{2} \cdot 2(1 + n)$

$S_n = n(1 + n)$

$S_n = n + n^2$

Jadi, rumus jumlah n suku pertama barisan aritmatika tersebut adalah $S_n = n + n^2$

#### 3. Barisan Geometri
**Barisan Geometri** adalah susunan bilangan yang dibentuk menurut urutan tertentu, di mana susunanbilangan di antara dua suku yang berurutan mempunyai rasio yang tetap (dilambangkan dengan huruf r).
Jika $a_1$ adalah suku pertama dan r adalah rasio yang tetap, maka suku ke 2 dan seterusnya adalah

$a_2 = a_1r$

$a_3 = a_2r = a_1r^2$

$a_4 = a_3r = a_1r^3$

Sehingga bentuk umum dari barisan geometri untuk suku ke-n adalah

$$
a_n = a_1 r^{n-1}
$$

Atau

$$
S_n = a_1 \frac{r^n - 1}{r - 1}
$$

***Keterangan :***

$a_n$ = $S_n$ = Suku ke–n

$a_1$ = Suku pertama

$r$ = Rasio yang tetap

$n$ = Banyaknya suku

**Contoh soal:**

Carilah suku ke-8 dari barisan geometri di mana suku pertama adalah 16 dan rasionya adalah 2

**Jawab:**

Diketahui : 

$a_1$ = 16

$r$ = 2

$n$ = 8

Maka : 

$S_8$ = $a_1r^{8-1}$

$S_8$ = $a_1r^7$

$S_8$ = $16(2)^7$

$S_8$ = 2048

#### 4. Deret Geometri
**Deret Geometri** adalah jumlah dari suku-suku atau bilangan-bilangan dalam suatu barisan geometri.
Bentuk deret geometri

$$
D_n = a_1 + a_1r + a_1r^2 + .... + a_1r^{n - 1} ...... (1)
$$

Atau dapat ditulis secara singkat

$$
D_n = \sum_{i=1}^{n} a_1r^{n - 1}
$$

Untuk mendapat rumus $D_n$ bisa dengan kalikan persamaan 1 dengan r

$rD_n = a_1r + a_1r^2 + .... + a_1r^{n - 1} + a_1r^n$

$D_n - rD_n = a_1 - a_1r^n$

$D_n(1 - r) = a_1(1-r^n)$ $\rightarrow$ $D_n$ = $\frac{a_1(1-r^n)}{(1-r)}$

***Keterangan :***

$a_1$ = Suku Pertama

$r$ = Rasio

Rumus Deret Geometri :
* Jika r < 1

$$
D_n = \frac{a_1(1-r^n)}{(1-r)}
$$

* Jika r > 1

$$
D_n = \frac{a_1(r^n-1)}{(r-1)}
$$

* Jika r = 1

$$
D_n = a_1 + a_1 + ..... + a_1
$$

$$
D_n = na_1
$$

**Contoh soal:**
Carilah jumlah suku ke-8 yang pertama dari barisan geometri berikut : 3, 6, 12, 24, . . .

**Jawab:**

Diketahui : 

$a_1$ = 3

$r$ = 2

$n$ = 8

Maka jumlah suku ke-8 ($D_8$) adalah : 

$D_8$ = $\frac{3(1-2^8)}{(1-2)} = 765$

#### 5. Deret Bilangan Kuadrat
**Deret bilangan kuadrat** adalah Deret dengan pola nilai berupa kuadrat bilangan bulat.
Contoh: **1,4,9,16,25,…**
Rumus suku ke-n : 

$$
U_n = U^2
$$

#### 6. Deret Bilangan Kubik
**Deret Bilangan Kubik** adalah Deret dengan pola nilai berupa kubik bilangan bulat.
Contoh: **1,8,27,64,125,…**
Rumus suku ke-n : 

$$
U_n = U^3
$$

#### 7. Deret Fibonacci
**Deret Fibonacci** adalah Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
Contoh: **0,1,1,2,3,5,8,…**
Rumus suku ke-n (rekursif) : 

$$
𝐹_𝑛=𝐹_(𝑛−1)+𝐹_(𝑛−2), 𝐹_0=0, 𝐹_1=1
$$

#### 8. String
**String** adalah deretan berhingga karakter berbentuk $a_1a_2a_3a_4…a_n$

Panjang string **S** adalah jumlah karakter di dalam string tersebut.

Contoh:  informatika adalah string dengan panjang 11 karakter 10100101 adalah string biner dengan panjang 8 bit

String kosong dilambangkan dengan $λ$, panjangnya = 0.

## 2. Penjumlahan Deretan
Jumlah $a_m,a_{m+1},a_{m+2},...., a_n$ adalah $a_m+a_{m+1}+a_{m+2}+....+ a_n.$
Atau dalam notasi sumasi : 
$\sum_{k=m}^{n} a_k$

***Keterangan :***

$k$ = indeks summasi

$m$ = batas bawah indeks

$n$ = batas atas indeks

Beberapa sumasi sudah ditemukan rumus penjumlahannya sebagai berikut:
![Gambar1](https://hackmd.io/_uploads/HkNscjym1e.png)

**Contoh soal :**
* Berapa nilai $\sum_{k=1}^{5} k^2$?

    **Jawab :**
    
    $\sum_{k=1}^{5} k^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55$
    
* Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda. Pada contoh 2 di atas batas bawah digeser dari 1 menjadi 0, akibatnya:

$$
\sum_{k=1}^{5} k^2 = \sum_{k=0}^{4} (k+1)^2
$$

* Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya : 
$$
\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2
$$

* Hitunglah nilai $\sum_{k=50}^{100} k^2$

    **Jawaban :**
    
    $\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2$
    
    $\sum_{k=50}^{100} k^2 = \sum_{k=1}^{100} k^2 - \sum_{k=1}^{49} k^2$
    
    Gunakan rumus : 
    
    $$
    \sum_{k=1}^{n} k^2 = \frac{n(n+1)(2n+1)}{6}
    $$
    
    $\sum_{k=50}^{100} k^2 = \frac{(100)(101)(201)}{6} - \frac{(49)(50)(99)}{6} = 338,350 - 40,425 = 297,925$

## 3. Sumasi Ganda
Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.
Contoh : $\sum_{i=1}^4 \sum_{j=1}^3 i j$
Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu  dilanjukan dengan sumasi terluar:
$\sum_{i=1}^4 \sum_{j=1}^3 i j = \sum_{i=1}^4 (i + 2i + 3i) = \sum_{i=1}^4 6i = 6 + 12 + 18 + 24 = 60$

## 4. Rekursi
**Rekursi** mempunyai arti suatu proses yang bias memanggil atau mendefinisikan objek dalam terminologi dirinya sendiri. Dalam sebuah rekursi sebenarnya tekandung pengertian sebuah prosedur atau fungsi. Perbedaannya adalah bahwa rekursi bisa memanggil dirinya sendiri, kalau prosedur atau fungsi harus diipanggil melalui pemanggil prosedur atau fungsi. 

### Fungsi Rekursi
Fungsi rekursif didefinisikan oleh dua bagian:
1.  **Basis**
    * Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit.
    * Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
2. **Rekurens**
    * Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri.
    * Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil.

**Contoh soal :**
Misalkan f didefinsikan secara rekusif sebagai berikut : 
<img src="https://hackmd.io/_uploads/H1Ed5gWQJe.png
          " alt="Deskripsi Gambar" width="300"> 
          
          
*NB :*
          
$n = 0 \rightarrow Basis$

$n > 0 \rightarrow Rekurens$

Tentukan nilai f(4)!
        
**Solusi :**

f(4) = 2f(3) + 4 

=  2(2f(2) + 4) + 4

=  2(2(2f(1) + 4) + 4) + 4

=  2(2(2(2f(0) + 4) + 4) + 4) + 4

=  2(2(2(2 $\cdot$ 3 + 4) + 4) + 4) + 4	

=  2(2(2(10) + 4) + 4) + 4

=  2(2(24) + 4) + 4

=  2(52) + 4

= 108	

**Cara lain menghitungnya :**

f(0) = 3
f(1) = 2f(0) + 4 = 2 $\cdot$ 3 + 4 = 10
f(2) = 2f(1) + 4 = 2 $\cdot$ 10 + 4 = 24
f(3) = 2f(2) + 4 = 2 $\cdot$ 24 + 4 = 52
f(4) = 2f(3) + 4 = 2 $\cdot$ 52 + 4 = 108

Jadi, f(4) = 108.



## Referensi
1. Deretan Artimatika https://lmsspada.kemdikbud.go.id/pluginfile.php/552772/mod_resource/content/2/%5B12%5D%20Barisan%20dan%20Deret%20Aritmetika.pdf
2. Deretan Geometri https://winalmuslim.wordpress.com/wp-content/uploads/2017/12/materi-2-barisan-deret-geometri.pdf