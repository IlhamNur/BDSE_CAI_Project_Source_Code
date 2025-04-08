# 🧠 BDSE_CAI_PROJECT_SOURCE_CODE

## 📌 Project Overview  

Proyek ini mencakup dua fokus utama:

1. **Credit Card Fraud Detection** menggunakan algoritma Machine Learning.
2. **Gender Classification from Images** menggunakan Convolutional Neural Networks (CNN).

Keduanya dilakukan secara end-to-end mulai dari preprocessing data, pelatihan model, evaluasi, hingga dokumentasi.

---

## 📁 Project Structure  

```
BDSE_CAI_PROJECT_SOURCE_CODE/
│── data/
│   ├── train/                  # Folder gambar latih (male/female)
│   ├── valid/                  # Folder gambar validasi (male/female)
│   ├── Training.zip            # ZIP data latih untuk gender classification
│   └── Validation.zip          # ZIP data validasi untuk gender classification
│
│── fraudTrain.csv              # Dataset pelatihan untuk fraud detection
│── fraudTest.csv               # Dataset pengujian untuk fraud detection
│── Capstone_Dataset.csv        # Dataset gabungan
│── best_final_model.pkl        # Model fraud detection yang telah disimpan
│── scaler.pkl                  # Skaler data yang digunakan untuk normalisasi
│── task.ipynb                  # Jupyter Notebook utama untuk seluruh project
│── requirements.txt            # Daftar dependencies Python
│── README.md                   # Dokumentasi proyek ini
```

---

## 🔧 Setup Instructions

1. **Ubah Directory**

```bash
cd BDSE_CAI_PROJECT_SOURCE_CODE
```

2. **Aktifkan Virtual Environment** (opsional tapi direkomendasikan)

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# Mac/Linux
source .venv/bin/activate
```

3. **Install Dependencies**

```bash
pip install -r requirements.txt
```

4. **Jalankan Notebook**

```bash
jupyter notebook
```

Buka `task.ipynb` dan jalankan langkah-langkah secara berurutan.

---

## 📊 Dataset Description

### Fraud Detection

- **fraudTrain.csv** dan **fraudTest.csv**: Berisi data transaksi keuangan dengan label fraud (1) dan non-fraud (0).
- **Capstone_Dataset.csv**: Dataset gabungan yang digunakan untuk eksplorasi dan visualisasi awal.

### Gender Classification

- Gambar dalam ZIP `Training.zip` dan `Validation.zip` telah diekstrak ke folder `data/train/` dan `data/valid/`, masing-masing dengan subfolder `male` dan `female`.

---

## 📌 Project Activities

### ✅ Activity 4–8: Fraud Detection

- Data cleaning, visualisasi, dan preprocessing.
- Penanganan imbalance dengan **SMOTE**.
- Pelatihan model ML: Logistic Regression, Random Forest, XGBoost, dll.
- Evaluasi: Confusion Matrix, ROC AUC, Precision, Recall, Accuracy.

### ✅ Activity 9–11: Gender Classifier

- Ekstraksi dan penataan gambar.
- Preprocessing: Resize, normalize, augmentasi.
- Arsitektur CNN menggunakan `Conv2D`, `MaxPooling`, dan `Dense`.
- Evaluasi model: Accuracy, ROC-AUC, Loss Curve.
- Simpan model terbaik.

---

## ✅ Key Features

- 📊 **EDA Lengkap** dengan visualisasi data distribusi fraud.
- 🧠 **ML Model Evaluation** dengan metrik evaluasi yang lengkap.
- 📸 **CNN untuk Klasifikasi Gambar** (Male/Female).
- 🧪 **Cross-validation & Hyperparameter Tuning**.
- 📂 **Modular & Terstruktur**.

---

## 🚀 Future Improvements

- Deploy model fraud detection ke dalam API (Flask/FastAPI).
- Tambahkan augmentasi data dan transfer learning untuk gender classification.
- Buat UI dashboard sederhana untuk presentasi hasil model.
