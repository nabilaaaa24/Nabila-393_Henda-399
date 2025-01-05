# Analisis Popularitas Lagu Berdasarkan Fitur Audio
Dataset yang digunakan : https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-01-21/readme.md
## Gambaran Proyek
Proyek ini mengeksplorasi dataset musik untuk mengidentifikasi hubungan antara popularitas lagu dengan berbagai fitur audio. Dengan analisis ini, bertujuan untuk memahami fitur mana yang paling berpengaruh dalam meningkatkan popularitas lagu dan memberikan wawasan yang dapat membantu industri musik atau platform streaming.
 Informasi ini dapat digunakan untuk:
- Mengidentifikasi genre dengan durasi rata-rata lagu terpanjang.
- Memberikan wawasan kepada industri musik tentang preferensi durasi pada genre tertentu.
- Membantu penyanyi, produser, atau platform streaming untuk menyesuaikan durasi lagu sesuai dengan tren genre.

## Wawasan Utama
1. **Fitur yang Paling Berpengaruh**:
   - **Acousticness** memiliki korelasi positif tertinggi terhadap popularitas lagu (0.085).
   - **Danceability** dan **Loudness** juga memiliki korelasi positif, meskipun tidak terlalu signifikan.
2. **Fitur dengan Pengaruh Negatif**:
   - **Instrumentalness** menunjukkan korelasi negatif tertinggi (-0.150), diikuti oleh **Duration** dalam bentuk milidetik dan menit (-0.144).
   - **Energy** juga memiliki pengaruh negatif terhadap popularitas (-0.109).
3. **Fitur yang Kurang Berpengaruh**:
   - **Mode**, **Speechiness**, **Key**, dan **Tempo** menunjukkan korelasi yang sangat kecil atau mendekati nol, menunjukkan bahwa fitur ini tidak memiliki dampak signifikan terhadap popularitas lagu.

## Metodologi
1. **Impor dan Pembersihan Data**:
   - Data diperiksa untuk nilai hilang dan outlier.
   - Kolom dengan nama yang redundan (seperti `duration_ms` dan `duration_min`) digabungkan untuk menghindari duplikasi.
2. **Analisis Data Eksploratif (EDA)**:
   - Korelasi antar fitur dihitung untuk memahami hubungan dengan popularitas lagu.
   - Visualisasi seperti scatter plot dan heatmap digunakan untuk mengidentifikasi pola.
3. **Wawasan dari Korelasi**:
   - Korelasi dihitung antara fitur audio dengan `track_popularity`.

## Hasil Analisis
Berikut adalah korelasi fitur audio terhadap popularitas lagu:
| Fitur             | Korelasi  |
|--------------------|-----------|
| Track Popularity   | 1.000     |
| Acousticness       | 0.085     |
| Danceability       | 0.065     |
| Loudness           | 0.058     |
| Valence            | 0.033     |
| Mode               | 0.011     |
| Speechiness        | 0.007     |
| Key                | -0.001    |
| Tempo              | -0.005    |
| Liveness           | -0.055    |
| Energy             | -0.109    |
| Duration (ms/min)  | -0.144    |
| Instrumentalness   | -0.150    |
![image](https://github.com/user-attachments/assets/996bef88-8092-4c45-8bc2-5cf8acfc307d)

## Rekomendasi
1. **Fokus pada Fitur Positif**:
   - Tingkatkan **Acousticness**, **Danceability**, dan **Loudness** untuk meningkatkan popularitas lagu.
2. **Pertimbangan Negatif**:
   - Hindari membuat lagu yang terlalu panjang atau dengan instrumental tinggi, karena fitur ini memiliki pengaruh negatif.
3. **Eksperimen Lanjutan**:
   - Lakukan eksperimen dengan meningkatkan **Valence** untuk melihat apakah ada efek jangka panjang pada popularitas lagu.

## Arah Pengembangan Selanjutnya
- Menyelidiki bagaimana kombinasi fitur audio memengaruhi popularitas.
- Mengembangkan model prediktif untuk memprediksi popularitas lagu berdasarkan fitur audio.
- Mengidentifikasi subgrup dalam genre untuk analisis yang lebih mendalam.

## File dalam Repositori
- **README.md**: Dokumen ini, memberikan gambaran umum tentang proyek.
- **music_analysis.ipynb**: Notebook Google colab yang berisi analisis lengkap, mulai dari pembersihan data hingga visualisasi dan interpretasi hasil.
https://colab.research.google.com/drive/1gb9BKosdgKoKscnfM-4Lt5LmjB32Nx-o?usp=sharing
## Kesimpulan
Proyek ini bertujuan untuk membantu pemangku kepentingan dalam industri musik memahami karakteristik lagu yang populer dan memberikan wawasan yang actionable.

## Authors
1. Henda Cantika Sari - (hendacantika23@gmail.com - 202110370311399)
2. Nabila Az-Zahro Ika P. R. (nabilazahro24@webmail.umm.ac.id- 202110370311393)
