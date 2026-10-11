# Proyecto Integrador ETL - Food Delivery

Proyecto final para el curso de Python para Análisis de Datos (ETL). Consiste en procesar y analizar información de restaurantes y sus menús para responder a una serie de preguntas de negocio sobre un servicio de delivery.

## Pasos del trabajo

1. Extract: Se cargaron los archivos CSV de restaurantes y menús con pandas para revisar cómo venían los datos (filas, columnas y nulos).
2. Transform: Se cambiaron los símbolos de precio por texto, se separó la columna de dirección en calle, ciudad y estado, se limpiaron los precios de los menús dejándolos en números flotantes, y se filtraron los restaurantes con más de 100 calificaciones para cruzarlos con los menús en la tabla df_master.
3. Load: Se creó la base de datos local delivery_insights.db en SQLite y se guardó la tabla master_food_data.
4. Business Intelligence: Se hicieron consultas SQL desde Python (pd.read_sql) y se armaron gráficos con matplotlib y seaborn para analizar los resultados.

## Principales conclusiones

- Milwaukee y Seattle son las ciudades que tienen más restaurantes consolidados.
- Casi todos los restaurantes (99.3%) son de precio económico o moderado.
- En Seattle se encuentra el precio promedio por plato más alto ($11.98 USD) entre las ciudades principales.
- La nota o puntaje que le dan los usuarios a los restaurantes no cambia mucho según el precio, manteniéndose cerca de 4.6 en promedio.

## Herramientas usadas

- Python (pandas, numpy, sqlalchemy, matplotlib, seaborn)
- Base de datos: SQLite
- Entorno: Databricks