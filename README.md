# Telco Customer Churn Analysis & Prediction
An end-to-end data analyze and machine learning project on customer churn behavior for a telecommunications company (Telco)

---

## Project Goals
* **Identify Churn Patterns (EDA):** Uncover high-risk customer segments (overall churn is **26.5%**, peaking in **Fiber optic** users and **Month-to-month** contracts).
* **Build a High-Recall Model:** Predict binary churn (`0 = Stay`, `1 = Churn`) while prioritizing **Recall** to minimize missed churning customers (*False Negatives*).
* **Drive Retention Strategy:** Highlight key churn drivers to guide *Marketing/CRM*, *Customer Success*, *Product*, and *Finance* teams.

---

## Features Breakdown
*	**Dependents**: Whether the customer has dependents or not.
*	**Tenure**: Number of months the customer has stayed with the company.
*	**OnlineSecurity**: Whether the customer has online security or not.
*	**OnlineBackup**: Whether the customer has online backup or not.
*	**InternetService**: Whether the client is subscribed to Internet service.
*	**DeviceProtection**: Whether the client has device protection or not.
*	**TechSupport**: Whether the client has tech support or not 
*	**Contract**: Type of contract according to duration.
*	**PaperlessBilling**: Bills issued in paperless form.
*	**MonthlyCharges**: Amount of charge for service on monthly bases.
*	**Churn**: Whether the customer churns or not.

---

## System Requirements
* **Environment:** Jupyter Notebook, VS Code, or Google Colab)
* **Libraries:** `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## Limitations
* **Missing Behavioral Context:** The dataset lacks customer demographics (age/location), network outage logs, and support ticket history.
* **No `CustomerID` Column:** Removing 77 exact duplicate rows may slightly risk dropping distinct customers with identical profiles and charges.
* **Precision vs. Recall Trade-off:** Using `class_weight='balanced'` achieves **80.2% Recall** at **~51.6% Precision**, meaning some loyal customers will also receive retention offers.

---

## Future Roadmap
- [ ] **Cost-Based Threshold Tuning:** Optimize the classification threshold using retention promo costs vs. Customer Lifetime Value (CLV).
- [ ] **Advanced Modeling & Feature Engineering:** Test *XGBoost/LightGBM* with *SMOTE*, and engineer new features like total active add-ons per user.
- [ ] **Interactive Web App:** Deploy a **Streamlit** dashboard for non-technical teams to upload `.csv` files and score customer churn risk.

---
## License & Copyright

Copyright (c) 2026 Cocorals. All rights reserved.

This system (software) and it's documentation are developed solely for academic purposes.
No part of this repository may be produced, distributed, or transmitted in any form without prior written permission from the author.

* Data Source: https://drive.google.com/drive/folders/1_fR7R0srpZgnFnanbrmELgnK-xmzMAHp
* Public presentation: https://canva.link/skdqiowxybi9v69
