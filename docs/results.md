# Hasil Model

Evaluasi final dilakukan satu kali pada periode test sintetis yang tidak
digunakan untuk pengembangan model.

| Metrik | Hasil |
| --- | ---: |
| ROC-AUC | **0.8954** |
| Average Precision | **0.2135** |
| Brier Score | **0.0129** |
| Expected Calibration Error | **0.0020** |
| Recall @ 5% review capacity | **52.31%** |

## Interpretasi operasional

Pada kapasitas review 5%, sistem berhasil memprioritaskan sebagian besar kasus
positif dalam antrean berukuran terbatas pada evaluasi sintetis ini. Hasil
tersebut mendukung penggunaan model sebagai decision-support queue, bukan
sebagai keputusan otomatis.

Metrik tidak boleh dibandingkan langsung dengan sistem lain tanpa menyamakan
populasi, prevalensi, definisi label, periode waktu, dan kapasitas review.
