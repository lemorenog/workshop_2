
# Inteligencia Artificial - Clasificación y Regresión

Este repositorio contiene el desarrollo completo de dos problemas principales de aprendizaje supervisado aplicados a datos biomédicos y de imágenes:

- **Problema 1:** Clasificación de fatiga muscular en ciclismo a partir de señales EMG.
- **Problema 2:** Regresión para estimar la edad a partir de imágenes faciales.

## Estructura del Proyecto

workshop_2/

├── README.md        

├── clasificacion/

│   ├── clasificacion.ipynb

│  

├── regresion/

│   ├── regresion.ipynb

│ 

---

## 1. Clasificación: Detección de Fatiga Muscular en Ciclismo

**Archivo:** [`clasificacion.ipynb`](clasificacion.ipynb)

- **Descripción:**  
  Se aborda la detección automática de fatiga muscular usando señales electromiográficas (EMG) multicanal. El flujo incluye:
  - Preprocesamiento y reducción del problema a dos clases (normal vs. desgaste).
  - Extracción de características en ventanas de 1 segundo (dominio tiempo y frecuencia).
  - Análisis exploratorio de datos (EDA) con visualizaciones y estadísticas.
  - Entrenamiento y comparación de modelos clásicos (kNN, Árboles, Random Forest, Gradient Boosting) y una Red Neuronal Profunda (DNN).
  - Evaluación crítica de resultados, análisis de overfitting/underfitting y selección del mejor modelo.
  - Pruebas con muestras artificiales y análisis de interpretabilidad.

- **Secciones clave:**
  - Análisis preliminar y EDA.
  - Feature engineering y construcción del dataset.
  - Entrenamiento, ajuste de hiperparámetros y comparación de modelos.
  - Evaluación final y visualización de resultados.

---

## 2. Regresión: Estimación de Edad a partir de Imágenes Faciales

**Archivo:** [`regresion.ipynb`](regresion.ipynb)

- **Descripción:**  
  Se desarrolla un modelo de regresión ordinal para estimar el grupo de edad (joven, medio, viejo) a partir de imágenes faciales. El flujo incluye:
  - Análisis exploratorio del dataset de imágenes (dimensiones, balance de clases, visualización).
  - Preprocesamiento: redimensionamiento, normalización y data augmentation.
  - Implementación de un pipeline reproducible con TensorFlow.
  - Diseño, entrenamiento y evaluación de una CNN custom para regresión.
  - Análisis de métricas (MAE, RMSE, R²), curvas de aprendizaje y diagnóstico de ajuste.
  - Pruebas de robustez ante transformaciones visuales y análisis crítico de resultados.

- **Secciones clave:**
  - EDA y justificación del enfoque de regresión ordinal.
  - Pipeline de procesamiento de imágenes.
  - Arquitectura y entrenamiento de la CNN.
  - Evaluación y análisis de errores.
  - Pruebas de robustez y discusión de resultados.

---

## Requisitos

- Python 3.8+
- Jupyter Notebook
- Bibliotecas: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `tensorflow`, `Pillow`, `scipy`, `datasets`

Instala los requisitos con:

```sh
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow pillow scipy datasets
