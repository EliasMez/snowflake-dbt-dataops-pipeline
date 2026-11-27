# Snowflake & dbt DataOps Pipeline

An automated data pipeline (Snowflake + dbt + GitHub Actions) for ingesting and transforming NYC TLC trip record data.

[![Live Documentation](https://img.shields.io/badge/docs-live_site-brightgreen)](https://eliasmez.github.io/snowflake-dbt-dataops-pipeline)
[![dbt Documentation](https://img.shields.io/badge/docs-dbt_site-FF694B)](https://eliasmez.github.io/snowflake-dbt-dataops-pipeline/dbt/)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=github-actions&logoColor=white)]()
[![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?logo=snowflake&logoColor=white)]()


## 📚 Documentation
*   **Project Documentation:** Available in multiple languages (🇬🇧 English, 🇫🇷 Français, 🇨🇳 中文, 🇪🇸 Español) at [https://eliasmez.github.io/snowflake-dbt-dataops-pipeline](https://eliasmez.github.io/snowflake-dbt-dataops-pipeline)
*   **dbt Documentation:** Technical documentation for data models, lineage, and tests at [https://eliasmez.github.io/snowflake-dbt-dataops-pipeline/dbt/](https://eliasmez.github.io/snowflake-dbt-dataops-pipeline/dbt/).


## 🚀 Quick Start
1.  **Fork** this repository.
2.  Add required Snowflake secrets in `Settings > Secrets > Actions`.
3.  Trigger the `Snowflake & dbt DataOps Pipeline` workflow manually via the GitHub Actions tab.

## 📊 Source Data
[**TLC Trip Record Data**](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) - NYC Taxi & Limousine Commission.

## 📘 Technical Reports

[**Data Platform Architecture & ELT**](./architecture_reference_dw_build.pdf) covers the design and implementation of the data warehouse, including dimensional modelling, Snowflake infrastructure setup, access management, and the full data pipeline from Python ingestion to dbt transformations and CI/CD.

[**Data Platform Operations & Governance**](./architecture_reference_dw_run.pdf) covers ongoing operations and evolution of the warehouse, including logging, alerting, maintenance planning, service indicators, backup policies, GDPR compliance, and structural model evolution.

## 📄 License
This project is licensed under the MIT License. Source data is provided by the NYC TLC under their terms of use.