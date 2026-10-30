<div align="center">
  <img src="assets/pi-mark.svg" alt="Precious Ikebude — PI Mark" width="56" height="56" />

  <h1>Precious Ikebude — BI Scientist building AI/ML systems</h1>

  <p>
    <strong>BI · Data Science · Machine Learning · LLM Apps · MLOps · Data Engineering</strong>
  </p>

  <p>
    <a href="https://github.com/ikebude/ai-ml-data-engineering"><strong>Portfolio Hub</strong></a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering/tree/main/showcase/carousels"><strong>LinkedIn Carousels</strong></a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf"><strong>Showcase Deck (PDF)</strong></a> ·
    <a href="https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pptx"><strong>Showcase Deck (PPTX)</strong></a> ·
    <a href="mailto:precious.ikebude@outlook.com"><strong>precious.ikebude@outlook.com</strong></a>
  </p>
</div>

---

## About Me

I bridge **executive Business Intelligence** (Power BI, SQL, governed KPI semantic layers, financial and risk reporting) and **production AI/ML systems** (calibrated fraud scoring, credit-risk scorecards, read-only NL-to-SQL agents, and containerised MLOps pipelines on FastAPI, Airflow, MLflow, and Docker).

With a background in **Economics (B.Sc., 2:1)** and **2+ years** delivering analytics, data governance, and machine learning work across accounting advisory, data-protection/fintech consulting, and personal ML products, I focus on what happens after the notebook: reproducible pipelines, calibrated probability outputs with decision thresholds tied to business cost, and interfaces that risk and operations teams actually use.

> **📄 Solutions Showcase Deck (2025–2026):**
> Browse the 26-slide architecture & product walkthrough — [**Download PDF**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf) | [**Download PowerPoint (.pptx)**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pptx)

---

## Featured Personal Products

> Source is public for every product except Lolo's Ledger (private; public case study linked).

| Product | Repository | Highlights & Verified Metrics | Stack |
| :--- | :--- | :--- | :--- |
| **Moniguard v2**<br/>*PoD & Mobile-Money Fraud Scoring* | [`ikebude/MLOps-Fraud-Detection`](https://github.com/ikebude/MLOps-Fraud-Detection) | Fraud scorer (0–1000 score + reason codes) on 60,000 **synthetic** Nigerian pay-on-delivery transactions with a strict 70/30 chronological split. **PR-AUC 0.877** (95% CI 0.845–0.905), **ROC-AUC 0.943**, **recall 0.892 at a 5% alert rate**, **47.9 ms p95** FastAPI latency. | Python, XGBoost, Isolation Forest, FastAPI, MLflow, Airflow, Docker |
| **Lolo's Ledger (FXLedger)**<br/>*Trading Journal, Risk Engine & Analytics* | [Case study: ai-ml-data-engineering/products/lolos-ledger](https://github.com/ikebude/ai-ml-data-engineering/tree/main/products/lolos-ledger)<br/>*Source private* | The archived desktop predecessor (FXLedger v1.1.0) (**521 unit tests + 25 Playwright E2E tests passing**) plus a Python risk and expectancy engine with behavioural tilt detection. Personal-edge attribution is gated until 100+ closed trades and never produces buy/sell signals. | TypeScript, React, Electron, NestJS, Playwright, Python |
| **BI Operations Agent**<br/>*Governed NL-to-SQL & KPI Anomaly Copilot* | [`ikebude/AIMLOps-BI-Operations-Agent`](https://github.com/ikebude/AIMLOps-BI-Operations-Agent) | Read-only NL-to-SQL over a governed YAML semantic layer with SQL AST guardrails (`sqlglot`), blocking mutations and leaks. Benchmark accuracy: **96.0%** across 25 gold-standard business questions with sub-150ms semantic parsing. | Python, FastAPI, DuckDB, sqlglot, React |
| **LoanLens & Customer Intelligence**<br/>*Credit Scorecard & Churn/CLV* | [`ikebude/ai-ml-data-engineering`](https://github.com/ikebude/ai-ml-data-engineering) | **LoanLens:** leak-free default model on 55,518 closed Prosper loans, tested on future loans: **ROC-AUC 0.707**, **KS 0.305**, with an approval-policy simulator. **Customer Intelligence:** churn **PR-AUC 0.841** / **ROC-AUC 0.933** on 7,043 customers, RFM segments and a weekly revenue-at-risk call list. | Python, Scikit-learn, Streamlit |
| **AIOps Expense Tracker**<br/>*NGN-First Expense Intelligence* | [`ikebude/AIOps_Expense_Tracker`](https://github.com/ikebude/AIOps_Expense_Tracker) | Nigerian-first personal and SME finance engine. **0.9204 Macro-F1** NLP transaction categoriser across 14 spending classes, **97.5%** receipt OCR extraction, and 3-month forward ETS expenditure forecasting (**20.42% holdout WAPE**). | Python, Scikit-learn, PaddleOCR, React, Vite |

---

## Industry Solutions (3Consulting Limited — Case Studies)

> *Company property of 3Consulting Limited. Presented publicly as architectural case studies with live links and stack documentation — no proprietary source code is hosted in public repositories.*

| Solution | Live Production Link | Case Study | Architecture & My Contributions |
| :--- | :--- | :--- | :--- |
| **SafeData**<br/>*NDPA / GDPR Data Retention & Disposal Platform* | [`safedata.3consult-ng.com`](https://safedata.3consult-ng.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/safedata) | Multi-tenant data-retention enforcement, Records of Processing Activities (RoPA), DSAR & consent-withdrawal disposal workflows, immutable SHA-256 audit hash-chaining, and automated PII discovery across enterprise data stores. |
| **FraudGuard**<br/>*Real-Time Transaction & Login Fraud Scoring* | [`fraudguard.3consult-ng.com`](https://fraudguard.3consult-ng.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/fraudguard) | Hybrid rule + ML ensemble (`0–1000` calibrated score + reason codes) for payment, PoD, and account-takeover events, velocity feature store, analyst triage & SAR case queue, and PSI model-drift monitoring. |
| **Africa Stablecoin Intelligence**<br/>*Pan-African Stablecoin & Regulatory Tracker* | [`africastablecoinintelligence.com`](https://africastablecoinintelligence.com) | [View Case Study](https://github.com/ikebude/ai-ml-data-engineering/tree/main/industry-work/africa-stablecoin-intelligence) | Live market-corridor analytics, USDT/USDC/cNGN liquidity & FX premium pipelines, 54-country central-bank regulatory intelligence tracker, and editorial research portal. |

---

## 📑 LinkedIn Case Study Carousels (PDF Downloads)

Each product and industry solution has a dedicated executive 6-slide case study carousel (16:9 widescreen, verified metrics, system architecture, and production UI mockups):

| # | Solution | Track | PDF Carousel Link |
| :-: | :--- | :--- | :--- |
| **01** | **SafeData** | 🏢 3Consulting Limited | [**Download 01-SafeData-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/01-SafeData-Case-Study-Carousel.pdf) |
| **02** | **FraudGuard** | 🏢 3Consulting Limited | [**Download 02-FraudGuard-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/02-FraudGuard-Case-Study-Carousel.pdf) |
| **03** | **Africa Stablecoin Intelligence** | 🏢 3Consulting Limited | [**Download 03-Africa-Stablecoin-Intelligence-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/03-Africa-Stablecoin-Intelligence-Case-Study-Carousel.pdf) |
| **04** | **Moniguard v2** | 🔬 Precious Ikebude | [**Download 04-Moniguard-v2-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/04-Moniguard-v2-Case-Study-Carousel.pdf) |
| **05** | **Lolo's Ledger** | 🔬 Precious Ikebude | [**Download 05-Lolos-Ledger-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/05-Lolos-Ledger-Case-Study-Carousel.pdf) |
| **06** | **BI Operations Agent** | 🔬 Precious Ikebude | [**Download 06-BI-Operations-Agent-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/06-BI-Operations-Agent-Case-Study-Carousel.pdf) |
| **07** | **LoanLens** | 🔬 Precious Ikebude | [**Download 07-LoanLens-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/07-LoanLens-Case-Study-Carousel.pdf) |
| **08** | **Customer Intelligence** | 🔬 Precious Ikebude | [**Download 08-Customer-Intelligence-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/08-Customer-Intelligence-Case-Study-Carousel.pdf) |
| **09** | **AIOps Expense Tracker** | 🔬 Precious Ikebude | [**Download 09-AIOps-Expense-Tracker-Case-Study-Carousel.pdf**](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/carousels/09-AIOps-Expense-Tracker-Case-Study-Carousel.pdf) |

---

## Portfolio Hub — [`ikebude/ai-ml-data-engineering`](https://github.com/ikebude/ai-ml-data-engineering)

All **11 Machine Learning, Statistical Modelling & Business Intelligence** projects live in the unified monorepo (upgrades to the remaining projects are in progress):

### Machine Learning & Statistical Modelling (6 Projects)
1. [**Prosper Loan Credit Risk (`prosper-loan-risk`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/prosper-loan-risk) — Out-of-time default scorecard and policy simulator (ROC-AUC 0.707, KS 0.305 on 13,880 future loans).
2. [**Waze User Churn Prediction (`waze-churn-prediction`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/waze-churn-prediction) — Behavioural churn analysis on 14,999 users.
3. [**TLC NYC Cab Fare Intelligence (`tlc-cab-fare-intelligence`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/tlc-cab-fare-intelligence) — NYC Yellow Taxi trip analysis and fare modelling.
4. [**Customer Intelligence (`customer-retention`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/customer-retention) — Calibrated churn (PR-AUC 0.841), RFM segmentation and a CLV backtest.
5. [**S&P 500 Financial Clustering (`sp500-analysis`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/sp500-analysis) — PCA dimensionality reduction + K-Means regime clustering across S&P 500 fundamentals, valuation multiples, and volatility profiles.
6. [**Cars Model Analysis (`cars-model-analysis`)**](https://github.com/ikebude/ai-ml-data-engineering/tree/main/machine-learning/cars-model-analysis) — Vehicle specification and pricing analysis.

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

- **B.Sc. Economics** — University of Nigeria, Nsukka *(Second Class Upper Division / 2:1, Sept 2017 – Nov 2022)*
- **Google Advanced Data Analytics Professional Certificate** — Coursera *(Apr 2025)*
- **Managerial Economics & Business Analysis Specialization** — Gies College of Business, UIUC *(Jun 2023)*
- **Microsoft Certified: Azure AI Engineer Associate** — *(In progress — target 2026)*


---

## Connect With Me

- **Email:** [precious.ikebude@outlook.com](mailto:precious.ikebude@outlook.com)
- **Portfolio Monorepo:** [github.com/ikebude/ai-ml-data-engineering](https://github.com/ikebude/ai-ml-data-engineering)
- **Solutions Deck (PDF):** [Precious-Ikebude-Solutions.pdf](https://github.com/ikebude/ai-ml-data-engineering/blob/main/showcase/Precious-Ikebude-Solutions.pdf)
- **Kaggle:** [kaggle.com/ikebude](https://www.kaggle.com/ikebude)
