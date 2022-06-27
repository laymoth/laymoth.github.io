---
title: "Aljabar Boolean"
date: 2022-06-26T19:14:53+07:00
toc: false
images:
tags:
  - Matematik Diskrit
---

Aljabar Boolean adalah ilmu yang mempelajari khusus himpunan B yang elemennya
hanya dua, yaitu konstanta 1 dan konstanta 0 atau true (T) dan false (F) beserta
operasinya. Juga terdapat dua jenis operasi, yaitu : union (+) yang dibaca : atau
(OR) dan irisan (.) yang dibaca : dan (AND)  
Asumsi yang berasal dari aksioma klosur (closure) :
Setiap elemen a, b, c, … (variabel) adalah anggota B (bernilai 1 atau 0),
sehingga: a + b ∈ B dan juga a . b ∈ B 

- **Aksioma dan prinsip dualitas**  
Terdapat lima aksioma (dalil yang kebenarannya tidak perlu dibuktikan lagi),
yang berpasang-pasangan (prinsip dualitas) yaitu :  
  
  Pertama : Aksioma Komutatif :  
 a + b = b + a dan pasangan dualitasnya :  
 a . b = b . a [seperti aljabar non Boolean]  
   
  Kedua : Aksioma Asosiatif :  
 a + ( b + c ) = ( a + b ) + c dan pasangan dualitasnya :  
 a . ( b . c ) = ( a . b ) . c [seperti aljabar non Boolean]  
   
  Ketiga : Aksioma Distributif :  
 a . ( b + c) = (a . b) + (a . c) dan pasangan dualitasnya :  
 a + (b . c ) = (a + b) . (a + c) [perlu dibuktikan]  
  
  Keempat : Aksioma Identitas (diri) :  
 a + 0 = a dan pasangan dualitasnya :  
 a . 1 = a [seperti aljabar non Boolean]  
  
  Kelima : Aksioma Komplemen (negasi) :  
 a + a’ = 1 dan pasangan dualitasnya :  
 a . a’ = 0  

 - **Prinsip dualitas**  
  Prinsip dualitas seperti berlaku pada aksioma di atas juga berlaku pada teorema dan hukum atau dalil (di bawah). 
     
    Yang dimaksud dengan prinsip dualitas adalah setiap persamaan Boolean selalu mempunyai pasangannya dengan cara mengganti dua hal, yaitu :  
    - (.) dengan (+) atau (+) dengan (.) dan  
    - (0) dengan (1) atau (1) dengan (0).  

- **Teorema dan prinsip dualitas**  
Terdapat dua teorema yang diturunkan dari aksioma atau teorema sebelumnya  
  
  Pertama, Teorema (1) atau teorema Idempoten :  
 a + a = a dan pasangan dualitasnya :  
 a . a = a
   
  Kedua, Teorema (2) atau teorema Konstanta :  
 a + 1 = 1 dan pasangan dualitasnya :  
 a . 0 = 0  

- **Hukum Absorpsi dan de Morgan dan prinsip dualitas**
Terdapat dua hukum atau dalil yang diturunkan dari aksioma dan teorema, yaitu :  
  
  Pertama, Hukum Absorpsi (Penyerapan) :  
 a + (a . b) = a dan pasangan dualitasnya :  
 a . (a + b) = a   
  
  Kedua, Hukum de Morgan :  
 (a . b)’ = a’ + b’ dan pasangan dualitasnya :  
 (a + b)’ = a’ . b’  
  
  **Pembuktian : Langsung**  
  - Teorema Idempoten (1a) dengan aksioma Identitas, Komplemen,
Distributif, Komplemen dan Identitas (sebelah kanan)  
a + a = a (dibuktikan)  
a + a = a + 0 (Identitas)  
a + a = a + (a . a’) (Komplemen)  
a + a = (a + a) . (a + a’) (Distributif)  
a + a = (a + a) . (1) (Komplemen)  
a + a = (a + a) (Identitas)  

  - Teorema Idempoten (1b) dengan aksioma Identitas, Komplemen,
Distributif, Komplemen dan Identitas (sebelah kanan)  
a . a = a (dibuktikan)  
a . a = a . 1 (Identitas)  
a . a = a . (a + a’) (Komplemen)  
a . a = (a . a) + (a . a’) (Distributif)  
a . a = (a . a) + (0) (Komplemen)  
a . a = (a . a) (Identitas)  

  - Teorema Konstanta (2a) dengan aksioma Komplemen, Asosiatif, teorema  
Idempoten (1a) dan aksioma Komplemen (sebelah kiri)
a + 1 = 1 (dibuktikan)  
a + (a + a’) = 1 (Komplemen)  
(a + a) + a’ = 1 (Asosiatif)  
a + a' = 1 (Idempoten)  
1 = 1 (Komplemen)  

  - Teorema Konstanta (2b) dengan aksioma Komplemen, Asosiatif, teorema  
Idempoten (1b) dan aksioma Komplemen (sebelah kiri)  
a . 0 = 0 (dibuktikan)  
a . (a . a’) = 0 (Komplemen)  
(a . a) . a’ = 0 (Asosiatif)  
a . a' = 0 (Idempoten)  
0 = 0 (Komplemen)  
  - Hukum absorpsi (a) dengan aksioma Identitas, Distributif, teorema  
Konstanta (2a), dan aksioma Identitas. (sebelah kiri)  
a + (a . b) = a (dibuktikan)  
(a . 1) + (a . b) = a (Identitas)  
a . (1 + b) = a (Distributif)  
a . 1 = a (Konstanta)  
a = a (Identitas)  

  - Hukum Absorpsi (b) dengan aksioma Identitas, Distributif, teorema  
Konstanta (2b) dan aksioma Identitas (sebelah kiri)  
a . (a + b) = a (dibuktikan)  
(a + 0) . (a + b) = a (Identitas)  
a + (0. b) = a (Distributif)  
a + 0 = a (Konstanta)  
a = a (Identitas)  

  **Pembuktian : Tidak langsung**  
  - Hukum de Morgan (a) : (a . b)’ = a’ + b’  
Diketahui : (a .b) .(a .b)’ = 0 (aksioma komplemen-b), buktikan : (a .b) .(a’ + b’) = 0, sehingga secara tidak langsung : (a . b ’) = (a’ + b’)
(melalui aksioma Distributif, Asosiatif, Komplemen dan teorema
Konstanta (2b) (sebelah kiri)  
(a . b) . (a’ + b’) = 0 (dibuktikan)  
(a . b) . a’ + (a . b) . b’ = 0 (Distributif)  
(a . a’) . b + a . (b . b’) = 0 (Asosiatif)  
0 . b + a . 0 = 0 (Komplemen)  
0 + 0 = 0 (Konstanta)  

  - Hukum de Morgan (b) : (a + b)’ = a’ . b’  
Diketahui : (a + b) + (a + b)’= 1 (aksioma komplemen-a),
buktikan : (a + b) + (a’ .b’)=1, sehingga
secara tidak langsung : (a + b)’ = (a’ .b’)  
(melalui aksioma Distributif, Asosiatif, Komplemen dan teorema
Konstanta (2a) (sebelah kiri)  
(a +b) +(a’ . b’) = 1 (dibuktikan)  
((a + b) + a’) . ((a + b) + b’) = 1 (Distributif)  
((a + a’) + b) . (a + (b + b’)) = 1 (Asosiatif)  
(1 + b) . (a + 1) = 1 (Komplemen)  
1 . 1 = 1 (Konstanta)  

  **Catatan** : Untuk memudahkan operasi distributif, maka misalkan :  
    - a . b = c (untuk pembuktian hukum de Morgan (a)  
(a . b) . (a’ + b’) = 0 menjadi : ( c ) . (a’ + b’) = 0, sehingga :  
( c ) . a’ + ( c ) . b’ = 0 atau : (a . b) . a’ + (a . b) . b’ = 0 … dst  

    - a + b = c (untuk pembuktian hukum de Morgan (b)  
(a +b) +(a’ . b’) = 1 menjadi : ( c ) +(a’ . b’) = 1, sehingga :  
(( c ) + a’) . (( c ) + b’) = 1 menjadi : ((a + b) + a’) . ((a + b) + b’) = 1 … dst  

  **Pembuktian substitusi** (melalui asumsi nilai 0 atau 1 dalam bentuk tabel)  
    Untuk itu diperlukan tabel nilai hasil operasi union dan irisan terhadap dua konstanta (0 dan 1) dan dua variabel (a dan b)  
  
  Satu konstanta (0 atau 1)

  Tabel 0
|---|---|------------------|
| 0 | 0 | 0 + 0 atau 0 . 0 |
| 0 | 0 | 0                |

  Tabel 1
|---|---|------------------|
| 1 | 1 | 1 + 1 atau 1 . 1 |
| 1 | 1 | 1                |


  Dua konstanta ( 0 dan 1 )
  Tabel union (+)
|---|---|------------------|
| 0 | 1 | 0 + 1 atau 1 + 0 |
| 0 | 1 | 1                |

  Tabel irisan (.)
|---|---|------------------|
| 0 | 1 | 0 . 1 atau 1 . 0 |
| 0 | 1 | 0                |

  Dua variabel (a dan b), berdasarkan 4 tabel di atas :  

  Tabel union (+)
|---|---|-------|
| **a** | **b** | **a + b** |
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

  Tabel irisan (.)
|---|---|-------|
| **a** | **b** | **a + b** |
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

  Aksioma Komutatif, Asosiatif dan Distributif (a) tidak perlu dibuktikan, kecuali Aksioma Distributif (b) 

  **Pembuktian**
  - Aksioma Distributif (b) :
    a + (b . c ) = (a + b) . (a + c) 
    Tabel kiri : 
|---|---|---|-----|---------|
| **a** | **b** | **c** | **b.c** | **a+(b.c)** |
| 0 | 0 | 0 | 0   | 0       |
| 0 | 0 | 1 | 0   | 0       |
| 0 | 1 | 0 | 0   | 0       |
| 0 | 1 | 1 | 1   | 1       |
| 1 | 0 | 0 | 0   | 1       |
| 1 | 0 | 1 | 0   | 1       |
| 1 | 1 | 0 | 0   | 1       |
| 1 | 1 | 1 | 1   | 1       |

    Tabel kanan : 
|---|---|---|-----|-----|-------------|
| **a** | **b** | **c** | **a+b** | **a+c** | **(a+b).(a+c)** |
| 0 | 0 | 0 | 0   | 0   | 0           |
| 0 | 0 | 1 | 0   | 1   | 0           |
| 0 | 1 | 0 | 1   | 0   | 0           |
| 0 | 1 | 1 | 1   | 1   | 1           |
| 1 | 0 | 0 | 0   | 1   | 1           |
| 1 | 0 | 1 | 0   | 1   | 1           |
| 1 | 1 | 0 | 0   | 1   | 1           |
| 1 | 1 | 1 | 1   | 1   | 1           |

    _Kolom paling kanan tabel kiri dan kanan bernilai sama (terbukti)_

  - Aksioma Identitas (a) : 
    a + 0 = a 
|---|---|-----|
| a | 0 | a+0 |
| 0 | 0 | 0 |
| 1 | 0 | 1 |

    _Kolom a dan kolom a + 0 bernilai sama_

  - Aksioma Identitas (b) : 
    a . 1 = a 
|---|---|-----|
| a | 1 | a.1 |
| 0 | 1 | 0 |
| 1 | 1 | 1 |

    _Kolom a dan kolom a . 1 bernilai sama_

  - Aksioma Komplemen (a) : 
    a + a’ = 1 
|---|---|-----|
| a | a’ | a + a’ |
| 0 | 1 | 1 |
| 1 | 0 | 1 |

    _Kolom paling kanan (a + a’) selalu bernilai 1 (terbukti)_

  - Aksioma Komplemen (b) : 
    a . a’ = 0 
|---|---|-----|
| a | a’ | a + a’ |
| 0 | 1 | 0 |
| 1 | 0 | 0 |

    _Kolom paling kanan (a + a’) selalu bernilai 0 (terbukti)_