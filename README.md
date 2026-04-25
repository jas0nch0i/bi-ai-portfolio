# Jason Choi | Business Intelligence, Analytics & AI Portfolio

<p align="left">
  <img src="https://img.shields.io/badge/Power%20BI-Business%20Intelligence-blue" />
  <img src="https://img.shields.io/badge/SQL-Analytics-blue" />
  <img src="https://img.shields.io/badge/Databricks-Data%20Modeling-blue" />
  <img src="https://img.shields.io/badge/AI%20Automation-Workflow%20Optimization-blue" />
  <img src="https://img.shields.io/badge/Executive%20Reporting-Decision%20Support-blue" />
</p>

Business intelligence, reporting, and AI-enabled automation projects focused on turning complex data into clear decisions, scalable workflows, and measurable business value.

---

> [!IMPORTANT]
> This portfolio highlights real-world BI, analytics, and automation work designed for executive visibility, KPI design, operational reporting, and AI-assisted process improvement.

## Overview

I build analytics solutions that help organizations improve visibility, streamline reporting, and make better decisions.

My work sits at the intersection of:
- Business intelligence and dashboard design
- KPI frameworks and performance reporting
- Data modeling and reporting infrastructure
- Reporting automation and workflow optimization
- AI-assisted analytics and decision support

---

## Core Focus Areas

| Area | Focus |
|---|---|
| **Business Intelligence** | Executive dashboards, operational reporting, KPI design |
| **Analytics Engineering** | SQL, Databricks, data modeling, reporting structure |
| **Automation** | Reporting workflows, repeatable processes, efficiency gains |
| **AI Enablement** | Prompt engineering, AI-assisted reporting, workflow acceleration |
| **Decision Support** | Business-facing insights, stakeholder reporting, operational clarity |

---

> [!NOTE]
> This portfolio is designed for recruiters, hiring managers, and collaborators who want to quickly understand how I approach reporting, analytics, automation, and business problem-solving.

## Featured Projects

### [1. Executive Dashboard Case Study](https://github.com/jas0nch0i/executive-operations-dashboard-case-study)
**Leadership-ready reporting for visibility, KPI tracking, and decision support**

A case study showing how fragmented operational data can be structured into clear dashboards, reporting logic, and executive-level decision support.

**What this project demonstrates**
- KPI design and business framing
- Dashboard structure for leadership use
- Reporting clarity and usability
- Operational performance visibility

---

### [2. AI-Assisted PowerBI Workflow](https://github.com/jas0nch0i/ai-assisted-powerbi-workflows)
**A practical framework for accelerating report development and iteration with AI**

This project demonstrates how AI can support dashboard prototyping, documentation, logic refinement, and repeatable BI workflow improvement.

**What this project demonstrates**
- AI-assisted dashboard development
- Documentation and process standardization
- Faster report iteration and refinement
- Practical use of prompt engineering in analytics workflows

---

### [3. Reporting Automation Toolkit](https://github.com/jas0nch0i/reporting-automation-toolkit)
**Reusable automation patterns for Power BI deployment, measure generation, theming, and documentation**

A toolkit of Python and TMDL-based automation patterns that compress recurring reporting work — measure authoring, theme application, semantic-model documentation, and PBIP deployment — into repeatable, version-controlled workflows.

**What this project demonstrates**
- Power BI deployment automation via PBIP / TMDL / Git
- Batch DAX measure generation from structured input (CSV → TMDL)
- Schema-validated theme JSON generation with structural color tokens
- Semantic-model documentation auto-generated from TMDL files
- Workflow orchestration with AI-assisted measure naming and description drafting

**Tech stack:** Python · pandas · Jinja2 · TMDL · PBIP · Power BI Desktop · Ajv (JSON Schema validation) · GitHub Actions

**Pilot results (framework targets, validated on internal pilot builds):**
- Dashboard deployment cycles reduced from ~6 close-reopen rounds to **2-3** through coordinate-table layout planning
- Measure authoring throughput **~5x faster** for batches of 15+ measures via templated generation
- Theme refresh on 30-visual report: **2 hours → 5 minutes** by switching to structural color tokens
- Semantic-model documentation generated in **<5 minutes** per model (previously a manual half-day exercise)

**Visuals**
- [Deployment workflow diagram](https://github.com/jas0nch0i/reporting-automation-toolkit/blob/main/images/01-deployment-pipeline.png)
- [Measure batch-generation flow](https://github.com/jas0nch0i/reporting-automation-toolkit/blob/main/images/02-measure-generation-flow.png)
- [Documentation auto-pipeline](https://github.com/jas0nch0i/reporting-automation-toolkit/blob/main/images/03-doc-auto-pipeline.png)
- [Before / after — themed dashboard](https://github.com/jas0nch0i/reporting-automation-toolkit/blob/main/images/04-theme-before-after.png)

---

### [4. Customer Segmentation Analysis](https://github.com/jas0nch0i/customer-segmentation-analysis)
**RFM segmentation, k-means clustering, and supervised churn classification on public retail data**

An end-to-end segmentation case study using the UCI Online Retail II dataset. RFM (Recency, Frequency, Monetary) features feed an unsupervised k-means clustering pipeline that surfaces five customer segments with distinct value and engagement profiles. A supplementary supervised-learning track trains a gradient-boosted classifier on the IBM Telco Churn dataset to predict at-risk customers and quantify driver importance.

**What this project demonstrates**
- Feature engineering for customer analytics (RFM, recency decay, monetary log-scaling)
- Unsupervised segmentation with k-means + elbow / silhouette validation
- Persona development translating cluster centroids into business-readable archetypes
- Supervised classification (Gradient Boosting / XGBoost) with calibrated probability outputs
- Model evaluation: confusion matrix, ROC / AUC, feature importance
- Business interpretation: segment-targeted retention and cross-sell recommendations

**Tech stack:** Python · pandas · scikit-learn · XGBoost · matplotlib · seaborn · Jupyter · Power BI (segment dashboard layer)

**Datasets (public)**
- [UCI Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii) — UK online retailer, ~1M transactions (2009–2011)
- [IBM Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) — 7,043 telecom customers with churn labels

**Sample results (5-cluster solution on bundled synthetic-retail dataset; structure mirrors UCI Online Retail II)**
- 5 segments identified: *Champions · Loyal Customers · At-Risk Spenders · New Casuals · Hibernating*
- Top segment (*Champions*) — 11% of customers, 37% of revenue
- Top 2 segments combined — 35% of customers, 68% of revenue
- Silhouette score: **0.55** (k=5)

**Sample results (gradient-boosted churn model on bundled synthetic Telco-like dataset)**
- ROC AUC: **0.77**
- Recall on churn class: **0.92** (threshold tuned for retention focus list)
- Top 3 features by importance: contract type (multi-year = protective), monthly + total charges, tenure
- Pipeline reproducible on real IBM Telco dataset — typical real-data ROC AUC ≈ 0.84

**Visuals**
- [RFM distribution](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/01-rfm-distribution.png)
- [Elbow & silhouette validation](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/02-elbow-silhouette.png)
- [Cluster scatter (PCA-projected)](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/03-cluster-scatter.png)
- [Segment persona heatmap](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/04-persona-heatmap.png)
- [Churn confusion matrix](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/05-churn-confusion.png)
- [Churn ROC curve](https://github.com/jas0nch0i/customer-segmentation-analysis/blob/main/images/06-churn-roc.png)

---

## What This Portfolio Shows

✅ Ability to translate business needs into analytics solutions
✅ Executive and operational reporting design
✅ KPI development and performance measurement
✅ Workflow improvement through automation
✅ Practical use of AI in reporting and analytics
✅ Machine learning for segmentation and prediction
✅ Clear communication between technical and business audiences

---

## Current Direction

I am currently building portfolio work centered on:
- Operational performance dashboards
- KPI and performance reporting
- AI-assisted BI development workflows
- Reporting automation and decision-support tools
- Customer analytics and segmentation

---

> [!TIP]
> Where needed, projects may use sample, recreated, or masked data to protect confidentiality while still demonstrating structure, logic, and business value.

## Connect

- 🔗 [LinkedIn](https://www.linkedin.com/in/jas0n-ch0i/)
- 📧 [Email me](mailto:jchoi815@gmail.com)
