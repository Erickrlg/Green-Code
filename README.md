# Green-Code
Repositorio de mi Primer proyecto en DIO sobre Utilización de Google NotebookLM
# 🌿 Miniguía de Estudios: IA Generativa y Green Coding
> **Proyecto de Aprendizaje Activo con Google NotebookLM**

Este repositorio contiene mi proyecto para el curso de **Desarrollo de IA** en la plataforma [DIO](https://www.dio.me/). Aquí exploro cómo la Inteligencia Artificial puede ayudarnos a escribir código más eficiente y sostenible (Green Coding).

---

## 📝 Contexto y Objetivos

El **Green Coding** es un enfoque de ingeniería de software que busca minimizar el consumo energético de las aplicaciones. En este proyecto, utilizo **Google NotebookLM** como mi socio de estudio para analizar documentación técnica y extraer mejores prácticas de optimización.

**Objetivos del proyecto:**
* Identificar patrones de código que consumen mucha energía (Hotspots).
* Aprender a usar la IA para auditar algoritmos bajo la métrica de eficiencia energética.
* Crear un flujo de trabajo replicable para revisiones de código "verdes".

---

## 📚 Curaduría de Fuentes
Para alimentar mi NotebookLM, seleccioné las siguientes fuentes técnicas:

1.  **Green Software Foundation:** [Principios del Software Verde](https://learn.greensoftware.foundation/) (Documentación base).
2.  **Microsoft Green Tech:** [Reportes sobre Software Sostenible](https://devblogs.microsoft.com/sustainable-software/).
3.  **IBM:** [O futuro da inteligência artificial e da eficiência energética](https://www.ibm.com/br-pt/think/insights/future-ai-energy-efficiency/).
4. **SiliconFlow:** [Guía Definitiva - Los Mejores LLM Energéticamente Eficientes para Implementación en 2026](https://www.siliconflow.com/articles/es/best-energy-efficient-LLMs-for-deployment)

---
### 🧠 Ingeniería de Prompts y "Cicatrices"

#### ❌ Primer Intento : Enfoque de Auditor
* **Prompt:** "[Actúa como un Auditor de Software Sostenible. Basándote exclusivamente en las fuentes que he subido, explica qué es el 'Software Carbon Intensity' (SCI) y menciona 3 estrategias prácticas que un desarrollador puede aplicar hoy mismo para reducirlo. Presenta la respuesta en una tabla comparativa.]"
* **Resultado:** NotebookLM generó la tabla, pero las estrategias eran muy teóricas y no mencionaba ejemplos de código específicos.
* **Dificultad (Cicatriz):** NotebookLM tiende a ser muy resumido si no se le pide explícitamente que "profundice en los ejemplos técnicos".
* **Troubleshooting:** Tuve que ajustar el prompt para pedirle que incluya fragmentos de código de ejemplo (Code Snippets).

#### ✅ Segundo Intento : Enfoque técnico de Ingeniería (Optimizado)
* **Prompt:** "[Actúa como un Desarrollador de Software Senior especializado en Green Coding. La respuesta anterior fue útil en cuanto a costos, pero ahora necesito evidencia técnica.

Basándote en mis fuentes:

1) Identifica un patrón de código 'sucio' (por ejemplo, un bucle ineficiente o una consulta pesada).
2) Proporciona un ejemplo de código (Snippet) en Python o JavaScript que sea ineficiente.
3) Proporciona la versión optimizada (Green) del mismo código.
4) Explica brevemente por qué la segunda versión consume menos ciclos de CPU o memoria.".]"
   
* **Resultado:** La IA pasó de dar consejos teóricos sobre costos a proporcionar comparativas de código (Inneficient vs. Green).
* **Mejora (Troubleshooting):** Al asignar un rol de "Desarrollador Senior" y pedir explícitamente "Snippets", obligué al modelo a buscar patrones algorítmicos en las fuentes en lugar de resúmenes ejecutivos.
* **Lección aprendida:** La especificidad en el formato de salida (pedir código) es clave para usar NotebookLM como herramienta de desarrollo y no solo de lectura.

---

## 📖 Miniguía de Estudo
### Resumen Estructurado
El Green Coding no es solo "ahorrar batería", es una disciplina que impacta en el costo operativo (Cloud) y la latencia del usuario. A través de este estudio, determiné que la **optimización de consultas a bases de datos** es el punto con mayor retorno de inversión energética.

### Glosario Clave

* **Software Carbon Intensity (SCI):** Es una especificación técnica que mide las emisiones de carbono de una aplicación basándose en el consumo de energía y la intensidad de carbono de la red.
Aplicación real: Un programador usa el SCI para calcular cuántos gramos de CO2 se emiten por cada mil transacciones procesadas en su API.
* **EcoQoS:** Es un nivel de Calidad de Servicio (QoS) en Windows que permite ejecutar procesos de forma eficiente para aumentar la duración de la batería y reducir el calor generado.
Aplicación real: Al desarrollar una aplicación de sincronización en segundo plano, el programador marca esos procesos con el nivel EcoQoS para que no drenen la energía del dispositivo del usuario.
* **Interrupción Temprana (Early Stopping):** Técnica de entrenamiento que predice si un modelo superará o no las expectativas de rendimiento y detiene el proceso si los resultados iniciales son pobres para ahorrar energía.
Aplicación real: Un desarrollador configura su pipeline de IA para cancelar automáticamente el entrenamiento de un modelo si la pérdida (loss) no disminuye en las primeras 5 épocas, evitando ciclos de CPU inútiles.
* **Hardware con limitación de potencia:** Configuración que limita el consumo eléctrico del procesador para maximizar la eficiencia, reduciendo el gasto energético hasta un 15% con un impacto mínimo en la velocidad.
Aplicación real: Un ingeniero de SRE configura sus servidores de pruebas para operar con un límite de potencia, aceptando un retraso del 3% en las pruebas a cambio de un ahorro energético significativo.
* **LLM Energéticamente Eficientes (Modelos Ligeros):** Modelos de lenguaje de tamaño reducido (normalmente entre 7B y 9B parámetros) optimizados para ofrecer alta calidad con requisitos mínimos de recursos.
Aplicación real: Un programador elige implementar Llama 3.1-8B en lugar de un modelo generalista masivo para una tarea de resumen de texto, reduciendo drásticamente la huella de carbono de la inferencia
* **Carbon Intensity:** Cantidad de carbono emitido por unidad de energía consumida.
* **Energy Proportionality:** La relación entre el uso de hardware y el consumo de energía.
* **Big O Notation:** Medida de la eficiencia de un algoritmo.

### Prompts Reutilizables
* `"Resume los principios de eficiencia energética aplicados a [Lenguaje X]."`
* `"Explica la diferencia de consumo entre un bucle 'for' tradicional y una operación vectorizada en este contexto."`

---

## 👨‍💻 Autor
Desarrollado por Erick Ledezma para el desafío de proyecto en DIO.
