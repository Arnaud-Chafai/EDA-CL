# Análisis Descriptivo del Petróleo
![Crude](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Screenshots/crude%20oil.jpg)

Este proyecto se centra en el análisis descriptivo y correlacional del mercado del petróleo . A partir de los datos diarios OHLC (Open, High, Low, Close) obtenidos de Yahoo Finance, el conjunto de datos ha sido enriquecido con información adicional recopilada mediante técnicas de web scraping . Posteriormente, se llevaron a cabo procesos de fusión , limpieza y estandarización para asegurar la calidad y consistencia de los datos.
---

## Tecnologías Utilizadas
Python:

- Pandas y Numpy
- Matplotlib y Seaborn
- BeautifulSoup (para web scraping)

## Estructura del Proyecto
Se obtienen datos de Yahoo Finance, OHLC (Open, High, Low, Close), que son precios de apertura, máximos, mínimos y cierre diarios, para los siguientes activos:
- CL (Futuros del Petróleo Crudo)
- Índice S&P 500
- EUR/USD (Euro frente al dólar)
- XLE (ETF del sector energético)

## Web Scraping de Noticias

Extracción de noticias relevantes con impacto directo en el mercado energético desde la página oficial de la Agencia Internacional de la Energía (AIE), utilizando técnicas de web scraping.
Web Scraping de Inventarios y Comercio Internacional.

Extracción de datos de los resultados semanales de inventarios de petróleo, así como datos de importación y exportación.

## Procesamiento de Datos

### Limpieza y Estandarización:
- Corrección de errores, normalización y manejo de valores faltantes.

### Joins y Merges:
- Integración de datos de Yahoo Finance, inventarios y noticias en un único dataset.

### Tratamiento de Valores Atípicos:
- Identificación y corrección de valores anómalos.

### Formateo de Fechas:
- Estandarización de las fechas para análisis temporal.

### Creación y Categorización de Variables:
- Generación de nuevas variables y categorización de datos clave.

## Análisis Exploratorio de Datos

### Análisis Descriptivo
- Exploración de las características generales de la exportaciones de barriles.
- Visualización de tendencias de las exportaciones.

### Análisis Correlacional
- Evaluación de la relación entre el precio del petróleo y otros activos financieros.
- Identificación de correlaciones con eventos macroeconómicos y datos de inventarios.

### Filtrados de Días en Máximos Históricos
- Un ejemplo del análisis es este filtro que identifica los días en máximos históricos y 
 muestra sus descripciones estadísticas, destacando patrones de comportamiento del precio.

## Objetivo:
El proyecto busca comprender el comportamiento del petróleo y su evaluación con la economía, analizando el impacto de su oferta y demanda. Además, se enfoca en identificar ineficiencias, tendencias y correlaciones que serán utilizadas para un futuro análisis predictivo, ayudando en la toma de decisiones de inversión.
