#  Análisis de Variación Presupuestaria y Control de Gastos Operativos

##  Descripción del Proyecto
Este proyecto analiza las desviaciones entre los gastos reales ejecutados y el presupuesto proyectado. A través de un modelo de datos relacional y un dashboard interactivo desarrollado en Power BI, la herramienta permite identificar sobreejecuciones y oportunidades de eficiencia operativa en tiempo real.

---

## Herramientas e Integración
* **Microsoft Excel:** Limpieza de datos, estructuración del conjunto de pruebas y tablas financieras.
* **Power BI:** Modelado relacional, métricas financieras en DAX y diseño de informe interactivo.
* **Diseño Visual (SVG):** Uso de lienzo personalizado para mejorar la experiencia de usuario (UX/UI) y organizar KPIs clave.

---

## Indicadores Clave y Métricas DAX
* **Gasto Real:** `Gasto Real = SUM(Fact_Gastos[Monto])`
* **Variación Absoluta ($):** `Variación = [Gasto Real] - SUM(Fact_Presupuesto[MontoProyectado])`
* **Variación Porcentual (%):** `Variación % = DIVIDE([Variación], SUM(Fact_Presupuesto[MontoProyectado]), 0)`

---

##  Hallazgos y Decisiones
1. **Detección de Desviaciones:** Identificación de categorías operativas con sobrecostos superiores al **10%** respecto a la proyección inicial.
2. **Alertas Visuales:** Implementación de reglas de formato condicional para alertar a los administradores de presupuesto antes del cierre mensual.

---

## 📂 Contenido del Repositorio
* `Dashboard Gastos & Presupuestos.pbix` - Informe interactivo de Power BI.
* `Gastos & Presupuestos.xlsx` - Modelo de datos financiero en Excel.
