Hi there

### 👩‍💻 About Me

Hi, I'm Qiuxia Fu. **Aspiring Data Engineer** who builds reliable data pipelines and warehouses that business teams can trust — data that arrives on time, stays correct, and is modeled for the questions people actually ask.

#### Currently:
🎓 M.Sc. in Information Systems, Stockholm University (Data Warehousing, Big Data with NoSQL, System Integration)

💼 Previously AI Project Manager at TikTok (ByteDance) — owned delivery of AI/LLM training-data pipelines across TikTok, CapCut and Lark, with 99%+ data fidelity

🔨 Building: a Databricks Lakehouse (Delta Lake · Medallion · Unity Catalog)

#### What I care about:
- Trustworthy data: tests, data-quality checks and CI so bad data is caught before anyone reports on it
- Pipelines that survive failure: incremental loads, idempotent writes, safe retries
- Modeling for the business: Kimball dimensional models with a clear grain, so analysts get consistent answers
- Knowing why something is slow: measure first, then fix the real bottleneck

---

### Featured Projects

**🛒 [Olist E-Commerce Data Warehouse](https://github.com/Qiuxia-Fu/Olist-E-Commerce-Order-Data-Warehouse) -> [Daily Incremental Pipeline](https://github.com/Qiuxia-Fu/Airflow-Orchestrated-Incremental-ETL-Pipeline)**
`dbt` `PostgreSQL` `SQL` `AirflowDocker` `GitHub Actions`

**Problem:** An e-commerce business has raw orders, customers and payments in separate tables. Analysts can't answer simple questions like "revenue by customer region over time" consistently, and when a customer moves, their history gets overwritten.

**What I built:**

- A **Kimball star schema** (10 dbt models: staging → snapshot → marts) over 99K orders, with grain and conformed dimensions defined in a bus matrix
- **SCD Type 2** on the customer dimension (dbt snapshots), so historical reports stay correct when a customer's attributes change; fixed a non-unique natural key with window-function deduplication
- **Upgrade:** turned it into a **daily incremental pipeline** orchestrated by Airflow, with watermark-based extraction and idempotent writes, so a failed run can be retried without duplicating data
- **GitHub Actions CI** runs unit tests and dbt data tests on every pull request

**🚕 [NYC Taxi PySpark Batch Pipeline](https://github.com/Qiuxia-Fu/NYC_Taxi_PySpark_Batch)**
`PySpark` `Python` `Parquet`

**Problem:** 22.5M+ trip records are too large to handle comfortably in pandas. The question was not just "use Spark" but when Spark actually helps, and what makes it slow.

**What I built:**

- A **Bronze / Silver / Gold** PySpark pipeline with data-quality filtering, broadcast joins to reference dimensions, and Hive-partitioned Parquet output
- A **benchmark against a memory-aware pandas baseline** on the same hardware. pandas won by 2.5x, and I traced the reasons: a non-splittable input format, redundant logging passes and untuned shuffle partitions, not a lack of parallelism

**📺 [YouTube Data ELT Pipeline](https://github.com/Qiuxia-Fu/YouTube-ELT)**
`Python` `Apache Airflow` `Docker` `GitHub Actions` `PostgreSQL` `pytest`

**Problem:** Channel performance data (views, likes, comments) lives behind an API and changes every day. It needs to land in a database automatically and be checked for quality before anyone uses it.

**What I built:**

- A daily ELT pipeline: YouTube Data API → PostgreSQL staging → core schema, orchestrated by **3 Airflow DAGs**
- Fully containerized with Docker Compose (Postgres, Redis, Airflow webserver, scheduler and worker)
- SODA data-quality checks plus **pytest** unit and integration tests, run in GitHub Actions CI/CD on every push

### 📂 Other Projects

- **💎 [Jewelry Retail BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMzg3NmJhZjQtMWVlNC00Yjc3LWI4NjEtMjYxYWFmYWFiOGQyIiwidCI6IjAzMTUxMzIxLWYwMDEtNDIxOC1hM2I5LTRkODM1MzgxNzRjYiJ9):** lets management see where revenue comes from (market, product, season). Star schema across multiple fact tables, an ETL pipeline and an interactive Power BI dashboard. `Power BI` `DAX` `SQL`
- **📉 [Telco Customer Churn Analysis](https://github.com/Qiuxia-Fu/Telco-Customer-Churn-Analysis):** finds which customers are most likely to leave. New customers churn at 46%, nearly 7x the rate of long-tenure customers; the top 3 risk segments were validated in SQL. `Python` `pandas` `SQL`

---

### 🧰 Tech Stack

**Languages:**
Python, SQL (PostgreSQL), dbt, Apache Airflow, Docker, SODA, pytest, GitHub Actions (CI/CD)

**Processing & Modeling:**
PySpark, dbt, pandas, Kimball dimensional modeling

**Orchestration:**
Apache Airflow

**Platform:**
Databricks

**Quality & DevOps:**
pytest, dbt tests, Docker, GitHub Actions, Git

**BI:**
Power BI, DAX

---

### 🔭 What I'm Working Toward

Data Engineer roles in Stockholm / Sweden. Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/qiuxia-fu-109736324/) or by email at rionafu1005@gmail.com.
