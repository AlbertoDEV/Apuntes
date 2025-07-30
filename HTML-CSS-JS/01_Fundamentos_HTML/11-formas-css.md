# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 2. Formas de añadir CSS al HTML

Antes de ver los selectores, es crucial entender las **tres formas principales de incluir CSS en tu documento HTML**. Esto es fundamental para que tus estilos puedan aplicarse.

Las tres maneras de añadir CSS son:

1.  **CSS en Línea (Inline CSS):**
    * **¿Cómo funciona?** Aplicas estilos directamente a un elemento HTML usando el atributo `style` dentro de la etiqueta de apertura.
    * **Cuándo usarlo:** Para estilos muy específicos y puntuales de un **solo elemento**. Generalmente **no es una buena práctica** para estilos grandes o reutilizables. Piensa en ello como pintar un pequeño detalle de un cuadro con un pincel muy fino.
    * **Ejemplo:**
        ```html
        <p style="color: blue; font-size: 18px;">Este texto es azul y más grande.</p>
        ```
    * **Ventajas:** Rápido para pruebas rápidas.
    * **Desventajas:** Dificulta el mantenimiento, no separa contenido de presentación, no es reutilizable.

2.  **CSS Interno o Incrustado (Internal/Embedded CSS):**
    * **¿Cómo funciona?** Escribes tus reglas CSS dentro de una etiqueta `<style>` que se coloca en la sección `<head>` de tu documento HTML.
    * **Cuándo usarlo:** Cuando tienes estilos específicos para una **sola página HTML** y no esperas reutilizarlos en otras páginas. Es como si pintaras el plano de una sola habitación de tu casa.
    * **Ejemplo:**
        ```html
        <!DOCTYPE html>
        <html lang="es">
        <head>
            <meta charset="UTF-8">
            <title>Mi Página con Estilos Internos</title>
            <style>
                body {
                    background-color: lightblue;
                }
                h1 {
                    color: navy;
                }
            </style>
        </head>
        <body>
            <h1>¡Hola desde mi página con estilo!</h1>
            <p>El fondo es azul claro y el título es azul marino.</p>
        </body>
        </html>
        ```
    * **Ventajas:** Útil para estilos únicos de una página.
    * **Desventajas:** Si tienes muchas páginas, cada una tendrá su propio bloque de estilos, lo que dificulta la gestión.

3.  **CSS Externo (External CSS):**
    * **¿Cómo funciona?** Creas un archivo separado con extensión `.css` (por ejemplo, `styles.css`) donde escribes todas tus reglas CSS. Luego, enlazas este archivo CSS a tu documento HTML usando la etiqueta `<link>` dentro de la sección `<head>`.
    * **Cuándo usarlo:** Esta es la **forma más recomendada y profesional** de añadir CSS. Es como tener un libro de diseño completo para toda tu casa, o incluso para todas las casas de un vecindario.
    * **Ejemplo:**
        * **Archivo `index.html`:**
            ```html
            <!DOCTYPE html>
            <html lang="es">
            <head>
                <meta charset="UTF-8">
                <title>Mi Página con Estilos Externos</title>
                <link rel="stylesheet" href="styles.css"> </head>
            <body>
                <h1>¡Hola desde mi página con estilo externo!</h1>
                <p>Mis estilos vienen de un archivo aparte.</p>
            </body>
            </html>
            ```
        * **Archivo `styles.css` (en la misma carpeta que `index.html`):**
            ```css
            body {
                background-color: lightgreen;
            }
            h1 {
                color: darkgreen;
            }
            ```
    * **Ventajas:**
        * **Separación de preocupaciones:** Mantiene el HTML limpio (solo estructura) y el CSS en su propio archivo (solo estilos).
        * **Reutilización:** Puedes usar el mismo archivo CSS para múltiples páginas, garantizando coherencia y facilitando cambios.
        * **Caché del navegador:** Los navegadores pueden guardar el archivo CSS en caché, lo que acelera la carga de tus páginas.
    * **Desventajas:** Necesitas un archivo adicional.
