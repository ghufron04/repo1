SCOPE

Scope adalah konsep dalam flow data variabel. 
Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

Blocks adalah code yang berada didalam curly braces {}.
Conditional, function, dan  looping menggunakan blocks.

Global scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.
Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.

Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.
Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks.

FUNCTION

Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur.
Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.

Parameter Function
Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.
Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan. Misalnya saat membuat function penambahan 2 buah nilai. Data yang dibutuhkan adalah 2 buah nilai tersebut.

Argumen Function
Argumen adalah nilai yang digunakan saat memanggil function.
Jumlah argumen harus sama dengan jumlah parameternya
Jadi jika di function penambahan ada 2 parameter nilai saat membuat function. Saat memanggil function kita gunakan 2 buah nilai argumen.

Default Parameter
Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.
Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen

Function Helper
Kita bisa menggunakan function yang sudah dibuat pada function lain.

Arrow Function
Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

Short Syntax Function
Zero Parameters 
const functionName = () => {};

One Parameters
const functionName = paramOne => {};

1< Parameters 
const functionName = (paramOne, paramTwo) => {};

Single line Block
const sumNumbers = number => number + number;

Multi line Block
const sumNumbers = number => {
	const sum = number + numner;
	return sum;
};


Data Type Built in Prototype & Method

JavaScript types

Primitive values

-Boolean type

Boolean mewakili entitas logis dan dapat memiliki dua nilai: benar dan salah

-Null type

Tipe Null memiliki tepat satu nilai: null

-Undefined type

Variabel yang belum diberi nilai memiliki nilai yang tidak terdefinisi (undefined)

-Number type

-BigInt type

BigInt adalah tipe data primitif numeric dalam JavaScript yang dapat mewakili bilangan bulat dengan presisi arbitrer(penengah).

-String type

Jenis JavaScript String digunakan untuk mewakili data tekstual.

-Objects

Dalam JavaScript, objek dapat dilihat sebagai kumpulan properti.

typeof untuk mengecek tipe data sebuah value.

properti lenght digunakan untuk mengecek panjang karakter/array.

method string toUpperCase untuk membuat value string menjadi kapital. method string toLowerCase untuk membuat value string menjadi kecil.

charAt metode mengembalikan karakter pada indeks tertentu dalam sebuah string.

includes metode untuk mencari karakter atau string di dalam string

method isNall untuk mengecek Itu adalah number atau bukan. method toString untuk mengubah number menjadi string. toFixed method yang mirip dengan toString.

parseInt dan parseFloat digunakan untuk mengubah string menjadi number


DOM HTML

Document Object Model(DOM) adalah sebuah API yang menyediakan fungsi-fungsi untuk memanipulasi dokumen.
Objek dari dokumen ini menyediakan sekumpulan fungsi dan atribut/data yang bisa kita manfaatkan dalam membuat program Javascript. Inilah yang disebut Application Programming Interface (API)

Ada beberapa cara untuk mengakses element di dalam HTML:
- getElementById = dengan ID
- getElementByClass = dengan class
- getElementByTag = dengan tag name

DOM Manipulasi

innerHTML

innerHTML adalah sebuah atribut di dalam (objek) elemen HTML yang berisi string HTML. Dengan innerHTML, kita dapat menampilkan output ke elemen yang lebih spesifik.

innerText

innerText fungsinya adalah untuk menentukan dan mengembalikan nilai konten dari suatu element dalam bentuk text atau string

createElement

append dan appendchild (hanya bisa menyisipkan sebuah node)

HTML DOM Event
EventListener
-click
-blur
-form submission