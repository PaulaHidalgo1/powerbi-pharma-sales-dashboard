# Dashboard de Ventas Farmacéuticas en Power BI

## Descripción del proyecto
Este proyecto consiste en la creación de un **dashboard interactivo en Power BI** para el análisis de ventas farmacéuticas mensuales. El objetivo es visualizar de forma clara la evolución de las ventas, comparar el rendimiento de las distintas categorías de medicamentos y destacar las categorías con mayor volumen de ventas.

---

## Dataset
Se utiliza el archivo `salesmonthly.csv`, que contiene datos agregados de ventas mensuales de diferentes categorías de medicamentos según la clasificación ATC.

- Número de registros: 70
- Variables principales:
  - `datum`: fecha (mes)
  - Categorías de medicamentos: M01AB, M01AE, N02BA, N02BE, N05B, N05C, R03, R06

---

## Herramientas utilizadas
- Power BI Desktop
- Power Query
- CSV

---

## Preparación de los datos
Antes de la visualización, se realizaron las siguientes transformaciones en Power Query:
- Conversión de la columna `datum` al tipo fecha.
- Creación de una columna calculada **Total Sales**, que representa el total de ventas mensuales sumando todas las categorías.
- Transformación de las columnas de categorías a un formato categórico mediante **unpivot**, permitiendo el análisis por categoría y la aplicación de filtros Top N.

---

## Visualizaciones del dashboard
El dashboard incluye los siguientes elementos:
- **Gráfico de líneas**: evolución de las ventas totales mensuales.
- **Gráfico de columnas**: comparación de ventas por categoría de medicamento.
- **Gráfico de barras (Top 3)**: categorías de medicamentos con mayor volumen de ventas.
- **Tarjeta KPI**: total acumulado de ventas.
- **Segmentador de fecha**: filtro interactivo por periodo temporal.
