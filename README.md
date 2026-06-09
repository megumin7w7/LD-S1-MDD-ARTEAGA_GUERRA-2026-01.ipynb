<div align="center">

# Laboratorios de Minería de Datos
### TECSUP 2026-I | Curso: Minería de Datos (C64893)

<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=24&pause=1000&color=4A90E2&center=true&vCenter=true&width=700&lines=Minería+de+Datos+—+12+Semanas;Clasificación+%7C+Clustering+%7C+NLP;Python+%7C+scikit-learn+%7C+Keras;Arteaga+Guerra%2C+Pedro+Sebastian" />

<br>

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![sklearn](https://img.shields.io/badge/scikit--learn-1.4-F7931E?style=for-the-badge&logo=scikit-learn)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?style=for-the-badge&logo=tensorflow)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen?style=for-the-badge)

</div>

---

##  Información del Repositorio

| Campo | Detalle |
|---|---|
| **Autor** | Arteaga Guerra, Pedro Sebastian |
| **Docente** | Pilar Rocío Sayán Mejía |
| **Institución** | TECSUP — Pasión por la Tecnología |
| **Curso** | Minería de Datos — C64893 |
| **Semestre** | 2026-I |
| **Cobertura** | Semanas 1 a 12 (3 Unidades) |

---

## Descripción General

Este repositorio contiene el desarrollo completo de los **12 Laboratorios del curso de Minería de Datos**, organizados en tres unidades temáticas que cubren desde los fundamentos del análisis exploratorio hasta modelos avanzados de clasificación, aprendizaje no supervisado y métodos probabilísticos de NLP.

Cada laboratorio incluye:
- ✅ Código Python ejecutado en **Google Colab / Jupyter Notebook**
- ✅ Análisis Exploratorio de Datos (EDA) con visualizaciones
- ✅ Implementación y evaluación de modelos de Machine Learning
- ✅ Respuestas a preguntas de reflexión y casos de negocio
- ✅ Conclusiones técnicas y de aprendizaje

---

## 🗂️ Estructura del Repositorio

```
📁 Mineria-de-Datos-TECSUP-2026/
│
├── 📓 LAB_S01_Intro_MineriaDatos.ipynb
├── 📓 LAB_S02_CRISP_DM_SEMMA.ipynb
├── 📓 LAB_S03_Almacenes_Datos_EDA.ipynb
├── 📓 LAB_S04_Preparacion_Datos.ipynb
├── 📓 LAB_S05_Taxonomia_Modelos_Metricas.ipynb     ← TelcoPerú Churn
├── 📓 LAB_S06_kNN_RegresionLogistica.ipynb          ← Heart Disease (UCI)
├── 📓 LAB_S07_SVM.ipynb                             ← Breast Cancer
├── 📓 LAB_S08_Arboles_RandomForest.ipynb            ← IBM HR Attrition
├── 📓 LAB_S09_XGBoost_Boosting.ipynb                ← TelcoPerú Churn
├── 📓 LAB_S10_Redes_Neuronales.ipynb                ← Credit Card Fraud
├── 📓 LAB_S11_Clustering_NoSupervisado.ipynb        ← Credit Card Fraud
└── 📓 LAB_S12_NaiveBayes_NLP.ipynb                 ← SMS Spam Collection
```

---

## Contenido por Unidad y Semana

### UNIDAD 1 — Fundamentos y Preparación de Datos (Semanas 1–5)

| Semana | Tema | Dataset | Técnicas Clave |
|:---:|---|---|---|
| 1 | Introducción a la Minería de Datos | Telco Customer Churn | KDD, CRISP-DM, exploración inicial |
| 2 | Metodologías: CRISP-DM y SEMMA | Problema real | Etapas CRISP-DM aplicadas |
| 3 | Almacenes de Datos y EDA | Dataset propio | OLAP, análisis exploratorio, entropía |
| 4 | Preparación de Datos | Pipeline Python | Limpieza, normalización, one-hot encoding |
| **5** | **Taxonomía de Modelos y Evaluación** | **Telco Customer Churn** | **Matriz de confusión, ROC-AUC, Gini, k-fold, umbral de decisión** |

**Laboratorio 5 — Caso TelcoPerú S.A.:** Análisis de costos FN/FP (S/ 325 vs S/ 25), comparación de DummyClassifier, curvas ROC, impacto del umbral de clasificación y restricción operacional de 300 clientes/mes.

---

### UNIDAD 2 — Modelos de Clasificación (Semanas 6–8)

| Semana | Tema | Dataset | Técnicas Clave |
|:---:|---|---|---|
| **6** | **k-NN y Regresión Logística** | **Heart Disease (UCI)** | **GridSearch para k óptimo, Odds Ratio, estandarización** |
| **7** | **SVM** | **Breast Cancer (UCI)** | **Kernels lineal/RBF, SMOTE, GridSearchCV, One-Hot Encoding** |
| **8** | **Árboles de Decisión y Random Forest** | **IBM HR Analytics Attrition** | **Gini, poda, importancia de variables, class_weight** |

**Laboratorio 6 — Heart Disease:** Comparación k-NN vs Regresión Logística para diagnóstico cardíaco. Análisis de Odds Ratio por variable clínica. Justificación de `scaler.transform()` vs `fit_transform()` en datos de test.

**Laboratorio 7 — Breast Cancer:** SVM con diferentes kernels (lineal, polinomial, RBF). Efecto del SMOTE en clase minoritaria. Comparación de estrategias de selección de variables.

**Laboratorio 8 — IBM HR Attrition:** Árbol de Decisión para predicción de renuncias. Análisis de profundidad óptima (overfitting). Variables más importantes: OverTime, MonthlyIncome, Age.

---

### UNIDAD 3 — Modelos Avanzados y No Supervisados (Semanas 9–12)

| Semana | Tema | Dataset | Técnicas Clave |
|:---:|---|---|---|
| **9** | **Gradient Boosting y XGBoost** | **Telco Customer Churn** | **scale_pos_weight, GridSearchCV, SHAP, umbral óptimo** |
| **10** | **Redes Neuronales Artificiales** | **Credit Card Fraud Detection** | **Keras/TF, Dropout, Early Stopping, SMOTE post-split** |
| **11** | **Clustering No Supervisado** | **Credit Card Fraud Detection** | **K-Means, jerárquico, Fuzzy C-Means, PCA, silueta** |
| **12** | **Naïve Bayes y NLP** | **SMS Spam Collection** | **BoW, TF-IDF, Multinomial NB, Bernoulli NB, Precision-Recall** |

**Laboratorio 9 — XGBoost TelcoPerú:** Optimización de hiperparámetros para churn prediction. Análisis ROI por umbral. Variables más importantes del modelo. Caso empresarial: 2.5M clientes, S/ 45M en pérdidas por abandono.

**Laboratorio 10 — Redes Neuronales:** Arquitectura RNA para detección de fraude (284,807 transacciones, 0.17% fraude). Análisis costo-beneficio de umbral 0.3 vs 0.5. Backpropagation, Adam, Early Stopping.

**Laboratorio 11 — Clustering:** Segmentación de transacciones financieras en clusters de comportamiento. Método del codo, silhouette score, dendrogramas, MiniBatch K-Means, Fuzzy C-Means, Canopy.

**Laboratorio 12 — Naïve Bayes/NLP:** Filtro de spam con BoW y TF-IDF. Comparación Gaussiano vs Multinomial vs Bernoulli NB. Pipeline de producción para filtrado de SMS en tiempo real.

---

## Hallazgos Clave del Curso

1. **Métricas vs Negocio:** El Accuracy es engañoso con datos desbalanceados. Recall, F1-Score y AUC-ROC son las métricas relevantes cuando el costo de los errores es asimétrico (FN >> FP en churn, fraude y diagnóstico médico).

2. **El umbral importa:** El umbral por defecto (0.5) raramente es óptimo en producción. Para TelcoPerú (FN = S/ 325 vs FP = S/ 25) el umbral óptimo es ~0.35–0.40; para detección de fraude, ~0.30.

3. **Preprocesamiento es el 80% del trabajo:** SMOTE después del split, `scaler.fit()` solo en train, `stratify=y` en splits desbalanceados, y `class_weight='balanced'` son buenas prácticas no negociables.

4. **Interpretabilidad vs Rendimiento:** Regresión Logística y Árboles de Decisión son preferibles cuando se debe explicar al negocio (hospitales, RRHH); XGBoost y RNA son preferibles cuando el rendimiento es prioritario.

5. **Clustering exploratorio:** El silhouette score bajo (~0.1) en datos de fraude es esperable — los clusters son perfiles de comportamiento, no grupos perfectamente separados.

---

## Tecnologías Utilizadas

| Categoría | Herramientas |
|---|---|
| **Lenguaje** | Python 3.12 |
| **Entorno** | Jupyter Notebook / Google Colab |
| **Manipulación de datos** | Pandas, NumPy |
| **ML Clásico** | scikit-learn (kNN, SVM, Árboles, Random Forest, Naïve Bayes) |
| **Boosting** | XGBoost, LightGBM |
| **Redes Neuronales** | TensorFlow / Keras |
| **Balanceo de clases** | imbalanced-learn (SMOTE) |
| **Visualización** | Matplotlib, Seaborn |
| **NLP** | scikit-learn (TF-IDF, CountVectorizer) |

---

##  Cómo ejecutar los notebooks

```bash
# 1. Clonar el repositorio
git clone https://github.com/[tu-usuario]/Mineria-de-Datos-TECSUP-2026.git
cd Mineria-de-Datos-TECSUP-2026

# 2. Instalar dependencias
pip install pandas numpy matplotlib seaborn scikit-learn xgboost \
            tensorflow keras imbalanced-learn scipy

# 3. Ejecutar cualquier notebook
jupyter notebook LAB_S09_XGBoost_Boosting.ipynb
```

> **Recomendación:** Cada notebook fue diseñado para Google Colab. Para ejecutarlos localmente, verifica que los paths de los datasets apunten a tu directorio local.

---

## 📖 Referencias Bibliográficas

- Gironés Roig, J. et al. (2017). *Minería de datos: modelos y algoritmos*. Editorial UOC.
- James, G. et al. (2023). *An Introduction to Statistical Learning* (2.ª ed.). Springer.
- Géron, A. (2023). *Hands-On Machine Learning* (3.ª ed.). O'Reilly Media.
- Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press.
- Burkov, A. (2019). *The Hundred-Page Machine Learning Book*. Andriy Burkov.
- Chen, T., & Guestrin, C. (2016). XGBoost. *KDD '16*, 785–794.
- Pedregosa, F. et al. (2011). Scikit-learn: Machine Learning in Python. *JMLR*, 12, 2825–2830.

---

<div align="center">

**TECSUP 2026-I | Minería de Datos | Arteaga Guerra, Pedro Sebastian**

</div>
