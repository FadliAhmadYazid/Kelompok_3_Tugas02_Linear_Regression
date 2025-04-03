# Analisis Prediksi Gaji Menggunakan Regresi Linear dan Polinomial

Repositori ini berisi implementasi model regresi linear dan polinomial untuk memprediksi gaji karyawan berdasarkan dataset "Salary Data". Analisis ini dilakukan sebagai bagian dari tugas mata kuliah Pembelajaran Mesin di Universitas Syiah Kuala.

## Anggota Kelompok 3

- Meutia Aini (2208107010005)
- Akhsania Maisa Rahmah (2208107010017)
- Fadli Ahmad Yazid (2208107010032)
- Muhammad Mahathir (2208107010056)
- Muhammad Aufa Zaikra (2208107010070)

## Deskripsi Proyek

Proyek ini menganalisis dataset "Salary Data" dari Kaggle yang berisi informasi karyawan seperti usia, jenis kelamin, tingkat pendidikan, jabatan pekerjaan, tahun pengalaman kerja, dan gaji tahunan. Fokus utama analisis adalah membangun model prediksi gaji menggunakan fitur utama: pengalaman kerja, tingkat pendidikan, dan jabatan pekerjaan.

## Tujuan

1. Memahami karakteristik dataset melalui eksplorasi data
2. Membangun model regresi linear dan polinomial untuk memprediksi gaji
3. Mengevaluasi performa model menggunakan metrik MAE, MSE, RMSE, dan R²
4. Menginterpretasikan hasil model dan menentukan model terbaik

## Struktur Repositori

- `Laporan_Proyek2ML.pdf`: Laporan lengkap proyek yang berisi metodologi, hasil, dan analisis
- `Notebook_Tugas02_Linear_Regression.ipynb`: Jupyter Notebook dengan implementasi kode dan visualisasi
- `README.md`: Dokumentasi proyek
- `Salary_Data.csv`: Dataset yang digunakan dalam analisis

## Dataset

Dataset "Salary Data" terdiri dari 6.704 entri dengan 6 kolom utama:
- Age: Usia karyawan (numerik, dalam tahun)
- Gender: Jenis kelamin (kategorikal: Male, Female, Other)
- Education Level: Tingkat pendidikan (kategorikal: High School, Bachelor's, Master's, PhD)
- Job Title: Jabatan pekerjaan (kategorikal)
- Years of Experience: Tahun pengalaman kerja (numerik)
- Salary: Gaji tahunan dalam dolar (numerik, variabel target)

## Metodologi

### Tahapan Analisis

1. **Pemahaman Dataset**: Eksplorasi awal dan statistik deskriptif
2. **Eksplorasi Data dan Pra-pemrosesan**:
   - Pemeriksaan dan penanganan missing values
   - Standardisasi nilai kategorikal
   - Encoding fitur kategorikal menggunakan OneHotEncoder
   - Standarisasi fitur numerik dengan StandardScaler
   - Analisis korelasi antar variabel
3. **Implementasi Model**:
   - Regresi Linear
   - Regresi Polinomial (derajat 2 dan 3)
4. **Evaluasi Model** menggunakan metrik:
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - R-squared (R²)
5. **Analisis Hasil** dan visualisasi perbandingan model

## Hasil Utama

Perbandingan performa model:

| Model | MAE | MSE | RMSE | R² |
|-------|-----|-----|------|-----|
| Regresi Linear | 15487.83 | 458246826.30 | 21406.70 | 0.84 |
| Regresi Polinomial (Derajat 2) | 10155.95 | 247653840.17 | 15737.02 | 0.91 |
| Regresi Polinomial (Derajat 3) | 9940.47 | 740203043.98 | 27206.67 | 0.74 |

## Kesimpulan

- Regresi polinomial derajat 2 memberikan performa terbaik dengan R² tertinggi (0.91) dan error terendah
- Pengalaman kerja memiliki hubungan non-linear dengan gaji, yang lebih baik ditangkap oleh model polinomial
- Regresi polinomial derajat 3 menunjukkan tanda-tanda overfitting dengan R² yang lebih rendah dan MSE yang jauh lebih tinggi

## Instalasi dan Penggunaan

1. Clone repositori ini:
   ```
   git clone https://github.com/FadliAhmadYazid/Kelompok_3_Tugas02_Linear_Regression.git
   ```

2. Instal dependensi yang diperlukan:
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

3. Jalankan Jupyter Notebook untuk melihat analisis lengkap:
   ```
   jupyter notebook Notebook_Tugas02_Linear_Regression.ipynb
   ```

## Referensi

- Dataset "Salary Data" dari Kaggle: [https://www.kaggle.com/datasets/mohithsairamreddy/salary-data](https://www.kaggle.com/datasets/mohithsairamreddy/salary-data)
