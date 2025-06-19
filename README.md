# Analisis Pola Perilaku Pelanggan Berdasarkan Pendapatan dan Skor Pengeluaran Menggunakan Metode K-Means Clustering

## Ringkasan Program

Proyek ini bertujuan untuk melakukan segmentasi pelanggan (customer segmentation) berdasarkan data perilaku mereka di sebuah mal. Dengan menggunakan algoritma **K-Means Clustering**, program ini mengelompokkan pelanggan ke dalam beberapa segmen berbeda berdasarkan dua fitur utama: **Pendapatan Tahunan (`Annual Income`)** dan **Skor Pengeluaran (`Spending Score`)**.

Analisis dimulai dari pemuatan data, eksplorasi data (EDA) untuk memahami distribusi demografis pelanggan seperti gender dan usia, hingga visualisasi pendapatan tahunan. Metode **Elbow** digunakan untuk menentukan jumlah cluster (segmen) yang optimal, yang dalam kasus ini ditemukan sebanyak **4 cluster**.

Hasil akhir dari program ini adalah 4 segmen pelanggan yang terdefinisi dengan jelas:
1.  **Pelanggan dengan Pendapatan Menengah dan Belanja Tinggi.**
2.  **Pelanggan dengan Pendapatan Tinggi dan Belanja Intensif (Royal).**
3.  **Pelanggan dengan Pendapatan Tinggi dan Belanja Sedikit (Hemat).**
4.  **Pelanggan dengan Pendapatan dan Belanja Rendah.**

Segmentasi ini divisualisasikan dalam bentuk *scatter plot* yang menunjukkan setiap cluster beserta titik pusatnya (centroid). Wawasan dari analisis ini sangat berguna bagi tim pemasaran untuk merancang strategi yang lebih personal dan efektif, sehingga dapat meningkatkan kepuasan pelanggan dan pendapatan mal.

## Bahasa dan Library yang Digunakan

### Bahasa Pemrograman
- **Python 3.13.3**

### Library
- **Pandas**: Digunakan untuk manipulasi dan analisis data, terutama untuk membaca dan mengelola dataset dari file `Mall_Customers.csv`.
- **Matplotlib**: Digunakan untuk membuat visualisasi data statis seperti diagram lingkaran (pie chart), diagram batang (bar chart), dan diagram sebar (scatter plot).
- **Scikit-learn**: Digunakan untuk implementasi algoritma machine learning, khususnya `KMeans` untuk melakukan clustering data.
- **Yellowbrick**: Digunakan sebagai alat bantu visualisasi machine learning. Dalam proyek ini, `KElbowVisualizer` dipakai untuk mengimplementasikan Metode Elbow secara visual guna menemukan jumlah cluster yang optimal.

## Langkah Menjalankan Program

Berikut adalah langkah-langkah untuk menjalankan program ini di lingkungan lokal Anda.

### 1. Prasyarat
Pastikan Anda telah menginstal Python 3 di sistem Anda. Anda juga perlu menginstal library-library yang dibutuhkan. Buka terminal atau command prompt dan jalankan perintah berikut:

```bash
pip install pandas matplotlib scikit-learn yellowbrick jupyter
```

### 2. Dataset
Program ini menggunakan dataset _Mall_Customers.csv_. Pastikan file ini berada di direktori yang sama dengan file notebook (learning.ipynb) atau sesuaikan path file di dalam kode jika diletakkan di lokasi berbeda.

### 3. Menjalankan Notebook
Unduh atau kloning repositori ini ke komputer Anda.
Buka terminal atau command prompt, arahkan ke direktori tempat Anda menyimpan file.
Jalankan Jupyter Notebook atau Jupyter Lab dengan perintah:
```
Bash
jupyter notebook
atau
Bash
jupyter lab
```
Setelah antarmuka Jupyter terbuka di browser Anda, klik dan buka file _learning.ipynb_.
Untuk menjalankan analisis, Anda dapat menjalankan setiap sel kode secara berurutan dari atas ke bawah. Anda bisa melakukannya dengan memilih sel dan menekan Shift + Enter atau melalui menu Run > Run All Cells.
Output dari setiap langkah, termasuk tabel data, visualisasi, dan hasil clustering akan ditampilkan langsung di bawah setiap sel kode.
