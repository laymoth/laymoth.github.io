---
title: "Pohon Biner"
date: 2022-06-27T09:05:42+07:00
toc: false
images: 
tags:
  - Matematik Diskrit
---

Pohon berakar (pohon) adalah beberapa graf yang terkoneksi seperti path sederhana yang unik dengan tanpa siklus pada verteks yang disebut akar R.  
Biasanya pohon digambarkan mulai dari akar (atas) ke daun (bawah), atau dari akar (kiri) ke daun (kanan).  
Pohon berurut adalah pohon berlabel mulai dari 0 (akar), 1, 2,… (node), 1.1,1.2,…, 2.1,2.2, … (cabang dari node), dan seterusnya sampai pada daun.  
Jumlah cabang untuk setiap node dapat berbeda. 

![Pohon Biner](/assets/pohon-biner.png)


#### Pohon Berakar Terurut
Pohon berakar terurut adalah pohon yang setiap anak dari induknya diurutkan dari kiri ke kanan (akar di atas).  
Urutan secara leksikografik mulai dari 0, 1, 1.1, 1.2, … , 2, 2.1,2.2, … dst.  
Akar membawahi anak (child), setiap anak dapat membawahi anak dari anak.  
Setiap anak mempunyai induk (parent).  
Anak 1.1 mempunyai sibling 1.2, 1.3 dan seterusnya (jika ada).  
Anak dari akar mempunyai nomor tingkat ke-1, anak dari anak mempunyai nomor tingkat ke-2, dan seterusnya.  
Kedalaman pohon adalah jumlah tingkat maksimal (sesuai dengan nomor tingkat tertinggi) dari salah satu cabang.  
Pohon dapat dianggap sebagai himpunan sub-pohon  .

#### Pohon Biner
Pohon biner merupakan struktur dasar matematika dan ilmu komputer.  
Istilah-istilah yang berlaku pada pohon (umum) seperti node, induk, anak, tingkat, kedalaman dsb., juga berlaku pada pohon biner.  
Pohon biner T adalah himpunan terbatas elemen yang disebut node. T dapat merupakan himpunan kosong (pohon kosong), atau terdiri dari node R sebagai akar yang dapat diikuti oleh dua pohon T1 dan T2 yang disjoin dan terurut.  
Perbedaan utama pohon biner terhadap pohon terurut adalah jumlah anak (suksesor langsung) dari node pada pohon biner selalu dua (jika ada), yang disebut node suksesor kanan dan node suksesor kiri.  
Jika node tidak mempunyai suksesor disebut node terminal (daun).  

Contoh:  
Pada gambar di bawah :  
T1, T2, T3 adalah merupakan pohon berakar.  
T1, T2, T3 adalah juga merupakan pohon berakar terurut, di mana : T1 dan T2 mempunyai urutan yang sama (A,B,C,D), T3 mempunyai urutan (A,C,B,D).  
T1, T2, T3 adalah juga merupakan pohon biner, di mana T1 dan T2 berbeda pada node D (pada T1: D adalah suksesor kiri, sedangkan pada T2: D adalah suksesor kanan)  .

![Pohon Biner 4 Node](/assets/m4-b4node.jpg)

Pohon biner serupa adalah pohon biner yang mempunyai kesamaan struktur (kesamaan suksesor kiri atau kanan dari semua cabang node).
Pohon biner salinan (copy) adalah pohon biner yang mempunyai kesamaan bentuk.
  
Ekspresi aljabar dapat direpresentasikan dengan pohon biner.  
Contoh : E = (2x + y).(5a - b)^3  

![Pohon Biner](/assets/m4-pb.jpg)

Pohon biner dapat dipakai dalam mengelola memori dengan menggunakan array
INFO, LEFT dan RIGHT
Contoh:
Representasikan urutan info mulai dari akar beralamat : 14 dalam bentuk pohon
biner : 

| Alamat | 1  | 2 | 3 | 4 | 5  | 6 | 7 | 8 | 9  | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 |
|--------|----|---|---|---|----|---|---|---|----|----|----|----|----|----|----|----|----|----|
| INFO   | H  | R |   | P | B  |   | E |   | C  | F  | Q  | S  |    | A  | K  | L  |    | D  |
| LEFT   | 4  | 0 |   | 0 | 18 |   | 1 |   | 0  | 15 | 0  | 0  |    | 5  | 2  | 0  |    | 0  |
| RIGHT  | 11 | 0 |   | 0 | 7  |   | 0 |   | 10 | 16 | 12 | 0  |    | 9  | 0  | 0  |    | 0  |

Jawaban:  

![13 Node](/assets/m4-13n.jpg)

#### Penelusuran (Traversal) Pohon Biner:
Ada tiga algoritma traversal pohon biner (rekursif), yaitu : pre-order, in-order dan
post-order  
**Pre-order:**
- Proses akar R
- Traverse sub pohon kiri dari R secara pre-order  
- Traverse sub pohon kanan dari R secara pre-order  

**In-order:**
- Traverse sub pohon kiri dari R secara in-order  
- Proses akar R  
- Traverse sub pohon kanan dari R secara in-order  

**Post-order:**
- Traverse sub pohon kiri dari R secara post-order  
- Traverse sub pohon kanan dari R secara post-order  

Contoh:

![6 Node](/assets/m4-6n.jpg)

Pre-order: ABDECF  
In-order: DBEACF  
Post-order: DEBFCA  
