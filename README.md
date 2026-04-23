🧬 Analisis Metilasi DNA: SAR vs Kontrol
Proyek ini bertujuan untuk menganalisis pola metilasi DNA pada penderita Stomatitis Aftosa Rekuren (SAR) dibandingkan dengan kelompok Kontrol. Menggunakan teknik Machine Learning untuk mengidentifikasi biomarker potensial berdasarkan persentase metilasi pada posisi nukleotida tertentu.

📊 Dataset
Data penelitian disimpan dalam format Excel (Data Metilasi DNA SAR.xlsx) yang mencakup:

Fitur: Persentase metilasi pada 6 posisi spesifik (Posisi 1 hingga Posisi 6).

Target: Klasifikasi subjek ke dalam kelas SAR atau Kontrol.

Karakteristik Data: Terdapat tantangan berupa missing values, terutama pada Posisi 6 (~73% kosong).

🛠️ Metodologi Analisis
Proses pengolahan data dalam notebook ini meliputi:

Data Cleaning: Pembersihan spasi pada string, konversi nilai non-numerik (NA) menjadi NaN, dan penyesuaian tipe data.

Exploratory Data Analysis (EDA): Visualisasi distribusi data menggunakan Boxplot untuk melihat perbedaan persebaran nilai metilasi antar kelompok.

Machine Learning:

Preprocessing: Standarisasi fitur menggunakan StandardScaler.

Model: Implementasi algoritma klasifikasi (seperti SVM atau Random Forest).

Optimasi: Tuning hyperparameter menggunakan GridSearchCV.

Validasi: Menggunakan Cross-Validation untuk memastikan model tidak overfit.

📈 Performa Model
Berdasarkan hasil evaluasi terakhir, model mencapai performa sebagai berikut:

Kelompok Kontrol: Precision 0.85, Recall 0.81, F1-Score 0.83.

Kelompok SAR: Precision 0.82, Recall 0.85, F1-Score 0.83.

Akurasi Keseluruhan: ~83%.

💻 Cara Penggunaan
Buka notebook SAR_vs_Kontrol_.ipynb di Google Colab.

Hubungkan (Mount) Google Drive untuk mengakses file dataset.

Pastikan library berikut terinstal:

Bash
pip install pandas numpy seaborn matplotlib scikit-learn
Jalankan semua sel untuk melihat hasil visualisasi dan performa klasifikasi.

🗂️ Struktur Proyek
SAR_vs_Kontrol_.ipynb: Notebook utama analisis.

Data Metilasi DNA SAR.xlsx: Dataset mentah (diperlukan di Google Drive).
