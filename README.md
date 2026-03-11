# Telecom X – Parte 2: Predicción de Cancelación de Clientes (Churn)

## Descripción del Proyecto

Este proyecto forma parte del programa **Oracle Next Education (ONE) en colaboración con Alura Latam**. El objetivo es desarrollar modelos de **Machine Learning capaces de predecir la cancelación de clientes (Churn)** en la empresa Telecom X.

En la **Parte 1 del desafío**, se realizó el proceso de **ETL (Extracción, Transformación y Limpieza de datos)** junto con un análisis exploratorio (EDA).

En esta **Parte 2**, se utilizan los datos tratados para construir modelos predictivos que permitan identificar clientes con mayor probabilidad de cancelar el servicio.

El objetivo final es ayudar a Telecom X a **anticiparse a la pérdida de clientes y diseñar estrategias de retención más efectivas**.

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

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

---

# Estructura del Proyecto
TelecomX-Churn-Prediction
│
├── TelecomX_Parte2.ipynb
├── datos_tratados.csv
└── README.md


### Archivos principales

**TelecomX_Parte2.ipynb**

Notebook principal que contiene:

- Preparación de los datos
- Análisis de correlación
- Entrenamiento de modelos de Machine Learning
- Evaluación de desempeño
- Interpretación de resultados

**datos_tratados.csv**

Dataset limpio generado en la **Parte 1 del desafío**, utilizado para entrenar los modelos predictivos.

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

# Análisis de la Proporción de Cancelación

Se analizó la distribución de la variable **churn** para verificar el balance entre las clases.

Esto permite identificar si existe **desbalance en los datos**, lo cual puede afectar el rendimiento de los modelos predictivos.

---

# División del Dataset

El conjunto de datos se dividió en:

- **70% datos de entrenamiento**
- **30% datos de prueba**

Se utilizó **estratificación** para mantener la misma proporción de churn en ambos conjuntos.

---

# Modelos Predictivos Utilizados

Se implementaron dos algoritmos de Machine Learning.

## Regresión Logística

Modelo lineal utilizado como modelo base interpretable.

Características:

- Sensible a la escala de los datos
- Requiere estandarización
- Permite analizar la influencia de cada variable mediante sus coeficientes

## Random Forest

Modelo basado en árboles de decisión.

Ventajas:

- Captura relaciones no lineales
- No requiere normalización
- Permite analizar la **importancia de las variables**

---

# Evaluación de los Modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy (Exactitud)
- Precision
- Recall
- F1-score
- Matriz de confusión

Estas métricas permiten analizar tanto el rendimiento general como la capacidad del modelo para identificar correctamente clientes en riesgo de cancelación.

---

# Importancia de Variables

Se analizaron las variables más relevantes para la predicción de churn.

Se utilizaron dos enfoques:

**Regresión Logística**

Interpretación de los coeficientes del modelo.

**Random Forest**

Importancia de variables basada en la reducción de impureza en los árboles.

Este análisis permite identificar los factores que más influyen en la cancelación de clientes.

---

# Principales Factores Asociados al Churn

El análisis sugiere que la cancelación de clientes está relacionada con factores como:

- Tiempo de permanencia del cliente
- Tipo de contrato
- Método de pago
- Cargos mensuales
- Servicios adicionales contratados

Estas variables permiten identificar perfiles de clientes con mayor riesgo de cancelación.

---

# Conclusiones Estratégicas

Los resultados muestran que es posible predecir la cancelación de clientes utilizando modelos de Machine Learning.

Esto permite a Telecom X:

- Detectar clientes con alto riesgo de abandono
- Implementar estrategias de retención anticipadas
- Diseñar campañas de fidelización más efectivas
- Optimizar la toma de decisiones basada en datos

El uso de modelos predictivos puede convertirse en una **herramienta estratégica para reducir la pérdida de clientes y mejorar la competitividad de la empresa**.

---

# Cómo Ejecutar el Proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/tuusuario/telecomx-churn-prediction
### 2. Abrir el notebook en Google Colab o Jupyter Notebook
### 3. Instalar dependencias si es necesario
pip install pandas numpy matplotlib seaborn scikit-learn
### 4. Ejecutar las celdas en orden


Autor

Sindy Campillo
Proyecto desarrollado como parte del programa
Oracle Next Education (ONE) – Alura Latam
