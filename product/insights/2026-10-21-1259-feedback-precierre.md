---
source: synthetic
corpus: product/data/comentarios_precierre_facturacion_30.csv
metrics-analysis: none
period: n/a to n/a
---

# Análisis de feedback: Precierre mensual de facturación

## Corpus
30 entradas: 10 `ticket`, 10 `review`, 10 `producto`. Sin fechas, así que no hay tendencia. Ninguna fuera de alcance.

Por autor: Carlos 15 (50 %), David 6, director de consultoría 5, director de formación 4. Los temas se inclinan hacia lo que necesita Carlos.

Todas las entradas son `synthetic`, generadas a partir del spec (`specs/2026-10-21-1156-precierre.md`) antes del primer precierre real (30-10). Son expectativas, no uso: no puede haber `bug` ni `usability`. Por tipo: 20 `request` (67 %), 8 `praise` (27 %), 2 `complaint` (7 %).

Las etiquetas de fuente están repartidas de forma artificial, así que no tienen el sesgo de una fuente real. Como el corpus sale del spec, en buena parte lo repite: que coincida con él no es evidencia.

No hay análisis de métricas: `metrics/2026-10-21-1300-precierre.md` está en `designed`. Este análisis va solo.

La columna `tema` del CSV no se ha usado, porque cada entrada tiene una etiqueta distinta. El etiquetado se ha hecho desde cero y el recuento, a mano (30 entradas, comprobado que suman 30).

## Temas

### F1. Cada duda sale con un responsable concreto, una fecha y una lista explícita
- **Entradas:** 7 (23 %): COM-002, 005, 009, 014, 015, 017, 025 · **Fuentes:** review 4, producto 2, ticket 1 · **Autores:** Carlos 4, director de consultoría 2, David 1
- **Parte de la feature:** dudas (responsable, fecha y lectura final)
- **Tipo:** request (5), praise (2)
- **Severidad:** alta. Es el tema más frecuente, y una duda sin dueño vuelve a Carlos, que es lo que mide su activación.
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** sí, en la historia 3.
- > «Si una duda tiene fecha pero nadie es responsable, en realidad sigue siendo una duda de Carlos. El responsable debe ser una persona concreta.» (COM-025)
- > «Que cada duda tenga responsable y fecha es clave. Si solo ponemos 'pendiente', dentro de dos días estamos igual.» (COM-005)

### F2. Estado claro de «listo» frente a «duda abierta», sin facturas provisionales
- **Entradas:** 4 (13 %): COM-016, 018, 021, 022 · **Fuentes:** ticket 2, producto 2 · **Autores:** solo Carlos
- **Parte de la feature:** estado por cliente el día 1
- **Tipo:** request
- **Severidad:** alta. Si falla, sale una factura que luego hay que rectificar.
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** sí, en la historia 4. La vista resumen de un vistazo (COM-021) no está.
- > «El mayor riesgo para mí es facturar un importe provisional y olvidarme de corregirlo después. El estado abierto debería impedirlo.» (COM-022)

### F3. Lista de clientes completa, generada de Bizmeo y con añadidos manuales
- **Entradas:** 4 (13 %): COM-001, 003, 012, 027 · **Fuentes:** producto 3, ticket 1 · **Autores:** Carlos 3, director de formación 1
- **Parte de la feature:** lista de clientes (orden del día)
- **Tipo:** request (3), praise (1)
- **Severidad:** media-alta. Un cliente que no está en la lista no se repasa.
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** sí, en la historia 1 y su caso límite.
- > «Un cliente sin horas imputadas pero con un curso previsto no debería desaparecer de la lista. Necesitamos poder añadirlo durante el precierre.» (COM-012)

### F4. Reunión corta, sencilla y centrada en excepciones
- **Entradas:** 4 (13 %): COM-006, 008, 020, 024 · **Fuentes:** producto 2, review 2 · **Autores:** David 2, Carlos 1, director de consultoría 1
- **Parte de la feature:** formato y duración del precierre
- **Tipo:** request (3), complaint (1)
- **Severidad:** media. El coste de tiempo recae en los participantes, que es lo que pregunta su encuesta de satisfacción.
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** en parte. El límite de 25 minutos y la opción «sin cambios» sí están. Pero el spec dice «cliente por cliente», mientras que COM-020 pide repasar solo excepciones.
- > «La reunión tiene que estar enfocada a excepciones. Repasar durante veinte minutos cosas que no han cambiado sería perder el tiempo.» (COM-020)
- > «Me preocupa que el precierre se convierta en otra reunión larga. Si realmente dura 20 o 25 minutos, sí le veo sentido.» (COM-008)

### F5. Los cambios de cada cliente afloran antes de facturar
- **Entradas:** 3 (10 %): COM-007, 010, 019 · **Fuentes:** ticket 3 · **Autores:** Carlos, David, director de formación
- **Parte de la feature:** columna de cambios
- **Tipo:** praise (2), request (1)
- **Severidad:** media
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** sí, en la historia 2.
- > «Hoy descubro algunas cancelaciones cuando ya estoy preparando la factura. Si eso aparece en el precierre, me ahorra una rectificación.» (COM-007)

### F6. Sustituye las preguntas sueltas y la búsqueda de hechos por una fuente común
- **Entradas:** 3 (10 %): COM-004, 023, 030 · **Fuentes:** ticket 1, review 1, producto 1 · **Autores:** David, director de formación, Carlos
- **Parte de la feature:** propuesta de valor del precierre
- **Tipo:** praise (2), request (1)
- **Severidad:** baja
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** es la propuesta de valor del spec.
- > «Si el precierre obliga a tener los hechos en un sitio común, reduce bastante la dependencia de lo que cada persona recuerda.» (COM-023)

### F7. Los clientes que no se repasan por una ausencia quedan visibles
- **Entradas:** 2 (7 %): COM-011, 028 · **Fuentes:** review 1, ticket 1 · **Autores:** los dos directores
- **Parte de la feature:** ausencias
- **Tipo:** request
- **Severidad:** media. Si falta un director, el nivel queda inconcluso.
- **Tendencia:** n/a
- **¿Lo cubre el spec?:** sí, en el caso límite de la historia 2.
- > «Necesitamos saber claramente qué clientes no hemos podido repasar por ausencia de alguien. No debería quedar como un hueco silencioso.» (COM-028)

## Lo que no repite el spec
Es lo único del corpus que aporta información:
- **F4:** «cliente por cliente» (spec) frente a «solo excepciones» (COM-020). Las dos ideas chocan con el límite de 25 minutos.
- **COM-013:** recibir la lista *antes* del precierre para llegar preparados. En el spec, la lista se prepara la misma mañana. Toca la creencia 15, la de que los directores «llegan sabiendo los cambios».
- **COM-021:** una vista resumen de un vistazo (con cambios, facturable, pendiente).

## Contra las hipótesis de métricas
No aplica: no hay análisis de métricas. Las preguntas reales se responden con `duda_abierta_dia1` el 2-11 y con la encuesta del 6-11.

El umbral de activación de Carlos (2 dudas abiertas o menos el 2-11) es la línea de la hipótesis del spec. Esta dice que Carlos empezará el cierre con como mucho 2 dudas abiertas, y que se equivoca si quedan 3 o más.

## Señales débiles
- COM-013: recibir la lista antes del precierre (`request`, director de consultoría).
- COM-026: el día 1 solo se siguen las excepciones (`praise`, David). Ya está en la historia 4.
- COM-029: el valor tendrá que demostrarse en las dudas abiertas, no en la fecha de la última factura (`complaint`, Carlos). Repite el aviso que ya tiene el propio spec.

## Overview
Al ser `synthetic`, no se anota ninguna creencia.
