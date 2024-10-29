# final-project
Lung Cancer Prediction

**Objective:** Tujuan dari proyek ini adalah membangun model prediksi yang dapat menilai kemungkinan seseorang terkena kanker paru-paru berdasarkan berbagai kebiasaan hidup, gejala, dan informasi demografis. Dengan menganalisis fitur yang ada dalam dataset, seperti kebiasaan merokok, gejala-gejala seperti batuk atau nyeri dada, serta faktor demografis seperti usia dan jenis kelamin, kita ingin mengembangkan model yang dapat memprediksi risiko kanker paru-paru dengan akurat. Model tersebut nantinya bisa membantu deteksi dini, yang sangat penting untuk meningkatkan peluang kesembuhan kanker paru-paru melalui penanganan medis yang lebih cepat.

**Background:** Kanker paru-paru merupakan salah satu penyebab utama kematian akibat kanker di seluruh dunia. Deteksi dini sangat penting untuk meningkatkan peluang hidup, namun mengenali siapa saja yang berisiko bisa menjadi tantangan. Faktor-faktor seperti kebiasaan merokok, penyakit kronis, kecemasan, dan gejala yang sering dikaitkan dengan kanker paru-paru (seperti batuk, sesak napas, atau nyeri dada) memiliki peran penting dalam menilai risiko. Namun, faktor-faktor ini saja tidak cukup untuk memberikan kepastian, sehingga dibutuhkan model prediksi yang lebih canggih untuk menilai risiko kanker paru-paru dengan lebih tepat.

Dataset Risiko Kanker Paru-paru menyediakan kumpulan data yang meliputi informasi demografis (seperti usia, jenis kelamin), indikator gaya hidup (seperti kebiasaan merokok dan konsumsi alkohol), serta gejala medis (seperti batuk, nyeri dada). Dengan menganalisis dataset ini, kami berupaya mengidentifikasi fitur-fitur yang paling berdampak pada risiko kanker paru-paru dan mengembangkan model machine learning yang bisa memprediksi kemungkinan seseorang didiagnosis dengan kanker paru-paru.

Dari hasil evaluasi yang diberikan, semua model memiliki kinerja yang cukup mirip dengan akurasi di sekitar 0.53 hingga 0.54. Namun, untuk menentukan model mana yang paling baik dalam memprediksi kanker paru, kita perlu melihat lebih jauh pada metrik-metrik evaluasi lainnya seperti Precision, Recall, dan F1-Score, terutama pada masing-masing kelas (positif dan negatif) serta matriks kebingungan (confusion matrix). Berikut analisis lebih lanjut:

**Accuracy:**

Semua model memiliki akurasi yang mirip, antara 0.53 dan 0.54. Ini menunjukkan bahwa tidak ada model yang jauh lebih baik dari yang lain dalam hal ini.

**Precision:**

Precision untuk kelas positif (1) pada model LightGBM (0.55) sedikit lebih tinggi dibandingkan model lainnya. Precision menunjukkan seberapa banyak dari prediksi positif yang benar-benar positif, yang penting jika kita ingin meminimalisir prediksi positif palsu.

**Recall:**

Recall untuk kelas positif (1) juga paling tinggi pada model LightGBM (0.55), artinya model ini mampu mendeteksi lebih banyak kasus kanker paru dibanding model lainnya.

**F1-Score:**

F1-Score untuk kelas positif (1) lagi-lagi lebih tinggi pada model LightGBM (0.55), yang merupakan trade-off antara Precision dan Recall. Hal ini menunjukkan keseimbangan yang lebih baik antara kedua metrik tersebut.

**Confusion Matrix:**

**Model LightGBM** memiliki distribusi yang cukup seimbang dalam mendeteksi kedua kelas (0 dan 1), dengan jumlah true positive (252) dan true negative (232) yang lebih tinggi dibandingkan beberapa model lainnya. Ini menunjukkan kemampuan model untuk memprediksi kedua kelas dengan lebih baik.

**Kesimpulan:**

Meskipun perbedaan antar model tidak terlalu besar, LightGBM menunjukkan kinerja yang sedikit lebih baik dibandingkan model lainnya berdasarkan F1-Score, Precision, dan Recall untuk kelas positif (1). Ini menjadikannya pilihan yang lebih baik jika tujuan utama adalah untuk mendeteksi kasus kanker paru dengan keseimbangan antara mengurangi false positives dan meningkatkan detection rate.