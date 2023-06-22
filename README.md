# Analisis_Predictivo_Datos
Realización de los distintos trabajos práctico de Análisis Predictivo de Datos

## Trabajo 1: Procesamiento de datos

  En la carpeta `data` se encuentra los datos crudos de ventas durante el 2022 de las diferentes sedes de una cadena de tiendas DuttyFree ubicadas en distintos aeropuertos del país.
  Esta información se encuentra en distintos archivos en formato `.parquet` los cuales deben ser reconstruidos. La compañía desea analizar los datos para apoyar su proceso de toma de decisiones. Sin embargo, estos datos son recolectados manualmente desde cada una de las sedes por lo que se requiere previamente realizar una limpieza y procesamiento de los datos.

## Trabajo 2: Árboles de Decisión y Regresiones Lineales

1. Análisis descriptivo de los datos. Se realiza:
    - Una descripción de cada variable del conjunto de datos.
    - Un recuento de variables nulas en los datos.
    - Un histograma de frecuencias de cada variable.
    - Un gráfico de barras comparando cada variable con la variable objetivo.
    - Un gráfico de mapa de calor de la correlación de los datos.
2. Modelo de árbol de decisión regresor.
    - Se divide el conjunto de datos en un conjunto de entrenamiento y un conjunto de prueba.
    - Se crean variables Dummy para las variables categóricas.
    - Se crea y entrena un modelo de árbol de decisión regresor.
    - Se entrenan lo hiperparámetros para ajustar el modelo.
    - Del modelo resultante, se calcula:
        - Score.
        - Mean Square Error.
        - Root of Mean Square Error.
3. Modelo de regresión lineal.
    - Estandarización de las variables numéricas utilizando la técnica `Z-Score`.
    - Creeación de variables Dummy para las variables categóricas.
    - Se divide el conjunto de datos en un conjunto de entrenamiento y un conjunto de prueba.
    - Se crea y entrena un modelo de regresión lineal múltiple.
    - Del modelo resultante, se calcula:
        - Score.
        - Mean Square Error.
        - Root of Mean Square Error.
4. De acuerdo a los resultados de los modelos, se argumenta cuál es el mejor.

## Trabajo 3: Clasificación de Imágenes de Aves de India

Se desea realizar una red neuronal que permita clasificar las especies de aves y para ello, utilice la técnica de Transferencia de Aprendizaje (Transfer Learning) para utilizar una red previamente entrenada y desarrollar un nuevo modelo.

Para hacer el entrenamiento, se debe descargar el archivo que contiene las imágenes del siguiente link:
https://drive.google.com/drive/folders/1F65hb4eVq8MqsCkeuolLTHI8302NsvrI?usp=sharing

Este data set contiene una serie de imágenes de aves comunes de India, las cuales se dividen en ciertas categorías distintas. Adicionalmente, cada categoría se ha dividido en 2 grupos, `/train` y `/valid`. Es decir, un grupo para entrenamiento y otro para validación.

Este archivo contiene la siguiente estructura

- filtered_training_set
    - train
        - Asian Green Bee-Eater
        - Brown-Headed Barbet
        - **...**
        - White-Breasted Waterhen
    - valid
        - Asian Green Bee-Eater
        - Brown-Headed Barbet
        - **...**
        - White-Breasted Waterhen
        
Las categorías de cada imagen se encuentran según la carpeta donde estén alojadas las imágenes.

## Trabajo Final: Detección de fraude

En este archivo se decide entrenar una red neuronal con el fin de detectar fraude en transacciones bancarias. Para esto, se toma de base un archivo `CSV` el cual contiene distintas categorías las cuales son:
- step
- type
- amount
- nameOrig
- oldbalanceOrg
- newbalanceOrig
- nameDest
- oldbalanceDest
- newbalanceDest
- isFraud
- isFlaggedFraud
  
Para este trabajo se hará uso de una librería de Python llamada `imbalanced-learn`, la cual nos permitirá analizar los datos del archivo `CSV` y hacer un análisis de los datos que están desbalanceados.

Se debe hacer un análisis de los datos para detemrinar si es necesario eleminar algún tipo de dato que no sea relevante para el estudio y entrenamiento de la red neuronal.
