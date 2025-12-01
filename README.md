# Megaline-
📞 Megaline — Análisis de Clientes y Rentabilidad por Plan Tarifario

Evaluación del comportamiento de usuarios y comparación de ingresos entre tarifas Surf y Ultimate.

🧠 Descripción general del proyecto

Este proyecto analiza el comportamiento de 500 clientes del operador de telecomunicaciones Megaline para determinar cuál de sus dos planes de prepago —Surf o Ultimate— genera mayores ingresos.

El análisis incluye limpieza profunda del dataset, consolidación mensual por usuario, cálculo de ingresos reales considerando límites y excedentes, visualización de distribuciones y pruebas de hipótesis para fundamentar la decisión comercial.

🛠️ Tecnologías utilizadas

Python

pandas (transformación y consolidación de datos)

numpy (estadística descriptiva)

matplotlib / seaborn (visualizaciones)

scipy.stats (pruebas de hipótesis)

Jupyter Notebook

📌 Metodología del proyecto
1️⃣ Preparación y limpieza del dataset

Importación de 5 tablas independientes: usuarios, llamadas, SMS, internet y planes.

Conversión de fechas, tipos numéricos y normalización de columnas.

Eliminación de duplicados, revisión de valores inconsistentes y tratamiento de ausentes.

Corrección de duración de llamadas (redondeo a minutos) y datos móviles (transformación MB→GB según política).

2️⃣ Construcción de métricas mensuales por usuario

Para cada cliente se calcularon:

Minutos utilizados por mes

Número de SMS enviados

Volumen de datos consumidos

Ingresos reales del usuario, considerando:

Cuota mensual del plan

Excedentes facturados por minuto, SMS o GB extra

Se generó un dataset consolidado con ingresos mensuales por tarifa.

3️⃣ Análisis exploratorio (EDA)

Histogramas y distribuciones de minutos, SMS y datos para ambos planes.

Media, varianza y desviación estándar por tipo de consumo.

Comparación visual entre Surf y Ultimate para entender perfiles de uso.

Identificación de patrones y diferencias en comportamiento mensual.

4️⃣ Pruebas de hipótesis

Se evaluaron dos afirmaciones clave:

🔹 Hipótesis 1:

"El ingreso promedio de los usuarios del plan Surf y Ultimate es igual."
Se aplicó t-test o Mann-Whitney U según normalidad y varianza.

🔹 Hipótesis 2:

"Los ingresos promedio de clientes en NY/NJ son diferentes al resto de regiones."
Incluyó:

Formulación de H₀ y H₁

Selección del nivel de significancia α

Interpretación estadística del p-value y toma de decisión

📈 Resultados principales

Las distribuciones de consumo muestran diferencias claras entre Surf y Ultimate.

La tarifa Ultimate suele generar ingresos más estables y elevados.

Los usuarios de Surf presentan mayor variabilidad asociada a excedentes.

En las pruebas estadísticas, se identificaron diferencias significativas entre planes.

🧪 Conclusión

Este proyecto demuestra competencias sólidas en:
✔ Limpieza avanzada de datos
✔ Integración y consolidación de múltiples fuentes
✔ Análisis de comportamiento del cliente
✔ Visualización de métricas de consumo
✔ Pruebas estadísticas para decisiones comerciales
✔ Documentación clara y reproducible
