# Metodologi Evaluasi

Showcase ini merangkum workflow tingkat tinggi tanpa menyertakan command,
konfigurasi, source code, atau feature contract internal.

## Rancangan eksperimen

Data sintetis berisi 1.000.000 baris dan dibagi berdasarkan waktu. Periode
awal digunakan untuk pengembangan model, periode berikutnya untuk calibration
dan model selection, lalu satu periode terakhir dipakai sebagai evaluasi
untouched test.

Pendekatan ini dipilih untuk mengurangi risiko leakage temporal dan memberi
gambaran yang lebih realistis tentang performa pada periode mendatang.

## Model dan decision support

Model utama menggunakan gradient-boosted trees (XGBoost). Probability
calibration diterapkan agar skor risiko lebih bermakna sebagai prioritas review,
bukan sekadar ranking.

TreeSHAP menyediakan konteks interpretasi lokal. Interpretasi tersebut
menjelaskan kontribusi model pada satu prediksi; bukan sebab fraud, bukti
pelanggaran, atau hubungan kausal.

Kapasitas review ditetapkan sebesar 5%. Model membantu memilih prioritas dalam
kapasitas tersebut, sementara analyst tetap melakukan investigasi dan keputusan
akhir.
