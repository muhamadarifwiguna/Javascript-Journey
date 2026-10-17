# Variabel

## Definisi Singkat

Variabel ialah “simpanan bernama” untuk data. Kita bisa memakainya untuk \
menyimpan barang, pengunjung, dan data lain.

## Analogi kehidupan sehari-hari

Bayangkan variabel itu seperti kotak penyimpanan barang atau sebuah wadah di dalam gudang yang diberi label nama. Di dalam kotak itu, kamu bisa menyimpan berbagai macam "barang" (data) seperti angka, teks, atau data yang lebih kompleks, lalu mengambil atau mengubah isinya kapan pun kamu butuh menggunakan label (nama) tersebut.

## Fungsi

- **Menyimpan Data Sementara:** Untuk menampung nilai yang nantinya akan diproses oleh program.
- **Membuat Kode Dinamis:** Nilai di dalam wadah bisa diubah-ubah selama program berjalan.
- **Mencegah Pengulangan Nilai (Reusability):** Daripada menulis nilai yang sama berulang-ulang di banyak tempat, cukup simpan sekali di dalam variabel dan panggil namanya.

## Syntax

```javascript
let message;

message = "Hello"; // simpan string
alert(message); // tampilkan isi variabel
```

kita juga bisa mengubah nilainya sebanyak yang kita mau.

```javascript
let message;

message = "Hello!";

message = "World!"; // value changed

alert(message);
```

Kita juga bisa mendeklarasi dua variabel dan mengkopi data dari satu ke yang lainnya.

```javascript
let hello = "Hello world!";

let message;

// mengkopi 'Hello world' dari hello ke message
message = hello;

// sekarang dua variabel punya data yang sama
alert(hello); // Hello world!
alert(message); // Hello world!
```

## Penamaan Variabel

Ada dua keterbatasan pada nama variabel di JavaScript:

1. Nama hanya boleh mengandung huruf, digit, atau simbol seperti $ and \_.
2. Karakter pertama tidak boleh digit.
3. Ketika namanya mengandung kata ganda, camelCase umum digunakan: kata demi kata digabung, setiap kata kecuali yang pertama dimulai dengan huruf kapital: _myVeryLongName._

Nama-nama ini valid dan manariknya dapat menggunakan tanda $ atau \_.

```javascript
let $ = 1; // menggunakan "$"
let _ = 2; // menggunakan "_"

alert($ + _); // 3
```

Sedangkan, nama-nama ini tidak valid.

```javascript
let 1a; // Karakter pertama tidak boleh digit.

let my-name; // hanya $ dan _ yang diperbolehkan.
```

Ada juga nama-nama yang tidak diperbnolehkan. Misalnya: _let, class, return,_ dan _function_ dikecualikan.

```javascript
let let = 5;
let return = 5;
```
