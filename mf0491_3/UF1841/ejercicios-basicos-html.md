#  Ejercicios Prácticos de HTML

---

## Instrucciones Generales
- Crea una carpeta llamada `ejercicios-html`
- Todos los ejercicios deben estar en archivos `.html` separados
- Nombra cada archivo como `ejercicio1.html`, `ejercicio2.html`, etc.

---

## Ejercicio 1: Estructura Básica 

### Objetivo
Crear la estructura fundamental de un documento HTML5.

### Tarea
Crea `ejercicio1.html` con:
1. La declaración DOCTYPE correcta para HTML5
2. El elemento `html` con el atributo de idioma en español (`lang="es"`)
3. El `head` que contenga:
   - Meta charset UTF-8
   - Un título: "Mi Primera Página"
4. El `body` con un encabezado `h1` que diga: "¡Bienvenidos a mi sitio web!"

### ✅ Verificación
- Abre el archivo en el navegador
- El título debe aparecer en la pestaña del navegador
- El encabezado debe verse en la página

---

## Ejercicio 2: Encabezados y Párrafos 

### Objetivo
Practicar con los diferentes niveles de encabezados y párrafos.

### Tarea
Crea `ejercicio2.html` con la estructura básica y dentro del `body`:

1. Un encabezado `h1` con el título: "Los Planetas del Sistema Solar"
2. Un encabezado `h2` que diga: "Planetas Interiores"
3. Un párrafo `p` que describa brevemente qué son los planetas interiores
4. Un encabezado `h2` que diga: "Planetas Exteriores"
5. Un párrafo `p` que describa brevemente qué son los planetas exteriores
6. Un encabezado `h3` que diga: "Dato Curioso"
7. Un párrafo `p` con algún dato curioso sobre el sistema solar

### ✅ Verificación
- Los encabezados deben mostrar diferentes tamaños (h1 > h2 > h3)
- Los párrafos deben estar separados por espacios

---

## Ejercicio 3: Listas

### Objetivo
Crear listas ordenadas y desordenadas.

### Tarea
Crea `ejercicio3.html` con la estructura básica y dentro del `body`:

1. Un `h1` con el texto: "Mis Cosas Favoritas"
2. Un `h2` con el texto: "Mis 3 Películas Favoritas"
3. Una lista ordenada `ol` con tus 3 películas favoritas
4. Un `h2` con el texto: "Mis Pasatiempos"
5. Una lista desordenada `ul` con al menos 4 pasatiempos
6. Un `h2` con el texto: "Mi Lista de Compras"
7. Una lista desordenada `ul` con 5 artículos de supermercado

### ✅ Verificación
- La lista ordenada debe mostrar números (1, 2, 3...)
- La lista desordenada debe mostrar viñetas (puntos)

---

## Ejercicio 4: Enlaces 

### Objetivo
Crear enlaces a otras páginas.

### Tarea
Crea `ejercicio4.html` con la estructura básica y dentro del `body`:

1. Un `h1` con el texto: "Mis Enlaces Favoritos"
2. Un `h2` con el texto: "Redes Sociales"
3. Una lista desordenada con enlaces a:
   - Google (abrir en nueva pestaña)
   - YouTube (abrir en nueva pestaña)
   - Wikipedia (abrir en nueva pestaña)
4. Un `h2` con el texto: "Mis Páginas"
5. Un párrafo que contenga un enlace a `ejercicio1.html` con el texto: "Ver mi primer ejercicio"

### Pistas
- Usa `target="_blank"` para abrir en nueva pestaña
- El atributo `href` indica la dirección del enlace

### ✅ Verificación
- Los enlaces deben ser clicables
- Los enlaces externos deben abrir en nueva pestaña
- El enlace a ejercicio1.html debe funcionar

---

## Ejercicio 5: Imágenes 

### Objetivo
Insertar imágenes en una página web.

### Tarea
Crea `ejercicio5.html` con la estructura básica y dentro del `body`:

1. Un `h1` con el texto: "Galería de Imágenes"
2. Un `h2` con el texto: "Mi Imagen Favorita"
3. Una imagen que puedes obtener de:
   - `https://picsum.photos/400/300` (imagen aleatoria)
   - O cualquier imagen de internet
4. La imagen debe tener:
   - Un texto alternativo `alt` descriptivo
   - Un ancho `width` de 400 píxeles
5. Un `h2` con el texto: "Otras Imágenes"
6. Dos imágenes más con sus respectivos textos alternativos

### Pistas
- Usa la etiqueta `<img>`
- El atributo `src` indica la ruta de la imagen
- El atributo `alt` describe la imagen (importante para accesibilidad)

### ✅ Verificación
- Las imágenes deben verse en la página
- Si pasas el mouse sobre la imagen, no debe mostrar el texto alternativo como tooltip (eso es normal en HTML5)

---

## Ejercicio 6: Estructura Semántica 

### Objetivo
Usar etiquetas semánticas de HTML5.

### Tarea
Crea `ejercicio6.html` con la siguiente estructura:

```
<header>
  └── <h1> con el nombre de una tienda ficticia
  └── <nav> con una lista de enlaces (Inicio, Productos, Contacto)

<main>
  └── <section>
      └── <h2> Bienvenidos
      └── <p> descripción de la tienda
  
  └── <section>
      └── <h2> Nuestros Productos
      └── <article>
          └── <h3> Producto 1
          └── <p> descripción del producto
          └── <p> Precio: $XX
      └── <article>
          └── <h3> Producto 2
          └── <p> descripción del producto
          └── <p> Precio: $XX

  └── <aside>
      └── <h3> Ofertas Especiales
      └── <p> información de ofertas

<footer>
  └── <p> con copyright y año actual
```

### Etiquetas semánticas a usar:
- `<header>` - encabezado de la página
- `<nav>` - navegación
- `<main>` - contenido principal
- `<section>` - secciones del contenido
- `<article>` - contenido independiente
- `<aside>` - contenido relacionado/secundario
- `<footer>` - pie de página

### ✅ Verificación
- La estructura debe seguir el esquema indicado
- Todos los elementos deben estar correctamente anidados

---

## Ejercicio 7 - Mi Página Personal (Opcional)

### Desafío
Crea `mipagina.html` con una página personal que incluya:
- Una foto (puede ser de internet)
- Tu nombre como título
- Una breve biografía (2-3 párrafos)
- Una lista de tus habilidades
- Una lista de tus redes sociales como enlaces
- Una cita motivadora favorita

### Pista
Puedes usar la etiqueta `<blockquote>` para citas.

---

## 📚 Resumen de Etiquetas Aprendidas

| Etiqueta | Uso |
|----------|-----|
| `<!DOCTYPE html>` | Declaración de documento HTML5 |
| `<html>` | Contenedor raíz |
| `<head>` | Metadatos del documento |
| `<body>` | Contenido visible |
| `<h1>` a `<h6>` | Encabezados |
| `<p>` | Párrafos |
| `<ul>` | Lista desordenada |
| `<ol>` | Lista ordenada |
| `<li>` | Elemento de lista |
| `<a>` | Enlaces |
| `<img>` | Imágenes |

---
