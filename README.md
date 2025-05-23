# 💼 Analisis Kualifikasi Pekerjaan dengan GenAI

## 📌 Judul Proyek
**Pemahaman Kualifikasi Pekerjaan Menggunakan GenAI: Analisis dan Rekomendasi Keterampilan**

## Project Overview
Proyek ini memanfaatkan kekuatan Generative AI (GenAI) untuk menganalisis dan mendapatkan insight dari dua dataset publik yang berisi deskripsi dan kualifikasi pekerjaan dari perusahaan teknologi besar: Google dan Amazon.

Tujuan dari proyek ini adalah untuk:
- Mengidentifikasi keterampilan yang paling banyak dicari.
- Menganalisis gap keterampilan antara minimum dan preferensi.
- Mengklasifikasikan posisi pekerjaan berdasarkan tingkat senioritas.
- Memberikan rekomendasi upskilling (peningkatan keterampilan) bagi pencari kerja menggunakan model bahasa besar (LLM).

## 📂 Tautan Dataset Mentah
1. [Google Job Skills Dataset (Kaggle)](https://www.kaggle.com/datasets/niyamatalmass/google-job-skills)
2. [Amazon Job Skills Dataset (Kaggle)](https://www.kaggle.com/datasets/atahmasb/amazon-job-skills)

## Analysis Process


## 📊 Insight & Findings
Beberapa temuan awal dari analisis menggunakan GenAI:
- 📌 **Keterampilan Paling Dicari**: Python, Machine Learning, Komunikasi, Cloud Computing, dan Agile Methodology.
- ⚠️ **Gap Keterampilan**: Banyak posisi yang membutuhkan pengalaman dengan sistem berskala besar, kolaborasi tim, dan cloud, namun tidak banyak dicakup dalam kurikulum dasar teknik.
- 🧩 **Distribusi Tingkat Pekerjaan**: Mayoritas posisi berada di level Menengah, diikuti oleh level Pemula dan Senior.
- 🎯 **Rekomendasi Upskilling**: Belajar tentang Cloud (AWS/GCP), pengembangan API, dan Data Analytics penting untuk peningkatan karier.
- 🧠 **Klasterisasi Kualifikasi**: GenAI mengelompokkan keterampilan sejenis menjadi tema besar seperti: Deep Learning, Infrastruktur Cloud, dan Proyek Tim.


## Conclusion & Recommendations

## 🤖 AI Support Explanation
Teknologi AI, khususnya LLM seperti GPT, digunakan untuk:
- Mengklasifikasikan dan menganalisis teks tidak terstruktur dari kolom `Minimum Qualifications` dan `Preferred Qualifications`.
- Menghasilkan ringkasan kualifikasi pekerjaan dan menyarankan bidang pengembangan diri.
- Mengklasifikasikan posisi pekerjaan berdasarkan tingkat senioritas menggunakan pemahaman semantik.
- Membersihkan data dan menggabungkan informasi dari dua sumber yang berbeda.

### Contoh Prompt yang Digunakan:
```plaintext
Title: Software Development Engineer
Minimum Qualifications: Sarjana Ilmu Komputer, pengalaman Java 2 tahun.
Preferred Qualifications: Pengalaman dengan AWS, Docker, dan Agile Development.

Tolong ringkas keterampilan utama, rekomendasi upskilling, dan klasifikasi tingkat senioritas.
