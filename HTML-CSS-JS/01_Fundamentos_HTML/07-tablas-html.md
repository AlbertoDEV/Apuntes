# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 7. Tablas: Creación de tablas básicas (`<table>`, `<tr>`, `<td>`, `<th>`)

Las **tablas** en HTML se usan para mostrar datos tabulares, es decir, información que está organizada en filas y columnas. Piensa en una hoja de cálculo, un horario, una tabla de precios o los resultados de un partido de fútbol. Las tablas son perfectas para presentar este tipo de datos de forma estructurada y legible.

Para crear una tabla básica, necesitas varias etiquetas que trabajan juntas:

* **`<table>`**: Esta es la etiqueta contenedora principal para toda la tabla. Todo el contenido de la tabla va dentro de ella.
* **`<tr>` (Table Row - Fila de Tabla)**: Define una **fila** dentro de la tabla. Cada `<tr>` que crees será una nueva fila en tu tabla.
* **`<th>` (Table Header - Encabezado de Tabla)**: Define una **celda de encabezado** en la tabla. Estas celdas suelen aparecer en la primera fila o columna y representan los títulos de las columnas o filas. El texto dentro de `<th>` se muestra en **negrita y centrado** por defecto, y son importantes semánticamente.
* **`<td>` (Table Data - Dato de Tabla)**: Define una **celda de datos** en la tabla. Estas son las celdas regulares que contienen la información.

Veamos un ejemplo práctico:

```html
<h2>Horario Semanal</h2>
<table>
    <tr>
        <th>Día</th>
        <th>Mañana</th>
        <th>Tarde</th>
    </tr>
    <tr>
        <td>Lunes</td>
        <td>Reunión</td>
        <td>Trabajo</td>
    </tr>
    <tr>
        <td>Martes</td>
        <td>Clases</td>
        <td>Gimnasio</td>
    </tr>
</table>
