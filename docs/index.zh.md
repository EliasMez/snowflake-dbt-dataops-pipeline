# {{ config.site_name }}

基于 Snowflake，使用 Python 和 dbt 对分析型数据进行摄取、存储和转换的开源 DataOps 参考架构。该项目可通过复刻（fork）代码仓库直接复现，实现了全生命周期的工程化与自动化：基础设施配置、增量加载、分析建模、质量校验、数据治理及文档生成。

<br>
<a href="https://github.com/EliasMez/{{ config.repo_name }}/">💻 项目源代码</a>
<br>
<a href="https://eliasmez.github.io/{{ config.repo_name }}/dbt">📚 在线 **dbt** 文档</a>
<br>

## 📊 数据来源

[**TLC 行程记录数据**](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) - 纽约市出租车和礼车委员会

数据包含：

- 上车和下车日期/时间
- 上下客区域（LocationID 区域编码）
- 距离、详细费用、支付类型
- 司机报告乘客数量

*由 NYC TLC 提供的原始公开数据，在数据管道下游经过质量与一致性校验。*

## 📄 许可证

本项目采用 MIT 许可证。源数据由 [纽约市 TLC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) 提供，并受其使用条款约束。