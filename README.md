# Proyecto Final: Análisis Integral del Ciclo de Vida del Cliente (CLV)

Este proyecto constituye el trabajo final del **Máster en Data & Analytics**. Consiste en el diseño, desarrollo y documentación de un flujo de **Análisis Exploratorio de Datos (EDA)** con el objetivo de realizar una analítica completa del ciclo de vida del cliente: desde la ingesta, unificación y limpieza de fuentes heterogéneas, hasta el desarrollo de un EDA profundo y la creación de un Dashboard operativo.

El análisis se centra en comprender el comportamiento de los clientes, optimizar la segmentación de valor y detectar factores críticos que influyen en la tasa de abandono (Churn), proporcionando recomendaciones estratégicas basadas en evidencia.

---

## Estructura del Proyecto
El repositorio está organizado para facilitar la inspección del código y la ejecución del entorno:

proyecto_final/

├── DataProject_ Proyecto EDA con Python.docx   #Documento original con las directrices y enunciados

├── README.md                                  #Descripción general del proyecto y documentación

├── analisis_exploratorio.ipynb                #Jupyter Notebook principal con el pipeline de código ejecutado y limpio

├── bank-additional.csv                        #Dataset original con los resultados de los contactos

└── customer-details.xlsx                      #Dataset original con la información socioeconómica de los clientes

---

## Acceso a los Datasets Originales
Debido al volumen y peso de los archivos de datos originales, estos han sido alojados en una unidad externa para optimizar la gestión del repositorio. Puedes descargarlos desde el siguiente enlace:

**[Descargar Datasets Originales (Google Drive)](https://drive.google.com/file/d/1OPITOw7VChkiga9UyGzuzuwP5mLC4ov2/view?usp=drive_link)**

---

## Herramientas y Tecnologías Utilizadas
- **Python 3.x** → Lenguaje de programación principal para el procesamiento de datos.
- **Jupyter Notebook / VS Code** → Entorno interactivo utilizado para el desarrollo, pruebas y documentación en vivo de las celdas de código.
- **Librerías del Ecosistema de Datos:**
    - `pandas` para la carga distribuidora de ficheros, indexación, unificación relacional (`merge`) y manipulación de DataFrames.
    - `numpy` para el soporte de operaciones matriciales y gestión de estructuras de datos nulos.
    - `matplotlib.pyplot` para la inicialización de lienzos dinámicos y optimización de gráficos.
    - `seaborn` para la construcción de gráficos estadísticos de alta densidad informativa.
- **Excel:** Diseño de Dashboard operativo para visualización ejecutiva.

---

## Proceso Metodológico de Desarrollo
1. **Ingeniería de Datos:** Unión de fuentes heterogéneas mediante `pd.merge()` sobre la clave `ID_Cliente` para consolidar un dataset único de trabajo.
2. **Limpieza Robusta:** Conversión de tipos de datos (datetime, numeric), imputación de nulos y estandarización de variables monetarias para garantizar la calidad del análisis.
3. **Análisis Exploratorio (EDA):** Evaluación profunda de distribuciones, identificación de *outliers* y análisis de correlación entre variables financieras y de comportamiento del cliente.
4. **Storytelling de Negocio:** Transformación de insights técnicos en recomendaciones estratégicas para la mejora de la retención y la conversión comercial.

***

**Nota sobre el proyecto:** Dado que este es un proceso de aprendizaje orientado a consolidar la ingeniería de datos y el análisis exploratorio con Python, se utilizó apoyo de una IA para depurar conflictos de entorno de ejecución, optimizar la sintaxis de los bucles de limpieza y estructurar de forma clara el flujo lógico del cuaderno. Esto garantizó la entrega de código limpio, idiomático (*Pythonic*) y eficiente.

***

## Resultados y Hallazgos Principales
Tras procesar más de **600,000 registros**, los hallazgos clave fueron:

- **Segmentación de Alto Valor:** El segmento "Premium" es el motor principal de ingresos (125,584 unidades), superando a otros segmentos.
- **Dominio del Canal Móvil:** El 60% de las ventas se concentran en dispositivos móviles, validando la necesidad de priorizar la optimización de UX en este canal.
- **Correlación NPS-Churn:** Se detectó una disparidad significativa en la satisfacción (NPS) entre los clientes que permanecen (-26.72%) y los que abandonan (-0.56%), sirviendo como señal de alerta temprana para retención proactiva.

## Recomendaciones Estratégicas
- **Focalización VIP:** Implementar estrategias de *upselling* dirigidas al segmento "Premium" para maximizar su lealtad.
- **Optimización UX Móvil:** Priorizar recursos técnicos en la experiencia móvil, dado que es el canal predominante de adquisición.
- **Alerta de Churn:** Institucionalizar un protocolo de reactivación automática para clientes cuyo NPS caiga por debajo de umbrales críticos.

---

## Habilidades Demostradas
- **Ingeniería de Datos Práctica:** Capacidad para enlazar archivos relacionales independientes garantizando la integridad del volumen de registros.
- **Estadística Descriptiva Aplicada:** Uso eficiente de métodos analíticos para sintetizar poblaciones de datos complejas en métricas de negocio.
- **Robustez de Entorno:** Resolución de conflictos de dependencias del Kernel mediante el despliegue directo del operador de instalación `%pip`.

---

## Acceso al Código
**Consulta el cuaderno completo con todas las celdas de limpieza y gráficos ejecutadas:**
[Abrir analisis_exploratorio.ipynb](./analisis_exploratorio.ipynb)

---

## Autor
**[Orlan Javier Parra Parra]**

[@orlanjavier6](https://github.com/orlanjavier6)

Máster en Data & Analytics
