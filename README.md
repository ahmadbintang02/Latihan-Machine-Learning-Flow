# Latihan Machine Learning Workflow

Repositori ini berisi dokumentasi dan implementasi alur kerja *end-to-end* Machine Learning yang saya pelajari pada program CodingCamp 2026 by DBS Foundation. Proyek ini mencakup seluruh proses mulai dari eksplorasi data, pelatihan model menggunakan algoritma regresi, hingga tahap *deployment* sederhana menggunakan Flask API.

## Cakupan Proyek

Dalam repositori ini, saya mendokumentasikan langkah-langkah berikut:
1. **Eksplorasi & Preprocessing Data**: Memuat dataset, menangani nilai yang hilang, dan menyiapkan data untuk pelatihan.
2. **Model Building**: Melatih model menggunakan **Gradient Boosting Regressor** untuk mendapatkan hasil prediksi yang optimal.
3. **Model Evaluation**: Menguji performa model dengan metrik evaluasi yang relevan.
4. **Model Persistence**: Menyimpan model yang telah dilatih menggunakan `joblib` agar dapat digunakan kembali tanpa pelatihan ulang.
5. **API Deployment**: Membuat web service sederhana menggunakan **Flask** yang menyediakan endpoint `/predict` untuk melayani request prediksi secara *real-time*.

## Teknologi yang Digunakan

* **Python**: Bahasa pemrograman utama.
* **Pandas & NumPy**: Manipulasi dan analisis data.
* **Scikit-Learn**: Library untuk algoritma Machine Learning.
* **Joblib**: Untuk serialisasi model.
* **Flask**: Framework web untuk pembuatan API.

## Struktur File

* `LatihanMachineLearningFlow.ipynb`: Notebook utama yang berisi seluruh proses eksperimen.
* `gbr_model.joblib`: File model yang sudah dilatih (akan dihasilkan setelah menjalankan notebook).
* `app.py`: (Opsional) Kamu bisa mengekstrak kode Flask dari notebook ke file Python ini untuk deployment yang lebih bersih.

## Cara Menjalankan API

1. Pastikan model `.joblib` sudah tersedia di direktori yang sama.
2. Jalankan aplikasi Flask:
   ```bash
   python app.py
