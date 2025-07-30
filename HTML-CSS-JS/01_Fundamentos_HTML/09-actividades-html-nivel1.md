# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 🏗️ Guía de Actividades de HTML (Nivel 1)

El objetivo de estas actividades es que combines varios de los conceptos que hemos visto para crear páginas web funcionales.

---

### Actividad 1: Crear tu primera página web simple con texto, imágenes y enlaces

El objetivo es integrar la estructura básica, encabezados, párrafos, enlaces e imágenes.

**Pasos a seguir:**

1.  **Crea tu archivo:**
    * Abre tu editor de código.
    * Crea un nuevo archivo y guárdalo como `mi-primera-web.html` en una carpeta dedicada.
    * Dentro de esa misma carpeta, crea una subcarpeta llamada `imagenes` (o `assets`) para tus imágenes.

2.  **Estructura básica:**
    * Comienza con la estructura HTML que aprendimos (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`).
    * Dale un `title` significativo a tu página (ej. "Mi Primera Página de Viajes").

    ```html
    <!DOCTYPE html>
    <html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Mi Primera Página de Viajes</title>
    </head>
    <body>
        </body>
    </html>
    ```

3.  **Añade texto con encabezados y párrafos:**
    * Dentro del `<body>`, usa un `<h1>` para el título principal.
    * Añade un `<h2>` o `<h3>` para una subsección.
    * Escribe al menos dos `<p>` con texto relevante. Usa `<strong>` y `<em>` en algunas palabras.

4.  **Inserta una imagen:**
    * Busca una imagen y **cópiala a tu carpeta `imagenes`**.
    * Inserta la imagen con `<img>`. Asegúrate de que la ruta en `src` sea correcta (ej., `imagenes/tokio.jpg`) y, **muy importante**, ¡ponle un `alt` descriptivo!

    ```html
    <img src="imagenes/tokio.jpg" alt="Un bullicioso cruce peatonal en Tokio de noche">
    ```

5.  **Crea al menos un enlace:**
    * Añade un enlace (`<a>`) a otra página web (ej., Wikipedia). No olvides el atributo `href`.
    * Puedes añadir un `target="_blank"` para que se abra en una nueva pestaña si es un enlace externo.

    ```html
    <p>Si quieres saber más sobre este destino, visita <a href="[https://es.wikipedia.org/wiki/Tokio](https://es.wikipedia.org/wiki/Tokio)" target="_blank">Wikipedia</a>.</p>
    ```

6.  **Guarda y visualiza:**
    * Guarda tu archivo HTML.
    * Abre el archivo directamente en tu navegador.
    * ¡Felicidades, acabas de crear tu primera página web!

---

### Actividad 2: Construir un formulario de contacto básico

Ahora, permite que la gente te contacte con un formulario básico.

**Pasos a seguir:**

1.  **Crea tu archivo (o añade a uno existente):**
    * Puedes crear un nuevo archivo `contacto.html` en la misma carpeta que `mi-primera-web.html`.
    * Asegúrate de tener la estructura HTML básica.

2.  **Define el formulario:**
    * Dentro del `<body>`, comienza con la etiqueta `<form>`. Por ahora, puedes dejar los atributos `action` y `method` vacíos o con `#`.

    ```html
    <form action="#" method="POST">
        </form>
    ```

3.  **Añade un campo de texto para el nombre:**
    * Usa una etiqueta `<label>` para "Nombre:".
    * Asóciala a un `<input type="text">` usando el atributo `for` y un `id` único.

    ```html
    <label for="nombre">Nombre:</label><br>
    <input type="text" id="nombre" name="nombre"><br><br>
    ```

4.  **Añade un campo de email:**
    * Usa `label` para "Email:".
    * Asóciala a un `<input type="email">`.

    ```html
    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email"><br><br>
    ```

5.  **Añade un campo de mensaje (área de texto multi-línea):**
    * Usa la etiqueta `<textarea>` para mensajes largos.
    * Asóciala con un `<label>`.

    ```html
    <label for="mensaje">Tu Mensaje:</label><br>
    <textarea id="mensaje" name="mensaje" rows="5" cols="30"></textarea><br><br>
    ```
    *(`rows` y `cols` controlan el tamaño visible del área de texto, puedes ajustarlos).*

6.  **Añade un botón de envío:**
    * Usa un `<button type="submit">` con un texto como "Enviar Mensaje".

    ```html
    <button type="submit">Enviar Mensaje</button>
    ```

7.  **Guarda y visualiza:**
    * Guarda tu archivo HTML.
    * Abre el archivo en tu navegador para ver el formulario.
