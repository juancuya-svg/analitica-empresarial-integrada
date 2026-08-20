# 📊 Analítica Empresarial Integrada

Repositorio académico desarrollado como parte del curso de **Analítica Empresarial Integrada** en **TECSUP**, utilizando como caso de estudio a **AgroAndes Export S.A.C.**, una empresa agroexportadora peruana.

## 👤 Autor

**JUAN DIEGO ALEJANDRO CUYA VERA**  
Carrera: **Big Data y Ciencia de Datos — TECSUP**  
GitHub: **@juancuya-svg**

## 🎯 Objetivo del laboratorio

El laboratorio busca comprender cómo los datos pueden convertirse en un activo estratégico para una organización y cómo la analítica contribuye a la toma de decisiones empresariales.

A lo largo del notebook se trabaja con información de embarques, fundos, productos y clientes de AgroAndes para:

- explorar y auditar la calidad de los datos;
- detectar inconsistencias y duplicados;
- normalizar categorías;
- realizar análisis descriptivo y diagnóstico;
- consultar datos mediante SQL con DuckDB;
- integrar información macroeconómica del BCRP;
- comparar el rendimiento de Pandas y Polars;
- introducir el diagnóstico de madurez analítica mediante el modelo DELTA.

## 🧰 Tecnologías utilizadas

- **Python**
- **Pandas**
- **Polars**
- **DuckDB**
- **Plotly**
- **NumPy**
- **econdata / BCRP**
- **Jupyter Notebook / Google Colab**
- **Git & GitHub**

## 📁 Datos analizados

El caso contiene cuatro fuentes principales:

| Fuente | Registros / elementos |
|---|---:|
| Embarques | 15,705 |
| Fundos | 6 |
| Productos | 20 |
| Clientes | 72 |

El período disponible comprende desde **03/01/2022 hasta 29/06/2026**.

## 🔎 Resultados observados

Durante la exploración se identificaron varios aspectos relevantes del conjunto de datos:

- El FOB acumulado registrado alcanza aproximadamente **US$ 261.8 millones**.
- Inicialmente aparecen **17 nombres de mercados**, debido a inconsistencias como `USA`, `EE.UU.`, `ESTADOS UNIDOS` o variantes de `Países Bajos`.
- Después de normalizar las categorías, se identifican **8 mercados reales**.
- Al eliminar duplicados exactos, el conjunto de análisis pasa de **15,705 a 15,585 registros**.
- **Estados Unidos** aparece como el principal mercado del caso, con aproximadamente **US$ 125.88 millones FOB**.
- En 2024 se registran aproximadamente **US$ 69.3 millones FOB**, frente a US$ 52.9 millones en 2023 y US$ 55.8 millones en 2025.
- Se integró el tipo de cambio publicado por el **Banco Central de Reserva del Perú (BCRP)** para analizar la facturación tanto en dólares como en soles.
- En una ejecución del benchmark con **1,570,500 filas**, Polars realizó la agregación aproximadamente **1.20× más rápido** que Pandas en esa máquina y operación específica.

> Los tiempos de rendimiento pueden variar según el equipo, el tamaño de los datos y la operación ejecutada.

## 🧠 Enfoque analítico

El notebook introduce la **escalera analítica**:

1. **Descriptiva:** ¿qué pasó?
2. **Diagnóstica:** ¿por qué pasó?
3. **Predictiva:** ¿qué podría pasar?
4. **Prescriptiva:** ¿qué decisión conviene tomar?

Además, se utiliza el modelo **DELTA de Davenport** para evaluar cinco dimensiones de madurez analítica:

- **D — Data**
- **E — Enterprise**
- **L — Leadership**
- **T — Targets**
- **A — Analysts**

## 📓 Notebook principal

El desarrollo completo del laboratorio se encuentra en:

`LAB_D1_AEI_JUAN_DIEGO_CUYA_VERA_PROFESIONAL.ipynb`

El notebook contiene el código, las explicaciones del laboratorio, análisis de los datos, consultas, visualizaciones y actividades de interpretación empresarial.

## ▶️ Ejecución

La forma recomendada de ejecutar el proyecto es mediante **Google Colab** o **Jupyter Notebook**.

1. Abrir el archivo `.ipynb`.
2. Ejecutar las celdas en orden.
3. Permitir la instalación de las dependencias indicadas en el notebook.
4. Para las consultas en vivo al BCRP se requiere conexión a Internet.

Los datos del caso se encuentran incorporados dentro del propio notebook y se extraen automáticamente durante la ejecución.

## 📌 Propósito académico

Este repositorio forma parte de mi formación en **Big Data y Ciencia de Datos**, y busca documentar de manera reproducible el proceso de convertir datos empresariales en información útil para la toma de decisiones.

---

**TECSUP — Big Data y Ciencia de Datos**  
**Autor:** JUAN DIEGO ALEJANDRO CUYA VERA
