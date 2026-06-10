# Chequeo de IA para empresas

Quiz interactivo de **10 preguntas / 3 minutos** que mide qué tan preparada está una empresa para aprovechar la inteligencia artificial. Al terminar, el usuario ve su puntaje (0–100), su nivel de madurez y su mayor "fuga" de tiempo y dinero por área.

🔗 **En vivo:** https://moneyrelax.github.io/chequeo-ia/

---

## ¿Qué hace?

- Evalúa la empresa en **5 dimensiones**: Procesos, Información, Equipo, Herramientas y Claridad.
- Calcula un **puntaje de preparación** y ubica al negocio en uno de 4 niveles: *En riesgo manual → Despertando → Lista para la IA → Avanzada*.
- Identifica la **dimensión más débil** y muestra un mensaje de diagnóstico personalizado.
- Captura el lead y abre **WhatsApp** con un mensaje prellenado para pedir el diagnóstico completo.
- (Opcional) Registra las respuestas en **Google Sheets** vía Apps Script.

## Cómo funciona

Es una sola página estática (`index.html`) — HTML, CSS y JavaScript, sin dependencias ni backend. Toda la lógica del quiz, el puntaje y la redirección a WhatsApp corre en el navegador.

## Configuración

Dentro de `index.html`, en la sección `CONFIGURACIÓN` del `<script>`:

| Variable | Para qué sirve |
|----------|----------------|
| `WHATSAPP` | Número de WhatsApp Business (solo dígitos, con indicativo de país). |
| `ENDPOINT` | URL del Web App de Google Apps Script para guardar respuestas. Si se deja vacío, la página funciona igual y los datos llegan por el mensaje de WhatsApp. |

## Despliegue

Publicado con **GitHub Pages** (rama `main`, carpeta raíz). Cualquier cambio sobre `index.html` en `main` se publica automáticamente en la URL de arriba.

## Licencia

Uso interno. Hecho por David · Consultoría práctica de IA para empresas en Colombia.
