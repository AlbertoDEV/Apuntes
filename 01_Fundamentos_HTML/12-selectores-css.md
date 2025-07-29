# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 3. Selectores básicos: Por etiqueta, clase (`.clase`), ID (`#id`)

Los **selectores CSS** son las instrucciones que le dices a tu navegador para que sepa exactamente a qué elementos HTML aplicar los estilos. Son la forma en que indicas "quiero estilizar *este* elemento" o "quiero estilizar *todos estos* elementos".

Aquí están los selectores más fundamentales que usarás constantemente:

1.  **Selector por Etiqueta (o Tipo):**
    * **¿Cómo funciona?** Selecciona **todos los elementos** de un tipo de etiqueta HTML específico.
    * **Sintaxis:** Simplemente escribes el nombre de la etiqueta HTML.
    * **Cuándo usarlo:** Cuando quieres aplicar el mismo estilo a todos los elementos de un tipo (ej., todos los párrafos, todos los encabezados `h1`).
    * **Ejemplo:**
        ```css
        p { /* Selecciona todos los elementos <p> */
            font-family: Arial, sans-serif; /* Cambia la fuente de todos los párrafos */
            line-height: 1.6; /* Aumenta el espaciado entre líneas */
        }

        h1 { /* Selecciona todos los elementos <h1> */
            text-align: center; /* Centra el texto del encabezado */
            color: #333; /* Color de texto gris oscuro */
        }
        ```
    * **Analogía:** Es como decir "Todas las sillas de la casa deben ser rojas".

2.  **Selector por Clase (`.clase`):**
    * **¿Cómo funciona?** Selecciona **todos los elementos** que tienen un atributo `class` específico. Puedes aplicar la misma clase a múltiples elementos HTML, y un elemento HTML puede tener múltiples clases.
    * **Sintaxis:** Un punto (`.`) seguido del nombre de la clase.
    * **Cuándo usarlo:** ¡Muy común y potente! Cuando quieres aplicar un estilo a un **grupo de elementos que comparten una característica visual o funcional**, sin importar su tipo de etiqueta.
    * **Ejemplo (HTML):**
        ```html
        <p class="resaltado">Este párrafo es importante.</p>
        <span class="resaltado">Esta parte del texto también se resalta.</span>
        <h2 class="resaltado">Un título resaltado</h2>
        ```
    * **Ejemplo (CSS):**
        ```css
        .resaltado { /* Selecciona todos los elementos con la clase "resaltado" */
            background-color: yellow; /* Fondo amarillo */
            font-weight: bold; /* Texto en negrita */
        }
        ```
    * **Analogía:** "Todos los muebles que tengan una etiqueta 'vintage' deben ser de madera oscura".

3.  **Selector por ID (`#id`):**
    * **¿Cómo funciona?** Selecciona un **único elemento** HTML que tiene un atributo `id` específico.
    * **Sintaxis:** Una almohadilla (`#`) seguida del valor del `id`.
    * **Cuándo usarlo:** Cuando quieres aplicar un estilo a un **elemento muy específico y único** en tu página (¡cada `id` debe ser único en todo el documento HTML!).
    * **Ejemplo (HTML):**
        ```html
        <div id="encabezado-principal">
            <h1>Bienvenido a mi sitio</h1>
            <p>Un subtítulo interesante.</p>
        </div>

        <button id="boton-compra">Comprar ahora</button>
        ```
    * **Ejemplo (CSS):**
        ```css
        #encabezado-principal { /* Selecciona el elemento con el ID "encabezado-principal" */
            border-bottom: 2px solid grey; /* Un borde inferior */
            padding: 20px; /* Relleno alrededor del contenido */
        }

        #boton-compra {
            background-color: green;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
        }
        ```
    * **Analogía:** "El sofá individual de la sala debe ser de cuero".

---

**Resumen rápido:**
* **Etiqueta:** Para todos los elementos de un tipo (`p`, `h1`, `div`).
* **Clase:** Para grupos de elementos que comparten un estilo (`.btn`, `.card`, `.error`). ¡Muy flexible y el más usado!
* **ID:** Para un único elemento específico (`#main-header`, `#sidebar`).
