# rappi-ecommerce-analysis
# 🛒 Análisis de Negocio y Conversión: RappiPlus

## 📌 Resumen del Proyecto
Este proyecto evalúa el desempeño del servicio **RappiPlus** mediante el análisis integral del ciclo de vida del usuario para apoyar decisiones de negocio basadas en datos. A través de la extracción de datos con SQL, limpieza y análisis en Python, y visualización en Tableau, se analizaron embudos de conversión, rentabilidad, retención por cohortes y los resultados de un experimento A/B en el flujo de pago (checkout).

## 🛠️ Herramientas y Tecnologías
* **Análisis de Datos:** Python (Pandas, SciPy)
* **Bases de Datos:** PostgreSQL (Extracción de eventos de usuario)
* **Visualización de Datos:** Tableau
* **Técnicas Aplicadas:** Análisis de Funnel, Retención por Cohortes, A/B Testing, Análisis de Rentabilidad (Revenue, COGS, Profit).

## 📊 Dashboards Interactivos
Los resultados clave y el análisis exploratorio están visualizados de forma interactiva en Tableau Public:
* 🔗 [Dashboard 1: Overview Ejecutivo (Rentabilidad y Marketing)](https://public.tableau.com/app/profile/jorge.moreno6260/viz/overview-rappi/overview?publish=yes)
* 🔗 [Dashboard 2: Detalle y Drill-down de Ventas](https://public.tableau.com/app/profile/jorge.moreno6260/viz/detalle-rappi/detalle?publish=yes)

## 💡 Hallazgos Clave y Recomendaciones Estratégicas
1. **Embudos de Conversión (Funnel):** El análisis en SQL reveló que la mayor caída de usuarios ocurre en la transición entre iniciar el checkout (`begin_checkout`) y agregar la información de pago (`add_payment_info`). 
2. **A/B Testing en el Checkout:** Se evaluó estadísticamente (Prueba Chi-cuadrado, $\alpha = 0.05$) el rediseño de la interfaz de pago. No se encontró evidencia estadísticamente sólida de que la nueva interfaz mejore la conversión.
3. **Recomendación Comercial:** Se recomienda **frenar el rollout** de la nueva interfaz de checkout para evitar costos de despliegue innecesarios, e iterar un nuevo diseño enfocado exclusivamente en reducir la fricción en el formulario de métodos de pago.

## 📂 Estructura del Repositorio
* `rappiplus_analisis_negocio.ipynb`: Código principal en Jupyter Notebook con el análisis completo (limpieza, SQL, cálculos de cohortes y test estadístico).
* `datasets/`: Carpeta con los archivos limpios generados (`orders_clean.csv`, `catalog_clean.csv`, `marketing_clean.csv`) utilizados para los tableros en Tableau.
* `README.md`: Resumen y conclusiones del proyecto.

## ✉️ Contacto
Para más detalles sobre este proyecto o explorar colaboraciones, puedes conectar conmigo en https://www.linkedin.com/in/jorge-alejandro-moreno-gomez/?isSelfProfile=true  o explorar otros de mis proyectos analíticos en este perfil de GitHub.
