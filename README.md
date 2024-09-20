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

![Categorización](https://private-user-images.githubusercontent.com/158542324/369427651-c439376a-1273-4a3b-b9b2-2df6d11c7fe3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjY4NDAwNjIsIm5iZiI6MTcyNjgzOTc2MiwicGF0aCI6Ii8xNTg1NDIzMjQvMzY5NDI3NjUxLWM0MzkzNzZhLTEyNzMtNGEzYi1iOWIyLTJkZjZkMTFjN2ZlMy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDkyMFQxMzQyNDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lZDdjMTJjNzQzZTYxOTlmZTk3YWRmNjM5OTIxM2NlOTk3MDg0ZmZjYTUwYzY3ZDQ1ZGM1MjYyOTY0Y2ZjM2Y3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.D9lihy62JiG8EyQnLBeGrtvmH_kG3Bo2UxIlmeYnVGM)

## Análisis Exploratorio de Datos

### Análisis Descriptivo
- Exploración de las características generales de la exportaciones de barriles.
- Visualización de tendencias de las exportaciones.
![Análisis Descriptivo](https://private-user-images.githubusercontent.com/158542324/369427663-20e51fcb-0a96-40a5-b84d-6d696c7d9361.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjY4NDA1NjMsIm5iZiI6MTcyNjg0MDI2MywicGF0aCI6Ii8xNTg1NDIzMjQvMzY5NDI3NjYzLTIwZTUxZmNiLTBhOTYtNDBhNS1iODRkLTZkNjk2YzdkOTM2MS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDkyMFQxMzUxMDNaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hMWZhNWVkNGQ3YjMxYTZhNzMzN2JmZTc5ZjBhMjNjNGIxMDU2MWU4YzczMWFjNDU4MTE4MmM1OTJkZTk5NjMwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.XMmPFIUGJ_1Odvs9ekxV_a-aVu0Ic23QPnlb0VkMLNg)

### Análisis Correlacional
- Evaluación de la relación entre el precio del petróleo y otros activos financieros.
- Identificación de correlaciones con eventos macroeconómicos y datos de inventarios.
![Análisis Correlacional](https://private-user-images.githubusercontent.com/158542324/369427656-cd23bb22-be04-4c3c-a870-2c2b8debd162.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjY4NDA1NjMsIm5iZiI6MTcyNjg0MDI2MywicGF0aCI6Ii8xNTg1NDIzMjQvMzY5NDI3NjU2LWNkMjNiYjIyLWJlMDQtNGMzYy1hODcwLTJjMmI4ZGViZDE2Mi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDkyMFQxMzUxMDNaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01Y2NkNGNmMTNjMzA1MDkxYWU5MDJjYTRiYTMzM2UzZDU3ZDhkZDRkZDU3MWNhNGIyYjE2NzI0MDc0OWVlZmRjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.lqakusZJlz75OCm91XT4EUMxKiIiIstdCYX7AU9oSYo)

### Filtrados de Días en Máximos Históricos
- Un ejemplo del análisis es este filtro que identifica los días en máximos históricos y 
 muestra sus descripciones estadísticas, destacando patrones de comportamiento del precio.
![Máximos Históricos](https://private-user-images.githubusercontent.com/158542324/369427666-18dcc853-815c-43ad-b375-b62329d754d0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjY4NDA1NjMsIm5iZiI6MTcyNjg0MDI2MywicGF0aCI6Ii8xNTg1NDIzMjQvMzY5NDI3NjY2LTE4ZGNjODUzLTgxNWMtNDNhZC1iMzc1LWI2MjMyOWQ3NTRkMC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwOTIwJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDkyMFQxMzUxMDNaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1kMDQwZDNlYWE3ODJkYWE5MzhkYWZmMzk1Yjc0YmYxNDI0ZjI2MTlmN2NkYzZlMjI5NWMwMDBjMjQxZjc3MjE5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.EUnkR5B40Fi-Y6ZFDHUPzUf1Ex1_kn9WZwKVOuCGgVI)

## Objetivo:
El proyecto busca comprender el comportamiento del petróleo y su evaluación con la economía, analizando el impacto de su oferta y demanda. Además, se enfoca en identificar ineficiencias, tendencias y correl-aciones que serán utilizadas para un futuro análisis predictivo, ayudando en la toma de decisiones de inversión.
