# Personal Bank Loan Classification - Klasifikasi Calon Nasabah Pinjaman Potensial Bank

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-green.svg)

## 📋 Deskripsi Project

Project ini merupakan implementasi machine learning untuk mengklasifikasikan calon nasabah pinjaman potensial bank menggunakan algoritma **Decision Tree** dan **Random Forest**. Tujuan utama adalah untuk mengidentifikasi nasabah yang kemungkinan besar akan membeli pinjaman pribadi berdasarkan berbagai fitur seperti umur, pendapatan, tingkat pendidikan, dan lainnya.

### 🎯 Tujuan Project

1. **Meningkatkan Efisiensi**: Memproses aplikasi pinjaman dengan lebih cepat dan akurat
2. **Optimasi Sumber Daya**: Mengalokasikan sumber daya untuk pemasaran produk pinjaman kepada nasabah yang paling potensial
3. **Meningkatkan Kepuasan Nasabah**: Memberikan pengalaman yang lebih baik dengan penawaran yang tepat

## 👥 Tim Pengembang

**Kelompok 1 - Foundation of Data Science (B)**

- I Made Dwika Dyananda Kumara (2105551074)
- Made Wahyu Adwitya Pramana (2105551092)
- I Kadek Rai Pramana (2105551094)

## 📊 Dataset

Dataset yang digunakan adalah **Bank Personal Loan Modelling** yang berisi informasi nasabah bank meliputi:

- **Demographics**: Umur, ZIP Code
- **Financial Information**: Pendapatan, CCAvg (Credit Card Average)
- **Banking Relationship**: Experience, Family Size, Securities Account, CD Account, Online, Credit Card
- **Education Level**: Tingkat pendidikan
- **Target Variable**: Personal Loan (0 = Tidak, 1 = Ya)

## 🛠️ Teknologi yang Digunakan

### Libraries & Framework

```python
# Data Processing & Analysis
- pandas
- numpy
- ydata_profiling

# Visualization
- matplotlib
- seaborn

# Statistical Analysis
- scipy
- pingouin

# Machine Learning
- scikit-learn
  - DecisionTreeClassifier
  - RandomForestClassifier
  - GridSearchCV
  - StratifiedKFold
  - PCA
  - StandardScaler
```

## 🚀 Cara Menjalankan Project

### Prerequisites

```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scipy pingouin scikit-learn ydata_profiling gdown
```

### Menjalankan Notebook

1. Clone repository ini:
```bash
git clone https://github.com/rai-pramana/FDS-Personal-Bank-Loan-Classification.git
cd FDS-Personal-Bank-Loan-Classification
```

2. Buka Jupyter Notebook:
```bash
jupyter notebook
```

3. Jalankan file notebook:
   - `UAS_FDS_Kelompok 1_Personal Bank Loan Classification.ipynb` - Notebook utama dengan analisis lengkap
   - `imbalanced-personal-bank-loan-classification.ipynb` - Notebook untuk handling imbalanced data

## 📈 Metodologi

### 1. Exploratory Data Analysis (EDA)
- Data profiling menggunakan ydata_profiling
- Analisis statistik deskriptif
- Visualisasi distribusi data
- Analisis korelasi fitur

### 2. Data Preprocessing
- Handling missing values
- Feature scaling menggunakan StandardScaler
- Handling imbalanced data (jika diperlukan)
- Feature engineering

### 3. Model Development
- **Decision Tree Classifier**
  - Model baseline
  - Mudah diinterpretasikan
  - Rentan terhadap overfitting

- **Random Forest Classifier**
  - Ensemble learning dengan multiple decision trees
  - Lebih robust terhadap overfitting
  - Higher performance

### 4. Model Evaluation & Optimization
- Train-Test Split dengan stratifikasi
- Cross-validation menggunakan StratifiedKFold
- Hyperparameter tuning dengan GridSearchCV
- Dimensionality reduction dengan PCA

### 5. Metrics Evaluation
- **Accuracy Score**: Tingkat akurasi keseluruhan
- **Precision Score**: Presisi prediksi positif
- **Recall Score**: Sensitivitas model
- **F1 Score**: Harmonic mean dari precision dan recall
- **ROC-AUC Score**: Area under ROC curve
- **Confusion Matrix**: Visualisasi performa klasifikasi
- **Classification Report**: Laporan komprehensif

## 📊 Hasil dan Temuan

*(Hasil akan bervariasi tergantung pada data dan hyperparameter yang digunakan)*

### Model Performance
- Model terbaik akan dipilih berdasarkan multiple metrics
- Analisis feature importance untuk memahami faktor penentu
- Visualisasi ROC curve dan confusion matrix

### Key Insights
- Identifikasi fitur-fitur yang paling berpengaruh terhadap keputusan pinjaman
- Rekomendasi strategi marketing berbasis data
- Trade-off antara precision dan recall

## 📁 Struktur Project

```
FDS-Personal-Bank-Loan-Classification/
│
├── UAS_FDS_Kelompok 1_Personal Bank Loan Classification.ipynb  # Notebook utama
├── imbalanced-personal-bank-loan-classification.ipynb          # Notebook handling imbalanced
├── README.md                                                    # Dokumentasi project
└── bank_personal_loan_modelling.xlsx                           # Dataset (downloaded)
```

## 🔍 Algoritma yang Digunakan

### Decision Tree
Decision Tree adalah algoritma yang membagi dataset menjadi subset yang lebih kecil berdasarkan nilai fitur tertentu, membentuk struktur seperti pohon keputusan.

**Kelebihan:**
- Mudah diinterpretasikan
- Tidak memerlukan feature scaling
- Dapat menangani data numerik dan kategorikal

**Kekurangan:**
- Rentan terhadap overfitting
- Sensitif terhadap noise dalam data

### Random Forest
Random Forest adalah algoritma ensemble yang terdiri dari banyak Decision Tree. Setiap pohon memberikan prediksi, lalu prediksi final diambil berdasarkan mayoritas voting.

**Kelebihan:**
- Lebih tahan terhadap overfitting
- Performance lebih baik dibanding single decision tree
- Dapat memberikan feature importance

**Kekurangan:**
- Lebih sulit diinterpretasikan
- Membutuhkan lebih banyak computational resources

## 📚 Referensi

- Scikit-learn Documentation: https://scikit-learn.org/
- Pandas Documentation: https://pandas.pydata.org/
- Seaborn Documentation: https://seaborn.pydata.org/

## 📝 License

This project is open source and available for educational purposes.

## 📧 Kontak

Untuk pertanyaan atau diskusi lebih lanjut, silakan hubungi tim melalui GitHub issues atau repository ini.

---

**Foundation of Data Science (B) - Ujian Akhir Semester**