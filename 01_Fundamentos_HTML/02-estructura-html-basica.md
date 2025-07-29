# 🚀 Nivel 1: Recién Empezado (Fundamentos)

## 💻 HTML: El Esqueleto de la Web

### 2. Estructura básica de un documento HTML

Si HTML es el esqueleto de tu página, la **estructura básica** es como la columna vertebral y el cráneo: son las partes fundamentales que todo cuerpo (o en este caso, documento HTML) necesita para funcionar.

Cualquier documento HTML que crees siempre tendrá estas partes principales:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Primera Página Web</title>
</head>
<body>
    <h1>¡Hola, mundo!</h1>
    <p>Esta es mi primera página web.</p>
</body>
</html>
```

Vamos a desglosar cada una de estas partes cruciales:

<!DOCTYPE html>: Esto es como la declaración de intenciones. Le dice al navegador que este documento es un archivo HTML5, la versión más reciente de HTML. Siempre va al principio.

<html lang="es">...</html>: Esta es la etiqueta raíz de todo el documento. Todo lo demás va dentro de ella. El atributo lang="es" le indica al navegador (y a los lectores de pantalla) que el idioma principal del contenido es el español, lo cual es bueno para la accesibilidad y el SEO.

<head>...</head>: Piensa en el <head> como el "cerebro" o la "cabeza" de tu página. Contiene información sobre el documento que no es visible directamente para el usuario, pero es vital para el navegador y los motores de búsqueda. Aquí se incluyen cosas como:

<meta charset="UTF-8">: Define la codificación de caracteres del documento. UTF-8 es el estándar y permite mostrar correctamente casi cualquier carácter de cualquier idioma (¡adiós a los caracteres raros!).

<meta name="viewport" content="width=device-width, initial-scale=1.0">: Esta metaetiqueta es crucial para el diseño web responsivo. Le dice al navegador cómo debe escalar la página en diferentes dispositivos (móviles, tablets, etc.) para que se vea bien en todas partes.

<title>Mi Primera Página Web</title>: El título de tu página, que aparece en la pestaña del navegador o en la ventana. Es muy importante para la usabilidad y el SEO.

Aquí también se enlazan los archivos CSS y JavaScript externos, pero eso lo veremos más adelante.

<body>...</body>: Este es el "cuerpo" de tu página, donde reside todo el contenido visible que los usuarios verán e interactuarán: textos, imágenes, videos, enlaces, formularios, etc. Si no está en el <body>, no aparecerá en la página.
