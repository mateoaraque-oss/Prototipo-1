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
