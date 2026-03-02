# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA

## 1) Caso y objetivo de negocio
- Empresa/sector (real o ficticia): RetailTech S.A., una empresa de comercio electrónico que vende productos electrónicos.
- Problema a resolver: Alta tasa de abandono de carrito en el sitio web.
- Objetivo de negocio (rentabilidad): Reduciendo la tasa de abandono de carrito, mejorando la conversión de usuarios en clientes.

## 2) Big Data: recogida masiva de datos
Describe por qué es Big Data (volumen, velocidad, variedad).
- Fuente 1: Registros de clics y eventos de los usuarios en el sitio web (acción de navegación, interacciones con productos, abandono de   carrito).
- Fuente 2: Datos de compras previas (historias de compra, frecuencia, valor promedio de pedido).
- Fuente 3: Datos de redes sociales y comentarios de productos.
- Volumen/velocidad (estimación): Más de 1 millón de interacciones diarias (usuarios y transacciones), con datos en tiempo real que se 
  actualizan cada segundo.
- Formatos (texto, eventos, series temporales, imágenes, etc.): Texto (comentarios, reseñas de productos), eventos (clics, 
  interacciones), series temporales (ventas por hora/día), imágenes (fotos de productos).

## 3) Tratamiento/análisis: pipeline de datos
Explica el flujo de forma ordenada:
- Ingesta (captura/eventos): Recopilación de datos en tiempo real desde el sitio web, redes sociales, y bases de datos internas (ventas 
  y usuarios).
- Limpieza/normalización: Eliminar duplicados, corregir errores tipográficos, y normalizar los datos de producto (categorías, precios) y 
  de usuario (fechas, dispositivos usados).
- Almacenamiento (data lake/warehouse): Los datos se almacenan en un data lake basado en Hadoop para su procesamiento posterior. Los 
  datos históricos de ventas se mantienen en un data warehouse.
- Preparación de variables (features): Se extraen características clave, como la frecuencia de visitas del usuario, el valor de los productos visualizados, tiempo de permanencia en el carrito, y el historial de compras.
- Análisis/BI (opcional): Dashboard de BI para monitorear en tiempo real la tasa de conversión, abandono de carrito, y efectividad de 
  las recomendaciones personalizadas.

## 4) IA aplicada: modelo y decisión
- Tipo de IA/técnica (clasificación, predicción, recomendación, anomalías, NLP...): Predicción de abandono de carrito utilizando modelos 
  de clasificación (Árboles de Decisión, Random Forest).
- Entrada del modelo (qué datos usa): Datos de comportamiento del usuario (navegación, clics), historial de compras previas, 
  características de los productos en el carrito.
- Salida del modelo (qué produce): Probabilidad de que un usuario abandone el carrito antes de finalizar la compra.
- Decisión que habilita (qué hace la empresa con esa salida): La empresa utiliza esta probabilidad para activar recomendaciones 
  personalizadas en tiempo real o descuentos para evitar el abandono y fomentar la compra.

## 5) Rentabilidad: KPIs antes/después (mínimo 3)
KPI 1: Tasa de conversión (compras/visitantes)
- Antes: 3%
- Después: 5%
- Por qué mejora la rentabilidad: La predicción de abandono de carrito permite ofrecer incentivos personalizados en tiempo real, lo que 
  aumenta las conversiones.

KPI 2: Valor promedio de pedido
- Antes: 50 euros
- Después: 60 euros
- Por qué mejora la rentabilidad: Las recomendaciones personalizadas aumentan el valor de los pedidos, sugiriendo productos 
  complementarios a los usuarios.

KPI 3: Costo de adquisición de cliente (CAC)
- Antes: 15 euros
- Después: 10 euros
- Por qué mejora la rentabilidad: Gracias a la mejora en la tasa de conversión, la empresa reduce los costos asociados a la adquisición 
  de nuevos clientes.

## 6) Diagrama del pipeline (ASCII o Mermaid)
(Pega aquí el diagrama)
   A [Captura de datos de usuarios y transacciones] --> B [Limpieza y normalización de datos]
    B --> C [Almacenamiento en Data Lake]
    C --> D [Preparación de características]
    D --> E [Entrenamiento de modelo IA]
    E --> F [Predicción de abandono de carrito]
    F --> G [Acción: Ofertas personalizadas/Descuentos]
    G --> H [Conversión aumentada]

## 7) Riesgos y mitigación
Riesgo 1: Falta de datos de calidad (errores o incompletitud en los datos de usuarios y transacciones).
- Mitigación 1: Implementación de procesos automatizados de validación y limpieza de datos para asegurar la calidad.

Riesgo 2: Desviación de los resultados debido a cambios en el comportamiento de los usuarios.
- Mitigación 2: Monitoreo constante del modelo de IA y actualización periódica de los algoritmos con datos nuevos.

## 8) Valoración (criterio c): importancia presente y futura de la IA (10–15 líneas)
- Importancia actual (hoy): La IA permite a RetailTech optimizar la experiencia del cliente y aumentar las ventas mediante la 
  personalización. Las recomendaciones basadas en IA mejoran la conversión y permiten acciones en tiempo real que responden a las 
  necesidades del consumidor.
- Importancia futura (3–5 años): La IA será aún más crucial con el avance de la tecnología de personalización. La capacidad de predecir 
  comportamientos a nivel individual permitirá una experiencia de compra completamente personalizada y fluida, lo que aumentará la 
  competitividad.
- Condiciones/limitaciones (datos, costes, regulación, ética, seguridad, empleo): La disponibilidad y calidad de los datos es esencial 
  para el éxito de la IA. Además, las preocupaciones sobre privacidad y seguridad, junto con la regulación de los datos personales, 
  pueden limitar el uso de ciertas tecnologías. La ética en el uso de IA también será un área clave de consideración, especialmente en 
  términos de sesgo algorítmico.
- Conclusión razonada: La IA está transformando la industria del retail al hacerla más eficiente y centrada en el cliente. Aunque hay 
  desafíos éticos y regulatorios que deben ser gestionados, la implementación de IA se está convirtiendo en una ventaja competitiva 
  clave que solo crecerá en importancia en el futuro cercano.
