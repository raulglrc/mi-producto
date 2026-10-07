# Hoja de captura — T1 precierre (cierre de octubre 2026)

**Creencia en prueba (13):** tras un precierre de 20 minutos el último día laborable del mes, el primer día del cierre quedan como mucho 2 dudas de facturación abiertas y la última factura sale como tarde el tercer día laborable.
**Umbral:** ≤ 2 dudas abiertas el lunes 2-11 **y** última factura como tarde el miércoles 4-11.
**Lo rellena:** Carlos.

## A. Punto de partida (septiembre)

| Dato | Valor |
|---|---|
| Fecha y hora de la última factura de septiembre (de los correos enviados) | |
| ¿Se pudo reconstruir? (sí / no) | |

## B. Precierre (viernes 30-10)

| Asistente | Rol | Procedencia | ¿Asistió? (sí / no) |
|---|---|---|---|
| Carlos Roldán | Socio-gerente, facturación | real (segmento) | |
| David Solé | Gestor de operaciones | real (segmento) | |
| | Director/a de consultoría | real (segmento) | |
| | Director/a de formación | real (segmento) | |

| Hora de inicio | Hora de fin | Duración (min) |
|---|---|---|
| | | |

## C. Dudas que salen del precierre

| # | Cliente | Duda | Responsable | Fecha comprometida | ¿Resuelta antes del 2-11? (sí / no) |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

## D. Dudas de facturación abiertas el lunes 2-11

| Al empezar el cierre, ¿cuántas dudas de facturación siguen abiertas? (incluidas las que no salieron en el precierre) | |
|---|---|
| ¿Cuáles? (cliente y duda) | |

## E. Facturas enviadas

| Cliente | Fecha | Hora |
|---|---|---|
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |
| | | |

## F. Registro por pasos del cierre

| Fecha | Paso | Minutos | ¿Esperando algo de alguien? (qué y de quién) |
|---|---|---|---|
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |

## Lectura (la hace `/analyze-solution-tests`)

| | Valor | Umbral |
|---|---|---|
| Dudas abiertas el 2-11 (D) | | ≤ 2 |
| Fecha de la última factura (E) | | ≤ 4-11 |
| ¿Asistieron los dos directores? (B) | | si no → `inconclusive` |
| ¿Se reconstruyó la fecha de septiembre? (A) | | si no → `inconclusive` |
