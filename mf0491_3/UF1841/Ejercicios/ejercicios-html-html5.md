# 🎮 Mini-Retos HTML & HTML5
## Ejercicios rápidos para practicar

---

##  PARTE 1: HTML Básico

---

###  Reto 1: ¿Qué es HTML?

**Reto rápido:** ¡Crea tu primer documento HTML!

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mi Primera Página</title>
</head>
<body>
    <!-- Escribe aquí tu nombre entre etiquetas h1 -->
    
</body>
</html>
```

**Tu misión:** Escribe tu nombre dentro de la etiqueta `<h1>` y guarda el archivo como `reto1.html`.

---

###  Reto 2: Estructura de un Elemento HTML

**Reto rápido:** ¡Identifica las partes!

Dado este elemento:
```html
<a href="https://google.com" target="_blank">Ir a Google</a>
```

**Responde:**
1. ¿Cuál es la **etiqueta de apertura**? ___________
2. ¿Cuál es el **contenido**? ___________
3. ¿Cuál es el **atributo** y su **valor**? ___________
4. ¿Cuál es la **etiqueta de cierre**? ___________

---

###  Reto 3: Tipos de Elementos HTML

**Reto rápido:** ¡Clasifica los elementos!

Escribe **"bloque"** o **"línea"** según corresponda:

| Elemento | ¿Bloque o Línea? |
|----------|------------------|
| `<div>` | ___________ |
| `<span>` | ___________ |
| `<p>` | ___________ |
| `<strong>` | ___________ |
| `<h1>` | ___________ |
| `<img>` | ___________ |

---

###  Reto 4: Atributos HTML Importantes

**Reto rápido:** ¡Completa los atributos!

```html
<!-- Agrega los atributos que faltan -->
<img ___="foto.jpg" ___="Una foto bonita">

<a ___="https://youtube.com" ___="_blank">YouTube</a>

<input ___="text" ___="usuario" ___="Escribe tu nombre">
```

**Pistas:** `src`, `alt`, `href`, `target`, `type`, `name`, `placeholder`

---

###  Reto 5: Etiquetas Básicas de Texto

**Reto rápido:** ¡Formatea este texto!

Convierte este texto plano en HTML con el formato indicado:

```
Título Principal
Este texto debe ser importante
Este texto debe ser enfatizado
Este texto debe ser tachado
Esta es una cita corta
```

Tu código:
```html
<!-- Escribe las etiquetas correctas -->




```

---

###  Reto 6: Enlaces e Imágenes

**Reto rápido:** ¡Crea un collage de enlaces!

Crea 3 enlaces que abran en nueva pestaña:
1. A tu red social favorita
2. A un sitio de noticias
3. A un sitio educativo

```html
<!-- Tu código aquí -->




```

**Bonus:** Agrega una imagen con un enlace (que al hacer clic en la imagen te lleve a otra página).

```html
<!-- Bonus aquí -->

```

---

###  Reto 7: iframe y SVG ⭐

**Reto rápido A - iframe:** ¡Incrusta un video!

```html
<!-- Completa para incrustar un video de YouTube -->
<iframe 
    ___="560" 
    ___="315" 
    ___="https://www.youtube.com/embed/dQw4w9WgXcQ"
    ___="accelerometer; autoplay; clipboard-write"
    ___="allowfullscreen">
</iframe>
```

**Reto rápido B - SVG:** ¡Dibuja una cara feliz!

```html
<svg width="100" height="100">
    <!-- Círculo amarillo (cara) -->
    <circle cx="50" cy="50" r="40" fill="yellow"/>
    
    <!-- Ojos - agrega 2 círculos negros pequeños -->
    
    
    <!-- Sonrisa - agrega un arco o rectángulo -->
    
</svg>
```

---

###  Reto 8: Listas y Tablas

**Reto rápido A - Listas:** ¡Tu lista de compras!

Crea una lista desordenada con 4 cosas que comprar:

```html
<ul>
    <!-- Agrega 4 elementos -->
    
    
    
</ul>
```

**Reto rápido B - Tablas:** ¡Tabla de colores!

| Color | Código |
|-------|--------|
| Rojo | #FF0000 |
| Verde | #00FF00 |
| Azul | #0000FF |

```html
<table>
    <thead>
        <tr>
            <th>Color</th>
            <th>Código</th>
        </tr>
    </thead>
    <tbody>
        <!-- Completa las filas -->
        
        
        
    </tbody>
</table>
```

---

###  Reto 9: Formularios HTML Básicos

**Reto rápido:** ¡Crea un mini formulario de registro!

```html
<form>
    <!-- Campo de nombre -->
    <label>Nombre:</label>
    <input type="___" name="nombre">
    
    <!-- Campo de email -->
    <label>Email:</label>
    <input type="___" name="email">
    
    <!-- Campo de contraseña -->
    <label>Contraseña:</label>
    <input type="___" name="password">
    
    <!-- Lista desplegable de país -->
    <label>País:</label>
    <select name="pais">
        <option>Argentina</option>
        <!-- Agrega 2 países más -->
        
    </select>
    
    <!-- Botón de enviar -->
    <button type="___">Registrarse</button>
</form>
```

---

###  Reto 10: Comentarios y Estructura de Documento

**Reto rápido:** ¡Arregla este documento!

Este HTML tiene errores. Corrígelo:

```html
<!-- Encuentra y corrige 5 errores -->
<html>
<head>
    <title>Mi Página
</head>
<body>
    Esto es un comentario: <!-- Esto si está bien -->
    <h1>Bienvenido
    <p>Este es un párrafo
    <img src="logo.png">
    <!-- Falta algo importante al final -->
```

**Errores encontrados:**
1. _________________________
2. _________________________
3. _________________________
4. _________________________
5. _________________________

---

## 🚀 PARTE 2: HTML5

---

###  Reto 11: ¿Qué es HTML5?

**Reto rápido:** ¡El DOCTYPE correcto!

¿Cuál es la declaración correcta para HTML5?

A) `<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN">`
B) `<!DOCTYPE html>`
C) `<!DOCTYPE HTML5>`

**Respuesta:** _____

**Tu reto:** Escribe la estructura básica de un documento HTML5 con idioma en español.

```html
<!-- Tu código aquí -->

```

---

###  Reto 12: Estructura Básica de HTML5

**Reto rápido:** ¡Etiqueta meta obligatoria!

```html
<head>
    <meta ___="viewport" ___="width=device-width, initial-scale=1.0">
    <meta ___="UTF-8">
    <title>Mi Sitio HTML5</title>
</head>
```

**Completa los atributos:** `charset`, `name`, `content`

---

###  Reto 13: Elementos Semánticos de Estructura

**Reto rápido:** ¡Maqueta esta página!

Asigna las etiquetas semánticas correctas a cada sección:

```html
<!-- ¿Qué etiqueta va aquí? Principal de la página -->
<___>
    <h1>Mi Blog</h1>
</___>

<!-- ¿Qué etiqueta va aquí? Navegación -->
<___>
    <a href="#">Inicio</a>
    <a href="#">Artículos</a>
    <a href="#">Contacto</a>
</___>

<!-- ¿Qué etiqueta va aquí? Contenido principal -->
<___>
    <article>
        <h2>Mi primer artículo</h2>
        <p>Contenido del artículo...</p>
    </article>
</___>

<!-- ¿Qué etiqueta va aquí? Información lateral -->
<___>
    <h3>Artículos populares</h3>
    <ul>
        <li><a href="#">Artículo 1</a></li>
        <li><a href="#">Artículo 2</a></li>
    </ul>
</___>

<!-- ¿Qué etiqueta va aquí? Pie de página -->
<___>
    <p>© 2024 Mi Blog</p>
</___>
```

---

###  Reto 14: Elementos Semánticos de Contenido

**Reto rápido:** ¡Estructura un artículo!

```html
<article>
    <header>
        <h2>Las Maravillas del HTML5</h2>
        <!-- Agrega información del autor con la etiqueta correcta -->
        <p>Por: <___>María García</___></p>
        <!-- Agrega la fecha con la etiqueta correcta -->
        <___>15 de marzo, 2024</___>
    </header>
    
    <p>HTML5 trajo muchas mejoras...</p>
    
    <!-- Agrega una imagen con descripción -->
    <___>
        <img src="html5-logo.png" alt="Logo HTML5">
        <___>Logo oficial de HTML5</___>
    </___>
    
    <footer>
        <p>Etiquetas: html5, web, desarrollo</p>
    </footer>
</article>
```

---

###  Reto 15: Elementos Multimedia

**Reto rápido A - Audio:** ¡Reproductor de audio!

```html
<audio controls>
    <source src="cancion.mp3" type="audio/mpeg">
    <source src="cancion.ogg" type="audio/ogg">
    <!-- Mensaje si no soporta audio -->
    Tu navegador no soporta audio HTML5.
</audio>
```

**Reto rápido B - Video:** ¡Reproductor de video!

```html
<video ___="400" ___="300" controls poster="miniatura.jpg">
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    Tu navegador no soporta video HTML5.
</video>
```

**Reto rápido C - Tu elección:**
¿Qué atributo usarías para que un video se reproduzca automáticamente (pero silenciado)?
```html
<video autoplay _____>
```

---

###  Reto 16: Formularios HTML5 Mejorados

**Reto rápido:** ¡Nuevos tipos de input!

```html
<form>
    <!-- Email con validación automática -->
    <label>Email:</label>
    <input type="___" required>
    
    <!-- Número con rango -->
    <label>Edad:</label>
    <input type="___" min="0" max="120">
    
    <!-- Selector de fecha -->
    <label>Fecha de nacimiento:</label>
    <input type="___">
    
    <!-- Selector de color -->
    <label>Color favorito:</label>
    <input type="___">
    
    <!-- Buscador -->
    <label>Buscar:</label>
    <input type="___" placeholder="Escribe aquí...">
    
    <!-- Teléfono -->
    <label>Teléfono:</label>
    <input type="___" pattern="[0-9]{9}">
    
    <!-- Slider -->
    <label>Volumen:</label>
    <input type="___" min="0" max="100" value="50">
    
    <!-- URL -->
    <label>Sitio web:</label>
    <input type="___" placeholder="https://">
</form>
```

**Bonus:** Agrega el atributo `required` a los campos obligatorios y `placeholder` como pista.

---

###  Reto 17: APIs de HTML5

**Reto rápido:** ¡Identifica la API!

Relaciona cada API con su función:

| API | Función |
|-----|---------|
| Geolocation | ___ Obtener ubicación del usuario |
| LocalStorage | ___ Guardar datos persistentes |
| Canvas | ___ Dibujar gráficos 2D/3D |
| Drag & Drop | ___ Arrastrar y soltar elementos |
| Web Workers | ___ Ejecutar scripts en segundo plano |

**Mini reto práctico - LocalStorage:**

```javascript
// Guardar un dato
localStorage.setItem('nombre', 'Juan');

// Recuperar el dato
let nombre = localStorage.getItem('nombre');
console.log(nombre); // Muestra: Juan

// Tu reto: Escribe cómo eliminar el dato
// Pista: usa removeItem o clear
```

---

###  Reto 18: HTML4 vs HTML5

**Reto rápido:** ¡Identifica la versión!

¿Es código HTML4 o HTML5? Marca con una X:

| Código | HTML4 | HTML5 |
|--------|-------|-------|
| `<div id="header">` | ___ | ___ |
| `<header>` | ___ | ___ |
| `<input type="email">` | ___ | ___ |
| `<input type="text">` | ___ | ___ |
| `<video src="v.mp4">` | ___ | ___ |
| `<object data="v.mp4">` | ___ | ___ |
| `<canvas>` | ___ | ___ |
| `<applet>` | ___ | ___ |

---

###  Reto 19: Buenas Prácticas

**Reto rápido:** ¡Encuentra los errores!

Este código tiene 6 malas prácticas. Encuéntralas:

```html
<!doctype html>
<html>
<head>
    <TITLE>Mi Página</TITLE>
</head>
<body>
    <img src=foto.png>
    <DIV class="contenedor">
        <P>Hola mundo
        <br></br>
        <a HREF="#">click aqui</a>
        <input type="text" NAME="campo">
    </div>
</body>
</html>
```

**Malas prácticas encontradas:**
1. _________________________
2. _________________________
3. _________________________
4. _________________________
5. _________________________
6. _________________________

---

###  Reto 20: Desafío Final 🏆

**¡Crea una página completa!**

Usando todo lo aprendido, crea una página personal que incluya:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tu Nombre - Página Personal</title>
</head>
<body>
    <!-- HEADER con navegación -->
    <header>
        <h1>Tu Nombre</h1>
        <nav>
            <!-- Agrega 3 enlaces -->
        </nav>
    </header>
    
    <!-- MAIN con contenido -->
    <main>
        <!-- SECTION: Sobre mí -->
        <section>
            <h2>Sobre Mí</h2>
            <p>Escribe algo sobre ti...</p>
        </section>
        
        <!-- SECTION: Hobbies (usa una lista) -->
        <section>
            <h2>Mis Hobbies</h2>
            <!-- Crea una lista -->
        </section>
        
        <!-- ASIDE: Enlaces interesantes -->
        <aside>
            <h3>Enlaces</h3>
            <!-- Lista de enlaces -->
        </aside>
        
        <!-- ARTICLE: Tu entrada de blog -->
        <article>
            <header>
                <h2>Mi primera entrada</h2>
                <time datetime="2024-03-15">15 marzo 2024</time>
            </header>
            <p>Contenido de tu entrada...</p>
            <figure>
                <!-- Agrega una imagen -->
                <figcaption>Descripción de la imagen</figcaption>
            </figure>
        </article>
    </main>
    
    <!-- FOOTER -->
    <footer>
        <p>© 2024 Tu Nombre</p>
    </footer>
</body>
</html>
```

---

## 📋 RESPUESTAS

<details>
<summary>🖱️ Click para ver las respuestas</summary>

### Reto 1
```html
<h1>Tu Nombre Aquí</h1>
```

### Reto 2
1. Etiqueta de apertura: `<a href="https://google.com" target="_blank">`
2. Contenido: `Ir a Google`
3. Atributos: `href="https://google.com"` y `target="_blank"`
4. Etiqueta de cierre: `</a>`

### Reto 3
- `<div>` → bloque
- `<span>` → línea
- `<p>` → bloque
- `<strong>` → línea
- `<h1>` → bloque
- `<img>` → línea

### Reto 4
```html
<img src="foto.jpg" alt="Una foto bonita">
<a href="https://youtube.com" target="_blank">YouTube</a>
<input type="text" name="usuario" placeholder="Escribe tu nombre">
```

### Reto 5
```html
<h1>Título Principal</h1>
<strong>Este texto debe ser importante</strong>
<em>Este texto debe ser enfatizado</em>
<del>Este texto debe ser tachado</del>
<q>Esta es una cita corta</q>
```

### Reto 7
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" allow="accelerometer; autoplay" allowfullscreen></iframe>
```

### Reto 13
```html
<header>, <nav>, <main>, <aside>, <footer>
```

### Reto 14
```html
<address>, <time>, <figure>, <figcaption>
```

### Reto 16
```html
type="email", type="number", type="date", type="color", type="search", type="tel", type="range", type="url"
```

### Reto 18
- `<div id="header">` → HTML4
- `<header>` → HTML5
- `<input type="email">` → HTML5
- `<input type="text">` → Ambos
- `<video>` → HTML5
- `<object>` → HTML4
- `<canvas>` → HTML5
- `<applet>` → HTML4 (deprecado)

### Reto 19
1. DOCTYPE en minúsculas (debería ser `<!DOCTYPE html>`)
2. `<TITLE>` en mayúsculas (debería ser `<title>`)
3. `src=foto.png` sin comillas
4. `<DIV>` en mayúsculas
5. `<P>` sin cerrar
6. `<br></br>` incorrecto (debería ser `<br>`)
7. `HREF` en mayúsculas
8. `NAME` en mayúsculas

</details>

---

## 🌟 BONUS: Retos Extra Rápidos

### ⚡ Flash Cards HTML

**Pregunta rápida - Responde en 5 segundos:**

1. ¿Qué etiqueta se usa para saltos de línea? → `<br>`
2. ¿Qué etiqueta crea un enlace? → `<a>`
3. ¿Qué atributo especifica la URL de una imagen? → `src`
4. ¿Qué elemento semántico es para navegación? → `<nav>`
5. ¿Qué input type se usa para emails? → `email`
6. ¿Qué etiqueta dibuja en canvas? → `<canvas>`
7. ¿Qué atributo hace un campo obligatorio? → `required`
8. ¿Qué etiqueta es para contenido relacionado? → `<aside>`

---

**¡Felicitaciones por completar todos los retos! 🎉**

*Creado para practicar HTML y HTML5 de forma divertida*
