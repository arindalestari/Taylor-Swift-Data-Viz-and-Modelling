# Taylor-Swift-Data-Viz-and-Modelling

Halo! 

Ini adalah mini project yang arinda buat untuk memprediksi tingkat popularitas pada lagu Taylor Swift.
Sebagai salah satu pendengar Taylor Swift sejak 2013, menurut saya akan menyenangkan melakukan proyek ilmu data dan pembelajaran mesin menggunakan kumpulan data lagu adalah tantangan yang sangat menarik. Saya senang mengerjakan mini project ini dengan mencoba beberapa model machine learning dan membandingkan performanya.

# Proses Analisa

Proses yang dikerjakan dalam project ini meliputi:
1. Instalasi Package yang dibutuhkan
2. Eksplorasi Data Analisis (preprocessing data dan visualisasi)
3. Teknik Fitur (Feature Engineering)
4. Evaluasi Model
5. Menyelidiki model yang paling baik untuk ditingkatkan secara lebih detail
6. Klasterisasi dengan K-Means

Model yang digunakan untuk melihat performa terbaik dengan hasil sebagai berikut:
![Tabel Perbandingan Performa Model Regresi](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/newplot%20(1).png)

Model dengan Performa Terbaik: **Gradient Boosting Descent** menunjukkan performa terbaik dengan MSE dan RMSE terendah serta R kuadrat tertinggi sehingga, saya gunakan model tersebut untuk memprediksi popularitas lagu Taylor Swift.
# Insight

1. Berdasarkan grafik visualisasi berikut, yang menempati urutan pertama pada 10 album berdasarkan tingkat popularitas adalah album The Tortured Poets Department (TTPD), untuk lagu yang menempati urutan pertama berdasarkan tingkat popularitas lagu dengan judul "fortnight".
![Diagram Batang](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Top%20Album.png)

![Diagram batang2](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Top%20Song.png)

2. Berikut merupakan plot klasterisasi antara valence dan energy
![Plot Klasterisasi](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Klasterisasi.png)

Dengan mengamati posisi titik-titik dalam scatter plot, kamu bisa melihat karakteristik umum dari setiap cluster:

* Cluster 0: Jika titik-titik dalam cluster ini cenderung berada di bagian kanan atas scatter plot, berarti cluster ini terdiri dari lagu-lagu dengan valence dan energy tinggi (lagu-lagu yang ceria dan berenergi).
* Cluster 1: Jika titik-titik dalam cluster ini berada di tengah, ini berarti cluster ini mungkin terdiri dari lagu-lagu dengan valence dan energy sedang (balance lah ya istilahnya).
* Cluster 2: Jika titik-titik dalam cluster ini berada di kiri bawah, ini berarti cluster ini terdiri dari lagu-lagu dengan valence dan energy rendah (lagu-lagu yang lebih sedih dan rendah energi).

3. Prediksi model gradient boosting 
Didapatkan hasil prediksi tingkat popularitas lagu Taylor Swift setelah dilatih data baru:

Mean Absolute Error: 5.627018846545834

Prediksi Popularitas: 80.34223731942195

Dari output diatas, rata-rata kesalahan prediksi model terhadap popularitas lagu Taylor Swift adalah sekitar 5.63 (dalam skala yang sesuai dengan popularitas lagu tersebut)dan prediksi popularitas lagu Taylor Swift yang diberikan pada model gradient boosting adalah 80.34 untuk tanggal 1 Juli 2024 dari skala ukuran popularitas berdasarkan data yaitu 0-100.

Analisis residual digunakan untuk melihat distribusi residual (perbedaan antara nilai aktual dan nilai yang diprediksi) dapat memberikan wawasan tentang kinerja model dengan plot berikut:

![plot 1](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/plot%20residual%20lonceng.png)

![plot 2](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/scatter%20plot.png)

* Distribusi residual yang normal (berbentuk lonceng) menunjukkan bahwa model memiliki error yang terdistribusi dengan baik.
* Ketika kita membuat plot prediksi vs nilai sebenarnya, garis y = x digambarkan sebagai garis merah putus-putus. Titik data (scatter plot) diatas yang berada dekat dengan garis merah menunjukkan bahwa nilai yang diprediksi oleh model hampir sama dengan nilai sebenarnya.
* Dalam konteks evaluasi model regresi, tujuan adalah agar titik-titik data sebanyak mungkin berada dekat dengan garis merah, menunjukkan bahwa model mampu memprediksi nilai dengan akurat.

# Apa yang harus diimprove pada mini project ini?

1. Detail pada hasil analisa Nilai MAE dan Nilai MAE setelah dilakukan teknik validasi silang hasilnya dapat dikatakan overfitting. Mengapa demikian? dikarenakan hasil antara MAE prediksi awal didapatkan 5.63 dan hasil dari MAE setelah dilakukan Cross-Validation 11.72 terdapat perbedaan yang sangat signifikan.
2. Prediksi popularitas lagu mungkin tidak dapat diandalkan sepenuhnya karena model menunjukan tanda-tanda overfitting sehingga, model perlu ditinjau ulang setelah model diperbaiki untuk mengurangi overfitting.
3. Lakukan hyperparameter tuning dengan teknik grid search atau random search.
4. Mencoba teknik regularization.
5. Mencoba pendekatan ensemble lain untuk peningkatan kinerja model.

  Untuk detail project lebih lanjut silahkan klik atau download file yang berformat .ipynb

  Semoga dengan adanya mini project ini bermanfaat untuk pemahaman penerapan machile learning pada dunia nyata. Sampai jumpa di mini project saya selanjutnya.
