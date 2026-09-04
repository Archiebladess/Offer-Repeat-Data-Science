# Offer-Repeat
# Data Science – Customer & Motorcycle Financing Analysis

## 📌 Project Overview

Project ini menggunakan dataset yang berisi informasi terkait customer, lokasi, metode pembayaran, tenor pembiayaan, karakteristik kendaraan, harga OTR, uang muka, cicilan, dealer, serta beberapa informasi pendukung lainnya.

## 📊 Dataset

Dataset awal terdiri dari:

* **319.978 baris**
* **28 kolom**

Beberapa variabel yang terdapat dalam dataset antara lain:

* `Customer ID`
* `Kelurahan`
* `Kecamatan`
* `Kode POS`
* `Cash/Credit`
* `Kode Dealer`
* `Finance Company`
* `Tenor`
* `Gender`
* `Tgl Lahir`
* `Agama`
* `Pekerjaan`
* `umur`
* `dp aktual`
* `cicilan`
* `warna`
* `dealer`
* `type series`
* `range dp`
* `wilayah`
* `9 segment`
* `kode motor`
* `OTR`
* `tahun rakit`
* `DLR group`
* `tgl cetak`
* `tgl mohon`
* `Kode Kota-Provinsi`

## 🔎 Data Processing

Tahapan preprocessing yang dilakukan dalam notebook meliputi:

1. **Memeriksa informasi dataset**

   * Melihat jumlah data
   * Mengecek tipe data
   * Mengidentifikasi missing value

2. **Menangani missing value**

   * Nilai tertentu seperti `N`, `NA`, `N/A`, `NULL`, `-`, dan `?` diperlakukan sebagai missing value.
   * Missing value pada variabel numerik diisi menggunakan **median**.
   * Missing value pada variabel kategorikal diisi menggunakan **modus**.

3. **Mengubah tipe data**

   * Beberapa variabel diubah menjadi tipe numerik.
   * Variabel tanggal dikonversi menjadi format datetime.

4. **Menghapus kolom yang tidak digunakan**

   Kolom berikut dihapus dari dataset untuk kebutuhan analisis:

   * `Customer ID`
   * `Tgl Lahir`
   * `tgl mohon`
   * `Kode POS`

5. **Menyimpan dataset hasil cleaning**

   Dataset yang telah dibersihkan disimpan sebagai:

   `dataset_clean.csv`

Tahapan tersebut dilakukan sebelum analisis lebih lanjut.

## 📈 Exploratory Data Analysis

Analisis eksploratif mencakup:

### Data Distribution

Statistik deskriptif digunakan untuk melihat distribusi beberapa variabel numerik, seperti:

* `dp aktual`
* `cicilan`
* `OTR`

Selain itu, dilakukan analisis proporsi untuk:

* metode pembayaran **Cash/Credit**
* **Tenor** pembiayaan
* **wilayah**

Hasil notebook menunjukkan bahwa sekitar **56,42%** data menggunakan kategori `Cash/Credit = 2`, sedangkan **43,58%** menggunakan kategori `Cash/Credit = 1`. Untuk tenor, kategori `2` merupakan kategori yang paling dominan, yaitu sekitar **77,77%**.

## 📉 Visualization

Project ini juga menggunakan visualisasi untuk membantu memahami distribusi dan karakteristik data.

Library yang digunakan untuk visualisasi antara lain:

* `Matplotlib`
* `Seaborn`

## 🛠️ Technologies & Libraries

Project dibuat menggunakan Python dengan beberapa library:

```text
Python
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
```

## 📁 Repository Structure

```text
.
├── DATA SCIENCE.ipynb
├── SPARC_dataset.csv
├── dataset_clean.csv
└── README.md
```

> Nama dan keberadaan file di atas menyesuaikan file yang digunakan dalam project.


## 🎯 Purpose

Project ini menunjukkan penerapan:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Statistical Description
* Data Visualization

---

*Project ini merupakan project pembelajaran Data Science.*
