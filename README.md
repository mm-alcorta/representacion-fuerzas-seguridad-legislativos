# representacion-fuerzas-seguridad-legislativos

# La representación de las fuerzas públicas de seguridad en el poder legislativo subnacional: análisis comparativo entre Brasil (2022) y Argentina (2023)

Este repositorio contiene las bases de datos, metodologías, fuentes y resultados del análisis estadístico desarrollado en la tesis de la Maestría en Derechos Humanos y Democratización para América Latina y el Caribe (CIEP - Universidad Nacional de San Martín / Global Campus of Human Rights).

* **Autora:** Mg. Mercedes Milagros Alcorta
* **Año:** 2025

---

## Diseño de la Investigación

### Pregunta de Investigación

¿Qué variables explican la presencia de representantes provenientes de las fuerzas públicas de seguridad en los órganos legislativos estaduales de Brasil y provinciales de Argentina?

### Objetivo General

Analizar la relación entre desigualdad social, violencia y la presencia de legisladores provenientes de las fuerzas públicas de seguridad en Brasil (elecciones estaduales de 2022) y Argentina (elecciones provinciales de 2023).

### Metodología

Análisis cuantitativo mediante el **Coeficiente de Correlación de Spearman**

---

## Operacionalización de Variables

### Variable Dependiente

**Legisladores provenientes de las fuerzas públicas de seguridad.**

**Brasil (Indicadores):**

* Policía Civil
* Policía Militar
* Fuerzas Armadas en retiro
* Fuerzas Armadas en servicio activo

**Argentina (Indicadores):**

* Policía Provincial
* Fuerzas Armadas

### Variables Independientes

**Desigualdad social**

* Brasil: Índice de Gini per cápita de los hogares (2021).
* Argentina: Coeficiente de Gini del ingreso per cápita familiar (2022).

**Violencia**

* Ambos países: Tasa de homicidios cada 100.000 habitantes.
* Brasil: 2021.
* Argentina: 2022.

---

## Código Utilizado

El análisis estadístico fue desarrollado en Python utilizando las siguientes bibliotecas:

* `pandas` (estructuración y manipulación de datos).
* `scipy.stats` (estimación del coeficiente de correlación por rangos de Spearman).
* `openpyxl` (exportación y formateo de archivos Excel).

El script automatiza el proceso de análisis mediante la carga de las bases de datos, el cálculo de correlaciones de Spearman entre las variables dependientes e independientes, la clasificación de la intensidad de las asociaciones y su significancia estadística, así como la generación de una matriz final de resultados en formato Excel.

---

## Principales Hallazgos

Los resultados obtenidos validan parcialmente la hipótesis inicial.

* **Fuerzas policiales:** No se observaron correlaciones estadísticamente significativas entre la desigualdad social o la violencia y la presencia de representantes policiales en ninguno de los dos países. Las correlaciones cercanas a cero o negativas sugieren que, en contextos de alta desigualdad y violencia estructural, las fuerzas policiales no son percibidas unívocamente por la ciudadanía como agentes de solución. Por el contrario, pueden ser asociadas a dinámicas de violencia institucional y criminalización de sectores socialmente vulnerables, limitando así su potencial capital electoral.

* **Fuerzas Armadas en Argentina:** A diferencia del resto de las instituciones analizadas, las Fuerzas Armadas argentinas mostraron una tendencia positiva moderada respecto de la desigualdad social y la violencia. Si bien estos resultados no alcanzan la significancia estadística convencional (p < 0.05), la cercanía a los márgenes evidencia una tendencia diferenciada que merece atención analítica. Desde una perspectiva teórica, este hallazgo sugiere que, en determinados contextos de crisis social y deterioro de las condiciones de seguridad, las Fuerzas Armadas pueden adquirir una imagen pública asociada al orden y la estabilidad institucional.

* **Apertura a nuevas líneas de investigación:** Los resultados indican que la representación política de los actores de seguridad depende de variables adicionales que exceden las variables macroestructurales consideradas en este estudio.

---

## Reproducción del Análisis

1. Descargar la base de datos incluida en el repositorio.
2. Ejecutar el archivo `analisis_spearman`.
3. El script procesará automáticamente la información y generará el archivo `resultados_spearman.xlsx` con los coeficientes de correlación obtenidos.

---

## Estructura del Repositorio

### Archivos principales

* `Spearman - Tesis de maestría.py`: script fuente en Python encargado del procesamiento y análisis estadístico.
* `Resultados_Spearman.xlsx`: matriz analítica exportada con los coeficientes obtenidos.
* `Base de datos Brasil (2022)-Argentina (2023).xlsx`: base de datos consolidada utilizada para el estudio.

### Hojas de trabajo de la base de datos

* `Argentina`: variables estructurales provinciales.
* `Brasil`: variables estructurales estaduales.
* `Legisladores electos Argentina`: registro y clasificación de legisladores provinciales.
* `Legisladores electos Brasil 2022`: nómina oficial y clasificación de diputados estaduales brasileños.

---

## Fuentes de Información

### Brasil

* Tribunal Supremo Electoral (TSE).
* Instituto Brasileño de Geografía y Estadística (IBGE).
* Instituto Igarapé.

### Argentina

* Instituto Nacional de Estadística y Censos (INDEC).
* Ministerio de Seguridad de la Nación.
* **Relevamiento propio:** elaborado a partir de legislaturas provinciales, portales periodísticos y sitios oficiales de los candidatos electos.

---

## Licencia

Este repositorio se publica con fines académicos y de investigación. Se permite su consulta, utilización y citación siempre que se reconozca adecuadamente la autoría y la fuente original del trabajo.
