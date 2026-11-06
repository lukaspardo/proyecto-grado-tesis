# Cronograma de ejecución investigativa — Issue #19

Fecha de revisión: 2026-11-05. Responsable de consolidación: Santiago (shibito9). Preparación asistida por Codex, para revisión humana.

**Estado: ENTREGADO_PENDIENTE_REVISION. Propuesta de 16 semanas, sin aprobación del tutor ni fecha de inicio confirmada.** No modifica el documento maestro ni los originales institucionales. No registra ejecución, resultados o cumplimiento de los objetivos.

## 1. Auditoría, procedencia y alcance del aporte

Se consultaron el cuerpo y los comentarios disponibles de los Issues [#10](https://github.com/lukaspardo/proyecto-grado-tesis/issues/10), [#17](https://github.com/lukaspardo/proyecto-grado-tesis/issues/17), [#18](https://github.com/lukaspardo/proyecto-grado-tesis/issues/18) y [#19](https://github.com/lukaspardo/proyecto-grado-tesis/issues/19) el 2026-11-05 mediante GitHub CLI. Son requisitos y aportes internos, no fuentes académicas ni aprobaciones del tutor.

### Estado de Git observado

- Rama inicial: `santiago/consolidacion-propuesta-issues-16-17`, commit `83e3929`. Índice sin cambios preparados.
- Tras `git fetch origin`, `main` y `origin/main` apuntaban a `4e2bf61ed3d698a45b3807fc421e0e01d8716935`, que incluye la metodología del #17 y la consolidación de la propuesta mediante los PR #22 y #23. Se utiliza esa base para evitar omitir la metodología ya integrada al repositorio; integración no implica aprobación académica.
- Ramas locales disponibles: `main`, `deivy/issue-11-deuda-tecnica`, `santiago/auditoria-proyecto`, `santiago/consolidacion-propuesta-issues-16-17`, `santiago/issue-10-alcance-definitivo` y `santiago/issue-17-metodologia`. Las referencias remotas incluyen además `karmadevz/comparativa-y-fundamentacion` y `karmadevz/docs/alineacion`. La rama de auditoría local estaba seis commits por delante de su referencia remota; no se alteró.
- La rama solicitada `santiago/issue-19-cronograma` no existía localmente ni entre las referencias remotas recuperadas; se crea desde `origin/main` para este aporte.
- Cambios preexistentes preservados: eliminación local de `material_profesor/Revision_Asesor_Analisis_Predictivo_Deuda_Tecnica. 1docx.docx`; archivos sin seguimiento `material_profesor/Revision_Analisis_Predictivo_Deuda_Tecnica. 1docx.docx` y `docs/aportes/deuda_tecnica/Fundamentación Académica de Deuda Técnica.pdf`. No se restauran, renombran, incluyen ni atribuyen esos cambios.

### Insumos y dependencias metodológicas

Rutas relativas a la raíz del repositorio. Se revisó texto; no se certifica maquetación del DOCX ni imágenes incrustadas. No se modificaron ni convirtieron originales.

| Dependencia / insumo | Evidencia consultada y estado observado | Consecuencia para el cronograma |
|---|---|---|
| #10 — alcance | `alcance_definitivo.md`, en esta misma carpeta; Issue cerrado, con comentario que mantiene pendiente la validación del profesor | No asumir eliminación aprobada de predicción, prototipo o dashboard. Plazo y alcance siguen sujetos al tutor. |
| #17 — metodología | `metodologia_reconstruida.md`, §§2, 5–9; Issue cerrado; comentario presenta borrador y PR #22, sin aprobación del tutor | Conservar tres objetivos, ocho fases, separación de herramientas y validación humana. Su aprobación metodológica permanece PENDIENTE. |
| #18 — evaluación | Issue abierto; [comentario de lukaspardo del 2026-11-04 UTC](https://github.com/lukaspardo/proyecto-grado-tesis/issues/18#issuecomment-6620853358) y [adjunto completo](https://github.com/user-attachments/files/34348538/protocolo.de.evaluacion.y.validacion.md), leído directamente, sin copiarlo al repositorio | Aporte entregado para revisión, no protocolo aceptado. Establece dimensiones, dos condiciones de consulta, evidencia y revisión humana; aún falta operacionalizar instrumentos, escalas, reglas de decisión/desacuerdo, revisores, muestra, repeticiones y reintentos. Resolver antes de corridas evaluables. |
| #19 — cronograma | Issue abierto, asignado a shibito9, sin comentarios en la consulta | Resolver ocho semanas frente a cuatro meses mediante una propuesta explícita de 16 semanas; no declarar cambio institucional aprobado. |
| Propuesta consolidada | `docs/propuesta/Propuesta_Proyecto_Integrador_actualizada_issues_16_17.docx`, texto de duración y cronograma | Conserva «8 semanas» en el campo de duración. Este aporte no corrige ese campo: propone su futura conciliación autorizada. |
| Maestro y antecedentes | `docs/documento_maestro.md`; `auditoria/inventario_aportes.md`; `auditoria/estado_centralizacion_2026-10-25.md` | Maestro aún mantiene definiciones pendientes. Los antecedentes orientan procedencia y reparto propuesto, no aceptación ni compromisos personales. |

Fortalezas de la propuesta: correspondencia explícita entre fases, objetivos y productos; controles antes de ejecutar; documentación y validación distribuidas. Limitaciones: alcance, disponibilidad, recursos y protocolo sin confirmar. Solapamientos: #17 define procedimiento y #18 evaluación; aquí solo se programan, sin sustituirlos. Contradicciones: ocho semanas del DOCX frente a 16 propuestas; condiciones opcionales del #17 frente a dos condiciones contempladas en el adjunto #18. Ambas requieren decisión registrada, no elección silenciosa.

Trazabilidad: #19 → este aporte → insumos anteriores → secciones potenciales de duración y cronograma de la propuesta, y §8 Metodología / §9 Prueba piloto del maestro, solo bajo autorización futura. No se crea un identificador AP ni fichas RAE: estas corresponden a las fuentes bibliográficas de F1, cuyos vínculos se mantienen PENDIENTES hasta verificarlos. Este cronograma es planificación propia, no evidencia académica. Aceptación de Santiago y tutor: PENDIENTE. Commit de integración al maestro: PENDIENTE; el commit de este aporte no equivale a esa integración.

## 2. Dos horizontes distintos

**Entrega de la propuesta académica:** prevista para finales de noviembre de 2026 según la instrucción de Santiago para esta tarea. Día exacto, requisitos finales y confirmación institucional: PENDIENTES. Ese hito comprende una propuesta coherente de alcance, metodología, evaluación, cronograma, recursos y pendientes, revisada por el equipo; no exige presentar como ya ejecutadas las 16 semanas ni fabricar resultados. Su consolidación no se realiza en este aporte.

**Ejecución investigativa propuesta:** duración declarada en este plan de **16 semanas consecutivas, S1–S16**, a partir de una fecha de inicio que deberá acordarse y registrarse. No se fija un calendario de 2026 ni se comprimen 16 semanas hasta noviembre. No se equiparan automáticamente 16 semanas con cuatro meses calendario. Las ocho semanas del DOCX son una inconsistencia identificada, no la duración adoptada en este plan. Su sustitución en el documento institucional requiere autorización y aprobación del plazo por el tutor.

Antes de iniciar S1 se propone confirmar el alcance investigativo, las formulaciones de objetivos y la ventana de 16 semanas. Si se exige otro plazo o se mantienen entregables de producto/predicción, deberá reestimarse el plan y dejar constancia de quién decide, fecha y evidencia. Una entrega de propuesta no resuelve por sí misma esas decisiones. Si no llega una aprobación, el calendario permanece propuesta; no se declara cumplido el #19 en su dimensión institucional.

## 3. Objetivos y fases de referencia

Se transcriben los objetivos específicos de §2 del aporte #17, como **base de trabajo pendiente de validación**, sin atribuir aprobación al tutor:

- **OE1:** Caracterizar las métricas y hallazgos relevantes obtenidos mediante SonarQube, así como las capacidades y limitaciones de los modelos de lenguaje aplicados al análisis de código, con relación a la identificación y gestión de posibles manifestaciones de deuda técnica.
- **OE2:** Aplicar SonarQube y un modelo de lenguaje seleccionado sobre un caso de estudio de software previamente delimitado, utilizando un procedimiento reproducible que permita registrar y contrastar los hallazgos obtenidos por ambas herramientas.
- **OE3:** Evaluar la complementariedad entre los resultados de SonarQube y el análisis del modelo de lenguaje, considerando su utilidad para apoyar la identificación, interpretación y priorización de posibles manifestaciones de deuda técnica mediante criterios técnicos y validación humana.

| Fase del #17 | Ventana propuesta | Objetivos | Producto parcial verificable |
|---|---|---|---|
| F1. Revisión y caracterización documental | S1–S4; comprobaciones y actualización hasta S16 | OE1 | Búsquedas, fuentes y acceso documentados; caracterización; vínculos RAE existentes o PENDIENTES. |
| F2. Preparación y delimitación del caso de estudio | S3–S6 | OE2 | Ficha de caso, licencia, commit, muestra, exclusiones, entorno y protocolo versionado. |
| F3. Configuración y ejecución del análisis con SonarQube | S5–S8 | OE1, OE2 | Configuración, logs, reporte íntegro y selección trazable. |
| F4. Preparación del contexto y análisis mediante LLM | S5–S6 preparación; S7–S10 ejecución controlada | OE1, OE2 | Modelo/configuración, prompts, contexto, condiciones y respuestas originales por corrida. |
| F5. Registro y contraste de resultados | S8–S11 | OE1, OE2, OE3 | Matriz de vínculos y contraste preliminar sin dictámenes anticipados. |
| F6. Validación humana | S9–S12 | OE3 | Dictámenes, evidencia, incertidumbre y desacuerdos conservados. |
| F7. Análisis de complementariedad | S11–S14 | OE3 | Análisis sustentado, incluidos errores, redundancias y resultados inconclusos. |
| F8. Síntesis de resultados y limitaciones | S13–S16 | OE1, OE3 | Informe del caso con evaluación de los tres objetivos y anexos trazables. |

El solapamiento opera por lotes terminados: F6 valida únicamente unidades ya contrastadas en F5; F7 analiza unidades revisadas y espera el cierre del conjunto para conclusiones. Preparar plantillas desde S1 y redactar secciones parciales durante todas las fases no equivale a anticipar F8 ni resultados.

## 4. Responsables propuestos y viabilidad

Asignaciones propuestas por este aporte, **no compromisos confirmados ni designación definitiva de expertos**:

- Santiago / shibito9: coordinación, coherencia metodológica, trazabilidad y consolidación documental.
- Deivy / deyvi0297: caracterización de deuda técnica y métricas, preparación y ejecución SonarQube, con apoyo de Lukas.
- KarmaDevz: caracterización, selección y configuración del LLM, contexto y consultas, con apoyo de Santiago. Se conserva el identificador registrado sin inferir identidad civil.
- Lukas / lukaspardo: coordinación del protocolo #18, instrumentos de contraste y validación humana, con apoyo del equipo. Competencias, número y designación de revisores por confirmar; coordinar no lo convierte en referencia experta aprobada.
- Equipo: revisión cruzada de evidencias y productos. Tutor: decisiones académicas, sujeto a disponibilidad; no se le atribuyen aprobaciones ni horas comprometidas.

Como supuesto de estimación propio, se propone reservar **6 horas por persona y semana**, en cuatro roles de equipo: 24 horas-persona/semana y 384 horas-persona en 16 semanas. Por persona: 4 h para actividad principal, 1 h para registro/redacción y 1 h para revisión/coordinación. No es disponibilidad verificada ni una cifra institucional; el equipo debe contrastarla con sus cargas antes de S1. Las actividades de cada fila comparten ese presupuesto y no constituyen dedicaciones completas acumulables.

La factibilidad se limita a un caso acotado, un modelo y una muestra manejable fijada en S6, sin entrenamiento ni aplicación automática de correcciones. El tamaño y número de consultas no se inventan: se estimarán con pruebas de factibilidad separadas de la evaluación. Las dos condiciones de consulta del adjunto #18 se presupuestarán solo tras decidir su inclusión y carga; no se ejecutará una comparación distinta de la aprobada sin registrar desviación. Hardware, licencia, acceso local/nube y disponibilidad de revisores se verifican antes de congelar el protocolo. S8 y S15 dejan margen para incidencias y revisión; si resulta insuficiente, se propone ajustar muestra o plazo con aprobación, preservando evidencia y resultados desfavorables, sin omitir validación.

## 5. Plan de 16 semanas

Los responsables son líderes propuestos; todos conservan su registro semanal. Cada revisión genera observaciones, responsable y decisión fechada. Ningún entregable de la tabla existe por el solo hecho de programarlo.

| Semana | Actividad y fase | Objetivos | Responsable / apoyo propuestos | Entregable parcial y control |
|---|---|---|---|---|
| S1 | F1: preguntas de búsqueda, fuentes, criterios y contraste del alcance; abrir registro de decisiones y plantillas de evidencia | OE1 | Santiago / equipo | Plan de búsqueda y pendientes; revisión de coherencia con #10 y tutor. |
| S2 | F1: lectura crítica, deuda frente a señales de calidad y capacidades/límites LLM; revisión del adjunto #18 | OE1 | Deivy y KarmaDevz / Lukas | Registro de fuentes con nivel de acceso; lista de vacíos del protocolo, sin adoptar métricas no aprobadas. |
| S3 | F1–F2: caracterizar métricas y modelos; comparar candidatos de caso y sus licencias/compatibilidad | OE1, OE2 | Deivy y KarmaDevz / Santiago | Caracterización preliminar y ficha comparativa de casos; revisión cruzada de fuentes y exclusiones. |
| S4 | F1–F2: justificar caso, lenguaje, unidad y selección de muestra; operacionalizar evaluación #18 | OE1, OE2, OE3 | Santiago y Lukas / equipo | Ficha candidata, instrumento de evaluación propuesto y registro de observaciones; revisión con tutor según disponibilidad. |
| S5 | F2–F4: preparar entorno y probar factibilidad SonarQube/LLM; ensayar registro y revisión humana | OE1, OE2, OE3 | Deivy y KarmaDevz / Lukas | Manifiesto de versiones/recursos y pruebas marcadas como ensayo; registro de fallos y carga observada. |
| S6 | F2–F4: ajustar a recursos; fijar caso/commit, muestra, reglas, modelo, prompts y protocolo #18 | OE2, OE3 | Santiago y Lukas / Deivy y KarmaDevz | Paquete versionado y decisión de paso: condiciones, escalas, revisores, repeticiones, reintentos y desacuerdos definidos. Sin ello, no iniciar corridas evaluables. |
| S7 | F3–F4: ejecutar SonarQube y preparar paquetes de contexto; iniciar consultas aprobadas sobre unidades fijadas | OE1, OE2 | Deivy y KarmaDevz / Santiago | Reporte original, logs, entradas/salidas de primer lote; comprobar commit y ausencia/presencia de diagnóstico suministrado. |
| S8 | F3–F5: completar análisis estático, revisar cobertura y registrar contraste inicial; margen de incidencias | OE1, OE2, OE3 | Deivy y Lukas / KarmaDevz | Selección trazable y matriz inicial; fallos/reintentos registrados sin sustituir originales. |
| S9 | F4–F6: continuar consultas y contraste; validar primer lote completo conforme al protocolo congelado | OE1, OE2, OE3 | KarmaDevz y Lukas / revisores por confirmar | Respuestas y dictámenes vinculados; comprobar evidencia localizable e incertidumbre. |
| S10 | F4–F6: completar consultas planificadas; continuar contraste y revisión humana | OE1, OE2, OE3 | KarmaDevz y Lukas / Santiago | Registro de consultas completo o desviaciones; revisión de integridad y separación de condiciones. |
| S11 | F5–F7: cerrar contraste; validar lotes restantes e iniciar análisis sobre unidades ya revisadas | OE1, OE2, OE3 | Lukas / equipo | Matriz contrastada y análisis preliminar identificado; auditoría de enlaces código–salida–dictamen. |
| S12 | F6–F7: cerrar dictámenes, aplicar reglas de desacuerdo y preservar inconclusos | OE3 | Lukas / revisores por confirmar y Santiago | Registro de validación y pendientes no resueltos; revisión antes del análisis final. |
| S13 | F7–F8: analizar utilidad para identificación, interpretación y priorización; redactar resultados y limitaciones | OE1, OE3 | Santiago y Lukas / equipo | Análisis argumentado y borrador de síntesis; contraste con literatura verificada, sin asumir mejoras. |
| S14 | F7–F8: consolidar análisis, amenazas a validez y respuesta a la pregunta | OE1, OE3 | Santiago / Deivy y KarmaDevz | Informe parcial con trazabilidad por objetivo y revisión crítica de resultados negativos/inconclusos. |
| S15 | F8: revisión integral, referencias, anexos y reproducibilidad documental; margen de correcciones | OE1, OE2, OE3 | Equipo / Santiago | Lista de comprobación y correcciones trazables; cualquier nueva corrida requerirá ID, motivo y condiciones registrados. |
| S16 | F8: consolidar informe del caso, conclusiones acotadas y evidencias; revisión final para entrega | OE1, OE2, OE3 | Santiago / equipo | Informe propuesto y balance de objetivos, límites y pendientes; entrega sujeta a requisitos del tutor. |

Durante S1–S16 se actualizan bitácora, procedencia, referencias y decisiones. Las revisiones de S2–S6 son de diseño/factibilidad; la validación de resultados se realiza en S9–S12 y se verifica de nuevo en S15. La documentación no se concentra al final.

## 6. Puertas de revisión y decisiones pendientes

| Momento / decisión | Evidencia o condición requerida | Estado y acción si no se resuelve |
|---|---|---|
| Antes de S1: horizonte y alcance | Tutor confirma 16 semanas, inicio y compatibilidad con entrega de propuesta de finales de noviembre de 2026; registrar día exacto de esa entrega | PENDIENTE. Mantener este plan como propuesta y conciliar el campo de ocho semanas en intervención autorizada posterior. |
| Antes de S1: formulaciones y diseño | Confirmar título/pregunta/OE, tipo, enfoque y estudio de caso del #17 | PENDIENTE. No declarar metodología aprobada por el estado cerrado del Issue. |
| Antes de S1: predicción y «anticipar» | Resolver si se exige predicción temporal, variable, horizonte y datos históricos | PENDIENTE. Este plan no demuestra predicción; si se exige, rediseñar evaluación y reestimar duración. |
| Antes de S1: prototipo y dashboard | Resolver obligatoriedad, mínimos y relación con informe | PENDIENTE. No programar su desarrollo como aprobado ni asumir autorizada su eliminación del compromiso institucional. |
| S4–S6: piloto y caso | Confirmar obligatoriedad, extensión, repositorio, licencia, lenguaje, commit, tamaño y muestra | PENDIENTE. OE2/OE3 requieren evidencia empírica; si el piloto no se autoriza, reformular objetivos y plan, sin declararlos cumplidos bibliográficamente. |
| S5–S6: modelo y recursos | Aprobar modelo/licencia, condición de código abierto, revisión exacta, hardware, local/nube, presupuesto y parámetros | PENDIENTE. Registrar factibilidad; no iniciar corridas evaluables con configuración indeterminada. |
| S6: protocolo #18 | Aceptar instrumentos, criterios evaluables, escalas/métricas pertinentes, condiciones de consulta, muestra, repeticiones, reintentos, revisores/competencias y resolución de desacuerdos | PENDIENTE de revisión del equipo y validación académica. El adjunto es un insumo. Sin cierre, solo ensayos exploratorios identificados; reprogramar, sin puntuar evaluación final. |
| Antes de S1 y en S6: disponibilidad | Equipo confirma dedicación y revisores; tutor confirma requisitos de entregables | PENDIENTE. Ajustar carga y registrar decisión; no atribuir a personas compromisos no aceptados. |
| S12 y S15: suficiencia de evidencia | Dictámenes, discrepancias, desviaciones y relación completa de artefactos | Control futuro, no aprobación ya obtenida. Conservar insuficiencias y no generalizar fuera del caso. |

Para cada decisión se requiere responsable que aprueba, fecha y evidencia localizable. Ninguna respuesta del tutor se inventa. Las estimaciones de remediación no se tratarán como costos reales, las alertas no equivalen automáticamente a deuda y ninguna herramienta constituye verdad de referencia. Si el LLM recibe el diagnóstico SonarQube, la coincidencia no se presentará como detección independiente. La complementariedad sigue siendo hipótesis; el informe admitirá ausencia de aporte o resultados inconclusos.

## 7. Comprobación de los criterios de aceptación del #19

Evaluación documental propia de esta propuesta; no es aceptación de Santiago ni del tutor y no autoriza cerrar el Issue.

| Criterio del Issue | Evidencia en este aporte | Resultado y límite |
|---|---|---|
| Duración del cronograma coincide con duración declarada | §2 declara 16 semanas; §5 cubre S1–S16 | Cumple internamente. La duración institucional de ocho semanas sigue sin corregirse, por restricción de alcance; conciliación y aprobación del tutor PENDIENTES. |
| Cada actividad tiene relación con objetivos | §§3 y 5: fases, objetivos por fila y productos | Cumple como planificación; no afirma cumplimiento experimental de objetivos. |
| Revisión y validación durante el proceso | §§5–6: revisiones desde S1, ensayo S5, control S6, validación S9–S12, auditoría S15 | Cumple en diseño; ejecución y aceptación del #18 PENDIENTES. |
| Cronograma viable para el equipo | §4: cuatro roles, presupuesto estimado, caso acotado y controles; §5 reserva margen y solapamiento por lotes | Viabilidad condicionada, no demostrada: disponibilidad, recursos, muestra y revisores por confirmar. |

Acción siguiente: Santiago y equipo revisan este aporte, acuerdan asignaciones y presentan al tutor los pendientes, coordinados con #10, #17 y #18. Solo después de aceptación y autorización explícita podrá trasladarse a documentos institucionales o maestro. Se conserva el estado del Issue #19 y no se realizan merge ni push.
