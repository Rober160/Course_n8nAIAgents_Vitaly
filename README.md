# Course_n8nVitaly
Curso n8n automatización realizado durante las prácticas en Vitaly

## ⚙️ ¿Qué es n8n?

**n8n** es una plataforma de **automatización de workflows de código abierto** que permite conectar aplicaciones, APIs y servicios de forma visual y flexible. Su enfoque **"low-code"** permite tanto a desarrolladores como a usuarios técnicos construir flujos complejos sin necesidad de escribir mucho código.

---

### 🚀 Características principales

- ✨ **Visual**: interfaz gráfica para crear flujos arrastrando y conectando nodos.
- 🔌 **Más de 300 integraciones**: conectores para APIs populares como OpenAI, Google Sheets, Slack, Notion, GitHub, etc.
- 🧠 **Funciona con IA**: integración fácil con modelos como GPT, Whisper, y bases vectoriales para crear agentes inteligentes.
- 🖥️ **Autoalojable o en la nube**: puedes ejecutarlo localmente, en servidores, o usar la versión cloud.
- 📦 **Extensible**: puedes crear tus propios nodos o ejecutar scripts personalizados en JavaScript.

---

### 🧩 ¿Para qué sirve n8n?

- Automatización de tareas repetitivas
- Integración entre servicios que no se comunican entre sí
- Procesamiento de datos y orquestación de flujos
- Construcción de agentes de IA y asistentes inteligentes
- Alertas, reportes, bots, ETL y mucho más

---

### 📘 Ejemplo de flujo con IA y n8n

1. El usuario envía una pregunta.
2. n8n la convierte en un **embedding vectorial**.
3. Consulta una **base de datos vectorial** para recuperar contexto.
4. Pasa el resultado al modelo de lenguaje (GPT).
5. Devuelve una respuesta inteligente al usuario.

---

✅ **n8n** es una herramienta poderosa para automatizar y escalar procesos, especialmente cuando se combina con inteligencia artificial.


_Este curso estará principalmente enfocado en la creación de Agentes de IA_

## 🤖 ¿Qué son los Agentes de IA?

Un **Agente de IA** es un sistema autónomo que puede **percibir su entorno, tomar decisiones y actuar** para lograr objetivos específicos, utilizando modelos de inteligencia artificial. A diferencia de un simple modelo de lenguaje (como GPT), un agente puede tomar acciones, interactuar con herramientas externas y adaptarse según el contexto.

---

### 🧩 ¿Cómo funciona un Agente de IA?

Un agente combina varios componentes:

1. **Entrada del usuario** (pregunta, comando, etc.)
2. **Razonamiento**: analiza qué debe hacer para cumplir el objetivo.
3. **Acción**: puede consultar una base de datos, llamar a una API, realizar cálculos, o generar texto.
4. **Memoria y contexto**: algunos agentes guardan historial o conocimientos previos para usarlos más adelante.
5. **Respuesta**: devuelve un resultado útil o toma una decisión.

---

### 🔧 Capacidades típicas de un agente

- Llamar a herramientas externas (API, buscadores, bases de datos, etc.)
- Realizar tareas secuenciales o condicionales
- Usar **RAG** para mejorar sus respuestas
- Aprender del entorno o del usuario
- Mantener **memoria de largo plazo**

---

### 🧠 Ejemplos de Frameworks de Agentes de IA

- [LangChain](https://www.langchain.com/)
- [AutoGPT](https://github.com/Torantulino/Auto-GPT)
- [CrewAI](https://github.com/joaomdmoura/crewAI)
- [AgentGPT](https://agentgpt.reworkd.ai/)
- Sistemas personalizados con **n8n**, **Python**, o **Node.js**

---

### 🔄 Integración con n8n

n8n permite crear **workflows automáticos** que usan agentes de IA para ejecutar tareas complejas:
- Procesar preguntas con contexto
- Recuperar datos externos vía API
- Almacenar y consultar memoria semántica (con bases vectoriales)
- Encadenar decisiones y acciones de forma dinámica

---

✅ Los agentes de IA son ideales para construir asistentes inteligentes, bots de soporte, automatización de tareas y sistemas de recomendación avanzados.

---

## 🧠 RAG (Retrieval-Augmented Generation) y Bases de Datos Vectoriales

### 🔍 ¿Qué es RAG?

**RAG (Retrieval-Augmented Generation)** es una técnica que combina modelos de lenguaje (como GPT) con bases de datos externas para mejorar la calidad de las respuestas generadas. En lugar de depender únicamente del conocimiento interno del modelo, RAG **recupera información relevante desde una base de datos vectorial** y la utiliza como contexto adicional para la generación de texto.

Esto permite que los agentes de IA respondan con información más precisa, actualizada y específica para cada caso.

---

### 📦 ¿Qué es una Base de Datos Vectorial?

Una **base de datos vectorial** almacena información en forma de vectores multidimensionales, que representan el significado semántico de textos, imágenes, audios, etc. Esto permite hacer **búsquedas por similitud**, encontrando contenido relacionado aunque no coincida textualmente.

Algunos ejemplos de bases de datos vectoriales:
- [FAISS](https://github.com/facebookresearch/faiss)
- [Pinecone](https://www.pinecone.io/)
- [Weaviate](https://weaviate.io/)
- [Qdrant](https://qdrant.tech/)
- [Chroma](https://www.trychroma.com/)

---

### ⚙️ ¿Cómo se usan juntos?

1. El input del usuario se transforma en un **embedding** (vector semántico).
2. Se consulta la base vectorial para **recuperar información relacionada**.
3. Esa información se **inyecta como contexto** en el prompt del modelo de lenguaje.
4. El modelo genera una respuesta basada en ese contexto enriquecido.

---

✅ Esto es especialmente útil para:
- Respuestas con conocimiento actualizado.
- Chatbots con memoria semántica.
- Búsqueda inteligente en documentos.
- Asistentes de soporte o FAQ automáticos.
