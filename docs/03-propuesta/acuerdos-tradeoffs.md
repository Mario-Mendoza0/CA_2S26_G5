---
sidebar_position: 1
---

# Acuerdos y Trade-offs

# Acuerdos Alcanzados y Justificación de Trade-offs

Durante la simulación de la Junta Directiva, el equipo evaluó los conflictos de arquitectura, presupuesto y operatividad entre los distintos módulos, alcanzando los siguientes 3 acuerdos clave:

---

### Acuerdo 1: Conectividad y Arquitectura de Datos (Local-First vs. Cloud Sync)
- *Conflicto:* El área de analítica requería sincronización continua en la nube, mientras que la operación de caja necesitaba garantizar la toma de pedidos en horas pico aun con fallas de internet.
- *Acuerdo Alcanzado:* Se implementará una arquitectura híbrida Local-First. El sistema POS funcionará en una base de datos local instalada en el negocio y se sincronizará automáticamente con la nube en segundo plano al detectar conexión o al cierre de turno.
- *Justificación del Trade-off:*
  - Ganancia: Disponibilidad del 100% en el punto de venta sin riesgo de caídas del sistema por problemas de conectividad.
  - Concesión: Los reportes del Dashboard no se verán en tiempo real segundo a segundo desde dispositivos externos, sino con un pequeño desfase o al cierre de caja.

---

### Acuerdo 2: Nivel de Rigidez en Recetas y Tolerancia de Mermas
- *Conflicto:* El módulo de recetas buscaba un descuento estricto gramo por gramo al seleccionar modificadores (ej. "sin cebolla" o "extra salsa"), mientras que el área de cocina requería flexibilidad por variaciones en el porcionado manual y agilidad operativa.
- *Acuerdo Alcanzado:* El sistema aplicará el descuento automático según la receta base, pero incorporará un margen de tolerancia (+/- 5%) y un módulo simplificado para registro de mermas directas en menos de 2 clics.
- *Justificación del Trade-off:*
  - Ganancia: Fluidez y rapidez en la preparación de platillos sin saturar al personal de cocina con registros complejos.
  - Concesión: Una ligera pérdida de precisión absoluta en el inventario de insumos a cambio de adaptabilidad al ritmo real de trabajo.

---

### Acuerdo 3: Canal de Notificaciones de Stock y Costos Operativos
- *Conflicto:* Se evaluó el envío de alertas automáticas vía SMS/WhatsApp para reabastecimiento crítico, pero esto introducía costos recurrentes por uso de APIs (Twilio/WhatsApp Business) afectando el retorno de inversión (ROI).
- *Acuerdo Alcanzado:* Se desestimaron las notificaciones de pago por terceros y se sustituyeron por alertas visuales de alta prioridad (pop-ups y códigos de color) dentro del panel POS/Dashboard, junto con un resumen diario enviado por correo electrónico.
- *Justificación del Trade-off:*
  - Ganancia: Mantenimiento del costo operativo mensual del software en $0 para el comerciante, maximizando el ROI.
  - Concesión: Dependencia de que el encargado o administrador revise las pantallas o su correo para gestionar los pedidos a proveedores.