<p align="center">
	<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Duan%20Nguyen%20Duy&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Analytics%20Engineer%20%7C%20SQL%20%7C%20Power%20BI%20%7C%20Airflow&descAlignY=58&descSize=18" alt="banner" />
</p>

<h1 align="center">Hello, I'm Duan Nguyen Duy 👋</h1>

<p align="center">
	Ho Chi Minh City
</p>

<p align="center">
	<a href="https://readme-typing-svg.demolab.com">
		<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=2F81F7&center=true&vCenter=true&width=760&lines=Analytics+Engineer+%40+Merkle+CXM;SQL+%7C+Power+BI+%7C+Data+Modelling;Airflow+%7C+PostgreSQL+%7C+Salesforce+Marketing+Cloud;Turning+customer+data+into+actionable+insights" alt="Typing SVG" />
	</a>
</p>

<p align="center">
	<a href="https://www.linkedin.com/in/duannguyen2606/"><img src="https://img.shields.io/badge/LinkedIn-duannguyen2606-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
	<a href="mailto:duannguyen2606@gmail.com"><img src="https://img.shields.io/badge/Email-duannguyen2606@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
	<a href="https://duan-n2d.github.io/"><img src="https://img.shields.io/badge/Portfolio-duan--n2d.github.io-181717?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio" /></a>
	<img src="https://komarev.com/ghpvc/?username=duan-n2d&label=Profile+views&color=2f81f7&style=for-the-badge" alt="Profile views" />
</p>

---

## 🧑‍💻 About Me
Analytics Engineer with 2+ years turning raw marketing, sales, and call-center data into reconciled datasets, data marts, and semantic layers. I defined the Lead → Call → Order funnel for operations and strategy teams, built layered views for 15+ enterprise clients at Antsomi, and created a Claude MCP semantic layer used daily by 10+ people. I combine strong SQL, data quality, and Power BI skills with the engineering depth to run the pipelines behind analytics.

## 🔄 Analytics Data Flow

```mermaid
flowchart LR
    A[(Marketing, Sales<br/>and Call Data)] --> B[Airflow<br/>Ingestion & Quality]
    B --> C[(PostgreSQL DWH)]
    C --> D[Layered Models<br/>Raw → Marts]
    D --> E[Metrics &<br/>Semantic Layer]
    D --> F[Power BI<br/>Lead → Call → Order]
    E --> G[Claude MCP<br/>Aggregate Questions]
    C <--> H[Salesforce<br/>Marketing Cloud]
```

## 💼 Experience

### 🚀 Junior Data Engineer | Dentsu – Merkle CXM
`September 2025 – Present`
- Defined and delivered the **Lead → Call (contacted) → Order (completed / cancelled) funnel** in Power BI with five-minute refreshes, joined on phone and uid, replacing Excel reporting for operations, agent management, and strategy teams.
- Built a **Claude MCP semantic layer** on the data warehouse after a Hugging Face LLM prototype. Documented tables, columns, types, metrics, and relationships; created one source-of-truth dataset per entity, aggregation tools, per-user session IDs and secret-based access, and a 12-month query limit. Used daily by 10+ people.
- Embedded SQL and Python data-quality checks in Airflow for source-to-target row counts, null and duplicate keys, freshness, and aggregate reconciliation.
- Built and operate **10–20 bidirectional Salesforce Marketing Cloud integrations** with databases, APIs, and SFTP using Airflow, Python, and Automation Studio. Implemented incremental loads by timestamp or ID, duplicate-safe insert/upsert/overwrite, retries, and alerts.
- Sole owner of a **lead-distribution platform** from design through monitoring, serving 8 teams / ~200 agents across ~100 campaigns and processing ~600k leads and ~1M call records monthly. A Next.js app and Python scheduler use agents' last-three-day call performance while balancing distribution, then send real-time ZNS notifications. Replaced manual Excel assignment, reducing hours-long delays, duplicate/missed leads, and staff standby; setup is done once at the start of each month.
- Designed the data flow from a day-partitioned call-center database to a **PostgreSQL DWH**, with Airflow DAGs running every 30 minutes to weekly.
- Enabled campaign users to ask ad-hoc aggregate questions in natural language against raw tables, reducing one-off dashboard requests.
- Run Airflow projects in Docker with GitHub/GitLab version control and GitHub Actions CI/CD.

### 📊 Data Analyst | Antsomi Co., Ltd
`October 2024 – September 2025`
- Built layered views (raw → intermediate → small data marts) for 15+ enterprise clients, including PNJ, AEON Mall, Mega Market, Highland Coffee, and ACFC, turning partitioned source data into analysis-ready datasets across fashion, retail, F&B, e-commerce, and education.
- Reconciled source-to-platform and raw-to-dashboard data; resolved primary-key mismatches by enforcing one profile per phone and labelling secondary numbers.
- Delivered ~10 Power BI report types across fashion, retail, F&B, e-commerce, and education, including sales, journey performance, demographics, RFM, association rules, and site tracking.
- Optimized SQL over 30M+ records per month with partition pruning, column selection, early filtering, pre-aggregation, and CTEs to temp tables, **cutting processing time 2–3×**.
- Integrated 3–5 POS, e-commerce, CRM, and loyalty sources per client through APIs, SFTP, and databases, mapping data to a reusable standard schema.
- Implemented Antsomi CDP 365 solutions and audience segments; clients used RFM clusters to target campaigns and association rules to design product bundles. Automated routine data tasks with Python, increasing team efficiency by 25%, and provided client training and technical support.

### 🧩 Developer Intern | ISONICX Solution Co., Ltd
`October 2022 – December 2023`
- Designed Salesforce data models with SOQL and developed and tested Lightning Web Components (LWC).

## 🛠️ Skills

- **Analytics engineering:** SQL tuning, window functions, CTEs, dimensional and layered modelling, metric definitions, documentation, semantic layers, reconciliation, data quality, Power BI
- **Engineering:** Python, Airflow, PostgreSQL, incremental/idempotent loading, API/SFTP/database integration, Salesforce Marketing Cloud, GitHub/GitLab, Docker, GitHub Actions CI/CD
- **Familiar:** dbt, PySpark, Azure Data Factory, Databricks, Synapse, Microsoft Fabric

## 🚀 Featured Projects

| Project | What it shows | Stack |
|---|---|---|
| [**OpenLake Commerce Platform**](https://github.com/duan-n2d/openlake-commerce-platform) | Open-source streaming lakehouse: Postgres CDC → Kafka → Flink → Iceberg, dbt marts, quality gates, lineage, BI and API | Debezium, Kafka, Flink, Iceberg, Trino, dbt, Dagster, Great Expectations |
| [**Elite Football DecisionOps Lakehouse**](https://github.com/duan-n2d/elite-football-club-decisionops-lakehouse) | Stakeholder-driven lakehouse with governed Gold data products, API, dashboard, and an AI copilot with SQL guardrails | Python, Spark/Delta, FastAPI, Streamlit, Databricks, Terraform |
| [**WorldCup Pulse**](https://github.com/duan-n2d/worldcup-pulse) | $0 serverless near-real-time pipeline: incremental medallion ETL, HF Dataset storage, BI and DataOps apps | GitHub Actions, Cloudflare Workers, DuckDB, Streamlit |
| [**Dylxn Assistant**](https://github.com/duan-n2d/dylxn-assistant) | Local-first RAG assistant over a Markdown data-engineering knowledge base | Python, Qdrant, E5 embeddings, Ollama, FastAPI |
| [**Azure End-to-End DE**](https://github.com/duan-n2d/Azure-End-to-End-Data-Engineering-Solution) | On-prem SQL Server → ADLS medallion lakehouse → Synapse → Power BI | ADF, Databricks, Delta Lake, Synapse, Key Vault |
| [**Analytics Case Studies**](https://github.com/duan-n2d/analytics-case-studies) | BI dashboards, RFM segmentation, ML experiments, and Data Got Talent 2024 submissions | Power BI, SQL, Python |

**Learning & research:** [AI-Augmented DE Roadmap](https://github.com/duan-n2d/learning-data-platform) · [Modern Data Stack deck](https://duan-n2d.github.io/modern-data-stack/) · [Churn prediction with time-series classification](https://github.com/duan-n2d/Predicting-customers-churn-using-time-series-classification) (MINIROCKET, LSTM — 95% accuracy, F1 79%)

## 🏅 Leadership

- **Software Team Leader, ITB Club (2021–2024):** led two Business Intelligence competitions (Seasons 6 and 7), delivered two data analysis and BI workshops for 5,000+ students, and built Power BI dashboards to track program metrics.
- **Subject Matter Advisor, BI Competition Season 9 (2025):** mentored student teams on methodology, dashboards, and data storytelling.

## 📜 Certifications

Microsoft DP-700 Fabric Data Engineer · DP-800 SQL AI Developer · Salesforce Data Cloud Consultant · Google Cloud Digital Leader

## 🎓 Education

**B.Sc. Management Information Systems** | University of Economics and Law, VNU-HCM `2021 – 2025`

Prospect Award, Data Got Talent 2023 · Full scholarship, VietSeeds Foundation (2021–2025)
<br>
[Google Business Intelligence Professional Certificate](https://coursera.org/share/b049321d82e58dbc2395ef1b6bdbd2a2) `April 2024 – May 2024`

## 📈 GitHub Stats

<p align="center">
	<img height="170" src="https://github-readme-stats.vercel.app/api?username=duan-n2d&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
	<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=duan-n2d&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

<p align="center">
	<img src="https://streak-stats.demolab.com?user=duan-n2d&theme=tokyonight&hide_border=true" alt="GitHub streak" />
</p>

<p align="center">
	<img src="https://github-readme-activity-graph.vercel.app/graph?username=duan-n2d&theme=tokyo-night&hide_border=true&area=true" alt="Contribution graph" />
</p>

## 🏆 GitHub Trophy

<p align="center">
	<img src="https://github-profile-trophy.vercel.app/?username=duan-n2d&theme=flat" alt="GitHub Profile Trophy" />
</p>

## 🐍 Contribution Snake

<p align="center">
	<picture>
		<source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/duan-n2d/duan-n2d/output/github-snake-dark.svg" />
		<source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/duan-n2d/duan-n2d/output/github-snake.svg" />
		<img alt="Contribution snake" src="https://raw.githubusercontent.com/duan-n2d/duan-n2d/output/github-snake.svg" />
	</picture>
</p>

## 🤝 Let's Connect
- LinkedIn: [duannguyen2606](https://www.linkedin.com/in/duannguyen2606/)
- Email: [duannguyen2606@gmail.com](mailto:duannguyen2606@gmail.com)
- Portfolio: [duan-n2d](https://duan-n2d.github.io/)

<p align="center">
	<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer" alt="footer" />
</p>
