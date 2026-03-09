

# Telecom X Parte 2 - Challenger Final- Predicción de Cancelación de Clientes (Churn)
![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple)
![Scikit-Learn](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Challenge](https://img.shields.io/badge/Challenge-Telecom%20X-blue)
![Status](https://img.shields.io/badge/Project-Completed-green)

## 🧰 Tecnologías utilizadas

<p align="left">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" width="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matplotlib/matplotlib-original.svg" width="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/scikitlearn/scikitlearn-original.svg" width="40"/>
</p>

## 📊 Modelos utilizados

- Regresión Logística
- Random Forest

Ambos modelos fueron evaluados utilizando métricas como accuracy, precision, recall, F1-score y matriz de confusión.

  
## 📌 Descripción del proyecto

Este proyecto tiene como objetivo desarrollar modelos de Machine Learning capaces de predecir la cancelación de clientes (churn) en Telecom X.

La cancelación de clientes representa un problema importante para las empresas de telecomunicaciones, ya que implica pérdida de ingresos y aumento en los costos de adquisición de nuevos clientes. Por ello, identificar de forma anticipada qué clientes tienen mayor probabilidad de cancelar el servicio permite implementar estrategias de retención más efectivas.

En este proyecto se analizan diferentes variables relacionadas con el comportamiento de los clientes y se construyen modelos predictivos que permiten estimar la probabilidad de cancelación.

---

# 🎯 Objetivo

Construir modelos de clasificación que permitan identificar clientes con mayor probabilidad de cancelar sus servicios, utilizando variables relacionadas con características del cliente, tipo de contrato y cargos del servicio.

---

# 📂 Estructura del proyecto
<img width="486" height="127" alt="image" src="https://github.com/user-attachments/assets/3462450d-0962-49b5-9dbf-65dfb7c22d0e" />


---

# 📊 Preparación de los datos

El dataset utilizado fue previamente tratado en la Parte 1 del Challenge Telecom X.

Durante la preparación de los datos se realizaron las siguientes etapas:

### Clasificación de variables

Las variables del dataset se clasificaron en:

- **Variables categóricas**
  - Género
  - Tipo de contrato
  - Servicios de internet
  - Servicios adicionales

- **Variables numéricas**
  - Tiempo de permanencia del cliente (tenure)
  - Cargos mensuales
  - Cargos totales

### Transformación de variables

Se realizaron los siguientes procesos de preparación de datos:

- Eliminación de columnas irrelevantes (por ejemplo: `customerID`).
- Codificación de variables categóricas utilizando **One-Hot Encoding**.
- Verificación de la proporción de cancelación (Churn).
- Análisis de correlación entre variables.

### División de datos

El dataset fue dividido en:

- **70% datos de entrenamiento**
- **30% datos de prueba**

Esta separación permite evaluar el rendimiento del modelo en datos no utilizados durante el entrenamiento.

---

## 🤖 Modelos Evaluados

Para predecir la cancelación de clientes se entrenaron y evaluaron dos modelos de clasificación:

- **Regresión Logística**
- **Random Forest**

La Regresión Logística requiere normalización de los datos, por lo que se aplicó **StandardScaler** antes del entrenamiento.  
Por otro lado, **Random Forest** no depende de la escala de los datos, por lo que se entrenó directamente sobre los datos originales.

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

### Modelo Seleccionado

El modelo **Random Forest** presentó un mejor desempeño general en comparación con la Regresión Logística, logrando capturar mejor las relaciones entre las variables del dataset.

Además, Random Forest permite analizar la **importancia de las variables**, lo que facilita identificar los factores que influyen en la cancelación de clientes.

---

# 📈 Métricas de evaluación

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy (Exactitud)
- Precision
- Recall
- F1-score
- Matriz de confusión

Estas métricas permiten analizar el desempeño del modelo y su capacidad para identificar correctamente clientes con riesgo de cancelación.

---

# 📊 Análisis exploratorio (EDA)

Durante el análisis exploratorio se identificaron patrones importantes en los datos.

Entre los principales hallazgos se destacan:

- Clientes con **contratos mensuales** presentan mayor probabilidad de cancelación.
- Clientes con **menor tiempo de permanencia** en la empresa presentan mayor riesgo de churn.
- Clientes con **cargos mensuales elevados** tienden a cancelar con mayor frecuencia.

Estos insights permiten comprender mejor los factores asociados a la cancelación.

---

# 📌 Conclusiones

El análisis permitió identificar variables clave que influyen en la cancelación de clientes.

Entre los factores más relevantes se encuentran:

- Tipo de contrato
- Tiempo de permanencia del cliente
- Cargos mensuales del servicio

El modelo Random Forest mostró un desempeño superior para predecir la cancelación, al capturar relaciones más complejas entre las variables.

---

# 💡 Recomendaciones para Telecom X

A partir de los resultados obtenidos se sugieren las siguientes estrategias:

- Incentivar contratos de mayor duración.
- Implementar programas de fidelización para clientes nuevos.
- Ofrecer beneficios o descuentos a clientes con cargos mensuales elevados.

Estas estrategias pueden contribuir a reducir la cancelación de clientes y mejorar la retención.

---

# ⚙️ Cómo ejecutar el proyecto

1. Clonar el repositorio o descargar los archivos.

2. Instalar las bibliotecas necesarias:
```python
pip install pandas numpy matplotlib seaborn scikit-learn'
```

3. Abrir el notebook:
```
telecom_churn_prediction.ipynb
```
4. Ejecutar todas las celdas para reproducir el análisis y los modelos.

---


