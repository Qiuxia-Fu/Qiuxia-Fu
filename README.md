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

**[NYC Taxi PySpark Batch Pipeline](https://github.com/Qiuxia-Fu/NYC_Taxi_PySpark_Batch)**
`PySpark` `Python` `Parquet`

Bronze/Silver/Gold batch pipeline processing 22.5M+ NYC taxi trip records with broadcast joins,
data-quality gating, and Hive-partitioned Parquet output — benchmarked against a memory-aware
pandas baseline and diagnosed a counter-intuitive result (pandas outperformed local-mode Spark)
down to its root causes.

**[Olist E-Commerce Order Data Warehouse](https://github.com/Qiuxia-Fu/Olist-E-Commerce-Order-Data-Warehouse)**
`dbt` `PostgreSQL` `SQL` `Docker`

Kimball star schema (10 dbt models, staging → snapshot → marts) for a 99K-order e-commerce
dataset, with SCD Type 2 on the customer dimension and 7 dbt tests enforcing data integrity.
Later extended with an Airflow-orchestrated incremental loading layer
([see upgrade](https://github.com/Qiuxia-Fu/Airflow-Orchestrated-Incremental-ETL-Pipeline)).

**[YouTube Data ELT Pipeline](https://github.com/Qiuxia-Fu/YouTube-ELT)**
`Python` `Apache Airflow` `Docker` `GitHub Actions` `pytest`

End-to-end ELT pipeline orchestrated by 3 daily Airflow DAGs, fully containerized via Docker
Compose, with automated data-quality checks (SODA) and a CI/CD pipeline running the full test
suite on every push.

### 📂 Other Projects

More projects — including an incremental-loading upgrade to the Olist warehouse and an earlier
churn/EDA analysis — are in [my repositories →](https://github.com/Qiuxia-Fu?tab=repositories)

---

### 🧰 Tech Stack

**Data Engineering:**
Python, SQL (PostgreSQL), dbt, Apache Airflow, Docker, SODA, pytest, GitHub Actions (CI/CD)

**Data & BI:**
pandas, Power BI (DAX), Excel

**Tools:**
Git, VS Code

---

### 🔭 What I'm Working Toward

Building reliable, tested, production-style data pipelines — bringing the same rigor I used to bring to delivery management (clear requirements, measurable quality, process discipline) to the pipelines themselves.

Open to Data Engineer / Analytics Engineer roles in Stockholm, Sweden.
