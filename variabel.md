# Variable

_Variable_ adalah lokasi tertentu pada memori komputer yang digunakan untuk menyimpan data sementara. Bisa dianalogikan _variable_ itu seperti sebuah kotak kardus yang diberi nama, lalu diisi dengan barang-barang tertentu.

Ada beberapa cara untuk mendeklarasikan _variable_. Jika kita hendak menggunakan standar ECMAScript 5 maka kita akan menggunakan kata kunci `var`, seperti di bawah ini:

```javascript
var namaOrang = "Budi";
var umur = 42;
```

Jika kita hendak menggunakan standar ECMAScript 6 maka kita akan menggunakan kata kunci `let` atau `const`, seperti di bawah ini: 

```javascript
let namaOrang = "Budi";
let umur = 42;

const pi = 3.14;
const kota = "Jakarta";
```

Berikut ini beberapa  antara menggunakan `var`, `let`, dan `const`:

1. Variable scoping `let` dan `const` yang lebih baik dibanding `var`. Ini akan kita jelaskan lebih lanjut di bab khusus.

2. `let` dan `var` dapat diubah-ubah nilainya setelah didefinisikan. Contoh:

```javascript
let namaOrang = "Asep"; // saat ini nilainya Asep
namaOrang = "Didit"; // saat ini nilainya berubah menjadi Didit

var umur = 29; // saat ini nilainya 29
umur = 30; // lalu diubah menjadi 30
```

3. `const` nilainya tidak dapat diubah setelah didefinisikan. Contoh:

```javascript
const pi = 3.14; // sekarang nilainya 3.14
pi = 4; // akan terjadi error
```

## Pro Tips

1. Sebisa mungkin gunakan standar ES6 `let` dan `const` untuk mendeklarasikan _variable_, untuk mengurangi kesalahan-kesalahan akibat nilai _variable_ yang mungkin tidak sengaja berubah.
2. Sebaiknya gunakan nama _variable_ yang memiliki makna, misal: `let age`, `let umur`, `let tanggalSekarang`, `const salary`, dll. Hindari penggunaan nama yang hanya memiliki 1 huruf, seperti: `let a`, `let i`, dsb.
3. Nama _variable_ sebaiknya ditulis dengan format Camel Case, seperti ini:`let kecilBesar`, `let namaOrangTua`, dsb. 
