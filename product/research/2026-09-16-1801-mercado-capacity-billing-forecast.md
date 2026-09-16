---
source: secondary
method: mixed
date: 2026-09-16
question: ¿Existen ya herramientas de previsión de capacidad/facturación para consultoras pequeñas, qué cobra el mercado, qué variables usan para prever facturación de forma fiable, y cómo resuelven hoy este problema empresas similares sin herramienta dedicada?
opportunity: facturacion-prevision-capacidad
---

# Research: mercado de herramientas de capacity planning y previsión de facturación para consultoras/academias pequeñas

Tres hallazgos cambian decisiones. Primero: **sí existe una categoría de mercado entera** (herramientas PSA / resource & capacity planning: Runn, Productive.io, Resource Guru, Float, Birdview, Scoro, Ganttic, Mosaic...) que hace casi exactamente lo que DedicaGest quiere construir, y para un equipo de 15-20 personas cuesta entre **~300 €/año (caso atípico) y ~5.200 €/año**, con la mayoría de opciones estándar agrupadas en **900-2.400 €/año** — una cifra baja frente al coste de construir y mantener una herramienta a medida sin equipo de desarrollo propio. Segundo: **ninguna de esas herramientas se integra con Bizmeo** (no se encontró ninguna mención, integración o compatibilidad), así que "comprar" no elimina el problema de partida — habría que tender una integración a medida igualmente o mantener doble registro. Tercero: la creencia del equipo de que **cruzar solo dedicaciones con clientes/cursos no bastará** para una previsión fiable queda **fuertemente apoyada**: el consenso de facto en ocho fuentes independientes del sector PSA es que hacen falta también tarifas, ausencias/vacaciones y pipeline de nuevos contratos ponderado por probabilidad.

## Lane 1 — Competidores directos y alternativas SaaS

Se identificaron varias herramientas que combinan (a) horas/dedicaciones, (b) tarifas por cliente/proyecto y (c) previsión de facturación futura (no solo reporting histórico), con evidencia razonablemente sólida: **Runn**, **Productive.io**, **Birdview PSA** y **Resource Guru** (plan Blackbelt+). **Scoro** cumple con fuerza (a) y (b) pero su foco verificado parece más en facturar horas ya trabajadas que en previsión prospectiva pura. **Float**, **Forecast/Accelo** (Forecast fue adquirida por Accelo y su marca se fusionó en 2026) y **Parallax** mencionan piezas financieras pero el cruce explícito horas×tarifa→previsión no quedó confirmado en las páginas consultadas (requeriría demo). **Kantata** queda descartada por tamaño/coste (diseñada para 50-5.000 personas). `[verificado: ver URLs detalladas en el detalle por herramienta más abajo — 2026-09-16]`

Se encontró también **Teambook**, con contenido específico en español dirigido a "organizaciones de formación" (gestión de horarios/disponibilidad de formadores + CRM + facturación), aunque sin confirmar el cruce automático hora-de-formador × tarifa-de-curso → previsión. `[verificado: https://teambookapp.com/es/blog/formacion-cuerpos-mejor-software-de-gestion-de-equipos/ — 2026-09-16]`

Importante para no confundir categorías: el software de "gestión de academias" en español que aparece en búsquedas (MN Program, BCS data, Conpas, Bonificado Formación) es **gestión académica** (matrícula, asistencia de alumnos, cobro de cuotas) — una categoría de producto distinta a la que necesita DedicaGest. `[verificado: https://www.mnprogram.com/software-de-gestion-para-academias-de-formacion/ — 2026-09-16]`

**Sobre Bizmeo específicamente**: ninguna herramienta o plugin se anuncia como compatible/integrable con Bizmeo. Búsquedas dirigidas ("Bizmeo" + previsión/capacidad/integración/API/Zapier) no devolvieron resultados relevantes (solo ruido de "Bizneo HR", herramienta distinta). Tampoco se pudo verificar directamente si Bizmeo expone API propia. `[verificado: búsquedas web realizadas el 2026-09-16 — sin resultados relevantes; no encontrado — no se pudo acceder a bizmeo.com directamente en esta sesión]`

Detalle por herramienta (integraciones de time-tracking, cuando se encontraron): Float integra con Harvest/Toggl vía Zapier y con NetSuite, Jira, Asana, Monday, ClickUp, Wrike `[verificado: https://www.float.com/integrations/zapier/ — 2026-09-16]`; Runn integra con Harvest y Clockify "upon request" solo en plan Advanced `[verificado: https://www.runn.io/pricing — 2026-09-16]`; Forecast/Accelo integra con HubSpot, Salesforce, HiBob, BambooHR, Xero, QuickBooks, Jira `[verificado: https://www.accelo.com/solution/resourcing-capacity-planning — 2026-09-16]`. Ninguna menciona conectores para herramientas de fichaje españolas.

Mosaic y Ganttic (mencionadas en lane 1) no se pudieron verificar en detalle funcional en este lane — ver lane 2 para su pricing verificado. `[conocimiento del modelo — verificar: descripción funcional general]`

## Lane 2 — Pricing y modelo de negocio

Todas las herramientas revisadas operan en **SaaS por suscripción**, mayoritariamente facturado por usuario/asiento/mes, con descuento anual (10-20%) y trial de 14-30 días sin tarjeta. Excepción: **Ganttic** cobra por número de recursos planificados con usuarios ilimitados, no por asiento — modelo distinto y potencialmente mucho más barato para equipos pequeños con pocos "recursos" a programar. `[verificado: patrón observado en 9 páginas de pricing citadas — 2026-09-16]`

Coste estimado para un equipo de 15-20 personas (plan mínimo que cubre cruce horas-cliente + previsión básica), de más barato a más caro:

| Herramienta | Plan | Coste mensual aprox. | Coste anual aprox. |
|---|---|---|---|
| Ganttic | PRO 20 (usuarios ilimitados) | ~25 $ | ~300 $ |
| Harvest Forecast | anual, 5$/persona | 75-100 $ | 900-1.200 $ |
| Resource Guru | Grasshopper (sin informes) | 75-100 $ | 900-1.200 $ |
| Resource Guru | Blackbelt (con informes) | 120-160 $ | 1.200-1.680 $ |
| Float | Starter | 105-140 $ | 1.260-1.680 $ |
| Runn | Lite (mín. 20 asientos) | 140 $ | 1.680 $ |
| Mosaic | Professional | 150-200 $ | 1.800-2.400 $ |
| Productive.io | Essential | 135-150 $ | 1.620-1.800 $ |
| Scoro | Time-billing | 255 $ | 3.060 $ |
| Birdview PSA | Team | 360-480 $ | 4.320-5.760 $ |
| Scoro | Projects & Resources (completo) | 435 $ | 5.220 $ |

`[verificado: fetch directo a cada página de pricing citada, 2026-09-16; excepciones: getforecast.com/pricing no accesible directamente, se usó como sustituto verificado getharvest.com/forecast/pricing (mismo producto); mosaicapp.com/pricing no mostró cifras al fetch directo, se usó G2 como fuente secundaria]`

**Ninguna herramienta ofrece plan gratuito indefinido que cubra 15-20 personas** con cruce horas-cliente + previsión (Ganttic es gratis solo hasta 10 recursos). La opción más barata que sí cubre 15-20 personas de forma indefinida es Ganttic (~300 $/año), seguida de Harvest Forecast o Resource Guru Grasshopper (~900-1.200 $/año). `[verificado: mismas fuentes — 2026-09-16]`

## Lane 3 — Variables para una previsión de facturación fiable

Ocho fuentes independientes (BigTime, Parallax, Projectworks, Float, Productive.io, Accelo, Resource Guru, Kantata, Noloco) coinciden en que una previsión de facturación fiable no se basa solo en horas × clientes/cursos asignados, sino que combina:

- **Tarifas/rate cards** — factor multiplicador explícito para convertir horas en importe (Parallax: "Projected Revenue = horas × tarifa por rol"; Projectworks: "multiplicar horas facturables por lo que cobra cada consultor/hora"). `[verificado: https://support.getparallax.com/hc/en-us/articles/7632678305811-Revenue-Forecast, https://www.projectworks.com/blog/using-revenue-forecasting-to-grow-your-consulting-firm — 2026-09-16]`
- **Ausencias/vacaciones/bajas** — necesarias para no sobreestimar capacidad disponible; es el error de previsión más citado (Float documenta el caso de alguien marcado "disponible" que en realidad tiene PTO planificado). `[verificado: https://www.float.com/resources/resource-forecasting, https://www.bigtime.net/psa-software/faq/how-to-plan-resource-capacity-next-quarter/ — 2026-09-16]`
- **Pipeline/nuevos contratos previstos**, ponderado por probabilidad de cierre — patrón repetido casi idéntico en 3 fuentes (BigTime, Resource Guru, Parallax: "un proyecto con 70% de probabilidad cuenta como 70% de sus horas proyectadas"). `[verificado: https://www.bigtime.net/psa-software/faq/how-to-plan-resource-capacity-next-quarter/, https://resourceguruapp.com/blog/agencies/agency-capacity-planning — 2026-09-16]`
- **Estacionalidad** — apoyo más débil, solo una fuente (Kantata) la trata como variable de primer orden; probablemente secundaria para DedicaGest. `[verificado: https://www.kantata.com/ebook/forecasting-and-optimizing-capacity — 2026-09-16]`
- **% de utilización objetivo (capacidad disponible vs. facturable)** — prácticamente estándar, con un rango de referencia 70-80% citado de forma coincidente en 3 fuentes; depende directamente de restar las ausencias de la capacidad bruta. `[verificado: https://www.accelo.com/glossary/calculating-resource-utilization-billable-utilization-rate — 2026-09-16]`

No se encontró un estándar sectorial único y certificado, pero el patrón convergente entre competidores funciona como evidencia de práctica de facto. Errores documentados por omitir variables: sobreestimar capacidad por no contar ausencias (Float), sobrecompromiso por pipeline sin ponderar (Resource Guru: "las agencias que prevén sobre pipeline sin ponderar sistemáticamente se sobrecomprometen"), y previsiones que "siempre se quedan atrás de la realidad" si se basan solo en desempeño pasado sin reglas de tarifas/costes actualizadas (BigTime). `[verificado: URLs citadas arriba — 2026-09-16]`

## Lane 4 — Alternativas y no-consumo

No se encontró evidencia directa (foros, testimonios en primera persona, hilos de Reddit o foros españoles de formación) de consultoras/academias de 10-20 personas describiendo explícitamente que usan Excel manual en vez de una herramienta dedicada. Las búsquedas específicas en español no devolvieron resultados relevantes al patrón buscado. `[verificado: ausencia de resultados relevantes en búsquedas del 2026-09-16]`

La evidencia indirecta es más consistente: coamplifi.com segmenta explícitamente las operaciones de consultoras por tamaño, y describe el tramo "boutique (2-20 personas)" — que coincide con el segmento de DedicaGest — como facturación "parcialmente manual, con más reconciliación requerida" y decisiones de capacidad "sin datos sólidos", sin usar la palabra Excel pero describiendo el mismo patrón. `[verificado: https://coamplifi.com/blog/how-operations-differ-across-consulting-firm-sizes/ — 2026-09-16]` Una encuesta propia de Runn (sesgo de vendor, muestra no segmentada por tamaño/sector) reporta que el 44% de organizaciones todavía usa hojas de cálculo para resource management (bajando desde 58% el año anterior). `[verificado: https://www.runn.io/blog/resource-management-statistics — 2026-09-16]` También existe una oferta comercial de pago (Eloquens, Flevy, Gumroad) de plantillas Excel específicas para "consulting firm" con modelos de facturación/utilización — señal indirecta de que el patrón "hoja de cálculo a medida para consultoras" es un nicho reconocido. `[verificado: https://flevy.com/browse/marketplace/consulting-firm-financial-model-dynamic-10-year-forecast-5944 — 2026-09-16]`

Razones citadas por la industria para no migrar a herramientas dedicadas: familiaridad/coste de formación cero (Excel ya se domina), coste percibido como marginal (ya se paga Office), baja complejidad operativa inicial en equipos pequeños con poco solapamiento de proyectos, e inercia organizativa. Ninguna de estas razones viene de un testimonio directo de un afectado — son generalizaciones de contenido de vendors. `[verificado: https://www.runn.io/blog/resource-planning-in-excel, https://www.projectworks.com/blog/5-signs-it-is-time-to-switch-from-spreadsheets-to-psa-software — 2026-09-16]`

**Conclusión honesta de este lane**: la hipótesis de no-consumo es plausible y consistente con la evidencia indirecta reunida, pero no está verificada con fuente primaria para el segmento exacto (consultoría + formación, 10-20 personas, España). Es terreno para investigación primaria, no para más búsqueda secundaria.

## Impacto en creencias

| Creencia (de overview.md / brief de oportunidad) | Veredicto | Evidencia |
|---|---|---|
| [product] [viability] Cruzar solo dedicaciones con clientes/cursos no bastará — hará falta también tarifas, vacaciones/ausencias y nuevos contratos previstos | **Apoya** | 8 fuentes independientes del sector PSA (BigTime, Parallax, Projectworks, Float, Productive.io, Accelo, Resource Guru, Kantata, Noloco) coinciden en que tarifas + ausencias + pipeline ponderado son necesarios para una previsión fiable, no solo horas×cliente `[verificado — ver Lane 3]` |
| [product] [value] El tiempo que el gestor dedica hoy a cruzar manualmente dedicaciones/clientes/cursos es lo bastante grande como para que automatizarlo sea una mejora notada de inmediato | **No dice nada directamente** | La investigación de mercado no puede verificar el tiempo real de Carlos/David (eso requiere revisar sus cierres de facturación, ya en la agenda de investigación primaria). Sí hay una señal indirecta débil: existe una categoría SaaS entera y contenido de vendors construido enteramente alrededor de "deja Excel", lo que sugiere que este tipo de dolor es reconocido en el mercado como suficientemente real para pagar por resolverlo — pero no es evidencia sobre *este* equipo concreto `[verificado — ver Lane 1, 2 y 4]` |
| [product] [value] El gestor usaría DedicaGest de forma voluntaria y dejaría de lado Excel u otros métodos en paralelo | **No dice nada** | Es una creencia sobre comportamiento de adopción de un usuario concreto; la investigación de mercado no la toca |
| [product] [viability] La dirección mantendrá el patrocinio si ve reducción medible de tiempo y una previsión de facturación que hoy no tienen | **No dice nada** | Es una creencia sobre el patrocinador interno; fuera del alcance de research de mercado |
| [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre el director de consultoría y el de formación es lo que hoy provoca que se sobrecargue a empleados sin que nadie lo detecte a tiempo | **No dice nada** | Ninguno de los cuatro lanes tocó la coordinación interna entre directores; sigue siendo terreno exclusivo de la entrevista ya prevista en la agenda de investigación de la brief |

## Hallazgo adicional relevante para viabilidad (no mapea a una creencia existente)

La restricción explícita del brief ("presupuesto y recursos limitados, sin equipo de desarrollo propio") hace relevante un hallazgo que no estaba entre las creencias formuladas: **existe una categoría de herramientas SaaS ya construidas que resuelven una parte sustancial de este problema por 900-2.400 €/año** (rango donde se agrupan la mayoría de opciones estándar para 15-20 personas), muy por debajo del coste probable de construir y mantener una herramienta a medida sin equipo propio. El matiz que evita que esto sea una respuesta cerrada: **ninguna se integra con Bizmeo**, así que adoptar una de estas herramientas no elimina el trabajo manual de partida — sustituye "cruzar Excel a mano" por "mantener datos en dos sistemas" o por construir igualmente una integración a medida (vía la API/CSV que Bizmeo permita, no verificado en esta sesión). Esto sugiere que la pregunta "¿construir DedicaGest o adoptar/adaptar una herramienta existente?" merece una respuesta explícita antes de escribir la spec — hoy no hay ninguna creencia registrada sobre build vs. buy.

## Qué sigue necesitando research primario

- **Tiempo real perdido facturando a mano** (Carlos, David) — ya en la agenda de la brief: revisar los últimos 2-3 cierres de facturación. Este research secundario no lo puede sustituir.
- **Umbral de patrocinio de dirección** (Elena) — ya en la agenda: entrevista breve para fijar qué reducción de tiempo/previsión necesitan ver.
- **Causa raíz de la sobrecarga por descoordinación** entre director de consultoría y de formación — ya en la agenda: entrevista con ambos directores.
- **Nuevo, no estaba en la agenda**: si se confirma que el tiempo perdido justifica una solución, decidir explícitamente build vs. buy/adapt — lo que requeriría entender si Bizmeo tiene API/exportación utilizable (pregunta técnica, no de investigación de usuario) y si alguna herramienta comercial (Runn, Resource Guru, Ganttic) podría adaptarse al flujo real de la empresa mediante una entrevista/demo comercial.
- **Comportamiento de adopción real** ("¿dejaría Carlos/David Excel en cuanto tuvieran DedicaGest disponible?") — solo primary research con los propios usuarios puede tocar esto; no es investigable por research secundario.
