# 🩺 Prediksi Angka Harapan Hidup Global (Life Expectancy)
#

## Latar Belakang Proyek

Proyek ini merupakan **Analisis Prediktif** untuk memodelkan dan memprediksi **Angka Harapan Hidup** (*Life Expectancy*) di berbagai negara. Kami menganalisis data historis dengan menggabungkan faktor-faktor kunci sosial, ekonomi, dan kesehatan untuk mengidentifikasi variabel yang paling berpengaruh.

*Notebook Jupyter* utama, **`tugas_akhir.ipynb`**, berisi alur kerja *Data Science* yang komprehensif, mulai dari pembersihan data, eksplorasi visual, hingga pembangunan model regresi dan simulasi skenario.

---

## 👥 Tim Pengembang

| Nama Lengkap | NIM |
| :--- | :--- |
| Fatecha Dena A | 24111814039 |
| Sattya Runa P | 24111814038 |
| Kirana Shofa D | 24111814104 |

---

## 📂 Dataset

Dataset yang digunakan adalah **`Life Expectancy Data.csv`**, yang mencakup data dari berbagai negara dan tahun.

### Fitur Kunci yang Dianalisis

Kami fokus pada hubungan antara angka harapan hidup (`Life expectancy`) sebagai variabel target dengan berbagai indikator:

* **`Adult Mortality`**: Tingkat kematian orang dewasa.
* **`GDP`**: *Gross Domestic Product* (Produk Domestik Bruto) per kapita.
* **`BMI`**: *Body Mass Index* (Indeks Massa Tubuh) rata-rata.
* **`Population`**: Jumlah populasi negara.
* **`Schooling`**: Rata-rata lama waktu bersekolah.
* **`Status`**: Status negara (*Developed* atau *Developing*).
* **Indikator Kesehatan Lain**: Termasuk pengeluaran kesehatan, imunisasi, dan kasus HIV/AIDS.

---

## 🛠️ Metodologi Analisis

Alur kerja analisis dibagi menjadi empat fase utama:

### 1. Pembersihan & Pra-pemrosesan Data
* **Penanganan Nilai Hilang**: Menggunakan strategi imputasi yang sesuai (misalnya, nilai median atau rata-rata).
* **Normalisasi Kolom**: Memperbaiki dan menstandardisasi nama-nama kolom.
* **Pengecekan Kualitas**: Mengidentifikasi dan menangani anomali atau *data point* yang tidak logis.

### 2. Eksplorasi Data & Visualisasi
* **Deteksi *Outlier***: Menggunakan **Boxplot** untuk memvisualisasikan distribusi data.
* **Analisis Korelasi**: Memahami hubungan antar variabel untuk pemilihan fitur.

### 3. Pelatihan Model Regresi
Kami melatih dan membandingkan empat algoritma *Machine Learning* untuk tugas regresi ini:

* **Regresi Linier** (*Linear Regression*)
* **Pohon Keputusan** (*Decision Tree*)
* **Random Forest**
* **K-Nearest Neighbors (KNN)**

### 4. Evaluasi & Validasi Model
Kinerja model diukur menggunakan metrik:
* **R² Score**: Mengukur proporsi variabilitas dalam variabel target yang dapat dijelaskan oleh model.
* **Root Mean Squared Error (RMSE)**: Mengukur rata-rata besarnya kesalahan prediksi.

---

## 🎯 Hasil Utama & Temuan

### Performa Model Terbaik

Model **Random Forest** terbukti menjadi yang paling akurat dalam memprediksi angka harapan hidup, mencapai kinerja yang luar biasa:

| Model | Metrik | Nilai |
| :--- | :--- | :--- |
| **Random Forest** | **R² Score** | **96.60%** |



> **Kesimpulan**: Algoritma *ensemble* seperti Random Forest sangat efektif dalam menangani kompleksitas dan non-linearitas hubungan antara berbagai faktor sosial-ekonomi dan kesehatan.

### Studi Kasus Simulasi

Sebuah simulasi dilakukan untuk menguji dampak langsung perubahan faktor tertentu:

* **Target Skenario**: Jepang, tahun 2010.
* **Intervensi**: Kenaikan PDB (*Gross Domestic Product*) sebesar **200%**.
* **Interpretasi**: Hal ini menggarisbawahi **hukum hasil yang semakin berkurang** (*law of diminishing returns*); di negara yang sudah maju dan memiliki harapan hidup tinggi, intervensi lain mungkin menjadi faktor penentu berikutnya.

---

## ▶️ Cara Menjalankan Proyek

Untuk mereplikasi hasil analisis ini, ikuti langkah-langkah di bawah:

1.  **Instalasi Python & Jupyter**: Pastikan Anda telah menginstal **Python (versi 3.x direkomendasikan)** dan **Jupyter Notebook/Lab**.

2.  **Instalasi Pustaka**: Instal semua dependensi yang diperlukan melalui `pip`. Pustaka utama yang digunakan adalah:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```

3.  **Jalankan Notebook**:
    * Buka *terminal* di direktori proyek.
    * Jalankan: `jupyter notebook`
    * Buka file **`tugas_akhir.ipynb`** dan jalankan semua sel secara berurutan.