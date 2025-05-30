
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





---

1. *Vilela, A., Marques, C., & Correia, E. (2018). Structural Equation Modelling (SEM) applied to sensory profile of Vinho Verde monovarietal wines.. Food research international, 111, 650-660 . https://doi.org/10.1016/j.foodres.2018.05.077.*
2. *Oliveira, J., Araújo, I., Pereira, O., Maia, J., Amaral, A., & Maia, M. (2004). Characterization and differentiation of five “vinhos verdes” grape varieties on the basis of monoterpenic compounds. Analytica Chimica Acta, 513, 269-275. https://doi.org/10.1016/J.ACA.2003.10.020*.
3. *Stanco, M., Lerro, M., & Marotta, G. (2020). Consumers’ Preferences for Wine Attributes: A Best-Worst Scaling Analysis. Sustainability. https://doi.org/10.3390/su12072819.*
4. *Capitello, R., Agnoli, L., Charters, S., & Begalli, D. (2021). Labelling environmental and terroir attributes: Young Italian consumers’ wine preferences. Journal of Cleaner Production. https://doi.org/10.1016/J.JCLEPRO.2021.126991.*
5. *Agnoli, L., Charters, S., Marks, D., & Tavilla, V. (2023). Old world assessment of new world provenance cues: An Italian perspective. International Journal of Market Research, 65, 708 - 725. https://doi.org/10.1177/14707853231202759.*
6. *Dhaliwal, P., Sharma, S., & Chauhan, L. (2022). Detailed Study of Wine Dataset and its Optimization. International Journal of Intelligent Systems and Applications. https://doi.org/10.5815/ijisa.2022.05.04.*
7. *Adithya, A. (2024). Wine Quality Detection Using Machine Learning: A Comparative Analysis of Classification Algorithms. INTERANTIONAL JOURNAL OF SCIENTIFIC RESEARCH IN ENGINEERING AND MANAGEMENT. https://doi.org/10.55041/ijsrem40168.*
8. *Talwandi, N., Khare, S., & Yadav, A. (2024). SipSmart: Elevating Palates with Machine Learning for Wine Quality Prediction. 2024 International Conference on Emerging Smart Computing and Informatics (ESCI), 1-5. https://doi.org/10.1109/ESCI59607.2024.10497300.*
9. *Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. Decis. Support Syst., 47, 547-553. https://doi.org/10.1016/j.dss.2009.05.016.*
