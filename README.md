# Práctica IA (RA4 · a) — Automatización y optimización

## 1) Proceso elegido
- Nombre del proceso: Clasificación de tickets
- Contexto (empresa/servicio web/IT): Los clientes envian las incidencias a través de la página web o por correo
- Rol/es implicados: cliente, agente, gerente y administrador

## 2) ANTES (sin IA)
- Pasos (5–7):
  1. El cliente tiene una incidencia.
  2. El cliente manda el ticket al soporte.
  3. El gerente lee el problema y manda a un agente a solucionarlo.
  4. El agente resuelve el problema.
  5. El administrador, gerente o agente cierra el ticket y lo da por solucionado.
- Tiempo aproximado por caso: 10 - 20 minutos
- Problemas / cuellos de botella: Que el cliente no se haya explicado bien y no se lleve al sitio lo necesario para resolver.
  Que el agente no sepa hacerlo y tenga que ir algún cargo superior con mayores conocimientos.

## 3) DESPUÉS (con IA)
- ¿Qué automatiza la IA?
  Clasificación y priorización automática de los tickets según su contenido.
  Respuestas iniciales automáticas para confirmar la recepción o sugerir soluciones rápidas.
- ¿Qué queda para humanos?
  Intervención en casos complejos que la IA no pueda resolver.
  Supervisión y validación de decisiones en situaciones críticas
- Datos necesarios (tipos de datos, sin datos personales):
  Texto de los tickets (descripción de problemas, categorías).
  Historial de incidencias y feedback de clientes.
- Modelo/técnica (NLP, clasificación, recomendación, visión, etc.):
  NLP para clasificación y análisis de texto.
  Clasificación supervisada para asignar los tickets a categorías y priorizar.

## 4) Optimización (mejora medible)
Define 3 métricas con valores antes/después:
- Tiempo: La IA puede reducir el tiempo de análisis y clasificación de tickets, permitiendo a los agentes centrarse solo en la resolución de problemas. Se estima que el tiempo de procesamiento se reduce a 5–7 minutos por ticket.
- Coste: La automatización mediante IA reduce la necesidad de intervención humana en la clasificación, asignación y seguimiento de los tickets. El coste laboral se reduce debido a la menor intervención manual, lo que disminuye el coste por ticket procesado.
- Calidad: La IA puede garantizar una clasificación más precisa y rápida, reduciendo el margen de error. Además, los tiempos de respuesta se optimizan, lo que mejora la experiencia del cliente. La calidad del servicio aumenta debido a la mayor rapidez en la asignación y resolución de problemas.

## 5) Diagrama del flujo (ASCII o Mermaid)
(Pega aquí el diagrama)
graph TD
    A[Cliente envía ticket] --> B{¿Ticket claro?}
    B -- Sí --> C[IA clasifica y prioriza ticket]
    B -- No --> D[IA solicita más detalles al cliente]
    D --> C
    C --> E[Asignación automática de agente]
    E --> F{¿Es el problema complejo?}
    F -- Sí --> G[Agente resuelve el problema]
    F -- No --> H[IA resuelve o responde automáticamente]
    G --> I[Administrador/gerente cierra el ticket]
    H --> I
    I --> J[Cliente recibe resolución y ticket cerrado]

## 6) Riesgos y mitigación
- Riesgo 1:
  Clasificación incorrecta de tickets por la IA
- Mitigación 1:
  Realizar una supervisión humana periódica para validar que la IA clasifique correctamente los tickets. Además, se pueden entrenar los modelos de IA continuamente con datos actualizados 
  y feedback de los agentes para mejorar la precisión.
- Riesgo 2:
  Dependencia de la IA en casos complejos
- Mitigación 2:
  Asegurar que los tickets más complejos sean redirigidos automáticamente a un agente humano. Implementar un sistema de alertas para agentes que avise cuando la IA detecta una posible 
  incidencia fuera de su capacidad de resolución.

## 7) Fuente oficial
- Enlace:
- #1 los roles: https://blog.invgate.com/es/roles-del-help-desk 
