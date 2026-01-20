# SPRINT 15: AUDITORÍA DE EXPERIMENTACIÓN AVANZADA (TEST A/B)

<div align="center">
  <a href="./proyecto15.ipynb">
    <img src="https://img.shields.io/badge/▶_Ver_Notebook_Completo-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Ver Notebook">
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp; <a href="../../README.md">
    <img src="https://img.shields.io/badge/🏠_Volver_al_Menú_Principal-2ea44f?style=for-the-badge&logo=github&logoColor=white" alt="Volver al Home">
  </a>
</div>

### 🛡️ Escenario (Situation)
Se lanzó una prueba A/B para evaluar un nuevo sistema de recomendaciones. Sin embargo, los datos mostraban inconsistencias temporales y de asignación de usuarios.

### 🎯 Objetivo (Task)
Auditar la integridad técnica del experimento antes de interpretar los resultados de negocio.

### 🔧 Implementación Técnica (Action)
* **Auditoría de Muestra:** Verificación de balance 50/50 y superposición de usuarios entre pruebas concurrentes.
* **Funnel Analysis:** Evaluación de conversión en `product_page` vs `purchase`.
* **Z-Test:** Prueba de proporciones para validar significancia.

### 🚀 Resultados (Result)
**AUDITORÍA NEGATIVA.** Se declaró la prueba como INVÁLIDA debido a fallos en el diseño experimental (fechas coincidentes con promociones navideñas y desbalance de muestra). Se evitó una toma de decisión errónea.

---
**Stack:** `Python` `Experimental Design Audit` `Statistical Inference`