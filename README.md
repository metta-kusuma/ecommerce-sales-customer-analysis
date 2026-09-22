Judul Proyek

Multi-Vendor E-Commerce Performance Analysis & Customer Retention Strategy

1. Ringkasan Eksekutif (Executive Summary)

Analisis ini mengolah dataset e-commerce staging sebanyak 100.000 transaksi dari 700 merchant dan 8.999 pelanggan dalam rentang waktu Maret hingga September 2026.

Tujuan utama analisis ini adalah untuk memahami pendorong utama pendapatan (Gross Merchandise Value / GMV), menilai efisiensi status pemenuhan pesanan (fulfillment), serta mengukur tingkat retensi pelanggan menggunakan metode RFM Analysis.

2. Temuan Utama (Key Insights)
- Total Pendapatan (GMV): Mencapai $8.032.882,17 dengan nilai transaksi berhasil (Delivered) sebesar $5.444.213,01 (68,07%).

- Kategori Paling Cuan: Electronics ($2,01 Juta) dan Apparel & Fashion ($2,00 Juta) menyumbang lebih dari 50% dari total pendapatan.

- Status Pesanan (Fulfillment):
	- Delivered: 68,07% (68.065 pesanan)
	- Shipped: 14,04% (14.043 pesanan)
	- Processing: 9,92% (9.921 pesanan)
	- Cancelled (Batal): 4,97% (4.973 pesanan)
	- Refunded (Dapat Uang Kembali): 3,00% (2.998 pesanan)

- Opsi Biaya Pengiriman (Shipping Fee):
	- Free Shipping ($0.00): 40,2% transaksi
	- Standard Shipping ($4.99): 40,0% transaksi
	- Express Shipping ($9.99): 19,8% transaksi

- Perilaku & Loyalitas Pelanggan (RFM):
	- Memiliki 8.999 pelanggan unik dengan repeat customer rate sebesar 100%.
	- Rata-rata pelanggan melakukan ~11 kali transaksi dalam rentang waktu 6 bulan, dengan total nilai belanja rata-rata ~$890 USD per pelanggan.


3. Teknologi yang Digunakan (Tech Stack)

Bahasa Pemrograman: Python

Library Analisis Data: Pandas, NumPy

Library Visualisasi: Matplotlib, Seaborn

Environment: Google Colab

4. Rekomendasi Bisnis Berbasis Data
1. Tekan Angka Pembatalan (Cancellation Rate): Ada sekitar 7,97% transaksi (Cancelled + Refunded) yang bikin potensi pendapatan hilang. Bisnis perlu bikin aturan waktu proses (SLA) yang ketat buat merchant agar stok barang selalu siap dan tidak memicu pembatalan.

2. Optimasi Strategi Ongkir: Karena 40,2% pembeli sangat menyukai Free Shipping, bisnis bisa bikin strategi Minimum Belanja Gratis Ongkir (misal: "Gratis Ongkir untuk Belanja di Atas $60"). Tujuannya untuk mendorong pelanggan belanja barang tambahan (Up-selling).

3. Fokus Promosi pada Kategori Unggulan: Berikan promo khusus atau garansi tambahan untuk kategori Electronics dan Apparel & Fashion karena dua kategori ini adalah penyumbang cuan terbesar dengan nilai rata-rata belanja (AOV) yang tinggi (~$80 USD).
