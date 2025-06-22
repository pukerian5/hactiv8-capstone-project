# Vehicle Pricing Classification - Capstone Project Hacktiv8

## 📌 Project Overview

Proyek ini bertujuan untuk mengevaluasi kelayakan harga mobil berdasarkan data historis penjualan kendaraan. Dengan pendekatan Exploratory Data Analysis (EDA) dan model machine learning, proyek ini mengklasifikasikan setiap transaksi sebagai:
- **Fair Price**
- **Overpriced**
- **Underpriced**

Tujuannya adalah membantu pelaku bisnis otomotif, khususnya platform jual-beli kendaraan, dalam:
- Menetapkan harga yang kompetitif,
- Memberi rekomendasi untuk pembeli dan penjual,
- Mengklasifikasi fairness harga.

---

## 🧾 Raw Dataset

Dataset digunakan berasal dari Kaggle:
> [Vehicle Sales Dataset on Kaggle](**https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data**)

Dataset telah dibersihkan, diproses, dan dikategorikan berdasarkan harga jual terhadap nilai MMR (Manheim Market Report).

---

## 🔍 Insight & Findings

1. **Volume Penjualan**:
   - Volume penjualan cenderung meningkat pasca awal tahun.
   - Brand terlaris: Chevrolet, Ford, dan Dodge.
  
2. **Harga Jual vs MMR**:
   - Banyak mobil dijual di bawah MMR (underpriced), terutama di brand populer.
   - Rata-rata harga jual berkisar 5–10% di bawah MMR.

3. **Seller Behavior**:
   - GM Remarketing dominan pada fair pricing.
   - "Enterprise Vehicle Exchange / TULSA" mendominasi underpriced sales.

4. **State-Wise Trends**:
   - Illinois memiliki proporsi fair price tertinggi (~72.1%).
   - California menunjukkan kecenderungan underpricing lebih tinggi (~39.3%).

---

## 🤖 AI Support Explanation

Model klasifikasi XGBoost digunakan untuk mengklasifikasikan kategori harga:
- **Fitur yang digunakan**: body, condition, car_age, odometer, make, dan lainnya.
- **Model**: Random Forest Classifier.
- **Hasil**:
  - Akurasi: ±75% (menggunakan predicted MMR)
  - Model cenderung baik dalam mengenali **Fair Price**, namun lebih menantang untuk kelas **Overpriced**.

---
