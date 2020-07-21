Kubernetes adalah salah satu produk open source untuk sistem manajemen container

Sama seperti docker swarm, kubernetes dapat melakukan manajemen container, akan tetapi kubernetes merupakan produk yang akan terus berkembang dan akan lebih banyak digunakan dibandingkan dengan docker swarm. Salah satu kelebihan dari kubernetes adalah kita dapat menggunakan kubernetes dashboard untuk memonitoring container, kita dapat melakukan deployment melalui dashboard dan pastinya struktur yang diusulkan oleh kubernetes dan docker swarm sangatlah berbeda. Berikut adalah struktur yang biasanya digunakan di dalam kubernetes.


Instalasi Kubernetes
Pada artikel ini, kita akan menggunakan 2 buat vm yaitu :

- VM Master : berfungsi sebagai node master, master disini berfungsi untuk mendeploy container ke dalam node worker kubernetes.
- VM Worker : berfungsi sebagai node worker.


Requirment Node Master
Adapun kebutuhan untuk node master adalah :

- Ram 3 GB
- Disk 10 GB
- Bridge Network
- IP 192.168.88.100
- Ubuntu 16.04 Server



Requirment Node Worker
Adapun kebutuhan untuk node worker adalah :

- Ram 2 GB
- Disk 10 GB
- Bridge Network
- IP 192.168.88.101
- Ubuntu 16.04 Server


Dengan requirment diatas, silahkan lakukan instalasi ubuntu server pada 2 vm tersebut yaitu pada vm master dan vm worker. IP yang digunakan disini adalah IP static, sehingga anda perlu melakukan sedikit konfigurasi pada jaringan ubuntu server.

Untuk melakukan instalasi kubernetes, anda wajib melakukan instalasi docker terlebih dahulu, bagi yang belum mengerti docker, silahkan baca artikel Belajar Docker


Setup Kubernetes

Setelah selesai melakukan instalasi kubernetes, tahapan selanjutnya adalah kita akan melakukan setup kubernetes. Setup kubernetes akan dilakukan secara bertahap, yaitu dilakukan pada node master terlebih dahulu kemudian akan dilakukan pada node worker.
