# Otomatisasi_Transfer_Kepemilikan_Google_Drive_dengan_Google_Apps_Script

Script ini adalah solusi otomatisasi berbasis Google Apps Script (GAS) untuk melakukan transfer kepemilikan folder dan file di Google Drive serta melakukan konfirmasi penerimaan transfer kepemilikan yang telah diberikan.

Script ini dirancang dengan sistem Looping Berantai (Time-driven Trigger) untuk mengatasi batas maksimal waktu eksekusi (timeout) 6 menit dari Google, sehingga aman digunakan untuk Google Drive.

🌟 Fitur Utama
1. code.gs untuk menjalankan perintah transfer kepemilikan : adalah script yang diletakan pada akun gmail drive yang folder dan filenya akan dilakukan transfer kepemilikan.
2. code.gs untuk menjalankan perintah terima transfer kepemilikan : adalah script yang diletakan pada akun gmail drive yang folder dan filenya akan menerima transfer kepemilikan dari pemilik sebelumnya.

🛠️ Persyaratan
1. Akun Google (Personal atau Workspace).
2. Akses ke Google Apps Script.

🚀 Cara Instalasi & Penggunaan

1. Pada akun gmail drive yang folder dan filenya akan dilakukan transfer kepemilikan
1.1. Memasang Script
- Buka Google Apps Script dan buat New Project (Proyek Baru).
- Beri nama proyek Anda, misalnya "Transfer Kepemilikan".
- Salin seluruh kode yang ada di file "code.gs untuk menjalankan perintah transfer kepemilikan" dan tempelkan ke dalam editor Apps Script. Hapus kode bawaan function myFunction() {}.
- Klik tombol Save (Simpan) berikon disket di bagian atas.
1. 2. Menjalankan Proses Pertama Kali
- Pada menu dropdown di sebelah kanan tombol Run (Jalankan), pilih fungsi mulaiProsesSistematis. ⚠️ PENTING: Pastikan Anda memilih mulaiProsesSistematis untuk eksekusi pertama, BUKAN prosesSebagian.
- Klik tombol Run.
- Google akan meminta otorisasi akses. Klik Review Permissions -> Pilih Akun Google Anda -> Klik Advanced (Lanjutan) -> Klik Go to Untitled project (unsafe) -> Pilih Allow (Izinkan).
- Biarkan script berjalan selama beberapa detik hingga indikator log menunjukkan proses sedang berjalan. Setelah itu, Anda bisa menutup tab browser. Script akan bekerja secara otonom di background server Google.

2. Pada akun gmail drive yang folder dan filenya akan menerima transfer kepemilikan dari pemilik sebelumnya
2.1. Memasang Script
- Buka Google Apps Script dan buat New Project (Proyek Baru).
- Beri nama proyek Anda, misalnya "Terima Transfer Kepemilikan".
- Salin seluruh kode yang ada di file "code.gs untuk menjalankan perintah terima transfer kepemilikan" dan tempelkan ke dalam editor Apps Script. Hapus kode bawaan function myFunction() {}.
- Klik tombol Save (Simpan) berikon disket di bagian atas.
2. 2. Menjalankan Proses Pertama Kali
- Pada menu dropdown di sebelah kanan tombol Run (Jalankan), pilih fungsi mulaiProsesSistematis. ⚠️ PENTING: Pastikan Anda memilih mulaiProsesSistematis untuk eksekusi pertama, BUKAN prosesSebagian.
- Klik tombol Run.
- Google akan meminta otorisasi akses. Klik Review Permissions -> Pilih Akun Google Anda -> Klik Advanced (Lanjutan) -> Klik Go to Untitled project (unsafe) -> Pilih Allow (Izinkan).
- Biarkan script berjalan selama beberapa detik hingga indikator log menunjukkan proses sedang berjalan. Setelah itu, Anda bisa menutup tab browser. Script akan bekerja secara otonom di background server Google.

3. Jeda waktu untuk menjalankan script : berikan jeda waktu 6 menit antara "Transfer Kepemilikan" dengan "Terima Transfer Kepemilikan" untuk menjalankan pertama kalinya.

📝 Lisensi
Bebas digunakan, dimodifikasi, dan didistribusikan untuk keperluan personal maupun organisasi.
