![People talking with managers in bank flat vector illustration](https://github.com/user-attachments/assets/dca3d228-7c41-4100-8cf4-fbc93b04531d)


# Bank Customer Segmentation using Clustering Model 

##  Introduction
Nama  : Vicky Belario

proyek ini dilakukan untuk menerapkan model clustering untuk Customer Segmentation 

## Goal
Membuat model clustering untuk melakukan Customer Segmentation pada dataset kartu kredit sebuah bank. Dataset  merupakan data informasi penggunaan kartu kredit selama 6 bulan terakhir.

---

## Dataset

| **Column Name**                | **Data Type** | **Description**                                                                                                                    |
| ------------------------------ | ------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| CUSTID                         | Object        | Identifikasi pemegang kartu kredit                                                                                                 |
| BALANCE                        | Float         | Jumlah saldo yang tersisa di akun untuk melakukan pembelian                                                                        |
| BALANCEFREQUENCY               | Float         | Seberapa sering saldo diperbarui, nilai antara 0 dan 1 (1 = sering diperbarui, 0 = tidak sering diperbarui)                        |
| PURCHASES                      | Float         | Jumlah pembelian yang dilakukan dari akun                                                                                          |
| ONEOFFPURCHASES                | Float         | Jumlah maksimum pembelian yang dilakukan dalam satu kali transaksi                                                                 |
| INSTALLMENTSPURCHASES          | Float         | Jumlah pembelian yang dilakukan dengan cicilan                                                                                     |
| CASH ADVANCE                   | Float         | Uang muka yang diberikan oleh pengguna                                                                                             |
| PURCHASESFREQUENCY             | Float         | Seberapa sering pembelian dilakukan, nilai antara 0 dan 1 (1 = sering membeli, 0 = tidak sering membeli)                           |
| ONEOFFPURCHASESFREQUENCY       | Float         | Seberapa sering pembelian dilakukan dalam satu kali transaksi, nilai antara 0 dan 1 (1 = sering membeli, 0 = tidak sering membeli) |
| PURCHASESINSTALLMENTSFREQUENCY | Float         | Seberapa sering pembelian dengan cicilan dilakukan, nilai antara 0 dan 1 (1 = sering dilakukan, 0 = tidak sering dilakukan)        |
| CASHADVANCEFREQUENCY           | Float         | Seberapa sering uang muka dibayar, nilai antara 0 dan 1 (1 = sering dibayar, 0 = tidak sering dibayar)                             |
| CASHADVANCETRX                 | Integer       | Jumlah transaksi yang dilakukan dengan "uang muka"                                                                                 |
| PURCHASESTRX                   | Integer       | Jumlah transaksi pembelian yang dilakukan                                                                                          |
| CREDIT LIMIT                   | Float         | Batas kredit kartu untuk pengguna                                                                                                  |
| PAYMENTS                       | Float         | Jumlah pembayaran yang dilakukan oleh pengguna                                                                                     |
| MINIMUM_PAYMENTS               | Float         | Jumlah pembayaran minimum yang dilakukan oleh pengguna                                                                             |
| PRCFULLPAYMENT                 | Float         | Persentase pembayaran penuh yang dilakukan oleh pengguna                                                                           |
| TENURE                         | Integer       | Masa layanan kartu kredit untuk pengguna                                                                                           |

---
## Daftar konten di bawah ini:

   1. Import Libraries
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.
   
   2. Query SQL
      > Tulis query yang telah dibuat untuk mengambil data dari Google Cloud Platform di bagian ini.

   3. EDA I (Exploratory Data Analysis)
      > Bagian ini berisi explorasi data pada dataset diatas dengan menggunakan query, grouping, visualisasi sederhana, dan lain sebagainya.
   
   4. Feature Engineering
      > Bagian ini berisi proses penyiapan data untuk proses pelatihan model, seperti transformasi data (normalisasi, encoding, dll.), dan proses-proses lain yang dibutuhkan.
   
   5. Model Definition
      > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

   6. Model Training
      > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.
   
   9. EDA II (Exploratory Data Analysis)
      > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis terkait dengan hasil pada model dan tuliskan hasil analisisnya**.

   10. Model Saving
       > Pada bagian ini, dilakukan proses penyimpanan model dan file-file lain yang terkait dengan hasil proses pembuatan model.

   11. Model Inference
       > Model yang sudah dilatih akan dicoba pada data yang bukan termasuk ke dalam train-set. Data ini harus dalam format yang asli, bukan data yang sudah di-scaled.
    

---
## Kesimpulan
- proyek ini membahas tentang mengimplementasikan algoritma Unsupervised Learning. 
- Metode yang digunakan untuk menyelesaikan permasalahannya adalah Principal Component Analysis (PCA) dan K-Means. 
- PCA akan digunakan untuk mereduksi atau mengurangi jumlah dimensinya, sedangkan K-Means digunakan untuk tahap clusteringnya.
- Untuk mencari nilai optimal dalam menentukan jumlah clustering, maka digunakan teknik ELBOW METHOD, siluette score,plot.
- Diperoleh jumlah Cluster paling optimal, yaitu 4.
- Setelah melalui beberapa analisis dan teknik pemrosesan, data yang digunakan dapat dikelompokkan berdasarkan 4 Clustering
