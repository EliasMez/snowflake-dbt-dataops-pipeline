# {{ config.site_name }}

Architecture de référence DataOps open-source pour l'ingestion, le stockage et la transformation de données analytiques sur Snowflake avec Python et dbt. Reproductible depuis un fork du dépôt, ce projet industrialise le cycle complet : provisionnement de l'infrastructure, chargement incrémental, modélisation analytique, contrôles de qualité, gouvernance et documentation.

<br> <br>
<a href="https://github.com/EliasMez/{{ config.repo_name }}/">💻 Code source du projet</a>
<br>
<a href="https://eliasmez.github.io/{{ config.repo_name }}/dbt">📚 Documentation <strong>dbt</strong> en ligne</a>
<br>

## 📊 Source des Données

[**TLC Trip Record Data**](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) - Commission des Taxis et Limousines de NYC

Les données incluent :

- Dates/heures de prise en charge et dépose
- Zones de prise en charge et de dépose
- Distances, tarifs détaillés, types de paiement
- Nombre de passagers rapporté par le chauffeur

*Données publiques brutes fournies par la NYC TLC soumises à des contrôles de qualité et de cohérence en aval dans le pipeline.*

## 📄 Licence

Ce projet est sous licence MIT. Les données source sont fournies par la [NYC TLC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) et soumises à leurs conditions d'utilisation.