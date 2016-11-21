# Conditional Statement

Saat kita menulis sebuah program, akan ada kondisi di mana program kita membutuhkan beberapa kemungkinan hasil. Pada saat itu lah kita akan membutuhkan _conditional statement_. Untuk membuat kondisi pada JavaScript kita menggunakan format berikut.

```javascript
if(value1 comparison_operator value2) {
    // blok kode untuk program jika kondisi true
} else {
    // blok kode untuk program jika kondisi false
}
```

Contoh penggunaannya seperti berikut ini.

```javascript
let gaji = 5500000;

if(gaji < 6000000) {
    console.log("Kamu pasti masih junior.");
} else {
    console.log("Levelmu sudah senior.");
}
```

Jika percabangan program kita lebih dari 1 kondisi, kita bisa menuliskan dengan cara seperti ini.

```javascript
let ongkos = 4500;

if(ongkos < 2000) {
    console.log("Tarif pelajar"); // true
} else if(ongkos > 2000 && ongkos < 5000) {
    console.log("Tarif normal"); // true
} else {
    console.log("Jangan lupa minta kembalian"); // false
}
```

`if ... else ...` juga bisa dibuat bersarang.

```javascript
let username = 'asepbagja';
let password = '123456';

if(username === 'asepbagja') {
    console.log('Username ditemukan'); // true
    
    if(password === '123456') {
        console.log('Login berhasil'); // true
    } else {
        console.log('Login gagal'); // false
    }
} else {
    console.log('Login gagal'); // false
}
```

## Pro Tips

Sebaiknya tidak membuat `if ... else ...` yang bersarang terlalu dalam, karena akan membuat alur program menjadi sulit dibaca.