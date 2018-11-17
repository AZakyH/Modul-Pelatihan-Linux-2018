# Instalasi
Sub-materi
1. [Persiapan](#1-persiapan)
2. [Teknik Instalasi](#2-teknik-instalasi)
3. [Membuat Virtual Machine](#3-membuat-virtual-machine)
4. [Instalasi Ubuntu](#4-instalasi-ubuntu-1604)

### 1. Persiapan
- File ISO Ubuntu 16.04 LTS ([Download](http://releases.ubuntu.com/16.04/ubuntu-16.04.5-desktop-amd64.iso))
- Installer VirtualBox ([Download](https://download.virtualbox.org/virtualbox/5.2.22/VirtualBox-5.2.22-126460-Win.exe))

### 2. Teknik Instalasi
Jika hendak menggunakan lebih dari satu sistem operasi atau sering disebut OS(operating system) pada suatu komputer biasanya ada dua pilihan teknik instalasi, yaitu **dual-boot** atau **virtualisasi**.
**Dual-boot** adalah teknik menginstall dua atau lebih OS pada satu komputer, dimana masing-masing OS berjalan secara mandiri. Pengguna hanya dapat menggunakan salah satu OS dalam satu watu, dengan cara memilih OS yang akan dipakai ketika menyalakan komputer.

![Tampilan GRUB Dual Boot Linux(Ubuntu) dan Windows](img/tampilan_grub_dual_boot.png "Tampilan GRUB Dual Boot Linux(Ubuntu) dan Windows")

Sedangkan **Virtualisasi** adalah teknik menginstal dan menjalankan suatu OS di atas OS lain sebagai host, yaitu dengan menggunakan program berjenis mesin virtual (virtual machine), salah satu contohnya adalah VirtualBox. Dengan mesin virtual ini, pengguna dapat menjalankan suatu OS, sebagai contoh Linux, pada saat OS lain berjalan, sebagai contoh Windows, sehingga pengguna dapat menjalankan beberapa OS sekaligus dalam satu waktu.

Berikut ini perbandingan termasuk kelebihan dan kekurangan dari kedua teknik instalasi tersebut:

|Dual-Boot|Virtual Machine|
|---|---|
|Secara umum lebih cepat, karena masing - masing OS berjalan secara mandiri|Secara umum lebih lambat, karena harus berbagi sumber daya prosesor dan memori dengan OS host|
|Kedua OS dapat bertukar data dengan mudah, asalkan saling mendukung format sistem file pada harddisk|Bertukar file antar OS tidak dapat dilakukan secara langsung, perlu beberapa konfigurasi|
|Hanya dapat menjalankan salah satu OS saja pada satu waktu|Dapat menjalankan beberapa OS sekaligus dalam satu waktu(asal spesifikasi komputer mencukupi)|
|Prosedur instalasi dan konfigurasi untuk dual-booting cukup rumit dan beresiko (kehilangan data), terutama pada saat partisi harddisk|Prosedur instalasi OS menjadi mudah tanpa harus bingung dengan hal-hal teknis seperti partisi harddisk|
|Ideal untuk penggunaan sehari-hari, yang membutuhkan performa penuh komputer|Ideal untuk sekedar mengetes suatu OS, atau sekedar menjalankan suatu program yang tidak dapat berjalan pada OS host|
|Jika terjadi kerusakan pada salah satu OS, ada kemungkinan berpengaruh dengan OS satunya|Kerusakan pada OS yang di virtualisasikan tidak akan berpengaruh pada OS host|

### 3. Membuat Virtual Machine
1. Install Oracle VM VirtualBox. Jika sudah ada, lanjut ke langkah 2.
2. Buka aplikasi Oracle VM VirtualBox di Windows kamu.  
![Tampilan awal Oracle VM VirtualBox](img/vb_home.png "Tampilan awal Oracle VM VirtualBox")

3. Klik **New** untuk membuat Virtual Machine baru. Isi **name** dengan nama 'Ubunru 16.04', **type** pilih Linux, dan pilih **version** sesuai sepesifikasi PC atau Laptop kamu. Kemudian klik **Next** untuk proses selanjutnya.  
![Membuat Virtual Machine baru Oracle VM VirtualBox](img/vb_buat_vm_baru.png "Membuat Virtual Machine baru Oracle VM VirtualBox")

4. Selanjutnya kamu disuruh untuk menentukan besaran memori, namun VirtualBox otomatis merekomendasikan besarnya memori. Jika sudah sesuai klik **Next**.  
![Set memori VM baru Oracle VM VirtualBox](img/vb_set_memori.png "Set memori VM baru Oracle VM VirtualBox")

5. Selanjutnya kamu disuruh untuk menentukan ukuran harddisk, namun VirtualBox otomatis merekomendasikan ukuran harddisk. Jika sudah sesuai klik **Next**.  
![Set ukuran harddisk VM baru Oracle VM VirtualBox](img/vb_set_disk.png "Set ukuran harddisk VM baru Oracle VM VirtualBox")

6. Klik **Next** saja pada proses ini untuk menuju proses selanjutnya.  
![Set tipe harddisk VM baru Oracle VM VirtualBox](img/vb_set_disk_type.png "Set tipe harddisk VM baru Oracle VM VirtualBox")

7. Klik **Next** saja pada proses ini untuk menuju proses selanjutnya.  
![Set tipe harddisk VM baru Oracle VM VirtualBox(2)](img/vb_set_disk_type2.png "Set tipe harddisk VM baru Oracle VM VirtualBox(2)")

8. Menentukan ukuran harddisk(direkomendasikan minimal 10GB). Klik **Create**.  
![Set ukuran harddisk VM baru Oracle VM VirtualBox(3)](img/vb_set_disk_size.png "Set ukuran harddisk VM baru Oracle VM VirtualBox(3)")

9. Yee, virtual machine yang kamu buat sudah jadi! Namun, kamu masih harus menginstall Ubuntu 16.04 pada virtual machine yang telah kamu buat.

### 4. Instalasi Ubuntu 16.04
Setelah berhasil membuat virtual machine, selanjutnya kita menginstall Ubuntu 16.04 pada virtual machine yang telah dibuat.
1. Pilih virtual machine yang ingin di install, lalu klik **Setting** -> **Storage** -> **Controller: IDE** -> **Empty** -> **Choose Virtual Optical Disk File** untuk memilih file ISO Ubuntu yang akan di install. Kemudian klik **Start**(tanda panah hijau)  
![Set file ISO Ubuntu VM baru Oracle VM VirtualBox](img/vb_set_iso.png "Set file ISO Ubuntu VM baru Oracle VM VirtualBox")  
![Set file ISO Ubuntu VM baru Oracle VM VirtualBox(2)](img/vb_get_iso_file.png "Set file ISO Ubuntu VM baru Oracle VM VirtualBox(2)")  
![Set file ISO Ubuntu VM baru Oracle VM VirtualBox(3)](img/vb_vm_jadi.png "Set file ISO Ubuntu VM baru Oracle VM VirtualBox(3)")

2. Yuhuu!! File ISO Ubuntu sudah berjalan. Selanjutnya tinggal ikuti langkah instalasinya. Klik **Install Ubuntu**.  
![Instalasi Ubuntu(1)](img/vb_install_ubuntu1.png "Instalasi Ubuntu(1)")

3. Tidak perlu mencentang apapun untuk menghemat waktu instalasi, kemudian klik **Continue**.  
![Instalasi Ubuntu(2)](img/vb_install_ubuntu2.png "Instalasi Ubuntu(2)")

4. Pilih **Erase disk and install Ubuntu**, lalu klik **Install Now**.  
![Instalasi Ubuntu(3)](img/vb_install_ubuntu3.png "Instalasi Ubuntu(3)")

5. Memilih zona waktu. Ketik **Jakarta**, lalu klik **Continue**.  
![Instalasi Ubuntu(4)](img/vb_install_ubuntu4.png "Instalasi Ubuntu(4)")

6. Memilih bahasa yang digunakan untuk penyesuaian keyboard. Ikuti saja defaultnya, langsung klik **Continue**.  
![Instalasi Ubuntu(5)](img/vb_install_ubuntu5.png "Instalasi Ubuntu(5)")

7. Mengatur nama, nama komputer, username, dan password. Biasanya ketika mengetikkan nama kita pada form **Your name**, form **Your computer's name** dan form **Pick a username** otomatis tergenerate sesuai nama yang kita ketikkan.  
![Instalasi Ubuntu(6)](img/vb_install_ubuntu6.png "Instalasi Ubuntu(6)")

8. Tunggu hingga proses instalasi selesai.  
![Instalasi Ubuntu(7)](img/vb_install_ubuntu7.png "Instalasi Ubuntu(7)")

9. Instalasi sudah selesai! Klik **Restart Now** untuk me-*restart* Ubuntu untuk menyudahi tahapan instalasi.  
![Instalasi Ubuntu(8)](img/vb_install_ubuntu8.png "Instalasi Ubuntu(8)")


##### Referensi
- https://abrari.wordpress.com/2009/12/12/dual-booting-vs-virtualisasi/
- https://id.wikihow.com/Memasang-Ubuntu-di-VirtualBox
- https://www.ubuntu.com/
- https://www.virtualbox.org/
