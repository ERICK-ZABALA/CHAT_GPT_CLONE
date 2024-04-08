# JavaScript ChatGPT Clone

Este es un clon simple de una interfaz de chat que utiliza la API de OpenAI GPT para generar respuestas automáticas. Este documento README explica la estructura y los elementos principales del código HTML proporcionado.

## Estructura del HTML

El archivo HTML sigue una estructura básica con dos secciones principales: `side-bar` y `main`.

### Sección `side-bar`

La sección `side-bar` contiene un botón para iniciar un nuevo chat y una sección para mostrar el historial de chat. También incluye un pequeño aviso para dar crédito al creador del proyecto.

```html
<section class="side-bar"> 
    <button>New chat</button>
    <div class="history"></div>
    <dnav>
        <p>Made by Ania</p>
    </nav>
</section>
```
Sección main
La sección main es donde se muestra el chat en sí. Incluye un título, un contenedor para la salida del chat, un área para escribir mensajes y un botón para enviar el mensaje.
```html
<section class="main"> 
    <h1>Erick GPT</h1>
    <p id="output"></p>
    <div class="bottom-section">
        <div class="input-container">
            <input/>
            <div id="submit">▶</div>
        </div>
    </div>
    <p class="info">Chat GPT April Version. Free Research Preview.
        Our goal is to make AI system more natural and safe to interact with.
        Your feedback will help us improve.
    </p>
</section>
```

# JavaScript ChatGPT Clone

Este es un proyecto que implementa un clon simple de una interfaz de chat utilizando la API de OpenAI GPT para generar respuestas automáticas. A continuación se explica el código JavaScript proporcionado.

## Variables Globales

- `OPENAI_API_KEY`: Esta variable almacena la clave de API de OpenAI. Asegúrate de reemplazar `'sk-XXXXXXX'` con tu propia clave de API.

- `submitButton`: Selecciona el botón de envío del mensaje del HTML.

- `outputElement`: Selecciona el elemento HTML donde se mostrarán las respuestas del chat.

- `inputElement`: Selecciona el elemento HTML de entrada de texto donde los usuarios escriben sus mensajes.

- `historyElement`: Selecciona el elemento HTML que contiene el historial de mensajes del chat.

- `buttonElement`: Selecciona el botón HTML para borrar el contenido del campo de entrada.

## Funciones

- `changeInput(value)`: Esta función actualiza el valor del campo de entrada con el valor pasado como argumento.

- `getMessage()`: Esta función maneja el evento de clic en el botón de envío del mensaje. Realiza una solicitud a la API de OpenAI con el mensaje del usuario y actualiza la salida del chat con la respuesta recibida. También agrega el mensaje del usuario al historial de mensajes.

- `clearInput()`: Esta función limpia el campo de entrada, estableciendo su valor en una cadena vacía.

## Event Listeners

- `submitButton.addEventListener('click', getMessage)`: Este event listener se activa cuando se hace clic en el botón de envío del mensaje. Llama a la función `getMessage()` para procesar y enviar el mensaje del usuario.

- `buttonElement.addEventListener('click', clearInput)`: Este event listener se activa cuando se hace clic en el botón para borrar el contenido del campo de entrada. Llama a la función `clearInput()` para limpiar el campo de entrada.

---

Archivos Adjuntos

+ styles.css: Se espera que este archivo contenga estilos para la interfaz de chat.
+ app.js: Este archivo se encargará de la lógica del chat y la integración con la API de OpenAI.

