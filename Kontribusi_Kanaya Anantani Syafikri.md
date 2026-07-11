  
**Nama         :** *Kanaya Anantani Syafikri*  
**NIM	         :** *25110500018*  
**Kelompok  :** *Kelompok 6*

**Role    :** *Role 1 \- API & Postman Tester*

1. **Kontribusi Pribadi**   
   Dalam praktikum UAS kelompok kali ini, saya bertanggung jawab sebagai pemilik peran **API & Postman Tester.** Saya berkontribusi dalam membuat dan menyusun seluruh skenario pengujian endpoint API di Postman yang dibagi ke dalam folder terstruktur (Folder 00 sampai 04). Saya menyiapkan pengujian skenario sukses, gagal, endpoint observability, serta membuat request di folder 04 untuk memicu dan menguji integrasi webhook n8n kelompok. Berkas bukti (evidence) berupa kumpulan screenshot request-response Postman juga sudah saya kumpulkan untuk laporan.  
     
2. **Proses Pengerjaan**  
   Proses pengerjaan diawali dengan mereset data pada folder 00 agar database kembali bersih dari history percobaan sebelum pengujian dimulai. Kemudian, saya menyusun skenario sukses pada folder 01 menggunakan data dari webhook dosen yang saya modifikasi dan memastikan menghasilkan respons 201 Created, lalu dilanjutkan dengan request GET by ID. Setelah itu, saya membuat skenario gagal pada folder 02 dengan sengaja mengosongkan beberapa kolom untuk memicu respons 400 Bad Request. Selanjutnya saya  mengecek folder 03 untuk menguji endpoint /api/observabilitylogs dan /api/observabilitymetrics guna memastikan semua log riwayat dan metrik performa server terekam dengan benar. Proses diakhiri dengan menjalankan folder 04 untuk mengirimkan data tes ke webhook n8n guna memastikan alur integrasi sistem berjalan dengan benar.  
     
3. **Kendala Teknis**  
   Adanya kendala salah status code pada skenario sukses data masuk. Di awal tes Postman, saya mengira respons sukses cukup berupa 200 OK. Namun ternyata terjadi ketidakcocokan karena standar untuk pembuatan data baru harusnya mengembalikan status 201 Created.  
     
4. **Solusi**  
   Memperbaiki test script di Postman. Saya mengubah kode validasinya agar mendeteksi status code 201 Created untuk setiap skenario sukses.  
     
   

