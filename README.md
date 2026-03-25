<div align="center">

# 📊 Data Mining Project – Customer Behavior Analysis

### 🔍 Análisis de comportamiento de usuarios y conversión de compras

</div>

---

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo analizar grandes volúmenes de datos de comportamiento de usuarios en un eCommerce para obtener insights clave sobre:

- 🛒 Conversión de usuarios (view → purchase)
- 🏷️ Marcas con mayor rendimiento
- ⏰ Horarios de mayor actividad
- 📉 Patrones de abandono (churn)

Se trabaja bajo la metodología **CRISP-DM**, aplicando técnicas de análisis exploratorio de datos (EDA) y procesamiento eficiente de datasets masivos.

---

## 🧠 Objetivos

- ✔️ Unificar múltiples datasets grandes (.gz)
- ✔️ Optimizar procesamiento de datos (uso de `Polars`)
- ✔️ Analizar tasas de conversión por marca
- ✔️ Identificar patrones de comportamiento por hora
- ✔️ Preparar base para modelos predictivos futuros

---

## 📂 Dataset

Dataset principal:

- 📦 **eCommerce Behavior Data (Kaggle)**
- 📅 Periodo: Oct 2019 – Apr 2020
- 📊 Más de **7 millones+ de registros**

### Estructura:

```text
event_time     → fecha y hora del evento
event_type     → tipo (view, cart, purchase)
product_id     → ID del producto
category_id    → categoría
category_code  → subcategoría
brand          → marca
price          → precio
user_id        → usuario
user_session   → sesión
