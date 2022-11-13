Sequelize
----------------------------------
Sequelize dengan migration

menjalankan migration : "npx sequelize cli db:migrate"

undo migration : reverts a migration.

migration menjalankan sesuai urutan filenya.

migration menjalankan struktur tabel.

mengisi data dummy : npx sequelize seed:create --name demo-user

menjalankan seed : npx sequelize db:seed --seed 'nama seed'

MongoDB
----------------------------------

Database noSQL

SQL biasanya menyimpan data dengan relasi tabel, MongoDB menggunakan dokumen dengan format JSON.

maksud noSQL?

adalah dalam mengelola database tidak membutuhkan Query atau fleksibel.


contoh collection

    Collection

    embed			reference

    cars			      cars		    	      user
    {			
                        {		  	       {
     nama :		     	  nama :			    id:
     merk :			      warna:		      nama:
     user : {		      merk :			  alamat:
             nama:		  user : objid		}
             age: 	     }
             address:
             }
     }

Mongoose
----------------------------------
koneksi database

skema model

Mongoose

Adalah library object modelling dari mongodb untuk nodejs.

Mongoose dapat digunakan untuk mengelola koneksi antara data. dan digunakan untuk menerjemahkan antara objek dalam kode dan objek di mongoDB.

populate berkaitan dengan relasi database. merupakan penggabungan dua collection atau lebih menjadi satu objek json.


Docker
----------------------------------
merupakan software yang menjalankan sebuah aplikasi menggunakan container( mirip seperti virtual machinenya oracle virtual box).

Docker menyebarkan kernel dari host OS, dan meng-container-kan suatu aplikasi agar bisa dijalankan dimana saja kapan saja.

Docker berfungsi sebagai penyedia layanan virtual bagi aplikasi yg diinstall pada sebuah host. 

Docker akan menyediakan hal-hal yang diperlukan untuk aplikasi mulai dari akses file, koneksi internet, hingga port agar aplikasi dapat berjalan dengan mulus

kenapa harus docker?

secara menyeluruh docker lebih enteng dibanding vm walau sebenarnya docker masih tergolong berat.

Docker Fundamental

    1.Docker File     : blueprint image
    2.Image           : template menjalankan container
    3.Container       : wujud dari image
    4.Docker Registry : Tempat download atau upload image.