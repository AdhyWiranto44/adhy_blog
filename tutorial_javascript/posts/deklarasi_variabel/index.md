# Deklarasi Variabel

## Definisi

Sebelum ECMAScript 2015 (ES Module 6) muncul, satu-satunya cara kita mendeklarasikan variabel pada javascript adalah dengan menggunakan keyword ```var``` dimana terdapat banyak masalah yang muncul, seperti:

1. Hoisting
2. Nilai selalu bisa diganti

### Hoisting

Hoisting adalah fenomena saat interpretasi kode javascript dilakukan. dimanapun kita melakukan deklarasi variabel, saat interpretasi dilakukan variabel tersebut akan dipindahkan ke baris awal di kode kita.

Perhatikan contoh berikut:

```js
nama = "Jihyo";
var nama;

printNama(nama);
```

Saat hoisting terjadi, kodenya akan menjadi seperti berikut:

```js
var nama;
nama = "Jihyo";

printNama(nama);
```

Lalu masalahnya ada dimana? Kita menjadi tidak tahu variabel mana yang DIGANTI value-nya dengan yang BARU dideklarasikan.

Maka keyword ```let``` dan ```const``` muncul untuk memperbaiki masalah tersebut.

### Nilai selalu bisa diganti

Jika kalian mengetahu bahasa pemrograman java, di sana ada keyword ```final``` kita dapat menentukan variabel mana yang konstan value-nya alias tidak akan pernah bisa diganti setelah dideklarasikan. Namun di javascript tidak ada keyword seperti itu.

Lalu masalahnya ada dimana? Data yang penting yang tidak boleh diganti seperti notasi PI (π) di fisika akan dengan mudah diganti. Kita tidak ingin hal ini terjadi.

Maka keyword ```const``` muncul untuk memperbaiki masalah tersebut.

## Berbagai cara deklarasi variabel

Setidaknya kita sudah mengerti alasan dibalik munculnya keyword ```let``` dan ```const``` ini.

Sekarang kita cari tahu bagaimana cara menuliskannya.

### Let

Jadi ```let``` ini adalah versi baru dari ```var``` yang perbedaannya ada pada lingkupnya, di mana variabel ```let``` tidak bisa diakses di luar lingkupnya, misalkan di lingkup ```function``` maka tidak akan bisa diakses di luar ```function``` tersebut.

Jika kita coba implementasikan kode di atas menggunakan ```let```.

```js
nama = "Jihyo";
let nama;

// kita anggap fungsi ini melakukan console.log(nama)
printNama(nama);
```

Maka akan muncul ```undefined``` artinya tidak ada value yang diisi pada variabel ```nama``` tersebut.

Namun jika kita menulisnya seperti berikut

```js
let nama;
nama = "Jihyo";

// kita anggap fungsi ini melakukan console.log(nama)
printNama(nama);
```

Maka value ```nama``` akan ditampilkan.

Jadi mulai sekarang kita ganti ```var``` menjadi ```let``` ya :).

### Const

Lalu ada ```const``` dimana dia adalah keyword untuk membuat sebuah variabel yang isinya tidak bisa kita ubah setelah kita definisikan.

## Tugas

Oke, sekarang coba kerjakan soal berikut:

1. Perhatikan kode berikut:
```js
let first_name = "Park";
const last_name = "Jihyo";
```
2. Gabungkan kedua variabel tersebut menjadi ```full_name``` dan tampilkan menggunakan ```console.log()```
3. Ganti value ```last_name``` menjadi ```Sooyoung``` lalu tampilkan menggunakan ```console.log()```. Lihat apa yang terjadi?