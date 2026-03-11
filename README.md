# Telecom X - Parte 2: Predicción de Cancelación de Clientes (Churn)

## Descripción del Proyecto

Este proyecto forma parte del programa **Oracle Next Education (ONE) en colaboración con Alura Latam** y tiene como objetivo desarrollar modelos de **Machine Learning capaces de predecir la cancelación de clientes (Churn)** en la empresa Telecom X.

En la **Parte 1 del desafío**, se realizó el proceso ETL y análisis exploratorio de los datos.  
En esta **Parte 2**, se construyen modelos predictivos que permiten identificar clientes con mayor riesgo de cancelación.

El objetivo final es proporcionar información estratégica que permita a Telecom X **anticipar la pérdida de clientes y diseñar estrategias de retención más efectivas**.

---

# Objetivo del Análisis

Desarrollar modelos predictivos que permitan:

- Identificar clientes con **mayor probabilidad de cancelar el servicio**
- Analizar **qué variables influyen más en el churn**
- Evaluar el desempeño de diferentes algoritmos de Machine Learning
- Generar **insights estratégicos para reducir la cancelación de clientes**

---

# Tecnologías Utilizadas

El proyecto fue desarrollado en **Python** utilizando las siguientes bibliotecas:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

---

# Estructura del Proyecto


TelecomX-Churn-Prediction/
│
├── TelecomX_Parte2.ipynb
├── datos_tratados.csv
├── README.md


### Archivos principales

**TelecomX_Parte2.ipynb**  
Notebook principal que contiene:

- Preparación de datos
- Análisis exploratorio adicional
- Construcción de modelos
- Evaluación de desempeño
- Interpretación de resultados

**datos_tratados.csv**  
Dataset limpio generado en la Parte 1 del desafío.

**README.md**  
Documentación del proyecto.

---

# Preparación de los Datos

Se utilizaron los datos tratados en la Parte 1 del desafío, que ya habían pasado por un proceso de limpieza y estandarización.

Las principales etapas de preparación incluyeron:

- Eliminación de columnas irrelevantes (por ejemplo, identificadores de clientes)
- Conversión de variables categóricas a variables numéricas mediante **One-Hot Encoding**
- Verificación de valores faltantes
- Análisis de correlación entre variables
- Análisis dirigido de variables clave como:

  - Tiempo de contrato
  - Gasto mensual
  - Gasto total

---

# Balanceo de Clases

Se analizó la proporción de cancelación de clientes utilizando:

```python
df['churn'].value_counts(normalize=True)
