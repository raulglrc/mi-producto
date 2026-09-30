# Insights: cierre de facturación y capacidad (10 entrevistas de ensayo)

- **Fuentes** (todas `source: synthetic`, modo exploración, guía `product/interview-guides/2026-09-24-1201-tiempo-cierre-facturacion.md`):
  - Perfil administración / facturación: `notas/ensayo/2026-10-01-carmen-aguirre.md`, `2026-10-05-mercedes-villalba.md`, `2026-10-06-ana-lucia-restrepo.md`, `2026-10-08-gustavo-herrera.md`, `2026-10-13-tomas-beltran.md`, `2026-10-14-nuria-salcedo.md`
  - Perfil operaciones / planificación: `notas/ensayo/2026-10-02-rodrigo-pizarro.md`, `2026-10-06-javier-montesinos.md`, `2026-10-07-pau-ferrer.md`, `2026-10-09-irene-castano.md`
- **source:** synthetic
- **Fecha:** 2026-09-30

> Son hipótesis que hay que contrastar con usuarios reales. No son evidencia. Además, son 10 empresas externas; DedicaGest es una herramienta interna, así que lo que decide son las entrevistas reales con las dos personas que hacen hoy el cruce (arquetipos `carlos-roldan` y `david-sole`). Este corpus sirve para afinar qué preguntarles y qué patrones buscar.

## Tiempos declarados y comprobados con ficheros

| Persona | Cierre mensual / puesta al día semanal | De eso, el cruce en sí |
|---|---|---|
| Carmen (admin.) | 2,5 días julio · 1,5 junio | la mañana del viernes (~5 h) |
| Nuria (admin.) | 2,5-3 días julio · 2 junio | «una hora» |
| Gustavo (admin.) | «3 días»; con los XML, ~2 | no lo separa |
| Ana Lucía (admin.) | 1,5 días (mitad, reuniones con socios) | 3 h |
| Mercedes (admin.) | «la semana», fragmentada | 2-3 h |
| Tomás (admin.) | 2 h (igualas, sin horas) | — |
| Rodrigo (ops.) | 3,5-4 h cada lunes | 5 min (macro) |
| Irene (ops.) | 2 h y pico cada lunes | 5 min |
| Javier (ops.) | dice 30 min; el fichero, 9:12-11:40 | — |
| Pau (ops.) | 40 min (Power BI) | 0 (automático) |

## 1. El cruce es corto; el tiempo se va en perseguir lo que no está en ningún fichero

**Recurrente: 9 de 10.** Donde se mide, cruzar Bizmeo con tarifas o con el plan cuesta entre 5 minutos y media jornada al mes. El resto del cierre —de 1,5 a 3 días en los perfiles de facturación por horas— se va en averiguar qué pasó de verdad: cursos aplazados o cancelados, bajas, acuerdos por WhatsApp, firmas que faltan, órdenes de compra. Tres personas corrigieron al entrevistador cuando dio por hecho que el problema era el cruce. Para el producto: automatizar el cruce ahorra poco. Lo que ahorra días es que esos hechos (cancelación, aplazamiento, baja, acuerdo con el cliente) se registren cuando pasan y los vea quien factura y quien planifica.

> Evidencia: «Si por cruce entiendes pegar Bizmeo con tarifas, eso es lo de menos, una hora. Lo que me come es saber qué ha pasado de verdad con cada curso […] está en la cabeza de Rocío.» — Nuria · «Pegar Bizmeo son cinco minutos. Lo que me lleva es que me cuenten las cosas.» — Irene · «Juntar horas es fácil.» — Ana Lucía

## 2. Las respuestas rápidas sobre capacidad se dan con datos incompletos y cuestan dinero

**Recurrente: 4 de 4 en operaciones, más 4 previsiones fallidas en administración.** Cuando dirección pregunta «¿hay gente libre?», se contesta en 10-20 minutos mirando solo lo planificado. Lo que falta son las ausencias (no están en Bizmeo: RR. HH. no las comparte), los encargos que otro director tiene en su propio fichero y la cartera comercial. Costes citados: 380.000 CLP de margen perdido en un curso (Rodrigo), unos 2.000 € de un formador externo (Irene), dos semanas de facturación perdidas (Pau), una previsión que se quedó un 18 % por debajo (Nuria). Pau, el único con las horas automatizadas, lo resume: el dato de horas está bien, el que no vale es el de lo que va a entrar. Para el producto: una previsión útil necesita ausencias, encargos de todos los que asignan y cartera con una probabilidad corregida. Sin eso, una previsión hecha solo con dedicaciones da falsa seguridad.

> Evidencia: «uno de los dos tenía vacaciones aprobadas que nadie me había avisado. […] Se fue casi todo el margen del curso.» — Rodrigo · «Marisa ya la tenía en octubre en Portugal con Rui, y eso estaba en el Word de Marisa, que yo no había mirado.» — Irene · «el 60 % es mentira, porque solo tiene lo que ya está firmado.» — Pau

## 3. El registro tardío bloquea facturas concretas, y lo ven como un problema de cultura

**Recurrente: 7 de 10.** Consultores en planta o en campo, vacaciones y formadores externos que no tienen acceso a Bizmeo (Nuria tiene 8, en papel) retrasan facturas entre 2 y 8 días; el caso más claro, 6.300 € que salieron el 12 en vez del 4 (Carmen). Todos facturan primero lo que está completo y dejan aparcado lo que falta. Rodrigo pidió dos veces por correo que se registrara a diario y no funcionó, y tres personas dicen que ninguna herramienta lo arregla. Para el producto: no prometer que arregla la puntualidad. Sí puede ver qué clientes están completos y se pueden facturar ya, quién bloquea qué factura y por cuánto dinero, y ofrecer una entrada sencilla para externos. Coincide con la encuesta de ensayo: quienes más carga tienen son quienes registran más tarde.

> Evidencia: «Si todo el mundo registrara el mismo día, yo cerraría en un día. Y eso no te lo arregla ningún programa, es cultura.» — Carmen · «Los relatores en terreno muchas veces no tienen señal, están en una faena a 3.000 metros.» — Rodrigo

## 4. Qué se factura y a qué precio son decisiones por cliente que no están escritas

**Recurrente: 5 de 6 en administración** (y coincide con el insight 5 de Carlos). Bolsas de horas, tarifas escalonadas por alumno, descuentos pactados en 2020, subidas por inflación, horas «de regalo» a un cliente estratégico, cancelaciones a medias: cada caso se resuelve buscando el contrato o reuniéndose con los socios, y la decisión no queda guardada. Ana Lucía tuvo 5 clientes con horas «raras» en julio y una hora de reunión solo por uno de ellos (15 sesiones hechas, 12 contratadas, se cobraron 13). Para el producto: reglas de facturación por cliente (bolsa, tarifa, qué cuenta como facturable) y un registro de decisiones que sirva al mes siguiente. Ahí está el trabajo de criterio que hoy se repite cada mes.

> Evidencia: «Quizás cómo decidimos qué es facturable. Porque yo creo que ahí está el problema de verdad, no en juntar horas.» — Ana Lucía · «hay dos clientes antiguos con una tarifa pactada entonces que nunca pasé bien a la hoja nueva […] Lo abro todos los meses.» — Carmen

## 5. Una herramienta nueva sobrevive si el dato le llega solo; si depende de que otros lo metan, se vuelve al Excel

**Recurrente: 3 casos de cambio de herramienta, y 6 de 10 con una herramienta antigua que sigue viva.** Irene compró el módulo de planificación de Bizmeo, lo llevó dos meses en paralelo con el Excel y lo dejó porque los directores no metían nada. Javier mantuvo Trello y Excel a la vez dos meses y se quedó con el Excel, porque Trello no suma horas. Pau dejó Harvest y el Excel antiguo del todo porque Power BI lee Bizmeo cada noche sin que nadie haga nada. Las herramientas antiguas que siguen vivas (la hoja «control horas 2020», la bitácora de 2015, la pizarra, los partes en papel) cubren siempre un hueco concreto que la herramienta nueva no cubre: kilometraje, tarifas antiguas, ausencias visibles para todos. Para el producto: no hay que depender de que los directores metan datos a mano, y hay que cubrir esos huecos concretos o convivir con ellos.

> Evidencia: «Y como los directores no metían nada en Bizmeo, pues al final solo el Excel.» — Irene · «Harvest lo cancelamos en junio de 2024 y no lo he vuelto a abrir.» — Pau

## Nota de segmento

4 de 10 no tienen el problema tal como está planteado: Tomás cobra una cuota fija (igualas), Javier justifica por acción formativa, Pau ya lo tiene automatizado y a Mercedes lo que le duele es cobrar con inflación. El problema aparece cuando se factura por horas y más de una persona asigna trabajo. Esa combinación es la que tiene la empresa propia, y es el filtro que conviene usar para cualquier panel externo.
