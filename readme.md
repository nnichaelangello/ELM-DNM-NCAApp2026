File json bisa dipakai untuk:
1. Tabel Kinerja Utama (Main Classification Performance Table):
- Isi: Komparasi model unggulan (ELM-DNM) melawan baseline (RF, SVM, MLP) dan state-of-the-art turunan DNM (Standar DNM, MODN).
- Metrik yang Dipakai: Rata-rata & 95% Confidence Interval (CI) dari Accuracy, F1-Score, dan ROC AUC.

2. Tabel Sensitivitas Medis & Diagnostik (Clinical Diagnostic Metrics Table):
- Isi: Komparasi khusus untuk mengukur kemampuan sistem di ranah kesehatan.
- Metrik yang Dipakai: Sensitivity (Recall kelas sakit), Specificity (Kemampuan mengenali kelas sehat), dan Balanced Accuracy (sebagai bukti penanganan dataset yang tidak seimbang).

3. Tabel Studi Ablasi Komponen (Component Ablation Study Table):
- Isi: Jejak kinerja dari model paling dasar hingga lengkap (ELM Linear $\rightarrow$ ELM Sigmoid $\rightarrow$ ELM Self-Gate $\rightarrow$ ELM-DNM No-Regularization $\rightarrow$ ELM-DNM Final).
- Metrik yang Dipakai: Accuracy, F1-Score, ROC AUC.

4. Tabel Analisis Fungsi Aktivasi & Arsitektur (Hyperparameter Effect Table):
- Isi: Perbandingan fungsi aktivasi (Sigmoid vs ReLU vs Tanh vs Linear) di-cross-check dengan variasi jumlah neuron (hidden size 50, 100, 200).
- Metrik yang Dipakai: Rata-rata Accuracy dan Sensitivity.

5. Tabel Analisis Biaya Komputasi Ekstensif (Comprehensive Computational Cost Table):
- Isi: Rincian setiap detik yang dihabiskan dalam pipeline.
- Metrik yang Dipakai: Preprocessing Time (detik), Training Time (detik), Inference Time (detik), Time per Epoch (detik, khusus gradient descent), dan Peak Memory Usage (MB).

6. Tabel Uji Signifikansi Statistik (Pairwise Statistical Significance Matrix):
- Isi: Matriks p-value atau ringkasan tolak/terima H0.
- Metrik yang Dipakai: Hasil Holm p-value, statisik Friedman chi2, dan Cohen's d_z (Effect Size).

7. Grafik Boxplot & Violin Plot Distribusi Performa

8. Kurva Perbandingan Waktu-Akurasi (Scatter Plot / Pareto Front)

9. Heatmap Matriks Kebingungan Lintas-Fold (Aggregated Confusion Matrix)

10. Grafik Laba-laba Multi-Metrik (Radar/Spider Chart)

11. Kurva Uji Pengaruh Regularisasi (Line Chart of Lambda Impact):

dan lain-lain