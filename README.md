# 📊 Telecom\_x2 – Predicción de Cancelación de Clientes (Churn)

Este proyecto aplica modelos de Machine Learning para predecir la cancelación de clientes (churn) en **Telecom X**. Tras un análisis exploratorio exitoso (Parte 1), esta segunda etapa se enfoca en el desarrollo de modelos predictivos que permiten identificar patrones clave asociados a la pérdida de clientes, con el objetivo de mejorar la retención.

---

## 🎯 Objetivo

Predecir si un cliente abandonará la empresa utilizando variables relevantes del servicio, contrato, comportamiento y datos demográficos. Esta predicción permite a Telecom X tomar decisiones estratégicas basadas en datos para reducir la tasa de cancelación.

---

## 🗂️ Estructura del proyecto

```
Telecom_x2/
│
├── data/
│   ├── telecom_churn_clean.csv     # Datos tratados y listos para modelado
│
├── notebooks/
│   └── 02_churn_modeling.ipynb     # Cuaderno principal con análisis y modelos
│
├── visualizations/
│   └── eda_plots/                  # Gráficos generados durante el EDA
│
├── README.md                       # Este archivo
└── requirements.txt                # Bibliotecas necesarias
```

---

## ⚙️ Preparación de los datos

Durante la etapa de preprocesamiento, se realizaron las siguientes tareas:

* **Clasificación de variables**: Se identificaron columnas categóricas y numéricas.
* **Codificación**: Las variables categóricas se codificaron usando One-Hot Encoding.
* **Normalización**: Se aplicó escalado a las variables numéricas donde fue necesario.
* **División de datos**: El conjunto fue dividido en `train` y `test` usando una proporción de 80/20.
* **Manejo de datos faltantes**: Se eliminaron o imputaron valores según el contexto.

---

## 📈 Exploración de Datos (EDA)

Se identificaron patrones importantes, como:

* Mayor tasa de cancelación entre clientes con contratos mensuales.
* Clientes con cargos adicionales tienden a cancelar con más frecuencia.
* Variables como tipo de contrato, servicio técnico y métodos de pago fueron altamente predictivas.

Gráficos generados: histogramas, boxplots, matrices de correlación, gráficos de barras segmentados, entre otros.

---

## 🤖 Modelado

Se probaron y compararon diferentes modelos de clasificación:

* Regresión Logística
* Random Forest
* XGBoost

Cada modelo fue evaluado usando métricas como **accuracy**, **precision**, **recall**, **F1-score** y la **matriz de confusión**.

---

## 🚀 Cómo ejecutar el proyecto

1. Clona el repositorio:

   ```bash
   git clone https://github.com/tu_usuario/Telecom_x2.git
   cd Telecom_x2
   ```

2. Instala las dependencias:

   ```bash
   pip install -r requirements.txt
   ```

3. Abre y ejecuta el cuaderno:

   ```bash
   jupyter notebook notebooks/02_churn_modeling.ipynb
   ```

---

## 📚 Requisitos

Las principales bibliotecas utilizadas son:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `xgboost`

---

## 🧠 Conclusiones

Este proyecto demuestra cómo aplicar técnicas de Machine Learning a problemas de negocio reales. Identificar a los clientes en riesgo de cancelación permite a las empresas tomar acciones preventivas y estratégicas basadas en datos.


