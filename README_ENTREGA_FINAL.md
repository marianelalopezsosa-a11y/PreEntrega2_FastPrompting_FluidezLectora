Generador de Adaptaciones Educativas con IA — Fast Prompting

Este repo contiene la POC de un pipeline simple de fast prompting para crear materiales inclusivos (texto→texto y texto→imagen) orientados a contextos reales de aula y a estudiantes con perfiles diversos (p. ej., dislexia leve, atención fluctuante, nivel A2 en progreso).

Estructura

ProyectoFinal_Prompts_Adaptaciones.ipynb: notebook principal (ejecutar en Jupyter/Colab).

infografia.png: imagen ya generada en NightCafe y incluida en el repositorio.

Objetivos (con mis datos)

Reducir 50–70% el tiempo docente dedicado a adecuaciones pedagógicas mediante prompts reutilizables.

Garantizar accesibilidad y claridad aplicando principios de Neuroeducación, DUA y pensamiento crítico (tipografía legible, oraciones cortas, listas, apoyos visuales).

Entregar un set mínimo funcional de materiales listos para uso en aula:

Resumen Adaptado (A2 en progreso),

Mapa Mental (estructura visual/Markdown),

Examen Interactivo gamificado (MCQ/V-F/completar + feedback inmediato),

Infografía (incluida) para refuerzo visual.

Dejar un proceso reproducible en Colab que pueda correrse con o sin API, y que permita personalizar por edad, nivel, fortalezas y desafíos.

Problema y Viabilidad

Problema: la adaptación de materiales para la diversidad del aula consume tiempo y no siempre mantiene consistencia de calidad/accesibilidad.

Solución: pipeline de fast prompting con placeholders para personalizar rápidamente + generación visual con NightCafe.

Viabilidad: se implementa en Google Colab (sin infraestructura), usa OpenAI API (opcional) para texto→texto y NightCafe (gratuito) para texto→imagen. Entregable listo en GitHub.

Metodología

Contexto: definir edad, nivel, fortalezas/desafíos del grupo (ej. 12 años, 6° grado bilingüe, dislexia leve; fortalezas en comprensión global y memoria verbal inmediata).

Prompts con placeholders: {{edad}}, {{nivel_educativo}}, {{dificultades_aprendizaje}}, {{fortalezas_aprendizaje}}, {{texto}}.

Generación:

Resumen Adaptado → texto claro + viñetas + vocabulario bilingüe + 1–2 preguntas de reflexión.

Mapa Mental → secciones ### + subviñetas + emojis (guía visual).

Examen gamificado → formatos variados + feedback por ítem + guía para docente.

Infografía (NightCafe) → diseño limpio, colores suaves, tipografía legible e íconos por sección (archivo incluido).

Accesibilidad: tipografía de palo seco, tamaño ≥14, oraciones cortas, listas, apoyos visuales, y—cuando se pida—MAYÚSCULAS.

Revisión: checklist de cobertura, claridad y adecuaciones; ajustes mínimos manuales.

Herramientas y Tecnologías

Google Colab + Jupyter Notebook.

OpenAI (chat/completions) para texto→texto (opcional; si no hay API, se copia el prompt a un asistente de IA y se pega la salida).

NightCafe para texto→imagen (ya usado; infografia.png incluida).

Markdown accesible y emojis/íconos para apoyos visuales.

GitHub para versionado y entrega pública.

Cómo usar

Abrí la notebook y completá los placeholders (edad, nivel, fortalezas, desafíos, texto base).

Ejecutá las celdas de Caso 1, 2 y 3:

Con OPENAI_API_KEY → la notebook genera texto automáticamente.

Sin API → imprime el prompt final para copiar/pegar en tu IA; pegá la salida en Resultados.

Infografía: ya está incluida como infografia.png. Si querés regenerarla, usá el prompt sugerido y reemplazá el archivo.

Pegá todos los resultados (resumen, mapa, examen, infografía) en la sección Resultados.

Subí todo a GitHub y compartí el link público.

(Opcional) Ejecutar con API
!pip install --upgrade openai
import os
os.environ["OPENAI_API_KEY"] = "sk-...tu_clave..."
# Luego usar la función helper y el prompt_final de cada caso.

Implementación (casos incluidos)

Caso 1 — Resumen Adaptado (A2 en progreso)
Perfil usado en pruebas: 12 años, 6° grado bilingüe, dislexia leve, fortalezas en comprensión global y memoria verbal inmediata.

Caso 2 — Mapa Mental
Estructura visual en Markdown con emojis y ramas temáticas.

Caso 3 — Examen Interactivo gamificado
MCQ, V/F, completar, respuesta breve + feedback inmediato por ítem + sección “Instrucciones para el Docente”.

Infografía (NightCafe)
Diseño accesible con bloques: Título, Datos clave, Ejemplos y Conclusión (infografia.png incluida).

Resultados (con mis datos)

Resumen Adaptado: texto claro con viñetas, vocabulario bilingüe (p. ej., nucleus), y 2 preguntas de reflexión.

Mapa Mental: secciones ### con subviñetas y emojis para guiar lectura y memoria.

Examen gamificado: evaluación accesible con retroalimentación inmediata y pauta para evaluación oral (si aplica).

Infografía: incluida (infografia.png), con colores suaves, tipografía legible e íconos por sección.

Conclusiones

El kit de prompts y el flujo en Colab reducen sensiblemente el tiempo de preparación y mejoran la consistencia de las adecuaciones.

La combinación texto→texto + texto→imagen facilita la comprensión y aumenta la accesibilidad.

El enfoque es escalable y reusable: se pueden sumar Guías de Estudio, Sugerencias Curriculares, Role-plays, etc.

Próximos pasos: agregar métricas de tiempo ahorrado y calidad percibida por docentes/estudiantes.

Referencias

PROMPT 2025 (colección propia de prompts accesibles).

Principios de Neuroeducación, DUA y buenas prácticas de accesibilidad educativa.

Guías de diseño visual NightCafe para generación de imágenes educativas.

Checklist de entrega

 Título, Resumen, Introducción y Viabilidad

 Objetivos

 Metodología

 Herramientas y tecnologías

 Implementación (código + prompts + infografía incluida)

 Resultados

 Conclusiones

 Referencias

Autora: Marianela López — Fundadora y CEO, Empujón Educativo
Contacto: marianelalopezsosa@gmail.com
 · 2615504081
Repositorio público: (pegar aquí el link de GitHub)
Fecha: 2025-09-18
