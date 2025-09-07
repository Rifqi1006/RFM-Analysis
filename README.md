# 📊 RFM Analysis  

Proyek ini melakukan analisis nilai pelanggan menggunakan metode **RFM (Recency, Frequency, Monetary)** pada dataset ritel online. RFM Analysis adalah teknik analisis segmentasi pelanggan yang mengelompokkan pelanggan berdasarkan tiga kriteria utama: kedekatan waktu transaksi terakhir (Recency), frekuensi transaksi (Frequency), dan jumlah nilai transaksi (Monetary). Analisis ini berguna untuk strategi pemasaran tertarget, manajemen hubungan pelanggan, dan optimasi loyalitas pelanggan.  

---

## 🎯 Tujuan  
- Menganalisis dan mengelompokkan pelanggan berdasarkan nilai RFM mereka.  
- Mengidentifikasi segmentasi pelanggan untuk strategi pemasaran yang lebih tertarget.  
- Menjadi portfolio yang menunjukkan kemampuan dalam menganalisis data serta menghasilkan actionable insights.  

---

## 📁 Struktur Proyek  
```
RFM-Analysis/
├── Online Retail - RFM.ipynb      # Jupyter notebook dengan analisis lengkap
├── RFM (Dashboard).pbit           # Dashboard Power BI
├── Model View.jpg                 # Skema model data
├── Project Process.jpg            # Preview dashboard
├── Dataframe RFM.csv              # Hasil analisis RFM
├── customer.png                   # Ikon pelanggan
├── customer-segmentation.png      # Ikon segmentasi pelanggan
├── average-revenue-per-user.png   # Ikon nilai rata-rata pelanggan
├── customer_segmentation.png      # ikon segmentasi pelanggan
├── customer.png                   # Ikon analisis pelanggan
├── growth.png                     # Ikon pertumbuhan pelanggan
└── README.md
```

---

## 📋 Dataset  
Dataset bersumber dari Kaggle: *Retail Sales Dataset*  
Data ini merepresentasikan penjualan toko online dari Januari – Desember 2010 

- Ukuran Data: 461.773 baris, 7 kolom  
- Karakteristik Data: berisi transaksi penjualan mencakup informasi pesanan, produk, jumlah, harga, dan pelanggan.  
- Struktur Kolom:
  - Data Transaksi Penjualan (`order_id`, `order_date`)  
  - Informasi Produk (`product_code`, `product_name`, `quantity`, `price`)  
  - Informasi Pelanggan (`customer_id`)  

---

## 📈 Metrik Analisis  
Analisis RFM dilakukan dengan tiga metrik utama:  

- **Recency** → Kedekatan waktu sejak transaksi terakhir pelanggan (dalam hari).  
- **Frequency** → Jumlah transaksi yang dilakukan pelanggan dalam periode tertentu.  
- **Monetary** → Total nilai pembelian yang dilakukan pelanggan.  

---

## 🖥️ Dashboard Preview  

Berikut adalah tampilan dashboard interaktif yang dibuat dengan Power BI.  

![Deskripsi Gambar](https://drive.google.com/uc?export=view&id=1NY_aHwdwUC8jp3NHuiGDHTY4wjaBw2pn)  

Dashboard interaktif ini memungkinkan pengguna untuk menganalisis segmentasi pelanggan berdasarkan nilai RFM, mengidentifikasi pelanggan bernilai tinggi, memantau distribusi recency, frequency, dan monetary value, serta mendapatkan wawasan untuk strategi retensi dan pemasaran yang tertarget.

---

## 👥 Segmentasi RFM  

![My Image](https://drive.google.com/uc?export=view&id=1Lo01lJ_WFW-YD_lCueev-piMSf3p4avc)

Analisis RFM mengelompokkan pelanggan ke dalam 10 segmentasi utama berdasarkan kombinasi nilai Recency (R), Frequency (F), dan Monetary (M):

| Segment | Jumlah Pelanggan | Recency (hari) | Frequency | Monetary | % Unique |
|---------|-----------------|----------------|-----------|----------|-----------|
| 01-Champion | 570 | 11.6 | 12.2 | 4,530 | 14.9% |
| 02-Loyal Customers | 591 | 42.4 | 6.7 | 2,430 | 15.4% |
| 03-Potential Loyalists | 395 | 23.9 | 2.4 | 729 | 10.3% |
| 04-Can't Lose Them | 46 | 126.9 | 9.9 | 3,116 | 1.2% |
| 05-Need Attention | 115 | 60.0 | 3.0 | 1,077 | 3.0% |
| 06-New Customers | 65 | 15.0 | 1.0 | 260 | 1.7% |
| 07-Promising | 162 | 33.0 | 1.0 | 299 | 4.2% |
| 08-At Risk | 329 | 136.2 | 3.8 | 1,269 | 8.6% |
| 09-About to Sleep | 424 | 59.3 | 1.4 | 497 | 11.1% |
| 10-Hibernating | 1,138 | 193.7 | 1.3 | 374 | 29.7% |

---

## 🔧 Teknologi dan Tools  
Analisis dilakukan menggunakan Python dengan dukungan library utama:  

- Bahasa Pemrograman: `Python`  
- Analisis Data: `Pandas`, `NumPy`  
- Visualisasi Data: `Matplotlib`, `Seaborn`, `Plotly`  
- Visualisasi Interaktif: `Power BI`  
- Pengolahan Tanggal/Waktu: `datetime`
- Environment: `Jupyter Notebook`   

---

## 🔍 Insight Utama  
- Dominasi Segment Bernilai Tinggi → Segment Champion (570 pelanggan) dan Loyal Customers (591 pelanggan) menyumbang nilai monetary tertinggi dengan rata-rata £4,530 dan £2,430 per pelanggan.  
- Potensi Pengembangan → Segment Potential Loyalists (395 pelanggan) menunjukkan recency yang baik (24 hari) dengan frequency menengah, berpotensi ditingkatkan menjadi Loyal Customers.  
- Perhatian Khusus Diperlukan → Segment At Risk (329 pelanggan) dan Can't Lose Them (46 pelanggan) memiliki nilai monetary tinggi tetapi recency sangat lama (>126 hari), membutuhkan strategi retensi segera.  
- Base Pelanggan Besar Tidak Aktif → Hibernating merupakan segment terbesar (1,138 pelanggan, 29.7%) dengan recency sangat lama (194 hari) dan aktivitas rendah, tetapi masih berpotensi diaktivasi kembali.  
- Pelanggan Baru Perlu Dikembangkan → New Customers (65 pelanggan) dan Promising (162 pelanggan) menunjukkan recency baik tetapi frequency dan monetary masih rendah, membutuhkan strategi onboarding yang efektif.  

