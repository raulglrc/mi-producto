# DedicaGest_AFPM

mode: new · internal

Gestor de dedicaciones y previsor de budget y proyectos para una empresa pequeña de consultoría y formación (15 trabajadores). Toma como base las dedicaciones que los empleados ya registran en Bizmeo y añade la capa que hoy falta: previsión de capacidad y facturación a corto, medio y largo plazo, cruzando esas dedicaciones con los cursos y clientes asignados a cada persona.

## Para quién

El gestor de equipo de una consultora/academia pequeña (15 consultores y formadores) que hoy necesita saber, por persona y por cliente, cuántas jornadas se invierten en cada cliente — para facturar y para prever capacidad y facturación a corto/medio/largo plazo. Los empleados registran sus dedicaciones en Bizmeo, pero esa herramienta no da la vista de previsión ni cruza capacidades con clientes/cursos asignados.

## Sponsor

Dos patrocinadores: el propio gestor y la dirección de la empresa. Ambos necesitan ver que se reduce el tiempo manual invertido en facturación (hoy consume mucho tiempo automatizable) y que aparece una previsión de facturación a corto/medio/largo plazo que hoy no existe — lo que además aporta una capa de visión estratégica a dirección.

## Creencias no verificadas

1. [product] [value] El tiempo que el gestor dedica hoy a cruzar manualmente dedicaciones (Bizmeo), clientes y cursos para facturar y prever capacidad es lo bastante grande (varias horas/semana) como para que automatizarlo sea una mejora que el gestor note y valore de inmediato.
2. [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre el director de consultoría y el director de formación es lo que hoy provoca que se sobrecargue a empleados con formaciones y servicios sin que nadie lo detecte a tiempo.
3. [product] [value] El gestor usaría DedicaGest de forma voluntaria y dejaría de lado sus métodos actuales (Excel u otros) en cuanto lo tuviera disponible, en vez de mantenerlos en paralelo "por si acaso".
   — weakened by [2026-09-24-1343-carlos-roldan-cierre-facturacion.md](insights/2026-09-24-1343-carlos-roldan-cierre-facturacion.md) (2026-09-24)
4. [product] [viability] La dirección mantendrá el patrocinio del proyecto si ve, en un plazo razonable, una reducción medible del tiempo dedicado a facturación y una previsión de facturación a corto/medio/largo plazo que hoy no tienen.
5. [product] [viability] Cruzar solo dedicaciones con clientes/cursos asignados no bastará para una previsión de facturación fiable — probablemente hará falta incorporar también tarifas, vacaciones/ausencias y nuevos contratos previstos.
6. [product] [viability] Construir DedicaGest a medida es mejor opción que adoptar o adaptar una herramienta comercial ya existente (tipo Runn, Resource Guru, Productive.io) para cubrir la previsión de capacidad y facturación, dado el presupuesto limitado y la falta de equipo de desarrollo propio.
7. [feature: bizmeo-en-origen] [feasibility] Bizmeo permite configurar un catálogo cerrado de clientes y proyectos que impide imputar con texto libre. Falso si solo admite texto libre o si el catálogo no aparece en la exportación.
8. [feature: bizmeo-en-origen] [value] Con el catálogo cerrado, el renombrado del cierre de octubre baja de una mañana a menos de 30 minutos. Falso si sigue por encima de 2 horas.
9. [feature: fuente-unica-asignaciones] [value] En un piloto de 4 semanas, al menos el 80 % de las asignaciones nuevas de los dos directores pasan por la fuente única antes de asignarse, y los choques descubiertos después bajan a 0-1. Falso si menos del 50 % pasan por ella.
10. [feature: dedicagest-a-medida] [feasibility] La exportación o la API de Bizmeo permiten leer dedicaciones por persona, cliente y proyecto de forma automática y estable, y hay una persona (interna o externa) que puede mantener la herramienta con 8 h al mes o menos. Falso si la lectura exige una exportación manual con un formato que cambia, o si nadie puede mantenerla.
11. [feature: dedicagest-a-medida] [value] En los 2 próximos cierres reales, el trabajo mecánico que la herramienta automatizaría (cruce con tarifas, renombrado, preparación de la previsión) suma al menos 1 jornada al mes entre Carlos y David. Falso si suma menos.
12. [opportunity: facturacion-prevision-capacidad] [value] En los 2 próximos cierres reales, al menos el 60 % del tiempo de cierre de Carlos y David se va en averiguar hechos no registrados (cancelaciones, aplazamientos, ausencias, acuerdos, horas sin imputar), no en cruzar datos. Falso si el cruce mecánico supera el 50 %.
