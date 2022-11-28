# BAB 3
## Server HTTP

### 1. Apa itu HTTP?
HTTP adalah akronim dari Hypertext Transfer Protocol. HTTP adalah sebuah protokol request dan response antara client dan server. Sebuah cliet HTTP biasanya akan dimulai dengan request yang membuat hubungan TCP/IP ke port tertentu di tuan rumah server. Setelah hubungan TCP/IP dibuat, client akan mengirimkan request HTTP ke server. Server akan mengirimkan response HTTP ke client. Setelah response HTTP dikirimkan, hubungan TCP/IP akan ditutup. HTTP adalah protokol yang bersifat stateless, artinya setiap request yang dikirimkan oleh client tidak akan mempengaruhi request yang akan dikirimkan oleh client selanjutnya. Sebuah client HTTP biasanya akan membuat hubungan TCP/IP baru untuk setiap request yang akan dikirimkan. Selain itu, HTTP juga merupakan protokol yang bersifat text-based, artinya semua request dan response yang dikirimkan menggunakan format text. Secara umum, HTTP memiliki 4 metode request, yaitu GET, POST, PUT, dan DELETE. Metode GET digunakan untuk mengambil data dari server. Metode POST digunakan untuk mengirimkan data ke server. Metode PUT digunakan untuk mengubah data yang ada di server. Metode DELETE digunakan untuk menghapus data yang ada di server. HTTP juga memiliki 3 status code, yaitu 1xx, 2xx, dan 3xx. Status code 1xx digunakan untuk informasi. Status code 2xx digunakan untuk menandakan bahwa request telah berhasil diproses. Status code 3xx digunakan untuk menandakan bahwa client harus melakukan redirect ke URL lain.

Response HTTP biasanya terdiri dari 3 bagian, yaitu status line, header, dan body. Status line merupakan baris pertama dari response HTTP yang berisi status code dan status message. Header merupakan baris-baris yang berisi informasi tambahan mengenai response HTTP. Body merupakan bagian dari response HTTP yang berisi data yang dikirimkan oleh server. Secara umum, response HTTP memiliki 3 jenis header, yaitu general header, response header, dan entity header. General header merupakan header yang berlaku untuk semua request dan response. Response header merupakan header yang berlaku untuk response HTTP. Entity header merupakan header yang berlaku untuk data yang dikirimkan oleh server. Secara umum, response HTTP memiliki 3 jenis body, yaitu text, HTML, dan JSON. Body text merupakan body yang berisi data dalam format text. Body HTML merupakan body yang berisi data dalam format HTML. Body JSON merupakan body yang berisi data dalam format JSON. 

### 2. Apa itu protokol ?
Protokol adalah sebuah aturan dalam sebuah jaringan yang harus ditepati antara si pengirim dan penerima. HTTP termasuk salah satu bentuk jenis protokol. Protokol selain HTTP ada banyak lagi, seperti FTP, SMTP, POP3, IMAP, dan masih banyak lagi. Protokol HTTP sendiri merupakan protokol yang digunakan untuk mengirimkan data antara client dan server. Protokol HTTP sendiri memiliki 4 metode request, yaitu GET, POST, PUT, dan DELETE. Metode GET digunakan untuk mengambil data dari server. Metode POST digunakan untuk mengirimkan data ke server. Metode PUT digunakan untuk mengubah data yang ada di server. Metode DELETE digunakan untuk menghapus data yang ada di server. HTTP juga memiliki 3 status code, yaitu 1xx, 2xx, dan 3xx. Status code 1xx digunakan untuk informasi. Status code 2xx digunakan untuk menandakan bahwa request telah berhasil diproses. Status code 3xx digunakan untuk menandakan bahwa client harus melakukan redirect ke URL lain. Di bab ini kita akan membahas tentang HTTP. HTTP merupakan protokol yang digunakan untuk mengirimkan data antara client dan server di packet tracer.
### Persiapan
1. Buka Packet Tracer
2. Klik File
3. Klik New
4. Klik Blank Topology
5. Klik OK
6. Dalam membuat server HTTP, kita membutuhkan 1 buah workstation dan 1 buah server yang terhubung langsung dengan kabel --tipe-cross.
7. Lakukan konfigurasi IP Address pada PC0 sebagaimana sebelumnya.
8. Lakuan konfigurasi IP address pada server0. Langkah-langkah mengkonfigurasi IP address untuk tipe Server-PT pada Cisco Packet Tracer sama dengan workstationnya (PC-PT).
9. Double klik pada server0, lalu jendela properti akan muncul.
10. Pastikan radio button service HTTP pada pilihan on. Anda juga dapat mengubah port default dari 80 ke port lainnya. Jika port yang digunakan sudah terpakai, maka akan muncul pesan error. Selain itu anda juga dapat mengubah default document yang akan ditampilkan oleh server. Default document yang akan ditampilkan adalah index.html. Jika file tersebut tidak ada, maka akan muncul pesan error. 
### Browsing Webßßßß
Double klik pada PC0, lalu buka browser. Ketikkan alamat IP address dari server0. Jika alamat IP address yang dimasukkan benar, maka akan muncul halaman default dari server. Jika alamat IP address yang dimasukkan salah, maka akan muncul pesan error. Tampilannya akan seperti gambar berikut.
![browsing](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSUxUhSF9YwG3kMYachKxVvbfT4kx6izs8BDQ&usqp=CAU)
### Kesimpuan dan Saran
1. HTTP merupakan protokol yang digunakan untuk mengirimkan data antara client dan server di packet tracer.
2. Workstation merupakan perangkat yang digunakan untuk mengakses server. Workstation dapat berupa PC, laptop, dan smartphone.
3. Server merupakan perangkat yang digunakan untuk menyimpan data. Server dapat berupa server web, server database, dan server file.
4. HTTP merupakan protokol yang digunakan untuk mengirimkan data antara client dan server di packet tracer.
5. Workstation dan server harus terhubung langsung dengan kabel --tipe-cross.
6. Jika konfigurasi yang dilakukan benar, maka akan muncul halaman default dari server.
7. Web browser di workstation digunakan untuk mengakses server.

### Pertanyaan
1. Apa itu HTTP ?
2. Apa itu workstation ?
3. Apa itu server ?
5. Apa yang harus dilakukan agar workstation dapat mengakses server ?
6. Apa yang harus dilakukan agar server dapat menerima request dari workstation ?
7. Apa yang harus dilakukan agar server dapat mengirimkan response ke workstation ?
8. Apa yang harus dilakukan agar workstation dapat menerima response dari server ?
9. Apa yang harus dilakukan agar workstation dapat menampilkan halaman default dari server ?
10. Bagaimana cara mengubah port default dari 80 ke port lainnya ?
11. Bagaimana cara mengubah default document yang akan ditampilkan oleh server ?
12. Apakah workstation dan server harus terhubung langsung dengan kabel --tipe-cross ?
