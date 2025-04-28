# Analisis De Datos Alura Store

## **Descripción del Proyecto**

Este proyecto está enfocado en analizar el rendimiento de las tiendas de Alura Store para ayudar al Sr. Juan a tomar una decisión estratégica sobre qué tienda vender para iniciar un nuevo emprendimiento. Se han analizado varios indicadores clave, como ingresos, ventas por categoría, satisfacción del cliente, costos de envío y rendimiento geográfico. El análisis se realizó utilizando Google Colab y se incluye un conjunto de códigos y visualizaciones para facilitar la comprensión y toma de decisiones.


## **Instalación y Requisitos**

Para ejecutar este proyecto, se debe utilizar Google Colab, lo cual facilita la ejecución en la nube sin necesidad de configuración local. Simplemente, abre el archivo `.ipynb` en Google Colab para comenzar.

### **Dependencias**

El proyecto requiere las siguientes bibliotecas de Python, las cuales están instaladas en el entorno de Google Colab:

- **Pandas**: Para la manipulación y análisis de datos en formato CSV.
- **Matplotlib**: Para la creación de gráficos y visualizaciones.
- **Folium**: Para la creación de mapas interactivos y análisis geográfico.
- **NumPy**: Para manejar arrays y cálculos matemáticos.
- **Seaborn**: Para visualizaciones adicionales y análisis estadístico.

En el archivo de Google Colab, las bibliotecas se instalan automáticamente cuando se ejecutan las celdas correspondientes. No es necesario instalar estas bibliotecas manualmente.

Las siguientes bibliotecas se utilizan para llevar a cabo el análisis de los datos:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import folium
from folium.plugins import HeatMap, MarkerCluster
import seaborn as sns
```

## **3. Cómo ejecutar el proyecto**

Para ejecutar el proyecto, sigue estos pasos:

1. Abre el archivo del proyecto en Google Colab.
2. Asegúrate de que las celdas de código estén correctamente ejecutadas.
3. Los datos de las tiendas se descargan automáticamente desde los enlaces de CSV proporcionados dentro del proyecto.
4. Los resultados se muestran en formato de tabla o gráfico, y se incluyen mapas interactivos que te permiten explorar las áreas de ventas.

Este proyecto está preparado para ser ejecutado tal como está en Google Colab, por lo que no es necesario hacer ninguna configuración adicional. Solo necesitas abrir el archivo `.ipynb` y seguir las instrucciones.

## **4. Descripción de los archivos CSV**

Los archivos CSV contienen los datos de ventas de cada tienda de la cadena Alura Store. Los archivos se encuentran disponibles en los siguientes enlaces:

- **Tienda 1**: [CSV Tienda 1](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_1%20.csv)
- **Tienda 2**: [CSV Tienda 2](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_2.csv)
- **Tienda 3**: [CSV Tienda 3](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_3.csv)
- **Tienda 4**: [CSV Tienda 4](https://raw.githubusercontent.com/alura-es-cursos/challenge1-data-science-latam/refs/heads/main/base-de-datos-challenge1-latam/tienda_4.csv)

Los datos incluyen información sobre los productos vendidos, ingresos, costos de envío, calificaciones de los clientes, fechas de compra, y coordenadas geográficas (latitud y longitud) para análisis geográficos.


## **Análisis y Visualizaciones**

En el proyecto se realiza un análisis exhaustivo de los datos con los siguientes objetivos:

1. **Cálculo de los ingresos totales por tienda**: Se compara el rendimiento económico de cada tienda.
2. **Análisis de ventas por categoría y producto**: Se determina cuál es el producto más vendido y la categoría que domina las ventas.
3. **Valoración del cliente**: Se calculan las calificaciones promedio de los productos y se determina cuál tienda tiene las mejores valoraciones.
4. **Costos de envío**: Se analizan los costos de envío de cada tienda.
5. **Análisis geográfico**: Se realiza un análisis de la distribución geográfica de las ventas, utilizando mapas de calor y marcadores interactivos.
6. **Análisis y Recomendaciones**: Basado en los resultados, se presenta una recomendación sobre qué tienda debería venderse para maximizar el rendimiento y crecimiento.


## **Pasos Realizados**

### 1. **Carga de datos**
- Se cargaron los datasets de las 4 tiendas.
- Se agregó una columna para identificar de qué tienda provenía cada registro.

### 2. **Análisis de ingresos**
- Se calcularon los ingresos totales por tienda.
- Se generaron gráficos de barras para visualizar y comparar ingresos.
- Se identificó la tienda con mayores y menores ingresos.

### 3. **Análisis de categorías de productos**
- Se agruparon los productos por categoría y tienda.
- Se crearon tablas para visualizar el top 5 de las categorías más vendidas por tienda.
- Se generaron gráficos circulares para representar la distribución de ventas por categoría.

### 4. **Satisfacción del cliente**
- Se calcularon las calificaciones promedio de cada tienda.
- Se identificó la tienda mejor valorada y las de menor valoración.

### 5. **Análisis de productos**
- Se determinaron los productos más vendidos y menos vendidos en cada tienda.
- Se generaron tablas ordenadas para facilitar la visualización.

### 6. **Costos de envío**
- Se calculó el costo de envío promedio de cada tienda.
- Se compararon los costos entre tiendas.

### 7. **Análisis geográfico**
- Se realizaron:
  - Gráficos de dispersión para ver la distribución de ventas.
  - Heatmaps para identificar zonas de alta concentración de ventas.
  - Mapas interactivos usando Folium para representar ventas y desempeño geográfico.
- Se analizaron zonas dominantes de cada tienda utilizando una cuadrícula geográfica.

### 8. **Resumen y comparación de tiendas**
- Se generó un resumen cuantitativo del número de zonas dominadas por cada tienda.
- Se analizó la tasa (%) de zonas de rendimiento superior para cada tienda.

## **Conclusiones y Recomendaciones**

- Tienda 1 genera los mayores ingresos, pero tiene baja valoración y altos costos de envío.
- Tienda 3 es la mejor en cuanto a satisfacción del cliente y en la venta del producto estrella (muebles).
- Tienda 4, aunque tiene el envío más económico, presenta los peores indicadores de ingresos, dominancia geográfica y valoración.

**Recomendación final:**  
> Basado en los datos analizados, se recomienda la venta de la Tienda 4, ya que tiene un rendimiento inferior en comparación con las demás tiendas, tanto en términos de ingresos, valoraciones de clientes y dominancia geográfica. La Tienda 3, por otro lado, se muestra como la más sólida para continuar con el crecimiento de la cadena Alura Store.

## **7. Posibles problemas y soluciones**

### **Superposición de puntos en los gráficos geográficos**
En áreas de alta densidad de datos, puede haber una superposición de puntos. Se recomienda utilizar **gráficos separados** por tienda o agregar capas de **HeatMap** para visualizar mejor las concentraciones de ventas.

### **Archivos CSV no se descargan correctamente**
Si los archivos CSV no se descargan correctamente, asegúrate de que el enlace sea accesible. En caso de problemas con el acceso, los archivos pueden descargarse manualmente desde los enlaces proporcionados y cargarse directamente en el proyecto.

---

# **Notas Adicionales**

- Todos los análisis y visualizaciones se generaron con datos simulados proporcionados por Alura para fines de entrenamiento y desarrollo de habilidades de Ciencia de Datos.
- Este proyecto sigue buenas prácticas de visualización y storytelling analítico.

# **Autor**
Evelyn Pareja Ríos 

Proyecto realizado como parte del Challenge de Data Science - Alura Latam.
