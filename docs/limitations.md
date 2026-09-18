# Limitations dan Responsible Use

- Dataset sepenuhnya sintetis dan bukan bukti performa pada bank nyata.
- Satu periode test tidak cukup untuk menyimpulkan kestabilan jangka panjang.
- Perubahan prevalensi, populasi, proses onboarding, atau pola serangan dapat
  mengubah calibration dan ranking.
- Recall pada kapasitas review tidak mengukur seluruh dampak bisnis atau biaya
  false positive.
- Interpretasi TreeSHAP bersifat lokal dan bukan penjelasan kausal.
- Skor tidak membuktikan seseorang melakukan fraud.
- Model tidak boleh digunakan untuk automated rejection atau approval.
- Deployment nyata memerlukan validasi populasi baru, fairness assessment,
  monitoring drift, audit trail, security review, dan human oversight.

Showcase ini sengaja tidak mempublikasikan dataset kerja, serialized model,
payload API, feature contract, konfigurasi training, notebook eksperimen, atau
detail implementasi internal.
