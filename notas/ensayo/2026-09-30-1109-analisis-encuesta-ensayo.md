---
source: survey
survey_design: product/surveys/2026-09-23-0200-carga-asignaciones-registro.md
results: notas/ensayo/respuestas_encuesta.csv
n: 30 (27 completas, 3 parciales)
status: BORRADOR — datos de ensayo, no evidencia real (ver «Denominador»)
---

# Análisis de encuesta: carga de trabajo, asignaciones y registro en Bizmeo

## Denominador y límites (leer primero)

| | Diseño | Export |
|---|---|---|
| Plantilla / alcance | 15 personas, 1 canal (Teams), enlace único | 30 respuestas, 1 canal |
| Bloque A (imparten) | objetivo 10 de 11-12 | 23 (20 completas) |
| Bloque B (asignan) | 2-3 personas | 6 (3 solo asignan + 3 imparten y asignan) |
| Solo admin/dirección | — | 4 |
| Ventana | 05-10 revisión, cierre 09-10 | respuestas del 01-10 al 09-10-2026 |

**Tres señales de que este CSV no es el resultado real de la encuesta:**

1. **30 respuestas de una plantilla de 15** (200 % de tasa de respuesta), con 6 personas en el bloque B cuando asignan 2-3. Con encuesta anónima y enlace único no hay forma de detectar duplicados.
2. **Fechas posteriores a hoy** (30-09-2026): todas las respuestas están fechadas entre el 1 y el 9 de octubre.
3. Contactos en `@example.com` y la carpeta se llama `ensayo`.

Por tanto este análisis vale como **ensayo del pipeline de análisis** (qué cortes hacer, qué preguntas funcionan, cómo se codifica Q12), no como evidencia. Todo lo que sigue se lee así. Aunque los datos fueran reales: canal único y propio, n muy por debajo de 30 → patrones y recuentos, nunca porcentajes; y no se puede cortar por canal.

## Objetivo 1 — Cuánta sobrecarga hay

**Creíamos:** hay sobrecarga frecuente y no se detecta a tiempo.

**Los datos (bloque A, 23 personas; «No lo sé» y vacíos aparte):**

- Q1 semanas con más horas de las previstas: ninguna 3 · 1-2 sem. 6 · 3-5 sem. 6 · 6-9 sem. 3 · 10+ 3 · no lo sé 2.
  → **6 personas con sobrecarga casi continua (≥6 de 12 semanas)**; el resto, puntual o nada.
- Q6 última vez con más carga (17 que la tuvieron): se reorganizó 7 · lo comentó y no cambió nada 6 · no lo comentó 4.
  → **10 de 17 casos no se corrigieron**, y en 4 nadie se enteró.

**Decisión que sugeriría:** la sobrecarga no es general, está concentrada en un grupo pequeño — justo ahí debe mirar la previsión de capacidad. Merece ir junto a facturación, no detrás.

## Objetivo 2 — Cómo llegan las asignaciones

**Creíamos (creencia 2):** la falta de datos compartidos entre director de consultoría y de formación provoca la sobrecarga.

**Corte clave — quién asigna (Q3) × sobrecarga:**

| Recibe encargos de… | n | Q1 ≥6 semanas | Q4 ≥2 choques | Q6: se reorganizó |
|---|---|---|---|---|
| **Ambos directores** | 6 | **6 de 6** | **6 de 6** | 0 de 5 |
| Cliente directo (sin ambos directores) | 4 | 0 (todos 3-5 sem.) | 0 | 1 de 4 |
| Un solo director / gestor / otro | 13 | 0 | 0 | 6 de 8 |

- Q4 choques con encargos de otro: ninguno 10 · 1 vez 4 · 2-3 veces 4 · 4+ 2 · no lo sé 2 — todos los ≥2 están en el grupo «ambos directores».
- Q5 antelación: <2 días 7 · 2-7 días 6 · 1-2 sem. 5 · 2-4 sem. 3 · >4 sem. 1. Los que se enteran con <2 días son sobre todo los de cliente directo.
- Bloque B (6): 3 de 6 han asignado y descubierto después encargos que no conocían (Q10); para comprobar la carga, 5 de 6 **preguntan a la persona**, 3 miran **su propia hoja**, 2 miran Bizmeo y **solo 1 pregunta al otro director** (Q11).

**Lectura:** el patrón apoya con fuerza la creencia 2 para quienes reciben de los dos directores. **Pero aparece una segunda vía que la creencia no contempla:** el cliente que asigna directamente al consultor (4-6 personas, sobrecarga moderada, se entera con <2 días, lo absorbe sin avisar). Ningún dato compartido entre directores lo habría detectado.

**Decisión que sugeriría:** la vista compartida entre directores es el núcleo, pero la previsión tiene que capturar también los encargos que entran por el cliente.

## Objetivo 3 — Calidad del registro en Bizmeo

**Creíamos:** los datos de Bizmeo quizá no basten como base para prever.

- Q7 cuándo registra (21): mismo día 4 · cada 2-3 días 5 · fin de semana 5 · **fin de mes o cuando se lo piden 6 · no registra 1**.
- Q8 correcciones en el último mes: ninguna 10 · 1 vez 5 · 2-3 veces 4 · 4+ 2.
- Q9 registro paralelo (20): **13 de 20** llevan uno (hoja de cálculo 6, agenda/notas 6, otro 1).
- **Cruce clave:** de los 5 con sobrecarga continua que respondieron, los 5 registran a fin de mes o nunca y los 5 han tenido ≥2 correcciones en el último mes (son 5 de los 7 que registran tarde). **Bizmeo está peor justo donde hay sobrecarga:** una previsión alimentada solo de Bizmeo infraestimaría la carga de las personas más cargadas.

**Decisión que sugeriría:** antes de prever sobre Bizmeo, resolver la puntualidad del registro (o capturar asignaciones planificadas, no solo horas registradas). Es condición previa, no un detalle.

## Q12 abierta — temas (17 respuestas con texto, 15 con contenido codificable; una respuesta puede tocar varios temas)

| Tema | Menciones | Cita |
|---|---|---|
| Descoordinación entre quienes asignan | 4 | «uno me lo pasó formación y otro consultoría, y ninguno sabía del otro» (R001) |
| Bizmeo no refleja la carga real | 4 | «Bizmeo no está al día así que acabo preguntando igualmente» (R021) |
| El cliente asigna directamente y se acepta sin mirar | 3 | «Los clientes me escriben a mí directamente y acepto sin mirar mucho» (R018) |
| Aviso tardío / se absorbe en silencio | 3 | «Lo dije tarde, la verdad, porque pensé que llegaba» (R011) |
| Se resolvió sin más / se exagera | 3 | «Creo que se exagera un poco, cuando alguien va justo se habla y se mueve algo» (R007, asigna) |
| Coste en facturación | 2 | «Estuve una tarde entera cruzando su excel con lo que había en el sistema» (R016, admin) |
| Picos estacionales (sept./enero) | 2 | «más un problema de picos puntuales (septiembre y enero)» (R026) |

Nota: las dos voces que minimizan el problema (R007, R026) son de personas que asignan — quien asigna ve menos sobrecarga que quien la recibe.

## Insights priorizados

1. **[Alto] La sobrecarga se concentra en quien recibe encargos de los dos directores** (6 de 6 con ≥6 semanas sobrecargadas y ≥2 choques; 0 de 17 del resto). Apoya la creencia 2 y define el segmento prioritario. *Por qué pendiente:* ¿por qué nadie consulta al otro director antes de asignar (1 de 6)?
2. **[Alto] Bizmeo es menos fiable justo en las personas sobrecargadas** (los 5 que respondieron registran a fin de mes o nunca). Una previsión solo con dedicaciones registradas nace ciega donde más importa → refuerza creencia 5. *Por qué pendiente:* ¿registran tarde porque van cargados, o es un hábito previo?
3. **[Medio] Hay una segunda vía de sobrecarga: el cliente directo** (4-6 personas, aviso <2 días, se absorbe sin decirlo). La creencia 2 no la cubre. *Por qué pendiente:* ¿cuántos encargos directos de cliente acaban registrados como asignación?
4. **[Medio] Comunicar no basta: 10 de 17 sobrecargas no se corrigieron** (6 lo dijeron y no cambió nada). *Por qué pendiente:* ¿qué falta para reorganizar — datos, autoridad, alternativas?
5. **[Bajo] Quien asigna percibe menos problema que quien recibe** (las dos respuestas que lo minimizan son de asignadores). Cuidado con validar la solución solo con los directores.

## Cantera para entrevistas (R1 = sí y R2 = sí)

Contradicen o matizan la creencia 2 — **entrevistar primero**:

- **R018 (Iván, por Teams)** — sobrecarga por cliente directo, sin choques entre directores.
- **R009 (lucia.ferrer@)** — cliente amplía horas de un día para otro; nadie se entera.
- **R015 (sin contacto)** — sobrecarga leve, se resolvió; sin datos de contacto, no localizable.

Confirman la creencia 2:

- R001 (Marta Llorente), R004 (Jorge Pascual — también asigna), R011 (Andrés Molina), R022 (Carla Soto).

Otras perspectivas:

- R021 (Tomás Rey) — asigna; Bizmeo no está al día.
- R016 (Elena Castro) — administración; coste en facturación (relevante para creencia 1).

## Contraste con las creencias del overview (solo si los datos fueran reales)

- **Creencia 2** [opportunity] — prometedora, con el matiz del cliente directo. No `confirmed` (muestra pequeña y autoseleccionada).
- **Creencia 5** [product][viability] — reforzada en su condición previa: el dato de partida de Bizmeo no es fiable donde hay sobrecarga.
- **Creencia 1** — la encuesta no mide el tiempo del gestor; solo una cita anecdótica (R016).
