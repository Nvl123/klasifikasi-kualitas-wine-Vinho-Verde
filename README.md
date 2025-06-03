
# **Klasifikasi Kualitas Wine Vinho Verde untuk Optimalisasi Strategi Penetapan Harga dan Target Pasar**

![gambar wine vinho verde](https://static.independent.co.uk/2023/07/13/11/vintages-buy-43784e0e-11dc-11ee-9aaf-3ad6dbe6fd05.jpg?quality=75&width=1250&crop=3%3A2%2Csmart&auto=webp)

## **Latar Belakang**
Region Vinho Verde di Portugal sudah lama dikenal sebagai produsen anggur yang unik dengan karakter rasa yang segar, asam, dan sedikit bergelembung (frizzante). Anggur dari daerah ini terdiri dari jenis putih dan merah, dengan varietas putih yang paling populer seperti Alvarinho, Loureiro, dan Arinto, sementara varietas merah biasanya menggunakan Vinhão dan Espadeiro. Anggur Vinho Verde biasanya dipasarkan sebagai minuman yang ringan dan terjangkau, sangat cocok untuk dikonsumsi sehari-hari maupun sebagai pendamping hidangan laut atau makanan ringan pada musim panas. [[1]](https://doi.org/10.1016/j.foodres.2018.05.077) [[2]](https://doi.org/10.1016/J.ACA.2003.10.020)

Namun, dengan semakin ketatnya persaingan di pasar anggur global dan perubahan selera konsumen yang kini lebih menghargai anggur berkualitas tinggi serta kisah asal-usul (terroir) yang jelas, produsen Vinho Verde mulai berfokus pada peningkatan kualitas produk mereka [[3]](https://doi.org/10.3390/su12072819). Konsumen saat ini cenderung memilih anggur yang tidak hanya enak, tetapi juga memiliki identitas geografis yang kuat, seperti jenis tanah, iklim, dan metode budidaya khas wilayah tertentu. Hal ini sejalan dengan tren global di mana atribut terroir dan cerita keaslian produk memainkan peran penting dalam keputusan pembelian, terutama di pasar yang menghargai tradisi dan keberlanjutan [[4]](https://doi.org/10.1016/J.JCLEPRO.2021.126991).

Terroir sendiri merujuk pada kondisi lingkungan tempat anggur ditanam—meliputi tanah, iklim, topografi, serta praktik budidaya—yang secara signifikan memengaruhi rasa dan karakter anggur tersebut [[5]](https://doi.org/10.1177/14707853231202759). Dengan memahami dan menonjolkan karakteristik terroir, produsen Vinho Verde dapat menciptakan anggur dengan profil rasa yang unik, membedakan diri dari kompetitor, dan meningkatkan daya tarik produknya di mata konsumen global.

Selain itu, untuk menyesuaikan diri dengan pasar yang semakin selektif, para produsen juga mulai memanfaatkan pendekatan klasifikasi kualitas berbasis analisis kimia, sensorik, bahkan machine learning guna mengelompokkan dan memasarkan anggur berdasarkan karakteristik unggulannya. Pendekatan ini membantu membangun kepercayaan konsumen, memperkuat reputasi merek, serta mendukung strategi penjualan yang lebih tertarget dan efisien [[6]](https://doi.org/10.5815/ijisa.2022.05.04). 

Oleh karena itu, klasifikasi dan peningkatan kualitas anggur Vinho Verde menjadi sangat penting untuk membantu produsen menentukan strategi harga yang tepat dan menargetkan segmen pasar yang berbeda, dari konsumen yang mencari anggur ringan dan ekonomis hingga pecinta anggur yang mengutamakan kualitas dan cerita di balik setiap botol.

---

## **Business Understanding**
### **Problem Statements**
1. Perubahan pasar yang lebih menginginkan wine dengan kualitas tinggi
2. Sulitnya proses klasifikasi kualitas anggur berdasarkan karakteristik kimiawinya yang kompleks
3. Kurangnya metode efektif yang dapat mengelompokkan anggur ke 
dalam kategori kualitas yang sesuai untuk strategi pemasaran.

### **Goals**
1. Mengembangkan model machine learning yang akurat untuk mengklasifikasikan kualitas anggur Vinho Verde berdasarkan data analisis kimia, sensorik, dan faktor terroir.
2. Meningkatkan efisiensi proses klasifikasi anggur sehingga produsen dapat dengan mudah mengelompokkan produk mereka ke dalam kategori kualitas yang tepat.
3. Memperkuat daya saing produk Vinho Verde di pasar global dengan menghadirkan produk yang memiliki identitas kualitas yang jelas dan berbasis data.

### **Solutions Statements**
1. Mengimplementasikan berbagai algoritma machine learning terkemuka seperti Random Forest, Support Vector Machine (SVM), XGBoost, K-Nearest Neighbours (KNN), dan Gradient Boosting untuk mengklasifikasikan kualitas anggur Vinho Verde berdasarkan parameter fisikokimia[[7]](https://doi.org/10.55041/ijsrem40168) [[8]](https://doi.org/10.1109/ESCI59607.2024.10497300) [[9]](https://doi.org/10.1016/j.dss.2009.05.016).
2. Menggunakan data input berupa parameter fisikokimia anggur (kandungan alkohol, volatilitas asam, tingkat keasaman, gula residu) yang telah terbukti efektif dalam merepresentasikan karakteristik kualitas anggur.
3. Melakukan evaluasi dan perbandingan performa model machine learning yang berbeda guna memilih model terbaik yang paling sesuai untuk klasifikasi kualitas anggur Vinho Verde.
4. Menerapkan pendekatan berbasis data untuk melengkapi atau menggantikan analisis sensorik manual, yang selama ini rentan subjektivitas dan keterbatasan sumber daya manusia.

---

## **Data Understanding**
### **Dataset Informations**
| Jenis | Keterangan |
|-------|------------|
|Nama   | Wine Quality|
|Sumber | [Kaggle](https://www.kaggle.com/datasets/rajyellow46/wine-quality)|
|Pengelola| [Raj Parmar](https://www.kaggle.com/rajyellow46)
|Lisensi| Tidak Spesifik|
|Visibilitas| Publik|
|Label| *Earth and Nature, Classification, Alcohol, Regression*|
|Kebergunaan| 7.6|

dataset ini diambil dari kaggle yang di unggah atau di kelola oleh [Raj Parmar](https://www.kaggle.com/rajyellow46) namun setelah di telusuri kembali ternyata asal dataset ini dari repository [UC Irvine Datasets](https://archive.ics.uci.edu/datasets) yang di unggah dengan nama yang sama [Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality).

### **Variabel Description**
| type  | fixed acidity | volatile acidity | citric acid | residual sugar | chlorides | free sulfur dioxide | total sulfur dioxide | density  | pH   | sulphates | alcohol | quality |
|-------|---------------|------------------|-------------|----------------|-----------|---------------------|----------------------|----------|------|-----------|---------|---------|
| white | 6.8           | 0.300            | 0.29        | 6.2            | 0.025     | 29.0                | 95.0                 | 0.99071  | 3.03 | 0.32      | 12.9    | 7       |
| white | 6.4           | 0.220            | 0.56        | 14.5           | 0.055     | 27.0                | 159.0                | 0.99800  | 2.98 | 0.40      | 9.1     | 5       |
| white | 6.4           | 0.595            | 0.14        | 5.2            | 0.058     | 15.0                | 97.0                 | 0.99510  | 3.38 | 0.36      | 9.0     | 4       |


dari tabel di atas kita mendapatkan informasi jumlah label atau variabel dari datase. terdapat 13 variabel:
1. `type` -> tipe wine 
2. `fixed acidity`-> Asam tetap dalam anggur
3. `Volatile acidity` -> Asam yang mudah menguap
4. `Citric acid` -> Asam Sitrat
5. `Residual sugar` -> Gula sisa pasca fermentasi
6. `Chlorides` -> kandungan garam (Klorida)
7. `Free sulfur dioxide` -> SO₂ bebas yang berfungsi sebagai pengawet
8. `Total sulfur dioxide` -> Jumlah total SO₂ (bebas + terikat) 
9. `Density` -> Masa jenis anggur
10. `pH` -> Tingkat keasaman
11. `Sulphates` -> Kandungan Sulfat
12. `Alcohol` -> Kandungan alkohol dalam persen volume
13. `Quality` -> Skor kualitas anggur  


| No | Column                | Non-Null Count | Data Type |
|----|-----------------------|----------------|-----------|
| 0  | type                  | 6497           | object    |
| 1  | fixed acidity         | 6487           | float64   |
| 2  | volatile acidity      | 6489           | float64   |
| 3  | citric acid           | 6494           | float64   |
| 4  | residual sugar        | 6495           | float64   |
| 5  | chlorides             | 6495           | float64   |
| 6  | free sulfur dioxide   | 6497           | float64   |
| 7  | total sulfur dioxide  | 6497           | float64   |
| 8  | density               | 6497           | float64   |
| 9  | pH                    | 6488           | float64   |
| 10 | sulphates             | 6493           | float64   |
| 11 | alcohol               | 6497           | float64   |
| 12 | quality               | 6497           | int64     |

kemudian pada tabel di atas kita mendapatkan informasi:
1. 10 variabel berbentuk `float64`, 1 berbentuk `object` dan 1 berbentuk `int64`
2. terdapat beberapa nilai null atau mungkin duplikat pada data, ini terlihat dari jumlah baris pada beberapa kolom jumlahnya berbeda.

| Statistik | fixed acidity | volatile acidity | citric acid | residual sugar | chlorides | free sulfur dioxide | total sulfur dioxide | density  | pH    | sulphates | alcohol | quality |
|-----------|---------------|------------------|-------------|----------------|-----------|---------------------|----------------------|----------|-------|-----------|---------|---------|
| count     | 6487          | 6489             | 6494        | 6495           | 6495      | 6497                | 6497                 | 6497     | 6488  | 6493      | 6497    | 6497    |
| mean      | 7.22          | 0.34             | 0.32        | 5.44           | 0.06      | 30.53               | 115.74                | 0.99     | 3.22  | 0.53      | 10.49   | 5.82    |
| std       | 1.30          | 0.16             | 0.15        | 4.76           | 0.04      | 17.75               | 56.52                 | 0.003    | 0.16  | 0.15      | 1.19    | 0.87    |
| min       | 3.80          | 0.08             | 0.00        | 0.60           | 0.01      | 1.00                | 6.00                  | 0.99     | 2.72  | 0.22      | 8.00    | 3.00    |
| 25%       | 6.40          | 0.23             | 0.25        | 1.80           | 0.04      | 17.00               | 77.00                 | 0.99     | 3.11  | 0.43      | 9.50    | 5.00    |
| 50%       | 7.00          | 0.29             | 0.31        | 3.00           | 0.05      | 29.00               | 118.00                | 0.99     | 3.21  | 0.51      | 10.30   | 6.00    |
| 75%       | 7.70          | 0.40             | 0.39        | 8.10           | 0.07      | 41.00               | 156.00                | 0.99     | 3.32  | 0.60      | 11.30   | 6.00    |
| max       | 15.90         | 1.58             | 1.66        | 65.80          | 0.61      | 289.00              | 440.00                | 1.04     | 4.01  | 2.00      | 14.90   | 9.00    |


dari tabel di atas kita mendapatkan beberapa informasi tambahan :
1. Kadar rata-rata fixed acidity adalah sekitar 7.22.
2. Residual sugar (gula tersisa) rata-rata 5.44, yang menunjukkan sebagian besar anggur memiliki kadar gula rendah sampai sedang.
3. Variabel residual sugar dan total sulfur dioxide memiliki standar deviasi cukup besar (4.76 dan 56.52), menunjukkan variasi nilai yang luas.
4. 50% (median) dari fixed acidity adalah 7.00, menunjukkan distribusi simetris mendekati rata-rata.
5. Median residual sugar adalah 3.00, lebih rendah dari rata-rata (5.44), artinya distribusi agak skew ke kanan (ada beberapa nilai tinggi ekstrim).
6. Fixed acidity maksimal 15.90, cukup jauh dari rata-rata, menunjukkan adanya beberapa anggur dengan kandungan asam tinggi.
7. Residual sugar maksimum sangat tinggi yaitu 65.80, kemungkinan ada anggur yang sangat manis.

### Univariate Analysis
![univariate](https://github.com/user-attachments/assets/58e3d0e5-da8e-4b42-a580-8aa75e7cd431)

dari hasil histogram maka:

1. `Fixed Acidity`-> cenderung normal dengan puncak frekuensi sekitar 6-7.
2. `Volatile Acidity` -> Distribusinya miring ke kanan, dengan nilai mayoritas volatile acidity rendah, sekitar 0.2-0.4, dan ada beberapa nilai tinggi yang jarang.
3. `Citric Acid` -> Sebagian besar nilai rendah, sekitar 0.2-0.4, dengan distribusi miring ke kanan dan banyak nilai kecil mendekati nol.
4. `Residual Sugar`-> didominasi oleh angka rendah (0-10), tapi ada beberapa nilai outlier yang cukup tinggi (hingga sekitar 60).
5. `Chlorides`-> sangat terkonsentrasi di bawah 0.1 dengan puncak frekuensi sangat tinggi pada nilai rendah.
6. `Free Sulfur Dioxide`-> berada di kisaran 10-50, dengan frekuensi menurun untuk nilai yang lebih tinggi.
7. `Total Sulfur Dioxide` -> relatif lebih merata, tapi tetap banyak nilai yang berkisar 100-200.
8. `Density`-> hampir seragam pada nilai sekitar 0.99-1.0 dengan sedikit variasi, mendekati distribusi normal dengan puncak di sekitar 0.995.
9. `pH` -> mendekati normal dengan nilai puncak sekitar 3.2-3.3.
10. `Sulphates` -> Mayoritas berkisar di 0.4-0.7, dengan distribusi miring ke kanan.
11. `Alcohol` -> tersebar cukup merata antara 9-12, dengan puncak frekuensi sekitar 9-10 dan 11.
12. `Quality` -> Distribusi kualitas anggur menunjukkan nilai paling banyak pada 5 dan 6, dengan sedikit nilai kualitas tinggi (7-8) dan rendah (3-4).

**Kesimpulan:**

- Sebagian besar fitur menunjukkan distribusi yang tidak simetris, dengan beberapa memiliki outlier yang signifikan seperti residual sugar dan sulfur dioxide.

- Nilai kualitas anggur lebih sering berada di rentang menengah (5-6).

- Data menunjukkan beberapa fitur sangat terkonsentrasi pada nilai rendah (seperti chlorides dan volatile acidity).

### Multivariate Analysis

![multivariate](https://github.com/user-attachments/assets/101c5d2f-3277-4da6-9db0-e1df9e12dbe2)



**Kesimpulan**
1. `residual sugar` dengan `total sulfur dioxide` mencapai `50`
2. `residual sugar` dengan `desnity` mencapai `55`
3. `free sulful dioxode` dengan `toal sulfur dioxide` mencapai `72`
4. `alcohol` dengan `desnity` memiliki hubungan negatif `-69` 

## **Data Preparation**
### **Calculate and remove missing values**

| Kolom                 | Jumlah Missing Values |
|-----------------------|----------------------|
| type                  | 0                    |
| fixed acidity         | 10                   |
| volatile acidity      | 8                    |
| citric acid           | 3                    |
| residual sugar        | 2                    |
| chlorides             | 2                    |
| free sulfur dioxide   | 0                    |
| total sulfur dioxide  | 0                    |
| density               | 0                    |
| pH                    | 9                    |
| sulphates             | 4                    |
| alcohol               | 0                    |
| quality               | 0                    |

Karena jumlah missing values sangat sedikit dibanding total data, menghapusnya tidak akan mengurangi informasi secara signifikan. Ini juga lebih sederhana dan menjaga kualitas data agar analisis dan model menjadi lebih akurat. Jadi, penghapusan missing values adalah pilihan yang tepat.


### **Calculate and remove duplicates values**
Setelah pengecekan, ditemukan `1.168` data duplikat. Data ini perlu dihapus agar tidak memengaruhi hasil analisis dan model, karena duplikat dapat menyebabkan bias dan overfitting. Oleh karena itu, penghapusan data duplikat adalah langkah penting untuk menjaga kualitas dataset.

### **Find Multicollinearity**

Multikolinearitas terjadi saat dua fitur sangat berkorelasi, menyebabkan informasi yang tumpang tindih. Hal ini bisa membuat model jadi tidak stabil dan sulit diinterpretasi.

Contoh output deteksi korelasi tinggi:

`Highly correlated feature pairs (>0.7):`

`free sulfur dioxide - total sulfur dioxide: 0.721`

Artinya, fitur free sulfur dioxide dan total sulfur dioxide sangat berkaitan **(korelasi 0.721)**, sehingga salah satunya bisa dihilangkan atau diolah ulang untuk menghindari masalah multikolinearitas.

### **Feature Engineering**

1. Encoding variabel kategorikal:
Variabel type diubah dari teks (white, red) menjadi angka (0, 1) karena komputer hanya bisa memproses data numerik dalam model machine learning.

2. Pembuatan fitur baru:
Beberapa fitur baru dibuat berdasarkan kombinasi dan rasio fitur asli untuk menangkap pola yang lebih kompleks, seperti:

- total_acidity sebagai jumlah dari fixed acidity dan volatile acidity untuk merepresentasikan total keasaman.

- acid_to_sugar_ratio mengukur keseimbangan antara asam dan gula, penting untuk rasa dan karakteristik anggur.

- so2_ratio menunjukkan proporsi sulfur dioksida bebas terhadap total, relevan untuk kualitas dan pengawetan.

- density_alcohol_interaction menangkap interaksi antara kepadatan dan kadar alkohol yang dapat memengaruhi sifat fisik anggur.

Fitur-fitur ini dibuat berdasarkan pemahaman domain untuk memperkaya informasi dan meningkatkan performa model.


### **Calculate and remove outliers**

![boxplto_outiers](https://github.com/user-attachments/assets/e3b49f60-356f-458a-a8ee-9123eaf84f46)


dari boxplot di atas dapat disimpulkan:
- Banyak fitur memiliki outlier yang signifikan, terutama untuk sulfur dioxide (free dan total), residual sugar, dan chlorides.
- Sebagian besar fitur menunjukkan distribusi data yang cukup terkonsentrasi di rentang tertentu, dengan outlier yang cukup jauh dari nilai normal.
- Untuk fitur seperti density, nilai sangat homogen.
- Outlier-outlier ini perlu diperhatikan karena dapat memengaruhi analisis atau pemodelan yang akan dilakukan.

untuk menangani outlier pada data akan digunakan metode IQR. Metode IQR adalah teknik statistik yang digunakan untuk mendeteksi dan menangani outlier pada dataset. IQR mengukur rentang tengah data dengan menghitung selisih antara kuartil ketiga (Q3) dan kuartil pertama (Q1).

**Langkah-langkah metode IQR**
1. Hitung Kuartil Pertama (Q1): Nilai yang memisahkan 25% data terendah.
2. Hitung Kuartil Ketiga (Q3): Nilai yang memisahkan 25% data tertinggi.
3. Hitung IQR:  IQR = Q3 - Q1
4. Tentukan batas bawah dan batas atas:  
 - Batas bawah = Q1 - 1.5 × IQR
 - Batas atas = Q3 + 1.5 × IQR
5. Identifikasi Outlier: Data yang berada di luar rentang antara batas bawah dan batas atas dianggap outlier.

Dengan cara ini, IQR mampu mengidentifikasi data yang jauh dari distribusi normal tanpa asumsi distribusi data tertentu. Menghapus outlier menggunakan metode IQR membantu menjaga kualitas data, mencegah distorsi statistik, dan meningkatkan performa model machine learning dengan fokus pada pola data yang representatif.


### **Remove High Correlation Feature**

- Menghapus fitur berkorelasi tinggi:
  Fitur yang sangat berkorelasi (lebih dari 0.8) dihapus untuk menghindari multikolinearitas, yang dapat membuat model menjadi tidak stabil dan berlebihan dalam belajar pola yang sama berulang kali.

- Pelatihan model Random Forest:  
  Model dilatih dengan fitur yang sudah dikurangi korelasinya untuk menentukan pentingnya masing-masing fitur terhadap prediksi kualitas anggur.  
  Alasan menggunakan Random Forest adalah karena model ini secara otomatis dapat mengukur kontribusi setiap fitur dalam proses prediksi, sehingga memudahkan identifikasi fitur yang paling berpengaruh tanpa perlu analisis manual yang rumit.


- Memilih fitur terpenting:
  Berdasarkan feature_importances_, dipilih 10 fitur teratas yang paling berpengaruh pada model. Langkah ini membantu menyederhanakan model sekaligus menjaga performa.
**Daftar 10 fitur terpenting**

No | Feature              | Importance
---|----------------------|-----------
1  | alcohol              | 0.1145
2  | density              | 0.0981
3  | so2_ratio            | 0.0881
4  | volatile acidity     | 0.0880
5  | total sulfur dioxide | 0.0817
6  | sulphates            | 0.0788
7  | chlorides            | 0.0787
8  | residual sugar       | 0.0768
9  | pH                   | 0.0768
10 | free sulfur dioxide  | 0.0738

Fitur final yang digunakan adalah 10 fitur teratas ini. Dengan memilih fitur ini, model menjadi lebih sederhana, cepat, dan fokus pada variabel yang paling memengaruhi prediksi kualitas anggur tanpa terganggu oleh fitur yang kurang relevan atau redundan.

### **Handling imbalance class**

Distribusi kelas target `quality` tidak seimbang, dimana beberapa kelas memiliki jumlah data sangat sedikit (misal kelas 3 dan 9), sementara kelas lain sangat dominan. Ketidakseimbangan ini dapat menyebabkan model bias terhadap kelas mayoritas dan performa buruk pada kelas minoritas. Untuk menangani ketidak seimbangan ini maka digunakan SMOTE (Synthetic Minority Over-sampling Technique) digunakan untuk membuat data sintetis pada kelas minoritas sehingga distribusi kelas menjadi seimbang. Teknik ini membantu model belajar dengan lebih adil dari semua kelas. setelah penggunaan SMOTE Distribusi kelas menjadi seimbang dengan jumlah sampel yang sama untuk setiap kelas (2032), sehingga model dapat lebih optimal dan tidak bias. Ukuran dataset juga meningkat dari jumlah asli menjadi 14224 data dengan 10 fitur.

**Distribusi Kelas Sebelum dan Sesudah SMOTE**

|**Original**|**Balanced**|
|--------|--------|
|3      13|3    2032|
|4     159 |4    2032|
|5    1456 |5    2032|
|6    2032 |6    2032 |
|7     784 |7    2032 | 
|8     136 |8    2032 |
|9       5 |9    2032 |

Dataset shape after SMOTE: (14224, 10)


### **Data Splitting**
Data splitting dilakukan agar model dapat belajar pola dari data training dan dievaluasi dengan data testing yang benar-benar baru, sehingga performa model menjadi lebih valid dan tidak bias.

Data splitting dilakukan sebelum penanganan skew dan standardisasi karena agar informasi dari data testing tidak “bocor” ke proses training (data leakage). Jika transformasi dilakukan sebelum split, parameter seperti mean dan standar deviasi dihitung dari seluruh data, termasuk data testing, sehingga evaluasi model tidak akurat.

Dengan melakukan split terlebih dahulu, transformasi seperti log transform dan standardisasi hanya dihitung dari data training dan kemudian diterapkan ke data testing, sehingga model diuji dengan data yang benar-benar baru dan hasil evaluasi lebih dapat dipercaya.


### Feature Scaling
Fitur memiliki skala dan satuan yang berbeda-beda, yang dapat mempengaruhi performa model terutama algoritma berbasis jarak seperti KNN, SVM, atau Gradient Boosting. Scaling memastikan setiap fitur memiliki kontribusi yang seimbang dalam pembelajaran model. StandardScaler melakukan standarisasi fitur dengan mengubah nilai setiap fitur agar memiliki rata-rata 0 dan standar deviasi 1. Scaler dilatih pada data pelatihan (`fit_transform`), kemudian digunakan untuk mentransformasi data uji (`transform`) agar konsisten. Setelah itu, data hasil scaling dikonversi kembali ke DataFrame agar lebih mudah dikelola.

Dengan langkah ini, model dapat belajar lebih efektif tanpa bias dari perbedaan skala fitur.

## **Modeling**
### **Modelling and Hyperparameter Tuning**

Pada tahap pemodelan, digunakan lima algoritma klasifikasi populer: Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), XGBoost, dan Gradient Boosting. Masing-masing model dilatih dan dievaluasi dengan menggunakan **Randomized Search** untuk mencari kombinasi hyperparameter terbaik secara efisien.

Setiap model memiliki beberapa hyperparameter utama yang di-tuning, misalnya jumlah estimator (`n_estimators`), kedalaman pohon (`max_depth`), laju pembelajaran (`learning_rate`), dan parameter spesifik seperti `C` dan `gamma` pada SVM atau `n_neighbors` pada KNN. Pemilihan rentang parameter didasarkan pada praktik terbaik dan karakteristik masing-masing algoritma.

### **Pros and Const Model**

- **Random Forest**  
  `Pro`: Robust terhadap overfitting, mudah diinterpretasi dengan feature importance.  
  `Contra`: Bisa lambat untuk dataset sangat besar dan kurang efektif untuk data sangat imbalanced tanpa penanganan khusus.  
  `Cara Kerja`: Membangun banyak pohon keputusan (decision trees) secara acak pada subset data dan fitur berbeda (bagging). Prediksi akhir didasarkan pada voting mayoritas dari semua pohon untuk klasifikasi.

- **Support Vector Machine (SVM)**  
  `Pro`: Efektif pada dataset berdimensi tinggi dan mampu menangani non-linearitas dengan kernel.  
  `Contra`: Sensitif terhadap pemilihan hyperparameter dan bisa lambat pada dataset besar.  
  `Cara Kerja`: Mencari hyperplane optimal yang memisahkan kelas dengan margin terluas, dan menggunakan fungsi kernel untuk mengubah data menjadi ruang berdimensi lebih tinggi agar kelas dapat dipisahkan secara linear.

- **K-Nearest Neighbors (KNN)**  
  `Pro`: Sederhana dan mudah diimplementasikan, bagus untuk data dengan pola lokal.  
  `Contra`: Performa menurun pada dimensi tinggi dan data besar, serta sensitif terhadap skala fitur.  
  `Cara Kerja`: Mengklasifikasikan data baru berdasarkan mayoritas label dari k tetangga terdekatnya menurut jarak tertentu (misal Euclidean distance).

- **XGBoost**  
  `Pro`: Sangat powerful, menggabungkan boosting dengan regularisasi sehingga meminimalisir overfitting.  
  `Contra`: Perlu tuning hyperparameter yang cermat dan lebih kompleks.  
  `Cara Kerja`: Menggunakan metode boosting gradient dimana model dibangun secara berurutan, setiap model baru memperbaiki kesalahan model sebelumnya dengan menambahkan pohon keputusan yang meminimalkan loss function dan regularisasi.

- **Gradient Boosting**  
  `Pro`: Baik untuk data dengan hubungan non-linear dan mampu menghasilkan prediksi akurat.  
  `Contra`: Lebih lambat dibanding Random Forest dan rentan overfitting jika tidak diatur dengan baik.  
  `Cara Kerja`: Mirip XGBoost, membangun model secara bertahap dengan menambahkan pohon keputusan yang mengoreksi kesalahan residual model sebelumnya melalui optimasi fungsi loss.


Untuk setiap model, dilakukan hyperparameter tuning menggunakan **Randomized Search**, yang memungkinkan eksplorasi lebih luas dan efisien dibanding grid search. Proses ini meningkatkan performa model dengan menemukan kombinasi parameter terbaik sesuai data.

1. **Random Forest:**

- n_estimators: jumlah pohon dalam hutan, diuji pada rentang 100 hingga 200 pohon.

- max_depth: kedalaman maksimum pohon, diuji pada nilai 10 dan tanpa batasan (None).

- min_samples_split: jumlah minimum sampel yang dibutuhkan untuk membagi sebuah node, diuji pada nilai 2 dan 5.

- min_samples_leaf: jumlah minimum sampel pada daun pohon, diuji pada nilai 1 dan 2.

- max_features: jumlah fitur yang dipertimbangkan saat mencari split terbaik, menggunakan metode 'sqrt'.

2. **Support Vector Machine (SVM):**

- C: parameter regularisasi, diuji pada nilai 1 dan 10.

- kernel: fungsi kernel yang digunakan, memakai kernel radial basis function ('rbf').

- gamma: parameter kernel, diuji pada opsi 'scale' dan 0.01.

3. **K-Nearest Neighbors (KNN):**

- n_neighbors: jumlah tetangga terdekat yang dipertimbangkan, diuji pada nilai 5 dan 9.

- weights: metode pemberian bobot pada tetangga, menggunakan 'uniform' (bobot sama).

- metric: metrik jarak yang digunakan, menggunakan jarak Euclidean.

4. **XGBoost:**

- n_estimators: jumlah pohon boosting, diuji pada 100 dan 200 pohon.

- max_depth: kedalaman maksimum tiap pohon, diuji pada nilai 3 dan 6.

- learning_rate: laju pembelajaran, menggunakan nilai 0.1.

- subsample: proporsi sampel yang digunakan setiap iterasi, menggunakan nilai 0.9.

- colsample_bytree: proporsi fitur yang dipakai untuk membangun tiap pohon, menggunakan nilai 0.9.

5. **Gradient Boosting:**

- n_estimators: jumlah pohon boosting, diuji pada 100 dan 200 pohon.

- max_depth: kedalaman maksimum tiap pohon, diuji pada nilai 3 dan 5.

- learning_rate: laju pembelajaran, menggunakan nilai 0.1.

- subsample: proporsi sampel yang digunakan setiap iterasi, menggunakan nilai 0.9.


## **Evaluation**

Dalam membandingkan performa model machine learning untuk klasifikasi kualitas anggur, digunakan beberapa metrik evaluasi berikut:

- **Test Accuracy**  
  Mengukur persentase prediksi yang benar pada data uji yang belum pernah dilihat model. Akurasi memberikan gambaran umum tentang seberapa baik model bekerja secara keseluruhan.

- **F1 Score**  
  Menggabungkan precision dan recall dalam satu nilai harmonis, terutama penting bila data tidak seimbang (imbalance). F1 Score memastikan model tidak hanya akurat secara keseluruhan, tetapi juga efektif dalam menangkap kelas minoritas dan menghindari false positive.

- **Cross-Validation Mean Accuracy**  
  Memberikan estimasi performa model yang lebih stabil dan generalisasi yang lebih baik dengan menguji model pada beberapa subset data (fold). Ini membantu menghindari overfitting dan memberikan gambaran yang lebih realistis mengenai performa model pada data baru.

- **Cross-Validation Standard Deviation**  
  Menunjukkan variasi performa model pada setiap fold cross-validation. Nilai yang kecil menandakan model yang konsisten dan stabil di berbagai pembagian data, sedangkan nilai besar bisa mengindikasikan ketidakstabilan atau sensitivitas model terhadap data tertentu.

Penggunaan keempat metrik ini bersama-sama memberikan evaluasi yang komprehensif: akurasi dan keseimbangan klasifikasi, serta kestabilan dan kemampuan generalisasi model.

##

| Model              | Test Accuracy | F1 Score | CV Mean Accuracy | CV Std Dev |
|--------------------|---------------|----------|------------------|------------|
| Random Forest      | 0.8569        | 0.8518   | 0.8408           | 0.0052     |
| XGBoost            | 0.8401        | 0.8359   | 0.8354           | 0.0027     |
| Gradient Boosting   | 0.8397        | 0.8375   | 0.8265           | 0.0022     |
| SVM                | 0.7880        | 0.7798   | 0.7710           | 0.0065     |
| KNN                | 0.7831        | 0.7653   | 0.7677           | 0.0049     |

## Model Terbaik
Model terbaik adalah **Random Forest** karena:
- Memiliki akurasi uji tertinggi (85.69%)
- F1 Score terbaik (0.8518), menunjukkan keseimbangan antara precision dan recall
- Cross-validation menunjukkan hasil yang stabil dengan standar deviasi kecil (0.0052)

## Penjelasan Metrik Evaluasi

### Accuracy
Persentase prediksi yang benar dari keseluruhan data.

Accuracy dihitung dengan rumus:
![Rumus akurasi](https://miro.medium.com/v2/resize:fit:1400/1*yUvmDn0nlVdS5BR10TRdKg.png)
### F1 Score
Harmonik rata-rata dari precision dan recall, mengukur keseimbangan antara keduanya.

![F1 Score Rumus](https://miro.medium.com/v2/resize:fit:1400/1*GFFeaVMjM4z7P5KpEGPOiw.png)

### Cross-Validation Mean Accuracy
Rata-rata akurasi yang didapat dari beberapa kali pembagian data secara bergantian untuk menguji stabilitas model.

### Cross-Validation Standard Deviation
Ukuran variasi akurasi dari hasil cross-validation, nilai kecil menunjukkan model yang konsisten.

## Cara Kerja Model Random Forest (Singkat)
Random Forest membangun banyak pohon keputusan (decision trees) secara acak pada subset data dan fitur yang berbeda (bagging). Prediksi akhir ditentukan berdasarkan voting mayoritas dari semua pohon tersebut. Metode ini mengurangi risiko overfitting dan meningkatkan akurasi prediksi.



---
# **Referensi**
1. *Vilela, A., Marques, C., & Correia, E. (2018). Structural Equation Modelling (SEM) applied to sensory profile of Vinho Verde monovarietal wines.. Food research international, 111, 650-660 . https://doi.org/10.1016/j.foodres.2018.05.077.*
2. *Oliveira, J., Araújo, I., Pereira, O., Maia, J., Amaral, A., & Maia, M. (2004). Characterization and differentiation of five “vinhos verdes” grape varieties on the basis of monoterpenic compounds. Analytica Chimica Acta, 513, 269-275. https://doi.org/10.1016/J.ACA.2003.10.020*.
3. *Stanco, M., Lerro, M., & Marotta, G. (2020). Consumers’ Preferences for Wine Attributes: A Best-Worst Scaling Analysis. Sustainability. https://doi.org/10.3390/su12072819.*
4. *Capitello, R., Agnoli, L., Charters, S., & Begalli, D. (2021). Labelling environmental and terroir attributes: Young Italian consumers’ wine preferences. Journal of Cleaner Production. https://doi.org/10.1016/J.JCLEPRO.2021.126991.*
5. *Agnoli, L., Charters, S., Marks, D., & Tavilla, V. (2023). Old world assessment of new world provenance cues: An Italian perspective. International Journal of Market Research, 65, 708 - 725. https://doi.org/10.1177/14707853231202759.*
6. *Dhaliwal, P., Sharma, S., & Chauhan, L. (2022). Detailed Study of Wine Dataset and its Optimization. International Journal of Intelligent Systems and Applications. https://doi.org/10.5815/ijisa.2022.05.04.*
7. *Adithya, A. (2024). Wine Quality Detection Using Machine Learning: A Comparative Analysis of Classification Algorithms. INTERANTIONAL JOURNAL OF SCIENTIFIC RESEARCH IN ENGINEERING AND MANAGEMENT. https://doi.org/10.55041/ijsrem40168.*
8. *Talwandi, N., Khare, S., & Yadav, A. (2024). SipSmart: Elevating Palates with Machine Learning for Wine Quality Prediction. 2024 International Conference on Emerging Smart Computing and Informatics (ESCI), 1-5. https://doi.org/10.1109/ESCI59607.2024.10497300.*
9. *Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. Decis. Support Syst., 47, 547-553. https://doi.org/10.1016/j.dss.2009.05.016.*
10. *Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Wine Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C56S3T.*
