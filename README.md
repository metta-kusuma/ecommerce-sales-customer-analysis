#  Multi-Vendor E-Commerce Sales & Customer Retention Analysis

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-1.5+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen?style=for-the-badge)

---

##  Executive Summary

Analisis ini mengolah dataset e-commerce staging sebanyak **100.000 transaksi** dari **700 merchant** dan **8.999 pelanggan** unik (periode Maret - September 2026). 

Tujuan utama proyek ini adalah mengevaluasi kinerja penjualan (**Gross Merchandise Value / GMV**), efisiensi pemenuhan pesanan (**fulfillment rate**), serta mengelompokkan perilaku pelanggan menggunakan metode **RFM Analysis (Recency, Frequency, Monetary)**.

---

##  Key Highlights & Metrics

| Metrik Bisnis | Nilai | Keterangan |
| :--- | :--- | :--- |
| **Total GMV** | **$8,032,882.17** | Total nilai transaksi kotor |
| **Delivered GMV** | **$5,444,213.01** | Total transaksi berhasil diselesaikan (68.07%) |
| **Total Orders** | **100,000** | Jumlah baris transaksi |
| **Unique Customers** | **8,999** | Total pelanggan unik |
| **Unique Merchants** | **700** | Total toko/penjual aktif |
| **Average Order Value (AOV)** | **~$80.33** | Rata-rata pengeluaran per transaksi |

---

##  Key Insights & Findings

### 1. Revenue Drivers by Category
* **Electronics** ($2,009,544.34) dan **Apparel & Fashion** ($2,004,865.71) merupakan pendorong utama pendapatan, menyumbang **>50% dari total GMV**.
* Rata-rata nilai belanja (*AOV*) tergolong stabil di seluruh kategori produk (~$80 USD).

### 2. Fulfillment & Order Status
* **Delivered:** 68.07% (68,065 pesanan)
* **Shipped:** 14.04% (14,043 pesanan)
* **Processing:** 9.92% (9,921 pesanan)
* **Cancelled & Refunded:** **7.97%** (7,971 pesanan gabungan) — mengindikasikan potensi kebocoran pendapatan akibat pembatalan merchant atau isu stok.

### 3. Shipping Fee Breakdown
* **Free Shipping ($0.00):** Dipilih oleh **40.2%** pelanggan.
* **Standard Shipping ($4.99):** Dipilih oleh **40.0%** pelanggan.
* **Express Shipping ($9.99):** Dipilih oleh **19.8%** pelanggan.

### 4. Customer Retention & RFM Analysis
* **Repeat Customer Rate:** **100%** (seluruh 8.999 pelanggan melakukan transaksi lebih dari 1 kali).
* **Frekuensi Transaksi:** Rata-rata pelanggan melakukan **~11 kali belanja** dalam rentang waktu 6 bulan.
* **Nilai Belanja Pelanggan:** Rata-rata satu pelanggan membelanjakan total **~$890 USD**.

---

##  Tech Stack & Libraries

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Environment:** Google Colab / Jupyter Notebook

---

##  Strategic Business Recommendations

1. **SLA & Penalti Merchant (Menekan Cancel Rate):**
   * Sekitar **7.97% transaksi batal/refund**. Terapkan aturan batas waktu pemrosesan (*Service Level Agreement*) serta penalti stok bagi 700 merchant untuk menekan kebocoran GMV.
2. **Program Ambang Belanja Gratis Ongkir:**
   * Mengingat **40.2% pembeli memilih Free Shipping**, buat strategi *Free Shipping threshold* (misal: "Gratis Ongkir untuk Belanja Minimum $60") untuk mendorong peningkatan nilai keranjang belanja (*Basket Size*).
3. **Fokus Promosi Kategori Unggulan:**
   * Berikan penawaran garansi ekstra atau *cross-selling* barang pendukung pada kategori **Electronics** dan **Apparel & Fashion** sebagai penyumbang cuan terbesar platform.

---

##  Repository Structure

```text
.
├── ecommerce_orders_staging_100k.csv    # Dataset mentah (100k rows)
├── ecommerce_data_analysis.ipynb        # Notebook analisis data (Python)
└── README.md                            # Laporan dokumentasi proyek
