#  Ejercicios Prácticos de CSS - Selectores


---

## Instrucciones Generales
- Crea una carpeta llamada `ejercicios-css`
- Dentro de ella, crea los archivos que se indican en cada ejercicio
- Vincula siempre el CSS al HTML con: `<link rel="stylesheet" href="styles.css">`

---

## Ejercicio 1: Selector Universal y de Elemento 

### Objetivo
Entender los selectores más básicos.

### Tarea
Crea `ejercicio1.html` y `styles.css`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 1 - Selectores Básicos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Los Selectores en CSS</h1>
    <p>El selector universal afecta a todos los elementos.</p>
    <p>El selector de elemento afecta solo a las etiquetas indicadas.</p>
    <h2>Subtítulo Importante</h2>
    <p>Este es otro párrafo para practicar.</p>
</body>
</html>
```

**CSS - Aplica estos estilos:**
1. Con el **selector universal** `*`:
   - Margen 0 y padding 0
   - Fuente Arial
2. Con el **selector de elemento** para `h1`:
   - Color de texto azul (`#2980b9`)
3. Con el **selector de elemento** para `h2`:
   - Color de texto verde (`#27ae60`)
4. Con el **selector de elemento** para `p`:
   - Tamaño de fuente 16px
   - Color de texto gris oscuro (`#333`)

### ✅ Verificación
- Todos los elementos deben usar fuente Arial
- Los encabezados deben tener colores diferentes
- Los párrafos deben ser grises y de 16px

---

## Ejercicio 2: Selector de Clase 

### Objetivo
Aprender a usar clases para aplicar estilos específicos.

### Tarea
Crea `ejercicio2.html` y actualiza `styles.css`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 2 - Clases</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Frutas del Mundo</h1>
    
    <p class="destacado">Las frutas son muy saludables.</p>
    
    <h2 class="destacado">Frutas Cítricas</h2>
    <p>El limón y la naranja son cítricos.</p>
    
    <h2>Frutas Tropicales</h2>
    <p class="destacado">El mango y la piña son tropicales.</p>
    
    <p class="_importante">Consulta con tu médico antes de cambiar tu dieta.</p>
</body>
</html>
```

**CSS - Crea las siguientes clases:**
1. Clase `.destacado`:
   - Fondo amarillo claro (`#fff3cd`)
   - Padding de 10px
   - Borde izquierdo de 4px sólido naranja (`#f39c12`)
2. Clase `.importante`:
   - Fondo rojo claro (`#f8d7da`)
   - Padding de 10px
   - Borde izquierdo de 4px sólido rojo (`#e74c3c`)
   - Texto en negrita (`font-weight: bold`)

### ✅ Verificación
- Los elementos con clase "destacado" deben tener fondo amarillo
- La clase se puede aplicar a diferentes elementos (h2 y p)
- El aviso importante debe tener fondo rojo y texto en negrita

---

## Ejercicio 3: Selector de ID 

### Objetivo
Diferenciar entre selectores de clase e ID.

### Tarea
Crea `ejercicio3.html`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 3 - IDs</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header id="cabecera">
        <h1>Mi Blog Personal</h1>
        <p>Un espacio para compartir ideas</p>
    </header>
    
    <main id="contenido-principal">
        <h2>Última Entrada</h2>
        <p>Este es el contenido de mi artículo...</p>
    </main>
    
    <footer id="pie-pagina">
        <p>© 2025 Mi Blog - Todos los derechos reservados</p>
    </footer>
</body>
</html>
```

**CSS - Aplica estilos usando selectores de ID:**
1. `#cabecera`:
   - Fondo azul oscuro (`#2c3e50`)
   - Texto blanco
   - Padding de 20px
   - Texto centrado
2. `#contenido-principal`:
   - Padding de 20px
   - Fondo blanco
3. `#pie-pagina`:
   - Fondo gris oscuro (`#34495e`)
   - Texto blanco
   - Texto centrado
   - Padding de 15px

### ✅ Verificación
- Cada sección debe tener su estilo único
- Recuerda: **un ID es único** (solo se usa una vez por página)

---

## Ejercicio 4: Selectores Descendentes y de Hijo 

### Objetivo
Comprender la diferencia entre seleccionar descendentes e hijos directos.

### Tarea
Crea `ejercicio4.html`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 4 - Descendentes e Hijos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <article>
        <h2>Artículo Principal</h2>
        <p>Este es un párrafo dentro del artículo.</p>
        <div>
            <p>Este párrafo está dentro de un div, dentro del artículo.</p>
        </div>
    </article>
    
    <section>
        <h2>Sección Secundaria</h2>
        <p>Este párrafo está en una sección.</p>
        <ul>
            <li>Elemento 1</li>
            <li>Elemento 2</li>
            <li>Elemento 3</li>
        </ul>
    </section>
    
    <aside>
        <p>Este párrafo está en un aside.</p>
    </aside>
</body>
</html>
```

**CSS - Aplica estos estilos:**
1. **Selector descendente** `article p`:
   - Todos los `p` dentro de `article` (sin importar el nivel)
   - Color azul (`#3498db`)
   - Fondo azul muy claro (`#e8f4fc`)

2. **Selector de hijo directo** `section > p`:
   - Solo los `p` que son hijos **directos** de `section`
   - Color verde (`#27ae60`)
   - Fondo verde muy claro (`#e8f8f0`)

3. **Selector descendente** `section li`:
   - Color púrpura (`#9b59b6`)

4. **Selector de elemento** `aside p`:
   - Color naranja (`#e67e22`)
   - Estilo cursiva (`font-style: italic`)

### ✅ Verificación
- El párrafo dentro del `div` (que está en `article`) también debe ser azul
- Solo el párrafo hijo directo de `section` debe ser verde
- Los elementos de la lista deben ser púrpura

---

## Ejercicio 5: Pseudoclases 

### Objetivo
Usar pseudoclases para estados especiales.

### Tarea
Crea `ejercicio5.html`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 5 - Pseudoclases</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Enlaces Interactivos</h1>
    
    <nav>
        <a href="#">Inicio</a>
        <a href="#">Servicios</a>
        <a href="#">Nosotros</a>
        <a href="#">Contacto</a>
    </nav>
    
    <h2>Lista de Tareas</h2>
    <ul class="tareas">
        <li>Estudiar HTML</li>
        <li>Practicar CSS</li>
        <li>Aprender JavaScript</li>
        <li>Hacer un proyecto</li>
        <li>Repasar conceptos</li>
    </ul>
    
    <h2>Párrafos Demostrativos</h2>
    <p>Primer párrafo del texto.</p>
    <p>Segundo párrafo del texto.</p>
    <p>Tercer párrafo del texto.</p>
    <p>Cuarto párrafo del texto.</p>
</body>
</html>
```

**CSS - Aplica las siguientes pseudoclases:**
1. Enlaces (`a`):
   - Color normal: azul (`#2980b9`)
   - Sin subrayado
   - Al pasar el mouse (`:hover`): subrayado y color más oscuro
   - Cuando está activo (`:active`): color rojo

2. Lista de tareas (`.tareas li`):
   - Primer elemento (`:first-child`): color verde, en negrita
   - Último elemento (`:last-child`): color rojo, en negrita
   - Elementos pares (`:nth-child(even)`): fondo gris claro (`#f0f0f0`)
   - Elementos impares (`:nth-child(odd)`): fondo blanco

3. Párrafos:
   - Primer párrafo (`p:first-of-type`): letra capital (tamaño 24px)
   - Último párrafo (`p:last-of-type`): borde inferior punteado

### ✅ Verificación
- Los enlaces deben responder al hover
- El primer y último elemento de la lista deben destacarse
- Las filas pares de la lista deben tener fondo gris

---

## Ejercicio 6: Selectores de Atributo 

### Objetivo
Seleccionar elementos basándose en sus atributos.

### Tarea
Crea `ejercicio6.html`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 6 - Atributos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Tipos de Enlaces</h1>
    
    <ul>
        <li><a href="https://google.com">Enlace externo (https)</a></li>
        <li><a href="mailto:correo@ejemplo.com">Enviar email</a></li>
        <li><a href="#seccion1">Ir a sección</a></li>
        <li><a href="documento.pdf" download>Descargar PDF</a></li>
        <li><a href="https://youtube.com" target="_blank">Abrir en nueva pestaña</a></li>
    </ul>
    
    <section id="seccion1">
        <h2>Formulario de Ejemplo</h2>
        <form>
            <input type="text" placeholder="Tu nombre">
            <input type="email" placeholder="Tu email">
            <input type="password" placeholder="Contraseña">
            <input type="submit" value="Enviar">
            <button type="button">Cancelar</button>
        </form>
    </section>
</body>
</html>
```

**CSS - Usa selectores de atributo:**
1. Enlaces que empiezan con "https" (`a[href^="https"]`):
   - Color verde (`#27ae60`)
   - Agregar ícono de candado con `::after`: contenido "🔒"

2. Enlaces de email (`a[href^="mailto"]`):
   - Color naranja (`#e67e22`)

3. Enlaces de descarga (`a[download]`):
   - Color púrpura (`#9b59b6`)
   - Fondo púrpura claro

4. Enlaces con target blank (`a[target="_blank"]`):
   - Agregar `::after` con contenido "↗" (indica que abre fuera)

5. Inputs de tipo texto/email (`input[type="text"], input[type="email"]`):
   - Padding 10px
   - Borde 2px sólido gris
   - Borde azul al enfocar (`:focus`)

6. Inputs de tipo password (`input[type="password"]`):
   - Fondo gris muy claro

7. Botones (`input[type="submit"], button`):
   - Fondo azul
   - Texto blanco
   - Padding 10px 20px
   - Sin borde
   - Cursor pointer

### ✅ Verificación
- Los enlaces externos deben ser verdes
- Los enlaces de email deben ser naranjas
- Los inputs deben responder al focus

---

## Ejercicio 7: Combinando Selectores 

### Objetivo
Practicar la combinación de múltiples selectores.

### Tarea
Crea `ejercicio7.html`:

**HTML:**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Ejercicio 7 - Combinación</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Tienda Online</h1>
    
    <div class="productos">
        <article class="producto destacado">
            <h3>Producto Premium</h3>
            <p class="precio">$99.99</p>
        </article>
        
        <article class="producto">
            <h3>Producto Normal</h3>
            <p class="precio">$49.99</p>
        </article>
        
        <article class="producto destacado">
            <h3>Otro Premium</h3>
            <p class="precio">$129.99</p>
        </article>
    </div>
    
    <div class="ofertas">
        <article class="producto">
            <h3>Producto en Oferta</h3>
            <p class="precio">$19.99</p>
        </article>
    </div>
</body>
</html>
```

**CSS - Combina selectores:**
1. Todos los `.producto`:
   - Fondo blanco
   - Padding 15px
   - Margen inferior 10px
   - Borde 1px sólido gris claro

2. Solo `.producto.destacado` (tiene AMBAS clases):
   - Borde dorado (`#f1c40f`) de 2px
   - Fondo amarillo muy claro

3. `.productos .producto` (solo productos dentro de .productos):
   - Ancho 300px

4. `.ofertas .producto`:
   - Fondo rojo muy claro (`#ffe6e6`)
   - Borde rojo (`#e74c3c`)

5. `.producto .precio`:
   - Tamaño de fuente 20px
   - Color verde oscuro (`#1e8449`)
   - En negrita

6. `.destacado .precio`:
   - Color rojo (`#e74c3c`)
   - Texto "¡Oferta!" antes del precio con `::before`

### ✅ Verificación
- Los productos destacados deben tener borde dorado
- Los productos en ofertas deben tener fondo rojizo
- Los precios de destacados deben ser rojos

---

## 📋 Resumen de Selectores CSS

| Selector | Ejemplo | Qué selecciona |
|----------|---------|----------------|
| Universal | `*` | Todos los elementos |
| Elemento | `p` | Todos los `<p>` |
| Clase | `.destacado` | Elementos con esa clase |
| ID | `#cabecera` | Elemento con ese ID (único) |
| Descendente | `article p` | `<p>` dentro de `<article>` |
| Hijo directo | `section > p` | `<p>` hijo directo de `<section>` |
| Atributo | `a[target]` | Elementos con ese atributo |
| Atributo con valor | `input[type="text"]` | Inputs de tipo texto |
| Atributo comienza con | `a[href^="https"]` | Enlaces que empiezan con https |
| Múltiples clases | `.clase1.clase2` | Elementos con AMBAS clases |
| Agrupación | `h1, h2, h3` | Todos esos elementos |

---





## 💡 Consejos para Recordar

1. **Clase (.)** → Se puede usar **múltiples veces** en una página
2. **ID (#)** → Se usa **solo una vez** por página
3. **Descendente (espacio)** → Cualquier nivel de profundidad
4. **Hijo directo (>)** → Solo el primer nivel de profundidad
5. **Agrupación (,)** → Mismos estilos para varios selectores
6. **Múltiples clases (sin espacio)** → Elemento debe tener TODAS las clases

---

¡Buena suerte! 🚀
