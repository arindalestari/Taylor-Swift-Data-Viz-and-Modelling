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

# Insight

Berdasarkan grafik visualisasi berikut, yang menempati urutan pertama pada 10 album berdasarkan tingkat popularitas adalah album The Tortured Poets Department (TTPD), untuk lagu yang menempati urutan pertama berdasarkan tingkat popularitas lagu dengan judul "fortnight".
![Diagram Batang](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Top%20Album.png)

![Diagram batang2](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Top%20Song.png)

Berikut merupakan plot klasterisasi antara valencedan energy
![Plot Klasterisasi](https://github.com/arindalestari/Taylor-Swift-Data-Viz-and-Modelling/blob/main/Klasterisasi.png)

Dengan mengamati posisi titik-titik dalam scatter plot, kamu bisa melihat karakteristik umum dari setiap cluster:

* Cluster 0: Jika titik-titik dalam cluster ini cenderung berada di bagian kanan atas scatter plot, berarti cluster ini terdiri dari lagu-lagu dengan valence dan energy tinggi (lagu-lagu yang ceria dan berenergi).
* Cluster 1: Jika titik-titik dalam cluster ini berada di tengah, ini berarti cluster ini mungkin terdiri dari lagu-lagu dengan valence dan energy sedang (balance lah ya istilahnya).
* Cluster 2: Jika titik-titik dalam cluster ini berada di kiri bawah, ini berarti cluster ini terdiri dari lagu-lagu dengan valence dan energy rendah (lagu-lagu yang lebih sedih dan rendah energi).

