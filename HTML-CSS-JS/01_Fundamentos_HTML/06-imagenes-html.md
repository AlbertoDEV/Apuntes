# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 6. Imágenes: Cómo insertar imágenes (`<img>`) en tu página

Una página web sin imágenes sería bastante aburrida, ¿verdad? Las imágenes son esenciales para hacer que tu contenido sea visualmente atractivo, transmitir información de manera rápida y mejorar la experiencia del usuario. Piensa en ellas como las fotografías y los dibujos que acompañan al texto en un libro o una revista.

La etiqueta que usamos para insertar imágenes es `<img>`. A diferencia de otras etiquetas que hemos visto, como `<p>` o `<h1>`, la etiqueta `<img>` es una **etiqueta vacía** o de **auto-cierre**. Esto significa que no necesita una etiqueta de cierre como `</img>` porque no envuelve contenido; su información se define a través de **atributos**.

Los atributos más importantes de la etiqueta `<img>` son:

* **`src` (source - fuente):** Este es el atributo fundamental. Le dice al navegador dónde encontrar el archivo de la imagen. El valor de `src` es la **ruta** a la imagen, que puede ser:
    * Una URL completa de una imagen en internet (por ejemplo, `https://ejemplo.com/imagen.jpg`).
    * Una ruta a una imagen que tienes guardada en tu propio proyecto (por ejemplo, `imagenes/mi-foto.jpg`). Es una buena práctica crear una carpeta `imagenes` o `assets` para organizarlas.
* **`alt` (alternative text - texto alternativo):** Este atributo es **crucial** y no debe omitirse. Proporciona una descripción textual de la imagen. Es importante por varias razones:
    * **Accesibilidad:** Los lectores de pantalla para personas con discapacidad visual leen este texto, permitiéndoles entender el contenido de la imagen.
    * **SEO (Optimización para Motores de Búsqueda):** Ayuda a los motores de búsqueda a entender de qué trata tu imagen, lo que puede mejorar la visibilidad de tu página.
    * **Fallback:** Si la imagen no se carga (por un error en la ruta, problema de conexión, etc.), este texto se mostrará en su lugar, informando al usuario de qué debería haber ahí.
    * Piensa en el `alt` como una pequeña descripción que le darías a alguien por teléfono sobre la imagen que estás viendo.

* **`width` y `height` (ancho y alto):** Estos atributos permiten especificar el ancho y el alto de la imagen en píxeles. Aunque son útiles para reservar espacio y evitar "saltos" en la página, **generalmente es mejor controlar el tamaño de las imágenes con CSS** para tener más flexibilidad y capacidad de respuesta. Sin embargo, para empezar, puedes usarlos.

* **Ejemplos de Imágenes:**

    1.  **Insertar una imagen local:**
        Si tienes una imagen llamada `paisaje.jpg` en una carpeta `assets` al mismo nivel que tu archivo HTML, el código sería:
        ```html
        <img src="assets/paisaje.jpg" alt="Un hermoso paisaje montañoso al atardecer">
        ```

    2.  **Insertar una imagen desde una URL externa:**
        ```html
        <img src="[https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)" alt="Logo de Google">
        ```

    3.  **Imagen con ancho y alto específicos (ejemplo, aunque CSS es preferible):**
        ```html
        <img src="assets/icono.png" alt="Un pequeño icono de un rayo" width="50" height="50">
        ```

Recuerda que el `alt` es tan importante como el `src`. ¡No lo olvides!
