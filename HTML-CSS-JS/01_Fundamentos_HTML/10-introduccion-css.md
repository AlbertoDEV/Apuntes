# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🎨 CSS: La Piel y la Ropa de la Web

### 1. ¿Qué es CSS y cómo estiliza el HTML?

Si HTML es el esqueleto de tu página web, entonces **CSS** (que significa **C**ascading **S**tyle **S**heets, u Hojas de Estilo en Cascada) es la **piel, la ropa, el maquillaje y la decoración**. Es lo que hace que tu esqueleto se vea bien. CSS es un lenguaje de estilos que describe cómo se deben presentar los elementos HTML en la pantalla (o en otros medios, como la impresión).

**Imagina esto:**
* Con HTML, creas una casa: pones las paredes (un `<div>`), las ventanas (`<input type="checkbox">`), el techo (`<header>`).
* Con CSS, pintas las paredes de azul, pones cortinas en las ventanas, eliges el tipo de tejas para el techo y añades un jardín con flores.

**¿Para qué sirve CSS?**
CSS te permite controlar la **apariencia visual** de tus elementos HTML:
* **Colores:** Cambiar el color del texto, del fondo, de los botones.
* **Fuentes:** Elegir el tipo de letra, el tamaño, si está en negrita o cursiva.
* **Disposición (Layout):** Organizar cómo se distribuyen los elementos en la página (uno al lado del otro, uno encima del otro, columnas, etc.).
* **Espaciado:** Definir el espacio entre elementos, el margen, el relleno.
* **Dimensiones:** Controlar el ancho y alto de los elementos.
* **Efectos visuales:** Sombras, transiciones, animaciones (¡más avanzado, pero posible!).

**¿Cómo funciona?**
CSS funciona aplicando "reglas de estilo" a los elementos HTML. Una regla CSS básica tiene dos partes:
1.  **Selector:** Le dice a CSS **qué elemento HTML** quieres estilizar.
2.  **Declaración:** Le dice a CSS **cómo quieres estilizarlo**, a través de propiedades y valores.

Por ejemplo:
```css
p { /* Selector: todos los párrafos */
    color: blue; /* Propiedad: color, Valor: azul */
    font-size: 16px; /* Propiedad: tamaño de fuente, Valor: 16 píxeles */
}
