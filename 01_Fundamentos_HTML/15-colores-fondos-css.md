# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 6. Colores y fondos: Cómo aplicar colores y usar imágenes de fondo

Ya hemos visto cómo cambiar el color del texto con `color`, pero CSS te permite mucho más: puedes colorear el fondo de elementos, usar imágenes como fondos, y controlar la opacidad.

Aquí tienes las propiedades clave:

1.  **`background-color`:**
    * **¿Qué hace?** Establece el **color de fondo** de un elemento.
    * **Valores:** Puedes usar nombres de colores (ej., `lightblue`), valores hexadecimales (ej., `#FFD700`), o valores RGB/RGBA (ej., `rgb(255, 99, 71)`). `RGBA` es especialmente útil porque la "A" al final significa "Alpha" y te permite controlar la **opacidad** (transparencia) del color, con `1` siendo totalmente opaco y `0` totalmente transparente.
    * **Ejemplo:**
        ```css
        .tarjeta-producto {
            background-color: #F0F8FF; /* Color de fondo blanco azulado */
            padding: 20px;
        }

        .mensaje-alerta {
            background-color: rgba(255, 0, 0, 0.5); /* Rojo con 50% de transparencia */
            color: white;
        }
        ```
    * **Curiosidad:** El `background-color` se extiende a través del área de **contenido** y **padding** del Modelo de Caja, pero no al margen.

2.  **`background-image`:**
    * **¿Qué hace?** Permite usar una **imagen como fondo** de un elemento.
    * **Valores:** La función `url()` que apunta a la ruta de tu imagen.
    * **Ejemplo:**
        ```css
        body {
            background-image: url('imagenes/fondo-patron.png'); /* Usa una imagen como fondo de toda la página */
        }

        .hero-section {
            background-image: url('imagenes/banner-viaje.jpg'); /* Una imagen grande para una sección destacada */
        }
        ```
    * **Consideraciones importantes al usar `background-image`:**
        * **`background-repeat`**: Controla si la imagen se repite para cubrir el espacio.
            * `repeat` (por defecto): La imagen se repite tanto horizontal como verticalmente.
            * `no-repeat`: La imagen aparece solo una vez.
            * `repeat-x`: La imagen se repite solo horizontalmente.
            * `repeat-y`: La imagen se repite solo verticalmente.
            ```css
            body {
                background-image: url('imagenes/fondo-patron.png');
                background-repeat: no-repeat; /* La imagen no se repite */
            }
            ```
        * **`background-position`**: Define la posición inicial de la imagen de fondo.
            * Puedes usar palabras clave (ej., `center`, `top right`) o valores (ej., `50% 50%`, `100px 200px`).
            ```css
            .hero-section {
                background-image: url('imagenes/banner-viaje.jpg');
                background-position: center center; /* Centra la imagen horizontal y verticalmente */
            }
            ```
        * **`background-size`**: Ajusta el tamaño de la imagen de fondo.
            * `auto` (por defecto): Mantiene el tamaño original.
            * `cover`: Escala la imagen para cubrir todo el área, recortando si es necesario.
            * `contain`: Escala la imagen para que sea visible por completo, pero puede dejar espacio vacío.
            * Valores específicos (ej., `100%`, `500px`).
            ```css
            .hero-section {
                background-image: url('imagenes/banner-viaje.jpg');
                background-size: cover; /* La imagen cubrirá toda la sección */
                background-position: center;
            }
            ```
        * **`background-attachment`**: Define si la imagen de fondo se desplaza con el contenido o se queda fija.
            * `scroll` (por defecto): Se desplaza con el contenido.
            * `fixed`: La imagen se queda fija en la ventana del navegador mientras el contenido se desplaza por encima.
            ```css
            body {
                background-image: url('imagenes/cielo.jpg');
                background-attachment: fixed; /* El cielo se queda fijo */
            }
            ```
    * **Propiedad abreviada `background`**: Puedes combinar varias propiedades de fondo en una sola línea, lo que es muy común.
        ```css
        body {
            background: lightblue url('imagenes/nubes.png') no-repeat center fixed;
        }
        /* Esto significa: color de fondo azul claro, imagen de nubes, no se repite, centrada, y fija al desplazarse. */
        ```
