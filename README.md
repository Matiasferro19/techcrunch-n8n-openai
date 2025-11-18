📰 Newsletter Automático con n8n + IA

El workflow realiza todo este proceso de principio a fin:

⚙️ Flujo del proceso

Schedule Trigger
Activa el flujo automáticamente en el horario configurado.

HTTP Request a TechCrunch Latest
Obtiene las últimas noticias desde:
https://techcrunch.com/latest

AI Agent (GPT-5 mini)

Traduce todas las noticias al español

Resume el contenido

Genera un listado en HTML limpio y ordenado

Mantiene los links originales clickeables

Formato de fecha
Se genera la fecha actual ({{$now}}) para mostrarla en el encabezado del email.

Render del email en HTML
Se inserta el contenido generado por IA dentro de un diseño HTML personalizado.

Gmail Node – Envío automático
Envía el newsletter a la casilla configurada.

🧠 Modelo de IA utilizado

Se utilizó GPT-5 mini, integrado mediante el nodo OpenAI Model en n8n, configurado para:

Traducción

Resumen

Generación de HTML

Preservación de enlaces

📌 Screenshot del modelo usado:

📸 Screenshots
🔧 1. Workflow completo

![Workflow](screenshots/Workflow.png)

🧠 2. Prompt utilizado en IA

![Prompt](screenshots/PromptIA1.png)


🤖 3. Modelo utilizado (GPT-5 mini)

![ModeloIA](screenshots/ModeloIA.png)

✉️ 4. Email generado (con link clickeable)

![Email](screenshots/Email.png)

🌐 5. Noticia en TechCrunch (original)

![Noticia](screenshots/NoticiaWeb.png)

📌 Nota sobre las fechas

La fecha que aparece en el email corresponde al día del envío.

Las fechas de las noticias son las del sitio original (TechCrunch).

Esto es normal en newsletters y mejora la claridad del contenido.

🛠️ Tecnologías utilizadas

n8n (automatización del flujo)

OpenAI – GPT-5 mini

HTML inline para emails

Gmail API

HTTP Scraping / API TechCrunch

🎯 Objetivo del proyecto

Este workflow es ideal como:

Proyecto de portfolio

Ejemplo real de automatización

Integración práctica de IA

Uso de APIs + node flows

Envío masivo automatizado de newsletters

📁 Export del workflow

El archivo workflow.json está incluido en este repositorio para importarlo directamente en n8n.
