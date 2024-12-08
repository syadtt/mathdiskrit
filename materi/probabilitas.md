---
title: probabilitas

---

# Probabilitas

## Teorema Bayes

Teorema Bayes memberi tahu kita bagaimana menghitung probabilitas kondisional dari suatu peristiwa berdasarkan pengetahuan sebelumnya tentang peristiwa itu. Dengan kata lain, ini memungkinkan kita untuk menghitung **probabilitas posterior** berdasarkan **probabilitas sebelumnya** :

$$
P(E|C) = \frac{P(C|E) \cdot P(E)}{P(C)}
$$

Dalam persamaan ini, kita memiliki empat istilah ini:

* **Posterior Probability** *P(E | C)*: probabilitas peristiwa E terjadi, mengingat kondisi C benar.
* **Prior Probability** *P(E)*: satu-satunya probabilitas peristiwa E terjadi, yang merupakan pengetahuan sebelumnya tentang peristiwa itu sendiri.
* **Likelihood** *P(C | E)*: probabilitas kondisi C menjadi benar, mengingat peristiwa E terjadi.
* **Marginal Probability** *P(C )*: satu-satunya probabilitas kondisi C menjadi benar.

#### Contoh 1
Jika Anda memiliki dua kelas $C_1$ dan $C_2$, serta fitur $x_1$, $x_2$ :

Diketahui:

- $P(C_1) = 0.5 \), \( P(C_2) = 0.5$

- $P(x_1|C_1) = 0.8 \), \( P(x_2|C_1) = 0.6$

- $P(x_1|C_2) = 0.4 \), \( P(x_2|C_2) = 0.7$

Untuk menghitung $P(C_1|X)$ dan $P(C_2|X)$:

1. $P(X|C_1) = P(x_1|C_1) \cdot P(x_2|C_1) = 0.8 \cdot 0.6 = 0.48$

2. $P(X|C_2) = P(x_1|C_2) \cdot P(x_2|C_2) = 0.4 \cdot 0.7 = 0.28$
3. Normalisasi:

   - $P(C_1|X) = \frac{P(X|C_1) \cdot P(C_1)}{P(X)} = \frac{0.48 \cdot 0.5}{0.48 + 0.28} \approx 0.63$

   - $P(C_2|X) = \frac{P(X|C_2) \cdot P(C_2)}{P(X)} = \frac{0.28 \cdot 0.5}{0.48 + 0.28} \approx 0.37$

Sehingga data $X$ lebih mungkin masuk ke $C_1$.



#### Contoh 2

Bagaimana kemungkinan/probabilitas usia paruh baya tekanan darah sangat tinggi  kemungkinan penyakit Hipertensi (H) atau Tidak (T)

| No | Usia        | Tekanan Darah   | Penyakit (H/T) |
|----|-------------|-----------------|----------------|
| 1  | Muda        | Normal          | T              |
| 2  | Muda        | Tinggi          | T              |
| 3  | Paruh baya  | Normal          | T              |
| 4  | Paruh baya  | Tinggi          | H              |
| 5  | Tua         | Normal          | H              |
| 6  | Tua         | Sangat Tinggi   | H              |
| 7  | Muda        | Normal          | T              |
| 8  | Tua         | Tinggi          | H              |

**Jawaban** :

$$
P(H|E) = \frac{P(E|H) \cdot P(H)}{P(E)}
$$

Di mana:

* P(H|E) adalah probabilitas hipotesis (H) diberikan bukti (E)
* P(E|H) adalah probabilitas bukti diberikan hipotesis
* P(H) adalah probabilitas awal hipotesis
* P(E) adalah probabilitas awal bukti

Dalam kasus ini, hipotesis adalah "Hipertensi" (H) dan buktinya adalah "Usia Paruh Baya" dan "Tekanan Darah Sangat Tinggi".

Langkah-langkah perhitungannya adalah sebagai berikut:
1. Menghitung P(H|E) untuk Hipertensi:

    a. P(E|H) = 1, karena tabel menunjukkan bahwa untuk Usia Paruh Baya dan Tekanan Darah Sangat Tinggi, hasilnya selalu Hipertensi (H).
    
    b. P(H) = 1/8 = 0,125, karena ada 8 baris total dalam tabel dan 1 di antaranya memiliki hasil H.
    
    c. P(E) = 1/8 = 0,125, karena ada 1 baris dalam tabel dengan Usia Paruh Baya dan Tekanan Darah Sangat Tinggi.
    
    d. Memasukkan nilai-nilai ini ke dalam rumus: P(H|E) = (1 * 0,125) / 0,125 = 1 atau 100%.

2. P(T|E) untuk Tidak Hipertensi: 

    a. P(E|T) = 0, karena tabel menunjukkan bahwa untuk Usia Paruh Baya dan Tekanan Darah Sangat Tinggi, hasilnya tidak pernah Tidak Hipertensi (T).
    
    b. P(T) = 7/8 = 0,875, karena ada 7 baris dengan hasil T dari total 8 baris.
    
    c. P(E) = 1/8 = 0,125, seperti yang dihitung sebelumnya.
    
    d. Memasukkan nilai-nilai ini ke dalam rumus: P(T|E) = (0 * 0,875) / 0,125 = 0 atau 0%.
    
Jadi, kesimpulannya adalah:

* Probabilitas Hipertensi pada usia paruh baya dengan tekanan darah sangat tinggi adalah 100%.
* Probabilitas Tidak Hipertensi pada usia paruh baya dengan tekanan darah sangat tinggi adalah 0%.

