🧪 Hepatitis Dataset Classification

Program ini memuat dan memproses dataset Hepatitis dari UCI Machine Learning Repository, lalu menerapkan beberapa algoritma klasifikasi untuk memprediksi kondisi pasien (mengidap hepatitis atau tidak).

📥 Dataset
Dataset diambil secara otomatis menggunakan `ucimlrepo` dengan ID UCI = `46`.

🔧 Langkah-Langkah

1. Import Data  
   Mengambil dataset dari UCI dan menggabungkan fitur serta target ke dalam satu DataFrame.

2. Preprocessing
   - Mengubah data kategorikal menjadi numerik (`LabelEncoder`)
   - Mengisi nilai kosong dengan median (`SimpleImputer`)
   - Menstandarisasi fitur numerik (`StandardScaler`)

3. Split Data  
   Memisahkan data menjadi training dan testing dengan rasio 70:30.

4. Model Training & Evaluation
   Melatih dan mengevaluasi performa 4 model klasifikasi:
   - Random Forest Classifier
   - Decision Tree Classifie
   - Naive Bayes
   - Logistic Regression

   Evaluasi dilakukan menggunakan:
   - Akurasi
   - Precision, Recall, F1-Score (via `classification_report`)
   - Confusion Matrix

5. Visualisasi
   - Menampilkan feature importances untuk Random Forest
   - Visualisasi pohon keputusan (Decision Tree)

📊 Output
Program mencetak:
- Classification report dari keempat model
- Grafik top 10 feature importances (Random Forest)
- Struktur visual dari Decision Tree

