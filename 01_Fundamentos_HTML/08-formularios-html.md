# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 8. Formularios: Elementos básicos de formulario (`<form>`, `<input>`, `<button>`, `<label>`)

Los **formularios** son la forma en que los usuarios pueden enviar información a un sitio web. Piensa en cualquier momento que has rellenado un campo de búsqueda, te has registrado en una página, has dejado un comentario o has iniciado sesión. ¡Todo eso se hace con formularios! Son como las "ventanillas" o "puertas de entrada" de datos en tu sitio web.

Para construir un formulario básico, necesitas varias etiquetas clave:

* **`<form>`**:
    * Esta es la etiqueta contenedora principal para todo el formulario. Todo lo que forma parte del formulario (campos de texto, botones, casillas, etc.) va dentro de esta etiqueta.
    * Tiene atributos importantes como `action` (a dónde se envían los datos cuando el formulario es enviado) y `method` (cómo se envían los datos, usualmente `GET` o `POST`). Por ahora, nos centraremos en los elementos internos.

* **`<input>`**:
    * Esta es una de las etiquetas más versátiles y comunes. Se usa para crear diferentes tipos de **campos de entrada** de datos, dependiendo del atributo `type`. Es una etiqueta de auto-cierre, al igual que `<img>`.
    * **Atributo `type`**: Esto define el tipo de entrada que el usuario puede proporcionar. Algunos de los tipos más comunes son:
        * `text`: Para una línea de texto simple (ej., nombre, dirección).
            ```html
            <input type="text">
            ```
        * `password`: Para contraseñas (el texto se oculta).
            ```html
            <input type="password">
            ```
        * `email`: Para direcciones de correo electrónico (los navegadores pueden validar el formato).
            ```html
            <input type="email">
            ```
        * `number`: Para números.
            ```html
            <input type="number">
            ```
        * `checkbox`: Para selecciones de sí/no o múltiples opciones.
            ```html
            <input type="checkbox">
            ```
        * `radio`: Para seleccionar una sola opción de un grupo. (Necesitan un atributo `name` común para agruparse).
            ```html
            <input type="radio" name="genero" value="masculino">
            <input type="radio" name="genero" value="femenino">
            ```
        * `submit`: Un botón para enviar el formulario.
            ```html
            <input type="submit" value="Enviar">
            ```
* **`<button>`**:
    * Se usa para crear botones. Aunque `input type="submit"` crea un botón de envío, `<button>` es más flexible porque puedes poner texto o incluso imágenes dentro de él.
    * Para que un botón envíe un formulario, su atributo `type` debe ser `submit` (es el valor por defecto si está dentro de un `<form>`).
    ```html
    <button type="submit">Enviar Formulario</button>
    ```

* **`<label>`**:
    * Esta etiqueta es **fundamental para la accesibilidad** y una buena práctica. Asocia un texto descriptivo a un control de formulario (como un `<input>`).
    * Para asociar un `<label>` a un `<input>`, debes darle un `id` único al `<input>` y luego usar ese `id` como valor del atributo `for` en el `<label>`.
    * Cuando el usuario hace clic en la etiqueta, el campo de entrada asociado se enfoca.
    * **Ejemplo:**
        ```html
        <label for="nombreUsuario">Nombre de Usuario:</label>
        <input type="text" id="nombreUsuario">
        ```
        Aquí, el `label` "Nombre de Usuario:" está asociado al `<input>` con `id="nombreUsuario"`.

---

**Ejemplo completo de un formulario simple:**

```html
<h2>Registro de Usuario</h2>
<form action="/procesar_registro" method="POST">
    <label for="nombre">Nombre:</label><br>
    <input type="text" id="nombre" name="nombre"><br><br>

    <label for="email">Email:</label><br>
    <input type="email" id="email" name="email"><br><br>

    <label for="password">Contraseña:</label><br>
    <input type="password" id="password" name="password"><br><br>

    <input type="checkbox" id="acepto" name="acepto_terminos">
    <label for="acepto">Acepto los términos y condiciones</label><br><br>

    <button type="submit">Registrarme</button>
</form>
