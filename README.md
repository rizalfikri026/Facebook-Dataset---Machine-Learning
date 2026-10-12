# Facebook-Dataset---Machine-Learning
Project ini merupakan praktikum Machine Learning yang menggunakan dataset Facebook untuk melakukan pengolahan data, analisis data, serta membangun model prediksi menggunakan Python. Project ini berfokus pada prediksi jumlah likes_received berdasarkan fitur-fitur yang tersedia dalam dataset.
# Facebook Dataset - Machine Learning


## Tujuan Project

Tujuan dari project ini adalah:

1. Memahami cara membaca dan mengolah dataset menggunakan Python.
2. Melakukan pemeriksaan dan pembersihan data.
3. Melakukan Exploratory Data Analysis (EDA) untuk memahami karakteristik dataset.
4. Mempersiapkan fitur yang akan digunakan dalam proses Machine Learning.
5. Membagi dataset menjadi data training dan data testing.
6. Membangun model Machine Learning untuk prediksi.
7. Mengevaluasi performa model menggunakan metrik evaluasi regresi.
8. Menyimpan model yang telah dilatih agar dapat digunakan kembali.

## Dataset

Dataset yang digunakan dalam project ini adalah `facebook.csv`.

Dataset ini berisi data aktivitas pengguna Facebook yang digunakan untuk latihan pengolahan data dan pemodelan Machine Learning.

Informasi dataset:

- Nama file: `facebook.csv`
- Format: CSV
- Bahasa pemrograman: Python
- Target prediksi: `likes_received`
- Jenis permasalahan: Regresi

Kolom `likes_received` digunakan sebagai target yang akan diprediksi oleh model. Fitur lainnya dipilih dan diproses sesuai kebutuhan pemodelan.

## Teknologi dan Library

Project ini menggunakan beberapa teknologi dan library berikut:

- **Python** — bahasa pemrograman utama.
- **Jupyter Notebook** — lingkungan untuk menjalankan kode dan mendokumentasikan proses analisis.
- **Pandas** — membaca, mengolah, dan menganalisis data.
- **NumPy** — mendukung operasi numerik.
- **Matplotlib** — membuat visualisasi data.
- **Seaborn** — membantu membuat grafik untuk eksplorasi data.
- **Scikit-learn** — melakukan preprocessing, pelatihan model, pembagian dataset, dan evaluasi.
- **Joblib** — menyimpan model Machine Learning.
- **Pickle** — menyimpan objek model ke dalam file.

## Tahapan Pengerjaan

### 1. Data Loading

Dataset `facebook.csv` dibaca menggunakan library Pandas. Tahap ini dilakukan untuk memuat data ke dalam DataFrame sehingga dapat diproses menggunakan Python.

### 2. Memahami Dataset

Data diperiksa melalui informasi kolom, tipe data, beberapa baris pertama, serta statistik deskriptif. Tujuannya adalah mengetahui struktur dan karakteristik dataset sebelum dilakukan pengolahan lebih lanjut.

### 3. Data Preprocessing

Tahap preprocessing dilakukan untuk mempersiapkan data sebelum digunakan dalam proses pemodelan. Tahap ini dapat mencakup pemeriksaan missing values, data duplikat, nilai ekstrem, dan penyesuaian tipe data sesuai kebutuhan.

### 4. Exploratory Data Analysis (EDA)

EDA dilakukan untuk memahami pola dan distribusi data. Proses ini dapat menggunakan statistik deskriptif serta visualisasi seperti histogram, box plot, dan heatmap korelasi.

### 5. Persiapan Fitur

Fitur yang digunakan untuk memprediksi `likes_received` dipisahkan dari kolom target. Kolom yang tidak relevan untuk pemodelan, seperti identifier pengguna, dapat dikeluarkan. Fitur kategorikal juga perlu dikonversi ke format numerik apabila diperlukan oleh algoritma.

### 6. Pembagian Dataset

Dataset dibagi menjadi data training dan data testing menggunakan `train_test_split`. Pembagian ini bertujuan agar model dilatih menggunakan data training dan dievaluasi menggunakan data testing yang terpisah.

### 7. Pembangunan Model

Beberapa algoritma regresi digunakan untuk mempelajari hubungan antara fitur masukan dan target prediksi. Model yang digunakan dalam project ini meliputi Least Angle Regression, Linear Regression, dan Gradient Boosting Regressor.

### 8. Evaluasi Model

Model dievaluasi menggunakan metrik Mean Absolute Error (MAE), Mean Squared Error (MSE), dan R-squared (R²). Hasil evaluasi digunakan untuk memahami tingkat kesalahan prediksi dan kemampuan model dalam menjelaskan variasi target.

### 9. Penyimpanan Model

Model Gradient Boosting Regressor dapat disimpan menggunakan Joblib atau Pickle. Penyimpanan ini bertujuan agar model dapat dimuat kembali tanpa perlu melakukan pelatihan ulang, selama dependensi dan proses preprocessing tetap sesuai.

## Algoritma Machine Learning

### 1. Least Angle Regression (LARS)

LARS merupakan algoritma regresi yang membangun hubungan antara fitur dan target secara bertahap. Algoritma ini dapat digunakan untuk mempelajari pola hubungan pada data numerik.

### 2. Linear Regression

Linear Regression merupakan algoritma regresi yang digunakan untuk memperkirakan hubungan linear antara fitur masukan dan nilai target. Algoritma ini menjadi salah satu metode dasar dalam permasalahan prediksi numerik.

### 3. Gradient Boosting Regressor

Gradient Boosting Regressor merupakan algoritma ensemble yang membangun sejumlah model secara bertahap. Setiap tahap berusaha memperbaiki kesalahan prediksi dari tahap sebelumnya sehingga dapat menghasilkan model prediksi yang lebih baik.

## Evaluasi Model

Evaluasi model dilakukan menggunakan beberapa metrik berikut:

| Metrik | Penjelasan |
|---|---|
| MAE | Mengukur rata-rata selisih absolut antara nilai aktual dan nilai prediksi. |
| MSE | Mengukur rata-rata kuadrat selisih antara nilai aktual dan nilai prediksi. |
| R² | Mengukur seberapa baik model menjelaskan variasi pada target yang diprediksi. |

Nilai evaluasi diperoleh setelah seluruh proses pelatihan dan pengujian dijalankan. Nilai MAE dan MSE yang lebih rendah umumnya menunjukkan kesalahan prediksi yang lebih kecil, sedangkan interpretasi R² bergantung pada hasil dan karakteristik dataset.

## Struktur Repository

Struktur repository project ini adalah sebagai berikut:

```text
facebook-machine-learning/
├── README.md
├── facebook.csv
└── facebook.rizal.ipynb
```

Keterangan:

- `README.md` berisi dokumentasi project.
- `facebook.csv` merupakan dataset yang digunakan.
- `facebook.rizal.ipynb` berisi kode Python dan tahapan pengerjaan Machine Learning.

File model seperti `gbr_model.joblib` dan `gbr_model.pkl` dapat ditambahkan setelah proses penyimpanan model berhasil dijalankan.

## Cara Menjalankan Project

### Persyaratan

Sebelum menjalankan project, pastikan Python dan Jupyter Notebook telah terpasang di komputer.

### 1. Clone Repository

Jalankan perintah berikut melalui terminal:

```bash
git clone https://github.com/USERNAME/facebook-machine-learning.git
```

Ganti `USERNAME` dengan username GitHub kamu dan sesuaikan nama repository jika berbeda.

### 2. Masuk ke Folder Project

```bash
cd facebook-machine-learning
```

### 3. Instal Library

Instal library yang dibutuhkan menggunakan perintah:

```bash
python -m pip install pandas numpy matplotlib seaborn scikit-learn jupyter joblib
```

### 4. Jalankan Jupyter Notebook

```bash
jupyter notebook
```

Setelah Jupyter Notebook terbuka di browser, pilih file `facebook.rizal.ipynb`.

### 5. Jalankan Program

Jalankan setiap cell notebook secara berurutan dari bagian awal hingga akhir. Pastikan file `facebook.csv` berada pada lokasi yang sesuai dan semua library telah terpasang dengan benar.

## Hasil yang Diharapkan

Setelah project dijalankan, hasil yang diharapkan meliputi:

- Informasi dan statistik deskriptif dataset.
- Hasil preprocessing dan eksplorasi data.
- Visualisasi untuk memahami karakteristik dataset.
- Model Machine Learning yang telah dilatih.
- Hasil prediksi dan evaluasi menggunakan MAE, MSE, dan R².
- File model yang tersimpan apabila proses penyimpanan berhasil dijalankan.

## Kesimpulan

Project ini merupakan penerapan dasar Machine Learning menggunakan dataset Facebook. Melalui project ini, proses pengolahan data, eksplorasi data, persiapan fitur, pelatihan model regresi, evaluasi performa, dan penyimpanan model dapat dipelajari secara bertahap. Hasil project dapat digunakan sebagai bahan pembelajaran untuk memahami alur kerja Machine Learning menggunakan Python.

## Catatan

Project ini dibuat untuk keperluan pembelajaran dan praktikum. Hasil prediksi bergantung pada kualitas dataset, pemilihan fitur, proses preprocessing, serta algoritma yang digunakan. Hasil evaluasi perlu diperiksa berdasarkan output aktual dari notebook.

Jika dataset berasal dari pihak lain, pastikan sumber dan ketentuan penggunaannya dicantumkan sesuai kebutuhan.
