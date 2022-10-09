Array
Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya.Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya.
Array pada javascript dihitung dari index data ke-0.Data pertama adalah index ke-0.
Seperti tipe data dan variabel pada umumnya, kita dapat mengupdate data pada Array

Const pada array
=Jika menggunakan let, kita dapat mengubah array  dengan array baru dan konten nilai yang ada di dalam array dengan nilai lain
=Const tidak bisa melakukan update data. Namun pada Array kita dapat melakukan update konten nilai di dalam array (mutable).
=Yang tidak bisa adalah mengubah array dengan array yang baru jika menggunakan const

Array memiliki 5 properti yang sering digunakan yaitu constructor, length, index, input, dan prototype.
Kita hanya membahas length. Untuk yang lainnya kamu bisa cek di link ini array properties and method
Properties adalah fitur yang sudah disediakan oleh Javascript untuk memudahkan developer.
Array memiliki method atau biasa disebut built-in methods.Artinya Javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan.
Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia.
Sama halnya dengan Array properti. Kita bisa cek dokumentasi untuk melihat method yang sudah tersedia pada link ini built-in methods atau MDN documentation

Looping pada array
Array memiliki built in methods untuk melakukan looping yaitu .map() dan .forEach()
Kita harus tahu kapan menggunakan .map() dan juga .forEach()
-.forEach() adalah method untuk melakukan looping pada setiap elemen array.
-.map() melakukan perulangan/looping dengan membuat array baru.
.map() dan .forEach() sama-sama melakukan looping dan mengembalikan nilai baru dari operasi yang dilakukan. Perbedaannya adalah .forEach tidak dapat membuat Array baru dari hasil operasi yang ada dalam looping. Lalu dari segi performance juga sangat jauh.
Jadi, gunakan .forEach() jika hanya memerlukan looping untuk menampilkan saja atau menyimpan ke database.
Gunakan .map() jika akan melakukan operasi pada array seperti yang dapat mengubah nilai array sebelumnya.

Multidimensional Array
Multidimensional Array bisa dianalogikan dengan array of array.Ada array didalam array.
Bayangkan multidimensional ini seperti Table.Baris pada table itu menunjukan jumlah array.Column pada table itu menunjukan isi dari tiap array.
Sama seperti array satu dimensi, multidimensional array juga dapat menggunakan Property dan Method built-in Array.

Object
Dalam kehidupan nyata, kita sebenarnya sudah sering menjumpai object.Entah itu benda mati atau benda hidup. Semuanya adalah object. 
Object didunia nyata dapat kita modelkan didalam programming.Jadi pada programming, object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)
Properti adalah data lengkap dari sebuah object.Method adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.
Object adalah salah satu tipe data yang sudah kita pelajari dalam materi javascript.
Sama seperti tipe data sebelumnya. Object dapat diassign kedalam sebuah variabel.
Sama seperti array, didalam object kita dapat menyimpan properti dengan tipe data apapun.
Kita dapat melakukan update pada variabel dengan tipe data Object.
-Object dapat mengupdate value dari key yang sudah tersedia
-Object dapat menambahkan key dan value baru
-Jika menggunakan constant pada variable object. Kita tidak bisa mengganti seluruh data object dengan object yang baru.
Jadi jika membutuhkan untuk update seluruh data object gunakan ‘let’ pada saat deklarasi variabel.
Kita dapat menghapus properti dari object menggunakan delete operator.

method
Jika value yang kita masukkan pada property berupa function.Maka itu disebut method. console adalah global javascript object.
log() adalah property yang berupa function dari object console. Sehingga kita memanggila dengan cara console.log().
pass by reference
Kita bisa mengubah data yang ada pada object melalui sebuah function dan memasukkan object sebagai parameter function.
Ini biasa disebut passed by reference.
looping object
Jika kita ingin menampilkan seluruh object properti. Kita bisa menggunakan looping. Jadi tidak perlu mengakses secara manual memanggil setiap propertinya.

Recursive
Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu.
Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.

Ciri dari rekursif:
-Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar.
-Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

Web Storage

Cookies
Cookies adalah data kecil yang dikirim dari situs web dan disimpan di komputer kita oleh web browser saat kita menjelajah. Disebut data kecil karena maksimum data yang dapat disimpan dalam cookies adalah 4096 bytes (4 KB).
Biasanya data yang disimpan di cookies adalah access token pengguna saat login atau data pencarian saat melakukan pencarian pada situs web tertentu. Hal ini yang biasanya dilakukan oleh situs pencarian untuk melacak pencarian kita dan menampilkan iklan yang berhubungan dengan pencarian kita sebelumnnya.

Namun ada beberapa kekurangan yang perlu kita perhatikan mengenai cookies di antaranya:
-Setiap kita mengakses situs web, cookies juga kembali dikirim sehingga memperlambat aplikasi web kamu dengan mengirimkan data yang sama.
-Cookies disertakan pada setiap HTTP request, sehingga mengirimkan data yang tidak dienkripsi melalui internet, maka saat kita ingin menyimpan data dalam cookies kita harus mengenkripsinya terlebih dahulu.
-Cookies hanya dapat menyimpan data sebanyak 4KB.
-Lalu cookies juga memiliki tanggal kadaluarsa. Tanggal ini telah ditentukan sehingga web browser bisa menghapus cookies jika tanggal sudah kadaluarsa atau tidak dibutuhkan.
Kita dapat memanfaatkan jenis web storage yang lain untuk mengatasi kekurangan yang dimiliki cookies.
Local Storage dan Session Storage
Dengan memanfaatkan local storage dan session storage, kita dapat menyimpan data lebih besar yaitu 5MB per page tanpa mempengaruhi kinerja situs web. Namun, penting untuk diketahui agar kita tidak menyimpan data sensitif seperti password ke dalam local storage ataupun session storage untuk menghindari serangan pencurian data. Pada lesson ini kita akan fokus mempelajari keduanya.

Local Storage
Local storage memiliki karakteristik sebagai berikut:
-Menyimpan data tanpa tanggal kadaluarsa.
-Data tidak akan dihapus ketika web browser ditutup dan akan tersedia seterusnya selama kita tidak menghapus data local storage pada web browser.
-Dapat menyimpan data hingga 5MB.
-Hanya dapat menyimpan data string.
-Untuk menyimpan data pada local storage, kita menggunakan method setItem() yang membutuhkan 2 parameter. Parameter pertama adalah key yang ingin kita simpan dan parameter kedua adalah data (value) dari key yang akan disimpan.

Session Storage
Berbeda dengan local storage, walaupun masuk ke dalam web storage, data yang tersimpan pada session storage akan hilang ketika session dari sebuah laman berakhir.

Session storage mempunyai beberapa karakteristik, yaitu:
-Data yang disimpan pada session storage akan terus tersimpan selama browser terbuka dan tidak hilang jika laman di-reload.
-Membuka banyak tab/window dengan URL yang sama, akan menciptakan session storage yang berbeda di masing-masing tab/window.
-Menutup tab/window akan mengakhiri session dan menghapus data yang tersimpan di session storage pada tab/window tersebut.
-Data yang tersimpan dalam session storage harus berbentuk string.
-Hanya dapat menyimpan data sebanyak 5MB.

Asynchronous
Javascript adalah bahasa pemrograman single-thread yang artinya hanya dapat mengeksekusi satu task pada satu waktu atau biasa disebut synchronous.
Pada konsep pemrograman (web development pada case kita) dikenal istilah Asynchronous. Asynchronous mengizinkan komputer memproses task yang lain sambil menunggu proses yang masih berlangsung.
Kita bisa membuat asynchronous secara simulasi artinya tidak murni asynchronous dengan beberapa cara:
-Callback
-Promises
-Async/Await

callback
Callback function adalah function yang kita letakan di dalam argumen/parameter pada function, dan function tersebut akan dieksekusi setelah function pertama menyelesaikan tugasnya.
Proses asynchronous identik dengan delay, dimana hasil dari proses tersebut membutuhkan selang waktu tertentu untuk menghasilkan output. Kita akan menemukan proses asynchronous pada proses Ajax, komunikasi HTTP, Operasi file, timer, dsb
setTimeout digunakan untuk simulasi asynchronous. Karena sebenarnya kita tidak bisa membuat proses asynchronous murni.

Promise
a Promise is an object that may produce a single value some time in the future: either a reloved value, or a reason that it's not resolved. -Eric Elliot.
Promise adalah salah satu fitur baru di ES6, biasa digunakan untuk melakukan http request/fetch data dari API.
Dalam pengambilan data, promise memiliki 3 kemungkinan state.
-Pending(sedang dalam proses)
-Fulfilled (berhasil)
-Rejected (gagal)

Async-await
Async - await adalah salah satu fitur baru dari javascript yang digunakan untuk menangani hasil dari sebuah Promise. Sedangkan await berfungsi untuk menunda sebuah kode dijalankan sampai proses asynchronous berhasil.
HTTP request fetch()
Fetch adalah native web API untuk melakukan HTTP calls dari external network.




