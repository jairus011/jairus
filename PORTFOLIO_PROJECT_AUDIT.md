# Portfolio Project Audit — September 2026

This file is the control panel for Jairus Omondi's GitHub portfolio.

Its purpose is to answer five questions for every project:

1. What does the project do?
2. What currently works?
3. Is it deployed?
4. Does it use an API?
5. What should be improved next?

## Portfolio priority

### Flagship projects

#### 1. financial-fraud-detection-dashboard
Status: Strong flagship
Deployment: Live on Render
API: No external API. Local model inference inside the Streamlit application.
Why it matters: Best current end-to-end fraud project: ETL, supervised modelling, anomaly detection, saved artifacts, tests, reproducibility, dashboard and deployment.
Portfolio action: Keep public and feature prominently.

#### 2. credit-risk-prediction
Status: Strong banking ML project
Deployment: Not currently deployed
API: None
Why it matters: Shows credit-risk modelling, preprocessing, model comparison and business interpretation.
Portfolio action: Keep public and feature prominently. A lightweight prediction UI may be worthwhile later, but deployment is not mandatory until the model pipeline is packaged cleanly.

#### 3. banking-sql-analytics
Status: Strong SQL/business analytics project
Deployment: Not required
API: None
Why it matters: Shows relational modelling, SQL querying, CTEs, views, window functions and banking-oriented reporting.
Portfolio action: Keep public and feature prominently. Do not force a web deployment just to say it is deployed.

#### 4. project-foresight-demand-inventory-intelligence
Status: Good collaborative data-science project
Deployment: Render service created; deployment troubleshooting in progress
API: None. Streamlit reads committed project outputs.
Why it matters: Demonstrates forecasting, inventory risk scoring, business decision support and collaboration.
Portfolio action: Keep public. Verify hosted deployment before adding a live badge/link.

#### 5. fraud-detection-portfolio
Status: Strong ML case study
Deployment: Not required in current form
API: None
Why it matters: Strong evidence of imbalanced classification and fraud-specific evaluation.
Portfolio action: Keep public and feature after the newer fraud dashboard.

#### 6. medicare-lab
Status: Technically strong but model performance is intentionally disclosed as poor
Deployment: Live on Render
API: None
Why it matters: Demonstrates reproducibility, testing, deployment and responsible ML reporting.
Portfolio action: Keep public, but do not position it above the banking/fraud projects.

## Secondary / progression projects

### banking-fraud-detection
Status: Older fraud project upgraded with Streamlit batch inference
Deployment: Render service created; deployment troubleshooting in progress
API: None
Portfolio action: Keep as evidence of progression, but the newer financial-fraud-detection-dashboard should remain the flagship fraud project.

### Bank-Marketing-dataset
Status: Notebook-based learning project
Deployment: Not needed
API: None
Portfolio action: Keep public but unpinned. Consolidate notebooks and verify metrics before any further promotion.

### toxicity-classification-project
Status: Notebook-based learning project
Deployment: Not needed
API: None
Portfolio action: Keep public but unpinned. Clean filenames and package training before considering any app.

### World-Population-Growth
Status: Early exploratory analysis
Deployment: Not needed
API: None
Portfolio action: Keep as learning history or archive later. It should not be pinned.

### portfolio-website
Status: Legacy static portfolio repository
Deployment: Superseded by the newer Vercel portfolio
API: None
Portfolio action: Do not feature. Consider archiving after confirming no links depend on it.

## What "API integrated" means

Not every project needs an API.

An API is useful when another application needs to send data to the model or retrieve results programmatically. For example:

- a frontend sends a loan application to a FastAPI endpoint
- an internal bank system sends a transaction for fraud scoring
- a dashboard fetches predictions from a backend service

A Streamlit app that loads a local model is not an API integration.

Do not add APIs merely to make a project look more advanced. Add one when it improves the architecture or demonstrates a real service boundary.

## Deployment rule

Deploy projects when the deployment adds portfolio value.

Good candidates:
- interactive Streamlit applications
- dashboards
- model demos
- APIs
- full-stack applications

Usually not worth deploying:
- SQL-only repositories
- exploratory notebooks
- static analysis notebooks
- projects without a stable inference workflow

## Documentation standard for every serious project

Every flagship repository should eventually contain:

- README.md — public project story
- PROJECT_STATUS.md — current truth about what works
- requirements.txt or equivalent environment definition
- .gitignore
- reproducible code or notebooks
- model/evaluation documentation where relevant
- screenshots for apps/dashboards
- deployment instructions if deployable
- API section explicitly saying whether an API exists
- limitations section
- next steps

## Current deployment inventory

Verified live:
- financial-fraud-detection-dashboard — Render
- medicare-lab — Render

Created but not yet verified live:
- banking-fraud-detection — Render
- project-foresight-demand-inventory-intelligence — Render

Not intentionally deployed:
- credit-risk-prediction
- fraud-detection-portfolio
- banking-sql-analytics
- Bank-Marketing-dataset
- toxicity-classification-project
- World-Population-Growth

## Cleanup order

1. Verify/fix the two new Render deployments
2. Add PROJECT_STATUS.md to all flagship repositories
3. Shorten and polish long/duplicated READMEs
4. Add deployment links only after live verification
5. Add screenshots to deployed apps
6. Package credit-risk inference cleanly before deciding whether to deploy it
7. Standardize repository descriptions and pinned projects
8. Archive or de-emphasize legacy projects only after confirming they are no longer needed
