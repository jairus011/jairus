# Portfolio Project Audit — September 2026

This file is a private working guide for Jairus Omondi's GitHub portfolio. It records what each repository is, whether it needs deployment, whether it uses an API, what is already working, and what should be improved next.

## Portfolio strategy

The goal is not to make every repository look identical. Different projects should prove different skills:

- **Interactive applications** should have a live deployment, clear setup instructions, input validation, and a visible limitations section.
- **Machine-learning case studies** should emphasize reproducible evaluation, metrics, preprocessing, and business interpretation. They do not need a web deployment unless an interface adds real value.
- **SQL/data-analysis projects** should emphasize schema design, queries, insights, and reproducibility. A deployment is optional.
- **Older learning projects** should either be cleaned up and clearly labelled as learning work or left unpinned so they do not distract from stronger projects.

## Project inventory

| Repository | Current role | Deployment | API integration | Portfolio decision |
|---|---|---|---|---|
| financial-fraud-detection-dashboard | End-to-end fraud ML application | Live on Render | No external API; local ML pipeline + SQLite | Keep as a flagship project |
| credit-risk-prediction | Credit-risk ML case study | Not required today | None | Keep as a flagship modelling project |
| fraud-detection-portfolio | Imbalanced fraud classification case study | Not required today | None | Keep; strong evidence of fraud-model evaluation |
| banking-sql-analytics | Banking SQL/database project | Not required | None | Keep; proves SQL and relational modelling |
| project-foresight-demand-inventory-intelligence | Forecasting + inventory decision dashboard | Deployment candidate | None | Upgrade README/dashboard and deploy |
| banking-fraud-detection | Older fraud model + Streamlit batch app | Deployment candidate | None | Repair runtime, improve app/README, deploy |
| medicare-lab | Educational healthcare ML prototype | Render-ready; live status to verify | None | Keep unpinned unless needed; model performance is intentionally documented as weak |
| toxicity-classification-project | Older ML learning project | No deployment needed | None | Clean documentation later; keep unpinned |
| World-Population-Growth | Exploratory analysis project | No deployment needed | None | Fix placeholder README values or keep unpinned |
| Bank-Marketing-dataset | Older marketing ML coursework/project | No deployment needed | None | Clean structure/documentation later; keep unpinned |
| portfolio-website | Older static portfolio | Separate from current portfolio | None | Do not feature if the newer portfolio is the active site |

## API notes

At the time of this audit, the reviewed public projects do **not** depend on an external third-party API. Their main runtime patterns are local model inference, CSV/SQLite data, Streamlit interfaces, SQL, and notebook analysis.

That is not a weakness. An API should be added only where it improves the architecture. If a later project exposes model predictions to another application, a FastAPI service would be appropriate and should then be documented explicitly.

## Current flagship set

The strongest public story is:

1. Financial Fraud Detection Dashboard — end-to-end ML application and deployment
2. Credit Risk Prediction — lending-risk modelling
3. Fraud Detection Portfolio — severe class imbalance and fraud metrics
4. Banking SQL Analytics — database and SQL skills
5. Project Foresight — forecasting, inventory intelligence, and dashboard
6. One additional project chosen for the job being targeted

## Maintenance rule

Every upgraded project should contain a `PROJECT_STATUS.md` file answering:

- What problem does this project solve?
- What is working now?
- How do I run it?
- Is it deployed? Where?
- Does it use an API?
- What data/model limitations matter?
- What was changed in the portfolio cleanup?
- What would I build next?

This makes it easy to return to an old project months later without having to rediscover its architecture.
