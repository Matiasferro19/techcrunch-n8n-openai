🚀 ¿Qué hace este workflow?

El workflow realiza todo este proceso de principio a fin:

Schedule Trigger
Activa el flujo automáticamente en el horario configurado.

HTTP Request a TechCrunch Latest
Obtiene las últimas noticias desde:
https://techcrunch.com/latest/

AI Agent (GPT-5 mini)

Traduce todas las noticias al español.

Resume el contenido.

Genera un listado en HTML limpio y ordenado.

Mantiene los links originales para que las noticias sean clickeables.

Formato de fecha
Se genera la fecha actual ({{$now}}) para mostrarla en el encabezado del email.

Render del email en HTML
Se inserta el contenido generado por IA dentro de un diseño HTML personalizado con título, fecha y estilos básicos.

Gmail Node – Envío del correo
Envía automáticamente el newsletter a la casilla configurada.

🧠 Modelo de IA utilizado

Se utilizó:
GPT-5 mini, integrado mediante el nodo OpenAI Model en n8n, configurado para:

Traducción

Resumen

Generación de HTML

Preservación de enlaces

👉 Agregá aquí tu screenshot del modelo usado.

📸 Screenshots
🔧 1. Workflow completo

(Insertar imagen del flujo completo)

🧠 2. Prompt utilizado en IA

(Insertar screenshot del prompt del AI Agent / OpenAI Model)

🤖 3. Modelo utilizado (GPT-5 mini)

(Insertar screenshot del nodo del modelo)

✉️ 4. Email generado (con noticia clickeada)

(Insertar screenshot del mail, con flecha indicando link clickeable)

🌐 5. Noticia en TechCrunch

(Insertar screenshot de la noticia original en la web)

📌 Nota sobre fechas

La fecha que aparece en el email corresponde al día del envío, mientras que las fechas de publicación de cada noticia se mantienen según el sitio original (TechCrunch).
Esto es normal en newsletters y mejora la claridad del contenido.

🛠️ Tecnologías utilizadas

n8n (automatización del flujo)

OpenAI (GPT-5 mini)

HTML inline para emails

Gmail API

HTTP Scraping desde TechCrunch

🎯 Objetivo del proyecto

Este workflow sirve como:

Ejemplo real de automatización con n8n

Integración práctica de IA en procesos diarios

Proyecto de portfolio para mostrar habilidades en:

APIs

Autonomía de agentes

HTML dinámico

IA aplicada a contenido

Automatizaciones reales

📁 Export del workflow

El archivo workflow.json está incluido en este repositorio para que puedas importarlo directamente en n8n.
