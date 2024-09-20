# Análisis Descriptivo del Futuro del Petróleo

Este proyecto se centra en el análisis descriptivo y correlacional del mercado del petróleo . A partir de los datos diarios OHLC (Open, High, Low, Close) obtenidos de Yahoo Finance, el conjunto de datos ha sido enriquecido con información adicional recopilada mediante técnicas de web scraping . Posteriormente, se llevaron a cabo procesos de fusión , limpieza y estandarización para asegurar la calidad y consistencia de los datos.

## Tecnologías Utilizadas
Python:

- Pandas (para manipulación de datos)
- Matplotlib y Seaborn (para visualización de datos)
- NumPy (para cálculos numéricos)
- BeautifulSoup (para web scraping)

## Estructura del Proyecto
Se obtienen datos de Yahoo Finance, OHLC (Open, High, Low, Close), que son precios de apertura, máximos, mínimos y cierre diarios, para los siguientes activos:

![Diagrama de la estructura del proyecto](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Diagrama%20de%20la%20estructura%20del%20proyecto.drawio.png)
- CL (Futuros del Petróleo Crudo)
- Índice S&P 500
- EUR/USD (Euro frente al dólar)
- XLE (ETF del sector energético)

## Web Scraping de Noticias

Extracción de noticias relevantes con impacto directo en el mercado energético desde la página oficial de la Agencia Internacional de la Energía (AIE), utilizando técnicas de web scraping.
Web Scraping de Inventarios y Comercio Internacional

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


![Diagrama de la estructura del proyecto](https://private-user-images.githubusercontent.com/158542324/369427651-c439376a-1273-4a3b-b9b2-2df6d11c7fe3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjY4NDAwNjIsIm5iZiI6MTcyNjgzOTc2MiwicGF0aCI6Ii8xNTg1NDIzMjQvMzY5NDI3NjUxLWM0MzkzNzZhLTEyNzMtNGEzYi1iOWIyLTJkZjZkMTFjN2ZlMy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDkyMFQxMzQyNDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lZDdjMTJjNzQzZTYxOTlmZTk3YWRmNjM5OTIxM2NlOTk3MDg0ZmZjYTUwYzY3ZDQ1ZGM1MjYyOTY0Y2ZjM2Y3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.D9lihy62JiG8EyQnLBeGrtvmH_kG3Bo2UxIlmeYnVGM)
## Objetivo:
El proyecto busca comprender el comportamiento del petróleo y su evaluación con la economía, analizando el impacto de su oferta y demanda. Además, se enfoca en identificar ineficiencias, tendencias y correl-aciones que serán utilizadas para un futuro análisis predictivo, ayudando en la toma de decisiones de inversión.
