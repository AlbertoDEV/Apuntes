# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 4. Propiedades de texto: Color, tamaño de fuente, tipo de fuente (`font-family`)

Las **propiedades de texto** en CSS son tus herramientas para estilizar todo lo relacionado con la tipografía en tu página web. Podrás cambiar el color, el tamaño y el tipo de letra, haciendo que tu texto sea más legible y visualmente atractivo. ¡Piensa en esto como elegir la pluma, la tinta y el tamaño de la letra para escribir en tu documento!

Aquí te presento las propiedades más importantes para empezar:

1.  **`color`:**
    * **¿Qué hace?** Establece el **color del texto** de un elemento.
    * **Valores:** Puedes usar nombres de colores (como `red`, `blue`), valores hexadecimales (como `#FF0000` para rojo, `#336699` para un azul verdoso), o valores RGB/RGBA (como `rgb(255, 0, 0)` o `rgba(0, 0, 0, 0.5)` para negro con 50% de transparencia).
    * **Ejemplo:**
        ```css
        p {
            color: navy; /* Hace que el texto del párrafo sea azul marino */
        }

        h1 {
            color: #E6B800; /* Un tono de oro para el encabezado */
        }
        ```

2.  **`font-size`:**
    * **¿Qué hace?** Controla el **tamaño del texto**.
    * **Valores comunes:**
        * `px` (píxeles): Un tamaño fijo. (Ej: `16px`).
        * `em`: Relativo al tamaño de fuente del elemento padre. Si el padre tiene `16px`, `1.5em` será `24px`. Es bueno para mantener la escalabilidad.
        * `rem`: Relativo al tamaño de fuente del elemento raíz (`<html>`). Similar a `em`, pero más predecible ya que solo depende de un único valor base.
        * `%` (porcentaje): Relativo al tamaño de fuente del elemento padre.
    * **Ejemplo:**
        ```css
        body {
            font-size: 16px; /* Tamaño base para toda la página */
        }

        h2 {
            font-size: 2em; /* Será el doble del tamaño del cuerpo (32px) */
        }

        .pequeno {
            font-size: 0.8rem; /* 80% del tamaño base del HTML */
        }
        ```

3.  **`font-family`:**
    * **¿Qué hace?** Define el **tipo de letra** o la fuente que se usará para el texto.
    * **Valores:** Se recomienda proporcionar una lista de fuentes separadas por comas. El navegador intentará cargar la primera de la lista; si no la encuentra, pasará a la siguiente. La última fuente debe ser un tipo de fuente genérica (como `serif`, `sans-serif`, `monospace`) como respaldo.
    * **Ejemplo:**
        ```css
        body {
            font-family: Arial, sans-serif; /* Intenta Arial, si no, cualquier fuente sans-serif */
        }

        h1 {
            font-family: "Times New Roman", Times, serif; /* Intenta Times New Roman, si no, Times, y finalmente cualquier serif */
        }
        ```
    * **Curiosidad:** Las fuentes con espacios en su nombre (como "Times New Roman") deben ir entre comillas.
