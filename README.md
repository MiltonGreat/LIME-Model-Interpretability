# Credit Risk Model Interpretability with LIME

![screenshot-localhost_8888-2025 04 03-13_34_01](https://github.com/user-attachments/assets/7e1028b9-6a57-4525-8692-1424d2e241cc)

### Project Overview

This project enhances a credit risk prediction model by using LIME (Local Interpretable Model-Agnostic Explanations) to validate and explain individual loan decisions. It answers:

- Why was an applicant classified as high/low risk?
- Which features drove the model’s decision?
- How can we improve fairness and transparency?

### Dataset

Features:
- Financial (e.g., AMT_INCOME_TOTAL, AMT_CREDIT)
- Demographic (e.g., CODE_GENDER, NAME_EDUCATION_TYPE)
- External credit scores (e.g., EXT_SOURCE_3)
- Target: TARGET (1 = default, 0 = non-default)

### Key Findings

**Top Risk Drivers**

- EXT_SOURCE_3 ≤ 0.42	(↑) Risk	- Reject applicants below this threshold.
- ORGANIZATION_TYPE_Emergency	(↓) Risk - Prefer applicants from stable sectors.
- FLAG_DOCUMENT_14 = 0 (↑)  Risk	- Enforce document submission for high-risk cases.

### Business Applications

1. Loan Approval Automation
- Auto-Approve: Applicants with EXT_SOURCE_3 > 0.5 and complete documentation.
- Flag for Review: Applicants with high-risk LIME explanations.

2. Regulatory Compliance
- Generate audit-ready reports showing decision logic.
- Demonstrate fairness across demographics (e.g., employment sectors).

3. Stakeholder Communication
- Loan Officers: Use LIME outputs to explain denials/approvals.
- Applicants: Provide plain-language summaries (e.g., "Your loan was denied due to low credit score").

### Conclusion

This project successfully validated and explained credit risk predictions using LIME (Local Interpretable Model-Agnostic Explanations), providing transparent, actionable insights into individual loan decisions. Here’s a summary of key outcomes and strategic recommendations:

### Source

![Home Credit Default Risk Dataset from Kaggle](https://www.kaggle.com/datasets/anggundwilestari/home-credit)
