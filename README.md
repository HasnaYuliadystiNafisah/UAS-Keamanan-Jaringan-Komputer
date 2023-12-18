# Implementasi Firewall Pada Kali Linux di VirtualBox
Salah satu langkah mendasar dalam melindungi sistem dan jaringan adalah menggunakan firewall. Firewall bertindak sebagai penghalang antara jaringan internal dan eksternal, mengontrol dan memonitor lalu lintas data berdasarkan aturan keamanan. Implementasi firewall menjadi suatu strategi yang sangat penting dalam konteks pengembangan keamanan sistem. Kali Linux sebagai distribusi Linux yang dikenal karena kehandalannya dalam pengujian keamanan jaringan memiliki alat bawaan yang dapat digunakan untuk membangun dan mengelola firewall yang perlu dilakukan implementasi dan konfigurasi yang tepat untuk memanfaatkanya. 

Melalui implementasi ini, diharapkan tercipta panduan praktis bagi pengguna Kali Linux di VirtualBox untuk mengimplementasikan firewall dengan benar. Hal ini tidak hanya meningkatkan keamanan sistem operasi, tetapi juga memberikan pemahaman yang lebih baik mengenai konsep keamanan jaringan dan konfigurasi firewall. 
# Tujuan dan Manfaat Implementasi
1. Mengimplementasikan konfigurasi firewall pada Kali Linux di VirtualBox.
2. Mengidentifikasi langkah-langkah konfigurasi firewall pada Kali Linux di VirtualBox.
3. Mengetahui dampak penggunaan firewall pada Kali Linux di VirtualBox.
# Pembahasan Implementasi
Penerapan firewall pada Kali Linux di VirtualBox tidak hanya bertujuan untuk melindungi terhadap serangan seperti pemindaian port, malware, dan virus, tetapi juga untuk menguji dan memastikan efektivitas kebijakan keamanan secara menyeluruh. 

Setelah berhasil menginstal Kali Linux di VirtualBox, langkah-langkah implementasi firewall menggunakan iptables dilakukan untuk meningkatkan keamanan sistem. Langkah-langkahnya melibatkan login ke Kali Linux, masuk ke terminal, melakukan root dengan perintah "sudo su", menginstal iptables dengan "sudo apt-get install iptables", dan melakukan pengecekan blokir dengan "iptables -L".

Selanjutnya, dilakukan implementasi firewall dengan memblokir situs detik.com menggunakan perintah "iptables -A INPUT -s 203.190.242.211 -j DROP". Setelah implementasi, dilakukan pengecekan dengan "iptables -L" yang menunjukkan IP detik.com telah terblokir. Uji coba dengan ping menghasilkan tidak ada reply, dan mencoba membuka detik.com di Firefox menghasilkan time out, menandakan bahwa implementasi firewall berhasil memblokir IP detik.com.
# Dampak Implementasi
Penggunaan firewall pada Kali Linux di VirtualBox memberikan dampak signifikan terhadap keamanan dan kinerja sistem. Dampak positif termasuk peningkatan keamanan jaringan dengan memblokir penyusupan, malware, dan akses tidak sah, serta mengurangi ketergantungan pada konfigurasi spesifik. Firewall juga memungkinkan pengaturan akses konten yang lebih baik.

Namun, terdapat dampak negatif, seperti keterbatasan akses yang dapat mengganggu pengguna jika pengaturannya terlalu ketat. Konfigurasi firewall yang tidak optimal juga dapat mempengaruhi kinerja jaringan dengan peningkatan latensi atau penghambatan komunikasi. Selain itu, firewall yang kurang dikonfigurasi mungkin tidak dapat mendeteksi serangan tersembunyi, sehingga memerlukan pemantauan dan konfigurasi berkala untuk menjaga keefektifan sistem.
# Disusun Oleh Kelompok 2
- Hasna Yuliadysti Nafisah (21050974009)
- Laili Nur Fadhilah (21050974037)
- Mukhamad Khoirul Nizam (21050974045)
- Talitha Aneira Naura Shada (21050974061)
- Tsabita Clara Anjani (21050974063)
