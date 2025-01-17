# Crop Yield Prediction using CNN-LSTM

## Identitas Lengkap
- **Nama**: Matthew Raymond Hartono  
- **NIM**: A11.2022.99XY  
- **Dosen**: Abu Salam, M.Kom  

## Ringkasan dan Permasalahan Project
### Ringkasan
Proyek ini bertujuan untuk memprediksi hasil panen tanaman berbasis data iklim dan variabel lain yang relevan. Model yang digunakan adalah kombinasi CNN (Convolutional Neural Network) dan LSTM (Long Short-Term Memory) untuk menangani data spasial dan temporal secara bersamaan.

### Permasalahan
Masalah utama yang ingin diselesaikan adalah ketidakpastian hasil panen akibat perubahan iklim yang sulit diprediksi, yang memengaruhi sektor agrikultur secara global.

### Tujuan
- Memprediksi hasil panen dengan akurasi tinggi.  
- Membantu petani dan pembuat kebijakan untuk mengelola hasil panen secara lebih efektif.

### Model / Alur Penyelesaian
![Model Workflow](https://github.com/matthewraymondh/Crop-Yield-Prediction-using-CNN-LSTM/blob/main/assets/workflow.png)

1. Pengumpulan dan preprocessing data.
2. Eksplorasi Data (EDA) dan Analisis Fitur.
3. Pembentukan model CNN-LSTM.
4. Pelatihan dan evaluasi model.
5. Diskusi hasil dan implementasi praktis.

## Penjelasan Dataset
- **Dataset**: Dataset mengandung data iklim (temperatur, curah hujan, kelembaban) dan hasil panen dari berbagai wilayah.
- **EDA**: Analisis statistik dan visualisasi hubungan antar fitur dilakukan untuk memahami pola data.
- **Proses Features Dataset**:
  - Normalisasi nilai fitur agar data terstandardisasi.
  - Transformasi data menjadi format time-series untuk digunakan pada LSTM.

## Proses Learning / Modeling
- **Arsitektur Model**: CNN digunakan untuk ekstraksi fitur spasial, sementara LSTM digunakan untuk mempelajari pola temporal.
- **Framework**: TensorFlow/Keras digunakan untuk membangun dan melatih model.
- **Hyperparameter**: Batch size, learning rate, dan jumlah epoch dioptimasi untuk mendapatkan performa terbaik.

## Performa Model
- **Metrics**: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), dan R2 Score digunakan untuk evaluasi.
- **Hasil**:
  - MAE: 12.45
  - RMSE: 18.32
  - R2 Score: 0.89

## Diskusi Hasil dan Kesimpulan
- Model CNN-LSTM mampu menangkap pola kompleks antara variabel iklim dan hasil panen dengan baik.
- Performanya menunjukkan potensi penggunaan model ini dalam skenario dunia nyata.
- Implementasi model ini dapat digunakan untuk perencanaan panen dan mitigasi risiko dalam pertanian.

## Deployment
Proyek ini dideploy menggunakan Streamlit Community Cloud untuk visualisasi hasil prediksi.  
**URL Deployment**: [Crop Yield Prediction App](https://streamlit.app/Crop-Yield-Prediction)

## Panduan Repository
1. Clone repository:
   ```bash
   git clone https://github.com/matthewraymondh/Crop-Yield-Prediction-using-CNN-LSTM.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan aplikasi Streamlit:
   ```bash
   streamlit run app.py
   ```

## Struktur Repository
- `data/` : Dataset yang digunakan.
- `notebooks/` : Jupyter Notebook untuk dokumentasi proses.
- `models/` : Model terlatih dan arsitekturnya.
- `assets/` : Gambar dan grafik pendukung.
- `app.py` : Aplikasi Streamlit.
- `README.md` : Dokumentasi proyek.

---

Repository ini dibuat sebagai bagian dari tugas UAS mata kuliah STKI. Silakan mengakses file dan dokumentasi lengkap melalui link repository ini: [STKI-NIM-UAS](https://github.com/matthewraymondh/Crop-Yield-Prediction-using-CNN-LSTM).
