# Segmentasi Pelanggan Mall dengan K-Means

Proyek ini adalah studi kasus untuk melakukan segmentasi pelanggan sebuah mall berdasarkan data pendapatan tahunan dan skor pengeluaran mereka. Tujuannya adalah untuk mengidentifikasi kelompok-kelompok pelanggan yang berbeda sehingga tim pemasaran dapat merancang strategi yang lebih relevan dan efektif untuk setiap segmen.

Analisis ini menggunakan algoritma clustering **K-Means** untuk mengelompokkan data ke dalam 5 segmen yang berbeda.

## Dataset

Dataset yang digunakan adalah `Mall_Customers.csv`, yang berisi fitur-fitur berikut:
- `CustomerID`: ID unik untuk setiap pelanggan.
- `Gender`: Jenis kelamin pelanggan.
- `Age`: Usia pelanggan.
- `Annual Income (k$)`: Pendapatan tahunan pelanggan dalam ribuan dolar.
- `Spending Score (1-100)`: Skor yang diberikan oleh mall berdasarkan perilaku pengeluaran pelanggan.

## Kebutuhan Sistem

Untuk menjalankan analisis ini, Anda memerlukan Python 3 dan library yang tercantum dalam file `requirements.txt`. Anda dapat menginstalnya menggunakan pip:

```bash
pip install -r requirements.txt
```

## Cara Menjalankan

1.  Pastikan Anda telah menginstal semua kebutuhan sistem.
2.  Letakkan dataset `Mall_Customers.csv` di direktori root proyek.
3.  Buka dan jalankan notebook Jupyter `customer_segmentation.ipynb`:

    ```bash
    jupyter notebook customer_segmentation.ipynb
    ```

## Hasil Segmentasi

Analisis menghasilkan 5 cluster pelanggan yang berbeda:

1.  **Target Utama (Merah):** Pelanggan dengan pendapatan tinggi dan skor pengeluaran tinggi. Mereka adalah segmen paling berharga.
2.  **Standar (Biru):** Pelanggan dengan pendapatan dan skor pengeluaran rata-rata. Merupakan kelompok pelanggan pada umumnya.
3.  **Hemat (Hijau):** Pelanggan dengan pendapatan tinggi tetapi skor pengeluaran rendah. Mereka cermat dalam berbelanja.
4.  **Boros (Cyan):** Pelanggan dengan pendapatan rendah namun skor pengeluaran tinggi. Mungkin lebih muda atau impulsif.
5.  **Prioritas Rendah (Magenta):** Pelanggan dengan pendapatan dan skor pengeluaran yang rendah. Kurang aktif berbelanja.

Visualisasi dari cluster-cluster ini dapat dilihat di dalam notebook.
