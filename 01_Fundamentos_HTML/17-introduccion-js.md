# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🧠 JavaScript: El Cerebro y los Músculos de la Web

### 1. ¿Qué es JavaScript y cómo funciona?

Hemos aprendido que **HTML** es el esqueleto de tu página (la estructura) y **CSS** es la piel y la ropa (el estilo). Pero, ¿qué pasa si quieres que tu página haga algo más que solo mostrar información estática? Aquí es donde entra **JavaScript** (JS).

**JavaScript es el cerebro y los músculos de la web.** Es un **lenguaje de programación** (¡ahora sí, de programación!) que permite hacer que las páginas web sean **interactivas y dinámicas**. Es lo que permite que una página web "cobre vida".

**Imagina esto con la analogía de la casa:**
* **HTML:** Construye las paredes, las puertas, las ventanas.
* **CSS:** Pinta las paredes, elige el diseño de las puertas, el color de las cortinas.
* **JavaScript:** Hace que la luz se encienda cuando pulsas un interruptor, que la puerta se abra al tocar un timbre, que una ventana se cierre automáticamente al llover.

**¿Para qué sirve JavaScript?**
JavaScript te permite añadir funcionalidades como:
* **Interactividad:** Responder a las acciones del usuario (clics en botones, pasar el ratón por encima de algo, escribir en un campo).
* **Manipular el contenido:** Cambiar texto, añadir o quitar elementos HTML dinámicamente.
* **Validación de formularios:** Comprobar si los datos que un usuario introduce son correctos antes de enviarlos al servidor.
* **Animaciones:** Crear efectos visuales y animaciones complejas sin recargar la página.
* **Cargar datos de forma asíncrona:** Obtener información de un servidor sin que la página tenga que recargarse (¡fundamental para aplicaciones modernas como redes sociales o tiendas online!).
* **Juegos y aplicaciones web completas:** Construir experiencias muy ricas directamente en el navegador.

**¿Cómo funciona JavaScript en el navegador?**
Cuando tu navegador carga una página HTML, también lee el código JavaScript. Luego, un "motor de JavaScript" (como V8 en Chrome o SpiderMonkey en Firefox) **ejecuta** ese código. JavaScript puede acceder y modificar el HTML y el CSS de la página a través de algo llamado **DOM (Document Object Model)**. Piensa en el DOM como un mapa de toda la estructura HTML de tu página que JavaScript puede leer y manipular.

**¿Cómo se añade JavaScript a HTML?**
La forma más común (y recomendada para la mayoría de los casos) es enlazar un archivo JavaScript externo usando la etiqueta `<script>` en tu HTML:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Página con JS</title>
</head>
<body>
    <h1>¡Mi página ahora es interactiva!</h1>
    <button id="miBoton">Haz clic aquí</button>

    <script src="script.js"></script> 
</body>
</html>
