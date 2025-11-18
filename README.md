📰 Newsletter Automático con n8n + IA

Automatización completa que obtiene noticias de TechCrunch, las traduce, resume y envía un newsletter limpio y moderno usando n8n + OpenAI.

⚙️ Flujo del proceso
1️⃣ Schedule Trigger (Disparador de horario)

Activa el flujo automáticamente en el horario configurado.

2️⃣ HTTP Request – TechCrunch Latest

Obtiene las últimas noticias desde:
https://techcrunch.com/latest

3️⃣ AI Agent – Modelo GPT-5 mini

El modelo realiza:

Traducción al español

Resumen del contenido

Generación de HTML ordenado

Preservación de enlaces clickeables

4️⃣ Formato de fecha

Se genera la fecha actual ({{$now}}) para mostrarla en el encabezado del email.

5️⃣ Render del Email en HTML

Inserta el contenido generado por IA dentro de un diseño HTML personalizado con título, fecha y estilo.

6️⃣ Gmail Node – Envío automático

Envía el newsletter final a la casilla configurada.

🧠 Modelo de IA utilizado

Se utilizó GPT-5 mini, integrado mediante el nodo OpenAI Model en n8n.

Funciones configuradas:

Traducción

Resumen

Generación HTML

Enlaces preservados

📌 Screenshot del modelo utilizado:


📸 Screenshots
🔧 1. Workflow completo

![Workflow](screenshots/Workflow.png)

🧠 2. Prompt utilizado para la IA

🤖 3. Configuración del modelo GPT-5 mini

✉️ 4. Email generado (con links clickeables)

🌐 5. Noticia original en TechCrunch

📌 Nota sobre las fechas

La fecha del email es la del envío.

Las fechas de cada noticia provienen del sitio original (TechCrunch).

Esto es completamente normal y mantiene la integridad del contenido.

🛠️ Tecnologías utilizadas

n8n (automatización del flujo)

OpenAI – GPT-5 mini

HTML inline para emails

Gmail API

HTTP Scraping / API de TechCrunch

🎯 Objetivo del proyecto

Este workflow sirve como:

Proyecto de portfolio

Ejemplo real de automatización

Caso práctico de IA aplicada

Integración de APIs

Envío automático de newsletters

📁 Export del workflow

El archivo workflow.json está incluido en este repositorio para importarlo directamente en n8n.
