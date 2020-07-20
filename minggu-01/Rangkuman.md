<h1>Pengantar Teknologi Cloud Computing</h1>

Jika kita diminta meringkas komputasi awan dengan empat kata kunci yang bisa kita bicarakan
pilih 'web', 'elastisitas', 'utilitas' dan 'skalabilitas'. Dalam bab ini, kita akan melihat teknologi dasar cloud. Aplikasi cloud diakses melalui
web, dan teknologi web adalah bagian integral dari cloud, jadi kita akan mulai dengan singkat meninjau keadaan terkini teknologi web. Kita kemudian akan beralih ke virtualisasi, sebuah teknologi cloud kunci yang memiliki banyak manfaat termasuk penggunaan yang lebih baik pada sumber daya. Virtualisasi dapat digunakan untuk memberikan elastisitas yang dibutuhkan untuk menawarkan awan komputasi sebagai utilitas. Kami kemudian mengalihkan perhatian kami ke pemrograman MapReduce model, awalnya dikembangkan oleh para pendiri Google dan sekarang biasa menyediakannya skalabilitas untuk banyak aplikasi terdistribusi yang khas dari awan dan terlalu besar untuk ditangani dalam kerangka waktu yang user-friendly oleh sistem tradisional.
	Di akhir bab ini, Anda akan dipandu melalui proses penciptaan
Mesin virtual Anda sendiri (VM) menggunakan VMWare dan open source Ubuntu (Linux)sistem operasi. Anda kemudian akan menjalankan pekerjaan MapReduce sederhana menggunakan virtual mesin anda. Kita akan menggunakan VM ini lagi di bab selanjutnya.

Teknologi Web 

Fitur aplikasi web dan cloud adalah sejumlah teknologi terpisah
diminta untuk bekerja sama. Aplikasi web minimum cenderung menggunakan HTTP,
XHTML, CSS, JavaScript, XML, pemrograman server (misalnya PHP) dan beberapa mekanisme untuk bertahan data (untuk diperiksa secara rinci di bab berikutnya). Kami akan memperkenalkan teknologi ini secara singkat disini; Jika Anda sudah terbiasa dengan teknologi web Anda dapat dengan aman melewatkan bagian ini. Di sisi lain, jika Anda benar-benar baru
Untuk teknologi web, Anda mungkin lebih suka memulai dengan mengerjakan tutorial dasar untuk HTML, CSS, JavaScript dan XML di situs W3 yang sangat baik: http: // www.w3schools.com/


HTTP

Sistem cloud dibangun di World Wide Web, dan web dibangun di atas dasar
sistem komunikasi jaringan yang dikenal sebagai HTTP atau Hypertext Transfer Protocol. HTTP adalah kunci untuk membangun sistem awan, dan pada tingkat rendah, setiap interaksi dalam aplikasi cloud menggunakan HTTP (Nixon 2009).
	Berners-Lee (yang awalnya mengusulkan World Wide Web) dan timnya adalah dikreditkan dengan menemukan HTTP asli. Versi pertama hanya memiliki satu metode,yaitu, GET, yang digunakan saat pengguna membuat permintaan untuk halaman web dari server. Sejumlah metode lain sejak itu telah ditambahkan termasuk:
-	HEAD yang meminta server untuk informasi tentang sumber daya
-	PUT yang menyimpan data di resource
-	POST yang mengirimkan data ke sebuah program untuk diproses di server
-	DELETE yang menghapus sumber daya yang ditentukan
	HTTP menggunakan permintaan sederhana / respon siklus yang memungkinkan dua pihak, sering disebut sebagai klien dan server, untuk berkomunikasi.
Setiap permintaan HTML yang Anda buat menggunakan browser atau aplikasi memiliki tiga bagian:
-	Baris permintaan yang terdiri dari metode HTTP, URL sumber daya dan
versi protokol (biasanya HTTP 1.1)
-	Serangkaian baris header yang berisi metadata tentang sumber daya.
-	Body terdiri dari aliran data Permintaan HTTP yang khas mungkin terlihat seperti:
GET/cloud/book/chapter4 HTTP /1.1
User-Agent: Mozilla/5.001 (windows; U; NT4.0; en-US;
rv:1.0)
Host: cloud-principles-practices.appspot.com

Saat server merespons, baris pertama mencakup kode status 3 digit (sering kode yang ada dirangkum di bawah ini) dan pesan yang menunjukkan apakah atau tidak permintaan itu berhasil, misalnya, HTTP /1.1 200 OK. Semua yang dibutuhkan oleh proses server
harus dikirim secara eksplisit sebagai parameter.
