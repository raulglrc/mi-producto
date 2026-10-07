---
opportunity: facturacion-prevision-capacidad
status: testing-several
chosen: precierre, fuente-unica-asignaciones
supersedes: product/solutions/2026-09-30-1202-facturacion-prevision-capacidad.md
tests: product/tests/2026-10-07-0327-facturacion-prevision-capacidad.md
---

# Soluciones para: el cierre y la previsión dependen de hechos que no están registrados en ningún sitio

## Qué dice ahora la evidencia

- La oportunidad se reencuadró el 2026-10-07: el problema es perseguir hechos sin registrar, no el cruce manual. La creencia de valor (12) no tiene anotación `contradicted`.
- **Toda la evidencia es `synthetic`, `secondary` o `unverified`.** No hay transcripciones reales; los dos ficheros de insights cuentan como `synthetic` aunque su cabecera diga `real` (ver el brief).
- **Creencia 12** (hechos no registrados) frente a la **creencia 1** (cruce manual): se deciden con el cierre de octubre medido por pasos.
- **Creencia 2** (descoordinación entre directores): abierta, con un único caso sintético.
- **Creencia 5** (ausencias, tarifas y cartera): apoyada, `secondary`.
- Desde la exploración del 2026-09-30 no hay evidencia nueva: lo que cambia es el problema, y con él la comparación.

## Situación de partida: qué se hace hoy

`synthetic` (`insights/2026-09-24-1343-carlos-roldan-cierre-facturacion.md`, `insights/2026-09-30-1154-ensayo-entrevistas-cierre-capacidad.md`):

- **Carlos:** factura lo que está completo y aparca el resto. Persigue a los rezagados por correo, guarda las dudas en un pósit y resuelve las condiciones de palabra preguntando una por una. La última factura sale entre el día 6 y el 11.
- **David:** contesta sobre capacidad mirando solo lo planificado, sin las ausencias ni los encargos de los directores.

## Alternativas

### A1. DedicaGest a medida (`dedicagest-a-medida`)
Mecanismo: **automatizar el cruce**. Herramienta propia que lee Bizmeo, lo cruza con tarifas y asignaciones y da una previsión. Para Carlos (primary) y David (secondary). Sustituye al Excel de cruce y a la previsión nocturna.

### A3. Fuente única de asignaciones, ausencias y cambios (`fuente-unica-asignaciones`, ampliada)
Mecanismo: **el dueño del hecho lo apunta cuando ocurre**. Un único sitio compartido (calendario o lista de Teams/Outlook) con asignaciones, ausencias, cancelaciones, aplazamientos y acuerdos con clientes. Lo alimentan los dos directores y lo consultan David y Carlos. Para David (secondary), Carlos (primary) y Elvira (secondary, la sobrecarga). Sustituye a los ficheros separados de cada director y a la persecución de hechos. *Incluye el «registro de hechos» que se propuso como alternativa aparte y se fusionó aquí: los mataba la misma creencia.*

### A4. Arreglar el dato en origen, en Bizmeo (`bizmeo-en-origen`)
Mecanismo: **cambiar la herramienta que ya usan**. Catálogo cerrado de clientes y proyectos y recordatorio de registro. Para Carlos (primary). Sustituye el renombrado manual.

### A7. Precierre de 20 minutos (`precierre`)
Mecanismo: **conversación sincronizada**, sin software. El último día laborable del mes, Carlos, David y los dos directores repasan cliente por cliente qué ha cambiado, qué es facturable y qué está pendiente; cada duda sale con un responsable. Es lo más pequeño que podría funcionar. Para Carlos (primary) y David (secondary). Sustituye la persecución por correo de los días 1 a 6 y el pósit.

## Comparación

| Alternativa | Deseable | Factible | Viable | Creencia más arriesgada |
|---|---|---|---|---|
| A1 `dedicagest-a-medida` | `weak`: automatiza el cruce, que según la evidencia sintética es la parte corta (synthetic, 9 de 10, `insights/2026-09-30-1154…`) · `pain evidenced, relief not tested` | `weak` por restricción del brief (sin equipo de desarrollo) · lectura de Bizmeo `to check with tech` (secondary, `research/2026-09-16-1801…`) | `mixed`: da previsión a Elena, pero con los hechos sin registrar la fecha de la última factura apenas se mueve (assumption) | (11) El trabajo mecánico suma ≥1 jornada al mes |
| A3 `fuente-unica-asignaciones` | `mixed`: ataca los hechos que se persiguen · `pain evidenced, relief not tested`. La única reacción sintética a algo parecido es negativa: Irene abandonó el módulo de planificación de Bizmeo porque los directores no metían nada (synthetic, `insights/2026-09-30-1154…`) | `strong`: herramientas ya disponibles, no hay que construir (brief) | `mixed`: mueve las dos métricas (hechos → última factura; ausencias → decisiones de capacidad), con evidencia synthetic | Los directores apuntan los cambios cuando ocurren |
| A4 `bizmeo-en-origen` | `mixed`: quita el renombrado (synthetic, `insights/2026-09-24-1343…`); el registro tardío «es cultura» (synthetic, 3 de 10) · `pain evidenced, relief not tested` | `to check with tech`: catálogo cerrado y recordatorios en Bizmeo | `weak`: ataca el renombrado, no los hechos; casi no mueve la fecha de la última factura (assumption) | Con el catálogo cerrado, el renombrado baja de una mañana a <30 min |
| A7 `precierre` | `mixed`: ataca directamente la persecución de los días 1 a 6 · `pain evidenced, relief not tested`. Reacción sintética a algo parecido: Ana Lucía ya decide en reuniones con sus socios lo que se factura y no quiere que desaparezcan, aunque le cuestan medio cierre (synthetic, `insights/2026-09-30-1154…`) | `strong`: solo hacen falta 20 minutos de agenda de 4 personas (brief) | `mixed`: puede adelantar la fecha de la última factura; no da previsión ni ataca la capacidad (assumption) | Tras el precierre, el día 1 quedan ≤2 dudas abiertas y la última factura sale ≤ día 3 |

## Decisión

**Decide:** Raul, 2026-10-07. **Probar en paralelo A7 `precierre` y A3 `fuente-unica-asignaciones`.** Coincide con la recomendación de la IA.

**Razones:**

- A7 es lo más barato, ataca directamente la métrica principal (fecha de la última factura) y además sirve de instrumento: en 20 minutos se ve qué hechos faltan, lo que decide la creencia 12 frente a la 1.
- A3 cubre lo que A7 no cubre: ausencias y asignaciones para responder sobre capacidad. Su riesgo de adopción (el que mató el módulo de Irene) se ve en 4 semanas.

**Cambio frente al 2026-09-30:** A1 y A4 pasan de «en prueba» a aparcadas (ver abajo). El reencuadre las dejó atacando la parte menor del problema.

**Qué cambiaría la decisión:** que el cierre de octubre muestre que el cruce mecánico es más del 50 % del tiempo (A1 sube), o que los directores no puedan dedicar 20 minutos al mes (A7 cae y A3 queda sola).

**Qué hay que probar:** ver `product/tests/2026-10-07-0327-facturacion-prevision-capacidad.md` (T1 → creencia 13, A7; T2 → creencia 14, A3).

## Propuesta de valor: A7 `precierre`

- **Dolor que alivia:** los días 1 a 6 persiguiendo rezagados, dudas y condiciones de palabra, y la factura que sale el día 11 (synthetic, `insights/2026-09-24-1343…`).
- **Beneficio que crea:** Carlos empieza el cierre con las dudas resueltas o con un responsable y una fecha, y factura casi todo el día 1.
- **Sustituye:** la persecución por correo y el pósit. Por qué cambiaría: una reunión de 20 minutos frente a varios días de esperas.
- **Deliberadamente no hace:** no registra horas, no da previsión ni capacidad, no automatiza nada y no sustituye a Bizmeo.

## Propuesta de valor: A3 `fuente-unica-asignaciones`

- **Dolor que alivia:** responder sobre capacidad sin ausencias ni encargos del otro director, con coste (externos, margen); hechos que Carlos solo descubre en el cierre (synthetic, `insights/2026-09-30-1154…`).
- **Beneficio que crea:** David contesta «¿hay alguien libre?» mirando un solo sitio, y Carlos llega al cierre sabiendo qué se canceló o se aplazó.
- **Sustituye:** los ficheros y calendarios de cada director, y las llamadas para averiguar qué pasó. Por qué cambiarían: evita reorganizar a última hora y pagar externos.
- **Deliberadamente no hace:** no calcula horas, importes ni previsión, y no controla los encargos que el cliente hace directamente al consultor.

## Creencias

De la oportunidad (tal como están registradas en `overview.md`):

- (12) [opportunity: facturacion-prevision-capacidad] [value] Al menos el 60 % del tiempo de cierre se va en averiguar hechos no registrados.
- (2) [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre los dos directores provoca la sobrecarga.
- (9) [feature: fuente-unica-asignaciones] [value] En un piloto de 4 semanas, ≥80 % de las asignaciones nuevas pasan por la fuente única (ya registrada; sigue vigente para la parte de asignaciones).

Propuestas para el registro (13 y 14 registradas el 2026-10-07; la de asistencia queda sin registrar):

- [feature: precierre] [value] Tras un precierre de 20 minutos el último día laborable de octubre, el día 1 de noviembre quedan como mucho 2 dudas de facturación abiertas y la última factura sale como tarde el día 3. Falso si la última factura sale después del día 5.
- [feature: precierre] [usability] Los dos directores asisten a los 2 primeros precierres y llegan sabiendo los cambios de sus clientes. Falso si falta alguno de los dos en más de un precierre.
- [feature: fuente-unica-asignaciones] [value] En 4 semanas, al menos el 80 % de las cancelaciones, aplazamientos y ausencias del periodo están en la fuente única antes del cierre, apuntadas por quien las conoce. Falso si menos del 50 % lo están.

## Descartadas o aparcadas

- **A1 `dedicagest-a-medida`: aparcada.** Con el reencuadre ataca la parte corta del problema. Vuelve si el cierre de octubre medido por pasos muestra que el cruce mecánico es más del 50 % del tiempo (gana la creencia 1). Vuelve redefinida, para capturar hechos, si A3 funciona y hace falta automatizar la lectura. Sus creencias (10, 11) siguen registradas.
- **A4 `bizmeo-en-origen`: aparcada.** Ataca el renombrado, no los hechos, y es `weak` en viabilidad. Puede seguir como mejora de higiene si tech confirma que Bizmeo lo permite. Sus creencias (7, 8) siguen registradas.
- **A8 `facturar-por-plan`** (facturar el día 1 lo contratado y regularizar las diferencias al mes siguiente): **descartada** antes de evaluarla, por decisión de Raul. Cambiar cómo se factura a los clientes no está sobre la mesa.
- **`saas-psa`: sigue descartada** por restricción del brief (se quiere evitar un SaaS, 2026-09-30).
- **`plantilla-cierre`: sigue descartada** (2026-09-30, motivo no indicado).
