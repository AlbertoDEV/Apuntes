# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 🔗 HTML: Enlaces - Cómo crear hipervínculos (`<a>`) para navegar entre páginas

La "web" se llama así por la telaraña (*web*) de conexiones que forman los **hipervínculos**, o simplemente **enlaces**. Son los que nos permiten saltar de una página a otra, navegar por internet y conectar diferentes documentos. Piensa en ellos como las **carreteras** que unen todas las ciudades en el mapa de internet.

---

### 🏷️ `<a>` (Anchor - Ancla)

La etiqueta `<a>` es la clave para crear enlaces en HTML.

- **Función**: Envuelve el texto o imagen sobre la que el usuario puede hacer clic.
- **Atributo principal**: `href` (Hypertext Reference), que indica **a dónde lleva** el enlace.

El valor de `href` puede ser:

- Una **URL externa**: `https://www.google.com`
- Una **página interna** de tu sitio: `acerca-de.html`
- Una **sección específica** de la misma página: `#contacto`

---

### 📎 Ejemplos de Enlaces

#### 🔗 Enlace a una página externa:
```html
<p>Visita mi buscador favorito: <a href="https://www.google.com">Google</a>.</p>
```
🧭 El texto "Google" es clickeable y te lleva a la página de Google.

---

#### 🏠 Enlace a una página interna:
```html
<p>¿Tienes preguntas? <a href="contacto.html">Contáctanos aquí</a>.</p>
```
🏡 Es como dar una dirección dentro de tu propio sitio web.

---

#### 🆕 Abrir un enlace en una nueva pestaña (`target="_blank"`):
```html
<p>Aprende más en <a href="https://es.wikipedia.org/" target="_blank">Wikipedia</a>.</p>
```
🔓 Esto abrirá el enlace en una **nueva pestaña**. Úsalo con moderación para no saturar al usuario.

---

#### ✉️ Enlace a una dirección de correo electrónico (`mailto:`):
```html
<p>Envíanos un correo a <a href="mailto:info@ejemplo.com">info@ejemplo.com</a>.</p>
```
📧 Esto abrirá el cliente de correo del usuario con un nuevo mensaje listo para enviar.

---

Los enlaces son la **columna vertebral de la navegación web**. Sin ellos, la web sería solo un montón de documentos aislados. ¡Úsalos sabiamente para conectar y guiar a tus usuarios!
