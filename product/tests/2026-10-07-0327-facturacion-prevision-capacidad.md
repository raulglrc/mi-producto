---
opportunity: facturacion-prevision-capacidad
solutions: product/solutions/2026-10-07-0320-facturacion-prevision-capacidad.md
status: designed
---

# Tests de solución para: el cierre y la previsión dependen de hechos que no están registrados en ningún sitio

## Por qué probar

Hay dos alternativas en prueba: A7 `precierre` y A3 `fuente-unica-asignaciones`. El dolor que atacan está evidenciado solo con fuentes `synthetic` y `unverified`, y nadie ha reaccionado todavía a ninguna de las dos. Lo más parecido a A3 que aparece en la evidencia (el módulo de planificación de Bizmeo de Irene, `synthetic`) se abandonó porque los directores no metían datos. Los dos tests se hacen con las personas reales del segmento y en el ciclo de octubre. T2 termina antes que T1, y el precierre de T1 sirve también como segunda comprobación de T2.

## T1. precierre: un precierre real a mano en el cierre de octubre

- **Test status:** ready
- **Belief under test:** (13) «[feature: precierre] [value] Tras un precierre de 20 minutos el último día laborable del mes, el primer día del cierre quedan como mucho 2 dudas de facturación abiertas y la última factura sale como tarde el tercer día laborable. Falso si sale después del quinto.»
- **Risk:** [value]
- **Test type:** concierge
- **What we do:**
  1. Antes del 30-10, Carlos saca de sus correos de envío la fecha de la última factura de septiembre (punto de partida real) y la apunta en la hoja de captura.
  2. Viernes 30-10: precierre de 20 minutos con Carlos, David y los dos directores. Se repasan cliente por cliente tres cosas: qué ha cambiado este mes (cancelaciones, aplazamientos, ausencias, acuerdos con el cliente), qué es facturable y qué queda pendiente. Cada duda sale con un responsable y una fecha.
  3. Lunes 2-11: Carlos cuenta las dudas de facturación que siguen abiertas al empezar el cierre.
  4. Carlos apunta la fecha y la hora de cada factura enviada hasta la última. Además, anota por pasos lo que hace durante el cierre (paso y minutos), porque eso sirve también a la agenda de las creencias 12 frente a 1.
- **With whom:** Carlos Roldán (primary), David Solé (secondary) y los dos directores de área (consultoría y formación). Son las 4 personas reales; se convocan directamente.
- **Material needed:**
  - Orden del día de una página: la lista de clientes activos del mes con tres columnas (cambios, facturable, pendiente → responsable y fecha).
  - Hoja de captura con: fecha de la última factura de septiembre; asistentes al precierre y su duración; dudas que salen del precierre (responsable y fecha); dudas abiertas el 2-11; fecha y hora de cada factura; registro por pasos del cierre (paso, minutos, qué se esperaba).
  - Se deja fuera a propósito: cualquier herramienta nueva, automatización o cambio en Bizmeo.
- **Material:** [product/tests/materials/t1-precierre/](materials/t1-precierre/) — orden del día, guion, hoja de captura, convocatoria
- **Duration:** 20 minutos de precierre (30-10) más el cierre de octubre (2-6 nov.)
- **Signal and threshold:** dudas de facturación abiertas el 2-11 **≤ 2**, y última factura enviada **como tarde el miércoles 4-11** (tercer día laborable). Se registra también la diferencia con la fecha de septiembre, pero no forma parte del umbral.
- **Decision rule:**
  - **continue** si se cumplen las dos condiciones.
  - **change** si la última factura sale el jueves 5-11 o el viernes 6-11, o si quedan 3-4 dudas abiertas. Se revisa qué hechos no aparecieron en el precierre y por qué (quién no los traía, si faltó tiempo).
  - **discard** si la última factura sale después del 6-11 (quinto día laborable) o quedan 5 o más dudas abiertas.
  - **inconclusive** si falta alguno de los dos directores al precierre, o si Carlos no puede reconstruir la fecha de septiembre. En ese caso se repite en noviembre, sin mover el umbral.
- **Expected provenance:** real
- **Next step if it passes:** repetir el precierre en los cierres de noviembre y diciembre con el mismo umbral, para descartar que octubre sea un mes atípico. Si los dos pasan → ready for spec (proceso de precierre).

## T2. fuente-unica-asignaciones: dos semanas de lista compartida, comprobada contra la conciliación de David

- **Test status:** designed
- **Belief under test:** (14) «[feature: fuente-unica-asignaciones] [value] Al menos el 80 % de las cancelaciones, aplazamientos y ausencias del periodo están en la fuente única antes de que se descubran por otra vía, apuntadas por quien las conoce. Falso si menos del 50 % lo están.»
- **Risk:** [value]
- **Test type:** concierge
- **What we do:**
  1. Martes 13-10 (el 12-10 es festivo): se crea una lista compartida en Teams y se explica en 5 minutos a los dos directores. La consigna: cada cancelación, aplazamiento, ausencia o asignación nueva se apunta en cuanto la conocéis.
  2. Lunes 19-10 y lunes 26-10: al conciliar Bizmeo con su Excel, David apunta cada cambio que descubre en la semana anterior y comprueba si ya estaba en la lista con una fecha anterior al descubrimiento.
  3. Viernes 30-10 (precierre de T1): los cambios que salen en el precierre se comprueban contra la lista de la misma forma.
  4. Recuento: cambios del periodo 13-23 oct. que ya estaban en la lista antes de descubrirse ÷ total de cambios descubiertos por cualquier vía.
- **With whom:** los dos directores de área (apuntan), David Solé (secondary, comprueba) y Carlos Roldán (primary, en el precierre). Son las personas reales.
- **Material needed:**
  - Lista compartida en Teams con cinco campos: tipo de cambio (cancelación, aplazamiento, ausencia, asignación nueva), persona o cliente afectado, fecha del hecho, fecha en que se apunta (automática), y quién lo apunta.
  - Hoja de captura para David: por cada cambio descubierto, la fecha del descubrimiento, la vía (conciliación del lunes, precierre, otro), si estaba en la lista y con qué fecha.
  - Se deja fuera a propósito: avisos o notificaciones, integración con Bizmeo, vista de capacidad y cualquier recordatorio a los directores durante las dos semanas, porque falsearía la señal.
- **Material:** pendiente de `/build-solution-test`
- **Duration:** 2 semanas de registro (13-23 oct.), con comprobaciones el 19-10, el 26-10 y el 30-10
- **Signal and threshold:** porcentaje de cambios descubiertos que ya estaban en la lista con fecha anterior. **≥ 80 %** → pasa.
- **Decision rule:**
  - **continue** si ≥ 80 %.
  - **change** si está entre 50 y 79 %. Se revisa qué tipo de cambio o qué director falla, y se prueba una versión distinta.
  - **discard** si < 50 %.
  - **inconclusive** si en el periodo se descubren menos de 5 cambios: en ese caso se amplía 2 semanas, con el mismo umbral.
- **Expected provenance:** real
- **Next step if it passes:** el piloto de 4 semanas de la creencia (9). David responde las preguntas sobre capacidad usando solo la lista, y se cuentan los choques de asignación descubiertos después.

## Results

*(Lo añade `/analyze-solution-tests`.)*

## Decision

*(Lo añade `/analyze-solution-tests`.)*
