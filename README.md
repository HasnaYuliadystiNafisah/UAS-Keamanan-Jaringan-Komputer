# Implementasi Firewall Pada Kali Linux di VirtualBox
Salah satu langkah mendasar dalam melindungi sistem dan jaringan adalah menggunakan firewall. Firewall bertindak sebagai penghalang antara jaringan internal dan eksternal, mengontrol dan memonitor lalu lintas data berdasarkan aturan keamanan. Implementasi firewall menjadi suatu strategi yang sangat penting dalam konteks pengembangan keamanan sistem. Kali Linux sebagai distribusi Linux yang dikenal karena kehandalannya dalam pengujian keamanan jaringan memiliki alat bawaan yang dapat digunakan untuk membangun dan mengelola firewall yang perlu dilakukan implementasi dan konfigurasi yang tepat untuk memanfaatkanya. 

Melalui implementasi ini, diharapkan tercipta panduan praktis bagi pengguna Kali Linux di VirtualBox untuk mengimplementasikan firewall dengan benar. Hal ini tidak hanya meningkatkan keamanan sistem operasi, tetapi juga memberikan pemahaman yang lebih baik mengenai konsep keamanan jaringan dan konfigurasi firewall. 
# Tujuan dan Manfaat Implementasi
1. Mengimplementasikan konfigurasi firewall pada Kali Linux di VirtualBox.
2. Mengidentifikasi langkah-langkah konfigurasi firewall pada Kali Linux di VirtualBox.
3. Mengetahui dampak penggunaan firewall pada Kali Linux di VirtualBox.
# Pembahasan dan Langkah-Langkah Implementasi
Penerapan firewall pada Kali Linux di VirtualBox tidak hanya bertujuan untuk melindungi terhadap serangan seperti pemindaian port, malware, dan virus, tetapi juga untuk menguji dan memastikan efektivitas kebijakan keamanan secara menyeluruh. 
1. Membuat Virtual Mesin Kali Linux di VirtualBox
   - Klik “Baru” untuk membuat mesin virtual baru
     
     ![Picture3](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/b09f7439-589c-406c-b8d2-11c6fd99790b)
     
   - Beri nama virtual mesin sesuai keinginan. Untuk kali linux sendiri menggunakan tipe “Linux” dengan versi “Linux 2.6/3.x/4.x(64-bit). Lalu klik “Lanjut”

     ![Picture1](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/903af5b4-73b0-476f-894a-61ebdd217717)
   - Untuk ukuran memori sesuaikan dengan laptop, di sini penulis menggunakan ukuran memori 4096MB atau setara dengan 4GB. Lalu klik “Lanjut”

     ![Picture2](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/7ed82dae-deef-4d58-8183-fc226f95d269)
   - Pilih “Buat hard disk virtual sekarang”, lalu klik “Buat”

     ![Picture4](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/d39669cd-f7c4-4ba6-b586-e748a9719fb2)
   - Selanjutnya untuk tipe hard disk pilih “VDI (Virtual Disk Image)” dan klik “Lanjut”
     
     ![Picture5](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/32f649c3-553e-401c-b98b-5b2a3fe6a620)
   - Penyimpanan pada hard disk fisik gunakan yang “Dialokasikan secara dinamik”. Lalu klik “Lanjut”
     ![Picture6](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/f376747b-a2a9-4410-a793-4993559873aa)

   - Lokasi dan ukuran berkas juga disesuaikan dengan keinginan, di sini penulis menggunakan 32GB. Selanjutnya klik “Buat”

     ![Picture7](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/4ae34cd4-4c5c-4c5b-8484-74d3a699c31b)

   - Virtual mesin kali linux berhasil dibuat
     
     ![Picture8](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/420826e3-ab84-43c5-bcc6-06229731f750)

   - Sebelum lanjut mengkonfigurasi kali linux, setting bagian penyimpanan dan jaringan terlebih dahulu. Untuk di bagian penyimpanan, tambahkan disk optik kali linux yang telah di unduh dari https://www.kali.org/get-kali/#kali-platforms.

     ![Picture9](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/7ff8b561-cea1-4102-a988-5f690c97da96)

     Sedangkan di bagian jaringan, ganti jaringan yang secara default “NAT” menjadi “Adaptor Ter-bridge”. Lalu klik “Ok” untuk menyimpan perubahan.
     
     ![Picture10](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/75dac6f1-3ae8-4d3d-ae8a-d445de9b0234)

   - `Pembuatan virtual mesin di virtual box berhasil dibuat
2. Installasi dan Konfigurasi Kali Linux 
   - Klik “Mulai” untuk mulai menjalankan kali linux
     
     ![Picture11](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/014f400e-766a-4ad7-b88a-c1a74817f65e)

   - Halaman pertama, akan menampilkan beberapa pilihan yang akan di install dan konfigurasi. Di sini penulis memilih “Graphical Install”

      ![Picture12](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/9b6b9117-abac-4c1e-bb54-41a4f5ceb188)

   - Selanjutnya, pengguna akan disuruh memilih bahasa, lokasi, dan jenis keyboard yang digunakan. Di sini penulis menggunakan Bahasa Indonesia, lokasi Indonesia, dan jenis keyboard Inggris Amerika
     
     ![Picture13](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/0da5daaf-4ac6-4b70-a5ee-3d7d47695c93)

     ![Picture14](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/58b145e7-d1a0-4c0c-9c16-76d841d5a8ce)

     ![Picture15](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/11cfa927-0e3e-482f-a9e6-77a961dfa321)

   - Selanjutnya, tunggu pemrosesan yang dilakukan oleh kali linux hingga selesai

     ![Picture16](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/e55828ef-795a-4fd3-8cc3-22a995190c55)

   - Pengguna akan dimintai untuk menuliskan nama host, nama domain, nama lengkap dari pengguna baru, dan juga nama untuk akun. Di sini penulis menyamakan semua nama dengan nama “laili”
     
     ![Picture17](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/cad40a93-575b-498a-b584-3de6de64ec57)

     ![Picture18](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/bd2b7731-9bee-403f-a392-185f69036110)

     ![Picture19](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/b3d0fa8f-7df5-4006-bd98-4bc3c87c2cd2)

     ![Picture20](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/ae1a683d-cfb0-459b-923b-e64328c0d4d2)

   - Setelah menuliskan semua nama yang diminta, selanjutnya pengguna juga dimintai untuk membuat kata sandi untuk akun kali linux nya.
     
     ![Picture21](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/9a827e4a-1bdf-43db-b10d-d7e5e7dac189)
     
   - Di pengaturan waktu, pengguna harus memilih pengaturan waktu yang sesuai dengan tempat tinggal pengguna. Di sini penulis memilih pengaturan waktu “WIB”
     
     ![Picture22](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/9a61eb48-35ed-4fce-826c-ac1732ec8277)

   - Untuk partisi hard disk, pilih “Terpadu – gunakan seluruh harddisk”
     
     ![Picture23](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/baa88417-cc92-4caa-afab-46651ec3d767)

   - Pilih harddisk yang akan di partisi dan lanjut pilih pola partisi, di sini penulis memilih “Semua berkas di satu partisi (disarankan untuk pemula)
     
     ![Picture24](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/a728cf3f-118b-472c-9e05-6c054bb4cc57)

     ![Picture25](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/52e12d64-b9c1-495f-9146-c8c35f7fd2af)

   - Setelah selesai partisi hard disk, selanjutnya pilih “Selesai mepartisi dan tulis perubahan-perubahannya ke hard disk” dak klik “Lanjutkan”
     
     ![Picture26](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/79af9094-2c18-42a0-8a3c-2031807b386a)

   - Pada bagian tulis perubahan yang terjadi pada hard disk, penulis memilih “ya”
     
     ![Picture27](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/8d00e9b9-465b-4e8c-9282-6bd7784f1936)

   - Semua pemrosesan hingga selesai
     
     ![Picture28](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/fe60fd4e-5da3-4193-8eec-8a45b63a08fa)

   - Pilih perangkat lunak yang ingin di install, ini menyesuaikan kebutuhan pengguna. Penulis memilih 3 perangkat lunak seperti pada gambar
     
     ![Picture29](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/cc21d6b0-4c22-44f4-8396-938c44ac9eea)

   - Tunggu pemrosesan perangkat lunak hingga selesai
     
     ![Picture30](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/8a30c687-f6b1-418e-95bb-510f11bb9a21)

   - Setelah pemrosesan selesai, pengguna akan diberikan pilihan untuk memasang boot loader GRUB atau tidak. Di sini penulis memilih untuk tidak memasang boot loader GRUB. Lalu klik “Lanjutkan

     ![Picture31](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/b8a9ed90-821b-4225-b8b2-0efdf5406847)
     
   - Untuk piranti pemasangan boot loader, penulis memilih yang sudah ada, yaitu “/dev/sda/ (ata-VBOX_HARDDISK_VB30cc22c5-bcd2de04)”
     
     ![Picture32](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/96c5a39e-d56b-4002-9018-79bfac5b7409)

   - Tunggu penyelesaian installasi hingga selesai
     
     ![Picture33](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/4fe83607-5f9f-4154-8e77-84548d44ce0b)

   - Setelah instalasi selesai, pilih “Lanjutkan” untuk melakukan boot ulang
     
     ![Picture34](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/63ddf084-5a73-45da-9dcd-36b7325f7c41)

3. Implementasi Firewall Dengan Kali Linux di VirtualBox
   - Setelah installasi selesai, pengguna akan di arahkan ke menu login dari kali linux. Dimana sebelum masuk, pengguna dimintai untuk memasukkan username dan password yang telah di buat

     ![Picture35](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/8f2c6c93-e138-4e0e-a95a-0ae67a3362fe)

   - Jika username dan password berhasil maka pengguna akan langsung diarahkan ke menu utama.
     
     ![Picture36](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/109a957c-19c7-4647-8a83-a2ae7d067522)

   - Setelah dari menu utama, pengguna masuk ke terminal dan melakukan root dengan menuliskan perintah “sudo su”

     ![Picture37](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/cd8a9f57-8a5b-4457-8f77-e8b7bcd4f77b)

   - Setelah berada di dalam root, install iptables dengan mengetikkan “sudo apt-get install iptables”
     
     ![Picture38](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/654b76b6-8821-4c08-abd6-874ad2b72045)

   - Selanjutnya, penulis akan melakukan pengecekan apakah sudah ada yang terblokir atau belum dengan menuliskan perintah “iptables -L”. Di awal belum ada yang terblokir. Untuk melakukan implementasi firewall, di sini penulis ingin mencoba untuk memblokir website dari detik.com. Dimana IP dari detik.com sendiri yaitu 203.190.242.211 maka untuk memblokirnya, dituliskan perintah “iptables -A INPUT -s 203.190.242.211 -j DROP” setelah itu enter. Penulis melakukan pengecekan lagi dengan menuliskan perintah “iptables -L” dan terlihat bahwa IP dari detik.com sudah masuk ke dalam list. Penulis mencoba melakukan ping ke IP detik.com tetapi tidak ada reply yang berarti tidak terhubung
     
     ![Picture39](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/3e55fa07-6058-4d03-8e15-eea27ea85792)
     
   - Penulis mencoba untuk membuka website detik.com di firefox dan menghasilkan time out. Hal ini berarti penulis sudah berhasil memblokir IP detik.com

     ![Picture40](https://github.com/HasnaYuliadystiNafisah/UAS-Keamanan-Jaringan-Komputer/assets/136795333/5d17ac83-6d63-43d4-90c8-acd8b1fc5ff0)

# Dampak Implementasi
Penggunaan firewall pada Kali Linux di VirtualBox memberikan dampak signifikan terhadap keamanan dan kinerja sistem. Dampak positif termasuk peningkatan keamanan jaringan dengan memblokir penyusupan, malware, dan akses tidak sah, serta mengurangi ketergantungan pada konfigurasi spesifik. Firewall juga memungkinkan pengaturan akses konten yang lebih baik.

Namun, terdapat dampak negatif, seperti keterbatasan akses yang dapat mengganggu pengguna jika pengaturannya terlalu ketat. Konfigurasi firewall yang tidak optimal juga dapat mempengaruhi kinerja jaringan dengan peningkatan latensi atau penghambatan komunikasi. Selain itu, firewall yang kurang dikonfigurasi mungkin tidak dapat mendeteksi serangan tersembunyi, sehingga memerlukan pemantauan dan konfigurasi berkala untuk menjaga keefektifan sistem.
# Disusun Oleh Kelompok 2
- Hasna Yuliadysti Nafisah (21050974009)
- Laili Nur Fadhilah (21050974037)
- Mukhamad Khoirul Nizam (21050974045)
- Talitha Aneira Naura Shada (21050974061)
- Tsabita Clara Anjani (21050974063)
