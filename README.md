# Mis Agentes IA

App web estática (un solo `Index.html`) para crear agentes de IA y chatear con ellos.

## Modelos (todos open-source)
- **En el navegador (por defecto):** Qwen2.5 / Llama 3.2 vía WebLLM + WebGPU. Gratis, privado, sin key ni servidor.
- **Groq / OpenRouter / DeepSeek:** el usuario pega su propia API key en Ajustes (se guarda solo en su navegador).
- **Ollama / servidor compatible OpenAI:** URL personalizada.

## Agentes funcionales
Cada agente puede activar herramientas: calculadora, fecha y hora, Wikipedia. El agente decide cuándo usarlas.

## Publicar
Es un sitio estático: súbelo a GitHub Pages, Netlify o Vercel (Settings → Pages → rama de esta carpeta).

## Seguridad
Nunca pongas una API key en el código. Una key anterior estuvo en el historial del repo: **revócala** en platform.deepseek.com.

## Compatibilidad con otras apps de IA
Botón ⇪ en cada agente:
- **Prompt** para pegar en ChatGPT / Claude / Gemini (o abrirlo directo en ChatGPT y Claude).
- **JSON portable** (`.agent.json`) con system prompt y herramientas en formato OpenAI function-calling.
- **cURL** listo para cualquier API compatible con OpenAI.
- **Enlace** para compartir: quien lo abra puede importar el agente.

Botón "Importar agente": acepta nuestro JSON, JSON de estilo OpenAI, un enlace compartido o un prompt de texto.

## Inspirado en
- **Open WebUI**: agentes = modelo + prompt + parámetros + conocimiento. Aquí: creatividad (temperature), base de conocimiento con recuperación ligera (BM25-lite; inyecta todo si es pequeña, o los fragmentos más relevantes) y variables `{{FECHA}} {{HORA}} {{DIA}}`.
- **LobeChat**: galería de agentes listos para añadir con un clic.
- Chat con markdown seguro, copiar respuesta y regenerar.
