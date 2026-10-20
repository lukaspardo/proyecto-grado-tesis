# Inventario de aportes del proyecto

Fecha de corte: 2026-10-19  
Repositorio: https://github.com/lukaspardo/proyecto-grado-tesis  
Commit local inspeccionado: 75bb53cf424948a1123e669170dc0e16fdf4c0c6  
Rama inspeccionada: santiago/auditoria-proyecto

## 1. Objetivo y alcance

Registrar los aportes existentes antes de reorganizar el repositorio, modificar documentos académicos o consolidar el documento maestro.

El inventario comprende:

- Los cuatro archivos versionados en docs/.
- Los seis adjuntos localizados en comentarios de los Issues.
- La relación entre archivos, tareas y responsables.
- Una evaluación preliminar del contenido y su siguiente acción.

Se identificaron diez ubicaciones de archivos que corresponden a ocho archivos distintos. Dos adjuntos son copias binarias idénticas de documentos versionados.

Los adjuntos se leyeron en memoria para calcular sus huellas SHA-256. No se guardaron copias locales.

Este inventario no demuestra que se hayan recuperado materiales compartidos fuera de GitHub, como documentos del grupo, archivos personales o conversaciones externas.

## 2. Criterios de clasificación

Los estados corresponden al aporte, no al Issue:

| Estado | Criterio |
|---|---|
| ENTREGADO_PENDIENTE_REVISION | Existe una entrega identificable, pero requiere revisión antes de decidir su incorporación o uso. |
| REQUIERE_AJUSTES | Hay contenido aprovechable, pero presenta problemas concretos de precisión, fuentes, alcance o método. |
| ACEPTABLE_PARA_INTEGRACION | Puede incorporarse para el propósito delimitado que se indica, sujeto a aprobación del responsable de integración. No implica que constituya una investigación validada. |
| INSUFICIENTE | No cubre una parte esencial del objetivo al que se relaciona; requiere desarrollo sustancial. |

La clasificación es una recomendación de auditoría. No constituye aprobación del equipo, no cambia el estado de los Issues y no autoriza integrar archivos.

Un Issue cerrado no convierte su entrega en aceptable.

## 3. Identificación de responsables

Se utilizan usuarios de GitHub como identificadores verificables.

Se distingue entre:

- Responsable asignado: usuario registrado en assignees del Issue.
- Publicador de la entrega: usuario que publicó el comentario con el adjunto.
- Autor del commit: identidad registrada en Git; no prueba por sí sola autoría intelectual.

No se infieren nombres completos a partir de alias.

En los DOCX de deuda técnica y SonarQube figura “lukas pardo gomez” como creador en los metadatos. Ese dato se registra como metadato declarado, no como verificación de identidad o autoría exclusiva.

## 4. Resumen del inventario

| ID | Archivo o aporte | Issue principal | Responsable asignado | Issue | Estado recomendado |
|---|---|---|---|---|---|
| AP-01 | docs/README.md | #1, relación inferida | lukaspardo | Cerrado | INSUFICIENTE |
| AP-02 | Delimitacion_alcance_y_criterios.odt | #5 | shibito9 | Cerrado | ACEPTABLE_PARA_INTEGRACION |
| AP-03 | Deuda Tecnica.docx | #2 | lukaspardo | Cerrado | INSUFICIENTE |
| AP-04 | Métricas seleccionadas.pdf | #3 | deyvi0297 | Cerrado | REQUIERE_AJUSTES |
| AP-05 | investigacion-llm-analisis-estatico.md | #4 | KarmaDevz | Cerrado | REQUIERE_AJUSTES |
| AP-06 | apuntes.txt | #4 | KarmaDevz | Cerrado | ENTREGADO_PENDIENTE_REVISION |
| AP-07 | Propuesta Metodológica.pdf | #6 | deyvi0297 | Cerrado | REQUIERE_AJUSTES |
| AP-08 | SonarQube.docx | #7 | lukaspardo | Cerrado | REQUIERE_AJUSTES |

Totales por archivo distinto:

- ENTREGADO_PENDIENTE_REVISION: 1.
- REQUIERE_AJUSTES: 4.
- ACEPTABLE_PARA_INTEGRACION: 1.
- INSUFICIENTE: 2.

AP-01 es un archivo de orientación del repositorio, no una investigación académica. Se incluye porque forma parte del inventario completo solicitado.

## 5. Registro detallado

### AP-01 — Orientación documental del repositorio

- Issue: #1, “Organizar repositorio,  backlog y documento maestro”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/1
- Estado del Issue: cerrado.
- Responsable asignado: lukaspardo.
- Archivo: docs/README.md.
- Autor del commit de incorporación: shibito9.
- Relación con el Issue: inferida por su función organizativa; no hay un enlace explícito desde el archivo.
- Tipo: Markdown de orientación.
- Objetivo aparente: presentar la documentación del proyecto.
- Fuentes identificadas: ninguna; no son necesarias para su función de navegación.
- Contenido comprobado: “Documentacion del proyecto”.
- Fortalezas: establece un punto inicial de documentación.
- Problemas: no explica alcance, organización, entregables, responsables, procedimiento de contribución ni documento maestro.
- Estado recomendado: INSUFICIENTE.
- Acción siguiente: definir posteriormente una guía de navegación y contribución. No modificar este archivo durante el inventario.

### AP-02 — Delimitación del alcance y criterios

- Issue: #5, “Delimitar alcanze y criterios del proyecto”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/5
- Estado del Issue: cerrado.
- Responsable asignado: shibito9.
- Confirmación de entrega: comentario publicado por shibito9.
- Archivo: docs/Delimitacion_alcance_y_criterios.odt.
- Autor del commit de incorporación: shibito9.
- Tipo: documento ODT de delimitación.
- Objetivo: establecer alcance, exclusiones, criterios observables y resultados esperados.
- Fuentes identificadas: no contiene bibliografía. Su contenido funciona principalmente como propuesta de decisiones del proyecto, no como revisión de literatura.
- Fortalezas:
  - Delimita el enfoque principalmente investigativo.
  - Excluye plataforma completa, entrenamiento propio y corrección automática.
  - Plantea un piloto exploratorio limitado.
  - Reconoce que el piloto no demostraría generalización.
- Problemas:
  - Los criterios son generales y todavía no tienen escalas o reglas de decisión.
  - No define qué evidencia sería suficiente para considerar útil la combinación.
  - No consta en el documento una aprobación formal del alcance por el equipo.
- Estado recomendado: ACEPTABLE_PARA_INTEGRACION.
- Límite de la recomendación: aceptable como documento de alcance interno; no constituye evidencia bibliográfica ni protocolo metodológico definitivo.
- Acción siguiente: someter el alcance a aprobación y desarrollar los indicadores en la metodología, manteniendo separado el original.

### AP-03 — Definición inicial de deuda técnica

- Issue: #2, “Definir deuda tecnica y buscar fuentes academicas”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/2
- Estado del Issue: cerrado.
- Responsable asignado y publicador: lukaspardo.
- Archivo versionado: docs/Deuda Tecnica.docx.
- Adjunto: https://github.com/user-attachments/files/33523736/Deuda.Tecnica.docx
- Metadato de creador del DOCX: “lukas pardo gomez”.
- Tipo: resumen conceptual en DOCX.
- Objetivo: definir deuda técnica y aportar fuentes académicas.
- Fuentes identificadas:
  - https://www.ibm.com/mx-es/think/topics/technical-debt
  - https://www.estudiarenfuniber.com/blog/2024/10/01/busqueda-de-fuentes-referencias/
- Fortalezas:
  - Introduce costos futuros, mantenimiento y decisiones de corto plazo.
  - Incluye enlaces de procedencia.
- Problemas:
  - No contiene artículos académicos seleccionados.
  - Enumerar buscadores y bases de datos no equivale a presentar fuentes científicas.
  - La definición se concentra en atajos y decisiones subóptimas.
  - No desarrolla categorías, límites ni diferencias entre deuda, defecto y code smell.
  - No vincula afirmaciones específicas con citas.
- Estado recomendado: INSUFICIENTE.
- Acción siguiente: solicitar una ampliación bibliográfica y conceptual que cubra el objetivo del Issue.
- Relación entre copias: archivo versionado y adjunto idénticos según SHA-256; constituyen un aporte con dos ubicaciones.

### AP-04 — Selección preliminar de métricas

- Issue: #3, “Investigar metricas de sonarqube aplicables al estudio”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/3
- Estado del Issue: cerrado.
- Responsable asignado y publicador: deyvi0297.
- Archivo mostrado en el comentario: Métricas seleccionadas.pdf.
- Adjunto: https://github.com/user-attachments/files/33605826/Metricas.seleccionadas.pdf
- Ubicación en Git: no se encontró una copia versionada.
- Tipo: PDF de dos páginas.
- Objetivo: seleccionar métricas y explicar su utilidad.
- Fuentes identificadas: no contiene bibliografía ni enlaces en el texto leído.
- Fortalezas:
  - Presenta seis conceptos: deuda técnica, relación de deuda, code smells, bugs, vulnerabilidades y cobertura.
  - Explica su utilidad en lenguaje accesible.
- Problemas:
  - Faltan claves técnicas, unidades, versión y referencias.
  - No justifica suficientemente la relación de cada indicador con deuda técnica.
  - Hay un apartado “Utilidad para el proyecto” sin métrica identificada.
  - La conclusión afirma un análisis completo del estado del proyecto sin sustento suficiente.
  - Se solapa con AP-08.
- Estado recomendado: REQUIERE_AJUSTES.
- Acción siguiente: contrastar definiciones y documentar coincidencias y diferencias con AP-08 antes de una futura unificación.

### AP-05 — Investigación sobre aportes de un LLM

- Issue: #4, “Investigar que puede aportar un LLM al analisis del codigo”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/4
- Estado del Issue: cerrado.
- Responsable asignado y publicador: KarmaDevz.
- Archivo: investigacion-llm-analisis-estatico.md.
- Adjunto: https://github.com/user-attachments/files/33519856/investigacion-llm-analisis-estatico.md
- Ubicación en Git: no se encontró una copia versionada.
- Tipo: revisión técnica y propuesta conceptual en Markdown.
- Objetivo: identificar aportes potenciales, limitaciones y riesgos del LLM.
- Fuentes identificadas:
  - SonarSource, Understanding measures and metrics.
  - Hou et al., revisión sistemática sobre LLM e ingeniería de software, DOI 10.1145/3695988.
  - Li, Avgeriou y Liang, mapeo sobre deuda técnica, DOI 10.1016/j.jss.2014.12.027.
  - Qwen2.5-Coder Technical Report, arXiv:2409.12186.
  - DeepSeek-Coder, arXiv:2401.14196.
  - StarCoder 2 and The Stack v2, arXiv:2402.19173.
  - Code Llama, arXiv:2308.12950.
- Verificación de fuentes:
  - Se comprobó la existencia de la documentación de SonarSource y los cuatro reportes de modelos.
  - Quedó pendiente completar la comprobación de los dos DOI.
  - No se verificó exhaustivamente la correspondencia de cada afirmación con cada fuente.
- Fortalezas:
  - Distingue aportes potenciales de resultados experimentales.
  - Diferencia priorización y predicción.
  - Considera línea base, validación humana, trazabilidad y riesgos.
  - Evita equiparar automáticamente alertas y deuda técnica.
- Problemas:
  - El encabezado conserva un título orientado a prototipo predictivo.
  - Falta armonizarlo con el alcance investigativo actual.
  - Las propuestas experimentales no constituyen un protocolo aprobado.
  - Los modelos candidatos no representan una selección final.
  - Falta completar la revisión bibliográfica.
- Estado recomendado: REQUIERE_AJUSTES.
- Acción siguiente: revisar alcance y referencias; identificar qué partes podrían incorporarse posteriormente al marco teórico y metodología.
- Relación secundaria: aporta antecedentes para #8, pero no demuestra que ese Issue esté cumplido.

### AP-06 — Apuntes exploratorios sobre LLM

- Issue: #4.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/4
- Estado del Issue: cerrado.
- Responsable asignado y publicador: KarmaDevz.
- Archivo: apuntes.txt.
- Adjunto: https://github.com/user-attachments/files/33519857/apuntes.txt
- Ubicación en Git: no se encontró una copia versionada.
- Tipo: notas de investigación en texto plano.
- Objetivo aparente: registrar preguntas, ideas y referencias para desarrollar la investigación.
- Fuentes identificadas: menciones a Li et al. 2015, Fowler, SonarSource y reportes de modelos; no contiene una bibliografía completa.
- Fortalezas:
  - Registra incertidumbres y preguntas pertinentes.
  - Advierte sobre alucinaciones, contexto incompleto y diferencia entre prioridad y predicción.
- Problemas:
  - No es una síntesis académica terminada.
  - Las menciones bibliográficas no sustentan individualmente las afirmaciones.
  - Gran parte del contenido se desarrolla en AP-05.
- Estado recomendado: ENTREGADO_PENDIENTE_REVISION.
- Acción siguiente: revisar su relación con AP-05 y decidir su conservación como antecedente de trabajo, evitando contarlo como una segunda investigación independiente.
- Límite: este estado no recomienda incorporarlo al documento maestro.

### AP-07 — Propuesta metodológica

- Issue: #6, “Definir metodologia de evaluación SonarQube + LLM”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/6
- Estado del Issue: cerrado.
- Responsable asignado y publicador: deyvi0297.
- Archivo mostrado: Propuesta Metodológica.pdf.
- Adjunto: https://github.com/user-attachments/files/33611499/Propuesta.Metodologica.pdf
- Ubicación en Git: no se encontró una copia versionada.
- Tipo: propuesta metodológica en PDF de cuatro páginas.
- Objetivo: definir procedimiento comparativo y matriz de evaluación.
- Fuentes identificadas: no contiene bibliografía ni enlaces en el texto leído.
- Fortalezas:
  - Propone extracción de hallazgos, consultas al LLM y registro de resultados.
  - Incluye claridad, viabilidad, complementariedad y priorización.
  - Presenta una matriz inicial.
- Problemas:
  - La matriz atribuye de antemano capacidades y beneficios a las herramientas.
  - La conclusión anticipa reducción de deuda y mejora de calidad sin resultados.
  - Faltan muestra, rúbrica, evaluadores y tratamiento de desacuerdos.
  - Faltan controles de versiones, parámetros y repetición.
  - No define suficientemente la medición del tiempo ni el costo de revisión humana.
  - Dar al LLM el hallazgo de SonarQube no permite demostrar detección independiente.
  - Algunas afirmaciones sobre las capacidades de SonarQube requieren fuente y versión.
- Estado recomendado: REQUIERE_AJUSTES.
- Acción siguiente: convertir la propuesta en un protocolo evaluable, sin anticipar beneficios, y contrastarla con AP-02 y AP-05.

### AP-08 — Profundización sobre métricas de SonarQube

- Issue: #7, “Seleccionar metricas de SonarQube para evaluar deuda tecnica”.
- Enlace: https://github.com/lukaspardo/proyecto-grado-tesis/issues/7
- Estado del Issue: cerrado.
- Responsable asignado y publicador: lukaspardo.
- Archivo versionado: docs/SonarQube.docx.
- Adjunto: https://github.com/user-attachments/files/33613926/SonarQube.docx
- Metadato de creador del DOCX: “lukas pardo gomez”.
- Tipo: documento técnico DOCX con cuatro capturas.
- Objetivo: explicar qué miden mantenibilidad, complejidad, duplicación y bugs, su relación con deuda técnica y su uso potencial.
- Fuentes identificadas:
  - Capturas de tablas de métricas.
  - No se registra explícitamente su URL, versión o fecha de consulta.
  - La documentación oficial de SonarSource se utilizó como contraste en la auditoría; no debe atribuirse como cita incorporada al documento.
- Fortalezas:
  - Sigue los apartados pedidos en el Issue.
  - Explica métricas y posibles usos.
  - Las capturas muestran claves técnicas y dos modos de métricas.
- Problemas:
  - Falta bibliografía y procedencia de las imágenes.
  - No establece el modo de SonarQube que adoptaría el estudio.
  - Contiene generalizaciones sin sustento, como crecimiento exponencial del costo por duplicación.
  - Presenta alta complejidad como violación de responsabilidad única sin matices suficientes.
  - No justifica los umbrales propuestos.
  - Requiere separar esfuerzo estimado, prioridad y deuda técnica en sentido amplio.
  - Se solapa con AP-04.
- Estado recomendado: REQUIERE_AJUSTES.
- Acción siguiente: revisar las afirmaciones, fijar referencias y especificar métricas candidatas con sus claves, unidades y límites.
- Relación entre copias: archivo versionado y adjunto idénticos según SHA-256.

## 6. Huellas de identificación

Las huellas identifican los bytes observados, no certifican autoría ni calidad académica.

| ID | Ubicación | Bytes | SHA-256 |
|---|---|---:|---|
| AP-01 | docs/README.md | 28 | 12687266bf626f60c4cd375ef62d8cd0e84150f4b8c179649867fb6fd37a8800 |
| AP-02 | docs/Delimitacion_alcance_y_criterios.odt | 39224 | 35471973ab7d8c80a1c16a97e8f8dff5b07c8a1721743b121a1bf692e6748956 |
| AP-03 | docs/Deuda Tecnica.docx | 16142 | 9bb11560477239473fd26dad646b5d9ed5d7f423a08162436710059fc578c838 |
| AP-03 | Adjunto #2: Deuda.Tecnica.docx | 16142 | 9bb11560477239473fd26dad646b5d9ed5d7f423a08162436710059fc578c838 |
| AP-04 | Adjunto #3: Metricas.seleccionadas.pdf | 100787 | 88082e4eff2b7006d2d2c59460ed9bbf3e9fd24c57afd53219f1a14c86a80247 |
| AP-05 | Adjunto #4: investigacion-llm-analisis-estatico.md | 21307 | 872c21bfcda461f1dc98b76a58d568e98e71c1559f84b839a766034d7d366956 |
| AP-06 | Adjunto #4: apuntes.txt | 4368 | 4763545528f7fcb446d2eeba54f0e7787f974c15abc60d173f8dc0196e8a4970 |
| AP-07 | Adjunto #6: Propuesta.Metodologica.pdf | 183253 | f5ebbc12491cc554044966c9fb5b840418caf628ba3bae430df10efcdc4d9575 |
| AP-08 | docs/SonarQube.docx | 477635 | 728a40f7e294154e1303c2ef911d245cd79274e2cfeaf480a78a3d16922846ee |
| AP-08 | Adjunto #7: SonarQube.docx | 477635 | 728a40f7e294154e1303c2ef911d245cd79274e2cfeaf480a78a3d16922846ee |

## 7. Tareas sin entregable específico localizado

| Issue | Responsable | Estado | Situación |
|---|---|---|---|
| #8 — Seleccionar LLM y seleccionar el protocolo de analisis de codigo | KarmaDevz | Abierto | AP-05 aporta antecedentes, pero no se localizó selección final ni protocolo específico entregado. |
| #9 — Diseñar caso de estudio para prueba piloto del proyecto | shibito9 | Abierto | Hay bosquejos en otros aportes, pero no se localizó diseño de un caso concreto. |

La ausencia de un entregable no se clasifica como INSUFICIENTE: no hay un archivo entregado al cual asignar ese estado.

## 8. Procedimiento de reproducción

Para repetir el inventario:

1. Registrar fecha, rama y commit inspeccionados.
2. Enumerar archivos versionados y comprobar el estado de trabajo.
3. Consultar los Issues abiertos y cerrados, incluyendo asignaciones y comentarios.
4. Recorrer todas las páginas de resultados si la API devuelve paginación.
5. Registrar cada enlace de adjunto y quién lo publicó.
6. Leer los archivos sin sobrescribir originales.
7. Calcular SHA-256 sobre los bytes de cada archivo y adjunto.
8. Comparar huellas antes de contar archivos como aportes distintos.
9. Revisar contenido y fuentes sin utilizar el cierre del Issue como criterio de aceptación.
10. Registrar por separado hechos comprobados, relaciones inferidas y pendientes.

En esta consulta se identificaron nueve Issues y seis adjuntos en comentarios. La consulta de Issues solicitó todos los estados y hasta cien resultados.

Los estados y asignaciones de GitHub pueden cambiar después de la fecha de corte. Las huellas permiten identificar los archivos observados, pero no congelan los metadatos de GitHub.

## 9. Límites de la revisión

- No se modificaron documentos, Issues, ramas ni commits.
- No se verificó exhaustivamente toda la literatura citada.
- La lectura de PDF y documentos de oficina fue principalmente textual y estructural; no certifica maquetación.
- Los metadatos y autores de commits no demuestran autoría intelectual exclusiva.
- No se examinó material externo al repositorio y a los adjuntos identificados.
- Las acciones siguientes son recomendaciones pendientes de autorización.
