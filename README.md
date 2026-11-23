# Hi, I'm Caio

Data Science & AI student at **IESB**, finishing my B.S. in Data Science and Artificial Intelligence. I build reproducible analytics pipelines, interactive dashboards and ML systems, with a focus on public data and territorial analysis.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Caio_Rosendo_J%C3%A1come-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/caio-rosendo-j%C3%A1come-69037a295)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face-caiorj2004-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/caiorj2004)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--5451--7975-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0001-5451-7975)

---

## Featured projects

### [pdad_tipologia_cluster](https://github.com/caiorj2004/pdad_tipologia_cluster): Typology of rural territories in the Federal District (Brazil)
My undergraduate thesis. A socioeconomic typology of rural territories built from the **PDAD Rural 2022** survey (5,075 households, 66,540 people after sample expansion), grouped into 49 region × subpopulation segments.
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
Streamlit dashboard plus a text-to-SQL AI assistant for hospital admissions data (AIH/DATASUS). End-to-end pipeline: scraping with Playwright, PostgreSQL, DuckDB over Parquet, and a LangChain agent (Groq, Bedrock).
- `Python` · `Streamlit` · `DuckDB` · `PostgreSQL` · `LangChain`

### [mlops-churn-project](https://github.com/caiorj2004/mlops-churn-project): End-to-end MLOps for churn prediction
Data validation with Pandera, versioning with DVC, model tracking and registry with MLflow, serving with FastAPI and a Streamlit front end. Two-layer deployment on AWS, runs locally with Docker Compose, CI on GitHub Actions.
- `Python` · `MLflow` · `DVC` · `FastAPI` · `Docker` · `AWS`

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

**Statistics and modeling:** PCA, clustering, bootstrap and resampling validation, spatial statistics, weighted survey estimation, Bayesian inference, generalized linear models.

---

## Experience and education

- Independent data professional at **Levav-IT**, a team of independent professionals that works on a per-project basis
- **B.S. in Data Science and Artificial Intelligence**, IESB (final semester, 2026)
- **Undergraduate thesis:** *Typology of Rural Territories of the Federal District: A Socio-Spatial Clustering Analysis with PDAD Rural 2022*
- Member of the **AgroTec** project group, working on data products for family farming in the DF
