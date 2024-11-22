# Análisis Descriptivo del Petróleo  
![Crude](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Screenshots/crude%20oil.jpg)  

Este proyecto es una continuación del EDA, enfocado en un análisis descriptivo, correlacional y de clustering del mercado del petróleo. A partir de datos OHLC (Open, High, Low, Close) obtenidos de Yahoo Finance, y enriquecidos con información adicional recopilada mediante web scraping, se han llevado a cabo procesos de limpieza, estandarización y fusión para garantizar la consistencia de los datos.

---

## Tecnologías Utilizadas  
**Python:**  
- Pandas y Numpy  
- Matplotlib y Seaborn  
- BeautifulSoup (para web scraping)  
- Scikit-learn  

---

## Estructura del Proyecto  

### Datos:  
Se trabajó con datos OHLC de los siguientes activos:  
- **CL**: Futuros del Petróleo Crudo  
- **S&P 500**: Índice bursátil  
- **EUR/USD**: Tipo de cambio euro-dólar  
- **XLE**: ETF del sector energético  

Además, se realizó web scraping para recopilar:  
- **Noticias relevantes** de la Agencia Internacional de Energía (AIE).  
- **Datos semanales de inventarios**, importación y exportación de petróleo.  

---

## Procesamiento de Datos  

1. **Limpieza y Estandarización:** Normalización de datos, manejo de valores nulos y corrección de outliers.  
2. **Joins y Merges:** Fusión de datos financieros, inventarios y noticias en un único dataset.  
3. **Creación de Variables Nuevas:** Generación de variables categóricas y continuas para análisis descriptivo y predictivo.  

---

## Análisis Exploratorio de Datos  

1. **Análisis Descriptivo:** Visualización de tendencias en exportación, importación y producción diaria.  
2. **Análisis Correlacional:** Relación entre el precio del petróleo, inventarios y eventos macroeconómicos.  
3. **Identificación de Patrones:** Filtrado de días clave (máximos históricos, eventos económicos) y análisis de comportamiento.  

![Crude](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Screenshots/Rachas_importacion.png)  
---

## Clustering (Continuación del EDA)  

### Metodología:  
1. Se analizaron 60 variables utilizando PCA para reducir la dimensionalidad.  
   - La varianza total explicada fue del 53% con tres componentes principales.  
   - **Variables clave:** exportación diaria, producción acumulativa y reservas semanales.  
2. Se utilizó el método del codo y la silueta para determinar el número óptimo de clusters (k=3).
![Crude](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Screenshots/Contribucion_PCA.png)  

### Resultados:  
Los clusters identificados fueron perfilados y desnormalizados, obteniendo tres grupos principales:  
- **High_Import:** Alta importación y volatilidad.  
- **High_Production_Export:** Alta producción y exportación; importación baja.  
- **Low_Reserves_Activity:** Reservas bajas y actividad reducida.  

### Análisis Complementario:  
- Visualización de coeficientes de silueta y distancias entre centroides para verificar consistencia.  
- Relación entre importación, exportación y variables como volatilidad y rango diario.  

![Crude](https://github.com/Arnaud-Chafai/EDA-CL/blob/main/Screenshots/Perfilado.png)  
---

## Conclusiones  

El análisis permitió identificar patrones clave en el mercado del petróleo:  
1. **Impacto de la importación:**  
   - Cuando la importación semanal aumenta y la producción baja, el petróleo sube y el dólar tiende a bajar.  

2. **Alta producción y exportación:**  
   - Produce un mercado más estable, con volatilidad y rango diario normales.  

3. **Reservas bajas con alta importación:**  
   - Tiende a reducir los precios del petróleo, lo que fortalece el dólar.  

