# Konsep
## 1. Struktur Folder
## 2. Repository
### 2.1. Apa itu Repository?  
   **Repository** adalah tempat menyimpan berbagai macam program atau aplikasi yang telah di buat sedemikian rupa sehigga bisa di akses melalui internet. Selain di internet, **Repository** juga tersedia di media seperti DVD sebagai alternatif **Repository** saat tak ada koneksi internet. Ketika kita melakukan download Repository melalui internet default servernya adalah server luar, seperti archive.ubuntu.com, security.ubuntu.com, dll. Untuk Fungsinya, disini Repository berperan sebagai penyedia aplikasi atau kumpulan paket software dari distro-distro linux, yang dapat di akses melalui internet.  
  
### 2.2. Dimana file Repositori itu berarda?  
File Repository ini langsung otomatis berada di laptop atau PC kita saat kita sudah menginstall linux dengan nama file biasanya "sources.list", terletak di folder apt di dalam folder etc. Jika ingin melihat Repository milik kita hanya perlu mengetikan :  
  

> sudo gedit /etc/apt/sources.list
  
Kita bisa melakukan edit seperti menambah, menghapus, mengganti Repostitory milik sobat sesuai yang sobat inginkan.  
  
### 2.3. Apakah Repository itu Penting?  
Adanya Repository di linux itu sangatlah _**Penting**_, karena itu adalah tempatnya paket-paket software untuk linux itu sendiri, kita hanya perlu langsung menginstall tanpa harus cari lagi paket softwarenya karena sudah tersedia di Repository tersebut. walau pun kita bisa juga mencar paket softwarenya secara manual dan menginstallnya juga, tetapi cara tersebut cukup ribet dan akan banyak memakan waktu. 
  
### 2.4. Apakah semua Paket software ada di Repostory? 
Tidak semua paket software langsung ada di repository, itu sebabnya kita harus tau nama file repository dan letaknya dimana, karena jika kita akan menginstall suatu software dan aplikasi, kemudian di Repository ternyata paketnya belum ada, kita bisa mencari repositorynya dan menambahkannya di di Repository kita dengan mengedit file sources.list tadi, yang berada di directory sudo gedit /etc/apt/sources.list.
