---
sidebar_position: 6
---

# Justificación

# Justificación de la Selección y Unificación de Información de Campo

## 1. Contexto y Antecedentes del Trabajo de Campo
Durante la fase de investigación de campo, el equipo llevó a cabo entrevistas estructuradas a dos comercios locales del sector de alimentos y bebidas:
* *TacoUsac:* Taquería / Establecimiento de comida rápida.
* *Kiosco Calin:* Puesto de panes / comida al paso.

El objetivo de estas entrevistas fue identificar las dinámicas operativas diarias, los flujos de trabajo en el punto de venta, la gestión de insumos y los principales cuellos de botella que afectan la eficiencia del servicio y la rentabilidad del negocio.

---

## 2. Decisión sobre la Integración de Información
Tras analizar los datos recolectados, las transcripciones y las evidencias de audio y fotografía de ambas visitas, el equipo tomó la decisión estratégica de *unificar la información y los requerimientos de ambos comercios* en un único modelo de solución integral, en lugar de trabajar con un negocio de forma aislada.

---

## 3. Justificación Técnica y Operativa de la Unificación

### A. Similitud en los Puntos de Dolor Operativos (Problemática Común)
A pesar de operar en formatos ligeramente distintos, ambos establecimientos mostraron vulnerabilidades y limitaciones operativas idénticas:
* *Ineficiencia en la toma de pedidos y cobro:* Registro manual de órdenes que genera demoras considerables durante las horas pico de atención.
* *Falta de control en el inventario y mermas:* Ausencia de un registro sistematizado de los ingredientes consumidos por platillo, provocando descuadres en stock e imposibilidad de rastrear desperdicios.
* *Riesgo de agotamiento de insumos (Stockout):* Dependencia de revisiones visuales empíricas para el reabastecimiento, lo que provoca desabasto inesperado de insumos clave en momentos de alta demanda.
* *Vulnerabilidad en la seguridad operativa:* Falta de perfiles de usuario diferenciados para autorizar anulaciones, descuentos o cierres de caja.

### B. Diseño de una Solución Escusable y Reutilizable
Construir un sistema enfocado exclusivamente en uno de los locales habría limitado el alcance de la solución a un caso muy particular. La unificación permite abstraer un *modelo de dominio general para pequeños y medianos comercios de alimentos*, garantizando que la arquitectura del software sea modular, parametrizable y fácilmente adaptable a diferentes tipos de menú o flujos de venta.

### C. Coherencia con la Metodología del Proyecto y la Junta Directiva
El desarrollo del proyecto exige la simulación de una *Junta Directiva Técnica* donde se evalúan decisiones de diseño, concesiones de arquitectura (trade-offs) y negociaciones entre diferentes funcionalidades. Unificar la información de ambos negocios proporciona un ecosistema de requerimientos lo suficientemente rico y complejo para que cada integrante asuma la defensa de un módulo específico (POS táctil, control de mermas, recetas, alertas de inventario, analítica de ventas y seguridad con ROI).