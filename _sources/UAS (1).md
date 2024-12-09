---
title: UAS

---



| P   | Q   | R   | S   |
| --- | --- | --- | --- |
|  T   |   T  |    T |   T  |
|  T   |   T  |    F |   F  |
|  F   |   F  |    F |   T  |
|  T   |   F  |    T |   T  |
|  F   |   T  |    F |   T  |
|  F   |   T  |    F |   T  |
|  T   |   T  |    T |   T  |
|  F   |   F  |    F |   F  |

soal 

1. $(P \to Q) \to (R \to S)$

2. buat graph A, B, C, D, E, F, G 
    - a. hitung Closennes centrality G
    - b. beetwinnes centrality F

Jawab:

1. 
| P   | Q   | R   | S   | $(P \to Q)$ |  $(R \to S)$   |   $(P \to Q) \to (R \to S)$  |
| --- | --- | --- | --- | ---------- | --- | --- |
| T   | T   | T   | T   | T          |  T   |   T  |
| T   | T   | F   | F   | T          |   T  |  T   |
| F   | F   | F   | T   |  T          |   T  |   T  |
| T   | F   | T   | T   |  F          |   T  |   T  |
| F   | T   | F   | T   |  T          |   T  |   T  |
| F   | T   | F   | T   |  T          |  T   |    T |
| T   | T   | T   | T   |   T         |  T   |    T |
| F   | F   | F   | F   |   T         |   T  |    T |

2. 
![Graph 2](https://hackmd.io/_uploads/BJ4iSG4N1l.png)

a. Hitung Closeness Centrality G
    
| Node | A    | B    | C    |  D   |  E   |   F  |   G  |
| ---- | ---- | ---- | --- | --- | --- | --- | --- |
| G | 2 | 2 |  1   |  1   |   2  | 1    |   0  |

$$
C_C(G) = \frac{7-1}{2+2+1+1+2+1+0} = \frac {6}{9}
$$

b. Hitunglah Betweeness Centrality F

| Node | A   | B   | C   | D   | E   | F   | G   |
| ---- | --- | --- | --- | --- | --- | --- | --- |
| A    |     |     |     |     |     |     |     |
| B    |     |     |     |     |     |     |     |
| C    |     |     |     |     |     |     |     |
| D    |     |     |     |     |     |     |     |
| E    |     |     |     |     |     |     |     |
| F    | 2   | 2   | 1   | 1   | 1   | 0   | 1 |
|  G    |     |     |     |     |     |     |     |


Jumlah Rute Terpendek = $2+2+1+1+1+0+1 = 8$

$$
C_B(F) = \frac{2}{(8-1)(8-2)/2} = \frac {2}{21}
$$