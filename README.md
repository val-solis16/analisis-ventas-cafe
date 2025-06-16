# analisis-ventas-cafe
Predicción del monto de ventas de un producto (café), por medio de un modelo lineal

## 📝 Descripción del Proyecto
Este proyecto consiste en un caso hipotético para una cadena de supermercados, que buscan predecir el monto total de ventas de un producto con base en ciertas características. Mi objetivo fue aplicar técnicas de análisis de datos para entender el comportamiento de las ventas y desarrollar un modelo predictivo del producto.

## 📊 Conjunto de Datos
El análisis se generó utilizando el dataset `ventas_supermercado.xlsx`. Este archivo contiene las siguientes columnas:
- `producto`: Descripción del producto vendido.
- `sede`: Ubicación geográfica del supermercado.
- `precio`: Precio unitario.
- `publicidad`: Monto invertido en publicidad.
- `descuento`: Porcentaje de descuento.
- `popularidad`: Popularidad del producto.
- `tiempo_en_estante`: Cantidad de días promedio que un producto permanece en estantería.
- `stock_inicial`: Cantidad de productos en stock al inicio del periodo.
- `promocion`: Si el producto tiene promoción (0=no, 1=sí).
- `demanda_regional`: Valor de demanda en la región.
- `ventas`: Total de ventas del producto (en dinero). 

## 🛠️ Herramientas y Tecnologías Utilizadas
- **Python:** Lenguaje de programación.
    - **Pandas:** Carga, limpieza y manipulación de datos.
    - **Matplotlib y Seaborn:** Visualizaciones de datos.
    - **scikit-learn:** Análisis de correlación, separación de datos y desarrollo de modelos de Regresión Lineal.
- **Google Colab:** Entorno de desarrollo.
- **Microsoft Excel:** Formato del dataset.

## 🚀 Metodología del análisis
Este proyecto sigue un proceso de trabajo estándar de análisis de datos, el cual incluye:
1.  **Carga de paquetes, librerías y data**  
2.  **Limpieza y Transformación de Datos:** Ajuste de valores nulos, tipos de datos, creación de nuevas características. 
3.  **Análisis Exploratorio de Datos (EDA) y Visualizaciones:**
    * Distribución de variables clave
    * Visualizaciones para identificar patrones y relaciones entre variables
    * Aplicación de técnicas estadísticas para la interpretación de datos
4.  **Análisis de Correlación:** Relación entre las variables de entrada y la variable objetivo (`ventas`). 
5.  **Proceso de Modelado:**
    * Separación de datos en conjuntos de entrenamiento y prueba.
    * Desarrollo de un modelo predictivo (en este caso: Regresión Lineal) para estimar el monto de ventas de café.
    * Evaluación del rendimiento del modelo utilizando métricas relevantes (R-cuadrado, MAE, RMSE).
6.  **Documentación de Resultados e Interpretación de Métricas** 

##💡 Hallazgos y Conclusiones
* Por medio de un pair plot, se pudo observar que la variable ventas tiene una distribución con una asimetría positiva, en comparación con las demás variables en donde se observa que no cuentan con una distribución normal. Por otra parte, según los gráficos de dispersión, los datos se encuentran muy dispersos entre sí, sin embargo si se observa el gráfico de ventas y popularidad, se puede ver que si hay una relación no tan dispersa, ya que indica que a mayor nivel de popularidad del producto, mayor será el nivel de ventas del mismo.
* De acuerdo con el scatter plot realizado, se puede ver la relación de ventas y popularidad anteriormente realizada, pero ahora con la categoría de promoción, entonces como se puede observar, efectivamente las ventas aumentan conforme crece la popularidad del café y aún más si este cuenta con una promoción.
* El modelo demostró un alto poder predictivo, explicando aproximadamente el 90.90% de la variabilidad en las ventas de café (R² = 0.90). Esto indica que las variables seleccionadas y el modelado son muy efectivos. Las predicciones del modelo se desvían de las ventas reales por solo ~13.4 unidades (RMSE), lo que confirma una buena precisión.

## 🚀 ¿Cómo reproducir este análisis?
1.  Clonar este repositorio en una máquina local.
2.  Abrir el notebook `notebook/Proyecto_MIN_ValeriaSolis.ipynb` en Google Colab o en Jupyter Notebook.
3.  Asegurarse de que el archivo `data/ventas_supermercado.xlsx` se encuentre en `data/`.
4.  Ejecutar todas las celdas para ver el análisis completo.


---
**Autora:** Valeria Solís Monge

**Contacto:** [valsolis1601@gmail.com] | [www.linkedin.com/in/valeria-solis-monge-411514325]

