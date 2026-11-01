<div align="center">
  <img src="assets/pi-mark.svg" alt="PI monogram" width="56" height="56" />

  <h1>Precious Chidiebere Ikebude</h1>

  <p><strong>BI Scientist building AI/ML systems</strong> · Lagos, Nigeria</p>

  <p>
    <a href="mailto:precious.ikebude@outlook.com">precious.ikebude@outlook.com</a> ·
    <a href="https://wa.me/2348136787181">WhatsApp +234 813 678 7181</a> ·
    <a href="https://ikebude.github.io">ikebude.github.io</a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering">Portfolio hub</a>
  </p>
</div>

---

I turn business data into dashboards people use, models that are measured honestly, and small services that run them. **3+ years** of data, BI and finance-analytics work since Nov 2022; currently **BI Scientist || AI/ML Engineer at 3Consulting Limited** (Lagos), after starting there as a Junior Data Analyst in Jun 2025. B.Sc. Economics (2:1).

**Open to:** BI Analyst · Data Analyst · Data Scientist · junior ML Engineer.

**Work:** remote (Nigeria or worldwide) or Lagos; full-time roles and short contracts (dashboards, SQL and reporting, churn or risk models).

**What I bring:** Power BI and SQL reporting that answers a business question; models judged on out-of-time data against a simple baseline, with calibrated probabilities and stated limitations; and the engineering around them (FastAPI, MLflow, Airflow, Docker, CI).

---

## Featured work

| Project | What it is | Results (from the repo's `reports/*.json`) | Stack |
| :--- | :--- | :--- | :--- |
| [**Moniguard**](https://github.com/ikebude/MLOps-Fraud-Detection) | Fraud scoring service for pay-on-delivery and mobile-money transactions: a 0–1000 score with reason codes | On 60,000 **synthetic** transactions, time-based 70/30 split: **PR-AUC 0.959** (95% CI 0.942–0.972) in batch evaluation and **0.837** when each transaction is scored on its own through the API, as in live use | Python, XGBoost, Isolation Forest, FastAPI, MLflow, Airflow, Docker |
| [**LoanLens**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/prosper-loan-risk) | Credit default scorecard on public Prosper loans, with a leakage gate in tests and an approval-policy simulator | Trained on 41,638 earlier loans, tested on 13,880 later ones: **ROC-AUC 0.705** (95% CI 0.695–0.714), **KS 0.303** | Python, scikit-learn, Streamlit |
| [**BI Operations Agent**](https://github.com/ikebude/AIMLOps-BI-Operations-Agent) | Ask business questions in plain English; answers come from a governed semantic layer through a read-only SQL guard, plus daily KPI anomaly checks | On **synthetic** retail data: **96.0%** (48/50) in-sample and **56.0%** (14/25) held-out questions correct, **12/12** unsafe prompts blocked, 36.6 ms p95 | Python, FastAPI, SQLite, sqlglot, Streamlit |
| [**Customer Intelligence**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/customer-retention) | Telco churn model that ranks a weekly call list by revenue at risk, plus RFM segments | 7,043 customers (public data): **PR-AUC 0.841**, ROC-AUC 0.933, 80.5% precision when calling 20% of customers | Python, scikit-learn, Streamlit |
| [**AIOps Expense Tracker**](https://github.com/ikebude/AIOps_Expense_Tracker) | NGN personal and small-business finance app, extended from a course starter | On **synthetic** data: categoriser **macro-F1 0.920** (rules baseline 0.780), receipt-text field match 97.5% (text parsing, not OCR), forecast WAPE 8.1% (naive 11.2%) | Python, scikit-learn, FastAPI, React |
| [**Lolo's Ledger**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/products/lolos-ledger) | Multi-asset trading journal and position-sizing risk engine with an AI analyst that never gives trading signals (source private; case study linked) | Qualitative: built on my desktop journal's engine and its tests | TypeScript, React, NestJS, PostgreSQL, Python |

More ML, SQL and Power BI projects, each with a short README and its numbers, are in the [portfolio hub](https://github.com/ikebude/ai-ml-data-engineering).

---

## Work at 3Consulting Limited

Shown as engineering case studies only; company source code is not public, and the public sites are *deployment pending verification*.

- **[FraudGuard](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/fraudguard)** (transaction fraud prevention): feature engineering for the scoring ensemble, Airflow and MLflow retraining, PostgreSQL-to-Kafka outbox, analyst dashboard. FraudGuard is the company's product; Moniguard above is my separate personal project.
- **[SafeData](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/safedata)** (NDPA/GDPR data retention and consent): retention-rule logic, PostgreSQL test-suite fixes, CI with linting, dependency auditing and secret scanning.
- **[Africa Stablecoin Intelligence](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/africa-stablecoin-intelligence)** (market and regulatory tracker): structured the market and regulatory indicators, Light/Dark/System theming, launch and indexing preparation.

---

## Skills

- **BI and analytics:** Power BI (DAX, Power Query, star schemas, row-level security), Tableau, Excel (pivot tables, VBA), KPI definitions
- **SQL:** PostgreSQL, SQL Server, SQLite, DuckDB; CTEs and window functions
- **Data science and ML:** Python (pandas, NumPy, scikit-learn, XGBoost, statsmodels, SHAP), R; imbalanced classification, probability calibration, credit scorecards (WoE, KS), RFM and CLV, time-series forecasting
- **ML engineering:** FastAPI, MLflow, Airflow, Docker and Docker Compose, GitHub Actions; TypeScript and React for front ends

---

## Education and certificates

- **B.Sc. Economics**, University of Nigeria, Nsukka. Second Class Upper (2:1), Sep 2017 – Nov 2022
- **Google Advanced Data Analytics Professional Certificate**, Coursera, Apr 2025
- **Managerial Economics & Business Analysis Specialization**, Gies College of Business (UIUC), Coursera, Jun 2023
- **Microsoft AI & ML Engineering Professional Certificate**, Coursera: *in progress, target Dec 2026*
- **Google Cybersecurity Professional Certificate**, Coursera: *in progress*
- **Planned next:** Microsoft Azure and Google Cloud professional certificates (data science / AI engineer associate)

---

## Contact

- **Email:** [precious.ikebude@outlook.com](mailto:precious.ikebude@outlook.com)
- **WhatsApp:** [+234 813 678 7181](https://wa.me/2348136787181)
- **Website:** [ikebude.github.io](https://ikebude.github.io)
- **Data-science portfolio:** [datascienceportfol.io/ikebude](https://www.datascienceportfol.io/ikebude)
- **GitHub:** [github.com/ikebude](https://github.com/ikebude) · portfolio hub [ai-ml-data-engineering](https://github.com/ikebude/ai-ml-data-engineering)
- **Kaggle:** [kaggle.com/ikebude](https://www.kaggle.com/ikebude)
