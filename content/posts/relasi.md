---
title: "Relasi"
date: 2022-06-26T22:41:20+07:00
toc: false
images:
tags:
  - Matematik Diskrit
---

#### Himpunan Produk
Himpunan hasil perkalian dua atau lebih himpunan terbatas, yang elemennya merupakan pasangan elemen dari himpunan-himpunan yang dikalikan dan bergantung pada urutannya. Simbol produk: X  
Secara umum : A X B ≠ B X A  
Contoh:  
A = {1,2,3}, B = {a,b}, C = {x}  
A X B = {<1,a>,<1,b>,<2,a>,<2,b>,<3,a>,<3,b>}, (ada 3 X 2 = 6 elemen)  
A X B X C = {<1,a,x>,<1,b,x>,<2,a,x>,<2,b,x>,<3,a,x>,<3,b,x>}, (ada 3 X 2 X 1 = 6 elemen)  
Berlaku ketentuan :  
(A X B) ∪ (A X C) = A X (B ∪ C) dan  
(A X B) ∩ (A X C) = A X (B ∩ C)  

#### Himpunan Relasi
Himpunan relasi (biner) R merupakan sub-himpunan dari himpunan produk P atau (R ⊂ P ) atau himpunan relasi adalah himpunan yang merelasikan elemen dua himpunan  
Contoh:  
A = {1,2}, B = {a,b}  
R = {<1,a>, <2,b>} merupakan himpunan relasi antara A dan B,  
Q = {<1,b>,<2,a>} juga merupakan himpunan relasi antara A dan B  
S = {<1,a>,<1,b>} juga merupakan himpunan relasi antara A dan B  
P = {<1,a>,<1,b>,<2,a>,<2,b>} merupakan himpunan relasi juga himpunan produk antara himpunan A dan B  

#### Operasi Relasi
Operasi relasi antar himpunan terbatas menghasilkan himpunan relasi  
Jenis operasi relasi : lebih besar (>), lebih kecil (<) dan sama dengan (=)  
Contoh :  
A = {1,3,4}, B = {2,3}  
A < B adalah R1 = {<1,2>, <1,3>}  
A > B adalah R2 = {<3,2>,<4,2>,<4,3>}  
A = B adalah R3 = {<3,3>}  

#### Representasi Relasi
Matriks  
Contoh :  
A = {1,2,3}, B = {x,y}  
R = {<1,x>, <2,y>, <3,y>}, adalah matriks (baris: A, kolom :B) :  
  
![Matriks](/assets/m2-matrix.png)

#### Graf Berarah
Contoh : relasi pada himpunan A = {1,2,3,4} adalah  
R = {<1,2>,<2,2>,<2,4>,<3,2>,<3,4>,<4,1>,<4,3>}  

![Graf Berarah](/assets/m2-graf.jpg)

#### Komposisi Relasi
Komposisi relasi (simbol: o) antara dua himpunan relasi akan menghasilkan himpunan relasi baru, jika ada elemen himpunan yang sama sebagai perantara  
Contoh-1 :  
A = {1,2,3}, B = {a,b}, C = {x,y}  
R = {<1,a>,<1,b>,<2,a>} (dapat ditulis : a R b = relasi elemen himpunan A dan B)  
S = {<a,x>,<b,x>,<b,y>} (dapat ditulis : b S c = relasi elemen himpunan B dan C)  
  
Himpunan komposisi relasi : T = R o S atau (a R b) o (b S c) atau (a T c ) adalah  
T = {<1,x>,<1,y>,<2,x>} (ada 2 <1,x> dari <1,a>o<a,x> dan <1,b>o<b,x>) 
   
Atau dengan cara mengalikan matris Mr dan Ms menjadi matriks Mt :  

![Matriks](/assets/m2-relasi.png)

Contoh-2 :  
X = {a, b, c}  
R = {<a,b>,<a,c>,<b,a>}  
S = {<a,c>,<b,a>,<b,b>,<c,a>}  
T = R o S = ?  

![Matriks](/assets/m2-contoh.png)

Jadi T = {<a,a>, <a,b>, <b,c>} 

#### Tipe Relasi
Refleksif : Jika a R a untuk semua elemen a di himpunan A  
Simetrik : Jika a R b berimplikasi b R a  
Antisimetrik : Jika a R b dan b R a berimplikasi a ≠ b  
Transitif : Jika a R b dan b R c berimplikasi a R c  
Ekivalen : Jika bertipe relasi refleksif, simetrik dan transitif  

Contoh :  
B = {1,2,3,4}  
R = {<1,1>,<1,2>,<2,1>,<2,2>,<3,3>} adalah relasi refleksif (di kanan dan kiri
semuanya mengandung : 1,2,3 dan kedua-duanya tidak ada 4)  
S = B X B adalah relasi simetrik (karena selalu ada pasangan seperti <1,3> dan <3,1>)  
R adalah juga relasi simetrik (ada <1,2> dan <2,1>, selain yang <1,1>,<2,2>,<3,3>)  
A = {<1,1>,<1,2>,<2,2>,<2,3>} adalah relasi antisimetrik (selain <1,1> dan <2,2>, ada <1,2> tetapi tidak ada <2,1> dan ada <2,3> tetapi tidak ada <3,2>)  
T = {<1,2>,<2,3>,<1,3>,<3,3>} adalah relasi transitif (ada <1,2> dan <2,3>, tetapi juga ada <1,3>)  

#### Partisi
Partisi dari suatu himpunan adalah klas himpunan relasi yang disjoin secara mutual (semua elemen himpunan adalah elemen salah satu elemen partisi). Elemen partisi disebut sel dan merupakan sub-himpunan dari himpunan yang dipartisi  
Contoh :  
S = {1,2,3,4,5,6}  
P=[{1,3,5},{2,4},{6}] adalah partisi dari S  
N1=[{1,2,3},{1,4,5,6}] adalah bukan partisi dari S (karena elemen 1 ada pada dua sel)  
N2 = [{1,2,5},{2,4,6,7}] adalah bukan partisi dari S (karena {2,4,6,7} bukan sub-himpunan S)  

#### Relasi Terner dan N-er 
Jika relasi melibatkan tiga himpunan disebut relasi terner dan menghasilkan
himpunan relasi dengan elemen berbentuk triplet  
Secara umum relasi yang melibatkan banyak (N) himpunan disebut relasi N-er 