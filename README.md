# analysis-everpeak
# 🚦 Mobility & Economy: Análisis de movilidad urbana y economía

## 📌 Descripción del proyecto

Este proyecto explora la relación entre la movilidad urbana y los indicadores económicos de 15 ciudades latinoamericanas durante 2024. A partir de datos de tráfico de **TomTom Traffic Index** e indicadores económicos de **OECD Cities**, se realizó un proceso de limpieza, transformación, integración y visualización de datos para identificar patrones de congestión vehicular y su posible relación con el PIB per cápita.

El análisis busca aportar información útil para comprender los desafíos de movilidad urbana y orientar futuras investigaciones sobre infraestructura de transporte y desarrollo económico.

## 🎯 Objetivo

Analizar la relación entre los indicadores de congestión vehicular, los tiempos de viaje y el PIB per cápita de diferentes ciudades latinoamericanas, mediante técnicas de análisis exploratorio y visualización de datos.

## 🛠️ Herramientas y tecnologías

- **Python:** lenguaje de programación utilizado para el análisis.
- **Pandas:** limpieza, transformación, agrupación e integración de datos.
- **NumPy:** soporte para operaciones numéricas.
- **Seaborn:** visualización y exploración de distribuciones.
- **Matplotlib:** creación y personalización de gráficos.
- **Jupyter Notebook:** entorno de desarrollo y documentación del análisis.

## 📊 Datos analizados

El proyecto integra dos fuentes de información:

- **TomTom Traffic Index:** indicadores de tráfico, congestión y tiempos de viaje.
- **OECD Cities:** indicadores económicos y demográficos de las ciudades.

**Cobertura:** año 2024, 15 ciudades y 7 países: Argentina, Brasil, Chile, Colombia, México, Perú y Uruguay.

Entre las principales variables analizadas se encuentran:

- `JamsDelay`: indicador de demora asociado a la congestión.
- `TrafficIndexLive`: índice de tráfico.
- `TravelTimeLivePer10KmsMins`: tiempo de viaje por cada 10 km.
- `city_gdp_capita`: PIB per cápita de la ciudad.
- `unemployment_pct`: porcentaje de desempleo.
- `population`: población.

## 🔍 Metodología

El análisis se desarrolló en las siguientes etapas:

1. **Exploración de datos:** revisión de la estructura, las columnas y los tipos de datos.
2. **Limpieza y preparación:** estandarización de nombres de columnas, conversión de fechas y corrección de formatos numéricos.
3. **Filtrado temporal:** selección de los registros correspondientes a 2024.
4. **Agregación:** cálculo de promedios anuales de indicadores de tráfico por ciudad.
5. **Integración de fuentes:** combinación de los datos de movilidad y economía mediante una unión `INNER` por ciudad y año.
6. **Análisis exploratorio:** elaboración de gráficos para estudiar la distribución de la congestión, el PIB per cápita y su comportamiento entre ciudades.
7. **Exportación:** generación de un archivo CSV con los datos integrados para su reutilización.

## 📈 Principales hallazgos

- **Ciudad de México** presentó el mayor promedio del indicador `JamsDelay` entre las ciudades evaluadas.
- La comparación visual no evidenció una relación directa y uniforme entre un PIB per cápita más alto y mayores niveles de congestión.
- El análisis de la distribución de `JamsDelay` permitió observar valores extremos que pueden influir en el promedio de los indicadores.
- Los resultados sugieren que la movilidad urbana debe analizarse considerando múltiples factores, más allá del desempeño económico de cada ciudad.

## 💡 Conclusiones y recomendaciones

El análisis exploratorio muestra que la relación entre movilidad urbana y economía no puede explicarse únicamente mediante el PIB per cápita. Para comprender mejor las diferencias entre ciudades, sería conveniente incorporar variables relacionadas con la densidad urbana, el parque automotor, la calidad de la infraestructura vial y la disponibilidad de transporte público.

Como siguiente paso, se recomienda complementar el análisis visual con medidas estadísticas de correlación y estudios adicionales que permitan evaluar con mayor precisión las relaciones entre los indicadores.

**Nota:** los resultados corresponden a una exploración descriptiva de los datos y no permiten establecer relaciones causales.

## 📁 Entregables

- `S5_ladb_mobility_economy_project_student.ipynb`: notebook con el proceso de análisis, el código y las visualizaciones.
- `ladb_mobility_economy_2024_clean.csv`: conjunto de datos integrado y exportado para análisis posteriores.

## 👩‍💻 Autora

**Nicole Lozano**  
Data Analytics Bootcamp | TripleTen

[GitHub: nlozano-analytics](https://github.com/nlozano-analytics)

---

*Proyecto desarrollado con fines de aprendizaje y aplicación de habilidades de análisis de datos con Python.*
