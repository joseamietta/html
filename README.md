## Contenido
Organiza en bloques o secciones de contenido dentro del ```<body>```. Es importante para la accesibilidad y el SEO que estos elementos se identifiquen con el objetivo o la estructura de ese contenido.

### ```<div>```
Sirve para crear secciones o agrupar contenidos.

```html
<div style="color: blue;">
 <h2> Ejemplo de div y span </h2>
  <p>
    Esto es un párrafo dentro de un div,
    <span style="color: red;"> y esto un span dentro de un párrafo.</span> 
  </p>
</div>
```

### ```<h>```
Los elementos de encabezado implementan seis niveles de encabezado del documento, ```<h1>``` es el más importante, y ```<h6>```, el menos importante.

```html
<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>
```

### ```<dl>```
Representa una lista descriptiva. El elemento encierra una lista de grupos de términos (especificados con el uso del elemento ```<dt>```) y de descripciones (proveídas con elementos ```<dd>```). Algunos usos comunes para este elemento son implementar un glosario o para desplegar metadatos (lista de pares llave-valor).

```html
<dl>
  <dt>Firefox</dt>
  <dd>
    A free, open source, cross-platform,
    graphical web browser developed by the
    Mozilla Corporation and hundreds of
    volunteers.
  </dd>

  <!-- Other terms and descriptions -->
</dl>
```

### ```<ol>```
Permite definir listas o viñetas ordenadas (“Ordered List”), bien con numeración o alfabéticamente.

```html
<ol>
 <li>punto uno</li>
 <li>punto dos</li>
 <li>punto tres</li>
</ol>
```

### ```<ul>```
Crea una lista no ordenada.

```html
<ul>
 <li>Esto</li>
 <li>Lo otro</li>
 <li>Lo de más allá</li>
</ul>
```

### ```<p>```
Es el apropiado para distribuir el texto en párrafos.

```html
<p>
Esto 
es un 
párrafo
</p>
```

### ```<pre>```
Representa texto preformateado.

```html
<!-- Un poco de codigo CSS -->
<pre>
body{
  color:  red;
}
a   {
  color:green;
}
</pre>
```

### ```<blockquote>```
Cita en bloque . Crea citas en bloque, marca las citas a otros autores o documentos.

```html
<blockquote cite="http://html.conclase.net/w3c/html401...def-BLOCKQUOTE">
  <p> 
    <strong>Nota.</strong> Recomendamos que las implementaciones de hojas
    de estilo porporcionen un mecanismo para insertar signos de puntuación de citas
    antes y después de una cita delimitada por un BLOCKQUOTE de un modo apropiado según 
    el contexto del idioma actual y el grado de anidamiento de las citas. 
  </p>
</blockquote>
```

## Semántica del texto en línea
Utilice la semántica del texto en línea HTML para definir el significado, estructura, o el estilo de una palabra, una línea o cualquier pieza arbitraria de texto.

### ```<a>```
El Elemento HTML Anchor ```<a>``` crea un enlace a otras páginas de internet, archivos o ubicaciones dentro de la misma página, direcciones de correo, o cualquier otra URL.

```html
<a href="https://developer.mozilla.org">MDN</a>
```

### ```<b>```
Indica que el texto debe ser representado con una variable bold, o negrita, de la tipografía que se esté usando.

```html
<p>
  Texto normal y... <b>Texto en negrita</b>
<p>
```

### ```<strong>```
El elemento strong es el apropiado para marcar con especial énfasis las partes más importantes de un texto.

```html
<p>
   <em>El dinero</em> es importante pero <strong>la salud</strong> lo es más.
</p>
```

### ```<br>```
El elemento HTML line break ```<br>``` produce un salto de línea en el texto (retorno de carro). Es útil para escribir un poema o una dirección, donde la división de las líneas es significante.

```html
Mozilla Foundation<br>
1981 Landings Drive<br>
Building K<br>
Mountain View, CA 94043-0801<br>
USA
```

### ```<em>```
El elemento HTML ```<em>``` es el apropiado para marcar con énfasis las partes importantes de un texto.

```html
<p>
   <em>El dinero</em> es importante pero <strong>la salud</strong> lo es más.
</p>
```

### ```<i>```
Muestra el texto marcado con un estilo en cursiva o italica.

```html
<p>
     Texto normal y... <i>Texto 'inclinado'</i>
</p>
```

### ```<span>```
span - abarcar. Sirve para aplicar estilo al texto o agrupar elementos en línea.

```html
<div style="border: 1px dotted blue;">
    <h4>Ejemplo de div y span </h4>
    <p>
        Esto es un párrafo dentro de un div,
        <span style="color: red;"> y esto un span dentro de un párrafo. </span>
    </p>
</div>
```

## Imagen y multimedia
HTML soporta varios recursos multimedia como imágenes, audio, y video.

### ```<audio>```
El elemento audio se usa para insertar contenido de audio en un documento HTML o XHTML. El elemento audio se agregó como parte de HTML 5.

```html
<audio src="http://developer.mozilla.org/@api/deki/files/2926/=AudioTest_(1).ogg"
       autoplay>
  Your browser does not support the <code>audio</code> element.
</audio>
```

### ```<img>```
El elemento de imagen HTML ```<img>``` representa una imagen en el documento.

```html
<!-- img element -->
<img src="foo" alt="bar">

<!-- img element, srcset attribute -->
<img srcset="foo-320w.jpg 320w, foo-480w.jpg 480w, foo-800w.jpg 800w" sizes="(max-width: 320px) 280px, (max-width: 480px) 440px, 800px" src="foo-800w.jpg" alt="bar">

<!-- picture and source elements, srcset attributes -->
<picture>
  <source media="(max-width: 799px)" srcset=foo-480w.jpg>
  <source media="(min-width: 800px)" srcset=foo-800w.jpg>
  <img src="foo-800w.jpg" alt="bar">
</picture>
```

### ```<video>```
El elemento video se utiliza para incrustar vídeos en un documento HTML o XHTML.

```html
<video src="videofile.ogg" autoplay poster="posterimage.jpg">
  Tu navegador no admite el elemento <code>video</code>.
</video>
```

## Contenido incrustado
Además de los contenidos multimedia habituales, HTML puede incluir otra variedad de contenidos, aunque no siempre es fácil interactuar con ellos.

### ```<iframe>```
Permite incrustar otra página HTML en la página actual.

```html
<iframe src="https://mdn-samples.mozilla.org/snippets/html/iframe-simple-contents.html" title="iframe Example 1" width="400" height="300">
  <p>Your browser does not support iframes.</p>
</iframe>
````

## Formularios

### ```<form>```
Representa una sección de un documento que contiene controles interactivos que permiten a un usuario enviar información a un servidor web.

```html
<!-- Formulario con conjunto de campos, leyenda y etiqueta -->
<form action="" method="post">
  <fieldset>
    <legend>Título</legend>
    <input type="radio" name="radio" id="radio"> <label for="radio">Clic aquí</label>
  </fieldset>
</form>
```

### ```<fieldset>```
El elemento fieldset permite organizar en grupos los campos de un formulario.

```html
<form>
    <fieldset>
        <legend>Información Personal</legend>
        Nombre: <input name='nombre' type='text' tabindex='1'>
        Apellidos: <input name='apellidos' type='text' tabindex='2'>
    </fieldset>

    <fieldset>
        <legend>edad</legend>
        <input type='checkbox' tabindex='20' name='edad' value='20-39'> 20-39
        <input type='checkbox' tabindex='21' name='edad' value='40-59'> 40-59
        <input type='checkbox' tabindex='22' name='edad' value='60-79'> 60-79
    </fieldset>
</form>
```

### ```<input>```
Se usa para crear controles interactivos para formularios basados en la web con el fin de recibir datos del usuario.
Hay distintos tipos de input y se definen con el atributo type.

```html
<p>A common form that includes input tags</p>
<form action="getform.php" method="get">
    <label>First name: <input type="text"></label><br>
    <label>Last name: <input type="text"></label><br>
    <label>E-mail: <input type="email"></label><br>
    <input type="submit" value="Submit">
</form>
```

### ```<textarea>```
Representa un control para la edición mutilínea de texto sin formato.

```html
<textarea name="textarea" rows="10" cols="50">Write something here</textarea>
```

### ```<select>```
Representa un control que muestra un menú de opciones. Las opciones contenidas en el menú son representadas por elementos ```<option>```

```html
<!-- The second value will be selected initially -->
<select name="select">
  <option value="value1">Value 1</option> 
  <option value="value2" selected>Value 2</option>
  <option value="value3">Value 3</option>
</select>
```
