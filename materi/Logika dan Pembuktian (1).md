---
title: Logika dan Pembuktian

---

# Logika Matematika

## Negasi
Apa itu Negasi?, Negasi atau ingkaran adalah penolakan dari pernyataan yang ada. Jika sebuah pernyataan bernilai salah maka negasinya bernilai benar dan jika pernyataan bernilai benar maka negasinya bernilai salah. Penulisan lambang negasi P adalah “ *$\sim p$* “. Untuk menentukan ingkaran atau negasi dari sebuah pernyataan maka penulisan ditambah kata “ tidak , tidak benar bahwa, atau bukan“ di depan pernyataan.

Tabel kebenaran dari negasi adalah sebagai berikut :

| *$p$* | *$\sim p$* |
| -------- | -------- |
| B     |  S   |
| S     |  B   |

**atau**

| *$P$* | *$\sim p$* |
| -------- | -------- |
| 1     | 0    |
| 0     | 1    |

## Konjungsi
Jika dua pernyataan digabungkan dengan kata “dan” maka pernyataan itu disebut konjungsi. Penulisan kata gabung “dan “ pada konjungsi dilambangkan dengan tanda : “ ($\wedge$) “. Sedangkan tabel kebenaran pernyataan-pernyataan konjungsi disampaikan dalam bentuk tabel sebagai berikut :



| *p* | *q* | *$p\wedge q$* |
| -------- | -------- | -------- |
| B     | B     | B     |
| B     | S     | S     |
| S     | B     | S     |
| S     | S     | S     |

**atau**

| *p* | *q* | *$p\wedge q$* |
| -------- | -------- | -------- |
| 1     | 1     | 1     |
| 1     | 0     | 0     |
| 0     | 1     | 0     |
| 0     | 0     | 0     |


## Disjungsi
Jika dua pernyataan digabungkan dengan kata “ atau “ maka pernyataan
majemuk ini disebut disjungsi. Disjungsi mempunyai dua arti yang
berbeda yaitu: (1) Disjungsi Inklusif dan (2) Disjungsi Eksklusif
Disjungsi inklusif mempunyai makna benar jika paling sedikit satu dari
pernyataan bernilai benar.
Lambang disjungsi inklusif adalah “ ($\vee$) “ dan tabel kebenarannya sebagai berikut :

| *p* | *q* | *$p\vee q$* |
| -------- | -------- | -------- |
| B     | B     | B     |
| B     | S     | B     |
| S     | B     | B     |
| S     | S     | S     |

**atau**

| *p* | *q* | *$p\vee q$* |
| -------- | -------- | -------- |
| 1     | 1     | 1     |
| 1     | 0     | 1     |
| 0     | 1     | 1     |
| 0     | 0     | 0     |

## Implikasi
Pernyataan majemuk yang berbentuk “ jika P maka Q “ disebut implikasi atau
kondisional. Lambang penulisan implikasi sebagai berikut :
“ P $\to$ Q “ atau “ P $\Rightarrow$ Q“
Pernyataan majemuk “ P $\to$ Q “ akan dikatakan bernilai salah jika P benar dan Q salah, dalam hal lain dikatakan benar.
Tabel kebenaran dari implikasi sebagai berikut : 

| *P* | *Q* | *$P\to Q$* |
| -------- | -------- | -------- |
| B     | B     | B     |
| B     | S     | S     |
| S     | B     | B     |
| S     | S     | B     |

**atau**

| *P* | *Q* | *$P\to Q$* |
| -------- | -------- | -------- |
| 1     | 1     | 1     |
| 1     | 0     | 0     |
| 0     | 1     | 1     |
| 0     | 0     | 1     |

## Biimplikasi
Pernyataan majemuk yang berbentuk “ P jika dan hanya jika Q “
disebut Biimplikasi. Penulisan Biimplikasi menggunakan lambang P $\Leftrightarrow$ Q “. Lambang di atas bermakna :
1. P jika dan hanya jika Q.
2. P ekuivalen Q.
3. P syarat yang perlu dan cukup untuk Q.

Jika P dan Q dua pernyataan yang tersusun sebagai “ P $\Leftrightarrow$ Q “ maka tabel
kebenarannya sebagai berikut : 

| *P* | *Q* | *$\Leftrightarrow$* |
| -------- | -------- | -------- |
| B     | B     | B     |
| B     | S     | S     |
| S     | B     | S     |
| S     | S     | B     |

**atau**

| *P* | *Q* | *$\Leftrightarrow$* |
| -------- | -------- | -------- |
| 1     | 1     | 1     |
| 1     | 0     | 0     |
| 0     | 1     | 0     |
| 0     | 0     | 1     |
## Referensi
https://cdn-gbelajar.simpkb.id/s3/p3k/Matematika/Per%20Pembelajaran/Matematika%20-%20PB3.pdf

## Contoh Soal
Buatlah tabel kebenaran untuk~pernyataan berikut $$P\lor(R\to\ Q)$$

$$\begin{array}{c|c|c|c|cc}P&Q&R&\ Q&R\to\ Q&P\lor(R\to\ Q)\\\hline\text{Т}&\text{Т}&\text{Т}&\text{-}&\text{T}&\text{T}\\\text{Т}&\text{Т}&\text{F}&\text{-}&\text{T}&\text{T}\\\text{T}&\text{F}&\text{T}&\text{-}&\text{F}&\text{T}\\\text{T}&\text{F}&\text{F}&\text{-}&\text{T}&\text{F}\\\text{F}&\text{T}&\text{T}&\text{-}&\text{T}&\text{T}\\\text{F}&\text{T}&\text{F}&\text{-}&\text{T}&\text{T}\\\text{F}&\text{F}&\text{T}&\text{-}&\text{F}&\text{F}\\\text{F}&\text{F}&\text{F}&\text{-}&\text{T}&\text{T}&\text{-}\end{array}$$
