# 📡 Telecom X - Predicción de Cancelación de Clientes

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)

## 🎯 Resumen del Proyecto
Este proyecto desarrolla un pipeline de **Machine Learning** para predecir qué clientes de la empresa "Telecom X" tienen mayor probabilidad de cancelar sus servicios. El objetivo es permitir que la empresa tome acciones proactivas de retención basadas en datos.

## 🧠 Misión Estratégica
Como Analista de Machine Learning, la misión fue transformar datos históricos en un modelo predictivo capaz de capturar la mayor cantidad de fugas posibles, priorizando la detección temprana sobre la exactitud general.

## 🛠️ Fases del Pipeline de Datos

1.  **Limpieza y Curaduría:** Eliminación de identificadores irrelevantes e imputación de valores nulos en la variable objetivo.
2.  **Ingeniería de Características:** * **One-Hot Encoding:** Transformación de variables categóricas.
    * **Estandarización:** Uso de `StandardScaler` para equilibrar escalas numéricas.
3.  **Balanceo de Clases:** Implementación de **SMOTE** para corregir el desbalanceo (73% vs 27%), logrando un set de entrenamiento equitativo.
4.  **Modelado:** Evaluación comparativa entre **Regresión Logística** y **Random Forest**.

## 📊 Resultados y Evaluación

| Métrica | Regresión Logística | Random Forest |
| :--- | :---: | :---: |
| **Accuracy** | 74.5% | 78.2% |
| **Recall (Sensibilidad)** | **80.0%** | 53.4% |
| **F1-Score** | 62.5% | 56.6% |

**Modelo Seleccionado:** **Regresión Logística**. 
*Justificación:* En un problema de Churn, es vital minimizar los falsos negativos. Con un **Recall del 80%**, este modelo identifica a la gran mayoría de clientes en riesgo.

## 💡 Insights y Estrategia de Negocio

A través del análisis de importancia de variables, se determinó:
* **Contrato Mensual:** Es el mayor predictor de fuga. Estrategia: Ofrecer incentivos para migración a contratos anuales.
* **Meses de Permanencia:** Los clientes nuevos son los más vulnerables. Estrategia: Programa de "Onboarding" y beneficios en los primeros 6 meses.
* **Fibra Óptica:** Presenta una tasa de abandono inusualmente alta. Estrategia: Auditoría de calidad técnica en este servicio.

## 🚀 Cómo ejecutar
1. Clona el repositorio.
2. Sube el archivo `telecom_x_cleaned.csv` a tu entorno.
3. Ejecuta el notebook en Google Colab para replicar los resultados.

---
## ✒️ Autor
* **Fernando Contreras Albarrán,** - [GitHub](https://github.com/Fernando99ing)
---
*Proyecto desarrollado como parte del Desafío Telecom X - 2026*
