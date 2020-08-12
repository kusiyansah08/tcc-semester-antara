Docker adalah platform terbuka yang membantu distribusi aplikasi secara universal. Docker telah menjadi standar untuk beberapa jenis sistem virtualisasi container dan telah diadopsi oleh berbagai perusahaan sebagai strategi container perangkat lunak.
Filosofi di balik Docker adalah untuk membantu memberikan eksekusi universal, menggunakan properti inheren kernel Linux yang menawarkan dukungan untuk penanganan aplikasi yang lebih mudah. Sebagai contoh, daripada menggunakan metode yang memungkinkan library interdependency, Docker memberikan pemisahan yang mulus, di mana library yang diberikan dipasang beberapa kali dalam container yang berbeda sehingga setiap instance individual library tidak saling bergantung dengan yang lain.
Pada LearnFazz, docker digunakan untuk melakukan deploy untuk server back-end dan database. Deployment ini dilakukan menggunakan https://portainer.docker.ppl.cs.ui.ac.id yang merupakan Docker yang telah disiapkan oleh Fakultas Ilmu Komputer UI.


Menyiapkan image
Image Docker adalah file, terdiri dari beberapa lapisan, yang digunakan untuk mengeksekusi kode dalam container Docker. Sebuah image pada dasarnya dibangun dari instruksi untuk versi aplikasi yang lengkap dan dapat dieksekusi, yang bergantung pada kernel OS host.

Menyiapkan volume
Pengaturan default Docker adalah melakukan penyimpanan pada container. Namun, untuk database, datanya dapat berubah sehingga dibentuklah volume


Menyiapkan network
Fungsi dari network adalah untuk memungkinkan komunikasi antar container. Driver yang digunakan pada network adalah bridge. Penggunaan bridge memungkinkan container yang ditempatkan pada network yang berbeda tetap bisa berkomunikasi.



Membuat container
Container adalah instansi dari suatu image yang sedang berjalan. Pada proyek kami, kami membuat container sebanyak jumlah environment yang ada. Untuk mempermudah pembuatan container, kami menggunakan Docker compose




