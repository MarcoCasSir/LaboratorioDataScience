📘 HOJA DE RUTA DEL PROYECTO
Predicción y Clasificación de Alquileres en Madrid

1. Inicio y Configuración
   📌 Introducción

Proyecto orientado al análisis, predicción y clasificación de alquileres en la provincia de Madrid mediante técnicas de ciencia de datos y machine learning.
📌 Importación de librerías

Se utilizarán:

    Numpy

    Pandas

    Matplotlib

    Seaborn

    Scikit‑learn

    TensorFlow / Keras

📌 Carga del dataset

Lectura del archivo CSV Madrid Province Rent Data. 2. Entendimiento de los Datos (CRISP‑DM)
📌 Inspección inicial

Uso de:

    .info()

    .describe()

    .head()

Para revisar columnas como price, floor_area, bedrooms, district, etc.
📌 Limpieza de datos (Data Wrangling)

    Gestión de valores nulos

    Eliminación de duplicados

    Conversión de tipos (texto → numérico cuando corresponda)

    Corrección de inconsistencias en year_built, floor, price

3.  Análisis Exploratorio de Datos (EDA)
    📌 Análisis univariante

        Histogramas de precio, área, habitaciones, etc.

📌 Análisis bivariante y multivariante

    Diagramas de dispersión (ej. floor_area vs price)

    relplot con hue o size para relaciones complejas

    Matriz de correlación

📌 Detección de outliers

Identificación de valores extremos que puedan sesgar el modelo.
📌 Estandarización

Comparación de densidades en un dataframe escalado para evaluar distribuciones. 4. Preparación de Datos con Pipelines
📌 Definición de features (X) y target (y)

    Regresión: price

    Clasificación: balcony

📌 Pipeline de preprocesamiento

    Variables numéricas:

        Imputación

        Transformación logarítmica (si hay asimetría)

        Escalado / normalización

    Variables categóricas:

        One‑Hot Encoding u Ordinal Encoding (district, orientation, etc.)

📌 División del dataset

Separación en train y test. 5. Modelado y Evaluación
🟦 Tarea A: Regresión (variable price)

Modelos:

    LinearRegression

    RandomForestRegressor

    Red neuronal con TensorFlow/Keras

Métricas:

    MSE

    RMSE

    MAE

    R²

🟩 Tarea B: Clasificación (variable balcony)

Modelos:

    LogisticRegression

    DecisionTreeClassifier

    Red neuronal con TensorFlow/Keras

Métricas:

    Accuracy

    Precision

    Recall

    F1‑score

6. Conclusiones y Documentación

   Justificación de las decisiones metodológicas

   Interpretación de resultados

   Limitaciones del estudio

   Propuestas de mejora futura
