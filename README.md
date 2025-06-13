Microsoft Edge settings and storage represent user-selected preferences and information and MUST not be extracted, overwritten or modified except through Microsoft Edge defined APIs.

# 📘 Proyecto Datathon – Cobertura educativa en Colombia

## 🎯 Descripción del reto

En este proyecto abordamos la cobertura educativa en Colombia por departamentos y zona (urbana, rural) y la matrícula contratada.

## Pregunta de investigación

> ¿Existen brechas en la cobertura geográfica de los establecimientos educativos en Colombia por departamento y zona, y cómo se distribuyen estos establecimientos según si tienen matrícula contratada (paga) o no?

## 💡 Hipótesis

> La cobertura geográfica de los establecimientos educativos en Colombia presenta desigualdades significativas entre zonas urbanas y rurales, y una mayor concentración de matrícula contratada (paga) en zonas urbanas y departamentos con mayor desarrollo económico".

## 🧭 Objetivo general

> Analizar la cobertura geográfica de los establecimientos educativos en Colombia, por departamento y zona, y evaluar la distribución de establecimientos con matrícula contratada (paga) en relación con su ubicación.

## 🎯 Objetivos específicos

1) Identificar la distribución de los establecimientos educativos por departamento.
2) Comparar la cobertura educativa por departamento entre las zonas (urbana y rural).
3) Analizar la proporción de establecimientos educativos que cuentan con matrícula contratada frente a los que no, según departamento y zona. 
4) Visualizar geográficamente la presencia y ausencia de matrícula contratada (paga) en los establecimientos educativos por departamento.

## Proceso de Limpieza Base de Datos
Grupo Analytik BQ  Ejecución de los Procesos ETL Y EDA Base de datos ESTABLECIMIENTOS_EDUCATIVOS-COLOMBIA_20250604

1.	Iniciamos nuestro proceso de ETL Y EDA, en la aplicación Colab. Redactando la pregunta de Investigación, Objetivo general y  específicos e hipótesis de nuestro proyecto. 
PROCESO EXTRACT
2.	Se realizó el cargue de Librerías 
●	 pandas: para manipulación y análisis de datos.
●	matplotlib: para la generación de gráficos y visualizaciones.
3.	Realizamos el cargue y  la lectura del archivo CSV. revisando las filas que contiene, para conocer la estructura del dataset, encontrando 22530 Filas y 35 Columnas.
PROCESO  TRANSFORM
4.	 Revisamos los valores únicos del data frame,  identificando especialmente columnas  claves  como Departamento, Zona, Matrícula entre otras, de acuerdo a nuestros objetivos,  para entender las categorías disponibles y detectar posibles inconsistencias.
5.	Se consultan valores duplicados, y  se verifican.
6.	Realizamos  eliminación de columnas Innecesarias, Eliminado en total 18 Columnas y 4 valores Duplicados. 
7.	Se realizó la limpieza de la columna zona  Estandarizando los valores de la columna (zona-rural) 
8.	Corregir Entradas inconsistentes como rural- urbana o urbana-rural
9.	Se unificaron estos valores en rural o urbana como corresponda.
10.	También se identificaron valores Nulos o faltantes.
11.	Se normaliza el carácter especial en las columnas para visualizar de forma correcta el nombre de los municipios.
PROCESO EDA
12.	Se creó un nuevo DataFrame df_cleaned con los datos limpios, que servirá como base para el análisis posterior.
13.	Se carga y conecta  el dataset limpio y se procede a leer nuevamente los datos depurados. 
14.	Se procede a cargar las librerías que son esenciales para manipulación de datos (pandas) y visualización de gráficos (matplotlib).
import pandas as pd
import matplotlib.pyplot as plt
15.	Se realiza una revisión de las columnas únicas por categorías de acuerdo a nuestros objetivos como  Departamento, Zona, Matrícula.
16.	Y ya podemos realizar un primer analisis afirmando que entre mas poblado es un departamento mas instituciones educativas tiene. 
Nota: En nuestro  dashboard  crear una tabla de establecimientos totales por departamento. Tambien se puede evidenciar que en los municipios con menor poblacion existe mayor % de establecimientos con matriculas pagas. 

## 🛠️ Herramientas utilizadas

- **Python**: pandas, matplotlib, seaborn (limpieza, EDA, análisis, visualizaciones, Machine Learning)
- **Google Colab**: Entorno de desarrollo
- **Power BI**: dashboard de visualización
- **GitHub**: control de versiones y trabajo colaborativo
- **Trello**: planificación ágil de tareas (SCRUM) (https://trello.com/b/hsfBRSzu/datathon-inclusion-educativa)
- **Canva / PowerPoint**: presentación final TED Talk

## 👥 Roles del equipo

- Nombre: María José Palomino Vargas: Coordinación general, Trello, control de entregables
- Nombre: Rosalyn Reyes: Creación de logo e identidad de marca del equipo 
- Nombre: Zuly Romero: Limpieza de datos y codificación inicial
- Nombre: Dayana Sepulveda: Análisis exploratorio (EDA) y visualizaciones en Python, Machine Learning
- Nombre: Yureinis Manotas: Diseño de dashboard en Power BI
- Nombre: Ivy Bonilla: Storytelling y presentación TED
- Nombre: María José Palomino Vargas Documentación, GitHub, README, commits

## 🔍 Flujo de trabajo

1. Revisión y limpieza del dataset nacional
2. Identificación de variables clave de inclusión
3. Análisis exploratorio por tipo de institución, zona y departamento
4. Desarrollo del dashboard interactivo
5. Redacción del guion y preparación de la TED Talk
6. Subida de entregables al repositorio

## 📊 Visualizaciones principales

- Gráfico de anillos cobertura por departamentos
- Gráfico de barras apiladas matrícula contratada por zonas
- Gráficos de barras agrupadas por departamento y zonas
- Mapa geográfico por departamento y matrícula contratada

  ## 📄✅ Entregables del proyecto
1. Repositorio en GitHub con:
    -Notebooks scripts de trabajo (limpieza, EDA, modelado, visualizaciones).
    -Archivo README con descripción del reto, hipótesis, enfoque, roles y pasos realizados
    -Evidencias de trabajo colaborativo: issues, branches, commits, pull requests, acceso tablero Kanban (Trello, Jira, Excel)
    -Dump o exportación de base de datos usada (.sql o .json/.csv según corresponda)
2. Dashboard con visualizaciones en Power BI o Tableau
4. Presentación final tipo TED Talk corporativo archivo de presentación .pptx o PDF
5. Identidad visual del equipo o Logo, fondo para videollamada, tono de comunicación, presentación.






