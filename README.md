# Run Emulator
Uji coba aplikasi wajib dilakukan seorang developer. Proses running atau debugging bisa dilakukan dengan dua cara, yaitu running dengan emulator atau peranti (device). Baik emulator maupun peranti memiliki kelebihan dan kekurangan masing-masing. Kita sebagai developer tinggal pilih mana yang sesuai  keperluan. <br>
### Berikut merupakan cara Run Emulator pada Android Studio <br>
#### Persiapan : <br>
Sebelum menggunakan emulator, pastikan beberapa hal berikut ini:  <br>
##### Virtualization <br>
Untuk menjalankan emulator di dalam Android Studio, pastikan aspek virtualization. Sistem Anda harus memenuhi persyaratannya, yakni ketentuan prosesor dan sistem operasi dari laptop / PC yang Anda gunakan. <br>
###### Processor <br>
•	Prosesor Intel: Jika laptop/pc Anda menggunakan prosesor Intel, maka pastikan ia mendukung Intel VT-x, Intel EM64T (Intel 64), dan Execute Disable (XD) Bit functionality. <br>
•	Prosesor AMD:  Jika laptop/pc Anda menggunakan AMD, maka pastikan bahwa ia support dengan AMD Virtualization (AMD-V) dan Supplemental Streaming SIMD Extensions 3 (SSSE3). <br>

###### Sistem Operasi <br>
•	Intel : Jika menggunakan processor Intel maka Anda dapat menjalankannya di sistem operasi Windows, Linux, maupun Mac. <br>
•	AMD : Untuk prosesor AMD maka hanya bisa menjalankannya di sistem operasi Linux. <br>

#### Menginstal Hardware Accelerated Execution Manager (HAXM) <br>
Setelah memenuhi persyaratan di atas, langkah selanjutnya adalah menginstal HAXM. HAXM adalah hardware-assisted virtualization engine yang menggunakan teknologi VT dari Intel untuk mempercepat aplikasi Android yang diemulasi di mesin host. HAXM diperlukan untuk menjalankan emulator di Android Studio. <br>
HAXM diperlukan jika sistem operasi yang Anda gunakan adalah Windows atau Mac. Untuk menginstalnya, ikuti petunjuk berikut ini. <br>
1.	Buka SDK Manager. <br>
2.	Pilih SDK Update Sites, kemudian hidupkan Intel HAXM. <br>
3.	Tekan OK. <br>
4.	Cari berkas installer-nya di directory folder sdk komputer Anda,
~sdk\extras\intel\Hardware_Accelerated_Execution_Manager\intelhaxm-android.exe. <br>
5.	Jalankan installer dan ikuti petunjuknya sampai selesai. <br>

#### Menggunakan Emulator <br>
OK, Anda sudah memastikan bahwa virtualization bisa berjalan di komputer. Kini ikuti langkah-langkah berikut untuk menjalankan aplikasi dengan menggunakan emulator built-in dari Android Studio. <br>

##### Membuat Virtual Device 







