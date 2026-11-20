# {{ config.site_name }}

Arquitectura de referencia DataOps de código abierto para la ingesta, el almacenamiento y la transformación de datos analíticos en Snowflake con Python y dbt. Reproducible desde un fork del repositorio, este proyecto automatiza el ciclo completo: aprovisionamiento de infraestructura, carga incremental, modelado analítico, controles de calidad, gobernanza y documentación.


<br>
<a href="https://github.com/EliasMez/{{ config.repo_name }}/">💻 Código fuente del proyecto</a>
<br>
<a href="https://eliasmez.github.io/{{ config.repo_name }}/dbt">📚 Documentación **dbt** en línea</a>
<br>

## 📊 Fuente de Datos

[**Datos de Registro de Viajes de la TLC**](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) - Comisión de Taxis y Limusinas de Nueva York

Los datos incluyen:

- Fechas/horas de recogida y entrega
- Zonas de origen y destino
- Distancias, tarifas detalladas, tipos de pago
- Número de pasajeros reportado por el conductor

*Datos públicos sin procesar proporcionados por la NYC TLC, sometidos a controles de calidad y coherencia aguas abajo en el pipeline.*

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Los datos de origen son proporcionados por la [NYC TLC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) y sujetos a sus términos de uso.