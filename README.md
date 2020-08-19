# Instalasi Sertifikat SSL

Di artikel Knowledge Base (KB) kali ini kami akan memberikan cara instalasi dan konfirgurasi untuk penerbitan dan pemasangan sertifikat SSL, namun sebelum lanjut alangkah lebih baiknya kita mengerti apa itu sertifikat SSL, jadi sertifikat SSL merupakan suatu sertifikat SSL merupakan singkatan dari Secure Sockets Layer, suatu teknologi keamanan standar global yang memungkinkan komunikasi terenkripsi antara peramban web dan server web. Sehingga informasi yang terdapat dalam website akan aman dari pencurian orang lain. Ibarat pagar yang mengelilingi rumah, SSL akan melindungi website dari berbagai indikasi pencurian data. Biasanya pada url suatu website yang memiliki sertifikat SSL akan bertransformasi menjadi HTTPS bukan lagi HTTP.

Selanjutnya untuk Sertifikat SSL Ada berbagai jenis dan untuk perbedaannya ialah berdasarkan pada jumlah nama domain atau subdomain yang dimiliki, seperti:

1. Tunggal – mengamankan satu nama domain atau subdomain yang memenuhi syarat sepenuhnya
2. Wildcard – melindungi satu nama domain beserta subdomainnya dalam jumlah yang tidak terbatas
3. Multi-Domain – mengamankan beberapa nama domain

Dari ketiga jenis setifikat SSL tersebut CloudKilat menyediakan dua layanan yaitu SSL Single dan Wildcard ( https://www.cloudkilat.com/layanan/tambahan#sertifikat-ssl ) 

Berikut ini tahapan untuk melakukan penerbitan layanan sertifikat SSL yang disediakan CloudKilat:

1. Siapkan email untuk melakukan approval sertifikat SSL
Perlu diketahui untuk approval Sertifikat SSL tidak bisa menggunakan akun email costum, namun hanya bisa menggunakan salah satu dari akun  email berikut:

- admin@domain.tld
- administrator@domain.tld
- hostmaster@domain.tld
- postmaster@domain.tld
- webmaster@domain.tld 

2. Apabila akun email sudah siap, selanjutnya kita harus melakukan genarate CSR pada layanan Kilat VM atau Hosting Anda. untuk detailnya kami mengacu pada tautan referensi berikut: https://support.plesk.com/hc/en-us/articles/213939845-How-to-generate-certificate-signing-request-CSR-for-domain-in-Plesk ( untuk control panel Plesk ) dan https://www.alphassl.com/support/create-ssl-csr.html (csr VPS)

3. Setelah generate CSR dilakukan, selanjutnya ialah melakukan konfigurasi SSL pada portal client area, dan berikut langkah-langkahnya:
  
  - Masuk ke **https://portal.cloudkilat.com/clientarea**
  - Pilih menu Services
  - Klik View Details pada layanan tambahan sertifikat SSL Anda
  - Klik Configure Now

4. Pada saat konfigurasi di Portal Client Area silakan mengisikan detail sebagai berikut:
   - Pada bagian Web Server Type (Misal: Apache )
   - Masukan CSR yang sebelumnya sudah Anda generate pada form yang telah disediakan
   - Kemudian Click Continue

5. Setelah konfigurasi dari sisi portal dilakukan selanjutnya ialah melakukan Approval pada email yang telah dipersiapkan untuk melakukan approval SSL.

6. Setelah email Approval disetujui, maka akan terbit sertifikat SSL dan cara konfigurasi setifikat SSL tersebut.
