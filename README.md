Prediksi Pembatalan Booking Hotel Menggunakan Machine Learning
Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi apakah sebuah pemesanan hotel akan dibatalkan atau tidak menggunakan model machine learning. Model prediksi ini dapat membantu tim pemasaran dan manajemen hotel untuk mengurangi kerugian akibat pembatalan dengan mengidentifikasi segmen tamu berisiko tinggi dan melakukan tindakan preventif seperti promosi khusus atau konfirmasi ulang.

Tujuan Bisnis
Mengurangi pembatalan dengan meningkatkan retensi tamu.

Mengalokasikan anggaran marketing secara lebih efisien berdasarkan prediksi pembatalan.

Membandingkan kerugian historis dengan kerugian berdasarkan hasil prediksi ML untuk menentukan strategi marketing yang optimal.

Dataset
Dataset yang digunakan adalah Hotel Booking Demand Dataset, yang berisi informasi tentang pemesanan hotel, termasuk:

Tipe hotel, negara asal tamu, channel pemesanan, segmentasi pasar, deposit type, jumlah special request, dst.

Target variabel: is_canceled (1 = dibatalkan, 0 = tidak dibatalkan)
*Dataset Hotel Booking Demand yang digunakan sudah disederhanakan

⚙️ Preprocessing
Mengganti kategori rare dengan label 'Other'

Menangani missing value dengan label 'Unknown' untuk fitur kategorikal

Encoding menggunakan OneHotEncoder

Scaling menggunakan RobustScaler (untuk menangani outlier)

Pipeline terpisah untuk numerik dan kategorikal

🤖 Model Machine Learning
Model yang diuji:

Logistic Regression
Decision Tree Classifier
K-Nearest Neighbors (KNN)
XGBoost
Random Forest Classifier (terpilih sebagai model terbaik)
LGBM

Model terbaik dipilih berdasarkan metrik:
Recall untuk kelas 1 (pembatalan) karena lebih penting untuk meminimalkan kerugian

Rencana Selanjutnya
Optimalisasi Fallback handling, Interpretasi dengan shap, uji coba resampling

