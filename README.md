# HTML

Lenguaje de marcado de texto, es la parte que nos permite estructurar nuestra pagina web, es como el esqueleto de nuestra aplicacion.
su principal objetivo es darle formato semantico a nuestra informacion a travez del uso de `elementos` que esta asu vez esta conformado por `etiquetas` de apertura y cierre y `contenido`.

> [!TIP] En algunos casos encontraremos los `elementos` huerfano estos solo estan confromados por una sola `etiqueta`.

## Estructura de un elemento en HTML

![alt text](file:///home/jalvarez/Proyectos/curso_html/image.png?msec=1779290378566)

## Estructura fundamental del documento html

- `<!DOCTYPE hmlt>` - Declaramos el tipo de documento, este elemento huerfano indica al navegaro que el documento con el que se esta trabajando y que debera renderizar es `html`, **Siempre deber estar en la primera linea**.
- `<html></html>` - Elemento raiz, envuelve todo el contenido de la pagina HTML, este elemento tien dos hijos principales.
  - `<head></head>` - Elemento de configuracion, contiene informacion inportante sobre el docuemnto como (titulo, enlaces css, informacio para motores de busqueda, descripcion entre otros).
    - `<title></title>` - Elemento de titulo de pagina, es el hijo de `head` y define el titulo que aparecera en la pestaña del navegador
  - `<body></body>` -
    
    ## Estructura de contenido semantico (secciones principales)

   Las etiquetas semánticas permiten organizar mejor el contenido.
   <header></header>
<nav></nav>
<main></main>
<section></section>
<article></article>
<aside></aside>
<footer></footer>
Descripción
<header> → encabezado de la página
<nav> → menú de navegación
<main> → contenido principal
<section> → sección de contenido
<article> → contenido independiente
<aside> → contenido secundario
<footer> → pie de página
## Estructura de texto

Las etiquetas de texto en HTML permiten organizar y dar significado al contenido dentro de una página web.

---

## Jerarquía de encabezados

Los encabezados permiten estructurar el contenido de forma jerárquica.

HTML posee 6 niveles de encabezados:

- `<h1>` → título principal
- `<h2>` → subtítulos
- `<h3>` → subsecciones
- `<h4>` a `<h6>` → niveles más específicos

> [!IMPORTANT]
> Se recomienda usar un solo `<h1>` por página.

### Ejemplo

```html
<h1>Curso de HTML</h1>

<h2>Estructura básica</h2>

<h3>Etiqueta html</h3>

<h3>Etiqueta body</h3>

<h2>Etiquetas de texto</h2>

<h3>Párrafos</h3>

<h4>Etiqueta p</h4>
```

---

## Párrafos y énfasis

Estas etiquetas permiten agregar texto y destacar información importante.

### Etiquetas principales

- `<p>` → párrafos
- `<strong>` → texto importante
- `<em>` → texto enfatizado
- `<mark>` → texto resaltado

### Ejemplo

```html
<p>Este es un párrafo.</p>

<p>
    Este texto tiene una palabra 
    <strong>importante</strong>.
</p>

<p>
    Este texto tiene <em>énfasis</em>.
</p>

<p>
    Texto <mark>resaltado</mark>.
</p>
```

---

## Listas

Las listas permiten organizar elementos relacionados.

### Tipos de listas

- `<ul>` → lista desordenada
- `<ol>` → lista ordenada
- `<li>` → elemento de lista

### Ejemplo

```html
<h2>Lista de compras</h2>

<ul>
    <li>Leche</li>
    <li>Pan</li>
    <li>Huevos</li>
</ul>

<h2>Pasos</h2>

<ol>
    <li>Encender cocina</li>
    <li>Calentar sartén</li>
    <li>Servir comida</li>
</ol>
```

---

## Citas y referencias

Permiten representar citas dentro del contenido.

### Etiquetas principales

- `<q>` → cita corta
- `<blockquote>` → cita extensa

### Ejemplo

```html
<p>
    Como dijo el profesor:
    <q>La práctica hace al maestro</q>
</p>

<blockquote>
    HTML es el lenguaje estándar para crear páginas web.
</blockquote>
```

---

## Código y texto técnico

Estas etiquetas permiten mostrar código fuente o texto técnico.

### Etiquetas principales

- `<code>` → código en línea
- `<pre>` → conserva espacios y saltos de línea

### Ejemplo

```html
<p>
    La etiqueta <code>p</code> crea párrafos.
</p>

<pre>
<code>
function saludar() {
    console.log("Hola mundo");
}
</code>
</pre>
```

---

## Líneas y saltos

Permiten separar o dividir contenido visualmente.

### Etiquetas principales

- `<br>` → salto de línea
- `<hr>` → línea horizontal

### Ejemplo

```html
<p>
    Primera línea <br>
    Segunda línea
</p>

<hr>

<p>Nuevo contenido</p>
```

---

# CSS (cascadig style sheet)
cascada de hojas de estilops, es el documento que nos permita darle estilo a nuestros elementos, posicionar, escalar,formato, color y transcisiones.
# maneras de apllicar css a nuestro documento html
### 1. en linea
 este manera de aplicar css es haciendo uso de los atributos de un elemento en este en especial usando el atributo 'style'
'''html
<p style="color:pink;size:23px">este es el texto </p>
'''

>[!TIP] en el caso de lo embebidos y los de archivos externos hay que entender  sobre selectores:son maneras de como yo identifico un elemneto dentro de un documento html, selector por etiqueta, id y clases, en el diseño web se recomienda solo los selectores de tipo clase.
### 2. embebidos
este tipo de aplicar estilo nos permite hacer uso de la etiqueta style para poder estilar nuestros elementos,
por convencio est etiqueta al ser de configuracion se debe usar en el 'head'.
### 3. archivo externo
