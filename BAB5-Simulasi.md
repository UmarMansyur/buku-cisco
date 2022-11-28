# BAB 5
## Simulasi Routing (Interconnect Network)

### 5.1.1. Topologi
Topologi adalah suatu jaringan yang terdiri dari beberapa node yang saling terhubung satu sama lain. Terdapat beberapa jenis topologi yang dapat digunakan dalam simulasi routing. Topologi yang digunakan dalam simulasi routing ini adalah topologi mesh. Topologi mesh adalah topologi jaringan yang terdiri dari beberapa node yang saling terhubung satu sama lain. Topologi mesh ini dapat digunakan untuk menghubungkan antar node dalam jaringan. Topologi mesh ini memiliki kelebihan yaitu dapat menghubungkan antar node dalam jaringan dengan mudah. Namun topologi mesh ini memiliki kekurangan yaitu jika terjadi kegagalan pada salah satu node maka akan mengakibatkan terputusnya jaringan. Topologi mesh ini dapat digunakan untuk menghubungkan antar node dalam jaringan. Topologi mesh ini memiliki kelebihan yaitu dapat menghubungkan antar node dalam jaringan dengan mudah. Namun topologi mesh ini memiliki kekurangan yaitu jika terjadi kegagalan pada salah satu node maka akan mengakibatkan terputusnya jaringan. Selain topologi mesh terdapat juga topologi bus, topologi ring, dan topologi star. Topologi bus adalah topologi jaringan yang terdiri dari beberapa node yang saling terhubung satu sama lain. Topologi bus ini memiliki kelebihan yaitu dapat menghubungkan antar node dalam jaringan dengan mudah. Namun topologi bus ini memiliki kekurangan yaitu jika terjadi kegagalan pada salah satu node maka akan mengakibatkan terputusnya jaringan. Topologi ring adalah topologi jaringan yang terdiri dari beberapa node yang saling terhubung satu sama lain. Topologi ring ini memiliki kelebihan yaitu dapat menghubungkan antar node dalam jaringan dengan mudah. Namun topologi ring ini memiliki kekurangan yaitu jika terjadi kegagalan pada salah satu node maka akan mengakibatkan terputusnya jaringan. Topologi star adalah topologi jaringan yang terdiri dari beberapa node yang saling terhubung satu sama lain. Topologi star ini memiliki kelebihan yaitu dapat menghubungkan antar node dalam jaringan dengan mudah. Namun topologi star ini memiliki kekurangan yaitu jika terjadi kegagalan pada salah satu node maka akan mengakibatkan terputusnya jaringan.

![topologimesh](https://1.bp.blogspot.com/-RZINsoZZu_c/XXId4FugTrI/AAAAAAAABFk/ZRp9BoL1vBwOdDJf2pvurvkNgbI_khXLwCPcBGAYYCw/s1600/Mesh-Topology.jpg) Gambar 5.1 Topologi Mesh

![topologiStar](https://blue.kumparan.com/image/upload/fl_progressive,fl_lossy,c_fill,q_auto:best,w_640/v1634025439/12840e5e238e727addd798c417c1c3092774f04de10480d2926796f8a3465210.png) Gambar 5.2 Topologi Star

![topologiBus](https://www.maxmanroe.com/vid/wp-content/uploads/2018/01/Pengertian-Topologi-Bus-jaringan.jpg) Gambar 5.3 Topologi Bus

![topologiRing](https://i1.wp.com/www.maxmanroe.com/vid/wp-content/uploads/2018/01/Pengertian-Topologi-Ring.jpg?fit=700%2C452&ssl=1ß) Gambar 5.4 Topologi Ring

Topologi yang digunakan pada simulasi ini adalah topologi bus. Topologi bus adalah topologi jaringan yang terdiri dari satu jalur yang menghubungkan semua node. Topologi bus ini memiliki kelebihan yaitu mudah dalam instalasi dan perawatan, namun memiliki kekurangan yaitu jika terjadi kerusakan pada jalur maka semua node akan terputus. 

### 5.1.2. Routing
Routing adalah proses untuk menentukan jalur yang akan dilalui oleh paket data dari satu node ke node lainnya. Routing ini dapat dilakukan dengan menggunakan algoritma routing. Algoritma routing yang digunakan pada simulasi ini adalah algoritma routing distance vector. Algoritma routing distance vector adalah algoritma routing yang mengirimkan informasi tentang jarak antar node. Algoritma routing distance vector ini memiliki kelebihan yaitu dapat mengirimkan informasi tentang jarak antar node, namun memiliki kekurangan yaitu jika terjadi perubahan pada jarak antar node maka akan mengakibatkan perubahan pada jalur yang akan dilalui oleh paket data. Selain algoritma routing distance vector terdapat juga algoritma routing link state dan algoritma routing path vector. Algoritma routing link state adalah algoritma routing yang mengirimkan informasi tentang jalur antar node. Algoritma routing link state ini memiliki kelebihan yaitu dapat mengirimkan informasi tentang jalur antar node, namun memiliki kekurangan yaitu jika terjadi perubahan pada jalur antar node maka akan mengakibatkan perubahan pada jalur yang akan dilalui oleh paket data. Algoritma routing path vector adalah algoritma routing yang mengirimkan informasi tentang jalur antar node. Algoritma routing path vector ini memiliki kelebihan yaitu dapat mengirimkan informasi tentang jalur antar node, namun memiliki kekurangan yaitu jika terjadi perubahan pada jalur antar node maka akan mengakibatkan perubahan pada jalur yang akan dilalui oleh paket data.

Pada simulasi ini algoritma routing yang digunakan adalah algoritma routing distance vector. Algoritma routing distance vector ini memiliki kelebihan yaitu dapat mengirimkan informasi tentang jarak antar node, namun memiliki kekurangan yaitu jika terjadi perubahan pada jarak antar node maka akan mengakibatkan perubahan pada jalur yang akan dilalui oleh paket data.

### Persiapan
Pada simulasi ini dibutuhkan 2 workstation, 2 swith dan 1 router. Sebagaimana pada gambar 5.5 dibawah ini.

![topologi](https://1.bp.blogspot.com/-ahWk9dlr1Bo/YGWa3XgqGzI/AAAAAAAAFdQ/ekcN7_PLkos3PTOFT2aAC1pZnEiFcnwmACLcBGAsYHQ/s568/4%2BIlustrasi%2BUntuk%2BDua%2BJaringan%2BBerbeda%2BTerhubung%2Bdengan%2BRouter0.png) Gambar 5.5 Topologi


Lakukan konfigurasi pada workstation (tanda merah pada gambar memilik arti sebagai ID host berdasarkan mask) sebagaimana tabel berikut:

IP Address|Subnet Mask|Gateway|
:--|:--|:--|
Pada workstation 1|192.168.1.1|255.255.255.0|192 168.1.5|
Pada workstation 2|10.0.0.1|255.0.0.0|10.0.0.5|

Keterangan:
1. Interface dengan IP Address 192.168.1.5 terkoneksikan secara fisik ke network 192.168.1.0
2. Interface dengan IP Address 10.0.0.5 terkoneksikan secara fisik ke network 10.0.0.0

Setelah itu lakukan konfigurasi sebagaimana berikut:

1. Double kil Router0 hingga muncul jendela konfigurasi properties Router0. Pilih tab configuration dan pilih interface FastEthernet0/0. Lalu masukkan IP Address pada interface 1 Router 0. Isikan IP Address yang sesuai dengan IP Address pada interface 1 workstation 1. Lalu klik OK. Berikut adalah hasil konfigurasi pada interface 1 Router 0.

2. Pastikan semua telah terkoneksi dengan baik degnen cara memeriksa routing table pada Router 0. Berikut adalah hasil routing table pada Router 0.

3. Pastikan semua telah terkoneksi dengan baik degnen cara memeriksa routing table pada workstation 1. Berikut adalah hasil routing table pada workstation 1.

| type| nwtwork | Port | Next Hop | Metrio |
| :-- | :-- | :-- | :-- | :-- |
| C | 10.0.0.0/8 | FastEthernet0/1 | --- | 0/0|
| C | 192.168.1.0/24| FastEthernet0/0 | --- | 0/0|ß

Keterangan:
Jika ip address yang melewati Router0 dan menuju network 10.0.0.0 dengan mask/8 maka paket data akan dilewati ke interface FastEthernet0/1. Type C berarti connected atau alamat yang dituju adalah alamat yang terhubung langsung dengan Router0 (workstation 1) sehingga tidak membuthkan Next Hop IP (Ip router lain).

### Konfigurasi Router Via CLI CISCO IOS
1. Masuk ke CLI CISCO IOS dengan cara klik kanan pada Router0 dan pilih Console. Berikut adalah tampilan CLI CISCO IOS. 

![gambar](https://i.ytimg.com/vi/nQ65Vq0UMrg/maxresdefault.jpg)

2. Ketik `n` pada prompt Continue with configuration dialog? [yes/no]: agar IOS langsung masuk ke CLI
3. Tekan Enter ketika muncul tulisan Press RETURN to get started!
4. Kemudian akan dimunculkan prompt Router> yang artinya kita sudah masuk ke CLI CISCO IOS. Mulai dari sini, disebut sebagai user mode. 
5. Untuk masuk ke privileged mode, ketikkan `enable` pada prompt Router> dan tekan Enter. Kemudian akan dimunculkan prompt Router# yang artinya kita sudah masuk ke privileged mode.
6. Jika muncul prompt Router# maka kita sudah masuk ke privileged mode. Untuk masuk ke global configuration mode, ketikkan `configure terminal` pada prompt Router# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config)# yang artinya kita sudah masuk ke global configuration mode.
7. Untuk mengatur IP Address pada interface 1 Router 0, ketikkan `interface fastEthernet0/0` pada prompt Router(config)# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config-if)# yang artinya kita sudah masuk ke interface configuration mode.
8. Untuk mengatur IP Address pada interface 1 Router 0, ketikkan `ip address 192.158.1.5 255.255.255.0` pada prompt Router(config-if)# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config-if)# yang artinya kita sudah masuk ke interface configuration mode.
9. ketik perintah `interfce fastEthernet0/0` setelah prompt Router(config)# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config-if)# yang artinya kita sudah masuk ke interface configuration mode.
10. Selanjutnya ketikkan `no shutdown` pada prompt Router(config-if)# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config-if)# yang artinya kita sudah masuk ke interface configuration mode.
11. Untuk keluar dari interface configuration mode, ketikkan `exit` pada prompt Router(config-if)# dan tekan Enter. Kemudian akan dimunculkan prompt Router(config)# yang artinya kita sudah keluar dari interface configuration mode.
12. Sampai tahap ini kita sudah berhasil mengatur IP Address pada interface 1 Router 0. Untuk melihat konfigurasi yang telah kita lakukan, ketikkan `show ip interface brief` pada prompt Router(config)# dan tekan Enter. Berikut adalah hasil konfigurasi yang telah kita lakukan. 
13. Lakukan hal yang sama untuk mengatur IP Address pada interface 2.

### Melakukan PING ke host di network lain
1. Pada workstation 1, buka command prompt dan ketikkan `ping 192.168.1.1 menuju  PC1(10.0.0.1).` Berikut adalah hasilnya.

![image](https://akupunyenetwork.com/wp-content/uploads/2021/07/VTP-ping-verifying.png)