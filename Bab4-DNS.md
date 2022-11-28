# Bab 4
## server DNS
### 1. Apa itu DNS?
DNS akronim dari Domain Name Sytem. DNS adalah sebuah sistem yang bertugas menyimpan informasi nama domain dan IP address. DNS juga dapat digunakan untuk mengubah nama domain menjadi IP address dan sebaliknya. DNS juga dapat digunakan untuk mengubah nama domain menjadi IP address dan sebaliknya digunakan untuk mengakses website. DNS server juga dapat digunakan untuk mengakses email server.

DNS server merupakan sebuah server yang berfungsi untuk menghubungkan antara nama domain dengan IP address. pengelolaan DNS terdiri dari 3 komponen yaitu: Root DNS Server, Top Level Domain (TLD) DNS Server, Authoritative DNS Server. Root DNS Server merupakan server DNS yang pertama kali diakses oleh client. Root DNS Server berfungsi untuk mengarahkan client ke TLD DNS Server. TLD DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Secara umum DNS server terdiri dari 2 jenis yaitu Primary DNS Server dan Secondary DNS Server. Primary DNS Server merupakan server DNS yang pertama kali diakses oleh client. Primary DNS Server berfungsi untuk mengarahkan client ke TLD DNS Server. Secondary DNS Server merupakan server DNS yang kedua yang diakses oleh client. Secondary DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server. Secondary DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server.

### 2. persiapan
Kita akan menggunakan 1 workstation, 1 switch dan 2 server. Tampilannya sebagaimana berikut ini:

![image](https://i.insider.com/602c130c2edd0f001a8d5ed9?width=900&format=jpeg&auto=webp)

### 3. Konfigurasi
1. Lakukan konfigurasi Static IP sebagai berikut:

|Device|IP Address|Subnet Mask|
|:-|:-|:-|
|Server0|192.168.123.1|255.255.255.0|
|Server1|192.168.123.2|255.255.255.0|
|Pada PC0|192.168.123.3|255.255.255.0|

Jangan lupa mengisi DNS Server pada konfigurasi IP Address. DNS Server yang digunakan adalah IP Address dari Server0.

2. Aktifkan layanan HTTP pada server0. Langkah-langkahnya sama seperti bahasa sebelumnya.

3. Double klik Server 1 hingga muncul jendela properties. Pada jendela tersebut, pilih tab DNS. Pada bagian DNS Server Address, masukkan IP Address dari Server0. Klik OK.
4. Pindahkan tab ke tab config. Pada bagian menu services, centang layanan DNS Server. Klik OK.
5. Field domain name isi dengan nama domain yang akan digunakan. Pada contoh ini, kita akan menggunakan domain cisco.com. Klik OK.
6. Pada bagian Forward Lookup Zones, klik kanan dan pilih New Zone. Pada jendela New Zone, masukkan nama domain yang akan digunakan. Pada contoh ini, kita akan menggunakan domain cisco.com. Klik OK.
7. Tambahkan record A pada domain cisco.com. Klik kanan pada domain cisco.com dan pilih New Host (A). Pada jendela New Host (A), masukkan nama host dan IP Address. Klik OK.
8. Kemudian, buka browser dan ketikkan nama host yang telah dibuat.

### 4. Penjelasan

  * Pada Server0, kita mengaktifkan layanan HTTP. Hal ini dilakukan agar kita dapat mengakses website yang ada pada Server0.
  * Pada Server1, kita mengaktifkan layanan DNS Server. Hal ini dilakukan agar kita dapat mengakses website yang ada pada Server0.
  * Pada Server1, kita menambahkan record A pada domain cisco.com. Record A berfungsi untuk mengarahkan client ke IP Address yang diminta. Pada contoh ini, kita menambahkan record A dengan nama host www.cisco.com dan IP Address
  * Pada PC0, kita mengisi DNS Server dengan IP Address dari Server0. Hal ini dilakukan agar PC0 dapat mengakses website yang ada pada Server0.
  * Pada PC0, kita mengakses website yang ada pada Server0 dengan cara mengetikkan nama host yang telah dibuat. Pada contoh ini, kita mengakses website dengan cara mengetikkan www.cisco.com.

### 5. Kesimpulan
DNS merupakan sebuah sistem yang bertugas menyimpan informasi nama domain dan IP address. DNS juga dapat digunakan untuk mengubah nama domain menjadi IP address dan sebaliknya. DNS juga dapat digunakan untuk mengubah nama domain menjadi IP address dan sebaliknya digunakan untuk mengakses website. DNS server juga dapat digunakan untuk mengakses email server.

DNS server merupakan sebuah server yang berfungsi untuk menghubungkan antara nama domain dengan IP address. pengelolaan DNS terdiri dari 3 komponen yaitu: Root DNS Server, Top Level Domain (TLD) DNS Server, Authoritative DNS Server. Root DNS Server merupakan server DNS yang pertama kali diakses oleh client. Root DNS Server berfungsi untuk mengarahkan client ke TLD DNS Server. TLD DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Authoritative DNS Server berfungsi untuk mengarahkan client ke IP address yang diminta. Secara umum DNS server terdiri dari 2 jenis yaitu Primary DNS Server dan Secondary DNS Server. Primary DNS Server merupakan server DNS yang pertama kali diakses oleh client. Primary DNS Server berfungsi untuk mengarahkan client ke TLD DNS Server. Secondary DNS Server merupakan server DNS yang kedua yang diakses oleh client. Secondary DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server. Secondary DNS Server berfungsi untuk mengarahkan client ke Authoritative DNS Server.

Dari percobaan yang telah dilakukan, kita dapat mengakses website yang ada pada Server0 dengan cara mengetikkan nama host yang telah dibuat. Pada contoh ini, kita mengakses website dengan cara mengetikkan www.cisco.com. Pada percobaan ini, kita menggunakan 2 server yaitu Server0 dan Server1. Server0 berfungsi untuk mengakses website. Server1 berfungsi untuk mengarahkan client ke IP Address yang diminta. Pada percobaan ini, kita menggunakan 2 server yaitu Server0 dan Server1. Server0 berfungsi untuk mengakses website. Server1 berfungsi untuk mengarahkan client ke IP Address yang diminta. Pada percobaan ini, kita menggunakan 2 server yaitu Server0 dan Server1. Server0 berfungsi untuk mengakses website. Server1 berfungsi untuk mengarahkan client ke IP Address yang diminta.