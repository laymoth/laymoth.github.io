---
title: "Fungsi"
date: 2022-06-26T23:43:49+07:00
toc: false
images:
tags:
  - Matematik Diskrit
---

Fungsi adalah pemetaan dari suatu himpunan A ke himpunan lain B secara unik (semua elemen pada A harus ada pemetaannya pada B secara unik, dan hasil pemetaan pada B boleh berasal dari lebih dari satu elemen di A).  
  
Simbol fungsi dari himpunan A ke himpunan B : 

![Fungsi](/assets/m3-fungsi.jpg)

Contoh :  
A = {1,2,3,4,5}  
Fungsi f (a) dalam bentuk himpunan elemen berpasangan <a,f(a)> :  
f = {<1,3>,<2,5>,<3,5>,<4,2>,<5,3>}  

#### Fungsi Riil
Hasil pemetaan fungsi bilangan bulat yang menghasilkan bilangan bulat berbentuk diskrit. Pemetaan fungsi bilangan riil yang menghasilkan bilangan riil berbentuk kontinu dengan jumlah elemen yang tidak berhingga.  
  
Ada empat pembatas fungsi riil  
Interval tertutup : [a,b] = {x : a < x < b}  
Interval terbuka atas : [a,b) = {x : a < x < b}  
Interval terbuka bawah : (a,b] = (x : a < x < b}  
Interval terbuka : (a,b) = {x : a < x < b}  
Fungsi kontinu dapat didekati dengan fungsi diskrit yang diinterpolasi 

#### Komposisi Fungsi
Komposisi dua fungsi atau lebih yang melibatkan himpunan perantara yang sama akan menghasilkan fungsi baru (fungsi komposisi) yang memetakan elemen himpunan pertama ke himpunan terakhir secara unik.  
Contoh :  
f : A → B; g : B → C; h = g o f atau g(f(a)) : A → C  

![FK](/assets/m3-fungsi-komposisi.jpg)

Misal :  
A = {a,b,c}; B = {x,y,z}; C = {r,s,t}  
f : A → B; g : B → C; h = g o f : A → C 
(g o f)(a) = g(f(a)) = g(y) = t  
(g o f)(b) = g(f(b)) = g (x) = s  
(g o f)(c) = g(f(c)) = g(y) = t  
Cara mengikuti panah :  
a → y → t; b → x → s; c → y → t  

#### Diagram peta Fungsi: Graf Berarah:
Contoh:  
f : A → B; b : B → A; h : C → B; e : B → C; dan d : A → C  
dapat dibuat dalam bentuk diagram peta sbb :  

![Diagram](/assets/m3-diagram.jpg)

#### Satu-Satu, Onto dan Invertibel
Fungsi satu-satu (Injektif) adalah jika setiap elemen yang dipetakan mempunyai peta yang berbeda-beda secara unik  
Fungsi Onto (Surjektif) adalah jika setiap elemen pemetaan adalah elemen pemetaan dari beberapa elemen yang dipetakan  
Fungsi bijektif adalah fungsi satu-satu dan onto sekaligus  
Fungsi invertibel adalah jika f : A → B juga ada g : B → A  
Fungsi konstan adalah jika hasil pemetaan menunjuk ke satu nilai  
Contoh :  
f1 : A → B; f2 : B → C; f3 : C → D dan f4 : D → E, seperti gambar :  

![Jenis Fungsi](/assets/m3-jenis-fungsi.jpg)

Fungsi satu-satu : f1 dan f2  
Fungsi onto : f2 dan f3  
Fungsi bijektif : f2  
Fungsi invertibel : f2  
Fungsi konstan : f4  

#### Fungsi Matematika dan Ilmu Komputer
**Fungsi Floor dan Ceiling**  

![Floor](/assets/m3-floor.png)

**Fungsi Modulus / Aritmatik Modular**  
Contoh:  
Modulo 12 : 5 + 8 = 1  

**Fungsi Faktorial**  
n! = 1.2.3….(n-2).(n-1).n = (n-1)!.n = (n-2)!.(n-1).n dst.  
Contoh:  
n!/(n-1)! = n.(n-1)!/(n-1)! = n  

**Fungsi Eksponensial dan Logaritmik**  
x = a^m = a.a…..a (m kali); a^0 = 1; a^-m = 1/a^m ; a^3 . a^5 = a ^(3+5) = a^8  
m = logb (x); b = basis  

#### Fungsi Rekursif
Fungsi rekursif adalah fungsi yang memanggil dirinya sendiri  
- Fungsi faktorial : jika n=0, maka n! =1  
 Jika n>0, maka n! = n.(n-1)!  
- Fungsi (Urutan) Fibonacci: (F)  
 Jika n=0 atau n=1, maka Fn = n  
 Jika n > 1, maka Fn = Fn-2 + Fn-1  
- Fungsi Ackermann : (A) menghasilkan deretan pasangan bilangan bulat positif  
 Jika m = 0, maka A(m,n) = n +1  
 Jika m ≠ 0, tetapi n = 0, maka A(m,n) = A(m-1,1)  
 Jika m ≠ 0 dan n ≠ 0, maka A9m,n) = A(m-1, A(m,n-1))  

#### Kardinalitas
Kardinalitas adalah jumlah elemen suatu himpunan. Simbol : |X|  
Contoh :  
Kardinalitas koleksi X dari fungsi dari A = {a,b,c} ke B = {1,2,3,4} adalah |X| = n(B) pangkat n(A) = 43 = 64  