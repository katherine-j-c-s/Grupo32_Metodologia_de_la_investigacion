# Evolución del precio del boleto y la demanda de viajes en el Subte de Buenos Aires (2014–2019)

## 📌 Segunda entrega del proyecto

Este repositorio contiene los avances correspondientes a la **segunda entrega del Trabajo Final Integrador** de la **Licenciatura en Ciencia de Datos de la Universidad del Gran Rosario (UGR)**.

El proyecto propone analizar la evolución del precio del boleto y la demanda de viajes en el sistema de Subterráneos de la Ciudad Autónoma de Buenos Aires durante el período **2014–2019**, explorando la relación entre las modificaciones tarifarias y las variaciones observadas en la demanda.

> **Estado del proyecto:** Segunda entrega — fundamentación teórica y definición metodológica.

---

## 🎯 Objetivo del proyecto

El objetivo general del proyecto es:

> **Analizar la evolución del precio del boleto y la demanda de viajes en el Subte de Buenos Aires entre 2014 y 2019, identificando patrones de variación en el sistema y diferencias entre líneas.**

El análisis busca estudiar la evolución temporal de ambas variables, considerando además el contexto inflacionario del período y las posibles diferencias en el comportamiento de la demanda entre líneas y estaciones.

---

## 📊 Fuentes de datos

El proyecto utiliza **8 fuentes de datos** correspondientes al período de estudio:

| Archivo                                        | Descripción                                                                        |
| ---------------------------------------------- | ---------------------------------------------------------------------------------- |
| `registro-historico-del-precio-del-boleto.csv` | Evolución mensual del precio del boleto entre 2014 y abril de 2019.                |
| `viajes_anual.csv`                             | Demanda anual total por línea entre 2014 y 2019.                                   |
| `historico_2014.csv`                           | Detalle de demanda por molinete, estación y franja horaria correspondiente a 2014. |
| `historico_2015.csv`                           | Detalle de demanda correspondiente a 2015.                                         |
| `historico_2016.csv`                           | Detalle de demanda correspondiente a 2016.                                         |
| `historico_2017.csv`                           | Detalle de demanda correspondiente a 2017.                                         |
| `historico_2018.csv`                           | Detalle de demanda correspondiente a 2018.                                         |
| `historico_2019.csv`                           | Detalle de demanda correspondiente a 2019.                                         |

Las fuentes se integrarán y procesarán para construir una estructura homogénea que permita realizar análisis temporales, comparaciones entre líneas y estaciones y estudiar la relación entre las variaciones tarifarias y la demanda.

---

## 🔎 Problemática

El precio del boleto del Subte presentó modificaciones durante el período 2014–2019, en un contexto caracterizado además por variaciones en el nivel general de precios de la economía argentina.

Por este motivo, una comparación directa de los valores nominales de la tarifa puede resultar insuficiente para interpretar su evolución. A su vez, las variaciones en la cantidad de viajes registrados pueden no presentar una relación uniforme con los cambios tarifarios.

El proyecto busca analizar esta problemática mediante datos históricos, considerando:

* Evolución mensual del precio del boleto.
* Evolución de la demanda de viajes.
* Variaciones interanuales.
* Diferencias entre líneas.
* Diferencias entre estaciones, cuando los datos lo permitan.
* Contexto inflacionario.
* Posible relación entre tarifa y demanda.
* Elasticidad-precio de la demanda, si los datos permiten realizar una estimación consistente.

El análisis será de carácter descriptivo y exploratorio. Las asociaciones identificadas no serán interpretadas automáticamente como relaciones causales.

---

## 🧪 Metodología

El proyecto seguirá un enfoque **cuantitativo, no experimental, longitudinal y retrospectivo**.

Las principales etapas previstas son:

1. **Relevamiento de las fuentes**

   * Identificación de variables.
   * Revisión de formatos.
   * Análisis de períodos y niveles de agregación.

2. **Integración de datos**

   * Unificación de los históricos 2014–2019.
   * Homogeneización de fechas, líneas y estaciones.
   * Integración con la información tarifaria.

3. **Limpieza y preparación**

   * Detección de valores faltantes.
   * Identificación de duplicados.
   * Revisión de inconsistencias.
   * Análisis de valores atípicos.
   * Documentación de los criterios de tratamiento.

4. **Análisis exploratorio**

   * Distribución de las variables.
   * Evolución temporal.
   * Comparaciones entre años.
   * Comparaciones entre líneas y estaciones.

5. **Análisis tarifario**

   * Evolución nominal del precio.
   * Variaciones porcentuales.
   * Consideración del contexto inflacionario.
   * Análisis en términos reales cuando la disponibilidad de datos lo permita.

6. **Análisis de la relación tarifa-demanda**

   * Comparación de variaciones de precio y demanda.
   * Análisis por período.
   * Análisis por línea y estación cuando corresponda.
   * Estimación de elasticidad-precio si los datos permiten realizarla de forma consistente.

7. **Visualización**

   * Construcción de gráficos e indicadores.
   * Desarrollo de un tablero interactivo en Power BI.

---

## 🛠️ Herramientas previstas

* **Python** para procesamiento y análisis de datos.
* **Pandas** para manipulación de datos.
* **NumPy** para operaciones numéricas.
* **Matplotlib** para visualización.
* **Power BI** para el desarrollo del tablero interactivo.
* **Git/GitHub** para el control y almacenamiento del proyecto.

Las herramientas y técnicas podrán ajustarse en función de las características y calidad de los datos durante las etapas de desarrollo.

---

## 📈 Resultados esperados

El proyecto busca obtener una caracterización de:

* La evolución del precio del boleto durante 2014–2019.
* La evolución de la demanda total y por línea.
* Las variaciones de la demanda ante cambios tarifarios.
* Las diferencias de comportamiento entre líneas y estaciones.
* La evolución de la tarifa considerando el contexto inflacionario.
* La posible relación entre precio y demanda.
* Indicadores que faciliten la interpretación de los datos.

Como resultado final se prevé desarrollar un **tablero interactivo en Power BI** que permita explorar las principales variables e indicadores del estudio.

---

## 📁 Estructura prevista del repositorio

```text
subte-precio-demanda-2014-2019/
│
├── data/
│   ├── registro-historico-del-precio-del-boleto.csv
│   ├── viajes_anual.csv
│   ├── historico_2014.csv
│   ├── historico_2015.csv
│   ├── historico_2016.csv
│   ├── historico_2017.csv
│   ├── historico_2018.csv
│   └── historico_2019.csv
│
├── notebooks/
│   └── ...
│
├── src/
│   └── ...
│
├── dashboard/
│   └── ...
│
├── docs/
│   └── ...
│
└── README.md
```

> La estructura podrá modificarse a medida que avance el desarrollo del proyecto.

---

## 👥 Integrantes

* **Katherine Contreras**
* **Maibach Mateo**
* **Joaquin Betes**
* **Emilce Robles**
* **Silvina Andrea Moyano**

### Universidad

**Universidad del Gran Rosario (UGR)**
**Licenciatura en Ciencia de Datos**

---

## 📚 Estado actual

Esta versión corresponde a la **segunda entrega del proyecto**. En esta etapa se presentan principalmente:

* La problemática y su contexto.
* Los objetivos.
* La hipótesis.
* El marco teórico inicial.
* Las fuentes de datos previstas.
* La metodología propuesta.
* Las herramientas y etapas de análisis.

Los resultados definitivos, visualizaciones finales, análisis estadísticos y tablero interactivo serán desarrollados en las etapas posteriores del proyecto.
