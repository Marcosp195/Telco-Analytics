Megaline Telecommunication Plan Analysis
1. Project Description
This project involves a preliminary analysis of the "Surf" and "Ultimate" prepaid plans from the telecommunications company, Megaline. The primary goal is to determine which of the two plans generates more revenue for the company. This analysis will provide the marketing department with actionable insights to adjust its advertising budget effectively.

The analysis is based on a sample of 500 Megaline customers, studying their consumption patterns for calls, text messages, and internet data throughout 2018.

2. Analysis Methodology
The workflow implemented in the Jupyter notebook (Analisis Telco.ipynb) follows the standard steps of a data analysis project:

a. Data Loading and Preparation
Data Loading: Five distinct datasets were loaded into Pandas DataFrames: calls, internet, messages, plans, and users.

Data Preprocessing and Cleaning:

Each DataFrame was inspected to identify and correct incorrect data types (e.g., converting object to datetime).

Missing values were handled, particularly in the churn_date column, to identify active customers.

The data was enriched by converting megabytes to gigabytes and rounding up minutes and gigabytes according to company rules.

b. Data Aggregation and Revenue Calculation
Usage data (calls, messages, internet) was aggregated per user, per month.

This aggregated data was merged with user plan information to create a consolidated master table.

Overage usage was calculated for each service (minutes, messages, data) that exceeded the limits of the contracted plan.

Finally, the total monthly revenue per user was calculated by adding the base plan cost to any additional overage charges.

c. Exploratory Data Analysis (EDA)
The behavior of users on both plans was studied and compared.

Descriptive statistics (mean, variance, etc.) were calculated for call, message, and data consumption.

Visualizations (histograms, box plots, and bar charts) were generated to compare consumption distribution and revenue between the "Surf" and "Ultimate" plans.

d. Statistical Hypothesis Testing
Two key hypotheses were formulated and tested using a Student's t-test for independent samples:

Hypothesis on Plan Revenue:

Null (H₀): The average revenue from "Ultimate" plan users is equal to the average revenue from "Surf" plan users.

Alternative (H₁): The average revenue from "Ultimate" and "Surf" plan users is different.

Hypothesis on Regional Revenue:

Null (H₀): The average revenue from users in the NY-NJ area is equal to that of users from other regions.

Alternative (H₁): The average revenue from users in the NY-NJ area is different from that of users from other regions.

3. Key Conclusions
The behavioral analysis showed that while Ultimate plan users tend to consume more services, Surf plan users frequently generate significant income from overage charges by exceeding their plan limits.

The hypothesis test results indicate that there is a statistically significant difference in the average revenue between the "Surf" and "Ultimate" plans, with the Ultimate plan generating higher average revenue for the company.

No statistically significant difference was found between the revenue from users in the NY-NJ area and those from other regions.

4. Technologies and Libraries Used
Python 3

Pandas: For data manipulation and analysis.

NumPy: For numerical calculations and data transformation.

Matplotlib: For generating graphs and visualizations.

SciPy (stats): For performing statistical hypothesis tests.

Análisis de Tarifas de Telecomunicaciones para Megaline
1. Descripción del Proyecto
Este proyecto consiste en un análisis preliminar de los planes de prepago "Surf" y "Ultimate" de la compañía de telecomunicaciones Megaline. El objetivo principal es determinar cuál de las dos tarifas genera más ingresos para la empresa, con el fin de que el departamento comercial pueda ajustar el presupuesto de publicidad de manera informada.

El análisis se basa en una muestra de 500 clientes de Megaline, estudiando sus patrones de consumo de llamadas, mensajes de texto y datos de internet durante el año 2018.

2. Metodología del Análisis
El flujo de trabajo implementado en el notebook de Jupyter (Analisis Telco.ipynb) sigue los pasos estándar de un proyecto de análisis de datos:

a. Carga y Preparación de Datos
Carga de Datos: Se cargaron 5 conjuntos de datos distintos en DataFrames de Pandas: calls, internet, messages, plans, y users.

Preprocesamiento y Limpieza:

Se revisó cada DataFrame para identificar y corregir tipos de datos incorrectos (ej. fechas en formato object a datetime).

Se manejaron los valores ausentes, particularmente en la columna churn_date, para identificar a los clientes activos.

Se enriquecieron los datos, por ejemplo, convirtiendo el consumo de megabytes a gigabytes y redondeando hacia arriba los minutos y gigabytes según las reglas de la compañía.

b. Agregación de Datos y Cálculo de Ingresos
Se agregaron los datos de consumo (llamadas, mensajes, internet) por cada usuario para cada mes.

Se unificaron los datos de consumo con la información del plan de cada usuario para crear una tabla consolidada.

Se calcularon los excedentes de consumo para cada servicio (minutos, mensajes, datos) que superaban los límites del plan contratado.

Finalmente, se calculó el ingreso mensual total por cada usuario, sumando el costo base del plan más los cargos adicionales por excedentes.

c. Análisis Exploratorio de Datos (EDA)
Se estudió y comparó el comportamiento de los usuarios de ambos planes.

Se calcularon estadísticas descriptivas (media, varianza, etc.) para el consumo de llamadas, mensajes y datos.

Se generaron visualizaciones (histogramas, diagramas de caja y gráficos de barras) para comparar la distribución del consumo y los ingresos entre los planes "Surf" y "Ultimate".

d. Pruebas de Hipótesis Estadísticas
Se formularon y probaron dos hipótesis clave utilizando la prueba t de Student para muestras independientes:

Hipótesis sobre los ingresos de los planes:

Nula (H₀): El ingreso promedio de los usuarios del plan "Ultimate" es igual al ingreso promedio de los usuarios del plan "Surf".

Alternativa (H₁): El ingreso promedio de los usuarios de los planes "Ultimate" y "Surf" es diferente.

Hipótesis sobre los ingresos por región:

Nula (H₀): El ingreso promedio de los usuarios del área de NY-NJ es igual al de los usuarios de otras regiones.

Alternativa (H₁): El ingreso promedio de los usuarios del área de NY-NJ es diferente al de los usuarios de otras regiones.

3. Conclusiones Principales
El análisis de comportamiento demostró que, aunque los usuarios del plan Ultimate tienden a consumir más servicios, los usuarios del plan Surf generan ingresos significativos por cargos extra al exceder frecuentemente los límites de su plan.

Los resultados de la prueba de hipótesis indican que existe una diferencia estadísticamente significativa en los ingresos promedio entre los planes "Surf" y "Ultimate", siendo el plan Ultimate el que genera mayores ingresos promedio para la compañía.

No se encontró una diferencia estadísticamente significativa entre los ingresos de los usuarios del área de NY-NJ y los de otras regiones.

4. Tecnologías y Librerías Utilizadas
Python 3

Pandas: Para la manipulación y análisis de los datos.

NumPy: Para cálculos numéricos y transformaciones de datos.

Matplotlib: Para la generación de gráficos y visualizaciones.

SciPy (stats): Para la ejecución de las pruebas de hipótesis estadísticas.