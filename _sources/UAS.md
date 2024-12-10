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

$$
C_B(F) = \sum_{s \neq v \neq t} \frac{\sigma_{st} (F)}{\sigma_{st}}
$$

**Diketahui :**

- Pasangan $(A, G)$:
   Jalur terpendek: $A \to B \to D \to F \to G$.  
   $\sigma_{AG} = 1$, dan $\sigma_{AG}(F) = 1$.

- Pasangan $(B, G)$:
   Jalur terpendek: $B \to D \to F \to G$.  
   $\sigma_{BG} = 1$, dan $\sigma_{BG}(F) = 1$.

- Pasangan $(C, G)$:
   Jalur terpendek: $C \to D \to F \to G$.  
   $\sigma_{CG} = 1$, dan $\sigma_{CG}(F) = 1$.

- Pasangan $(D, G)$:
   Jalur terpendek: $D \to F \to G$.  
   $\sigma_{DG} = 1$, dan $\sigma_{DG}(F) = 1$.

- Pasangan $(E, G)$:
   Jalur terpendek: $E \to F \to G$.  
   $\sigma_{EG} = 1$, dan $\sigma_{EG}(F) = 1$.

- Normalisasinya : 
$$
\text{Jumlah pasangan} = \binom{7}{2} = \frac{7(7-1)}{2} = 21
$$

- Total Kontribusi $\frac {\sigma_{st}(F)} {\sigma_{st}}$ untuk semua pasangan $(s,t)$ : 

$$
C_B(F) = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 5.
$$

**Jadi :**

Betweenness centrality normalisasi : 

$$
C_B(F) = \frac{5}{21} \approx 0.3556.
$$