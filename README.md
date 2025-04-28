# Analisis De Datos Alura Store

## **Descripción del Proyecto**

Este proyecto tiene como objetivo analizar datos de ventas de cuatro tiendas de la cadena **Alura Store** para identificar cuál de ellas sería más recomendable vender, basándose en criterios financieros, geográficos, de satisfacción del cliente y desempeño de productos.

Se utilizaron herramientas de análisis de datos, visualización gráfica y geolocalización para obtener una visión integral del rendimiento de cada tienda.

## **Herramientas Utilizadas**

- Python
- Pandas
- Matplotlib
- Seaborn
- Folium
- Numpy

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
> Vender la Tienda 4 y concentrar esfuerzos en fortalecer la Tienda 3, que muestra el mejor desempeño general.

---

# **Estructura de Carpetas**

```bash
Proyecto_Alura_Store/
│
├── datos/
│   ├── tienda_1.csv
│   ├── tienda_2.csv
│   ├── tienda_3.csv
│   └── tienda_4.csv
│
├── notebooks/
│   ├── analisis_ventas.ipynb
│   ├── analisis_categorias.ipynb
│   ├── analisis_geografico.ipynb
│
├── mapas/
│   ├── mapa_heatmap
│   ├── mapa_distribucion
│   └── mapa_zonas_dominantes
│
├── graficos/
│   ├── ingresos_tiendas.png
│   ├── categorias_mas_vendidas.png
│   └── calificaciones_promedio.png
│
└── README.md
```

---

# **Notas Adicionales**

- Todos los análisis y visualizaciones se generaron con datos simulados proporcionados por Alura para fines de entrenamiento y desarrollo de habilidades de Ciencia de Datos.
- Este proyecto sigue buenas prácticas de visualización y storytelling analítico.
