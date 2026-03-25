<div align="center">

#  Proyecto de Minería de Datos – Laboratorio 1

<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=28&pause=1000&color=4A90E2&center=true&vCenter=true&width=650&lines=Minería+de+Datos;Análisis+Exploratorio;Telco+Customer+Churn;Python+y+Jupyter" />

<br>

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Data Mining](https://img.shields.io/badge/Curso-Minería%20de%20Datos-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completado-green?style=for-the-badge)

</div>

---

<div align="center">

## 🚀 Navegación Rápida

<a href="#-descripción"><kbd> Descripción </kbd></a>
<a href="#-dataset"><kbd> Dataset </kbd></a>
<a href="#-hallazgos-clave"><kbd> Hallazgos Clave </kbd></a>
<a href="#-tecnologías"><kbd> Tecnologías </kbd></a>
<a href="#-ejecución"><kbd> Ejecución </kbd></a>

</div>

---

## 📌 Descripción

Este repositorio contiene el desarrollo del **Laboratorio 1 de Minería de Datos** (Autor: Arteaga Guerra Pedro), correspondiente a la Semana 1 del curso impartido por la docente Pilar Rocio Sayan Mejia (TECSUP 2026-I). 

El proyecto se centra en la aplicación de técnicas de **Análisis Exploratorio de Datos (EDA)** y preprocesamiento utilizando Python sobre datos del sector de telecomunicaciones. Además, incluye la aplicación de pruebas estadísticas (Mann-Whitney U, Chi-cuadrado y V de Cramér) para validar hipótesis sobre el comportamiento de los usuarios.

**Objetivos principales del notebook:**
* Realizar la carga, limpieza inicial y análisis estructural del conjunto de datos.
* Identificar y tratar valores nulos (ej. en la variable `TotalCharges`).
* Analizar la distribución de la variable objetivo (`Churn`) y entender el impacto del desbalance de clases.
* Generar visualizaciones clave (histogramas, boxplots, matrices de correlación) para entender el comportamiento de los clientes.
* Extraer conclusiones de negocio accionables para estrategias de retención.

---

## 📂 Dataset

<div align="center">
<img src="https://cdn-icons-png.flaticon.com/512/2921/2921222.png" width="120"/>
</div>

* **Fuente de datos:** `Telco Customer Churn` (Extraído de IBM / Kaggle)
* **Formato del archivo:** `.csv`
* **Volumen:** 7,043 registros y 21 columnas analizadas.
* **Variable Objetivo:** `Churn` (Indica si el cliente canceló o no su servicio; 73.5% No / 26.5% Sí).

**Variables principales analizadas:**
* `tenure` → Meses de antigüedad del cliente en la empresa (Variable numérica, promedio: 32 meses).
* `MonthlyCharges` → Monto cobrado mensualmente al cliente (Variable numérica).
* `TotalCharges` → Gasto total acumulado por el cliente (Variable numérica).
* `Contract` → Tipo de contrato del cliente (Variable categórica: Month-to-month, One year, Two year). Es la variable con mayor fuerza de asociación con el abandono.

---

## 💡 Hallazgos Clave y Conclusiones de Negocio

A través del análisis estadístico y visual, se identificó el perfil de riesgo de los clientes más propensos a abandonar la empresa:

1. **El impacto del contrato:** Los clientes con contratos mensuales (Month-to-month) tienen una tasa de cancelación significativamente mayor frente a los contratos anuales.
2. **Retención inicial crítica:** Los clientes más nuevos tienden a darse de baja del servicio rápidamente. Existe un problema claro de retención en los primeros meses, indicando que a menor tiempo (`tenure`), mayor probabilidad de abandono.
3. **Sensibilidad al precio:** Los clientes que cancelan tienden a concentrar pagos mensuales más altos, lo que sugiere una fuga hacia la competencia buscando mejores ofertas.
4. **Validación Estadística:** Se demostró mediante pruebas estadísticas (V de Cramér) que variables como el género (`gender`) tienen una asociación casi nula con la decisión de abandonar el servicio, mientras que el tipo de contrato (`Contract`) es un factor determinante.

---

## ⚙️ Tecnologías y Librerías

El análisis fue desarrollado en **Jupyter Notebook** (`.ipynb`) y exportado a formato `.html` para su visualización. Las principales herramientas utilizadas son:

* **Pandas:** Para manipulación, limpieza y estructuración del DataFrame.
* **NumPy:** Para cálculos numéricos.
* **Matplotlib & Seaborn:** Para la creación de gráficos exploratorios (Barras, Histogramas, Boxplots, Heatmaps).
* **SciPy (`scipy.stats`):** Para la ejecución de pruebas de hipótesis (Mann-Whitney U, Chi-cuadrado y cálculo de V de Cramér).

---

## 🚀 Ejecución

Para reproducir este análisis en un entorno local:

1. Clona este repositorio o descarga los archivos.
2. Asegúrate de tener instalado Python 3.x y Jupyter Notebook.
3. Instala las dependencias necesarias ejecutando: 
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
