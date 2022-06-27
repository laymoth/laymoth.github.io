---
title: "Macam Macam Percabangan Dan Perulangan"
date: 2022-06-27T21:22:58+07:00
draft: true
toc: false
images:
tags:
  - Algoritma dan Pemrograman
---

#### Percabangan if else
Karakteristrik : terdapat pengkodisian yang cukup kompleks yang mempengaruhi hasil

Contoh :
```
nilaiUjian = 10
if((x < 100) & (x>80))
 cetak lulus terbaik
else if((x < 100) & (x>50))
 cetak lulus
else
 cetak gagal
```

#### Percabangan switch case
Karakteristrik : tidak terdapat pengkodisian yang ada hanyalah penukaran bilangan

Contoh :
```
noAbsent = 3
switch(noAbsent)
 case  1 :
 Ahmad Jainudin
 case 2 :
 Boby Sugandi
 case 3 :
 Dodi Sukmawan
 case 4 :
	Bukan Mahasiswa
```

#### Percabangan case when
Karakteristrik : terdapat pengkodisian tetapi tidak ada percabangan bersarang

Contoh :
```
warna = “merah”
case when warna = “biru”
 then “cocok”
 else “tidak cocok”
end
```

#### Pengulangan For
Karakteristrik : looping dengan menggunakan pengkondisian

Contoh :
```
for(i=0; i<10; i++)
  cetak i
```

#### Pengulangan while
Karakteristrik : looping dengan menggunakan batas tertentu
Contoh :
```
x = {10, 8, 5, 4, 3}
while(x)
 cetak x
```

#### Pengulangan do while
Karakteristrik : looping dengan menggunakan kondisi tetapi loopingnya di jalankan dulu baru cek kondisi

Contoh :
```
x = 3
do{
  cetak x	
} while(x<2)
```