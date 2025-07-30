# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 7. Display: `block`, `inline`, `inline-block` (controlando cómo se muestran los elementos)

La propiedad `display` es como la "regla de comportamiento" de tus elementos HTML. Define cómo un elemento se muestra en el navegador, cómo interactúa con el espacio a su alrededor y cómo se relaciona con otros elementos. Comprender `display` es fundamental para el **layout** (diseño y disposición) de tu página.

Existen muchos valores para `display`, pero en este nivel, nos centraremos en los tres más básicos y comunes: `block`, `inline` e `inline-block`.

1.  **`display: block;`**
    * **Comportamiento:**
        * Cada elemento `block` ocupa su propia "línea completa" en la página. Es decir, siempre comienza en una nueva línea y se extiende por todo el ancho disponible por defecto (a menos que le especifiques un `width`).
        * Los elementos `block` respetan `width`, `height`, `margin` y `padding`.
        * Siempre se apilan verticalmente, uno encima del otro.
    * **Analogía:** Piensa en un **párrafo en un documento Word**. Cada párrafo empieza en una nueva línea y ocupa todo el ancho de la página.
    * **Ejemplos de elementos HTML que son `block` por defecto:**
        * `<div>`
        * `<h1>` a `<h6>`
        * `<p>`
        * `<ul>`, `<ol>`, `<li>`
        * `<form>`
    * **Ejemplo CSS:**
        ```css
        .mi-div {
            background-color: lightcoral;
            width: 200px; /* Aquí le das un ancho, sino ocuparía el 100% */
            height: 100px;
            margin: 10px;
        }
        ```

2.  **`display: inline;`**
    * **Comportamiento:**
        * Los elementos `inline` solo ocupan el **espacio que necesitan para su contenido**. No fuerzan una nueva línea; se colocan uno al lado del otro, como palabras en una frase.
        * **No respetan `width` ni `height`** que les asignes (se ignorarán).
        * Solo respetan `margin-left` y `margin-right` y `padding-left` y `padding-right`. Los `margin-top` y `margin-bottom` así como `padding-top` y `padding-bottom` se ignoran o se aplican de forma muy limitada y no empujan elementos vecinos.
    * **Analogía:** Piensa en **palabras individuales en una frase**. No inician una nueva línea a menos que se acabe el espacio.
    * **Ejemplos de elementos HTML que son `inline` por defecto:**
        * `<span>`
        * `<a>` (enlaces)
        * `<strong>`, `<em>`
        * `<img>` (aunque tiene algunas características especiales en cuanto a su tamaño)
    * **Ejemplo CSS:**
        ```css
        .enlace-inline {
            background-color: lightgreen;
            padding: 5px; /* Solo padding izquierdo y derecho se verán bien */
            /* width: 100px; <--- Esto no funcionaría */
        }
        ```

3.  **`display: inline-block;`**
    * **Comportamiento:**
        * Es una mezcla de ambos: se comporta como un `inline` (se coloca uno al lado del otro en la misma línea), pero **también respeta `width`, `height`, `margin` y `padding`** como un `block`.
        * Comienza en la misma línea que el contenido previo y siguiente.
    * **Analogía:** Imagina varias **fotos pequeñas en una galería**, colocadas una al lado de la otra, pero cada una con su propio marco (`margin`/`padding`) y tamaño definidos.
    * **Cuándo usarlo:** Ideal para elementos que quieres que estén uno al lado del otro, pero que también necesitas controlar su tamaño y espaciado vertical. Por ejemplo, botones de navegación, iconos con texto, o elementos de un menú horizontal.
    * **Ejemplo CSS:**
        ```css
        .boton-menu {
            display: inline-block; /* Se pone al lado de otros, pero permite ancho/alto/margen */
            background-color: dodgerblue;
            color: white;
            padding: 10px 15px;
            margin: 5px;
            border-radius: 5px;
            width: 120px; /* Podemos darle un ancho */
            text-align: center;
        }
        ```

---

**Resumen rápido de `display`:**

| Propiedad       | Inicia nueva línea | Acepta `width`/`height` | Acepta `margin`/`padding` (todos los lados) |
| :--------------- | :----------------- | :---------------------- | :---------------------------------------- |
| `block`          | Sí                 | Sí                      | Sí                                        |
| `inline`         | No                 | No                      | Solo horizontal (`left`/`right`)          |
| `inline-block`   | No                 | Sí                      | Sí                                        |
