# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 3. Etiquetas de texto: Encabezados (`<h1>` a `<h6>`), párrafos (`<p>`), negrita (`<strong>`), cursiva (`<em>`)

Ahora que sabemos qué es HTML y cómo se estructura un documento básico, ¡es hora de ponerle contenido! Las **etiquetas de texto** son como las herramientas básicas de escritura en la web. Te permiten organizar y dar formato al texto para que no sea solo un "mazacote" ilegible.

Piensa en un periódico o una revista: tienen titulares grandes, subtítulos más pequeños, párrafos de texto, palabras destacadas en negrita o cursiva. Las etiquetas HTML nos permiten hacer lo mismo en nuestras páginas web.

Aquí están las más comunes y su función:

* **Encabezados (`<h1>` a `<h6>`)**:
    * Sirven para definir **títulos y subtítulos**.
    * `<h1>` es el más importante (el título principal de tu página o sección), y `<h6>` es el menos importante. Imagina que `<h1>` es el titular de un periódico y `<h6>` es un subtítulo muy pequeño.
    * No solo cambian el tamaño visual del texto, sino que son **semánticamente importantes** para los motores de búsqueda y la accesibilidad (le dicen a los lectores de pantalla que esa es una sección importante). ¡No los uses solo para hacer el texto más grande!
    * **Ejemplo:**
        ```html
        <h1>Mi Blog de Viajes</h1>
        <h2>Mis Aventuras por Asia</h2>
        <h3>Un día en Tokio</h3>
        ```

* **Párrafos (`<p>`)**:
    * Es la etiqueta más básica para **texto regular** o bloques de contenido.
    * Cada vez que quieras escribir un párrafo de texto, usa la etiqueta `<p>`. El navegador automáticamente le dará un poco de espacio arriba y abajo para separarlo de otros elementos.
    * **Ejemplo:**
        ```html
        <p>Hoy visité el famoso cruce de Shibuya, ¡fue increíble ver a tanta gente!</p>
        <p>Después, disfruté de un delicioso ramen en un pequeño local tradicional.</p>
        ```

* **Negrita (`<strong>`)**:
    * Se usa para darle **énfasis fuerte** a una parte del texto. Significa que ese contenido es **importante**.
    * Aunque visualmente hace el texto negrita, su propósito principal es indicar la importancia del texto, no solo su apariencia.
    * **Ejemplo:**
        ```html
        <p>Asegúrate de llevar tu <strong>pasaporte</strong> cuando viajes.</p>
        ```

* **Cursiva (`<em>`)**:
    * Se usa para dar **énfasis de énfasis** (¡valga la redundancia!), como un énfasis tonal o para una palabra clave que quieres destacar. Piensa en el énfasis que le darías a una palabra al hablar.
    * Aunque visualmente hace el texto cursiva, su propósito es el énfasis, no solo la apariencia.
    * **Ejemplo:**
        ```html
        <p>Ella susurró: "Necesito que me escuches <em>atentamente</em>".</p>
        ```
