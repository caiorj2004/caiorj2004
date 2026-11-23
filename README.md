# Hi, I'm Caio

Data Science & AI student at **IESB**, finishing my B.S. in Data Science and Artificial Intelligence. I build reproducible analytics pipelines, interactive dashboards and ML systems, with a focus on public data and territorial analysis.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Caio_Rosendo_J%C3%A1come-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/caio-rosendo-j%C3%A1come-69037a295)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face-caiorj2004-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/caiorj2004)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--5451--7975-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0001-5451-7975)

---

## Featured projects

### [pdad_tipologia_cluster](https://github.com/caiorj2004/pdad_tipologia_cluster): Typology of rural territories in the Federal District (Brazil)
My undergraduate thesis. A socioeconomic typology of rural territories built from the **PDAD Rural 2022** survey (5,075 households, 66,540 households after sample expansion), grouped into 49 region × subpopulation segments.
- Pipeline of 29 Python scripts: data auditing, weighted exploratory analysis, PCA by dimension (Monte Carlo parallel analysis) and K-Means (K = 3).
- Stability and structure checks: bootstrap against a null model, leave-one-out by region and by subpopulation, spatial statistics (Moran's I, join counts).
- Fully reproducible with a single command, MIT-licensed and archived on Zenodo ([DOI 10.5281/zenodo.24373560](https://doi.org/10.5281/zenodo.24373560)).
- `Python` · `pandas` · `scikit-learn` · `statsmodels` · `GeoPandas` · `libpysal / esda`

### [prototipo_tcc](https://github.com/caiorj2004/prototipo_tcc): Territorial intelligence platform for family farming
A multi-page analytics app in pure Python that cross-references **6 public data sources** on family farming in the DF: Agricultural Census 2017, IBGE 2024, CNPO (organic producers), CAF/MDA, rural credit (Central Bank) and PDAD Rural 2022. It also exposes the results of my thesis.
- Dash + Plotly front end, per-source pandas pipelines with `@lru_cache`, CSV export on every chart.
- Docker (Gunicorn, non-root user, healthcheck), Parquet via Git LFS, pytest smoke tests and CI on GitHub Actions.
- [Live on Hugging Face Spaces](https://huggingface.co/spaces/caiorj2004/prototipo_tcc)
- `Python` · `Dash` · `Plotly` · `Docker` · `Tailwind CSS`

### [aih_sus](https://github.com/caiorj2004/aih_sus): Dashboard and AI assistant for Brazilian public-health data (SUS)
Streamlit dashboard and a text-to-SQL AI assistant for hospital procedure data from the SUS hospital information system (AIH/SIH, DATASUS), covering 25 months for every municipality in Brazil.
- End-to-end pipeline: async scraping of the TabNet legacy system with Playwright, SQLite staging, strongly typed load into PostgreSQL.
- Diagnosed and fixed out-of-memory crashes on Streamlit Cloud by moving the app to read-only DuckDB over Parquet: the full country (139k rows) now loads in ~3 s within 1 GB.
- LangChain agent with tool calling (Groq, AWS Bedrock optional): read-only SQL guardrails, per-session limits, the executed SQL shown with every answer, and interactions logged to PostgreSQL for auditing.
- pytest suite (including the agent with a scripted fake model), CI on GitHub Actions and a technical report in LaTeX. [Live app](https://aihsus-nf7jpftw8cba5pcupt6uoo.streamlit.app/)
- `Python` · `Streamlit` · `DuckDB` · `PostgreSQL` · `LangChain` · `Playwright`

### [mlops-churn-project](https://github.com/caiorj2004/mlops-churn-project): End-to-end MLOps for churn prediction
Turned a "works on my machine" training script into a reproducible system, step by step, with each tool introduced to solve a concrete problem.
- Data contract with Pandera, data versioning with DVC (`dvc repro` pipeline), experiment tracking and Model Registry in MLflow with a `@champion` alias and data → code → model lineage.
- Serving with FastAPI (Pydantic input contracts) and a Streamlit front end; two-layer deployment on AWS (ECR image, EC2 with IAM Role, PostgreSQL on a separate instance).
- The whole architecture also runs locally with one command (Docker Compose, or SQLite without Docker), so it doesn't depend on the cloud.
- pytest and GitHub Actions CI that rebuilds everything on every push, from `dvc pull` to a live API call against the containers.
- `Python` · `MLflow` · `DVC` · `FastAPI` · `Docker` · `AWS` · `GitHub Actions`

---

## Tools I work with

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly%20%2F%20Dash-3F4F75?logo=plotly&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?logo=mlflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonwebservices&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![Apache Spark](https://img.shields.io/badge/PySpark-E25A1C?logo=apachespark&logoColor=white)
![Microsoft Fabric](https://img.shields.io/badge/Microsoft_Fabric-117865?logo=microsoft&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?logo=duckdb&logoColor=black)
![DVC](https://img.shields.io/badge/DVC-13ADC7?logo=dvc&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?logo=langchain&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?logo=powerbi&logoColor=black)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)

**Statistics and modeling:** multivariate analysis (PCA, factor analysis, clustering, discriminant analysis), bootstrap and resampling validation, spatial statistics, weighted survey estimation, Bayesian inference (PyMC), generalized linear and mixed models.

---

## Experience and education

- **Data Science intern, ANTT** (Brazil's National Land Transportation Agency), Nov 2024 – Oct 2026
  - Data observability pipeline on a Microsoft Fabric Lakehouse: ingestion from a CKAN API, structural and completeness checks, IQR outlier detection and business-rule alerts for open-data auditing
  - Dimensional modeling with PySpark and Delta tables; classification models and executive Power BI dashboards (advanced DAX)
  - Fault-tolerant web scraping across public sources (Selenium, BeautifulSoup, requests) and unsupervised NLP (TF-IDF + K-Means) to organize news and regulatory publications by topic
- **Data Scientist intern, DatAí**, Aug – Oct 2024
  - Streamlit dashboards for economic indicators (municipal, state and regional GDP) backed by PostgreSQL via SQLAlchemy, with choropleth maps, time series and dynamic rankings in Plotly and pandas
- **Independent data professional, Levav-IT**, a team of independent professionals working on a per-project basis
- **B.S. in Data Science and Artificial Intelligence**, IESB (2026)
- **Undergraduate thesis:** *Typology of Rural Territories of the Federal District: A Socio-Spatial Clustering Analysis with PDAD Rural 2022*, developed in the **AgroTec** research group (funded by FAPDF)
