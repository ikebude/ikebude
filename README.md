<div align="center">
  <img src="assets/pi-mark.svg" alt="Precious Ikebude — PI Mark" width="56" height="56" />

  <h1>Precious Ikebude — BI Scientist building AI/ML systems</h1>

  <p>
    <strong>BI · Data Science · Machine Learning · LLM Apps · MLOps · Data Engineering</strong>
  </p>

  <p>
    <a href="https://github.com/ikebude/ai-ml-data-engineering"><strong>Portfolio Hub</strong></a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf"><strong>Showcase Deck (PDF)</strong></a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pptx"><strong>Showcase Deck (PPTX)</strong></a> ·
    <a href="mailto:precious.ikebude@outlook.com"><strong>precious.ikebude@outlook.com</strong></a>
  </p>
</div>

---

## About Me

I bridge **executive Business Intelligence** (Power BI, SQL, governed KPI semantic layers, financial and risk reporting) and **production AI/ML systems** (calibrated fraud scoring, credit-risk scorecards, read-only NL-to-SQL agents, and containerised MLOps pipelines on FastAPI, Airflow, MLflow, and Docker).

With a background in **Economics (B.Sc., 2:1)** and **3+ years** delivering analytics, data governance, and machine learning systems across fintech, banking, and enterprise consulting, I focus on what happens after the notebook: reproducible pipelines, calibrated probability outputs with decision thresholds tied to business cost, and interfaces that risk and operations teams actually use.

> **📄 Solutions Showcase Deck (2025–2026):**
> Browse the 26-slide architecture & product walkthrough — [**Download PDF**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf) | [**Download PowerPoint (.pptx)**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pptx)

---

## Featured Personal Open-Source Products

| Product | Repository | Highlights & Verified Metrics | Stack |
| :--- | :--- | :--- | :--- |
| **Moniguard v2**<br/>*PoD & Mobile-Money Fraud Platform* | [`ikebude/MLOps-Fraud-Detection`](https://github.com/ikebude/MLOps-Fraud-Detection) | End-to-end Nigerian pay-on-delivery & mobile-money fraud scoring engine (`0–1000` risk scale + reason codes) trained on 60,000 chronological transactions (`3.40%` base fraud rate). **`PR-AUC = 0.877`** (95% bootstrap CI `0.845–0.905`), **`ROC-AUC = 0.985`**, **`Recall@5% alert budget = 0.892`**, **`47.9 ms` p95 FastAPI scoring latency**, PSI drift monitor & champion/challenger gate (`20/20` pytest passing). | Python, LightGBM, Scikit-learn, FastAPI, MLflow, Airflow, Docker |
| **Lolo's Ledger (FXLedger)**<br/>*Multi-Asset Trading Journal & AI Coach* | [`ikebude/FX-Trading-Journal`](https://github.com/ikebude/FX-Trading-Journal) · [`ikebude/AI-Trading-Intelligence`](https://github.com/ikebude/AI-Trading-Intelligence) | Offline-first desktop & web trading journal, position-sizing risk engine (`1%` equity / drawdown guardrails), expectancy & R-multiple analytics, and rule-adherence AI coach across Forex, Crypto, Stocks, Futures, and Options. **`521/521` unit tests + `25` Playwright E2E tests passing**. | TypeScript, React 18, Electron, NestJS, Prisma, SQLite/PostgreSQL, Playwright |
| **BI Operations Agent**<br/>*Governed NL-to-SQL & KPI Anomaly Copilot* | [`ikebude/AIMLOps-BI-Operations-Agent`](https://github.com/ikebude/AIMLOps-BI-Operations-Agent) | Read-only NL-to-SQL copilot backed by a governed YAML semantic layer (`SELECT`/`WITH` AST guardrail, automatic `LIMIT` enforcement), robust **MAD z-score** KPI anomaly detector, and weekly executive brief generator (`100%` execution accuracy on benchmark suite). | Python, FastAPI, DuckDB, SQLAlchemy, YAML Semantic Layer, Pytest |
| **LoanLens & Customer Intelligence**<br/>*Credit-Risk Scorecard & CLV/Churn Suite* | [`ikebude/ai-ml-data-engineering`](https://github.com/ikebude/ai-ml-data-engineering) | **LoanLens:** Prosper P2P probability-of-default scorecard (`WoE + Logistic Regression` & `LightGBM`, calibrated `A–E` risk bands, KS/Gini policy simulator, fairness audit). **Customer Intelligence:** RFM segmentation, calibrated churn propensity, and `BG/NBD + Gamma-Gamma` lifetime value engine. | Python, Scikit-learn, LightGBM, DuckDB, FastAPI, Streamlit |
| **AIOps Expense Tracker**<br/>*NGN-First Categoriser, OCR & Spend Forecaster* | [`ikebude/AIOps_Expense_Tracker`](https://github.com/ikebude/AIOps_Expense_Tracker) | Multi-currency (`NGN`/`USD`/`GBP`/`EUR`) expense intelligence service with `TF-IDF + Logistic Regression` merchant categoriser, receipt OCR parser, seasonal budget forecaster, and MAD anomaly alerts. *(Started from the Code with Mosh course starter; rebuilt and extended by me.)* | Python, FastAPI, Scikit-learn, React, TypeScript, Vite |

---

## Industry Solutions (3Consulting Limited — Case Studies)

> *Company property of 3Consulting Limited. Presented publicly as architectural case studies with live links and stack documentation — no proprietary source code is hosted in public repositories.*

| Solution | Live Production Link | Case Study | Architecture & My Contributions |
| :--- | :--- | :--- | :--- |
| **SafeData**<br/>*NDPA / GDPR Data Retention & Disposal Platform* | [`safedata.3consult-ng.com`](https://safedata.3consult-ng.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/safedata) | Multi-tenant data-retention enforcement, Records of Processing Activities (RoPA), DSAR & consent-withdrawal disposal workflows, immutable SHA-256 audit hash-chaining, and automated PII discovery across enterprise data stores. |
| **FraudGuard**<br/>*Real-Time Transaction & Login Fraud Scoring* | [`fraudguard.3consult-ng.com`](https://fraudguard.3consult-ng.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/fraudguard) | Hybrid rule + ML ensemble (`0–1000` calibrated score + reason codes) for payment, PoD, and account-takeover events, velocity feature store, analyst triage & SAR case queue, and PSI model-drift monitoring. |
| **Africa Stablecoin Intelligence**<br/>*Pan-African Stablecoin & Regulatory Tracker* | [`africastablecoinintelligence.com`](https://africastablecoinintelligence.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/africa-stablecoin-intelligence) | Live market-corridor analytics, USDT/USDC/cNGN liquidity & FX premium pipelines, 54-country central-bank regulatory intelligence tracker, and editorial research portal. |

---

## Portfolio Hub — [`ikebude/ai-ml-data-engineering`](https://github.com/ikebude/ai-ml-data-engineering)

All **11 Machine Learning, Statistical Modelling & Business Intelligence** projects live in the unified monorepo with reproducible `src/` pipelines, automated tests, and executive insights:

### Machine Learning & Statistical Modelling (6 Projects)
1. [**Prosper Loan Credit Risk (`prosper-loan-risk`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/prosper-loan-risk) — Probability-of-default scorecard (`ROC-AUC 0.903`, `KS 0.654`), WoE binning, and expected-loss cutoff optimisation across 113,937 loans.
2. [**Waze User Churn Prediction (`waze-churn-prediction`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/waze-churn-prediction) — Behavioural churn propensity modelling (`ROC-AUC 0.818`, `Recall@20% = 0.548`) with session-intensity and streak feature engineering.
3. [**TLC NYC Cab Fare Intelligence (`tlc-cab-fare-intelligence`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/tlc-cab-fare-intelligence) — Trip fare prediction (`R² = 0.934`, `MAE = $1.84`) and anomaly detection over NYC Yellow Taxi records.
4. [**Customer Retention & Cohort CLV (`customer-retention`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/customer-retention) — RFM segmentation, cohort decay matrices, and survival/churn risk scoring for B2B & retail retention teams.
5. [**S&P 500 Financial Clustering (`sp500-analysis`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/sp500-analysis) — PCA dimensionality reduction + K-Means regime clustering across S&P 500 fundamentals, valuation multiples, and volatility profiles.
6. [**Used Car Valuation & Hedonic Pricing (`cars-model-analysis`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/cars-model-analysis) — Non-linear depreciation curves and gradient-boosted valuation intervals (`R² = 0.912`).

### Analytics, SQL & Business Intelligence (5 Projects)
7. [**CRM B2B Sales Funnel Analysis (`crm-sales-analysis`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/analytics-and-bi/crm-sales-analysis) — Pipeline stage leakage diagnostics, rep win-rate quartiles, and cycle-time attribution across 8,800 B2B opportunities.
8. [**Executive Power BI Dashboards (`power-bi-dashboards`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/analytics-and-bi/power-bi-dashboards) — Star-schema data models, DAX time-intelligence measures, and row-level security (RLS) across Finance, HR, and Sales packs.
9. [**Enterprise BI & Relational Analytics (`bi-analytics`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/analytics-and-bi/bi-analytics) — Data quality remediation framework, customer wealth segmentation, and supply-chain margin diagnostics.
10. [**Global Data Analytics Suite (`global-data-analytics`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/analytics-and-bi/global-data-analytics) — Cross-market cohort retention, content catalogue clustering, and macroeconomic panel studies.
11. [**Production SQL Querying Patterns (`sql-querying`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/analytics-and-bi/sql-querying) — Advanced CTEs, window functions, cohort retention queries, and revenue waterfall reconciliations.

---

## Core Technical Stack

- **Business Intelligence & Analytics:** Power BI (DAX, Power Query M, Star Schema, Row-Level Security), Tableau, Advanced Excel (VBA, Pivot Models), KPI Semantic Layers, Executive Storytelling
- **Machine Learning & Data Science:** Python (`scikit-learn`, `LightGBM`, `XGBoost`, `statsmodels`, `SHAP`, `pandas`, `numpy`), Cost-Sensitive Imbalanced Classification, Probability Calibration, Credit Scorecards (WoE/IV), RFM & BG/NBD CLV, Time-Series Forecasting
- **AI Agents & MLOps:** FastAPI, MLflow, Apache Airflow, NL-to-SQL Guardrails, DuckDB, SQLAlchemy, Docker & Docker Compose, GitHub Actions CI/CD, Azure Container Registry, Model Drift Monitoring (PSI / KS / MAD)
- **Databases & Engineering:** PostgreSQL, MS SQL Server, SQLite, DuckDB, TypeScript / React / Electron / NestJS

---

## Education & Credentials

- **B.Sc. Economics** — University of Nigeria, Nsukka *(Second Class Upper Division / 2:1, Oct 2018 – Aug 2023)*
- **Google Advanced Data Analytics Professional Certificate** — Coursera *(Apr 2025)*
- **Microsoft Certified: Azure AI Engineer Associate** — *(In View, 2026)*
- **Managerial Economics & Business Analysis Specialization** — Gies College of Business, UIUC *(Jun 2023)*

---

## Connect With Me

- **Email:** [precious.ikebude@outlook.com](mailto:precious.ikebude@outlook.com)
- **Portfolio Monorepo:** [github.com/ikebude/ai-ml-data-engineering](https://github.com/ikebude/ai-ml-data-engineering)
- **Solutions Deck (PDF):** [Precious-Ikebude-Solutions.pdf](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf)
- **Kaggle:** [kaggle.com/ikebude](https://www.kaggle.com/ikebude)
