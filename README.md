Hi there

### 👩‍💻 About Me

Hi, I'm Qiuxia Fu (also feel free to call me Riona) — a data-driven professional transitioning from AI/data project management into Data Engineering.

I spent 3+ years managing the delivery side of AI/data pipelines (annotation, model training data, quality standards) without touching the pipelines myself — now I'm building them directly: ELT pipelines, orchestration, containerization, automated data quality and CI/CD.

- 🎓 M.Sc. in Information Systems, Stockholm University 
- 💼 Previously AI Project Manager at TikTok (ByteDance), managing end-to-end delivery of AI/LLM training data across TikTok, CapCut and Lark
- 🔍 Particularly interested in data pipeline engineering, workflow orchestration and data quality automation
- 📊 Comfortable bridging delivery/process thinking with hands-on engineering — from requirements to production-ready pipelines
- 📫 Reach me via GitHub or [LinkedIn](https://www.linkedin.com/in/qiuxia-fu-109736324/)

---

### ⭐ Featured Projects

**[YouTube Data ELT Pipeline](https://github.com/Qiuxia-Fu/YouTube-ELT)**
`Python` · `PostgreSQL` · `Apache Airflow` · `Docker` · `SODA` · `pytest` · `GitHub Actions`

An end-to-end ELT pipeline extracting YouTube video metadata and turning it into query-ready, quality-checked data.

- Built an ELT pipeline extracting video-level metadata (views, likes, comments, duration, upload date) via the YouTube Data API, loading raw data into a PostgreSQL staging schema and transforming it into a core schema
- Orchestrated the pipeline with 3 Apache Airflow DAGs on a daily schedule, running fully containerized via Docker Compose (Postgres, Redis, Airflow webserver/scheduler/worker)
- Implemented automated data quality checks with SODA and unit/integration tests with pytest, wired into a GitHub Actions CI/CD pipeline that builds/pushes the Docker image and runs the test suite on every push

**[Olist E-Commerce Order Data Warehous](https://github.com/Qiuxia-Fu/Olist-E-Commerce-Order-Data-Warehouse)** | `Python` · `PostgreSQL` · `dbt` · `Docker` · `Git`)

A Kimball-style dimensional data warehouse built on a 99K-order Brazilian e-commerce dataset, with SCD Type 2 tracking on the customer dimension.

- Designed a star schema (10 dbt models across staging → snapshot → marts layers) from a 99K-order, 96K-customer dataset, defining business process, grain, and conformed dimensions via an enterprise bus matrix
- Implemented SCD Type 2 on the customer dimension using dbt snapshots, resolving a non-unique natural key issue via window-function deduplication; validated with a before/after historical comparison
- Enforced data integrity with 7 dbt tests (not_null, unique, relationships) across staging and mart models, all passing; auto-generated model documentation and lineage graph via dbt docs
- Containerized the full stack (PostgreSQL) with Docker Compose for one-command reproducibility

**Business Intelligence Dashboard Project**
`Power BI` · `DAX` · `SQL` · `Excel`

An end-to-end BI solution for a multinational jewelry retail dataset. [View dashboard](https://app.powerbi.com/view?r=eyJrIjoiMzg3NmJhZjQtMWVlNC00Yjc3LWI4NjEtMjYxYWFmYWFiOGQyIiwidCI6IjAzMTUxMzIxLWYwMDEtNDIxOC1hM2I5LTRkODM1MzgxNzRjYiJ9)

- Designed a star schema data model with conformed dimensions across multiple fact tables
- Built an ETL pipeline to clean, transform and load raw retail data into the dimensional model
- Delivered an interactive Power BI dashboard tracking global revenue, product performance and seasonal trends

**[Telco Customer Churn Analysis](https://github.com/Qiuxia-Fu/Telco-Customer-Churn-Analysis)**
`Python` · `SQL` · `Pandas`

An end-to-end churn analysis on a telecom customer dataset.

- Analyzed a 7,000-customer dataset to identify key churn drivers (27% overall churn rate)
- Built a tenure-based segmentation showing new customers churn at nearly 7x the rate of long-tenure customers
- Used SQL (window functions, CASE WHEN) to validate findings and surface the top 3 highest-risk segments

---

### 🧰 Tech Stack

**Data Engineering**
Python, SQL (PostgreSQL), dbt, Apache Airflow, Docker, SODA, pytest, GitHub Actions (CI/CD)

**Data & BI**
pandas, Power BI (DAX), Excel

**Tools**
Git, VS Code

---

### 🔭 What I'm Working Toward

Building reliable, tested, production-style data pipelines — bringing the same rigor I used to bring to delivery management (clear requirements, measurable quality, process discipline) to the pipelines themselves.

Open to Data Engineer / Analytics Engineer roles in Stockholm, Sweden.
