Python Pandas Jupyter

Análisis exploratorio y predictivo para la retención de clientes en telecomunicaciones.


 
 Contexto 
    
Instalación
    
 Análisis 
    
 Resultados 
    
 Conclusiones 
 



Churn Banner



El presente proyecto aborda el problema de la fuga de clientes (Churn) en una empresa de telecomunicaciones (Telco). El objetivo principal es transformar datos crudos en conocimiento accionable que permita al equipo de negocio tomar decisiones estratégicas para reducir la pérdida de ingresos.

Se utilizó el enfoque de Minería de Datos propuesto por Gironés Roig et al. (2017), transitando por las fases de Datos, Información, Patrones y Conocimiento.



Para ejecutar este análisis de forma local, asegúrate de tener Python instalado.

Clona el repositorio:
git clone https://github.com/tu-usuario/telco-churn-analysis.git
Instala las dependencias necesarias:
shell

pip install -r requirements.txt
(Principales librerías: Pandas, Numpy, Matplotlib, Seaborn, Scipy)
Ejecuta el notebook principal:
shell

jupyter notebook Laboratorio_1_Telco.ipynb
<div align="right">
<br>
<a href="#"><kbd> <br> 🡅 <br> </kbd></a>
</div>

<a id="analisis"></a>
<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=25&pause=1000&color=CCA9DD&vCenter=true&width=435&height=25&lines=ANÁLISIS" width="450"/>

El análisis se estructuró en dos grandes bloques:

1. Exploración de Datos (EDA)
Se identificó un desbalance en la variable objetivo (26.5% de fugas) y se limpiaron datos inconsistentes en la columna TotalCharges.

2. Pruebas Estadísticas
Para validar hipótesis de negocio, se aplicaron tests de significancia:

Mann-Whitney U: Confirmó que la antigüedad (tenure) y los cargos mensuales difieren significativamente entre clientes que se quedan y los que se van.
Chi-cuadrado + V de Cramér: Reveló que el tipo de contrato (Contract) es la variable categórica con mayor fuerza de asociación al Churn.
<div align="center">
<table><tr><td>

Tenure vs Churn

</td><td>

Contract vs Churn

</td></tr></table>
</div>

<div align="right">
<br>
<a href="#"><kbd> <br> 🡅 <br> </kbd></a>
</div>

<a id="resultados"></a>
<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=25&pause=1000&color=CCA9DD&vCenter=true&width=435&height=25&lines=RESULTADOS" width="450"/>

El perfil de cliente con mayor riesgo de fuga se define por tres características clave:

Característica
Hallazgo
Contrato	Clientes con contrato Month-to-month (mensual).
Antigüedad	Clientes nuevos (tenure bajo).
Precios	Clientes con cargos mensuales altos (MonthlyCharges).

Matriz de Correlación
Se detectó una correlación negativa moderada entre antigüedad y fuga: a mayor tiempo en la empresa, menor probabilidad de cancelación.

<div align="center">
<img src="assets/correlation_matrix.png" alt="Correlation Matrix" width="70%"/>
</div>

<div align="right">
<br>
<a href="#"><kbd> <br> 🡅 <br> </kbd></a>
</div>

<a id="conclusiones"></a>
<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=25&pause=1000&color=CCA9DD&vCenter=true&width=435&height=25&lines=CONCLUSIONES" width="450"/>

Basado en los datos, la recomendación estratégica principal es:

[!IMPORTANT]
Implementar una campaña de retención agresiva enfocada en migrar clientes de contrato mensual a contratos anuales, ofreciendo incentivos durante los primeros meses de vida del cliente.

Esto se justifica en que el compromiso a largo plazo (contratos anuales) reduce drásticamente la tasa de cancelación.

<div align="right">
<br>
<a href="#"><kbd> <br> 🡅 <br> </kbd></a>
</div>

<div align="center">
<br>
<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=25&pause=1000&color=CCA9DD&vCenter=true&width=435&height=25&lines=GRACIAS" width="450"/>
</div>

<div align="right">
<sub>Last edited on: 27/03/2026<span id="last-edited"></span></sub>
</div>
