# Proyecto de Predicción de Abandono de Clientes (Churn Prediction)

Este proyecto implementa modelos de machine learning para predecir el abandono de clientes (churn) utilizando dos enfoques:

1. **PySpark**: Para procesamiento distribuido de grandes volúmenes de datos
2. **Scikit-learn**: Para un enfoque tradicional con Random Forest

## 📋 Requisitos Previos

- Python 3.12.6+
- Java 22 (requerido para PySpark)
- pip (gestor de paquetes de Python)

## 🛠 Instalación de Dependencias

### 1. Configurar entorno virtual (recomendado)

```bash
python -m venv venv
# Linux/Mac
source venv/bin/activate
# Windows
venv\Scripts\activate
```

### 2. Instalar dependencias principales

```bash
pip install -r requirements.txt
```

Si no tienes un archivo `requirements.txt`, instala las dependencias manualmente:

```bash
pip install pyspark pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

### 3. Instalar PySpark (si no se instaló con pip)

```bash
pip install pyspark
```

## 📂 Estructura del Proyecto

```sh
/idbd-machine-learning/
│
├── data/                   # Datos del proyecto
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/              # Jupyter Notebooks
│   └── churn_pyspark.ipynb # Análisis con PySpark
│   └── churn_sklearn.ipynb # Análisis con Scikit-learn
│
├── requirements.txt        # Dependencias del proyecto
└── README.md               # Este archivo
```

## 📊 Dataset

El dataset utilizado es el "Telco Customer Churn" disponible en Kaggle:

- Contiene 7,043 registros y 21 columnas
- Variables demográficas, servicios contratados y facturación

[Kaggle: Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)

## 📌 Notas Adicionales

Para ejecutar PySpark en local, puedes necesitar configurar:

```bash
export PYSPARK_PYTHON=python3
export PYSPARK_DRIVER_PYTHON=python3
```

La primera ejecución puede tardar mientras descarga las dependencias de Spark.

Para desarrollo en Windows, asegúrate de tener Java instalado y en el PATH.

## 🤝 Autores

- Giacomo Baldessari
- Eduardo Miranda
- David Rodríguez

## 📄 Licencia

Este proyecto está bajo la licencia MIT.
