# Open Source Teleradiology
SiTerMid, a PHP teleradiology integrated with Orthanc's PACS, allows radiologists remote access. Streamline, cut time, and enhance medical team collaboration for fast and accurate diagnosis. Innovative solutions for healthcare quality.
Panduan Instalasi dan Penggunaan Sistem Teleradiologi SiTerMid v2.0
I. Instalasi
A. Xampp
Download Xampp

Unduh Xampp versi 7.4.33 melalui link ini.
Instalasi Xampp

Lakukan instalasi Xampp sesuai dengan direktori yang diinginkan.
B. SiTerMid
Download Source Code SiTerMid

Unduh source code SiTerMid dari portal sitermid.my.id.
Instalasi Database

Extract archive sitermid.rar pada C:/xampp/htdocs.
Buka localhost/phpmyadmin.
Buat database dan lakukan import sitermid.sql dari folder htdocs/sitermid.
C. Orthanc
Download Orthanc

Unduh versi terbaru dari Orthanc melalui link ini.
Install Orthanc pada direktori yang diinginkan.
Konfigurasi Orthanc

Buka file konfigurasi C:\Program Files\Orthanc Server\Configuration\orthanc.json.
Ubah nilai RemoteAccessAllowed menjadi true dan AuthenticationEnabled menjadi false.
II. Testing dan Konfigurasi
Testing Orthanc

Lakukan testing dengan membuka panel PACS melalui URL http://ipaddress:8042.
Testing SiTerMid

Jalankan Xampp dan pastikan server Apache dan MySQL berjalan.
Buka browser dan akses SiTerMid melalui URL http://localhost/SiTerMid atau http://ip-address/SiTerMid.
Konfigurasi Status PACS

Ganti default URL PACS pada SiTerMid dari localhost:8042 menjadi ipaddress:8042.
III. Alur Penggunaan Sistem SiTerMid v2.0
A. Radiografer
Use Case Diagram

Registrasi data pasien pada modalitas.
Melakukan pemeriksaan radiologi.
Mengirimkan citra hasil pemeriksaan ke PACS system.
Activity Diagram

Login.
Dashboard.
Interaksi dengan Data Pasien.
B. Dokter Spesialis Radiologi
Use Case Diagram

Menerima hasil pemeriksaan dari Radiografer.
Melakukan ekspertise terhadap citra radiologi.
Mengirimkan kembali hasil ekspertise pada sistem.
Activity Diagram

Login.
Dashboard.
Ekspertise.
IV. Kinerja Pengguna
A. Radiografer
Registrasi data pasien pada modalitas.
Melakukan pemeriksaan radiologi dan pengiriman hasil ke PACS system.
Menyediakan data yang diperlukan Dokter Spesialis Radiologi.
B. Dokter Spesialis Radiologi
Menerima hasil pemeriksaan dari Radiografer.
Melakukan ekspertise terhadap citra radiologi.
Memberikan hasil ekspertise kembali ke sistem untuk dokumentasi.
Mengambil keputusan berdasarkan analisis citra radiologi.
