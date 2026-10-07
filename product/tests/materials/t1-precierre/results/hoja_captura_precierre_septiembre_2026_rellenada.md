# Hoja de captura — T1 precierre (cierre de septiembre 2026)

**Creencia en prueba (13):** tras un precierre de 20 minutos el último día laborable del mes, el primer día del cierre quedan como mucho 2 dudas de facturación abiertas y la última factura sale como tarde el tercer día laborable.
**Umbral:** ≤ 2 dudas abiertas el jueves 1-10 **y** última factura como tarde el lunes 5-10.
**Lo rellena:** Carlos.

## A. Punto de partida (septiembre)

| Dato | Valor |
|---|---|
| Fecha y hora de la última factura de septiembre (de los correos enviados) | 02-10-2026, 17:42 |
| ¿Se pudo reconstruir? (sí / no) | sí |

## B. Precierre (miércoles 30-09)

| Asistente | Rol | Procedencia | ¿Asistió? (sí / no) |
|---|---|---|---|
| Carlos Roldán | Socio-gerente, facturación | real (segmento) | sí |
| David Solé | Gestor de operaciones | real (segmento) | sí |
| Marta Vega | Directora de consultoría | real (segmento) | sí |
| Laura Martín | Directora de formación | real (segmento) | sí |

| Hora de inicio | Hora de fin | Duración (min) |
|---|---|---|
| 16:35 | 16:55 | 20 |

## C. Dudas que salen del precierre

| # | Cliente | Duda | Responsable | Fecha comprometida | ¿Resuelta antes del 1-10? (sí / no) |
|---|---|---|---|---|---|
| 1 | Acme Industrial | Diferencia de horas entre el parte de consultoría y el registro de operaciones | David Solé | 01-10 | sí |
| 2 | Grupo Norte | Falta confirmar una ampliación de alcance incluida en la propuesta | Marta Vega | 01-10 | sí |
| 3 | Formación Delta | Confirmar si el último taller se factura completo | Laura Martín | 02-10 | sí |
| 4 | Iberdata | Validar una tarifa excepcional acordada con el cliente | David Solé | 01-10 | sí |
| 5 | Nova Servicios | Diferencia entre fecha de prestación y fecha del parte | Carlos Roldán | 01-10 | sí |
| 6 | Atlas Tech | Falta la referencia de compra del cliente | Carlos Roldán | 02-10 | sí |

## D. Dudas de facturación abiertas el jueves 1-10

| Al empezar el cierre, ¿cuántas dudas de facturación siguen abiertas? (incluidas las que no salieron en el precierre) | 2 |
|---|---|
| ¿Cuáles? (cliente y duda) | Formación Delta — criterio de facturación del taller; Iberdata — confirmación final de tarifa |

## E. Facturas enviadas

| Cliente | Fecha | Hora |
|---|---|---|
| Grupo Norte | 01-10-2026 | 10:08 |
| Nova Servicios | 01-10-2026 | 11:21 |
| Acme Industrial | 01-10-2026 | 15:36 |
| Atlas Tech | 02-10-2026 | 09:47 |
| Beta Retail | 02-10-2026 | 10:32 |
| Soluciones Médicas | 02-10-2026 | 12:15 |
| Gamma Logistics | 02-10-2026 | 14:08 |
| TecnoRed | 02-10-2026 | 15:26 |
| Servicios Delta | 05-10-2026 | 09:18 |
| Formación Delta | 05-10-2026 | 10:41 |
| Iberdata | 05-10-2026 | 11:23 |
| Resto de clientes | 05-10-2026 | 12:06 |

## F. Registro por pasos del cierre

| Fecha | Paso | Minutos | ¿Esperando algo de alguien? (qué y de quién) |
|---|---|---|---|
| 01-10 | Revisar diferencias de horas Acme Industrial | 30 | Sí — confirmación de David sobre partes |
| 01-10 | Validar ampliación Grupo Norte | 20 | No |
| 01-10 | Revisar tarifa Iberdata | 25 | Sí — confirmación del cliente |
| 01-10 | Preparar facturas validadas | 45 | No |
| 02-10 | Confirmar criterio Formación Delta | 30 | Sí — respuesta de Laura |
| 02-10 | Revisar referencias de compra | 25 | Sí — clientes |
| 02-10 | Emitir segunda tanda de facturas | 40 | No |
| 05-10 | Cerrar Formación Delta | 30 | No |
| 05-10 | Cerrar Iberdata | 35 | Sí — última confirmación del cliente |
| 05-10 | Emitir últimas facturas y comprobación final | 55 | No |

## Lectura (la hace `/analyze-solution-tests`)

| | Valor | Umbral |
|---|---|---|
| Dudas abiertas el 1-10 (D) | 2 | ≤ 2 |
| Fecha de la última factura (E) | 05-10-2026, 12:06 | ≤ 05-10-2026 |
| ¿Asistieron los dos directores? (B) | sí | si no → `inconclusive` |
| ¿Se reconstruyó la fecha de septiembre? (A) | sí | si no → `inconclusive` |
