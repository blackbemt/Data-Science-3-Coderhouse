# Proyecto Final - Data Science III

Este repositorio contiene el trabajo final del curso **Data Science III**, donde se abordaron dos subcampos clave del aprendizaje automático: **Procesamiento de Lenguaje Natural (NLP)** y **Deep Learning aplicado a imágenes**.

---

## Proyecto 1: Clasificación de Texto con NLP

En la primera parte del proyecto se trabajó con un conjunto de datos de reseñas en texto. Se desarrollaron las tareas más usuales de preprocesamiento de NLP.

- **Limpiar y normalizar texto** (minúsculas, stopwords, lematización).
- **Tokenizar y vectorizar** mediante técnicas como Bag of Words o TF-IDF.
- **Detectar los idiomas** mediante langdetect

---

## Proyecto 2: Clasificador de Imágenes con Deep Learning

El segundo y más extenso proyecto consistió en desarrollar una **red neuronal convolucional (CNN)** para clasificar imágenes de **perros y gatos**.

### Objetivo

Construir un modelo capaz de aprender diferencias visuales entre ambas clases y generalizar su aprendizaje a nuevas imágenes.

### Dataset

Se utilizó un conjunto de imágenes redimensionadas a 150x150 pixeles y convertidas a escala de grises, dividido en conjuntos de entrenamiento, validación y prueba.

### Arquitectura del Modelo

El modelo CNN fue construido con `Keras` y `TensorFlow`, incluyendo:

- Varias capas `Conv2D` con `ReLU` y `MaxPooling`.
- `BatchNormalization` y `Dropout` para combatir el sobreajuste.
- Capa `Flatten` y `Dense` con activación `sigmoid` para clasificación binaria.

### Aumento de Datos (Data Augmentation)

Se aplicó `ImageDataGenerator` para generar nuevas imágenes de entrenamiento mediante rotación, desplazamientos y volteos horizontales. Esto **mejoró considerablemente la capacidad de generalización** del modelo.

### Resultados Finales

Tras la optimización y aumento de datos:

- **Precisión (Accuracy):** `93%`
- **Precision / Recall / F1-score (ambas clases):** `0.91` | 
- **Balance perfecto** entre gatos y perros, sin sesgo hacia una clase.

### Conclusión

> El modelo CNN superó ampliamente a una clasificación aleatoria (≈50%) y alcanzó un rendimiento robusto y estable. La técnica de data augmentation fue determinante para mejorar el desempeño y reducir el sobreajuste.

---

## Tecnologías Utilizadas

- Python
- TensorFlow / Keras
- Scikit-learn
- Matplotlib / Seaborn
- Numpy / Pandas
- NLTK / re (para NLP)

---
