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
- **Preparación:**
  - Pide a cada uno que tenga abiertos durante la entrevista los ficheros de **los dos últimos cierres de meses con actividad normal** (no agosto; normalmente junio y julio): la exportación de Bizmeo, el Excel de cruce o de asignaciones y las facturas emitidas. Se trabaja sobre esos ficheros, no de memoria.
  - Pregunta antes si **guarda los ficheros de cada cierre o los sobrescribe**. Si los sobrescribe, que traiga lo que conserve con fecha: los correos de envío de facturas, el calendario, el historial de exportaciones de Bizmeo o las versiones anteriores del fichero.

## Calentamiento (5 min)

- ¿Qué necesitas tener en la mano para empezar el cierre de cada mes, y quién te lo da?
- ¿Desde cuándo lo haces así? ¿Cómo se hacía antes?

> Nota para quien entrevista: confirma que la persona participó directamente en al menos uno de los últimos 3 cierres. Si no participó en ninguno, no encaja en el perfil. Apunta lo que diga sobre "antes"; el objetivo 3 se apoya en ello.

## Cuerpo principal

### Objetivo 1: cuánto tiempo cuesta (15 min)

**Pregunta de apertura (según el perfil):**
- *A Carlos:* "Vamos a repasar el último cierre de un mes normal (el de julio, o el de junio si julio fue raro) con los ficheros delante. Cuéntame desde el primer momento en que te pusiste con él. ¿Qué hiciste primero?"
- *A David:* "Vamos a repasar el lunes pasado, cuando pusiste al día el Excel de asignaciones, con los ficheros delante. Cuéntame desde el primer momento en que te pusiste con ello. ¿Qué hiciste primero?"

Repreguntas:
- Vamos paso a paso: ¿qué hiciste primero y cuánto rato le dedicaste? ¿Y después? *(A Carlos, día a día hasta el día en que envió la última factura. A David, hasta que dio la hoja por cerrada, aunque se alargara a otros días.)*
- ¿Hay algo que nos ayude a comprobar esas horas: el calendario, la hora del correo o la fecha de modificación del fichero?
- ¿Y el anterior (cierre, o lunes)? ¿Se pareció a este?
- Si aparece un paso que no esperabas (una justificación, una subvención, un informe…): "Eso que acabas de mencionar, cuéntame la última vez paso a paso. ¿Cuánto tiempo te llevó?"
- Si ese rato no existiera, ¿qué harías con él? Cuéntame la última vez que algo se quedó sin hacer porque estabas con esto.
- *(Solo a David)* En el último cierre mensual, ¿qué hiciste tú y cuánto rato te llevó?

> **Creencia en juego:** automatizar el cruce ahorraría "varias horas a la semana", y el gestor lo notaría y lo valoraría.
> **Qué indicaría que nos equivocamos:** que el cierre les cueste menos de una jornada al mes entre los dos y el cruce semanal de David menos de 1 hora, o que el tiempo se concentre en un solo paso que se resuelve con algo trivial. También cuenta como señal en contra que las cifras solo se sostengan de memoria y ningún fichero ni fecha las respalde, o que ese tiempo no le quite nada que le importe.
> Anota la cifra que da cada uno y compárala con las señales del brief: "~3 días/mes" (sintético) y "~1 jornada/mes" (stakeholder). Si solo cuenta un mes atípico (agosto, diciembre), vuelve a un mes normal antes de seguir.

### Objetivo 2: dónde se va el tiempo (10 min)

**Pregunta de apertura:** "De todo lo que acabas de contar, ¿en qué parte se te fue más tiempo?"

Repreguntas:
- ¿Qué otros ficheros o fuentes abriste además de la exportación de Bizmeo? ¿De dónde salen?
- ¿En qué momento no cuadraron los números? ¿Qué hiciste para cuadrarlos?
  - Si nombra a otras personas: ¿cuánto tiempo estuviste esperando a que lo corrigieran? ¿Qué hiciste mientras tanto?
- Si aparece un paso que no esperabas: "Cuéntame la última vez paso a paso. ¿Cuánto tiempo te llevó?"
- *(Solo a Carlos)* Cuéntame la última vez que un cliente os devolvió o cuestionó una factura. ¿Qué pasó?
  *(A David no se le hace: su equivalente, comprometerse con un cliente o un curso sin tener gente, sale en el objetivo 3.)*

> **Creencia en juego:** el problema es el cruce manual de datos.
> **Qué indicaría que nos equivocamos:** que el tiempo se vaya sobre todo en perseguir a la gente para que registre o en esperar a que corrija (un problema de disciplina de registro, no de herramienta), o en decisiones comerciales (qué se cobra y qué no) que ninguna automatización resuelve.
> **Solo para quien entrevista**, después de la respuesta espontánea: comprueba si han salido tarifas, cursos cerrados, ausencias y contratos nuevos. No leas la lista en voz alta. Lo que nombre por sí solo es la señal para la creencia 5; lo que salga solo al preguntarle, anótalo aparte.

### Objetivo 3: mirar hacia delante y cambios de herramienta (10 min)

**Pregunta de apertura (según el perfil):**
- *A Carlos:* "¿Cuándo fue la última vez que alguien (los socios, el banco) te preguntó cómo iba a cerrar el trimestre? ¿Qué hiciste para contestar?"
- *A David:* "¿Cuándo fue la última vez que alguien te preguntó si había gente libre para un cliente o un curso nuevo? ¿Qué hiciste para contestar?"

Repreguntas:
- ¿De dónde sacaste la cifra? ¿Cuánto tardaste en tenerla?
- ¿Qué pasó después con esa respuesta? ¿Se tomó alguna decisión con ella?
- Si expresa desconfianza en la cifra: ¿qué pasó la última vez que no se cumplió?
- Antes de [la herramienta actual; ver el calentamiento] usabais [lo de antes]. ¿Cuándo fue la última vez que abriste una de esas hojas, o algo que haga lo mismo que Bizmeo? ¿Para qué?
  - Si no vivió ese cambio: "Cuéntame la última vez que empezaste a usar algo nuevo para gestionar el trabajo (una hoja, una herramienta, un proceso). ¿Qué pasó con lo que usabas antes? ¿Cuándo lo abriste por última vez?"

> **Creencias en juego:** que una previsión aporta valor (el brief) y que el gestor dejaría sus métodos actuales (creencia 3).
> **Qué indicaría que nos equivocamos:** que las peticiones de previsión sean raras o se resuelvan bien en minutos, o que tras el cambio anterior el Excel o las hojas sigan abriéndose hoy para lo mismo.
> **No preguntes** "¿usarías una herramienta que…?" ni "¿lo mantuviste en paralelo?". Solo vale lo que ya han hecho, con fecha.
> Si sale sobrecarga cruzada entre consultoría y formación (una persona asignada a la vez por las dos áreas sin que nadie lo viera), anótala para la guía de la creencia 2 y no la persigas aquí.

## Cierre (5 min)

- ¿Qué debería haberte preguntado y no te he preguntado?
- ¿Hay alguien más que toque este proceso y con quien debería hablar?
- ¿Nos pasas una copia (anonimizada si hace falta) del Excel de cruce del último cierre, para anotar los pasos?
- Gracias.

## Plan de reclutamiento

- **Canal:** contacto directo con las dos personas del perfil. La encuesta `product/surveys/2026-09-23-0200-carga-asignaciones-registro.md` **no** es la fuente aquí: su segmento es otro (quién recibe y quién asigna el trabajo), y sus opt-ins servirán para la guía de la creencia 2.
- **Filtro:**
  1. ¿Participaste directamente en al menos uno de los últimos 3 cierres de facturación o en la actualización semanal de capacidad? → Si no, **no encaja**.
  2. ¿Tienes acceso a los ficheros de esos cierres (la exportación de Bizmeo, el Excel, las facturas), o al menos a rastros con fecha (correos de envío, calendario)? → Si no, la entrevista pierde la parte de datos. **Aplázala** hasta que los tenga.
- **Objetivo:** 2 entrevistas, una por persona, por separado. Con n=2 no se puede hablar de saturación. Lo que salga es **evidencia real de dos casos concretos**: sirve para confirmar o contradecir la creencia 1 en *esta* empresa, no para generalizar. Si hay otra persona que toque el proceso (lo sabremos por la pregunta de referidos), se añade.

## Pretest notes

### 2026-09-24: ensayo con `product/personas/carlos-roldan.md` (sintético)

Es control de calidad de la guía, no evidencia. Lo que dijo el arquetipo no se usa como hallazgo.

**Qué cambió:**
- **Mes de referencia:** de "agosto" a "el último cierre de un mes normal". Agosto es un mes atípico, y el mes representativo se acababa contando de memoria.
- **Preparación y filtro:** ahora se pregunta si guarda los ficheros de cada cierre o los sobrescribe, y se aceptan rastros con fecha como alternativa. La exportación sobrescrita dejaba el objetivo 1 sin respaldo.
- **Objetivo 1:** la pregunta de fechas y la de horas (que era doble y ambigua con "ese día") pasan a ser un recorrido día a día. Se añaden una repregunta general para pasos inesperados y la pregunta "¿qué dejaste de hacer?", que cubre la parte de la creencia 1 de que el gestor lo note y lo valore.
- **Objetivo 2:** la lista de ejemplos (tarifas, cursos…) sale de la pregunta y queda como nota para quien entrevista. Dirigía la respuesta y contaminaba la creencia 5. La repregunta de "pedir a alguien que corrija" se fusiona con la anterior y ahora mide el tiempo de espera. "Último error de facturación" pasa a "última vez que un cliente cuestionó una factura", al final del bloque.
- **Objetivo 3:** la apertura se separa por perfil (trimestre para Carlos, capacidad para David), y se añade una repregunta para cuando desconfía de la cifra. "¿Lo mantuviste en paralelo?" pasa a "¿cuándo abriste por última vez…?", apoyándose en el calentamiento en vez de repetirlo.
- **Calentamiento:** la pregunta triple pasa a "qué necesitas y quién te lo da", para captar el traspaso entre los dos participantes.

**Qué se dejó igual a propósito:**
- La duración y el reparto de tiempos: con los cambios, el recorrido cabe en 45 min.
- El plan de reclutamiento: la pregunta de referidos ya permite añadir a una tercera persona.
- Las preguntas de cierre: funcionaron.

### 2026-09-24: segunda pasada con `product/personas/david-sole.md` (sintético)

Sirve para comprobar los cambios de la primera pasada con el otro perfil. Es control de calidad de la guía, no evidencia.

**Qué funcionó de la primera ronda:** sin la lista de ejemplos, David nombró sus fuentes por sí solo; la repregunta sobre la espera sacó el tiempo real de espera; y la apertura del objetivo 3 separada por perfil dio un episodio concreto con consecuencias.

**Qué cambió:**
- **Objetivo 1:** la apertura depende del perfil. Para David, el punto de partida es la actualización del lunes pasado, porque su coste es semanal y el cierre mensual solo le lleva una mañana. Antes, su coste de verdad era una única pregunta al final y sin repreguntas. El cierre mensual de David pasa a ser una repregunta.
- **Objetivo 1:** "Esos días, ¿qué dejaste de hacer?" pasa a "¿qué harías con ese rato?… la última vez que algo se quedó sin hacer". La versión anterior daba "nada" cuando el coste está integrado en la rutina. La introdujo la primera pasada.
- **Objetivo 2:** la pregunta de la factura cuestionada queda "Solo a Carlos".
- **Objetivo 3:** alternativa para quien no vivió el cambio de herramienta. Sin ella, la creencia 3 se quedaba sin evidencia con David. La introdujo la primera pasada.
- **Objetivo 3:** nota para desviar la sobrecarga cruzada entre áreas a la guía de la creencia 2.

**Qué se dejó igual a propósito:**
- El plan de reclutamiento: los referidos de David apuntan al director de formación (que lleva el calendario de cursos), y el plan ya permite añadirlo.
- Las repreguntas del objetivo 2, que funcionaron con los dos perfiles.
