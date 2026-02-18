# Predicción y Clasificación de Alquileres en Madrid

## Indice

- [Predicción y Clasificación de Alquileres en Madrid](#predicción-y-clasificación-de-alquileres-en-madrid)
  - [Indice](#indice)
  - [Descripcion del Proyecto](#descripcion-del-proyecto)
  - [Hoja de Ruta del Proyecto](#hoja-de-ruta-del-proyecto)
    - [1. Inicio y Configuracion](#1-inicio-y-configuracion)
    - [2. Entendimiento de los Datos (CRISP-DM)](#2-entendimiento-de-los-datos-crisp-dm)
    - [3. Analisis Exploratorio de Datos (EDA)](#3-analisis-exploratorio-de-datos-eda)
    - [4. Preparacion de Datos con Pipelines](#4-preparacion-de-datos-con-pipelines)
    - [5. Modelado y Evaluacion](#5-modelado-y-evaluacion)
      - [Tarea A: Regresion (price)](#tarea-a-regresion-price)
      - [Tarea B: Clasificacion (balcony)](#tarea-b-clasificacion-balcony)
    - [6. Conclusiones y Documentacion](#6-conclusiones-y-documentacion)
  - [Tecnologias Utilizadas](#tecnologias-utilizadas)
  - [Como Ejecutar el Proyecto](#como-ejecutar-el-proyecto)

---

## Descripcion del Proyecto

Proyecto orientado al analisis, prediccion y clasificacion de alquileres en la provincia de Madrid mediante tecnicas de ciencia de datos y machine learning.

Objetivos principales:

- Predecir el precio de alquiler de una vivienda (tarea de regresion).
- Clasificar si un inmueble dispone de balcon (tarea de clasificacion).

---

## Hoja de Ruta del Proyecto

### 1. Inicio y Configuracion

- Introduccion al proyecto
- Importacion de librerias: Numpy, Pandas, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras
- Carga del dataset: archivo CSV "Madrid Province Rent Data"

---

### 2. Entendimiento de los Datos (CRISP-DM)

- Inspeccion inicial con `.info()`, `.describe()`, `.head()`
- Limpieza de datos:
  - Gestion de valores nulos
  - Eliminacion de duplicados
  - Conversion de tipos
  - Correccion de inconsistencias en year_built, floor, price

---

### 3. Analisis Exploratorio de Datos (EDA)

- Analisis univariante: histogramas de precio, area, habitaciones
- Analisis bivariante y multivariante:
  - Diagramas de dispersion
  - Relplot con hue o size
  - Matriz de correlacion
- Deteccion de outliers
- Estandarizacion para comparacion de distribuciones

---

### 4. Preparacion de Datos con Pipelines

- Definicion de features (X) y target (y)
  - Regresion: price
  - Clasificacion: balcony
- Preprocesamiento:
  - Numericas: imputacion, transformacion logaritmica, escalado
  - Categoricas: One-Hot Encoding u Ordinal Encoding
- Division del dataset en train y test

---

### 5. Modelado y Evaluacion

#### Tarea A: Regresion (price)

Modelos:

- LinearRegression
- RandomForestRegressor
- Red neuronal con TensorFlow/Keras

Metricas:

- MSE
- RMSE
- MAE
- R2

#### Tarea B: Clasificacion (balcony)

Modelos:

- LogisticRegression
- DecisionTreeClassifier
- Red neuronal con TensorFlow/Keras

Metricas:

- Accuracy
- Precision
- Recall
- F1-score

---

### 6. Conclusiones y Documentacion

- Justificacion de decisiones metodologicas
- Interpretacion de resultados
- Limitaciones del estudio
- Propuestas de mejora futura

---

## Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow / Keras

---

## Como Ejecutar el Proyecto
