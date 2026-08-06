<div align="center">

# Rishav Sah

### Data Scientist (Applied AI/ML)

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&pause=1500&color=58A6FF&center=true&vCenter=true&width=560&lines=I+build+things+that+ship." alt="Typing SVG" />
</a>



<br/>

[![Email](https://img.shields.io/badge/rsah.pro@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rsah.pro@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishav-sah-b1966b190/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/rishav-sah)
![Location](https://img.shields.io/badge/Miami,_FL-Open_to_relocation-2EA043?style=for-the-badge&logo=googlemaps&logoColor=white)

</div>

---

## About

I build systems that turn messy, unstructured, multi-source information into things you can actually run analysis on — and I document where they break.

Two years of production fintech engineering at an early-stage startup, then eighteen months of graduate research at FIU's College of Business working on financial panel data, corporate disclosure NLP, and AI-assisted legal document review. The through-line is the same in both: understand the domain, reconcile the sources, validate before you conclude, and be explicit about what the data can and cannot support.

Finishing an **M.S. in Data Science (May 2026)**. Currently looking for ML / applied AI / data engineering roles where the data is difficult and the correctness bar is high.

---

## What I'm Working On

**Data & Research Assistant** — Florida International University, College of Business · *Dec 2024 – May 2026*

| | |
|---|---|
| **Cross-source panel construction** | Reconstructed a dormant FDI study from 2018 materials and assembled a **100+ country, 15-year panel** from World Bank, Bloomberg, Compustat, and WRDS — reconciling mismatched country identifiers, reporting frequencies, and coverage windows into one analysis-ready dataset. |
| **Disclosure NLP** | Firm-level textual measures on cybersecurity-risk disclosures across **640 filings** from **80 breach-linked firms** and **240 matched controls**, using normalization, vectorization, and cosine similarity — plus the methodological diagnostic separating what was computed from what the data could support. |
| **LLM failure analysis** | Diagnosed failure modes in an LLM-assisted document-review loop (run-to-run output variance, non-standardized field extraction, unverified citations) and specified the remediation architecture: schema-constrained extraction, deterministic validation, human routing for ambiguous records. |
| **Structured legal research** | A **50-state** nonprofit audit-requirements dataset from LexisNexis covering **12 fields per jurisdiction** — audit triggers, revenue thresholds and basis, effective dates, exemptions, review rules, agencies, and statutory citations. |
| **Recurring data pipelines** | Standardized a monthly minute-level FX extract across **12 currency pairs** with fixed naming conventions and completeness checks before handoff. |

<details>
<summary><b>Before this: Software Development Engineer, myPaisaa (Finsave Technologies) — Dec 2021 – Dec 2023</b></summary>

<br/>

Full-stack work at an early-stage fintech digitizing chit-fund and financial-service workflows. Angular admin portal, Ionic mobile app, Java Spring Boot services.

- Owned the frontend of the **Paid Subscriber Module** — subscriber records, document collection, verification status, disbursement — coordinating API contracts across three surfaces serving **10K registered** and **6K monthly active** users.
- Built a configurable filtering service (date ranges, subscriber and payout status, search, sort, pagination) adopted across **15+** financial reporting and payout modules, collapsing per-screen implementations into one shared component.
- Rebuilt multi-step onboarding and KYC to persist applicant state across interruptions, rejections, and pending-verification holds, so stalled applicants resumed at their last completed step.
- Instrumented the mobile app with event tracking across onboarding, KYC steps, and document submission — product's first funnel-level view of applicant drop-off.
- Handled **10–15 production tickets/week** on-call, tracing defects through client state, API contracts, and stored data.

</details>

---

## Featured Work

### 🏗️ [Telco Data Platform — OLTP → Lakehouse → Warehouse → ML](https://github.com/rishav-sah/telco-churn-data-platform)
Local end-to-end data platform: 3NF Postgres source with CDC outbox and watermarks, Spark bronze/silver with SCD2 merges and DQ quarantine, dbt star schema in the warehouse, Airflow orchestration. The churn model trained from point-in-time warehouse features reproduces the reference CSV-trained model's ranking power — **ROC-AUC 0.8477 vs 0.848, 4.6× lift at the top decile** — on independently simulated history. Phases 6 and 8 (lineage tooling, cloud IaC) are deliberately deferred and marked as such in the repo.

`Postgres` · `Spark` · `Delta` · `dbt` · `Airflow` · `MinIO` · `MLflow` · `Docker Compose`

### 🔎 [AI-Powered Investor Intelligence Platform](https://github.com/rishav-sah/AI-Powered-Investor-Intelligence-Platform)
RAG service over investor documents. Ingests annual reports, extracts KPIs with Azure OpenAI, and indexes content in Azure AI Search for semantic retrieval. Modular FastAPI backend with a PostgreSQL KPI store and insights dashboard, containerized on AKS behind an ACR CI/CD pipeline. Currently running against a three-company demo corpus; retrieval quality is not yet formally evaluated.

`Python` · `FastAPI` · `Azure OpenAI` · `Azure AI Search` · `PostgreSQL` · `Docker` · `AKS`

### 📉 [Telco Customer Churn — End-to-End ML Service](https://github.com/rishav-sah/telco-churn-app)
XGBoost churn classifier on **7,043 records / 30 features**, threshold tuned to **0.35** — lifting recall **0.74 → 0.82** at **ROC-AUC 0.84**. Training gated on **25 Great Expectations checks**, runs tracked in MLflow, served through a Pydantic-validated FastAPI `/predict` endpoint on AWS ECS Fargate.

`Python` · `XGBoost` · `MLflow` · `Great Expectations` · `FastAPI` · `Docker` · `AWS ECS`

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**ML & Modeling**

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-2B6CB0?style=flat-square)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)

**GenAI & NLP**

![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![BERT](https://img.shields.io/badge/BERT-4285F4?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-5A4FCF?style=flat-square)
![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Azure AI Search](https://img.shields.io/badge/Azure_AI_Search-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)

**MLOps & Cloud**

![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Great Expectations](https://img.shields.io/badge/Great_Expectations-FF6600?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_ECS_·_S3_·_ALB-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure_AKS_·_ACR-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-00ADD4?style=flat-square)

**Data & Serving**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-F97316?style=flat-square)

**Full-Stack — Prior Production Experience**

![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Ionic](https://img.shields.io/badge/Ionic-3880FF?style=flat-square&logo=ionic&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=flat-square)
![Google Analytics](https://img.shields.io/badge/Google_Analytics-E37400?style=flat-square&logo=googleanalytics&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Financial & Legal Data Sources**

![Bloomberg](https://img.shields.io/badge/Bloomberg_Terminal-000000?style=flat-square&logo=bloomberg&logoColor=white)
![WRDS](https://img.shields.io/badge/WRDS-011F5B?style=flat-square)
![Compustat](https://img.shields.io/badge/Compustat-1B365D?style=flat-square)
![World Bank](https://img.shields.io/badge/World_Bank-002244?style=flat-square)
![IMF](https://img.shields.io/badge/IMF-003366?style=flat-square)
![LexisNexis](https://img.shields.io/badge/LexisNexis-9B1B30?style=flat-square)
![SEC EDGAR](https://img.shields.io/badge/SEC_Filings-1F3864?style=flat-square)

---

## Education

**M.S. Data Science** — Florida International University, Miami, FL · *Aug 2024 – May 2026*

**B.Tech. Computer Science & Engineering** — KIIT University, Odisha, India · *Aug 2018 – May 2022*

---

## Let's Talk

I'm interested in roles and collaborations involving **financial and legal text extraction**, **RAG and LLM evaluation**, **panel data construction from heterogeneous sources**, and **getting models out of notebooks and behind an API**.

If you're working on any of that — or you want to compare notes on why your extraction pipeline gives you a different answer every Tuesday — reach out.

[![Email](https://img.shields.io/badge/Email_me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rsah.pro@gmail.com)
[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishav-sah-b1966b190/)

<!--
====================================================================
GITHUB STATS BLOCK — currently disabled on purpose.

These cards report *volume*, not quality. Right now your public
profile is two strong projects, so a stats card mostly advertises a
small repo count and a thin contribution history, which undercuts
everything above it.

Turn this on once you have ~6 months of consistent public commits or
5+ substantive public repos. Until then, the featured-work section
does more for you. Uncomment by deleting this comment marker and the
closing one below.

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=rishav-sah&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true" height="165" alt="GitHub stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rishav-sah&layout=compact&theme=github_dark&hide_border=true&langs_count=8" height="165" alt="Top languages" />

<br/>

<img src="https://streak-stats.demolab.com?user=rishav-sah&theme=github-dark&hide_border=true" alt="GitHub streak" />

</div>
====================================================================
-->

<div align="center">

<br/>

![Profile views](https://komarev.com/ghpvc/?username=rishav-sah&label=Profile%20views&color=58A6FF&style=flat-square)

<sub>M.S. Data Science, May 2026 · Miami, FL · Open to relocation</sub>

</div>
