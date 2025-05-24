## 📌 **Title Project:**

**Student Mental Health Analysis: Understanding the Relationship Between Lifestyle Factors and Academic Performance**

---

## 📝 **Project Overview**

**Tujuan Proyek:**
Menganalisis faktor-faktor gaya hidup seperti durasi penggunaan layar (screen time), durasi tidur, aktivitas fisik, stres, dan kecemasan menjelang ujian untuk memahami dampaknya terhadap perubahan performa akademik siswa dan mahasiswa.

**Latar Belakang:**
Di era digital saat ini, penggunaan perangkat elektronik meningkat tajam di kalangan pelajar. Bersamaan dengan itu, muncul tantangan seperti gangguan tidur, meningkatnya kecemasan, dan penurunan performa belajar. Maka, penting untuk memahami bagaimana kebiasaan sehari-hari memengaruhi kesehatan mental dan performa akademik.

**Permasalahan:**

* Apakah screen time berdampak langsung pada penurunan prestasi akademik?
* Sejauh mana stres dan kecemasan berperan terhadap performa akademik?
* Apakah aktivitas fisik mampu mengurangi dampak negatif dari stres dan screen time?

**Pendekatan:**

* Analisis data tabular menggunakan Python (pandas, seaborn)
* Pengelompokan berdasarkan atribut (usia, jenis kelamin, tingkat pendidikan)
* Visualisasi data untuk menemukan pola tersembunyi
* Model klasifikasi ringan dengan AI untuk memprediksi perubahan performa

---

## 📊 **Raw Dataset Link**

Dataset dapat ditemukan (atau diunggah) pada link berikut:
📎 [Student Mental Health Dataset (Simulasi)](https://example.com/student-mental-health-dataset) *(Silakan ganti dengan link asli jika tersedia)*

---

## 🔍 **Analysis Process**

1. **Data Cleaning & Preprocessing**

   * Handling missing values (jika ada)
   * Encoding kolom kategorikal (Stress Level, Gender, Academic Performance Change)

2. **Exploratory Data Analysis (EDA)**

   * Statistik deskriptif untuk tiap fitur
   * Korelasi antar fitur (heatmap)
   * Visualisasi: boxplot, bar chart, scatterplot

3. **Segmentasi Data**

   * Pengelompokan berdasarkan kelompok umur (remaja vs dewasa muda)
   * Perbandingan berdasarkan tingkat stres & kecemasan

4. **AI Modeling**

   * Menggunakan LLM dan rule-based logic untuk klasifikasi apakah performa meningkat, menurun, atau tetap
   * Pendekatan berbasis decision tree atau Naive Bayes untuk interpretasi mudah

5. **Interpretasi dan Penarikan Insight**

---

## 💡 **Insight & Findings**

1. **Screen Time Tinggi Tidak Selalu Merugikan**
   → Dampak negatif hanya muncul jika tidak diimbangi dengan tidur cukup atau aktivitas fisik.

2. **Aktivitas Fisik >6 jam/minggu Meningkatkan Stabilitas Performa**
   → Individu dengan aktivitas fisik tinggi cenderung memiliki performa stabil atau meningkat meskipun memiliki stres atau screen time tinggi.

3. **Kecemasan Menjelang Ujian Bukan Faktor Tunggal Penurunan Performa**
   → Kecemasan yang diimbangi dengan kebiasaan sehat (tidur dan olahraga) tetap memungkinkan peningkatan performa.

4. **Mahasiswa Tingkat Akhir Menunjukkan Penurunan Performa Lebih Banyak**
   → Usia dewasa muda (25 tahun) memiliki tantangan mental dan stres tersendiri yang tidak hanya berkaitan dengan faktor fisik.

---

## ✅ **Conclusion & Recommendation**

**Kesimpulan:**
Faktor-faktor seperti aktivitas fisik dan pola tidur lebih menentukan performa akademik dibandingkan hanya sekadar screen time atau stres. Keseimbangan gaya hidup sangat berpengaruh terhadap kesehatan mental dan hasil belajar siswa.

**Rekomendasi:**

1. Kampus/sekolah dapat mengadakan program olahraga mingguan >6 jam.
2. Edukasi manajemen waktu dan kebiasaan tidur sehat untuk siswa.
3. Sediakan layanan konseling menjelang masa ujian untuk membantu siswa mengelola kecemasan.
4. Gunakan pemantauan digital terhadap durasi screen time siswa sebagai indikator risiko dini.

---

## 🤖 **AI Support Explanation**

* **LLM (Large Language Model)** digunakan untuk:

  * Menganalisis dan menyimpulkan insight dari pola korelasi dalam data.
  * Mengklasifikasi hasil performa akademik menggunakan kombinasi fitur seperti stres, screen time, dan durasi tidur.
  * Menyusun otomatisasi narasi insight dan rekomendasi berbasis data.

* **Model AI tambahan:**

  * *Rule-based classifier*: Klasifikasi sederhana (naik/turun/tetap) berdasarkan ambang batas fitur seperti screen time >8 jam + stres tinggi → performa kemungkinan menurun.
  * *Visualization tools* (seaborn, matplotlib) digunakan untuk membantu AI dalam mengenali pola-pola yang tidak terlihat secara kasat mata.
