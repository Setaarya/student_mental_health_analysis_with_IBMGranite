## 📌 **Title Project:**

# **Student Mental Health Analysis: Understanding the Relationship Between Lifestyle Factors and Academic Performance**

---

## 📝 **Project Overview**

**Tujuan Proyek:**
Menganalisis korelasi dan pengaruh faktor-faktor gaya hidup utama (screen time, durasi tidur, dan aktivitas fisik) terhadap perubahan performa akademik dan tingkat stres siswa serta mahasiswa. Proyek ini bertujuan untuk mengidentifikasi pola-pola signifikan yang dapat membantu dalam pengembangan strategi peningkatan kesehatan mental dan performa akademik melalui analisis data berbasis AI.

**Latar Belakang:**
Kesehatan mental siswa dan mahasiswa menjadi isu krusial dalam sistem pendidikan modern, terutama selama era pembelajaran daring yang telah mengubah lanskap pendidikan secara fundamental. Pandemi dan transisi ke pembelajaran online telah menciptakan tantangan baru yang kompleks, mulai dari meningkatnya screen time, perubahan pola tidur, hingga berkurangnya aktivitas fisik yang berdampak signifikan pada kesehatan mental dan performa akademik.
Dataset yang digunakan dalam proyek ini adalah Student Mental Health Dataset dari Kaggle yang berisi tanggapan dari 1.000 siswa mengenai kondisi kesehatan mental mereka selama era pembelajaran daring. Data dikumpulkan melalui survei komprehensif yang berfokus pada berbagai aspek psikologis serta perilaku yang dipengaruhi oleh pendidikan jarak jauh, memberikan gambaran nyata tentang dampak pembelajaran online terhadap wellbeing siswa.
Dengan memanfaatkan teknologi AI dan machine learning, khususnya model IBM Granite sebagai large language model generatif, proyek ini berusaha mengungkap hubungan kompleks antara gaya hidup dan performa akademik melalui pendekatan analisis data yang komprehensif.

**Permasalahan:**

* Bagaimana pengaruh durasi screen time terhadap tingkat stres dan performa akademik siswa selama pembelajaran daring, serta apakah terdapat ambang optimal screen time yang mampu menyeimbangkan kesehatan mental dan hasil belajar?
* Sejauh mana durasi tidur memengaruhi performa akademik dan tingkat stres siswa selama pembelajaran daring, serta apakah terdapat durasi tidur optimal yang dapat berperan sebagai faktor protektif bagi kesejahteraan akademik?
* Sejauh mana aktivitas fisik berperan sebagai faktor mitigasi terhadap peningkatan stres dan penurunan performa akademik akibat gaya hidup tidak sehat selama pembelajaran daring, seperti screen time berlebih dan kurang tidur?
* Bagaimana pengembangan model prediksi berbasis AI dapat mengintegrasikan interaksi antara screen time, durasi tidur, dan aktivitas fisik untuk mengidentifikasi siswa berisiko tinggi terhadap stres tinggi dan penurunan performa akademik, serta merekomendasikan kombinasi gaya hidup optimal sebagai intervensi preventif?

**Pendekatan:**

1. Analisis Korelasi Menggunakan IBM Granite AI
   
     Pemanfaatan IBM Granite Large Language Model untuk analisis mendalam hubungan antara:
  
    * Screen Time (hrs/day) dengan Stress Level dan Academic Performance Change
    * Sleep Duration (hrs) dengan Stress Level dan Academic Performance Change
    * Physical Activity (hrs/week) dengan Stress Level dan Academic Performance Change

3. Model Prediksi Personal Berbasis IBM Granite
   
    Pengembangan predictive model menggunakan IBM Granite AI untuk:

    * Memprediksi Academic Performance Change berdasarkan kombinasi lifestyle factors individual
    * Risk assessment berbasis AI untuk mengidentifikasi probabilitas academic decline

---

## 📊 **Raw Dataset Link**

Dataset dapat ditemukan pada link berikut:

📎 [Student Mental Health Dataset](https://www.kaggle.com/datasets/utkarshsharma11r/student-mental-health-analysis)

Dataset ini berisi tanggapan dari 1.000 siswa mengenai kondisi kesehatan mental mereka selama era pembelajaran daring. Data dikumpulkan melalui survei dan berfokus pada berbagai aspek psikologis serta perilaku yang dipengaruhi oleh pendidikan jarak jauh.

Dataset terdiri dari 10 kolom, yang mencakup informasi demografis, kebiasaan gaya hidup, serta indikator kesehatan mental yang dilaporkan sendiri. Berikut ringkasan kolomnya:

| Kolom                            | Deskripsi                                                            |
| -------------------------------- | -------------------------------------------------------------------- |
| **Name**                         | Nama depan siswa (tidak penting untuk analisis, dapat dianonimkan)   |
| **Gender**                       | Jenis kelamin responden (Laki-laki/Perempuan)                        |
| **Age**                          | Usia responden dalam tahun                                           |
| **Education Level**              | Jenjang pendidikan (misal: Kelas 8, BTech, MSc)                      |
| **Screen Time (hrs/day)**        | Rata-rata waktu layar per hari selama pembelajaran daring            |
| **Sleep Duration (hrs)**         | Rata-rata durasi tidur harian                                        |
| **Physical Activity (hrs/week)** | Durasi olahraga/mobilitas fisik per minggu                           |
| **Stress Level**                 | Tingkat stres yang dirasakan (Rendah, Sedang, Tinggi)                |
| **Anxious Before Exams**         | Apakah siswa merasa cemas sebelum ujian (Ya/Tidak)                   |
| **Academic Performance Change**  | Perubahan kinerja akademik yang dirasakan (Meningkat, Sama, Menurun) |

---

## 🔍 **Analysis Process**

1. **Exploratory Data Analysis (EDA)**

   * Penghapusan Kolom yang Tidak Relevan
      - Kolom ‘Name’ tidak memiliki kontribusi dalam proses analisis atau pemodelan karena hanya berisi nama depan siswa. Penghapusan dilakukan untuk menjaga privasi data dan          menghilangkan atribut non-informatif yang tidak relevan terhadap outcome analisis.
        
   * Pengacakan Data dan Pengambilan Sampel
      - Mengacak urutan data secara acak namun tetap konsisten (dengan random_state=42) untuk menghindari bias urutan. Mengambil sampel acak sebanyak 500 data dari total 1.000 entri.
        
   * Konversi Tabel ke Format Teks
      - Langkah ini memungkinkan data dikonversi menjadi representasi teks agar dapat digunakan dalam model bahasa besar (Large Language Model).
        
   * Heatmap dan Korelasi Antar Fitur
      ![download123](https://github.com/user-attachments/assets/57cb0f37-29ad-4446-a46f-fa6b9f31afa1)


3. **AI Modeling**

   * Menggunakan LLM dan rule-based logic untuk klasifikasi apakah performa meningkat, menurun, atau tetap
   * Pendekatan berbasis decision tree atau Naive Bayes untuk interpretasi mudah

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
