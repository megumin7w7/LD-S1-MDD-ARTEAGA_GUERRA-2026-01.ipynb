<div align="center">

# 📊 Data Mining Project – Customer Behavior Analysis

<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=28&pause=1000&color=4A90E2&center=true&vCenter=true&width=600&lines=Big+Data+Analysis;Ecommerce+Insights;Conversion+%26+Churn+Analysis" />

<br>

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![Polars](https://img.shields.io/badge/Polars-Fast%20DataFrame-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Progress-green?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Big%20Data-red?style=for-the-badge)

</div>

---

<div align="center">

## 🚀 Quick Navigation

<a href="#-descripcion"><kbd> Descripción </kbd></a>
<a href="#-dataset"><kbd> Dataset </kbd></a>
<a href="#-analisis"><kbd> Análisis </kbd></a>
<a href="#-tecnologias"><kbd> Tecnologías </kbd></a>
<a href="#-ejecucion"><kbd> Ejecución </kbd></a>

</div>

---

## 📌 Descripción

Este proyecto analiza **millones de registros de comportamiento de usuarios en eCommerce** para identificar:

- 🛒 Conversión de usuarios (**view → purchase**)  
- 🏷️ Marcas con mayor rendimiento  
- ⏰ Horarios de mayor actividad  
- 📉 Patrones de abandono  

---

## 🧠 Enfoque del Proyecto

<div align="center">

Carga de datos (.gz)
↓
Procesamiento eficiente (Polars)
↓
Filtrado y limpieza
↓
Transformación (fechas → horas)
↓
Análisis de conversión
↓
Insights de negocio


</div>

---

## 📂 Dataset

<div align="center">

<img src="https://cdn-icons-png.flaticon.com/512/2921/2921222.png" width="120"/>

</div>

- 📦 Dataset: eCommerce Behavior  
- 📊 +7 millones de registros  
- 📅 Oct 2019 – Apr 2020  

### Columnas principales:

```text
event_time     → fecha del evento
event_type     → view / cart / purchase
product_id     → producto
brand          → marca
price          → precio
user_id        → usuario
