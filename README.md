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
# Dampak Implementasi
Penggunaan firewall pada Kali Linux di VirtualBox memberikan dampak signifikan terhadap keamanan dan kinerja sistem. Dampak positif termasuk peningkatan keamanan jaringan dengan memblokir penyusupan, malware, dan akses tidak sah, serta mengurangi ketergantungan pada konfigurasi spesifik. Firewall juga memungkinkan pengaturan akses konten yang lebih baik.

Namun, terdapat dampak negatif, seperti keterbatasan akses yang dapat mengganggu pengguna jika pengaturannya terlalu ketat. Konfigurasi firewall yang tidak optimal juga dapat mempengaruhi kinerja jaringan dengan peningkatan latensi atau penghambatan komunikasi. Selain itu, firewall yang kurang dikonfigurasi mungkin tidak dapat mendeteksi serangan tersembunyi, sehingga memerlukan pemantauan dan konfigurasi berkala untuk menjaga keefektifan sistem.
# Disusun Oleh Kelompok 2
- Hasna Yuliadysti Nafisah (21050974009)
- Laili Nur Fadhilah (21050974037)
- Mukhamad Khoirul Nizam (21050974045)
- Talitha Aneira Naura Shada (21050974061)
- Tsabita Clara Anjani (21050974063)
