{% docs __overview__ %}
# Snowflake & dbt DataOps Pipeline — dbt Documentation

Technical documentation for the dbt transformation layer of the **Snowflake & dbt DataOps** reference architecture. It covers data modeling, quality tests, source definitions, and model lineage across the warehouse layers.

- 📚 [Global Project Documentation](https://eliasmez.github.io/snowflake-dbt-dataops-pipeline/)
- 💻 [Project Source Code](https://github.com/EliasMez/snowflake-dbt-dataops-pipeline/)

## Transformation Architecture

The dbt project structures transformations across distinct modeling layers from raw ingestion to analytics-ready datasets:

- **Sources & Seeds (`raw`):** Immutable landing tables loaded from public trip records and reference seeds (`taxi_zone_lookup`).
- **Staging (`staging`):** Standardized, type-cast, and cleaned views (`stg_taxi_trips`) enforcing naming conventions and schema validation.
- **Intermediate (`intermediate`):** Business logic and trip-level metric calculations (`int_trip_metrics`) isolated prior to dimensional modeling.
- **Core & Marts (`marts`):** Dimensional models (**Dimensions** and **Fact Tables**) and business-oriented **Analytical Marts** exposed for reporting and BI consumption.

Each model is documented with column descriptions, data quality tests, and explicit upstream/downstream dependencies.

## Navigating the Documentation

- **Project Tab:** Browse the dbt project structure, model definitions, tests, and documentation.
- **Database Tab:** Inspect tables and views organized by Snowflake database and schema.
- **Lineage Graph:** Click the graph icon in the **bottom-right corner** to explore end-to-end model and source dependencies.

---
{% enddocs %}

{% docs __source_raw__ %}
## Data Source — Raw

The source data comes from **TLC Trip Record Data** (New York City Taxi & Limousine Commission).

The dataset includes:
- Pick-up and drop-off timestamps
- Pick-up and drop-off taxi zone IDs
- Trip distances and passenger counts
- Detailed fare breakdowns, surcharges, and payment types

Raw public data provided by the NYC TLC, subject to downstream quality and consistency checks within the pipeline.
{% enddocs %}

{% docs __dbt_utils__ %}
## dbt_utils

The **dbt_utils** package provides core SQL generation and testing macros used across the project to standardize surrogate key generation, schema validation, and data integrity checks.
{% enddocs %}

{% docs __dbt_expectations__ %}
## dbt_expectations

The **dbt_expectations** package is used to implement extended data quality assertions across staging, intermediate, and mart models, including:
- Completeness and nullability checks
- Value range and accepted set validations
- Row count and schema consistency assertions
{% enddocs %}

{% docs __dbt_date__ %}
## dbt_date

The **dbt_date** package provides date and calendar utility macros (installed as a dependency of `dbt_expectations`).

Temporal dimensions in this project are built directly from observed source timestamps in SQL to match the exact coverage of the ingested data across hourly, daily, weekly, monthly, and yearly grains.
{% enddocs %}