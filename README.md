## 📘 Project Overview

This project investigates the effect of hormonal therapy on the survival of breast cancer patients using survival analysis techniques. Most breast cancers are hormone-receptor positive, meaning they grow in response to estrogen or progesterone. Hormonal treatments like tamoxifen or aromatase inhibitors are commonly used to slow progression.

Using data from 686 patients, this analysis compares survival outcomes between those who received hormonal therapy and those who did not, adjusting for various clinical and biological covariates.

---
## 📁 Data
Filename: breast_cancer_R.csv

Rows: 686 patients

Variables: 10 columns

-time — Survival time

-cens — Event indicator (1 = event occurred, 0 = censored)

-horTh — Hormonal therapy status

-age — Patient age

-menostat — Menopause status

-tsize — Tumor size

-tgrade — Tumor grade

-pnodes — Positive lymph nodes

-progrec — Progesterone receptor level

-estrec — Estrogen receptor level

---
## 📊 Methods Used
**1. Kaplan-Meier Survival Analysis**
Stratified by hormonal therapy (horTh)

Median survival:

   Without therapy: 1528 days

   With therapy: 2018 days

Log-rank test p-value: 0.0034 → significant difference

**2. Cox Proportional Hazards Model**
Covariates included: horTh, age, menostat, tsize, tgrade, pnodes, progrec, estrec

Initial model failed the proportional hazards assumption


