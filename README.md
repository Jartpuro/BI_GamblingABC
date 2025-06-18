# 🎲 BI_GamblingABC

Repositorio oficial del proyecto de analítica descriptiva y predictiva para el comportamiento de usuarios en plataformas de apuestas. Se construye un modelo visual y explicativo en **Power BI** utilizando métricas clave como conversión, retorno y rentabilidad.

## 📈 Visor en Línea

Accede al informe interactivo publicado en Power BI:
👉 [Ver informe en Power BI](https://app.powerbi.com/view?r=eyJrIjoiY2UxNDZlMzItZjgzMS00NGNkLTk1NDYtZWNhYTEzOGMwYjFmIiwidCI6ImJiYTAwZDQzLWQwYWItNGRkZi04YzkwLWExNjZlYzgzM2VmMCIsImMiOjR9)

---

## 📊 Objetivo del Proyecto

Explorar, limpiar y visualizar datos históricos de actividad de usuarios en una casa de apuestas en línea con el fin de:

- Analizar patrones de comportamiento.
- Evaluar rentabilidad y retorno por usuario.
- Medir la efectividad del funnel de conversión (Clicks → Registros → Depósitos → Apuestas).
- Proyectar métricas clave a futuro (Net Revenue, Total Apostado).

---

## 🧮 Métricas Principales

- **Tasa de Conversión**  
  `= DIVIDE(SUM([Primer Deposito]), SUM([Registros]))`

- **Ingreso Promedio por Usuario (ARPU)**  
  `= DIVIDE(SUM([Net Revenue]), SUM([Personas Apostaron]))`

- **Tasa de Retorno**  
  `= DIVIDE(SUM([Net Revenue]), SUM([Total Apostado]))`

---

## 📁 Contenido del Repositorio

----> 📂 data/ → Datos originales en crudo utilizados para análisis y modelado
----> 📂 images/ → Recursos visuales y capturas del dashboard Power BI
----> 📂 notebooks/ → Scripts de procesamiento en Jupyter: limpieza, modelado y conexión a MySQL

## 📓 Proceso Documentado (`/notebooks`)

El cuaderno de trabajo en Jupyter describe paso a paso:

1. **Lectura de datos**:
   - Extracción desde archivos `.xlsx` con estructuras no convencionales (datos embebidos en columnas únicas tipo CSV).
   
2. **Exploración y limpieza (EDA)**:
   - Conversión de fechas, casting de tipos, manejo de valores nulos, y formateo monetario.

3. **Tratamiento avanzado**:
   - Cálculo de métricas clave como `Tasa de Conversión`, `Ingreso Promedio por Usuario` y `Net Revenue`.
   - Imputación de valores faltantes mediante interpolación y regresión multivariada.

4. **Carga a Base de Datos (MySQL)**:
   - Generación de una base de datos relacional con `SQLAlchemy` y `pymysql`.
   - Reemplazo completo de registros mediante `to_sql`.

5. **Modelado predictivo (Proyección 720 días)**:
   - Uso de técnicas como Holt-Winters, SARIMAX y XGBoost.


----> 📂 outputs/ → Archivos procesados, exportaciones limpias y datasets listos para análisis
📄 Inzale_JART.pbix → Archivo de Power BI con el informe visual completo
