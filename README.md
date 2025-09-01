# PreEntrega2 – Fast Prompting en Acción  
## POC: Informes Automatizados de Fluidez Lectora con IA

### 👩‍🎓 Alumna
Marianela López – Comisión 84180

---

## 📌 Descripción del problema
La evaluación de la fluidez lectora demanda mucho tiempo docente, no está estandarizada y, si se retrasa, los estudiantes con dificultades no reciben intervención a tiempo.  
Este proceso requiere escuchar pruebas individuales, contar palabras correctas por minuto (WCPM), registrar errores, analizar métricas oculomotoras y luego elaborar informes narrativos.

---

## 💡 Propuesta de solución
Automatizar la **generación de informes de fluidez lectora** mediante IA generativa.  
A partir de un **JSON con resultados de lectura**, la IA produce un informe narrativo con:
- Resumen ejecutivo  
- Clasificación de precisión y fluidez  
- Errores tipificados  
- Análisis de métricas oculomotoras  
- Recomendaciones SMART (6–8 semanas)

---

## 🧪 Técnicas de Fast Prompting aplicadas
- **Zero-shot prompting:** generar informe directo sin ejemplos.  
- **One-shot prompting:** guiar con un ejemplo de salida.  
- **Few-shot prompting:** varios ejemplos para máxima consistencia.  
- **Prompt sanitizador:** protección de PII (nombres, teléfonos, etc.).  

---

## 🔧 Cómo usar la notebook
1. Abrir `PreEntrega2_FastPrompting_POC.ipynb` en Google Colab o Jupyter.  
2. Cargar un JSON de ejemplo en la variable `reading_json`.  
3. Ejecutar prompts en ChatGPT u otro LLM, pegar las salidas en las celdas correspondientes.  
4. Comparar resultados entre Zero, One y Few-shot.  
5. Completar notas en la sección de evaluación.  

---

## 📊 Resultados esperados
- Informes más claros y estandarizados.  
- Ahorro de tiempo docente.  
- Intervención pedagógica temprana.  
- Validación de que Fast Prompting mejora la propuesta inicial de la Pre-entrega 1.

---

## 📂 Estructura del repositorio

