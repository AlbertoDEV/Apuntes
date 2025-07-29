# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 🏗️ Guía de Actividades de CSS (Nivel 1)

El objetivo de estas actividades es que apliques los conceptos de CSS que hemos visto a tus páginas HTML, transformando su apariencia.

---

### Actividad 1: Estilizar tu página web básica con colores, fuentes y espaciado

Aquí usarás las propiedades de color, fuentes y el Modelo de Caja en tu archivo `mi-primera-web.html`.

**Pasos a seguir:**

1.  **Prepara tu entorno:**
    * Abre tu archivo `mi-primera-web.html` y crea un nuevo archivo en la misma carpeta llamado `estilos.css`.

2.  **Vincula el CSS a tu HTML:**
    * En el `<head>` de `mi-primera-web.html`, añade la etiqueta `<link>`:

    ```html
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Mi Primera Página de Viajes</title>
        <link rel="stylesheet" href="estilos.css"> </head>
    ```

3.  **Aplica estilos generales al `body` (en `estilos.css`):**
    ```css
    body {
        font-family: Arial, sans-serif;
        font-size: 18px;
        background-color: #f4f4f4; /* Un gris muy claro */
        color: #333;
    }
    ```

4.  **Estiliza tus encabezados (en `estilos.css`):**
    * Selecciona tus `<h1>` y `<h2>`.
    * Cambia su `color`, centra el texto de `<h1>` (`text-align: center;`) y añade un `margin-bottom` para separarlos.

5.  **Dale estilo a tus párrafos (en `estilos.css`):**
    * Selecciona los `<p>`.
    * Ajusta el `line-height` (ej., `1.6`) y añade un `margin`.

6.  **Aplica estilos a tu imagen:**
    * Si tu imagen es grande, asígnale una clase en HTML (ej., `<img src="..." alt="..." class="imagen-pagina">`).
    * En tu CSS, selecciona esa clase (`.imagen-pagina`).
    * Asígnale `max-width: 100%;` y `height: auto;`.
    * Añádele un `border` y un `margin`.

7.  **Estiliza tus enlaces (en `estilos.css`):**
    * Selecciona los `<a>`.
    * Cambia su `color` y elimina el subrayado (`text-decoration: none;`).

8.  **Guarda y visualiza:**
    * Guarda ambos archivos y abre `mi-primera-web.html` en tu navegador.

---

### Actividad 2: Diseñar el formulario de contacto usando selectores y el modelo de caja

Ahora vamos a darle una apariencia más agradable a tu formulario de contacto.

**Pasos a seguir:**

1.  **Prepara tu archivo:**
    * Abre tu archivo `contacto.html`. Asegúrate de que también esté enlazado a `estilos.css`.

2.  **Estiliza el contenedor `<form>` (en `estilos.css`):**
    ```css
    form {
        background-color: white;
        padding: 20px;
        border: 1px solid #ddd;
        border-radius: 8px; /* Pequeñas esquinas redondeadas */
        width: 400px;
        margin: 20px auto; /* Centra el formulario y le da margen arriba/abajo */
    }
    ```

3.  **Estiliza las etiquetas (`label`) (en `estilos.css`):**
    * Selecciona la etiqueta `label`.
    * Aplica `display: block;`, añade un `margin-bottom` (ej., `5px`) y cambia el `font-weight` a `bold`.

4.  **Estiliza los campos de entrada (`input` y `textarea`) (en `estilos.css`):**
    * Selecciona `input[type="text"], input[type="email"], input[type="password"], textarea`.
    * Dales un `width: 100%;`, `padding` (ej., `8px`), un `border` y `border-radius`.
    * Añade un `margin-bottom` (ej., `15px`).
    * **Muy importante:** `box-sizing: border-box;`
    ```css
    input[type="text"],
    input[type="email"],
    input[type="password"],
    textarea {
        width: 100%; /* Ocupa el 100% del ancho disponible */
        padding: 8px;
        margin-bottom: 15px;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box; /* Incluye padding y border en el ancho/alto */
    }
    textarea {
        resize: vertical; /* Permite al usuario redimensionar verticalmente */
    }
    ```

5.  **Estiliza el botón de envío (en `estilos.css`):**
    * Selecciona `button[type="submit"]` (o `input[type="submit"]`).
    * Dale un `background-color` llamativo, `color: white;`, `padding` (ej., `10px 15px`).
    * Cambia el cursor a `pointer` (`cursor: pointer;`) y quita el borde (`border: none;`).
    * Puedes añadir un `border-radius`.
    ```css
    button[type="submit"] {
        background-color: #007bff; /* Azul vibrante */
        color: white;
        padding: 10px 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 1em;
    }
    button[type="submit"]:hover { /* Efecto al pasar el ratón */
        background-color: #0056b3;
    }
    ```

6.  **Guarda y visualiza:**
    * Guarda tus archivos HTML y CSS y abre `contacto.html` en el navegador.
