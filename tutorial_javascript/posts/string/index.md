# String

## Definisi

String adalah salah satu tipe data yang ada pada javascript.

## Cara Penulisan String

Cara penulisan value-nya dibungkus menggunakan "kutip dua" atau 'kutip satu' atau dengan \`backtick\`.

Contoh:
```js
var nama1 = "Adhy";

var nama2 = 'Dicky';

var nama3 = `Zikri`;
```

## Menampilkan string ke layar

Jika kita ingin menampilkan variabel (tidak hanya yang bertipe string) kita bisa melakukannya dengan berbagai cara, salah satunya dengan perintah:

```js
console.log(nama1);
```

Jika belum tahu cara menggunakannya, kalian bisa cek dahulu cara menggunakan javascript melalui [web browser]() dan [terminal]().

## Manipulasi String

Manipulasi string bermanfaat untuk mengelola data pada aplikasi kita, misalkan mencari tahu banyaknya karakter pada sebuah kalimat, menyambungkan value sebuah variabel dengan variabel lain, mencari, dan mengganti.

### .length

Mengetahui banyaknya karakter pada suatu string (spasi termasuk)

```js
var jeongyeon = "Yoo Jeongyeon";

var panjang_karakter = nama.length;

console.log(panjang_karakter);  // 13
```

### Concatenation

Menggabungkan dua variabel atau lebih.

```js
var first_name = "Minatozaki";
var last_name = "Sana";

var full_name = first_name + " " + last_name;
console.log(full_name); // "Minatozaki Sana"

var hmm = true + 1;
console.log(hmm); // 2
```

Loh ```true``` itu apa? kok hasilnya 2?

Preview saja, true ini bertipe data boolean yang nilainya antara ```true``` atau ```false```.

### String Interpolation

String interpolation ini adalah bentuk baru dari concatenation yang muncul di versi ES6. Cara penulisannya diselimuti dengan \`backtick\` lalu variabel-nya diselimuti dengan ${}. Membuat penulisan lebih mudah, rapi, dan cepat.

```js
var full_name = `${first_name} ${last_name}`;

console.log(full_name); // "Minatozaki Sana"
```

### Includes

Includes adalah fungsi milik variabel yang bertipe data string.

Gunanya adalah untuk mencari tahu apakah ada suatu kata atau karakter dalam suatu kalimat. Jika ketemu maka fungsi tersebut akan mengembalikan nilai ```true``` jika sebaliknya maka ```false```.

Perlu dicatat bahwa fungsi ```includes``` ini bersifat ```Case-Sensitive``` atau dalam kata lain kita wajib memerhatikan besar kecilnya huruf.

```js
var full_name = `${first_name} ${last_name}`;

var ketemu = full_name.includes("Sana");
console.log(ketemu); // true

var tidak_ketemu = full_name.includes("sana");
console.log(tidak_ketemu); // false
```

### Replace

Seperti namanya, fungsi ```replace``` adalah mengganti kata atau karakter dengan yang lain.

Juga ```Case-Sensitive```.

```js
var original_name = "Minatozaki Sana";

var terganti = teks.replace("Minatozaki", "Kim");
console.log(terganti); // Kim Sana

var gagal_terganti = teks.replace("minatozaki", "Kim");
console.log(terganti); // Minatozaki Sana
```

## Tugas

Oke, sekarang kerjakan tugas berikut:

1. Buat variabel dengan value ```Choa Tzaya```
2. Replace agar hasilnya menjadi ```Chou Tzuyu```. Jangan replace langsung variabel nya :)
3. Tampilkan hasilnya ke layar