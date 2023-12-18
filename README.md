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
     
     ![Picture3](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/a5b0b9b9-e660-4c99-b710-eea4f12d023b)
     
   - Beri nama virtual mesin sesuai keinginan. Untuk kali linux sendiri menggunakan tipe “Linux” dengan versi “Linux 2.6/3.x/4.x(64-bit). Lalu klik “Lanjut”

     ![Picture1](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/6a03f7e3-5ef7-4fb1-9d0c-d7e81baeeb72)
   - Untuk ukuran memori sesuaikan dengan laptop, di sini penulis menggunakan ukuran memori 4096MB atau setara dengan 4GB. Lalu klik “Lanjut”

     ![Picture2](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/57410bf5-9463-4a2f-9bc2-d8d1b8aaed2e)
   - Pilih “Buat hard disk virtual sekarang”, lalu klik “Buat”

     ![Picture4](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/990b2bc6-72d3-47dd-b602-d9689c2b1291)
   - Selanjutnya untuk tipe hard disk pilih “VDI (Virtual Disk Image)” dan klik “Lanjut”
     
     ![Picture5](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/a4ee5647-e664-4e71-833b-fcdb005e8f47)
   - Penyimpanan pada hard disk fisik gunakan yang “Dialokasikan secara dinamik”. Lalu klik “Lanjut”
     ![Picture6](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/3ab64eb9-3a55-4146-92e0-08ecb56ad236)

   - Lokasi dan ukuran berkas juga disesuaikan dengan keinginan, di sini penulis menggunakan 32GB. Selanjutnya klik “Buat”
     ![Picture7](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/36676d0d-1349-47d8-856a-9bd066aa3cb5)

   - Virtual mesin kali linux berhasil dibuat
     
     ![Picture8](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/e55e906a-add0-449a-983b-73bfd04dade9)

   - Sebelum lanjut mengkonfigurasi kali linux, setting bagian penyimpanan dan jaringan terlebih dahulu. Untuk di bagian penyimpanan, tambahkan disk optik kali linux yang telah di unduh dari https://www.kali.org/get-kali/#kali-platforms.
     ![Picture9](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/9db8979f-e72e-44dd-a2cf-9561186d4e7b)

     Sedangkan di bagian jaringan, ganti jaringan yang secara default “NAT” menjadi “Adaptor Ter-bridge”. Lalu klik “Ok” untuk menyimpan perubahan.
     
     ![Picture10](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/1c648c2d-1eb1-48f0-9967-4a411d2748ec)

   - `Pembuatan virtual mesin di virtual box berhasil dibuat
2. Installasi dan Konfigurasi Kali Linux 
   - Klik “Mulai” untuk mulai menjalankan kali linux
     
     ![Picture11](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/97bad2a9-b5a1-4808-9b87-30103f796555)

   - Halaman pertama, akan menampilkan beberapa pilihan yang akan di install dan konfigurasi. Di sini penulis memilih “Graphical Install”
     ![Picture12](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/3de389d7-02e7-4b48-841f-dd54e8e3a502)

   - Selanjutnya, pengguna akan disuruh memilih bahasa, lokasi, dan jenis keyboard yang digunakan. Di sini penulis menggunakan Bahasa Indonesia, lokasi Indonesia, dan jenis keyboard Inggris Amerika
     
     ![Picture13](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/b5cefe94-2f7a-41e6-861a-96433377e85b)
     
     ![Picture14](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/1186e4db-767c-43f7-848f-6dfa1225e83f)
     
     ![Picture15](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/5c78c919-9f4c-49bc-9168-5a0bd203094b)

   - Selanjutnya, tunggu pemrosesan yang dilakukan oleh kali linux hingga selesai

     ![Picture16](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/e0cad7e9-27fa-4912-8adf-ea374e546680)

   - Pengguna akan dimintai untuk menuliskan nama host, nama domain, nama lengkap dari pengguna baru, dan juga nama untuk akun. Di sini penulis menyamakan semua nama dengan nama “laili”
     
     ![Picture17](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/2ae414df-d7aa-4e5c-be11-7368600aaf9e)

     ![Picture18](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/0fdf1b84-98cd-4be0-9b67-93daefdad10e)

     ![Picture19](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/4a29a5e3-0171-41c3-afac-4f5051168f23)

     ![Picture20](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/bdfa8d7b-5aad-4c39-b917-71fad62095e1)

   - Setelah menuliskan semua nama yang diminta, selanjutnya pengguna juga dimintai untuk membuat kata sandi untuk akun kali linux nya.
     
     ![Picture21](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/e9cea63b-4c11-48a7-8dd4-18f500763dea)
     
   - Di pengaturan waktu, pengguna harus memilih pengaturan waktu yang sesuai dengan tempat tinggal pengguna. Di sini penulis memilih pengaturan waktu “WIB”
     
     ![Picture22](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/16aae342-f838-4503-82c8-e0d59b1ec283)

   - Untuk partisi hard disk, pilih “Terpadu – gunakan seluruh harddisk”
     
     ![Picture23](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/3a63c7f6-4bad-4178-bf3c-4b9dc566b12d)

   - Pilih harddisk yang akan di partisi dan lanjut pilih pola partisi, di sini penulis memilih “Semua berkas di satu partisi (disarankan untuk pemula)
     
     ![Picture24](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/85720fc0-9fca-40e9-b461-e22e0adfb62c)

     ![Picture25](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/b7af7cb8-167a-4c3a-8508-d1095a49809f)

   - Setelah selesai partisi hard disk, selanjutnya pilih “Selesai mepartisi dan tulis perubahan-perubahannya ke hard disk” dak klik “Lanjutkan”
     
     ![Picture26](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/1c655509-0f24-4795-b671-a00b9711253b)

   - Pada bagian tulis perubahan yang terjadi pada hard disk, penulis memilih “ya”
     
     ![Picture27](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/750653d0-26b9-41d3-9373-ef3b55ad1f43)

   - Semua pemrosesan hingga selesai
     
     ![Picture28](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/1f3aaf1f-1c7a-4844-ad2e-700e43f0c5e5)

   - Pilih perangkat lunak yang ingin di install, ini menyesuaikan kebutuhan pengguna. Penulis memilih 3 perangkat lunak seperti pada gambar
     
     ![Picture29](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/30d3208b-c7d2-46ac-98a3-f06ddc7092ed)

   - Tunggu pemrosesan perangkat lunak hingga selesai
     
     ![Picture30](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/598707de-d260-42c2-9ba6-ebba37c7e337)

   - Setelah pemrosesan selesai, pengguna akan diberikan pilihan untuk memasang boot loader GRUB atau tidak. Di sini penulis memilih untuk tidak memasang boot loader GRUB. Lalu klik “Lanjutkan

     ![Picture31](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/ee11e4e8-7b76-4a2f-ac73-402769a025c1)
     
   - Untuk piranti pemasangan boot loader, penulis memilih yang sudah ada, yaitu “/dev/sda/ (ata-VBOX_HARDDISK_VB30cc22c5-bcd2de04)”
     
     ![Picture32](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/9a998c17-40ec-4f9e-abb7-abc847eda7f6)

   - Tunggu penyelesaian installasi hingga selesai
     
     ![Picture33](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/3618f680-4518-42d2-b37f-512cf9d3b83f)

   - Setelah instalasi selesai, pilih “Lanjutkan” untuk melakukan boot ulang
     
     ![Picture34](https://github.com/HasnaYuliadystiNafisah/TF/assets/136795333/4ac9c915-7140-4b46-b4fd-c3b3dd0fcbce)

# Dampak Implementasi
Penggunaan firewall pada Kali Linux di VirtualBox memberikan dampak signifikan terhadap keamanan dan kinerja sistem. Dampak positif termasuk peningkatan keamanan jaringan dengan memblokir penyusupan, malware, dan akses tidak sah, serta mengurangi ketergantungan pada konfigurasi spesifik. Firewall juga memungkinkan pengaturan akses konten yang lebih baik.

Namun, terdapat dampak negatif, seperti keterbatasan akses yang dapat mengganggu pengguna jika pengaturannya terlalu ketat. Konfigurasi firewall yang tidak optimal juga dapat mempengaruhi kinerja jaringan dengan peningkatan latensi atau penghambatan komunikasi. Selain itu, firewall yang kurang dikonfigurasi mungkin tidak dapat mendeteksi serangan tersembunyi, sehingga memerlukan pemantauan dan konfigurasi berkala untuk menjaga keefektifan sistem.
# Disusun Oleh Kelompok 2
- Hasna Yuliadysti Nafisah (21050974009)
- Laili Nur Fadhilah (21050974037)
- Mukhamad Khoirul Nizam (21050974045)
- Talitha Aneira Naura Shada (21050974061)
- Tsabita Clara Anjani (21050974063)
