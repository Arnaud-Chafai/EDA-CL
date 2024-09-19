# Análisis Descriptivo del Futuro del Petróleo

Este proyecto se centra en el análisis descriptivo y correlacional del mercado del petróleo . A partir de los datos diarios OHLC (Open, High, Low, Close) obtenidos de Yahoo Finance, el conjunto de datos ha sido enriquecido con información adicional recopilada mediante técnicas de web scraping . Posteriormente, se llevaron a cabo procesos de fusión , limpieza y estandarización para asegurar la calidad y consistencia de los datos.

### Tecnologías Utilizadas
Idioma: Python

- Pandas (para manipulación de datos)
- Matplotlib y Seaborn (para visualización de datos)
- NumPy (para cálculos numéricos)
- BeautifulSoup (para web scraping)

### Estructura del Proyecto
Se obtienen datos de Yahoo Finance, OHLC (Open, High, Low, Close), que son precios de apertura, máximos, mínimos y cierre diarios, para los siguientes activos:

- CL (Futuros del Petróleo Crudo)
- Índice S&P 500
- EUR/USD (Euro frente al dólar)
- XLE (ETF del sector energético)

### Web Scraping de Noticias

Extracción de noticias relevantes con impacto directo en el mercado energético desde la página oficial de la Agencia Internacional de la Energía (AIE), utilizando técnicas de web scraping.
Web Scraping de Inventarios y Comercio Internacional

Extracción de datos de los resultados semanales de inventarios de petróleo, así como datos de importación y exportación.

### Procesamiento de datos

##### Limpieza y Estandarización:
- Corrección de errores, normalización y manejo de valores faltantes.
##### Joins y merges
- Integración de datos de Yahoo Finance, inventarios y noticias en un único dataset.
##### Tratamiento de Valores Atípicos
- Identificación y corrección de valores anómalos.
##### Formateo de Fechas
- Estandarización de las fechas para análisis temporal.
##### Creación y Categorización de Variables
- Generación de nuevas variables y categorización de datos clave.

### Objetivo:
El proyecto busca comprender el comportamiento del petróleo y su evaluación con la economía, analizando el impacto de su oferta y demanda. Además, se enfoca en identificar ineficiencias, tendencias y correl-aciones que serán utilizadas para un futuro análisis predictivo, ayudando en la toma de decisiones de inversión.
