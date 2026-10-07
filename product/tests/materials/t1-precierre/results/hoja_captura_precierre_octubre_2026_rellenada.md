# Hoja de captura — T1 precierre (cierre de octubre 2026)

**Creencia en prueba (13):** tras un precierre de 20 minutos el último día laborable del mes, el primer día del cierre quedan como mucho 2 dudas de facturación abiertas y la última factura sale como tarde el tercer día laborable.
**Umbral:** ≤ 2 dudas abiertas el lunes 2-11 **y** última factura como tarde el miércoles 4-11.
**Lo rellena:** Carlos.

## A. Punto de partida (septiembre)

| Dato | Valor |
|---|---|
| Fecha y hora de la última factura de septiembre (de los correos enviados) | 02-10-2026, 18:47 |
| ¿Se pudo reconstruir? (sí / no) | sí |

## B. Precierre (viernes 30-10)

| Asistente | Rol | Procedencia | ¿Asistió? (sí / no) |
|---|---|---|---|
| Carlos Roldán | Socio-gerente, facturación | real (segmento) | sí |
| David Solé | Gestor de operaciones | real (segmento) | sí |
| Marta Vega | Directora de consultoría | real (segmento) | sí |
| Laura Martín | Directora de formación | real (segmento) | sí |

| Hora de inicio | Hora de fin | Duración (min) |
|---|---|---|
| 16:40 | 17:04 | 24 |

## C. Dudas que salen del precierre

| # | Cliente | Duda | Responsable | Fecha comprometida | ¿Resuelta antes del 2-11? (sí / no) |
|---|---|---|---|---|---|
| 1 | Acme Industrial | Faltan horas de consultoría de la última semana; operaciones tiene 38 h y el consultor reporta 42 h | David Solé | 02-11 | no |
| 2 | Grupo Norte | No coincide el importe del pedido con la propuesta firmada; hay una ampliación de alcance pendiente de validar | Marta Vega | 02-11 | sí |
| 3 | Formación Delta | Pendiente confirmar si el último taller de octubre se factura completo o como sesión reprogramada | Laura Martín | 03-11 | no |
| 4 | Iberdata | Falta el visto bueno del cliente para aplicar una tarifa excepcional acordada verbalmente | David Solé | 02-11 | no |
| 5 | Nova Servicios | Diferencia entre fecha de prestación y fecha indicada en el parte de trabajo | Carlos Roldán | 02-11 | sí |
| 6 | Atlas Tech | Factura preparada pero falta confirmar la referencia de compra del cliente | Carlos Roldán | 03-11 | sí |

## D. Dudas de facturación abiertas el lunes 2-11

| Al empezar el cierre, ¿cuántas dudas de facturación siguen abiertas? (incluidas las que no salieron en el precierre) | 3 |
|---|---|
| ¿Cuáles? (cliente y duda) | Acme Industrial — diferencia de 4 h entre operaciones y parte del consultor; Formación Delta — criterio de facturación del taller reprogramado; Iberdata — pendiente autorización para aplicar la tarifa excepcional |

## E. Facturas enviadas

| Cliente | Fecha | Hora |
|---|---|---|
| Grupo Norte | 02-11-2026 | 10:12 |
| Nova Servicios | 02-11-2026 | 11:36 |
| Atlas Tech | 03-11-2026 | 09:18 |
| Beta Retail | 03-11-2026 | 12:04 |
| Soluciones Médicas | 03-11-2026 | 16:22 |
| Gamma Logistics | 04-11-2026 | 09:41 |
| TecnoRed | 04-11-2026 | 11:07 |
| Servicios Delta | 04-11-2026 | 13:26 |
| Acme Industrial | 05-11-2026 | 10:53 |
| Formación Delta | 05-11-2026 | 15:17 |
| Iberdata | 05-11-2026 | 17:46 |
| Resto de clientes | 05-11-2026 | 18:05 |

## F. Registro por pasos del cierre

| Fecha | Paso | Minutos | ¿Esperando algo de alguien? (qué y de quién) |
|---|---|---|---|
| 02-11 | Revisar diferencias de horas Acme Industrial | 35 | Sí — confirmación de David sobre partes de horas |
| 02-11 | Validar ampliación de alcance Grupo Norte | 20 | No |
| 02-11 | Revisar criterio de facturación Formación Delta | 30 | Sí — confirmación de Laura |
| 02-11 | Revisar tarifa excepcional Iberdata | 25 | Sí — autorización de cliente |
| 02-11 | Preparar facturas ya validadas | 40 | No |
| 03-11 | Cerrar discrepancia Acme Industrial | 45 | Sí — respuesta del consultor |
| 03-11 | Confirmar facturación Formación Delta | 35 | Sí — confirmación del cliente |
| 04-11 | Obtener autorización Iberdata | 50 | Sí — cliente |
| 04-11 | Recalcular importes y revisar facturas | 55 | No |
| 05-11 | Emitir últimas facturas y comprobación final | 70 | No |

## Lectura (la hace `/analyze-solution-tests`)

| | Valor | Umbral |
|---|---|---|
| Dudas abiertas el 2-11 (D) | 3 | ≤ 2 |
| Fecha de la última factura (E) | 05-11-2026, 18:05 | ≤ 4-11 |
| ¿Asistieron los dos directores? (B) | sí | si no → `inconclusive` |
| ¿Se reconstruyó la fecha de septiembre? (A) | sí | si no → `inconclusive` |
