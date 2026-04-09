# 🚗 Ride-Hailing Driver Acceptance Prediction
**Optimizing Matchmaking Efficiency using Machine Learning**

## 📌 Project Overview
Proyek ini menganalisis fenomena "pilih-pilih order" oleh mitra pengemudi pada platform ride-hailing (seperti Gojek/Grab). Fokus utamanya adalah memprediksi kemungkinan sebuah pesanan akan ditolak berdasarkan faktor lingkungan dan detail pesanan, guna mengurangi waktu tunggu pelanggan.

## 📊 Key Insights (EDA)
Berdasarkan analisis pada dataset simulasi, ditemukan beberapa temuan kunci:
* **Threshold Jarak:** Driver memiliki kecenderungan menolak pesanan secara signifikan (probabilitas >40%) jika jarak jemput melebihi **1.5 km**.
* **Dampak Cuaca:** Kondisi hujan menurunkan probabilitas penerimaan order sebesar **20%**, menunjukkan perlunya penyesuaian tarif dinamis atau insentif khusus.
* **Metode Pembayaran:** Pesanan dengan metode non-tunai (E-Wallet) menunjukkan tingkat penerimaan yang lebih stabil dalam simulasi ini.

## 🛠️ Tech Stack & Methodology
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib
* **Algorithm:** Random Forest Classifier
* **Evaluation:** Confusion Matrix & Feature Importance

## 🤖 Machine Learning Results
Model ini dikembangkan untuk mendeteksi potensi kegagalan penjemputan:
* **Accuracy:** ~66% (Baseline)
* **Recall (Ditolak):** 72% — Model sangat sensitif dalam menangkap pesanan yang berisiko ditolak.
* **Predictive Power:** Untuk pesanan jarak jauh (>3.5km) saat hujan, model memberikan **probabilitas penolakan hingga 89%**.

## 💡 Business Recommendations
1. **Dynamic Pickup Incentive:** Memberikan bonus otomatis bagi driver jika jarak penjemputan di atas 1.5 km untuk menyeimbangkan biaya operasional driver.
2. **Rain-Specific Surge:** Penyesuaian tarif saat hujan untuk mengompensasi risiko pengemudi di jalan.
3. **Priority Dispatch:** Mengalokasikan driver terdekat secara lebih agresif untuk pesanan yang diprediksi memiliki risiko penolakan tinggi.

---
*Created as part of my Data Science Journey.*
