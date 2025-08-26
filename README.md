# Uber Ride Performance 2024

## About the Project
Proyek ini berfokus pada analisis operasional layanan Uber Ride untuk memberikan pandangan menyeluruh tentang kinerja bisnis. Tujuannya adalah membangun dashboard interaktif menggunakan Power BI yang memungkinkan pemangku kepentingan (stakeholders) memantau metrik kunci (KPI), mengidentifikasi tren, dan memahami perilaku pelanggan serta pengemudi secara mendalam.

## Dataset Overview
Dataset ini berisi 148.770 baris data dengan 21 kolom yang mencakup informasi berikut:
1. Date : Tanggal Pemesanan
2. Time : Waktu pemesanan
3. Booking ID : Pengidentifikasi unik untuk setiap pemesanan perjalanan
4. Booking Status : Status pemesanan (Completed, Cancelled by Customer, Cancelled by Driver etc)
5. Customer ID : Pengidentifikasi unik untuk pelanggan
6. Vehicle Type : Jenis kendaraan (Go Mini, Go Sedan, Auto, eBike/Bike, UberXL, Premier Sedan)
7. Pickup Location : Lokasi awal perjalanan
8. Drop Location : Lokasi tujuan perjalanan
9. Avg VTAT : Rata-rata waktu kendaaraan saat tiba
10. Avg CTAT : Rata-rata waktu pelanggan saat tiba
11. Cancelled Rides by Customer : Bendera perjalanan yang dibatalkan oleh pelanggan
12. Reason for Cancelling by Customer : Alasan pembatalan pelanggan
13. Cancelled Rides by Driver : Bendera perjalanan yang dibatalkan oleh driver
14. Driver Cancellation Reason : Alasan pembatalan pengemudi
15. Incomplete Rides : Bendera perjalanan tidak selesai
16. Incomplete Rides Reason : Alasan perjalanan tidak selesai
17. Booking Value :  Total tarif perjalanan
18. Ride Distance : Jarak yang ditempuh selama perjalanan (dalam KM)
19. Driver Ratings : Peringkat yang diberikan kepada driver (skala 1-5)
20. Customer Ratings : Peringkat yang diberikan kepada customer (skala 1-5)
21. Payment Method : Metode yang digunakan untuk pembayaran (UPI, Cash, Credit Card, Uber Wallet, Debit Card)

## Tools
Aplikasi yang digunakan selama mengerjakan projek ini:
1. Microsoft Power BI

## Exploratory Data Analysis
Untuk melakukan analisis pada projek ini, saya menggunakan Microsoft Power BI untuk mengubah raw data menjadi sesuatu yang lebih menarik dan insightful. 

1. Key Statistics:
   <img width="1308" height="124" alt="image" src="https://github.com/user-attachments/assets/fd537c9e-9b23-4213-8d17-45981a5301d0" />
   Dari total 150 ribu pemesanan, sekitar 93 ribu perjalanan berhasil diselesaikan, dengan tingkat keberhasilan 62%. Namun, data tersebut juga menunjukkan bahwa 25% pemesanan berakhir dengan pembatalan. Menariknya, pembatalan yang dilakukan oleh pelanggan (27 ribu perjalanan) jauh lebih tinggi daripada yang dilakukan oleh pengemudi (10,5 ribu perjalanan). Hal ini menyoroti potensi masalah dalam perilaku pelanggan atau kegunaan aplikasi yang perlu mendapat perhatian lebih lanjut.
   
2. Revenue Distribution
   
   <img width="364" height="229" alt="image" src="https://github.com/user-attachments/assets/39deeab6-0bbf-4b8e-a9a3-298e31d49dba" />

   Mayoritas pendapatan berasal dari pembayaran digital melalui UPI (40%), menunjukkan bahwa pelanggan semakin nyaman dengan transaksi non-tunai. Pembayaran tunai masih memegang porsi yang signifikan (25%), menunjukkan bahwa banyak pelanggan masih bergantung pada metode pembayaran tradisional. Saluran digital lain seperti Kartu Kredit, Uber Wallet, dan Kartu Debit berkontribusi cukup signifikan. Keseimbangan ini menunjukkan adanya pergeseran berkelanjutan menuju adopsi digital, tetapi uang tunai tetap relevan.

3. Cancellation Patterns

   <img width="791" height="242" alt="image" src="https://github.com/user-attachments/assets/3b83eb15-ded9-42f5-9285-2391c06ee516" />
   <img width="827" height="303" alt="image" src="https://github.com/user-attachments/assets/77d362a0-a811-40ca-8390-9554a37b7b44" />


   Pembatalan oleh pelanggan sering kali disebabkan oleh masalah seperti salah alamat (22,5%), pengemudi tidak pindah (22,2%), atau perubahan rencana (21,9%). Alasan-alasan ini menunjukkan adanya masalah teknis (akurasi GPS/alamat) dan keputusan perilaku. Di sisi lain, pembatalan oleh pengemudi terdistribusi secara merata: masalah kapasitas (25%), masalah yang berkaitan dengan pelanggan (25,3%), dan masalah pribadi atau terkait mobil (24,9%). Hal ini menunjukkan bahwa pembatalan oleh pengemudi tidak didominasi oleh satu masalah saja, melainkan beberapa tantangan kecil.
   
4. Vehicle Type Usage
   
   <img width="461" height="268" alt="image" src="https://github.com/user-attachments/assets/d3b5af6f-41b7-444f-a184-806856bccb27" />

   Pilihan kendaraan terpopuler adalah Mobil (37 ribu pemesanan), diikuti oleh Go Mini (30 ribu) dan Go Sedan (27 ribu). Tren ini menunjukkan bahwa pelanggan umumnya lebih menyukai pilihan yang ekonomis dan nyaman untuk perjalanan harian. Pilihan yang lebih besar dan premium seperti Premier Sedan dan Uber XL mencatat pemesanan yang jauh lebih sedikit, menunjukkan bahwa layanan ini melayani basis pelanggan yang niche.

   
5. Revenue Trend Across Months

   <img width="716" height="330" alt="image" src="https://github.com/user-attachments/assets/5769c529-ebaa-4f1b-a8ee-c71509b35f89" />

   Tren pendapatan bulanan relatif stabil, berfluktuasi antara 4,0 juta dan 4,6 juta per bulan. Puncak pendapatan tertinggi terjadi pada bulan April, menunjukkan adanya pengaruh musiman atau promosi. Setelah itu, pendapatan stabil tanpa fluktuasi yang signifikan, mencerminkan permintaan yang stabil sepanjang tahun.

   

## Dashboard
Berikut adalah dashboard dari hasil analisis:
<img width="1277" height="717" alt="Screenshot 2025-08-26 150859" src="https://github.com/user-attachments/assets/d810715e-cf2e-4617-b312-77f4b9561974" />


## Conclusion
1. Booking Success Rate tercatat cukup baik yaitu 66%, namun angka cancellation rate sebesar 25% masih tergolong tinggi. Hal ini perlu ditekan agar revenue dapat meningkat secara signifikan.
2. Metode pembayaran didominasi oleh UPI dan Cash, mencerminkan adanya kombinasi perilaku cash-driven society sekaligus tren peralihan ke digital payment.
3. Alasan pembatalan antara customer dan driver terdistribusi hampir merata, menunjukkan adanya isu di berbagai aspek, seperti kendala teknis (aplikasi & GPS), komunikasi, serta ketersediaan kendaraan yang perlu diperbaiki.
4. Auto dan Go Mini menjadi jenis kendaraan dengan penggunaan tertinggi, menandakan adanya demand besar pada kategori ekonomis.

## Recommendation
Berdasarkan temuan tersebut, terdapat beberapa rekomendasi strategis yang dapat dilakukan. Pertama, optimasi alamat dan GPS perlu ditingkatkan untuk mengurangi masalah wrong address maupun kasus driver not moving. Kedua, peningkatan komunikasi antara customer dan driver dapat dilakukan melalui notifikasi yang lebih jelas serta penyediaan fitur in-app chat yang lebih efektif. Ketiga, diperlukan inisiatif retensi driver, seperti pemberian insentif khusus bagi pengemudi dengan tingkat pembatalan rendah dan rating yang tinggi, sehingga kualitas layanan tetap terjaga. Selain itu, promosi pada layanan Premier dan XL dapat ditingkatkan untuk mendorong permintaan di segmen high-value rides. Terakhir, perlu adanya fokus pada perluasan penggunaan pembayaran digital melalui promo dan diskon yang menarik, khususnya pada metode UPI dan dompet digital, guna meningkatkan kenyamanan transaksi sekaligus mengurangi ketergantungan pada pembayaran tunai.

## Kontributor
- Nama :  Rizka Hasna Nabila
- Email : rizkahasna94@gmail.com
- Github : @rizkaa-hn
- Linkedin : https://www.linkedin.com/in/rizkahasnanabila/ 
