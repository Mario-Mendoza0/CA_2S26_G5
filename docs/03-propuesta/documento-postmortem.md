---
sidebar_position: 2
---

# Documento Postmortem

# Documento Postmortem: Proyecto 2 - Sistema POS Unificado

---

## 1. Resumen Ejecutivo
El presente documento analiza el desempeño del equipo durante el diseño, negociación y documentación del Sistema POS Unificado para Restaurantes. Se evalúan los aciertos, los obstáculos superados y las lecciones aprendidas durante el ciclo de vida del proyecto.

---

## 2. ¿Qué Salió Bien? (Aciertos y Fortalezas)

* **Definición Clara de la Arquitectura:** La adopción del enfoque *Local-First* garantizó la disponibilidad del sistema en el punto de venta sin comprometer la integridad operativa ante fallas de red.
* **Debate Asertivo en la Junta Directiva:** La negociación entre los 6 módulos se realizó de manera estructurada, logrando justificar cada *trade-off* sin afectar el Retorno de Inversión (ROI).
* **Uso Eficiente de Herramientas Colaborativas:** El seguimiento de tareas mediante Trello y la integración continua en GitHub permitieron mantener una estructura limpia y alineada a los requerimientos del curso.
* **Inclusión de Analítica Operativa:** La incorporación de métricas visuales (como el análisis de Horas Pico) aportó un valor real para la toma de decisiones estratégicas del negocio.

---

## 3. Principales Retos y Obstáculos (¿Qué Famosos "Cuellos de Botella" Encontramos?)

1. **Sincronización de Tiempos para la Grabación:** Coordinar los horarios de los 6 integrantes para grabar la sesión extendida de la Junta Directiva (45-50 minutos) representó una dificultad logística importante.
2. **Estandarización del Formato:** En las primeras etapas hubo discrepancias en el nombrado de archivos y carpetas, lo que requirió una reestructuración intermedia para cumplir al 100% con la guía.
3. **Equilibrio entre Rigidez de Recetas y Agilidad en Cocina:** Encontrar un punto medio entre el control estricto de inventario y la fluidez del personal en momentos de alto tráfico fue el debate técnico más complejo.

---

## 4. Soluciones Implementadas y Mitigación

* **Negociación de Tolerancia (+/- 5%):** Se acordó un margen de flexibilización en el descuento de insumos e integración de un botón directo de mermas en cocina, resolviendo el conflicto operativo.
* **Reorganización Temprana del Repositorio:** Se estandarizó la nomenclatura de las 4 carpetas principales (`01-recoleccion-informacion`, `02-analisis`, `03-propuesta`, `04-tabla-participacion`) antes de realizar los *commits* finales.

---

## 5. Lecciones Aprendidas (Para Futuros Proyectos)

* **Documentación Progresiva:** Crear y actualizar la estructura del repositorio desde el primer día evita acumulaciones de trabajo de edición a última hora.
* **Priorización de Trade-offs Fijos:** Tener definidos los puntos no negociables (ej. costo $0 de mensajería) agiliza las discusiones en mesas redondas y juntas directivas.
* **Valor del Material Visual:** Desarrollar mockups y gráficas de datos antes de las exposiciones fortalece la defensa técnica de cada módulo ante el cliente o evaluador.