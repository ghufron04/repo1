Async await dan Catch

menangkap promise dengan async await
contoh :

    let nonton3 = (kondisi) =>{
        return new Promise((resolve,reject)=>{
            if(kondisi == "jalan"){
                resolve("nonton terpenuhi")
            }
            reject("batal nonton coi")
        })
    }

    async function asinkNontonton (){
        let result = await nonton3("jalan")
        console.log(result)
    }

menggunakan try catch untuk error handler

contoh :

    async function asinkNontonton (){
        try{
        let result = await nonton3("alan")
        console.log(result)  
        } catch (error){
            console.log(error)
        }

    }

fetch => object promise
menangkapnya dengan then catch atau async await

contoh dengan then catch

      fetch("https://digimon-api.vercel.app/api/digimon")
    .then(result => {
        console.log(result)
        return result.json()
    })
    .then(result => {
        console.log(result)
    })

contoh dengan async await :

    let getDataDigimon = async () => {
        let response = await fetch("https://digimon-api.vercel.app/api/digimon")
        let result = await response.json()
        console.log(result)
    }
    getDataDigimon()


Git dan Git hub lanjutan

-Melakukan Clone /download pada repository
-colab dengan membuat organisasi di github
-switch/checkout digunakan untuk berbindah branch
-git merge dev untuk menghindari konflik di github
-untuk mengepush pada branch git push -u origin (nama branch)
-melakukan pull request
-melakukan pull dan merge regis/log dari branch dev ke A/B
-konlik terjadi ketika ada 2 atau lebih orang yang mengedit satu file yang sama


Responsive Web Design
          
kegunaan meta viewport : adalah salah satu cara agar web site menjadi responsif
gambar menjadi responsif deangan max-width
menggunakan css relatif unit em dan rem
perbedaan antara persen(%) dan vw adalah persen mengikuti div dan vw akan mengikuti ukuran layar


Media Query

menggunakan kondisi dimana jika kondisi terpenuhi maka settingan yang diatur akan diaplikasikan
flex hanya horizontal
grid vertikal dan horizontal


Bootstrap

bootstrap adalah framework css untuk mempermudah styling pada website

Breakpoints pada bootstrap

Breakpoints adalah the building blocks dari desain responsif. Digunakan untuk mengontrol kapan tata letak dapat disesuaikan pada area pandang atau ukuran perangkat tertentu.
Menggunakan media query untuk merancang CSS dengan breakpoint. media query adalah fitur CSS yang memungkinkan menerapkan gaya secara kondisional berdasarkan sekumpulan parameter browser dan sistem operasi.
