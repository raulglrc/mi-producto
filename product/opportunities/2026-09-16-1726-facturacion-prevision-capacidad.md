---
status: framed
segment: Gestión operativa y administrativa de una consultora/academia de 15 personas (consultores y formadores)
personas: david-sole, carlos-roldan, elvira-ametller, elena-puig
---

# Opportunity: Facturación manual y falta de previsión de capacidad/facturación

El gestor operativo y el socio-gerente de administración dedican varios días cada mes a cruzar a mano Bizmeo, tarifas y asignaciones para poder facturar — y no tienen ninguna vista de capacidad o facturación futura, así que toman decisiones (contratar, aceptar un cliente nuevo) sin datos, y sobrecargan a empleados con formaciones y servicios sin darse cuenta.

## Segmento y personas

- **David Solé** (gestor de operaciones) — sufre directo: asigna sin visión clara de capacidad futura.
- **Carlos Roldán** (socio-gerente) — sufre directo: factura a mano cada mes, varios días perdidos.
- **Elvira Ametller** (formadora junior) — sufre la consecuencia: acaba sobrecargada sin que nadie lo detecte a tiempo.
- **Elena Puig** (directora) — sufre indirecto: decide contrataciones/pricing sin datos fiables.
- **Ramón Ferrer** — no sufre este problema; de hecho preferiría que se siguiera resolviendo "a mano".

No se detecta ninguna persona que falte para este segmento.

## Señales

| Señal | Provenance | Source |
|---|---|---|
| Carlos dedica cerca de tres días al mes a cruzar Bizmeo con tarifas para facturar | synthetic | `product/personas/carlos-roldan.md` |
| David pierde 3-4 horas/semana cruzando su Excel con Bizmeo | synthetic | `product/personas/david-sole.md` |
| Elvira no tiene ninguna vista de su carga frente a la de sus compañeros | synthetic | `product/personas/elvira-ametller.md` |
| Hay sobrecarga real de empleados por falta de datos/coordinación compartida entre el director de consultoría y el director de formación | unverified | Raul (stakeholder), conversación |
| Resolver la facturación ahorraría aproximadamente 1 jornada al mes al responsable financiero | unverified | Raul (stakeholder), conversación |

## Resultado de negocio

Producto interno — mueve la métrica de los sponsors (el propio gestor y dirección) en tres frentes:
- Tiempo administrativo ahorrado (horas/días al mes que Carlos y David dejan de perder).
- Reducción de sobrecarga/riesgo de fuga de empleados por asignaciones descoordinadas.
- Visión estratégica fiable para que Elena decida contrataciones, tarifas y foco de clientes.

## Restricciones

- Cualquier solución debe partir de/integrarse con los datos que ya se registran en Bizmeo — no lo sustituye.
- Presupuesto y recursos limitados: empresa de 15 personas, sin equipo de desarrollo propio.

## Creencias

- [product] [value] El tiempo que el gestor dedica hoy a cruzar manualmente dedicaciones (Bizmeo), clientes y cursos para facturar y prever capacidad es lo bastante grande (varias horas/semana) como para que automatizarlo sea una mejora que el gestor note y valore de inmediato.
- [product] [viability] La dirección mantendrá el patrocinio del proyecto si ve, en un plazo razonable, una reducción medible del tiempo dedicado a facturación y una previsión de facturación a corto/medio/largo plazo que hoy no tienen.
- [opportunity: facturacion-prevision-capacidad] [value] La falta de datos compartidos entre el director de consultoría y el director de formación es lo que hoy provoca que se sobrecargue a empleados con formaciones y servicios sin que nadie lo detecte a tiempo.

## Agenda de investigación

| Creencia                                                              | Instrumento                                                                                                                                 | Decisión que desbloquea                                                                                      | Para cuándo                                                    |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------- |
| [product] [value] tiempo perdido facturando a mano                    | Revisar los últimos 2-3 cierres de facturación con Carlos y David para medir el tiempo real invertido (dato ya existente / interview breve) | Confirma si el ahorro de tiempo justifica construir la herramienta frente a un arreglo más ligero            | Antes de escribir la spec                                      |
| [product] [viability] dirección mantiene el patrocinio                | `/design-interview` breve con Elena/dirección para fijar el umbral concreto (cuánta reducción de tiempo / qué previsión necesitan ver)      | Fija el criterio de éxito que dirección exigirá                                                              | Antes de la spec                                               |
| [opportunity] falta de coordinación entre directores causa sobrecarga | `/design-interview` con el director de consultoría y el de formación para verificar casos concretos de sobrecarga por descoordinación       | Confirma si la causa raíz es realmente la falta de datos compartidos (y no otra cosa, ej. exceso de demanda) | Antes de priorizar esta oportunidad frente a la de facturación |

## Candidate ideas (not evaluated)

Ninguna surgida durante este framing — el input original describía el área de la oportunidad, no una solución concreta.
