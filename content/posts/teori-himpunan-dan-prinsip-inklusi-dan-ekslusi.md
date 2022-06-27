---
title: "Teori Himpunan & Prinsip Inklusi & Ekslusi"
date: 2022-04-09T10:27:00+07:00
toc: false
tags:
  - Matematik Diskrit
---

#### Himpunan, Sub Himpunan, Sub-himpunan, himpunan, himpunan, dan Elemen  
Himpunan &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Huruf besar (kapital)  
Elemen &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Huruf kecil  
φ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Himpunan kosong, himpunan yang tidak memiliki elemen  
U &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Himpunan universal atau semesta  
A = {1, 2, 3, 4, 5} &nbsp; Himpunan A mempunyai elemen : 1,2,3,4 dan 5  
B = {6, 7, 8, 9, 0}  
A ≠ B  
C = {x: x bilangan bulat, 0 < x < 6}  
A = C &nbsp;&nbsp;&nbsp;&nbsp; Himpunan A sama dengan C, jika elemen A sama dengan elemen C  
1 ∈ A &nbsp;&nbsp;&nbsp;&nbsp; 1 adalah elemen himpunan A, atau 1 kepunyaan A  
1 ∉ B &nbsp;&nbsp;&nbsp;&nbsp; 1 bukan elemen himpunan B, A ≠ B  
D = {7, 9}  
E = { } atau E = φ &nbsp;&nbsp;&nbsp;&nbsp; E adalah himpunan kosong  
D ⊆ B atau B ⊇ D &nbsp;&nbsp;&nbsp;&nbsp; D adalah sub-himpunan B atau B mengandung D  
D ⊂ B atau B ⊃ D &nbsp;&nbsp;&nbsp;&nbsp; D adalah sub-himpunan murni B  
  
Contoh : simbol himpunan :  
N = himpunan bilangan bulat positif  
Q = himpunan bilangan rasional  
Z = himpunan bilangan bulat  
R = himpunan bilangan riil  
N dapat dijadikan himpunan semesta (U) dari himpunan A, B, D & E   

#### Diagram Venn, Komparabel, Disjoin
Himpunan B dan D komparabel, karena D ⊆ B 
Himpunan A dan B disjoin

![Diagram Venn](/assets/m1-diagramvenn.jpg)

#### Operasi himpunan dan Produk
Union : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A ∪ B = { x : x ∈ A atau x ∈ B}  
Interseksi : &nbsp; A ∩ B = { x : x ∈ A dan x ∈ B}  
Komplemen (absolut) : &nbsp;&nbsp;&nbsp; A’ = {x : x ∈ U, x ∉ A}  
Komplemen (relatif) : &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A – B = { x : x ∈ A, x ∉ B} (perbedaan A terhadap B)  

![Union dan Interseksi Himpunan](/assets/m1-union.jpg)

![Komplemen Absolut dan Komplemen Relatif](/assets/m1-komplemen.jpg)

Perbedaan simetri A dan B atau A ⊕ B adalah  
(A ∪ B) – (A ∩ B) atau (A – B) ∪ (B – A)  
Jika : A ⊆ B, maka A ∩ B = A dan A ∪ B = B  

#### Hukum aljabar himpunan dan Dualitas
Hukum de Morgan  
(A ∪ B)’ = A’ ∩ B’ dan (A ∩ B)’ = A’ ∪ B’  
Hukum idempoten:  
A ∪ A = A dan A ∩ A = A  
Hukum asosiatif :  
(A ∪ B) ∪ C = A ∪ (B ∪ C) dan (A ∩ B) ∩ C = A ∩ (B ∩ C)  
Hukum komutatif:  
A ∪ B = B ∪ A dan A ∩ B = B ∩ A  
Hukum distributif :  
A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C) dan A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)  
Hukum Identitas  
A ∪ φ = A dan A ∩ U = A  
Hukum Konstanta :  
A ∪ U = U dan A ∩ φ = φ  
Hukum Komplemen :  
A ∪ A’ = U dan A ∩ A’ = φ  
Hukum Absorpsi :  
A ∩ (A ∪ B) = A dan A ∪ (A ∩ B) = A  
Prinsip dualitas : tukar ∩ dengan ∪ dan U dengan φ atau sebaliknya  
Perbedaan simetri : ⊕, memenuhi hukum asosiatif, komutatif, dan distributif  

#### Himpunan terbatas dan Prinsip Inklusi dan Eksklusi Himpunan terbatas dan Prinsip Inklusi dan Eksklusi
Himpunan terbatas A adalah himpunan A yang jumlah elemennya (n(A)) terbatas  
Prinsip inklusi dan eksklusi dua dan tiga himpunan terbatas yang berbeda:  
n(A ∪ B) = n(A) + n(B) – n(A ∩ B) atau n(A ∩ B) = n(A) + n(B) – n(A ∪ B)  
n(A ∪ B ∪ C) = n(A) + n(B) + n(C) – n(A ∩ B) – n(A ∩ C) – n(B ∩ C) +n(A∩B∩C)  

#### Koleksi
Koleksi adalah himpunan dari himpunan
Contoh :
K = [{1, 2, 3}, {2, 4}, {3, 5}] 