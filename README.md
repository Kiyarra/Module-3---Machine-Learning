[Data California House ](https://drive.google.com/drive/u/0/folders/19YA_f36uGR86hTnZuX-Ech59s3AFzXXo)

### **Contents**

1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

## 1. Business Problem Understanding

**Context**

Dataset yang digunakan pada projek ini merupakan kumpulan data perumahan di wilayah California, Amerika Serikat, yang diambil dari hasil sensus tahun 1990.

Dataset ini memuat berbagai informasi demografis seperti pendapatan rata-rata penduduk, jumlah populasi, dan tingkat hunian rumah di setiap distrik.

Selain itu, terdapat juga informasi geografis seperti latitude dan longitude, serta karakteristik rumah seperti jumlah kamar, jumlah kamar tidur, dan usia rata-rata rumah di wilayah tersebut.

Informasi ini sangat relevan bagi industri properti, karena dapat menggambarkan bagaimana kondisi sosial-ekonomi suatu daerah berhubungan dengan nilai pasar properti di area tersebut.

**Problem Statement**

Salah satu tantangan utama yang dihadapi developer perumahan adalah menentukan harga jual rumah yang tepat serta memilih lokasi pengembangan yang sesuai dengan daya beli dan kebutuhan pasar.
Kesalahan dalam menilai potensi suatu wilayah dapat berdampak pada kerugian besar — misalnya membangun rumah dengan harga tinggi di daerah dengan pendapatan rendah, atau sebaliknya, membangun rumah standar di kawasan elit dengan potensi keuntungan besar.
Oleh karena itu, dibutuhkan sebuah pendekatan berbasis data yang mampu membantu developer memahami hubungan antara faktor demografis, geografis, dan karakteristik rumah terhadap nilai pasar properti di California.

**Goals**

Tujuan utama dari projek ini adalah membangun model machine learning yang mampu memprediksi median house value atau harga jual median rumah berdasarkan fitur-fitur yang tersedia dalam dataset.

Dengan memanfaatkan variabel seperti jumlah kamar, pendapatan rata-rata penduduk, kepadatan populasi, dan jarak terhadap laut, model ini diharapkan dapat membantu perusahaan properti untuk:

1. Menentukan strategi harga yang kompetitif,
2. Mengidentifikasi wilayah potensial untuk investasi, dan
3. Merancang strategi pemasaran dan pengembangan produk yang sesuai dengan karakteristik pasar lokal.

Selain itu, hasil prediksi juga dapat menjadi dasar pengambilan keputusan strategis jangka panjang, seperti:
- perencanaan ekspansi kawasan perumahan,
- penerapan dynamic pricing strategy, dan
- evaluasi portofolio investasi berdasarkan tren demografi dan lokasi geografis.

**Analytic Approach**

Pendekatan analitik yang digunakan adalah regresi, karena target variabel yang ingin diprediksi, yaitu median_house_value, bersifat numerik dan kontinu.

Tahapan analisis diawali dengan eksplorasi data untuk memahami pola hubungan antara fitur demografis, geografis, dan karakteristik rumah dengan harga median.
Selanjutnya, dilakukan pembangunan model prediktif menggunakan beberapa algoritma regresi seperti Linear Regression, Decision Tree, Random Forest, Gradient Boosting, dan XGBoost.

Pemilihan algoritma terbaik akan didasarkan pada performa model dalam meminimalkan error, dengan tujuan akhir menghasilkan model yang akurat, stabil, dan dapat diinterpretasikan secara bisnis.

**Metric Evaluation**

Untuk mengevaluasi performa model, digunakan beberapa metrik regresi, antara lain:
- Root Mean Squared Error (RMSE) : untuk mengukur rata-rata deviasi kuadrat dari prediksi terhadap nilai aktual,
- Mean Absolute Error (MAE) ; untuk menghitung rata-rata kesalahan absolut, dan
- Mean Absolute Percentage Error (MAPE) : untuk mengukur rata-rata kesalahan dalam bentuk persentase.

> Semakin kecil nilai RMSE, MAE, dan MAPE, semakin baik model dalam memprediksi harga rumah.

Selain itu, jika model yang digunakan bersifat linear, metrik tambahan seperti R-squared (R²) atau Adjusted R² dapat digunakan untuk mengukur seberapa baik variabel-variabel independen menjelaskan variasi target.
Namun, metrik ini tidak relevan untuk model non-linear seperti Random Forest atau XGBoost.
