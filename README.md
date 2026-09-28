# Proyecto Final - Text Mining & Image Recognition

Postgrado en Análisis y Predicción de Datos, Universidad Galileo
Tercer Trimestre, 2026

## Contenido

El notebook `Proyecto_Final.ipynb` contiene los dos problemas del proyecto:

**Problema 1 - Word Cloud:** identificación de los 3 usuarios más mencionados en un dataset de 1.6 millones de tweets (Sentiment140), construcción de un corpus por usuario y análisis del contexto de las menciones mediante remoción de stopwords, lematización, stemming y wordclouds.

**Problema 2 - Fruits and Vegetables Recognizer:** clasificación de imágenes de 3 frutas (manzana, banana, naranja) y 3 verduras (zanahoria, papa, pepino) con redes neuronales convolucionales. Se compararon 3 arquitecturas y se evaluó su robustez ante rotación, escala e iluminación.

## Resultados principales

| Problema | Resultado |
|---|---|
| 1 | Usuarios más mencionados: @mileycyrus (4,580), @tommcfly (3,904) y @ddlovato (3,474) |
| 2 | Modelo seleccionado: CNN con filtros de 5×5 y AveragePooling. Accuracy en prueba: 98.57% (imágenes originales) y 97.97% (imágenes modificadas) |

## Datasets

Los datasets no se incluyen en el repositorio por su tamaño.

- Problema 1: Sentiment140 - [enlace de descarga](https://drive.google.com/file/d/1zIo_BgbuuoN_gCU_kpimZ4PMX8t0C0hI/view)
- Problema 2: Fruits and Vegetables Dataset - [enlace de Kaggle](https://www.kaggle.com/datasets/muhriddinmuxiddinov/fruits-and-vegetables-dataset)

Para ejecutar el notebook, los datasets deben ubicarse así:

    Proyecto/
    ├── tw_source.csv/tw_source.csv
    ├── archive/Fruits_Vegetables_Dataset(12000)/
    └── Proyecto_Final.ipynb

## Ejecución

    python -m venv .venv
    .venv\Scripts\activate
    pip install -r requirements.txt

Luego se abre `Proyecto_Final.ipynb` y se selecciona el kernel `.venv`. El Problema 2 se puede ejecutar de forma independiente desde la celda "Problema 2", sin volver a cargar el dataset de tweets.
