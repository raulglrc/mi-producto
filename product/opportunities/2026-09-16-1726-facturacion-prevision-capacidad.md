---
status: framed
reframed: 2026-10-07
segment: Gestión operativa y administrativa de una consultora/academia de 15 personas (consultores y formadores)
personas: carlos-roldan, david-sole, elvira-ametller, elena-puig
---

# Opportunity: el cierre y la previsión dependen de hechos que no están registrados en ningún sitio

Quien factura (Carlos) y quien planifica (David) pierden días cada mes persiguiendo hechos que no están registrados en ningún sitio: cursos cancelados o aplazados, ausencias y bajas, acuerdos con clientes, horas sin imputar. Por eso la última factura sale tarde, y las respuestas sobre capacidad y previsión se dan sin esos hechos, con coste: externos no previstos, margen perdido, facturación aplazada y sobrecarga que nadie ve a tiempo. **Por qué ahora:** la exploración del 2026-09-30 eligió soluciones con la formulación anterior («cruzar a mano»), y la evidencia nueva apunta a que el cruce es la parte corta.

> **Reencuadre 2026-10-07.** La formulación del 2026-09-16 («dedican varios días a cruzar a mano Bizmeo, tarifas y asignaciones») pasa a ser una parte menor del problema. Toda la evidencia que lo motiva es `synthetic`. Si las entrevistas reales con Carlos y David muestran que el cruce mecánico es más de la mitad del cierre, se vuelve a la formulación anterior.

## Segmento y personas

| Persona | Tipo | ¿Sufre este problema? |
|---|---|---|
| **Carlos Roldán** (socio-gerente, facturación) | primary | Sí, directamente: persigue rezagados, dudas pendientes y condiciones de palabra antes de facturar |
| **David Solé** (gestor de operaciones) | secondary *(type propuesto, no está en su fichero)* | Sí, directamente: responde sobre capacidad sin ausencias ni encargos de los directores |
| **Elvira Ametller** (formadora) | secondary *(type propuesto)* | Sí, la consecuencia: sobrecarga que nadie detecta a tiempo |
| **Elena Puig** (directora general) | tertiary *(type propuesto)* | Indirectamente: decide contrataciones y aceptar clientes con previsiones poco fiables. Es quien responde la creencia de viabilidad |
| **Ramón Ferrer** (socio-fundador) | negative *(type propuesto)* | No: prefiere seguir con su Excel |

**Persona que falta:** el **director/a de área que asigna** (consultoría y formación). Tiene los hechos que los demás persiguen: qué se canceló, qué se aplazó, a quién asignó. Hoy ninguna persona lo modela → `/generate-personas`.

*Nota:* `javier-roldan.md`, `marta-sole.md` y `pol-ametller.md` repiten el contenido de Carlos, David y Elvira, y no se han usado.

## Señales

| Señal | Provenance | Source |
|---|---|---|
| El cruce en sí cuesta entre 5 minutos y media jornada al mes; el resto del cierre (1,5-3 días) se va en averiguar qué pasó (9 de 10) | synthetic | `insights/2026-09-30-1154-ensayo-entrevistas-cierre-capacidad.md` |
| Respuestas de capacidad en 10-20 minutos sin ausencias ni encargos de otros, con coste (≈2.000 €, margen perdido, 2 semanas de facturación aplazada, previsión un 18 % por debajo) | synthetic | ídem |
| El registro tardío bloquea facturas concretas (7 de 10); lo ven como cultura | synthetic | ídem |
| Carlos: cierre del día 1 al 6, con una factura retrasada al 11; dudas pendientes en un pósit; previsión montada de noche con tarifa media y sin vacaciones | synthetic | `insights/2026-09-24-1343-carlos-roldan-cierre-facturacion.md` |
| Para una previsión fiable hacen falta tarifas, ausencias y cartera ponderada por probabilidad | secondary | `research/2026-09-16-1801-mercado-capacity-billing-forecast.md` |
| Carlos dedica cerca de tres días al mes al cierre; David, 3-4 h a la semana | synthetic | `personas/carlos-roldan.md`, `personas/david-sole.md` |
| Hay sobrecarga real por falta de datos compartidos entre los dos directores | unverified | Raul (stakeholder), conversación |
| Resolver la facturación ahorraría aproximadamente 1 jornada al mes al responsable financiero | unverified | Raul (stakeholder), conversación |

> Los dos ficheros de insights llevan hoy `source: real` en la cabecera, pero se extrajeron de transcripciones `synthetic` (`interviews/2026-09-24-1312-carlos-roldan.md` y `notas/ensayo/`). Aquí cuentan como `synthetic` hasta que existan transcripciones reales y su propio fichero de insights. La encuesta de ensayo (`notas/ensayo/`) no cuenta como señal.

## Resultado de negocio

Producto interno, con dos métricas para los sponsors (el gestor y dirección):

- **Principal: el día del mes en que sale la última factura.** Valor de partida sintético: entre el día 6 y el 11. El valor real se mide en el cierre de octubre.
- **Secundaria: euros perdidos por decisiones de capacidad tomadas sin datos.** Externos no previstos, margen perdido, facturación aplazada.
- **Vigilado:** la sobrecarga de empleados (que no empeore y que se detecte antes).

## Restricciones

- Cualquier solución debe partir de los datos que ya se registran en Bizmeo, o integrarse con ellos. No lo sustituye.
- Presupuesto y recursos limitados: empresa de 15 personas, sin equipo de desarrollo propio.
- Se quiere evitar un SaaS (decisión del 2026-09-30, `corrections.md`).

## Creencias

Referenciadas del registro de `product/overview.md`:

- (1) [product] [value] El tiempo de cruce manual es lo bastante grande como para que automatizarlo se note. *Con este reencuadre es la hipótesis rival de la nueva creencia; las mismas mediciones resuelven las dos.*
- (2) [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre los dos directores provoca la sobrecarga.
- (4) [product] [viability] La dirección mantendrá el patrocinio si ve una reducción medible y una previsión.
- (5) [product] [viability] Cruzar solo dedicaciones con clientes no bastará para una previsión fiable.

Nueva (propuesta para el registro):

- [opportunity: facturacion-prevision-capacidad] [value] En los 2 próximos cierres reales, al menos el 60 % del tiempo de cierre de Carlos y David se va en averiguar hechos no registrados (cancelaciones, aplazamientos, ausencias, acuerdos, horas sin imputar), no en cruzar datos. Falso si el cruce mecánico supera el 50 %.

## Agenda de investigación

| Creencia | Instrumento más barato | Decisión que desbloquea | Para cuándo |
|---|---|---|---|
| Nueva [opportunity] [value] hechos no registrados, y (1) como rival | Las 2 entrevistas reales con la guía `interview-guides/2026-09-24-1201-tiempo-cierre-facturacion.md`, más un registro por pasos del cierre de octubre (paso, minutos, qué se esperaba) | Si gana el cruce: A1 tal como está. Si ganan los hechos: A1 se redefine (capturar hechos, no solo cruzar) y A3 sube | Cierre de octubre (1-6 nov.), antes de `/clarify-idea` |
| (2) descoordinación entre directores | Entrevista con los dos directores, más el piloto de A3 `fuente-unica-asignaciones` | Priorizar A3 frente a A1 | Noviembre |
| (4) patrocinio de dirección | Entrevista breve con Elena: qué día de última factura y qué previsión le bastan | Fija el umbral de éxito de la métrica principal | Antes de `/write-spec` |
| (5) variables de la previsión | Ya apoyada (secondary). En las entrevistas reales, confirmar qué hechos faltan más a menudo | Qué datos captura primero cualquier solución | Con las entrevistas reales |

## Candidate ideas (not evaluated)

En el framing original no surgió ninguna. Las alternativas ya se evaluaron en [2026-09-30-1202-facturacion-prevision-capacidad.md](../solutions/2026-09-30-1202-facturacion-prevision-capacidad.md):

- `dedicagest-a-medida` — chosen (en prueba en paralelo). *Con el reencuadre, su creencia de valor (11) depende de que el cruce mecánico sea grande, que es justo lo que se pone en duda; revisar tras el cierre de octubre.*
- `fuente-unica-asignaciones` — chosen (en prueba en paralelo)
- `bizmeo-en-origen` — chosen (en prueba en paralelo)
- `saas-psa` — discarded (se quiere evitar un SaaS)
- `plantilla-cierre` — discarded (motivo no indicado)
