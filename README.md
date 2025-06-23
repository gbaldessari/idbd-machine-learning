# Proyecto de Predicción de Abandono de Clientes (Churn Prediction)

Este proyecto implementa modelos de machine learning para predecir el abandono de clientes (churn) utilizando dos enfoques:

1. **PySpark**: Para procesamiento distribuido de grandes volúmenes de datos
2. **Scikit-learn**: Para un enfoque tradicional con Random Forest

## 📋 Requisitos Previos

- Python 3.12.6+
- Java 22 (requerido para PySpark)
- pip (gestor de paquetes de Python)

## 🛠 Configuraciones Iniciales

### 1. Configurar entorno

Para instalar y configurar correctamente PySpark se debe seguir el siguiente tutorial:
[How to install PySpark](https://medium.com/@marcelopedronidasilva/how-to-install-and-run-pyspark-locally-integrated-with-vscode-via-jupyter-notebook-on-windows-ff209ac8621f)

### 2. Instalar dependencias principales

```bash
pip install -r requirements.txt
```

En caso de que existan problemas, instala las dependencias manualmente:

```bash
pip install pyspark pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
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

## 🤝 Autores

- Giacomo Baldessari
- Eduardo Miranda
- David Rodríguez
