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

