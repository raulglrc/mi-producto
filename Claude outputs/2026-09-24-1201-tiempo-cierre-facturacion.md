---
opportunity: facturacion-prevision-capacidad
mode: exploration
beliefs:
  - "[product] [value] El tiempo que el gestor dedica hoy a cruzar manualmente dedicaciones (Bizmeo), clientes y cursos para facturar y prever capacidad es lo bastante grande (varias horas/semana) como para que automatizarlo sea una mejora que el gestor note y valore de inmediato."
  - "[product] [value] El gestor usaría DedicaGest de forma voluntaria y dejaría de lado sus métodos actuales en cuanto lo tuviera disponible (señal secundaria)."
  - "[product] [viability] Cruzar solo dedicaciones con clientes/cursos no bastará para una previsión fiable (señal secundaria)."
---

# Guía de entrevista: el tiempo real del cierre de facturación

- **Objetivos de aprendizaje:**
  1. **Cuánto tiempo cuesta de verdad** el cierre mensual (facturación) y el cruce semanal de capacidad, medido sobre los últimos 2-3 cierres reales y no sobre la impresión que tienen de ellos. → Decide si el ahorro justifica construir una herramienta o basta con un arreglo más ligero (una plantilla o una exportación mejor). Viene de la agenda de investigación del brief (fila 1: "antes de escribir la spec").
  2. **Dónde se va ese tiempo:** qué pasos, qué fuentes de datos además de Bizmeo, y qué errores y retrabajos aparecen. → Decide qué paso atacar primero y qué datos necesitaría cualquier solución.
  3. **Qué pasa hoy cuando hace falta mirar hacia delante**, y qué ocurrió la última vez que cambiaron de herramienta o de proceso. → Da la primera evidencia real sobre el valor de una previsión y sobre si el Excel acaba conviviendo con la herramienta nueva.
- **Perfil de los participantes:** las dos personas reales que hoy hacen el cruce a mano.
  - El socio-gerente responsable de administración y facturación (arquetipo: `product/personas/carlos-roldan.md`).
  - El gestor de operaciones y planificación (arquetipo: `product/personas/david-sole.md`).
  - Las personas son **arquetipos sintéticos**: la entrevista sirve para contrastarlos, no para confirmarlos.
- **Modo:** exploración
- **Duración:** 45 min por persona. Las entrevistas son **por separado**, porque según el brief sus cifras no siempre cuadran y una entrevista conjunta tendería a alinearlas.
- **Preparación:** pide a cada uno que tenga abiertos durante la entrevista los ficheros de su último cierre (la exportación de Bizmeo, el Excel de cruce o de asignaciones y las facturas emitidas). Se trabaja sobre esos ficheros, no de memoria.

## Calentamiento (5 min)

- ¿Cómo describirías tu papel en el cierre de cada mes? ¿Qué te llega, de quién, y qué entregas tú?
- ¿Desde cuándo lo haces así?

> Nota para quien entrevista: confirma que la persona participó directamente en al menos uno de los últimos 3 cierres. Si no participó en ninguno, no encaja en el perfil.

## Cuerpo principal

### Objetivo 1: cuánto tiempo cuesta (15 min)

**Pregunta de apertura:** "Vamos a repasar el cierre de agosto con los ficheros delante. Cuéntame desde el primer momento en que te pusiste con él. ¿Qué hiciste primero?"

Repreguntas:
- ¿Qué día empezaste y qué día terminaste? ¿Fue en bloques o de forma dispersa?
- ¿Cuántas horas calculas que le dedicaste ese día? ¿Hay algo (el calendario, la hora del correo, la fecha de modificación del fichero) que nos ayude a comprobarlo?
- ¿Fue un mes típico? Si no, ¿cómo fue el cierre de julio, o el anterior?
- *(Solo a David)* Fuera del cierre, ¿cuánto te llevó la semana pasada poner al día el Excel de asignaciones con lo que hay en Bizmeo?

> **Creencia en juego:** automatizar el cruce ahorraría "varias horas a la semana".
> **Qué indicaría que nos equivocamos:** que el cierre les cueste menos de una jornada al mes entre los dos y el cruce semanal de David menos de 1 hora, o que el tiempo se concentre en un solo paso que se resuelve con algo trivial. También cuenta como señal en contra que las cifras solo se sostengan de memoria y ningún fichero ni fecha las respalde.
> Anota la cifra que da cada uno y compárala con las señales del brief: "~3 días/mes" (sintético) y "~1 jornada/mes" (stakeholder).

### Objetivo 2: dónde se va el tiempo (10 min)

**Pregunta de apertura:** "De todo lo que acabas de contar, ¿en qué parte se te fue más tiempo?"

Repreguntas:
- ¿Qué datos necesitaste además de lo que registra Bizmeo? ¿De dónde salen (tarifas, cursos cerrados, ausencias, contratos nuevos)?
- ¿En qué momento no cuadraron los números? ¿Qué hiciste para cuadrarlos?
- ¿Tuviste que pedir a alguien que corrigiera o completara sus horas? ¿Cuántas veces y a quién?
- Cuéntame el último error de facturación que tuviste que corregir. ¿Cómo lo detectaste y cuánto tiempo te llevó arreglarlo?

> **Creencia en juego:** el problema es el cruce manual de datos.
> **Qué indicaría que nos equivocamos:** que el tiempo se vaya sobre todo en perseguir a la gente para que registre (un problema de disciplina de registro, no de herramienta) o en decisiones comerciales (qué se cobra y qué no) que ninguna automatización resuelve.
> Aquí también se ve qué variables usan ya hoy (tarifas, ausencias…), que es una señal para la creencia 5.

### Objetivo 3: mirar hacia delante y cambios de herramienta (10 min)

**Pregunta de apertura:** "¿Cuándo fue la última vez que alguien te preguntó cómo iba a cerrar el trimestre, o si había gente libre para un cliente nuevo? ¿Qué hiciste para contestar?"

Repreguntas:
- ¿De dónde sacaste la cifra? ¿Cuánto tardaste en tenerla?
- ¿Qué pasó después con esa respuesta? ¿Se tomó alguna decisión con ella?
- Cuéntame la última vez que cambiasteis una herramienta o un proceso de gestión (por ejemplo, cuando empezasteis con Bizmeo). ¿Qué pasó con lo que usabais antes? ¿Lo mantuviste en paralelo? ¿Durante cuánto tiempo?

> **Creencias en juego:** que una previsión aporta valor (el brief) y que el gestor dejaría sus métodos actuales (creencia 3).
> **Qué indicaría que nos equivocamos:** que las peticiones de previsión sean raras o se resuelvan bien en minutos, o que en cambios anteriores el Excel siguiera vivo durante meses "por si acaso".
> **No preguntes** "¿usarías una herramienta que…?". Solo vale lo que ya han hecho.

## Cierre (5 min)

- ¿Qué debería haberte preguntado y no te he preguntado?
- ¿Hay alguien más que toque este proceso y con quien debería hablar?
- ¿Nos pasas una copia (anonimizada si hace falta) del Excel de cruce del último cierre, para anotar los pasos?
- Gracias.

## Plan de reclutamiento

- **Canal:** contacto directo con las dos personas del perfil. La encuesta `product/surveys/2026-09-23-0200-carga-asignaciones-registro.md` **no** es la fuente aquí: su segmento es otro (quién recibe y quién asigna el trabajo), y sus opt-ins servirán para la guía de la creencia 2.
- **Filtro:**
  1. ¿Participaste directamente en al menos uno de los últimos 3 cierres de facturación o en la actualización semanal de capacidad? → Si no, **no encaja**.
  2. ¿Tienes acceso a los ficheros de esos cierres (la exportación de Bizmeo, el Excel, las facturas)? → Si no, la entrevista pierde la parte de datos. **Aplázala** hasta que los tenga.
- **Objetivo:** 2 entrevistas, una por persona, por separado. Con n=2 no se puede hablar de saturación. Lo que salga es **evidencia real de dos casos concretos**: sirve para confirmar o contradecir la creencia 1 en *esta* empresa, no para generalizar. Si hay otra persona que toque el proceso (lo sabremos por la pregunta de referidos), se añade.
