# ✈️ British Airways — Customer Booking Prediction Model

> **Machine Learning Analysis | Heathrow Terminal 3 Capacity Planning**  
> British Airways Virtual Experience Programme — Task 2

---

## 📌 Project Overview

Built a **Random Forest classification model** on 50,000 British Airways customer bookings to predict whether a customer will complete a booking. The model identifies the strongest conversion signals — helping BA prioritise marketing, optimise checkout flows, and plan terminal capacity.

---

## 🏆 Key Results

| Metric | Score |
|---|---|
| **ROC-AUC** | **0.745** |
| **Recall** | **73.6%** |
| **Accuracy** | 65.1% |
| **F1 Score** | 0.386 |

> Validated with **5-Fold Stratified Cross-Validation** · `class_weight='balanced'` · 200 estimators

---

## 🔍 Top Features by Importance

| Rank | Feature | Importance | Business Insight |
|---|---|---|---|
| 1 | **Booking Origin** | **51.6%** | Strongest predictor — customers from certain origins book far more reliably |
| 2 | **Length of Stay** | 12.1% | Longer stays correlate with higher booking completion |
| 3 | **Flight Duration** | 10.3% | Long-haul routes see more committed conversions |
| 4 | **Extras Selected** | 4.2% | Add-on selectors are more likely to complete |
| 5 | **Purchase Lead** | 4.0% | Early planners complete bookings at higher rates |

---

## 💡 Business Recommendations

1. **Target by Origin** — Prioritise proactive marketing to high-converting booking-origin segments identified by the model.
2. **Long-Stay Incentives** — Upsell packages and early-bird discounts for passengers with stays > 7 days.
3. **Bundle Extras Early** — Prompt seat/meal/baggage selection at checkout — extras correlate strongly with conversion.

### ⚠️ Model Limitations
ROC-AUC of 0.745 is promising but class imbalance (85/15 split) limits precision (0.26). Enriching data with loyalty tier and historical behaviour would improve model precision significantly.

---



## 🛠️ Tech Stack

- **Python** — Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Model** — Random Forest Classifier (200 estimators, class_weight='balanced')
- **Validation** — 5-Fold Stratified Cross-Validation
- **Dataset** — 50,000 customer bookings · 17 features

---

## ⚙️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/british-airways-ml-booking.git
cd british-airways-ml-booking

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebook
jupyter notebook notebooks/task2_booking_prediction_model.ipynb
```

---

## 📦 requirements.txt

```
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
```

---

## 🗂️ Task 1 — Lounge Eligibility (Bonus)

Built a structured **lookup table** for Heathrow Terminal 3 lounge eligibility:
- **8 customer groupings** across booking classes and loyalty tiers
- **3 access tiers** (Full Access / Restricted / No Access)
- Used for capacity planning and customer communication

---

## 👤 Author

**Kashish Yadav**  
B.Tech AI & Robotics · World College of Technology and Management, Gurgaon  
[LinkedIn](https://linkedin.com/in/kashish-yadav-6b73782a3) · kashishrao68@gmail.com

---

## 📜 Certificate

Completed as part of the **British Airways Virtual Experience Programme** on Forage — March 2026.

---

*⭐ If you found this useful, give it a star!*
