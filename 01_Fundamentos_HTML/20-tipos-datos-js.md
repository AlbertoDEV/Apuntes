---

### 🧠 ¿Qué es JavaScript y para qué sirve en la web?

Imagina la creación de una página web como la construcción de una casa:

* **HTML 🏡: El Esqueleto**
    * Piensa en HTML (HyperText Markup Language) como los cimientos, las paredes y el techo de tu casa. Es la **estructura básica** que define los contenidos: los textos, las imágenes, los formularios, etc. Sin HTML, no hay página, solo un espacio vacío.

* **CSS 🎨: La Decoración**
    * CSS (Cascading Style Sheets) sería la pintura de las paredes, los muebles, las cortinas y toda la decoración que hace que la casa sea atractiva y agradable a la vista. Con CSS le das **estilo y apariencia** a tus elementos HTML, definiendo colores, tamaños, fuentes y cómo se organizan visualmente.

* **JavaScript ✨: La Vida y la Interacción**
    * Ahora, ¿qué hace que una casa sea funcional y se sienta "viva"? Son las luces que se encienden y apagan, las puertas que se abren con un sensor, la nevera inteligente, el termostato que ajusta la temperatura automáticamente. ¡Eso es JavaScript!
    * JavaScript es el **lenguaje de programación** que permite que tu página web sea **interactiva y dinámica**. Es el **cerebro y los músculos** que hacen que las cosas sucedan y respondan al usuario.

---

### 🚀 ¿Para qué usamos JavaScript en la web?

Gracias a JavaScript, una página web puede hacer cosas asombrosas como:

* **Reaccionar a las acciones del usuario 🖱️:**
    * Cuando haces clic en un botón, pasas el ratón por encima de una imagen, escribes en un campo de texto o envías un formulario. JavaScript detecta estas acciones y puede hacer que algo cambie en la página.
* **Actualizar contenido dinámicamente 🔄:**
    * ¿Has notado cómo en redes sociales aparecen nuevas publicaciones o notificaciones sin que tengas que recargar toda la página? Eso es JavaScript en acción, que permite cargar nueva información del servidor y mostrarla al instante.
* **Crear animaciones y efectos visuales 🎬:**
    * Desde menús desplegables suaves, carruseles de imágenes, hasta complejas animaciones que hacen tu sitio más atractivo y moderno.
* **Validar formularios 📝:**
    * Antes de que la información de un formulario se envíe a un servidor, JavaScript puede verificar si has rellenado todos los campos obligatorios, si un email tiene el formato correcto, o si una contraseña cumple ciertos requisitos. Esto mejora la experiencia del usuario y evita errores.
* **Comunicarse con servidores (APIs) 📡:**
    * JavaScript puede pedir o enviar información a otros servicios en internet (como una aplicación del tiempo que te da el pronóstico o una base de datos de productos para un e-commerce). Esto se hace a menudo usando las llamadas **APIs (Interfaces de Programación de Aplicaciones)**.
* **Crear juegos y aplicaciones web completas 🎮:**
    * Muchos juegos que juegas en tu navegador están completamente construidos con JavaScript. También permite el desarrollo de aplicaciones web complejas que se comportan casi como programas de escritorio.

En resumen, si HTML define lo que hay y CSS cómo se ve, **JavaScript le da la capacidad de interactuar, funcionar y "vivir"**.

---
---

### 📝 Variables: Los Contenedores de Información de JavaScript

Imagina que JavaScript es como una oficina, y en esa oficina necesitas guardar diferentes tipos de información: un número de teléfono, un nombre, una lista de tareas pendientes. Para eso, usarías archivadores, cajas o etiquetas. En JavaScript, esos "contenedores" son las **variables**.

Una **variable** es básicamente un espacio con nombre en la memoria de tu ordenador donde puedes almacenar datos. Piensa en ella como una etiqueta que le pones a una caja para saber qué hay dentro.

En JavaScript, declaramos variables usando una de estas tres palabras clave: `let`, `const` o `var`. ¡Cada una tiene su propia personalidad!

---

#### `var`: El Antiguo Luchador (¡Con algunas peculiaridades!)

`var` es la forma más antigua de declarar variables en JavaScript. Funciona, pero tiene algunas características que a veces pueden ser confusas, especialmente para los principiantes. Es como un coche clásico: funcional, pero con algunos detalles que los modelos nuevos han mejorado.

* **Alcance:** Las variables declaradas con `var` tienen un **alcance de función**. Esto significa que si declaras `var` dentro de una función, solo existe dentro de esa función. Si la declaras fuera, es global.
* **Re-declaración y Re-asignación:** Puedes re-declarar y re-asignar el valor a una variable `var` cuantas veces quieras.

    ```javascript
    var edad = 30;
    console.log(edad); // Muestra: 30

    var edad = 31; // ¡Se puede redeclarar!
    console.log(edad); // Muestra: 31

    edad = 32; // También se puede reasignar
    console.log(edad); // Muestra: 32
    ```

---

#### `let`: El Moderno y Flexible

`let` se introdujo en una versión más reciente de JavaScript (ES6) para solucionar algunas de las "peculiaridades" de `var`. Es el tipo de variable que usarás muy a menudo.

* **Alcance de Bloque:** A diferencia de `var`, `let` tiene un **alcance de bloque**. Esto significa que la variable solo existe dentro del bloque de código (definido por `{ }`) donde fue declarada. Esto ayuda a evitar errores y a mantener tu código más organizado.
* **Re-asignación, pero no Re-declaración:** Puedes cambiar el valor de una variable `let` (`re-asignar`), pero no puedes declararla de nuevo en el mismo ámbito.

    ```javascript
    let nombre = "Ana";
    console.log(nombre); // Muestra: Ana

    nombre = "María"; // Se puede reasignar
    console.log(nombre); // Muestra: María

    // let nombre = "Pedro"; // ¡Esto daría un error! Ya está declarada en este ámbito.

    if (true) {
        let ciudad = "Madrid"; // 'ciudad' solo existe aquí dentro
        console.log(ciudad); // Muestra: Madrid
    }
    // console.log(ciudad); // ¡Esto daría un error! 'ciudad' no está definida aquí.
    ```

---

#### `const`: La Constante Fiel

`const` también se introdujo con `let` en ES6. Su nombre lo dice todo: ¡es para valores que no cambian! Piensa en ella como una caja sellada.

* **Alcance de Bloque:** Al igual que `let`, `const` tiene un **alcance de bloque**.
* **No Re-asignación ni Re-declaración:** Una vez que asignas un valor a una variable `const`, ¡no puedes cambiarlo ni re-declararla! Por eso, siempre debes inicializarla con un valor cuando la declaras. Es ideal para valores que sabes que no cambiarán, como el valor de PI o el nombre de tu aplicación.

    ```javascript
    const PI = 3.14159;
    console.log(PI); // Muestra: 3.14159

    // PI = 3.14; // ¡Esto daría un error! No se puede reasignar.

    const nombreApp = "MiGranApp";
    console.log(nombreApp); // Muestra: MiGranApp

    // const nombreApp = "OtraApp"; // ¡Esto daría un error! No se puede redeclarar.
    ```
    ⚠️ **Importante:** Aunque el valor de una `const` no se puede re-asignar, si esa `const` contiene un **objeto** o un **array**, sí se pueden modificar sus propiedades internas o elementos. ¡Es como si la caja no se pudiera cambiar, pero sí lo que hay dentro de ella! (Esto lo veremos mejor cuando hablemos de tipos de datos complejos).

---

### ¿Cuándo usar cada una? 🤔

* Usa **`const`** por defecto para la mayoría de tus variables. Esto hace que tu código sea más predecible y evita cambios accidentales.
* Si sabes que el valor de la variable va a cambiar más tarde (por ejemplo, en un contador), usa **`let`**.
* **Evita usar `var`** en código nuevo. Aunque lo verás en código antiguo, es una buena práctica usar `let` y `const` para un código más limpio y con menos errores.

---
---

### 📦 Tipos de Datos: Clasificando la Información en JavaScript

Si las variables son las cajas donde guardamos la información, los **tipos de datos** son la **clasificación de esa información**. Es como saber si en una caja hay manzanas, libros, o herramientas. Saber qué tipo de dato es algo en JavaScript es crucial porque el lenguaje se comporta de manera diferente con cada tipo.

JavaScript es un lenguaje de **tipado dinámico**, lo que significa que no necesitas especificar el tipo de dato cuando declaras una variable. El motor de JavaScript lo averigua automáticamente basándose en el valor que le asignas.

Vamos a ver los tipos de datos más comunes y esenciales:

---

#### 🔢 1. Números (`Number`)

Este tipo de dato se usa para cualquier tipo de número, ya sean enteros (como 10, 250) o decimales (como 3.14, 0.5).

```javascript
let edad = 30; // Un número entero
let precio = 99.99; // Un número decimal
let temperatura = -5; // Números negativos también
