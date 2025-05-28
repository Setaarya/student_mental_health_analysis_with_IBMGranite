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


3. **AI Analysis**

   * Menggunakan model LLM IBM Granite untuk menganalisis data yang disediakan dan mencari insight baru
   * Menggunakan model LLM IBM Granite untuk membuat sebuah prediksi dengan data yang disediakan

---

## 💡 **Insight & Findings**

1. **Ringkasan Sebaran Data Kategorikal**

   Dataset mencakup keberagaman responden berdasarkan gender, usia (15–26 tahun), dan jenjang pendidikan dari kelas 8 hingga pascasarjana. Variabel kesejahteraan psikologis                 menunjukkan mayoritas siswa mengalami tingkat stres rendah hingga sedang, dengan lebih dari setengahnya merasa cemas sebelum ujian dan sebagian besar melaporkan performa akademik        yang tetap atau meningkat selama pembelajaran daring.

2. **Ringkasan Sebaran Data Numerik**

   Durasi screen time berkisar antara 2 hingga 15 jam per hari, sementara durasi tidur bervariasi dari 5 hingga 12 jam. Aktivitas fisik mingguan memiliki rentang yang luas, mulai dari      tidak ada sama sekali (0 jam) hingga 16 jam per minggu.

3. **Korelasi Antara Screen Time dengan Stress Level**

   Hasil analisis menunjukkan bahwa screen time yang tinggi cenderung berkorelasi dengan peningkatan tingkat stres. Individu dengan tingkat stres "tinggi" umumnya memiliki durasi           screen time yang lebih tinggi (8,1–11,5 jam/hari). Meskipun demikian, terdapat beberapa anomali di mana individu dengan stres "sedang" juga memiliki screen time tinggi, namun            jumlahnya relatif sedikit. Tidak ditemukan pola yang menunjukkan bahwa screen time rendah berhubungan dengan stres tinggi, sehingga kemungkinan terdapat faktor lain yang lebih           dominan dalam menyebabkan stres pada kasus-kasus tersebut.

4. **Korelasi Antara Screen Time dengan Academic Performance**
   
   Korelasi antara screen time dan performa akademik menunjukkan hasil yang beragam. Beberapa individu dengan screen time tinggi (hingga 11,5 jam/hari) justru melaporkan peningkatan        performa akademik, sementara lainnya mengalami penurunan atau tidak ada perubahan. Hal ini menunjukkan bahwa screen time yang tinggi tidak selalu menjadi indikator penurunan             prestasi belajar.

5. **Korelasi Antara Sleep Duration dengan Stress Level**

   Individu dengan stres rendah memiliki rentang tidur yang bervariasi (4,5–9 jam) tanpa pola yang jelas. Pada stres sedang, umumnya durasi tidur berkisar antara 5–8,7 jam, dengan          kecenderungan sedikit lebih panjang. Namun, tidur kurang dari 5 jam pada kelompok ini sering dikaitkan dengan stres yang lebih tinggi. Sementara itu, individu dengan stres tinggi        umumnya memiliki durasi tidur yang lebih pendek (2–7,6 jam).

6. **Korelasi Antara Sleep Duration dengan Academic Performance**
    
   Performa akademik yang meningkat umumnya terjadi pada siswa dengan durasi tidur 5,1–8,8 jam. Siswa dengan performa tetap memiliki rentang tidur yang lebih luas (3,2–8,8 jam) tanpa       pola khusus. Sebaliknya, penurunan performa akademik cenderung dikaitkan dengan durasi tidur yang lebih pendek (2,0–7,3 jam), dan hampir tidak ditemukan kasus tidur lebih dari 7,5       jam dalam kelompok ini.

7. **Korelasi Antara Physical Activity dengan Stress Level**

   Aktivitas fisik yang tinggi (>7 jam/minggu) cenderung berhubungan dengan tingkat stres yang rendah. Sebaliknya, tingkat aktivitas fisik yang rendah (<4 jam/minggu) sering ditemukan      pada individu dengan stres sedang hingga tinggi. Aktivitas fisik sedang (5–7,5 jam/minggu) menunjukkan korelasi yang bervariasi, namun tetap ada kecenderungan bahwa semakin tinggi       aktivitas fisik, semakin rendah tingkat stres yang dirasakan.

8. **Korelasi Antara Physical Activity dengan Academic Performance**

   Aktivitas fisik yang tinggi (>7 jam/minggu) umumnya berkorelasi dengan peningkatan performa akademik. Aktivitas fisik sedang (4–6,5 jam/minggu) menunjukkan hasil yang bervariasi,        dengan sebagian individu mempertahankan atau meningkatkan performanya. Sementara itu, aktivitas fisik yang rendah (<4 jam/minggu) lebih sering dikaitkan dengan stagnasi atau             penurunan performa akademik. Pola ini mengindikasikan bahwa semakin tinggi tingkat aktivitas fisik, semakin besar kemungkinan peningkatan dalam performa akademik.

9. **Rekomendasi Model LLM IBM Granite**

   Rekomendasi Mengurangi Stres dan Meningkatkan Prestasi Akademik

   Batasi Screen Time
   - Screen time >7,5 jam/hari terkait stres tinggi dan penurunan prestasi. Batasi penggunaan layar dan ambil istirahat rutin.

   Tidur Cukup (7-9 Jam)
   - Tidur kurang dari 7 jam berhubungan dengan stres dan prestasi menurun. Terapkan jadwal tidur teratur dan lingkungan tidur nyaman.

   Aktivitas Fisik >6 Jam/Minggu
   - Aktivitas fisik rendah terkait stres tinggi dan prestasi menurun. Tingkatkan olahraga atau aktivitas bergerak rutin.

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
