# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 📋 HTML: Listas - Ordenadas (<ol>), Desordenadas (<ul>) y Elementos de Lista (<li>)

Las listas son un elemento fundamental en cualquier página web. Nos permiten organizar información de forma clara y fácil de leer, ya sea una receta, pasos a seguir o una simple enumeración de puntos. Piensa en ellas como las listas que haces en tu día a día: la lista de la compra, una lista de tareas pendientes o los pasos para armar un mueble.

HTML nos ofrece dos tipos principales de listas y una etiqueta para los elementos dentro de ellas:

---

### 🔹 Listas Desordenadas (`<ul>` - *Unordered List*)

- Se usan para agrupar elementos donde **el orden no importa**.
- Visualmente, muestran los elementos con **viñetas** (círculos, cuadrados, etc.).

#### Ejemplo:
```html
<h2>Mis Frutas Favoritas</h2>
<ul>
    <li>Manzana</li>
    <li>Plátano</li>
    <li>Naranja</li>
</ul>
```

🛒 *Imagina que vas al supermercado y apuntas las frutas que necesitas; el orden en el que las escribes no cambia lo que son.*

---

### 🔸 Listas Ordenadas (`<ol>` - *Ordered List*)

- Se usan cuando **el orden de los elementos sí importa**.
- Visualmente, los elementos aparecen con **números** (1, 2, 3...) o **letras** (A, B, C...).

#### Ejemplo:
```html
<h2>Pasos para hacer café</h2>
<ol>
    <li>Hierve agua.</li>
    <li>Muele los granos de café.</li>
    <li>Vierte el agua caliente sobre el café.</li>
    <li>Disfruta de tu café.</li>
</ol>
```

☕ *Si inviertes los pasos para hacer café, el resultado no sería el mismo, ¿verdad? Por eso es una lista ordenada.*

---

### ✅ Elemento de Lista (`<li>` - *List Item*)

- Esta etiqueta representa **cada elemento individual** dentro de una lista.
- Siempre debe ir dentro de una `<ul>` o una `<ol>`.

#### Ejemplo:
```html
<ul>
    <li>Este es un ítem de lista desordenada</li>
    <li>Este es otro ítem</li>
</ul>

<ol>
    <li>Este es un ítem de lista ordenada</li>
    <li>Y este es el segundo</li>
</ol>
```
