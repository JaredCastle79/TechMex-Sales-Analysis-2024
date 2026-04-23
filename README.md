# Análisis de Ventas TechMex 2024

## Descripción del Proyecto
TechMex es una empresa mexicana de tecnología con presencia en 5 ciudades. 
El Director Comercial necesitaba entender el comportamiento de ventas del año 
2024 para tomar decisiones de inversión para el siguiente año. Se realizó un 
análisis completo de 500 transacciones cubriendo regiones, productos, 
vendedores y tendencias temporales.

## Problema que resolvimos
El equipo directivo no tenía claridad sobre:
- Qué región estaba generando menos ingresos y por qué
- Si el producto más vendido era también el más rentable
- Si existían caídas estacionales que requirieran atención inmediata

## Lo que hicimos
**Limpieza y preparación de datos**
- Revisión de nulos, duplicados y tipos de datos
- Creación de columnas calculadas: venta bruta, descuento en pesos, 
  venta neta y margen de ganancia

**Análisis con SQL**
- Ventas y participación porcentual por región usando subconsultas
- Ranking de productos por rentabilidad con window functions (RANK)
- Tendencia mensual con variación porcentual mes a mes usando LAG y CTEs

**Visualizaciones**
- Dashboard de 4 gráficas: ventas por región, tendencia mensual, 
  margen por categoría y ranking de productos
- Exportado como imagen e incrustado directamente en el Excel

**Reporte en Excel**
- 4 hojas: Por Región, Por Producto, Tendencia Mensual, Data Completa
- Dashboard visual incrustado en el archivo

## Hallazgos principales
- CDMX concentra el 35% de los ingresos totales — riesgo de dependencia regional
- La Laptop es el producto más vendido Y el más rentable con margen del 38%
- Mayo registró una caída del 63% vs el mes anterior — posible efecto post-Semana Santa
- Septiembre fue el mejor mes del año con $3M MXN en ventas

## Recomendación al director
Concentrar el presupuesto de marketing en Q3 para capitalizar el pico de 
septiembre, y diseñar una promoción en mayo para suavizar la caída estacional.

## Herramientas utilizadas
- **Python** — pandas, matplotlib, seaborn, numpy
- **SQL** — SQLite con GROUP BY, window functions, CTEs y LAG
- **Excel** — reporte multi-hoja con dashboard incrustado

## Archivos
- `Dia1_ef.ipynb` — notebook completo con análisis
- `Reporte_TechMex_2024.xlsx` — reporte Excel con dashboard
