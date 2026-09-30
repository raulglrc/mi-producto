---
opportunity: facturacion-prevision-capacidad
status: testing-several
chosen: dedicagest-a-medida, fuente-unica-asignaciones, bizmeo-en-origen
---

# Soluciones para: facturación manual y falta de previsión de capacidad y facturación

## Qué dice ahora la evidencia

- La creencia de valor de la oportunidad no tiene anotación `contradicted`. **Toda la evidencia es `synthetic`, `secondary` o `unverified`**: todavía no hay entrevistas reales con Carlos ni con David.
- **Creencia 1 (tiempo del cruce):** sin verificar, con señales sintéticas contrarias. Carlos (sintético) sitúa 1,5-2 días del cierre en cruzar tarifas (`insights/2026-09-24-1343-carlos-roldan-cierre-facturacion.md`). En cambio, en 10 entrevistas de ensayo el cruce es corto y el tiempo se va en perseguir información (`insights/2026-09-30-1154-ensayo-entrevistas-cierre-capacidad.md`, synthetic).
- **Creencia 5 (hacen falta más variables):** muy apoyada. 8 fuentes secundarias coinciden en tarifas, ausencias y cartera ponderada por probabilidad (`research/2026-09-16-1801-mercado-capacity-billing-forecast.md`), y las entrevistas sintéticas apuntan a lo mismo.
- **Creencia 3 (dejar el Excel):** `weakened` (synthetic).
- **Creencia 2 de la oportunidad (descoordinación entre directores):** abierta. Solo hay un caso sintético; la encuesta de ensayo no cuenta como evidencia.
- **Creencia 6 (construir o comprar):** ningún SaaS se integra con Bizmeo (secondary). No se sabe si Bizmeo expone una API.

## Situación de partida: qué se hace hoy

`synthetic`, a verificar en las entrevistas reales de la guía `interview-guides/2026-09-24-1201-tiempo-cierre-facturacion.md`:

- **Carlos:** exporta Bizmeo y lo cruza en su Excel de tarifas. Renombra a mano los proyectos escritos en texto libre (una mañana al mes) y lleva las dudas pendientes en un pósit. Monta la previsión trimestral de noche, en unas 3 horas, con una tarifa media «de cabeza».
- **David:** cada lunes concilia su Excel de asignaciones con Bizmeo (3-4 h, según la persona sintética). Contesta sobre disponibilidad mirando solo lo planificado.
- **Sobrecarga:** se detecta tarde o nunca (unverified, conversación con Raul).

## Alternativas

### A1. DedicaGest a medida (`dedicagest-a-medida`)
Mecanismo: **automatizar**. Una herramienta propia que lee las dedicaciones de Bizmeo y las cruza con tarifas por cliente y asignaciones. Da una previsión de capacidad y facturación que incluye ausencias y cartera. Ataca el cierre y la previsión. Para Carlos (primaria) y David (secundaria), con Elena (terciaria) como destinataria de la previsión. Sustituye al Excel de cruce, al pósit y a la previsión nocturna.

### A3. Fuente única de asignaciones y ausencias, con regla de consulta (`fuente-unica-asignaciones`)
Mecanismo: **cambiar la regla**, sin software nuevo. Un único calendario compartido de asignaciones y ausencias (calendario de Outlook o Teams compartido, o el módulo de planificación de Bizmeo), que mantienen el director de consultoría, la directora de formación y David. Se aplica la regla «no se asigna sin mirarla». Ataca la sobrecarga y la respuesta sobre capacidad. Para Elvira (secundaria, la sufre) y David (secundaria). Sustituye a los Excel y calendarios separados de cada director.

### A4. Arreglar el dato en origen, dentro de Bizmeo (`bizmeo-en-origen`)
Mecanismo: **cambiar la herramienta que ya usan**. Catálogo cerrado de clientes y proyectos (nada de texto libre), recordatorio de registro semanal y fecha de corte antes del cierre. Ataca el renombrado y parte de la persecución de horas. Para Carlos (primaria). Sustituye la mañana mensual de renombrado. Es el «arreglo ligero» que la guía de entrevista quería descartar o confirmar.

## Comparación

| Alternativa | Deseable | Factible | Viable | Creencia más arriesgada |
|---|---|---|---|---|
| A1 `dedicagest-a-medida` | `mixed`: ataca el cruce y la previsión, pero las señales sintéticas dicen que el cruce en sí es corto (synthetic, `insights/2026-09-30-1154…`, `insights/2026-09-24-1343…`) | `weak` por restricción del brief (sin equipo de desarrollo propio) · lectura de Bizmeo `to check with tech` (secondary, `research/2026-09-16-1801…`) | `mixed`: mueve las dos métricas de los sponsors (tiempo y previsión), pero el coste de construcción y mantenimiento es `unknown` | Se puede construir **y mantener** sin equipo de desarrollo, y el trabajo mecánico que automatiza suma ≥1 jornada al mes |
| A3 `fuente-unica-asignaciones` | `unknown`: depende de la creencia 2, que está abierta (unverified; un caso synthetic en `insights/2026-09-30-1154…`) | `strong`: no hay que construir nada; calendario compartido o módulo de Bizmeo ya disponibles (brief) | `mixed`: ataca sobrecarga y fuga, no el tiempo de facturación (brief) | Los dos directores consultan y actualizan la fuente **antes** de asignar (el caso synthetic de Irene dice que no: el módulo murió porque no metían nada) |
| A4 `bizmeo-en-origen` | `mixed`: quita la mañana de renombrado (synthetic, `insights/2026-09-24-1343…`); el registro tardío «es cultura» (synthetic, 3 de 10, `insights/2026-09-30-1154…`) | `to check with tech`: ¿permite Bizmeo un catálogo cerrado y recordatorios? Cumple la restricción «no sustituye Bizmeo» (brief) | `weak`: ahorra ~medio día al mes y no da previsión, que es lo que espera dirección (creencia 4, unverified) | Con catálogo cerrado, el renombrado del cierre baja de una mañana a <30 min |

## Decisión

**Decide:** Raul, 2026-09-30. **Probar en paralelo A1, A3 y A4.**

**Recomendación de la IA (difiere):** probar en paralelo A4 y A2 (SaaS de planificación alimentado con Bizmeo, en periodo de prueba gratuito), con A1 y A3 aparcadas. Razones:

- A2 resolvía construir o comprar (creencia 6) antes de gastar en A1.
- A1 tenía factibilidad `weak` por falta de equipo de desarrollo.
- A3 dependía de la creencia 2, que está abierta.

**Motivo de la diferencia:** se quiere evitar un SaaS. Queda registrado en `corrections.md`.

**Consecuencia:** la creencia 6 se decide por preferencia, no por evidencia. La comparación de costes con un SaaS (900-2.400 €/año, secondary) queda sin rebatir, así que la prueba de A1 tiene que medir también el coste de mantenimiento.

**Pruebas y qué resuelve cada una:**

| Alternativa | Prueba | Resuelve | Cuándo |
|---|---|---|---|
| A4 | Configurar el catálogo cerrado en Bizmeo antes del cierre de octubre y medir el tiempo de renombrado frente a la mañana declarada | `[feature: bizmeo-en-origen]` value + feasibility; parte de la creencia 1 | Cierre de octubre (1-6 nov.) |
| A3 | Piloto de 4 semanas: calendario único y regla de consulta. Se cuentan las asignaciones nuevas que pasan por él y los choques descubiertos después | `[feature: fuente-unica-asignaciones]` value; aporta a la creencia 2 junto a la entrevista con los directores | Octubre-noviembre |
| A1 | (a) Sesión técnica: qué exporta Bizmeo, si hay API, con qué identificadores, y quién mantendría la herramienta y con cuántas horas al mes. (b) Las 2 entrevistas reales con Carlos y David para medir el trabajo mecánico del cierre | `[feature: dedicagest-a-medida]` feasibility + value; creencia 1 | Antes de `/write-spec` |

Las tres pruebas se refuerzan entre sí: A4 limpia el dato que A1 leería, y A3 crea la fuente de asignaciones y ausencias que la previsión de A1 necesita (creencia 5). Si A3 o A4 resuelven la mayor parte del dolor, A1 se reduce o se aparca.

## Propuesta de valor: A1 `dedicagest-a-medida`

- **Dolor que alivia:** los días de cierre cruzando Bizmeo con tarifas, y una previsión que se monta de noche con datos malos (synthetic, `insights/2026-09-24-1343…`).
- **Beneficio que crea:** Carlos cierra en horas, no en días. Puede contestar «¿cómo cerramos el trimestre?» con una cifra que incluye ausencias y cursos firmados.
- **Sustituye:** el Excel de cruce, el pósit de pendientes y la previsión nocturna. Por qué cambiaría: el Excel no avisa durante el mes, y los errores se descubren en el cierre.
- **Deliberadamente no hace:** no sustituye a Bizmeo como herramienta de registro, no emite facturas (eso sigue en el ERP) y no prevé la cartera comercial con probabilidades hasta que exista esa fuente.

## Propuesta de valor: A3 `fuente-unica-asignaciones`

- **Dolor que alivia:** encargos de los dos directores que coinciden sin que nadie lo sepa, y sobrecarga que se detecta tarde (unverified, stakeholder; un caso synthetic).
- **Beneficio que crea:** David contesta «¿hay alguien libre?» mirando un solo sitio, que incluye las ausencias. Elvira deja de enterarse del choque cuando ya lo tiene encima.
- **Sustituye:** los ficheros y calendarios separados de cada director. Por qué cambiarían: evita reorganizar a última hora y pagar externos.
- **Deliberadamente no hace:** no calcula horas ni facturación, no automatiza nada y no controla las asignaciones que el cliente hace directamente al consultor.

## Propuesta de valor: A4 `bizmeo-en-origen`

- **Dolor que alivia:** la mañana mensual de renombrar proyectos escritos a mano, y los errores que ese renombrado arrastra (synthetic, `insights/2026-09-24-1343…`).
- **Beneficio que crea:** una exportación de Bizmeo que se cruza sin limpiar, que es la base que necesitan A1 o cualquier otra solución.
- **Sustituye:** el renombrado manual. Por qué cambiaría: cuesta cero y no añade herramientas.
- **Deliberadamente no hace:** no intenta arreglar la puntualidad del registro con reglas más duras (la evidencia sintética dice que es cultura), no da previsión y no cambia el cruce con tarifas.

## Creencias

De la oportunidad (referenciadas tal como están registradas):

- [product] [value] El tiempo que el gestor dedica hoy a cruzar manualmente dedicaciones (Bizmeo), clientes y cursos para facturar y prever capacidad es lo bastante grande (varias horas/semana) como para que automatizarlo sea una mejora que el gestor note y valore de inmediato.
- [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre el director de consultoría y el director de formación es lo que hoy provoca que se sobrecargue a empleados con formaciones y servicios sin que nadie lo detecte a tiempo.
- [product] [viability] Construir DedicaGest a medida es mejor opción que adoptar o adaptar una herramienta comercial ya existente […] (creencia 6: decidida por preferencia, ver «Decisión»).

Propuestas para el registro (solo las que resuelven las pruebas):

- [feature: bizmeo-en-origen] [feasibility] Bizmeo permite configurar un catálogo cerrado de clientes y proyectos que impide imputar con texto libre. Falso si solo admite texto libre o si el catálogo no aparece en la exportación.
- [feature: bizmeo-en-origen] [value] Con el catálogo cerrado, el renombrado del cierre de octubre baja de una mañana a menos de 30 minutos. Falso si sigue por encima de 2 horas.
- [feature: fuente-unica-asignaciones] [value] En un piloto de 4 semanas, al menos el 80 % de las asignaciones nuevas de los dos directores pasan por la fuente única antes de asignarse, y los choques descubiertos después bajan a 0-1. Falso si menos del 50 % pasan por ella.
- [feature: dedicagest-a-medida] [feasibility] La exportación o la API de Bizmeo permiten leer dedicaciones por persona, cliente y proyecto de forma automática y estable, y hay una persona (interna o externa) que puede mantener la herramienta con 8 h al mes o menos. Falso si la lectura exige una exportación manual con un formato que cambia, o si nadie puede mantenerla.
- [feature: dedicagest-a-medida] [value] En los 2 próximos cierres reales, el trabajo mecánico que la herramienta automatizaría (cruce con tarifas, renombrado, preparación de la previsión) suma al menos 1 jornada al mes entre Carlos y David. Falso si suma menos.

## Descartadas o aparcadas

- **A2 `saas-psa`** (SaaS de planificación de recursos, como Runn, Resource Guru o Ganttic, alimentado con la exportación de Bizmeo): **descartada**. Decisión de producto: se quiere evitar un SaaS. Era la recomendación de la IA para resolver construir o comprar. Volvería si la sesión técnica de A1 concluye que nadie puede mantener una herramienta a medida.
- **A5 `plantilla-cierre`** (plantilla de cierre en Excel con Power Query, reglas por cliente, lista de pendientes y pestaña de previsión): **descartada** por decisión de Raul antes de evaluarla. El motivo no se indicó. Volvería si A1 resultara inviable y A4 no bastara.
