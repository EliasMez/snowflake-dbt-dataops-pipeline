# {{ config.site_name }}

Open-source DataOps reference architecture for ingesting, storing, and transforming analytical data on Snowflake using Python and dbt. Reproducible from a fork of the repository, this project automates the end-to-end lifecycle: infrastructure provisioning, incremental loading, analytical modeling, quality checks, governance, and documentation.


<br>
<a href="https://github.com/EliasMez/{{ config.repo_name }}/">💻 Project source code</a>
<br>
<a href="https://eliasmez.github.io/{{ config.repo_name }}/dbt">📚 Online **dbt** documentation</a>
<br>

## 📊 Data Source

[**TLC Trip Record Data**](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) - NYC Taxi and Limousine Commission

The data includes:

- Pickup and dropoff dates/times
- Pickup and dropoff zones
- Distances, detailed fares, payment types
- Passenger count reported by the driver

*Raw public data provided by the NYC TLC, subject to downstream quality and consistency checks within the pipeline.*

## 📄 License

This project is licensed under the MIT License. The source data is provided by the [NYC TLC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) and subject to their terms of use.