# Metodología reconstruida para el Issue #17

**BORRADOR METODOLÓGICO PARA REVISIÓN DEL EQUIPO Y DEL TUTOR**  
Fecha: 2026-11-01. Responsable de consolidación: Santiago (shibito9). Preparación asistida por Codex.  
Estado del borrador: **BORRADOR_PENDIENTE_REVISION**. No constituye aceptación académica ni aprobación del tutor.

## 1. Estado, procedencia y dependencias

Este aporte responde exclusivamente al [Issue #17](https://github.com/lukaspardo/proyecto-grado-tesis/issues/17), asignado a shibito9. Propone un procedimiento investigativo reproducible; no registra experimentos ejecutados ni resultados. Base de Git revisada: `8a97b36c38083f1fffa299861f95eba14f07a691`, rama de trabajo `santiago/issue-17-metodologia`.

Se revisaron los cuerpos y todos los comentarios disponibles de los Issues #17, #10 y #16 el 2026-11-01. El #17 estaba abierto y sin comentarios. Dependencias:

- [Issue #10](https://github.com/lukaspardo/proyecto-grado-tesis/issues/10): figuraba cerrado, pero `alcance_definitivo.md` sigue siendo un borrador pendiente de validación del profesor. Su comentario del 2026-10-21 distingue integración del borrador y validación pendiente. El cierre posterior no aporta por sí mismo evidencia de aprobación.
- [Issue #16](https://github.com/lukaspardo/proyecto-grado-tesis/issues/16): abierto. El comentario de KarmaDevz del 2026-10-28 presenta recomendaciones de título, resumen, objetivos y metodología sujetas a revisión del equipo y aprobación del tutor. No se adoptan como decisiones aprobadas. Según la información proporcionada por Santiago para esta revisión, el equipo ya revisó el documento completo `revision_titulo_resumen.md`. Este confirma como propuesta las inconsistencias entre predicción/dashboard y alcance investigativo, la posibilidad de una prueba piloto pequeña y la necesidad de mantener los cambios de alcance pendientes de aprobación. La revisión del equipo no constituye aprobación del tutor.
- Issue #18: dependencia de trabajo indicada por Santiago para el protocolo detallado de evaluación. Aquí se establece su ubicación y la evidencia necesaria, sin fijar rúbrica definitiva, escalas, pesos, umbrales ni métricas finales.

### Insumos revisados y límites de uso

Las rutas de esta tabla parten de la raíz del repositorio. Se revisó texto de los documentos de oficina y PDF; no se certifican su maquetación ni el contenido de imágenes incrustadas. Los aportes son antecedentes, no publicaciones académicas independientes ni aprobaciones.

| Insumo | Procedencia o responsable registrado | Uso y límite de verificación |
|---|---|---|
| `docs/documento_maestro.md` | Esqueleto autorizado por Santiago | Pregunta, objetivos, metodología y alcance figuran pendientes. Se mantiene intacto. |
| `material_profesor/Revision_Analisis_Predictivo_Deuda_Tecnica. 1docx.docx` | Archivo local preexistente no versionado; autoría de sus cambios PENDIENTE | Contiene la pregunta y objetivos reformulados transcritos en §2. Es base de trabajo local, sin evidencia de aprobación del tutor. |
| `material_profesor/Revision_Asesor_Analisis_Predictivo_Deuda_Tecnica. 1docx.docx` | Original institucional versionado | Leído desde HEAD porque aparece eliminado en el árbol local preexistente. Incluye propuesta original y comentarios del asesor; no se restaura ni modifica. |
| `docs/aportes/metodologia/alcance_definitivo.md` | Entregable #10, shibito9 | Registra discrepancias y pendientes; su nombre no significa aprobación. |
| `docs/aportes/metodologia/Delimitacion_alcance_y_criterios.odt` | AP-02, #5, shibito9 según inventario | Fortalezas: delimitación, cautelas y piloto. No aporta bibliografía ni protocolo definitivo; condiciona piloto al tiempo. |
| `docs/aportes/metodologia/Propuesta.Metodologica.pdf` | AP-07, #6, deyvi0297 según inventario | Aprovechable como secuencia de extracción, consulta y contraste. Anticipa beneficios y carece de controles suficientes; no se adopta su matriz como evaluación aprobada. |
| `docs/aportes/llm/fundamentacion_academica_llm.md` | Aporte centralizado de la rama de KarmaDevz, #13 | Distingue evidencia, interpretación e hipótesis; orienta registro de contexto y revisión humana. No se revalidaron aquí los artículos originales ni sus cifras. Conserva limitación de acceso al texto completo de DePalma et al. |
| `docs/aportes/llm/investigacion-llm-analisis-estatico.md` | AP-05, #4, KarmaDevz | Antecedente de contraste y trazabilidad; contiene arquitectura con reporte/dashboard y modelos candidatos, sin selección aprobada. |
| `docs/aportes/sonarqube/Metricas.seleccionadas.pdf` | AP-04, #3, deyvi0297 | Métricas candidatas; faltan claves, versiones y fuentes precisas. No justifica un análisis completo de toda la deuda. |
| `docs/aportes/sonarqube/SonarQube.docx` | AP-08, #7, lukaspardo | Explicaciones y candidatos; contiene equivalencias y generalizaciones que requieren ajustes. |
| `docs/aportes/sonarqube/Metricas_SonarQube.docx` | Centralización registrada en `auditoria/estado_centralizacion_2026-10-25.md`; autoría intelectual PENDIENTE | Incluye claves y límites de estimaciones, pero también equipara señales con deuda y propone gobernanza del prototipo. No se adopta su selección como definitiva. |

El inventario `auditoria/inventario_aportes.md` identifica AP-02, AP-04, AP-05, AP-07 y AP-08 y recomienda revisión o ajustes según cada aporte; sus estados no autorizan integración. Las fuentes académicas y la documentación técnica citadas por estos insumos requieren comprobación directa en fase 1 antes de sustentar afirmaciones del informe. Este borrador contiene una **propuesta metodológica propia**, razonada desde los requisitos del #17 y las restricciones documentadas; el fundamento directo del diseño de estudio de caso y del proceso empírico se delimita en §3, sin presentar la clasificación final como validada.

Trazabilidad prevista: #17 → este archivo → insumos y fuentes verificadas → fichas RAE existentes o PENDIENTES → secciones potenciales 8, 9, 10 y 11 del maestro → commit de integración **PENDIENTE**. No se crean fichas RAE ni se modifica el maestro. Aceptación para uso posterior: **PENDIENTE de Santiago y de la revisión académica correspondiente**.

## 2. Pregunta y objetivos utilizados como base de trabajo, pendientes de validación

Se transcriben literalmente las formulaciones del DOCX local identificado en §1, sin reformularlas. Estas formulaciones se utilizan como base de trabajo y continúan pendientes de validación; no se declaran aprobadas por el tutor ni integradas al maestro. La discrepancia con el maestro y el original institucional se registra en §8.

**Pregunta de investigación**

> ¿De qué manera la combinación de métricas de análisis estático obtenidas mediante SonarQube y el análisis de un modelo de lenguaje puede apoyar la identificación, interpretación y priorización de posibles manifestaciones de deuda técnica en un caso de estudio de software?

**Objetivo general**

> Evaluar la complementariedad entre las métricas de análisis estático obtenidas mediante SonarQube y el análisis de un modelo de lenguaje para apoyar la identificación, interpretación y priorización de posibles manifestaciones de deuda técnica en un caso de estudio de software.

**Objetivos específicos**

1. Caracterizar las métricas y hallazgos relevantes obtenidos mediante SonarQube, así como las capacidades y limitaciones de los modelos de lenguaje aplicados al análisis de código, con relación a la identificación y gestión de posibles manifestaciones de deuda técnica.
2. Aplicar SonarQube y un modelo de lenguaje seleccionado sobre un caso de estudio de software previamente delimitado, utilizando un procedimiento reproducible que permita registrar y contrastar los hallazgos obtenidos por ambas herramientas.
3. Evaluar la complementariedad entre los resultados de SonarQube y el análisis del modelo de lenguaje, considerando su utilidad para apoyar la identificación, interpretación y priorización de posibles manifestaciones de deuda técnica mediante criterios técnicos y validación humana.

La pregunta se abordaría contrastando información estática, interpretaciones del modelo y decisiones humanas sobre el mismo caso. Identificar significa registrar candidatos observables; interpretar exige vincularlos con código y contexto; priorizar exige una justificación revisable conforme al protocolo pendiente del #18. Ninguna de estas tareas acredita predicción temporal ni reducción de deuda.

## 3. Propuesta de tipo, enfoque y diseño de investigación

Se propone una investigación **aplicada, de alcance exploratorio y descriptivo**, mediante un **estudio de caso delimitado con contraste entre resultados de herramientas**. Es aplicada porque examinaría un problema concreto de análisis de software; exploratoria porque indagaría una complementariedad no demostrada; descriptiva porque documentaría hallazgos, explicaciones, discrepancias y límites del caso. No se propone inferir efectos causales ni generalización estadística.

Se propone un **enfoque predominantemente cualitativo**, centrado en descripciones técnicas y juicios humanos argumentados, con posibilidad de incorporar registros cuantitativos descriptivos si el protocolo del Issue #18 los define. Estos registros podrían relacionarse con las interpretaciones y prioridades en la fase 7; su incorporación no establece por sí sola un enfoque mixto. La clasificación final del tipo, enfoque y diseño requiere validación metodológica y del tutor.

La justificación del diseño es su correspondencia con los objetivos: caracterizar insumos (OE1), aplicarlos bajo condiciones documentadas (OE2) y examinar el aporte contextual y sus errores con revisión humana (OE3). Esta es una propuesta para validación del equipo y tutor, no una decisión ya aprobada. El fundamento directo del estudio de caso se apoya en Runeson y Höst (2009, §2.1), quienes lo describen como un método empírico para investigar fenómenos contemporáneos en su contexto. Esto orienta la propuesta de examinar el análisis de software dentro de un caso delimitado y contextualizado; no acredita por sí solo la adecuación final del caso todavía pendiente.

Wohlin et al. (2012) presentan los estudios empíricos en ingeniería de software desde una perspectiva de proceso; la descripción editorial consultada identifica delimitación, planificación, ejecución, análisis y presentación de resultados. Se utiliza este fundamento únicamente para orientar la organización del procedimiento empírico. La conservación de configuraciones, entradas y salidas se propone aquí para facilitar su reproducción, sin atribuir al libro esta lista concreta ni afirmar que la reproducibilidad esté demostrada.

**Referencias y alcance de consulta (2026-11-01):**

- Runeson, P., & Höst, M. (2009). Guidelines for conducting and reporting case study research in software engineering. *Empirical Software Engineering, 14*, 131–164. https://doi.org/10.1007/s10664-008-9102-8. Se consultó directamente el texto HTML editorial, incluida §2.1, para el fundamento citado; no se declara una revisión exhaustiva de todas sus recomendaciones.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M. C., Regnell, B., & Wesslén, A. (2012). *Experimentation in Software Engineering*. Springer. https://doi.org/10.1007/978-3-642-29044-2. Se consultaron la descripción editorial y el índice, no el texto completo del libro. Esta limitación restringe la atribución al enfoque de proceso allí descrito.

Estas fuentes no se utilizan para avalar capacidades de SonarQube o del LLM, criterios del #18 ni la clasificación final propuesta. La fundamentación adicional y su revisión metodológica permanecen pendientes.

## 4. Caso de estudio y papeles de los participantes

### Unidad de estudio

Se propone que el caso sea una unidad de software delimitada —repositorio o componente con sus dependencias pertinentes— en un commit o versión inmutable y un contexto documentado. Se propone tratar los archivos, funciones y hallazgos como unidades de observación internas, sin contarlos como proyectos independientes. Repositorio, lenguaje, tamaño, licencia, límites y selección final: **PENDIENTES**. Este repositorio de tesis no se asume como corpus de código.

Se propone seleccionar el caso justificando acceso y permiso de análisis, licencia, compatibilidad con herramientas, disponibilidad de contexto, factibilidad en los recursos y plazo disponibles y posibilidad de repetir el análisis. El procedimiento prevé documentar candidatos, razones de selección y descarte, inclusión/exclusión de archivos y límites de la muestra antes de consultar resultados del LLM. No se exige que el caso produzca resultados favorables. Se propone registrar los cambios de versión en otra corrida identificada, sin mezclar resultados.

### SonarQube

Se propone utilizar SonarQube para obtener reportes de reglas y métricas bajo una configuración registrada. Sus hallazgos son señales para contraste, **no deuda técnica automáticamente confirmada ni ground truth**. El procedimiento prevé separar regla incumplida, métrica, interpretación de deuda y eventual prioridad, conservar el esfuerzo de remediación como estimación de la herramienta, no como costo real comprobado, y verificar claves, unidades y disponibilidad contra la documentación de la versión seleccionada, registrando URL y fecha; aquí no se fija una lista final ni umbrales de calidad.

### LLM de código abierto

Se propone utilizar un modelo existente para analizar código y contexto, explicar candidatos y formular recomendaciones o prioridades argumentadas para revisión. No es un lenguaje de programación ni un verificador que ejecute y pruebe automáticamente el programa. Sus salidas pueden contener errores y no son ground truth ni evidencia académica por sí mismas. Modelo, licencia, versión exacta y configuración quedan **PENDIENTES**; disponibilidad de pesos no bastará para denominarlo de código abierto sin verificar las condiciones de la versión. No se contempla entrenamiento propio ni aplicación automática de refactorizaciones en este procedimiento.

Como propuesta comparativa, pueden contemplarse dos condiciones si el protocolo del Issue #18 las aprueba: análisis del código y contexto sin diagnóstico previo de SonarQube; e interpretación asistida con el reporte explícitamente incorporado. No son obligatorias ni forman todavía parte de un protocolo aprobado. Si se aprueban ambas, se propone conservar la consulta sin diagnóstico antes de la asistida, utilizando sesiones separadas y un contexto base trazable. La primera solo permite hablar de una consulta sin diagnóstico suministrado: no elimina sesgos de selección ni posibles datos de entrenamiento. La segunda permite estudiar interpretación contextual, pero su coincidencia con SonarQube **no es detección independiente**. Su factibilidad, extensión e inclusión quedan pendientes del protocolo del #18 antes del piloto; el procedimiento prevé declarar cualquier condición no ejecutada.

### Validación humana

Se propone que las personas revisoras contrasten las salidas con el código y la documentación disponible y justifiquen cada decisión. Identidades, competencias, cantidad de revisores y forma de resolver desacuerdos se definirán antes de evaluar, mediante el #18 y validación del tutor. El procedimiento prevé conservar dictámenes iniciales, evidencia, discrepancias y decisiones posteriores con autor y fecha. Si no puede resolverse una discrepancia, se mantendrá como inconclusa. El juicio humano también tiene límites: no se presentará como verdad infalible ni referencia exhaustiva de todos los problemas del caso.

## 5. Procedimiento reproducible propuesto

Las fases describen trabajo futuro. Antes de las corridas evaluables deberán estar fijados el caso, las condiciones de consulta y la versión del protocolo del #18. Las pruebas de factibilidad se identificarán aparte para evitar confundir ajuste del procedimiento con resultados evaluados.

### Fase 1. Revisión y caracterización documental

Registrar preguntas de búsqueda, bases consultadas, cadenas, fechas, criterios de inclusión/exclusión y motivos de selección. Separar corpus bibliográfico, corpus de código y resultados experimentales de forma conceptual, sin autorizar reorganización de carpetas. Para cada fuente, registrar publicación, autores, fecha, tipo, localizador y nivel de acceso; distinguir resumen de texto completo. Comprobar qué afirmación respalda y qué limitaciones tiene. Vincular fichas RAE existentes o marcar el vínculo PENDIENTE.

Caracterizar deuda técnica, señales de calidad, análisis estático y LLM sin confundirlos. Contrastar las métricas candidatas de los aportes SonarQube con documentación oficial versionada, diferenciándola de validación académica independiente. Entregable previsto: registro documental y caracterización argumentada para OE1, con fuentes verificadas y pendientes visibles.

### Fase 2. Preparación y delimitación del caso de estudio

Aplicar los criterios de selección de §4 y registrar repositorio, procedencia, permiso/licencia, commit, lenguaje y versión, tamaño observado, límites, dependencias, documentación y exclusiones. Preservar una instantánea identificable y registrar entorno y comandos necesarios. Definir el conjunto de unidades que se inspeccionará y el método de selección antes de consultar el LLM, incluyendo exclusiones justificadas. Congelar las condiciones evaluables y el protocolo del #18; registrar cualquier cambio posterior como desviación. Entregable: ficha del caso y manifiesto de ejecución para OE2.

### Fase 3. Configuración y ejecución del análisis con SonarQube

Registrar edición, versión, modo, analizadores y plugins, scanner, perfil de calidad, reglas activas y parámetros, métricas y unidades, exclusiones y definición de código nuevo si se usa. Conservar configuración reproducible sin credenciales, comandos, logs, fecha e identificador de análisis sobre el commit fijado. Archivar reporte original completo y documentar errores o análisis parciales.

Seleccionar hallazgos mediante el método previamente declarado, conservando universo accesible, criterios, incluidos y excluidos. Vincular cada hallazgo a identificador original, regla, archivo, líneas y métricas disponibles. Si se incluyen unidades sin alerta para contraste, registrar el motivo; ausencia de alerta no significa ausencia de deuda. Entregables: reporte íntegro y registro de selección para OE1 y OE2.

### Fase 4. Preparación del contexto y análisis mediante LLM

Fijar modelo y artefacto exactos, entorno y parámetros. Preparar paquetes de contexto identificables: fragmentos con archivo y líneas del commit, dependencias pertinentes y documentación efectivamente disponible. Registrar lo incluido, lo omitido, orden, fragmentación y truncamiento; no inventar requisitos de negocio. Versionar los prompts completos, incluidos mensajes de sistema, instrucciones, plantillas y entradas instanciadas.

Ejecutar la(s) condición(es) de consulta previamente aprobadas en el protocolo del Issue #18, sin trasladar respuestas entre sesiones cuando corresponda. Si se aprueba la condición asistida, conservar exactamente qué diagnóstico de SonarQube recibió el modelo. Solicitar evidencia localizable y declaración de incertidumbre sin exigir confirmación de una alerta ni mejora. Registrar toda respuesta original, fallos, reintentos y repeticiones previstas; no elegir únicamente respuestas favorables. Número de repeticiones y reglas de reintento: PENDIENTES de fijación antes de evaluar. Entregables: entradas y respuestas originales trazables para OE2.

### Fase 5. Registro y contraste de resultados

Relacionar reporte, unidades de código, consultas y respuestas sin reemplazar los originales por resúmenes. Registrar coincidencias, diferencias, candidatos adicionales, afirmaciones sin respaldo y asuntos no comparables; son observaciones preliminares, no etiquetas definitivas de acierto. Si se aprueban y ejecutan ambas condiciones, mantener separados los resultados sin diagnóstico previo y los asistidos. La selección basada en alertas limita cualquier afirmación sobre cobertura de identificación.

Entregable: registro de contraste inicial para OE2 y OE3. Una coincidencia no confirma deuda, ni un desacuerdo demuestra que alguna herramienta esté equivocada.

### Fase 6. Validación humana

Aplicar la versión previamente fijada del protocolo del #18 a los resultados del contraste. Registrar qué materiales vio cada revisor y cuándo, su dictamen, fundamento localizable, incertidumbre y cualquier revisión de su decisión. Distinguir evaluación del hallazgo, interpretación y prioridad recomendada. Conservar desacuerdos y el procedimiento efectivamente aplicado para resolverlos, sin borrar dictámenes iniciales.

Si el protocolo no está definido, solo procede revisión exploratoria expresamente identificada; no se emiten puntuaciones finales ni se declara cumplida la evaluación. Entregable previsto: registros de revisión humana vinculados a cada unidad y a la versión del protocolo para OE3. Este documento no define sus escalas ni métricas finales.

### Fase 7. Análisis de complementariedad

Contrastar la información del reporte aislado con la aportada mediante LLM y con las decisiones humanas sobre las mismas unidades. Relacionar datos registrados con explicaciones verificadas: qué información adicional pudo sustentarse, qué fue redundante, erróneo, omitido o no evaluable y qué apoyo a la priorización pudo justificarse. Aplicar solo los criterios y análisis autorizados en el protocolo del #18, conservando su versión y las bases utilizadas.

La complementariedad es una hipótesis: el contraste puede mostrar aportes limitados, errores, ausencia de valor adicional o resultados inconclusos. No se presupone superioridad, reducción de deuda ni prevención de riesgos. Entregable: análisis argumentado y trazable para OE3, con resultados favorables y desfavorables tratados con el mismo cuidado.

### Fase 8. Síntesis de resultados y limitaciones

Responder la pregunta y valorar cada objetivo con enlaces a evidencia real; separar observación, interpretación e hipótesis pendiente. Documentar sesgos de selección, contexto insuficiente, variabilidad del modelo, exposición previa de revisores, límites de la referencia humana y amenazas a reproducibilidad y generalización. Declarar condiciones no ejecutadas y desviaciones.

Entregable: informe del caso y relación de evidencias para OE1–OE3. Las conclusiones solo corresponderán al caso, commit, lenguaje, muestra, herramientas y condiciones evaluadas. No se inferirán capacidad predictiva, costos reales evitados, reducción de deuda o eficacia de un producto a partir de este ejercicio.

## 6. Registro mínimo para reproducibilidad

Todos los valores concretos están PENDIENTES hasta seleccionar y ejecutar el caso. La siguiente tabla define evidencia exigible, no resultados ni una rúbrica. Cada corrida tendrá identificador, fecha, ejecutor y vínculos persistentes entre sus entradas, salidas y revisión; se conservarán huellas de los artefactos cuando sea posible.

| Registro | Contenido que debe preservarse |
|---|---|
| Caso | URL/repositorio o procedencia, permiso/licencia, componente, alcance y exclusiones, tamaño observado, commit completo o versión inmutable, lenguaje y versión. |
| Entorno | Sistema, hardware relevante, dependencias, versiones, comandos y pasos de preparación necesarios para repetir el procedimiento. |
| SonarQube | Edición y versión, modo, scanner, analizadores/plugins, configuración exportable, perfil, reglas y parámetros, métricas y unidades, exclusiones y código nuevo si aplica. |
| Análisis estático | Identificador y fecha de análisis, commit, logs, reporte original íntegro, fallos y limitaciones de cobertura. |
| Selección | Universo accesible, método y justificación, hallazgos seleccionados y excluidos, ID original, regla, mensaje, severidad, archivo, líneas y valores observados. |
| LLM | Nombre, proveedor/proyecto, versión y revisión exacta de pesos o huella, licencia verificada, runtime y versión, cuantización y entorno local/remoto. |
| Configuración LLM | Temperatura, top-p/top-k si aplican, semilla si está disponible, límite de salida y ventana de contexto, plantilla de conversación, herramientas habilitadas o ausencia de ellas, valores por defecto efectivos y parámetros no controlables. |
| Prompts | Texto completo y versión de instrucciones de sistema y usuario, plantilla e instancia efectivamente enviada; condición sin diagnóstico/asistida y cambios entre versiones. |
| Contexto | Código y documentación exactos, procedencia, commit, archivos y líneas, orden, fragmentación, truncamiento, omisiones y diagnóstico SonarQube recibido o ausencia explícita. |
| Respuestas | Salidas originales completas y sin correcciones, ID de consulta/corrida, fecha, errores, reintentos, repeticiones y motivos; separar anotaciones posteriores. |
| Revisión humana | Versión del protocolo #18, criterios aplicados, revisor y competencia, materiales visibles, fecha, dictamen inicial, evidencia, prioridad justificada cuando proceda, incertidumbre, desacuerdos y decisión posterior con responsable. |
| Contraste | Vínculo caso–hallazgo–consulta–respuesta–revisión; coincidencias, diferencias y aportes sustentados, resultados no evaluables, datos y procedimiento de análisis efectivamente utilizados. |
| Desviaciones | Cambios de caso/configuración/protocolo, motivos, responsable y efecto; distinguir pruebas de factibilidad de corridas evaluables. |

La repetibilidad del procedimiento no garantiza identidad literal de las respuestas del LLM. Los parámetros no controlables y la variación observada deberán informarse. No se sobrescribirán reportes, prompts, respuestas ni dictámenes originales; las síntesis mantendrán el vínculo con ellos. Este borrador no crea carpetas ni fija todavía ubicaciones de esos futuros artefactos.

## 7. Decisiones pendientes de validación del tutor

| Decisión | Qué debe resolverse y registrarse |
|---|---|
| Predicción | Si sigue siendo exigible y qué significa «anticipar». Este diseño no valida predicción temporal; mantenerla requeriría variable futura, datos históricos, horizonte y evaluación temporal separados. |
| Prototipo ejecutable | Obligatoriedad, alcance mínimo y relación con el informe. Ejecutar herramientas para investigar no acredita un prototipo aprobado. |
| Dashboard | Obligatoriedad y función. No se incluye su desarrollo como fase aprobada ni se asume autorizada su eliminación del compromiso institucional. |
| Alcance definitivo del piloto | Obligatoriedad, extensión, plazo y factibilidad; resolver piloto condicionado al tiempo frente a evaluación empírica necesaria para OE2 y OE3. |
| Selección final del caso | Repositorio, unidad, licencia/permiso, lenguaje, tamaño, versión, muestra y exclusiones. |
| Selección/configuración final del LLM | Modelo, condición de código abierto, revisión exacta, recursos, ejecución local/nube, contexto y parámetros; validar condiciones de consulta. |
| Protocolo de evaluación detallado | Entregable del #18: criterios operativos, instrumentos, revisores, desacuerdos, análisis y métricas finales, antes de corridas evaluables. |
| Tipo, enfoque y diseño | Confirmar o ajustar la propuesta de §3 y completar fundamento metodológico académico. |
| Coherencia documental | Confirmar la base de pregunta/objetivos aquí transcrita y conciliar título/resumen mediante #16 y alcance mediante #10, sin cambios silenciosos al original institucional. |

Para cada decisión futura deberán registrarse quién decide, fecha, evidencia localizable, contenido confirmado y pendientes. No se identificó evidencia suficiente para completar esos campos como aprobaciones del tutor.

## 8. Contradicciones, solapamientos y acciones siguientes

- **Maestro frente a formulación local:** el maestro no adopta pregunta ni objetivos; el DOCX local sí contiene la formulación investigativa de §2. Se preservan ambas versiones y se declara cuál sirve de base, sin integrar ni modificar ninguna.
- **Dentro del DOCX local:** pregunta y objetivos investigativos coexisten con metodología de prototipo predictivo y dashboard y con el error «un lenguaje de programación basado en Transformers». Este borrador propone una metodología coherente con §2 y distingue modelo de lenguaje y lenguaje de programación; no corrige el original.
- **Original institucional frente a delimitación interna:** el primero compromete prototipo, predicción y dashboard; AP-02 limita la aplicación y condiciona el piloto al tiempo. `alcance_definitivo.md` propone un ejercicio empírico obligatorio, pero mantiene pendiente la decisión del profesor. No se declara resuelta esa diferencia.
- **Beneficios anticipados:** AP-07 atribuye capacidades favorables y concluye reducción de deuda y mejora de calidad sin resultados propios. Se conserva solo como antecedente; esas conclusiones no se trasladan a este diseño.
- **Hallazgos frente a deuda:** los aportes SonarQube se solapan en métricas y contienen equivalencias fuertes entre code smells, complejidad y deuda; `Metricas_SonarQube.docx` incorpora límites útiles, pero también afirmaciones de deuda directa, gobernanza y garantías del prototipo. Aquí no se adoptan esas equivalencias, políticas ni garantías. Claves, unidades, versiones y selección final requieren revisión técnica posterior.
- **Comparación asistida frente a identificación:** AP-07 entrega el hallazgo al modelo antes de contrastarlo. Esa coincidencia no permite demostrar detección independiente. Se explicita la información recibida en cada condición y el límite de seleccionar unidades a partir de SonarQube.
- **Aportes LLM y evaluación:** sus propuestas de refactorización, arquitectura, dashboard y métricas candidatas no son decisiones aprobadas ni se incorporan como entregables de #17. Su solapamiento con evaluación se remite al #18 y la selección final del modelo sigue pendiente.

El diseño propuesto busca vincular las tres tareas investigativas con registros que faciliten la reproducción del procedimiento, separar herramientas y revisión humana y admitir conclusiones desfavorables o inconclusas. La reproducibilidad no ha sido demostrada. Limitaciones: selección de caso/modelo, aceptación de alcance, validación metodológica final y protocolo detallado aún pendientes. Acción siguiente recomendada: revisión de Santiago y equipo, validación del tutor de las decisiones de §7 y coordinación con #18. No corresponde integrar todavía este borrador al maestro ni declarar cumplida la investigación.

## 9. Matriz de correspondencia con los objetivos específicos

Se usan los números y textos exactos de §2. La matriz muestra cómo podrían cumplirse mediante trabajo y evidencia verificables; no declara su cumplimiento actual.

| Objetivo específico | Fase metodológica | Evidencia/entregable |
|---|---|---|
| OE1. Caracterizar las métricas y hallazgos relevantes obtenidos mediante SonarQube, así como las capacidades y limitaciones de los modelos de lenguaje aplicados al análisis de código, con relación a la identificación y gestión de posibles manifestaciones de deuda técnica. | 1, 3, 4, 5 y 8 | Registro de búsqueda y fuentes con nivel de verificación; caracterización conceptual; reglas y métricas justificadas para la versión usada; reporte estático, respuestas originales y contraste que aporten evidencia sobre capacidades y limitaciones observadas del LLM; síntesis del caso. |
| OE2. Aplicar SonarQube y un modelo de lenguaje seleccionado sobre un caso de estudio de software previamente delimitado, utilizando un procedimiento reproducible que permita registrar y contrastar los hallazgos obtenidos por ambas herramientas. | 2, 3, 4 y 5 | Ficha del caso y commit; manifiesto de configuración; reporte SonarQube; selección trazable; prompts completos versionados, contexto y respuestas originales por condición; registro inicial de contraste. |
| OE3. Evaluar la complementariedad entre los resultados de SonarQube y el análisis del modelo de lenguaje, considerando su utilidad para apoyar la identificación, interpretación y priorización de posibles manifestaciones de deuda técnica mediante criterios técnicos y validación humana. | 5, 6, 7 y 8 | Contraste vinculado al código; protocolo detallado pendiente del #18; dictámenes humanos, criterios y decisiones argumentadas; discrepancias y límites; análisis de complementariedad y síntesis que admita resultados negativos o inconclusos. |
