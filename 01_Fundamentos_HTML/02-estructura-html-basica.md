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

- `<!DOCTYPE html>`: Esto es como la **declaración de intenciones**. Le dice al navegador que este documento está escrito en **HTML5**, la versión más reciente del lenguaje. Siempre debe ir al principio del archivo.

- `<html lang="es">...</html>`: Esta es la **etiqueta raíz** de todo el documento. Todo el contenido debe ir dentro de ella. El atributo `lang="es"` indica que el idioma principal es español, lo cual es útil para la accesibilidad y el SEO.

- `<head>...</head>`: Piensa en el `<head>` como el **"cerebro"** de tu página. Contiene información **sobre** el documento (no visible directamente para el usuario) que es vital para el navegador y los motores de búsqueda. Aquí se incluyen elementos como:

  - `<meta charset="UTF-8">`: Define la **codificación de caracteres** del documento. UTF-8 es el estándar universal, compatible con casi todos los caracteres de todos los idiomas. (¡Adiós a los caracteres extraños!)

  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Esta metaetiqueta es esencial para el diseño **responsivo**. Le dice al navegador cómo escalar la página en distintos dispositivos para que se vea bien tanto en móviles como en computadoras.

  - `<title>Mi Primera Página Web</title>`: Define el **título** de tu página, que aparece en la pestaña del navegador. Es importante tanto para la experiencia del usuario como para el SEO.

  Aquí también se pueden enlazar archivos CSS y JavaScript externos (lo veremos más adelante).

- `<body>...</body>`: Este es el **"cuerpo"** de tu página. Contiene **todo el contenido visible**: textos, imágenes, videos, enlaces, formularios, etc. Si algo no está dentro del `<body>`, **no se mostrará** en la página.
