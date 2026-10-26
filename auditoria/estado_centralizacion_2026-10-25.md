# Estado de centralización — 2026-10-25

Repositorio: https://github.com/lukaspardo/proyecto-grado-tesis

Centralizar un archivo NO significa aprobar académicamente su contenido. Este registro documenta presencia y procedencia; no evalúa fuentes ni resultados académicos.

## Ramas comprobadas

Se ejecutaron `git fetch --all --prune`, `git switch main` y `git pull --ff-only`. Main pasó de `007eaed` a `2b3b2de`, incorporando `Metricas_SonarQube.docx`.

| Rama/aporte | Archivo / ubicación final | Estado | Issue | Observación |
|---|---|---|---|---|
| karmadevz/comparativa-y-fundamentacion | docs/aportes/llm/fundamentacion_academica_llm.md | INTEGRADO | #13 | Fast-forward de 2b3b2de a 5b4370d; contenido conservado. |
| karmadevz/comparativa-y-fundamentacion | docs/aportes/llm/comparativa_modelos_codigo_abierto.md | INTEGRADO | #8 | Mismo fast-forward; únicamente dos archivos añadidos en un commit. |
| deivy/issue-11-deuda-tecnica | Árbol completo de la rama, punta 007eaed | YA_EN_MAIN | #11, por nombre de rama | Comparación main...origin/rama: 2 commits exclusivos de main y 0 de la rama; no se mezcló. No contiene el PDF #11. |
| santiago/auditoria-proyecto | auditoria/inventario_aportes.md; auditoria/estado_proyecto_2026-10-19.md; árbol completo de la rama, punta beee67f | YA_EN_MAIN | #1 | Comparación: 5 commits exclusivos de main y 0 de la rama; no se mezcló. |
| santiago/issue-10-alcance-definitivo | docs/aportes/metodologia/alcance_definitivo.md; árbol completo de la rama, punta bda365b | YA_EN_MAIN | #10 | Comparación: 3 commits exclusivos de main y 0 de la rama; no se mezcló. |

Comparaciones efectuadas con main en `5b4370d` y referencias remotas recién actualizadas. Las tres ramas restantes están absorbidas por historial.

## Entregables y ubicaciones

Se consultaron todos los Issues y comentarios mediante API paginada, incluyendo abiertos y cerrados. No se modificó ningún Issue. Se descargaron los diez adjuntos identificados; salvo el PDF #11, se compararon en memoria sin guardar nuevas copias.

| Rama/aporte / publicador | Archivo | Ubicación final | Estado | Issue | Observación |
|---|---|---|---|---|---|
| lukaspardo | Deuda.Tecnica.docx | docs/aportes/deuda_tecnica/Deuda Tecnica.docx | YA_EN_MAIN | #2 | Adjunto 33523736: SHA-256 idéntico. |
| deyvi0297 | Metricas.seleccionadas.pdf | docs/aportes/sonarqube/Metricas.seleccionadas.pdf | YA_EN_MAIN | #3 | Adjunto 33605826: SHA-256 idéntico. |
| KarmaDevz | apuntes.txt | docs/aportes/llm/apuntes.txt | YA_EN_MAIN | #4 | Adjunto 33519857: igualdad al normalizar CRLF a LF. |
| KarmaDevz | investigacion-llm-analisis-estatico.md | docs/aportes/llm/investigacion-llm-analisis-estatico.md | YA_EN_MAIN | #4, #13 | Adjuntos 33519856 y 33874384 idénticos entre sí; igualdad con archivo local al normalizar CRLF a LF. El adjunto #13 no es el nuevo archivo fundamentacion_academica_llm.md. |
| shibito9 | Delimitacion_alcance_y_criterios.odt | docs/aportes/metodologia/Delimitacion_alcance_y_criterios.odt | YA_EN_MAIN | #5 | Archivo versionado y comentario de entrega; no hay adjunto en ese comentario. |
| deyvi0297 | Propuesta.Metodologica.pdf | docs/aportes/metodologia/Propuesta.Metodologica.pdf | YA_EN_MAIN | #6 | Adjunto 33611499: SHA-256 idéntico. |
| lukaspardo | SonarQube.docx | docs/aportes/sonarqube/SonarQube.docx | YA_EN_MAIN | #7 | Adjunto 33613926: SHA-256 idéntico. |
| KarmaDevz | comparativa_modelos_codigo_abierto.md | docs/aportes/llm/comparativa_modelos_codigo_abierto.md | INTEGRADO | #8 | Adjunto 33874691: igualdad con archivo integrado al normalizar CRLF a LF. |
| shibito9 | alcance_definitivo.md | docs/aportes/metodologia/alcance_definitivo.md | YA_EN_MAIN | #10 | Historial absorbido; comentario del Issue indica validación del profesor pendiente. |
| lukaspardo | Metricas_SonarQube.docx | docs/aportes/sonarqube/Metricas_SonarQube.docx | YA_EN_MAIN | #12 | Adjunto 33851627: SHA-256 idéntico tras actualizar main. |
| Deivy (identificación aportada por Santiago) | Fundamentación Académica de Deuda Técnica.docx; fundamentacion_academica_deuda_tecnica.md | docs/aportes/deuda_tecnica/Fundamentación Académica de Deuda Técnica.docx; docs/aportes/deuda_tecnica/fundamentacion_academica_deuda_tecnica.md | INTEGRADO | #11 | El PDF anterior estaba corrupto. Santiago informó la recepción posterior del DOCX válido, colocado manualmente; se conserva el original y se crea una extracción fiel a Markdown. Centralización NO equivale a aprobación académica. |

Issue #9: sin comentarios ni adjuntos en la consulta; no se identificó un entregable específico nuevo que centralizar.

### Evidencia del PDF #11

- Comentario: https://github.com/lukaspardo/proyecto-grado-tesis/issues/11#issuecomment-6391087495
- Descarga: https://github.com/user-attachments/files/33915823/base.academica.sobre.deuda.tecnica.pdf
- Tamaño recibido: 299590 bytes.
- SHA-256: `fb912413aa0ee50e78475d954fe9b64359c93d4689d8fb60f6bbd746cc2cb1fe`.
- Cabecera `%PDF-1.4` y marcador `%%EOF` presentes; no bastan para validar el archivo.
- Apertura estricta con `pypdf.PdfReader`: `PdfReadError: startxref not found`. No se pudo leer su contenido con este lector.
- Conservado únicamente como descarga temporal fuera del repositorio; no incorporado ni reconstruido.

### Recepción posterior del DOCX del Issue #11

- Procedencia: archivo colocado manualmente y señalado por Santiago como entregable válido de Deivy que sustituye al PDF corrupto; no se infiere que esté adjunto en GitHub.
- Original: `docs/aportes/deuda_tecnica/Fundamentación Académica de Deuda Técnica.docx`.
- Versión derivada autorizada: `docs/aportes/deuda_tecnica/fundamentacion_academica_deuda_tecnica.md`.
- Validación técnica: paquete ZIP sin errores de integridad, XML legible y apertura completa con `python-docx`; 118 párrafos, sin imágenes, tablas nativas, notas al pie ni revisiones registradas.
- SHA-256 del original, comprobado antes y después de la extracción: `cb1027bbf7c45186dfcf8cd381f319f0a763d390e1ef48bdaa459214317e17e4`.
- Conversión: se conserva todo el texto y su orden, incluida la tabla escrita con sintaxis Markdown, autores, DOI y tres fichas RAE. Las 24 viñetas de Word se representan con `-`; solo se adaptan separaciones de párrafo y espacios finales. No se corrigió redacción ni se añadieron fuentes. No hay contenido visual que requiera nota de conversión.
- Las fuentes y afirmaciones académicas no se verificaron en esta operación. Centralizar NO significa aprobar académicamente el aporte.
- Estado del entregable #11: INTEGRADO. La evidencia histórica del PDF corrupto se conserva arriba.

## Límites y control de cambios

- No se reescribieron aportes, no se mezcló contenido académico ni se modificó `docs/documento_maestro.md`.
- No se eliminaron archivos ni se añadieron copias de los adjuntos ya representados en main.
- Los dos archivos de KarmaDevz quedaron versionados en main mediante el commit existente `5b4370d`.
- Además del fast-forward, se incorporan este registro, el DOCX original de Deivy y su versión Markdown mediante el único commit autorizado: `chore: centralizar aporte académico de deuda técnica`.
- No se hizo push.
