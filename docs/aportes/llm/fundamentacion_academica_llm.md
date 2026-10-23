# Fundamentación académica: aportes y limitaciones de los LLM para el análisis de código y deuda técnica

**Proyecto:** Título pendiente  
**Estado:** Borrador para revisión
**Fecha de consulta:** 21 de octubre de 2026.

## 1. Propósito y alcance

Examinar evidencia académica sobre modelos de lenguaje grandes (LLM) aplicados al análisis, comprensión y mantenimiento de código, y establecer qué aportes podrían evaluarse en este proyecto en relación con la deuda técnica. Se distinguen expresamente **hallazgos publicados**, **interpretaciones para este proyecto** e **hipótesis pendientes de validación**. Los resultados obtenidos con un modelo, lenguaje o conjunto de proyectos no se extrapolan automáticamente a otros.

La deuda técnica comprende compromisos de diseño e implementación que pueden incrementar el costo de evolución del software. Un *code smell* es una posible señal de problemas de diseño o mantenibilidad; no equivale automáticamente a deuda técnica confirmada ni a un defecto funcional.

## 2. Fichas de fuentes académicas (insumos RAE)

### Fuente 1. Revisión general de LLM en ingeniería de software

- **Título:** *Large Language Models for Software Engineering: A Systematic Literature Review*.
- **Autores:** Xinyi Hou, Yanjie Zhao, Yue Liu, Zhou Yang, Kailong Wang, Li Li, Xiapu Luo, David Lo, John Grundy y Haoyu Wang.
- **Año:** 2024.
- **Publicación:** *ACM Transactions on Software Engineering and Methodology*, 33(8), artículo 220, pp. 1–79.
- **DOI:** https://doi.org/10.1145/3695988
- **Objetivo:** Sistematizar las aplicaciones, estrategias de evaluación y limitaciones de los LLM en ingeniería de software.
- **Metodología:** Revisión sistemática de 395 trabajos de investigación publicados entre enero de 2017 y enero de 2024; clasificación de modelos, tareas, datos y estrategias de evaluación.
- **Hallazgos reportados:** Existe investigación sobre múltiples tareas de ingeniería de software y distintas estrategias de adaptación y evaluación de LLM. El desempeño depende de la tarea, de los datos y de la forma de evaluación; la literatura identifica vacíos de investigación.
- **Limitaciones:** La revisión agrega estudios heterogéneos; no constituye una prueba experimental de desempeño en este proyecto ni demuestra superioridad frente a SonarQube. El período de búsqueda termina en enero de 2024.
- **Utilidad para este proyecto — interpretación propia:** Sirve para organizar el marco conceptual y justificar que cada capacidad se evalúe mediante tareas y métricas específicas, evitando generalizaciones.

### Fuente 2. Detección de code smells

- **Título:** *Detecting Code Smells using ChatGPT: Initial Insights*.
- **Autores:** Luciana Lourdes Silva, Janio Rosa da Silva, Joao Eduardo Montandon, Marcus Andrade y Marco Tulio Valente.
- **Año:** 2024.
- **Publicación:** *Proceedings of the 18th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement (ESEM '24)*, pp. 400–406.
- **DOI:** https://doi.org/10.1145/3674805.3690742
- **Objetivo:** Evaluar la capacidad de ChatGPT para identificar cuatro tipos de *code smells* en proyectos Java.
- **Metodología:** Evaluación empírica con un conjunto de ejemplos de Blob, Data Class, Feature Envy y Long Method, distribuidos en tres niveles de severidad. Comparación de un prompt genérico con uno que enumera explícitamente los smells; métricas de precisión, exhaustividad (*recall*) y F1.
- **Hallazgos reportados:** Las probabilidades de una respuesta correcta fueron 2,54 veces mayores con el prompt específico que con el genérico. La medida F1 fue 0,52 para smells críticos y 0,43 para los leves. Son resultados parciales, no una detección infalible.
- **Limitaciones:** Estudio de alcance inicial; cuatro smells, proyectos Java y configuración concreta de ChatGPT. Los resultados no demuestran desempeño general en otros lenguajes, modelos ni repositorios.
- **Utilidad para este proyecto — interpretación propia:** Fundamenta experimentar con prompts explícitos, taxonomías de problemas y evaluación contra etiquetas verificadas; permite argumentar que la calidad de la detección depende de cómo se formula la solicitud.

### Fuente 3. Reparación de problemas identificados por SonarQube

- **Título:** *An evaluation study of large language models for addressing code quality issues*.
- **Autores:** Rares Patcas y Simona Motogna.
- **Año:** 2026.
- **Publicación:** *Empirical Software Engineering*, 31, artículo 118.
- **DOI:** https://doi.org/10.1007/s10664-026-10858-8
- **Objetivo:** Evaluar si distintos LLM pueden reparar problemas de calidad previamente identificados por SonarQube, sin introducir problemas adicionales y conservando el comportamiento del programa.
- **Metodología:** Estudio empírico en 20 repositorios Python seleccionados de un conjunto de 80; comparación de seis modelos (GPT-4o, Gemini 2.0 Flash, Claude 3 Opus, Mistral Large, Grok 3 y DeepSeek V3). Los hallazgos de SonarQube se incorporaron a prompts estructurados con código contextual. Se evaluaron sintaxis, cambios en alertas y preservación semántica.
- **Hallazgos reportados:** La reducción media de incidencias señaladas por SonarQube fue aproximadamente 36,02 % entre modelos y proyectos. El mejor resultado de reducción en un proyecto fue 71,54 % con Grok 3. Los resultados variaron según el modelo y los problemas tratados; algunas correcciones introdujeron incidencias nuevas.
- **Limitaciones:** Se centra en proyectos Python, una selección de repositorios, versiones específicas de modelos y reglas de SonarQube. Reducir advertencias no garantiza reducir toda la deuda técnica ni preservar funcionalidad. Las cifras de reducción de alertas no deben confundirse con tasa de reparaciones semánticamente correctas.
- **Utilidad para este proyecto — interpretación propia:** Es el antecedente más directamente relacionado con un flujo híbrido: SonarQube detecta y el LLM interpreta o propone soluciones. Sugiere validar por separado la desaparición de alertas, la corrección técnica y la utilidad para desarrolladores.

### Fuente 4. Refactorización con ChatGPT

- **Título:** *Exploring ChatGPT’s code refactoring capabilities: An empirical study*.
- **Autores:** Kayla DePalma, Izabel Miminoshvili, Chiara Henselder, Kate Moss y Eman Abdullah AlOmar.
- **Año:** 2024.
- **Publicación:** *Expert Systems with Applications*, 249 (parte B), artículo 123602.
- **DOI:** https://doi.org/10.1016/j.eswa.2024.123602
- **Objetivo:** Investigar capacidades y limitaciones de ChatGPT para refactorizar código.
- **Metodología:** Estudio empírico de tareas de refactorización realizadas con ChatGPT, según el resumen editorial del artículo.
- **Hallazgos reportados:** La fuente documenta una evaluación empírica de la refactorización, motivada por las dudas sobre la fiabilidad de la interpretación del código por ChatGPT. **No se consignan tasas ni resultados específicos**, porque no fueron verificables en el resumen consultado.
- **Limitaciones:** La ficha se basa en metadatos y resumen editorial; debe consultarse el texto completo antes de atribuir conclusiones experimentales detalladas.
- **Utilidad para este proyecto — interpretación propia:** Aporta un antecedente específico para justificar pruebas de refactorización, con revisión de cambios y pruebas de regresión.

## 3. Síntesis crítica de capacidades

| Capacidad | Estado de evidencia | Alcance y cautela | Posible aplicación en este proyecto |
|---|---|---|---|
| Analizar y clasificar problemas de código | **Respaldada en condiciones concretas** | Silva et al. evalúan cuatro smells en Java, con resultados moderados y sensibles al prompt. | Contrastar etiquetas del LLM con casos revisados por personas. |
| Comprender o explicar código | **Investigada; no validada para este proyecto** | La revisión de Hou et al. incluye tareas de ingeniería de software; producir una explicación convincente no prueba que sea correcta. | Evaluar explicaciones contra el código y el juicio de desarrolladores. |
| Proponer refactorizaciones | **Investigada empíricamente** | DePalma et al. estudian esta tarea; esta revisión no atribuye una tasa de éxito no comprobada. | Pedir propuestas sin aplicarlas automáticamente. |
| Corregir alertas de análisis estático | **Respaldada en un entorno específico** | Patcas y Motogna documentan reducción de incidencias de SonarQube, con variación y posibles efectos secundarios. | Probar un flujo de sugerencia, verificación estática y pruebas. |
| Medir mantenibilidad global | **No demostrada para este proyecto** | Una calificación o explicación generada por LLM no sustituye automáticamente métricas estables y reproducibles. | Comparar consistencia de evaluaciones con indicadores establecidos. |
| Priorizar deuda técnica según impacto | **Hipótesis para este proyecto** | Los estudios aquí examinados no validan una priorización integral que incorpore costo, riesgo y contexto de negocio de este proyecto. | Diseñar una evaluación con criterios explícitos y validación humana. |
| Superar a SonarQube | **No demostrado** | La reparación de alertas detectadas por SonarQube no equivale a una comparación de superioridad en detección. | Formular una evaluación de complementariedad, no de reemplazo. |

## 4. Riesgos y medidas de control

| Riesgo | Consecuencia posible | Medida propuesta para el proyecto |
|---|---|---|
| Alucinaciones | Inventar defectos, dependencias, reglas o justificaciones. | Exigir referencia a archivo, fragmento y evidencia verificable. |
| Respuestas incorrectas | Diagnósticos falsos o recomendaciones que rompan funcionalidad. | Revisión humana y pruebas automatizadas; no aplicar cambios sin aprobación. |
| Contexto insuficiente | Omitir dependencias, requisitos, convenciones o restricciones arquitectónicas. | Suministrar función, módulo, dependencias relevantes y descripción de la regla; documentar el contexto entregado. |
| Dependencia del prompt | Diferentes resultados ante instrucciones similares. | Versionar prompts y parámetros; repetir pruebas con formulaciones controladas. |
| Variabilidad entre modelos | Inconsistencia en severidad, explicación o reparación. | Registrar nombre y versión del modelo, fecha y configuración. |
| Confundir alertas con deuda real | Inflar estimaciones o priorizar problemas de bajo impacto. | Separar hallazgo técnico, interpretación y decisión de prioridad. |
| Riesgos de confidencialidad | Exposición de código o información interna a proveedores externos. | Evaluar políticas de datos, anonimización o ejecución local según requisitos. |
| Ausencia de validación humana | Incorporar conclusiones o cambios injustificados. | Mantener aprobación humana y trazabilidad de cada recomendación. |

Estas medidas son **propuestas metodológicas para este proyecto**, no resultados ya comprobados por el proyecto.

## 5. Propuesta de evaluación futura en este proyecto (no ejecutada)

1. Seleccionar un conjunto acotado de archivos o funciones con hallazgos de análisis estático.
2. Conservar el reporte original de SonarQube: regla, ubicación, severidad y descripción.
3. Preparar un prompt versionado con código y contexto pertinente; solicitar explicación, evidencia y, si procede, refactorización sugerida.
4. Registrar respuestas completas, modelo, versión y configuración.
5. Comparar cada explicación con el código real y con una revisión humana; clasificar aciertos, errores, omisiones y afirmaciones no sustentadas.
6. Si se proponen modificaciones, comprobar sintaxis, pruebas y nuevas alertas sin asumir equivalencia entre estos controles.
7. Evaluar por separado si las recomendaciones ayudan a priorizar deuda técnica según criterios explícitos: impacto, esfuerzo, riesgo y relevancia para el proyecto.

**Métricas candidatas:** precisión, recall y F1 para detección cuando exista un conjunto de referencia; porcentaje de explicaciones aceptadas por revisores; frecuencia de afirmaciones no sustentadas; consistencia entre ejecuciones; porcentaje de cambios que pasan pruebas; tiempo de revisión humana. Estas métricas aún no han sido medidas en este proyecto.

## 6. Conclusiones para socialización

**Conclusión basada en fuentes:** Hay evidencia académica de que los LLM pueden identificar ciertos *code smells* y contribuir a reparar problemas detectados por herramientas estáticas en escenarios delimitados. Su rendimiento no es uniforme: varía con el prompt, el modelo y el tipo de problema.

**Interpretación propia:** El uso más defendible para este proyecto es estudiar los LLM como apoyo para explicar hallazgos, proponer alternativas y facilitar el análisis humano, manteniendo la detección estática y la revisión técnica como mecanismos independientes de contraste.

**Hipótesis pendientes:** Que los LLM mejoren la comprensión de la deuda técnica por parte del equipo, reduzcan el tiempo de análisis, produzcan prioridades útiles o aumenten la mantenibilidad del software este proyecto. Ninguno de estos beneficios puede afirmarse como logrado antes de evaluarlo.

**Preguntas que debe poder responder el integrante:** ¿Qué mide F1 y por qué un valor de 0,52 no significa detección perfecta? ¿Por qué un prompt específico cambia el resultado? ¿Por qué disminuir alertas de SonarQube no demuestra conservar la funcionalidad? ¿En qué se diferencia un *code smell* de deuda técnica confirmada? ¿Qué resultados proceden de artículos y cuáles son propuestas para este proyecto?

## 7. Bibliografía

DePalma, K., Miminoshvili, I., Henselder, C., Moss, K., & AlOmar, E. A. (2024). Exploring ChatGPT’s code refactoring capabilities: An empirical study. *Expert Systems with Applications, 249*, 123602. https://doi.org/10.1016/j.eswa.2024.123602

Hou, X., Zhao, Y., Liu, Y., Yang, Z., Wang, K., Li, L., Luo, X., Lo, D., Grundy, J., & Wang, H. (2024). Large language models for software engineering: A systematic literature review. *ACM Transactions on Software Engineering and Methodology, 33*(8), Article 220, 1–79. https://doi.org/10.1145/3695988

Patcas, R., & Motogna, S. (2026). An evaluation study of large language models for addressing code quality issues. *Empirical Software Engineering, 31*, Article 118. https://doi.org/10.1007/s10664-026-10858-8

Silva, L. L., Silva, J. R. da, Montandon, J. E., Andrade, M., & Valente, M. T. (2024). Detecting code smells using ChatGPT: Initial insights. En *Proceedings of the 18th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement* (pp. 400–406). ACM. https://doi.org/10.1145/3674805.3690742

## 8. Estado de revisión

**Pendiente de revisión académica y técnica.** Antes de integrar al documento maestro, comprobar la lectura del texto completo de DePalma et al., verificar la transcripción bibliográfica conforme a la norma exigida por el programa y trasladar las fichas a la matriz RAE institucional. No se ha realizado una evaluación experimental propia de este proyecto.
