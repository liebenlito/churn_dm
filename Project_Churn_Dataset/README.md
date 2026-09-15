# Customer Churn Project Dataset

Dataset sintetis untuk running case mata kuliah Pengantar Data Mining.

## Skenario
Sebuah perusahaan telekomunikasi ingin memahami faktor yang terkait dengan churn, mendeteksi pelanggan berisiko, dan menyusun tindakan retention.

- Snapshot date: 2026-08-31
- Target: `churn_next_30d`
- Definisi target: Yes = pelanggan berhenti berlangganan dalam 30 hari setelah snapshot.

## Ukuran data
- Pelanggan unik: 2,000
- Baris raw customer: 2,020 (termasuk 20 duplicate rows disengaja)
- Churner: 334
- Churn rate: 16.70%
- Monthly usage: 24,000 baris
- Support tickets: 2,440 baris
- Post-churn feedback: 334 baris

## File
- `churn_customers_raw.csv`
- `churn_monthly_usage.csv`
- `churn_support_tickets.csv`
- `churn_post_churn_feedback_DO_NOT_USE_FOR_PREDICTION.csv`
- `data_dictionary.csv`

## Catatan pembelajaran
- Beberapa missing values dan duplicate rows sengaja ditambahkan untuk preprocessing.
- `customer_id` adalah identifier, bukan feature model.
- `service_basket` cocok untuk association rules.
- `churn_monthly_usage.csv` cocok untuk trend analysis / temporal feature engineering.
- Post-churn feedback terjadi setelah outcome dan tidak boleh dipakai sebagai predictor karena target leakage.

Dataset ini sepenuhnya sintetis dan tidak mewakili pelanggan nyata.
