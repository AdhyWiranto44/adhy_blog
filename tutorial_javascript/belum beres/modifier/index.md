# Modifier

Keyword ```var``` ini ada lagi bentuknya, seperti ```let``` dan ```const```, mulai sekarang saya akan mengganti ```var``` dengan ```let```.

Nah, karena sudah disebutkan sekalian saja saya jelaskan.

Jadi ```let``` ini adalah versi baru dari ```var``` yang perbedaannya ada pada lingkupnya, di mana variabel ```let``` tidak bisa diakses di luar lingkupnya, misalkan di lingkup ```function``` maka tidak akan bisa diakses di luar ```function``` tersebut.

Lalu ada ```const``` dimana dia adalah keyword untuk membuat sebuah variabel yang isinya tidak bisa kita ubah setelah kita definisikan.

---

Sekarang kita bahas perbandingan ```var``` dengan ```let```.

```js
const tambah = (a,b) => {
  return a + b;
}

const num1 = 4;
const num2 = 5;
console.log(tambah(num1, num2));
```