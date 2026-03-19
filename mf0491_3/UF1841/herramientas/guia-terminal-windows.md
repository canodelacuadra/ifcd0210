# Guía de Introducción a la Terminal para Desarrollo Web

## Introducción

La terminal es una de las herramientas más poderosas con las que cuenta un desarrollador web. Aunque las interfaces gráficas modernas han simplificado muchas tareas, dominar la línea de comandos te permitirá trabajar de manera más eficiente, automatizar procesos repetitivos y acceder a funcionalidades avanzadas que no están disponibles en las interfaces visuales. En el mundo del desarrollo profesional, la terminal es una herramienta indispensable que todo programador debe dominar, independientemente del lenguaje o framework que utilice.

Para los desarrolladores que trabajan en Windows, la instalación de Git incluye **Git Bash**, una terminal que emula el comportamiento de las terminales Unix/Linux. Esto es especialmente útil porque la mayoría de los servidores web y entornos de producción funcionan con sistemas basados en Unix, por lo que aprender los comandos en este entorno te preparará para escenarios reales de desarrollo y despliegue de aplicaciones.

---

## ¿Qué es la Terminal?

La terminal, también conocida como línea de comandos, consola o shell, es una interfaz de texto que permite interactuar directamente con el sistema operativo mediante comandos escritos. A diferencia de las interfaces gráficas donde haces clic en iconos y menús, en la terminal escribes instrucciones específicas que el sistema ejecuta inmediatamente. Esta forma de interacción puede parecer intimidante al principio, pero ofrece un control mucho más preciso y directo sobre el sistema.

En Windows, la terminal predeterminada es el **Símbolo del sistema (cmd.exe)** o **PowerShell**, pero al instalar Git obtenemos **Git Bash**, que proporciona un entorno similar a Linux. Esto es particularmente valioso para desarrolladores web porque la mayoría de las herramientas modernas de desarrollo (Node.js, npm, webpack, etc.) están diseñadas pensando en entornos Unix, y sus comandos funcionan mejor en Git Bash que en la terminal nativa de Windows.

### Ventajas de usar la terminal

- **Velocidad**: Escribir comandos suele ser más rápido que navegar por menús y ventanas, especialmente para tareas repetitivas.
- **Automatización**: Puedes crear scripts que ejecuten múltiples comandos en secuencia, ahorrando horas de trabajo manual.
- **Acceso remoto**: La terminal es la herramienta principal para conectarse a servidores remotos mediante SSH.
- **Control total**: Tienes acceso a todas las funcionalidades del sistema, incluyendo opciones avanzadas no disponibles en interfaces gráficas.
- **Portabilidad**: Los comandos que aprendas funcionarán en cualquier sistema Linux/Unix, lo que es esencial para desarrollo web profesional.

---

## Abrir Git Bash en Windows

Para comenzar a trabajar con la terminal, primero necesitas abrir Git Bash. Existen varias formas de hacerlo, y es útil conocerlas todas para poder acceder rápidamente a la terminal desde diferentes contextos:

### Método 1: Desde el menú de inicio
1. Haz clic en el botón de **Inicio** de Windows
2. Escribe "Git Bash" en el buscador
3. Haz clic en **Git Bash** en los resultados
4. La terminal se abrirá lista para recibir comandos

### Método 2: Desde el menú contextual (recomendado)
1. Abre el Explorador de Archivos de Windows
2. Navega hasta la carpeta donde quieras trabajar
3. Haz clic derecho en un espacio vacío de la carpeta
4. Selecciona **"Git Bash Here"** del menú contextual
5. La terminal se abrirá ya posicionada en esa carpeta

Este segundo método es muy recomendado porque te ahorra el paso de navegar hasta la carpeta deseada después de abrir la terminal. Es una práctica común entre desarrolladores y acelera significativamente el flujo de trabajo diario.

---

## Conceptos Fundamentales

Antes de profundizar en los comandos específicos, es importante entender algunos conceptos básicos que te ayudarán a comprender cómo funciona la terminal y cómo interactuar con ella de manera efectiva.

### El prompt

El **prompt** es el texto que aparece al inicio de cada línea en la terminal, justo antes del cursor. Te indica que la terminal está lista para recibir un comando. En Git Bash, el prompt tiene generalmente este formato:

```
usuario@nombre-equipo MINGW64 ~/carpeta_actual
$
```

La información que muestra incluye:
- **usuario**: Tu nombre de usuario en el sistema
- **nombre-equipo**: El nombre de tu computadora
- **MINGW64**: Indica que estás usando el entorno MinGW (Git Bash)
- **~/carpeta_actual**: La ruta de la carpeta donde te encuentras (el directorio de trabajo)

### Directorio de trabajo (Current Working Directory)

El directorio de trabajo es la carpeta donde "estás parado" en ese momento. Todos los comandos que ejecutes que involucren archivos (crear, eliminar, copiar) operarán en esta carpeta por defecto, a menos que especifiques otra ruta. Saber siempre en qué directorio estás es fundamental para evitar errores como borrar archivos equivocados.

### Rutas absolutas y relativas

Las **rutas** son direcciones que indican la ubicación de archivos y carpetas en el sistema:

- **Ruta absoluta**: Indica la ubicación completa desde la raíz del sistema de archivos. En Windows con Git Bash, la raíz suele ser `C:/` o `/c/`. Ejemplo: `/c/Users/TuUsuario/Proyectos/mi-web`
  
- **Ruta relativa**: Indica la ubicación partiendo desde el directorio actual donde te encuentras. Es más corta y conveniente. Ejemplo: si estás en `/c/Users/TuUsuario` y quieres ir a `Proyectos/mi-web`, la ruta relativa es simplemente `Proyectos/mi-web`

### Caracteres especiales en rutas

- `~` (tilde): Representa tu directorio personal (home), generalmente `C:\Users\TuUsuario`
- `.` (punto): Representa el directorio actual
- `..` (dos puntos): Representa el directorio padre (la carpeta que contiene la actual)
- `/` (barra): Separa las carpetas en la ruta (en Git Bash se usa estilo Unix)

---

## Comandos Básicos de Navegación

Los comandos de navegación te permiten moverte por el sistema de archivos, explorar carpetas y conocer tu ubicación actual. Son los comandos que más utilizarás en tu día a día como desarrollador, así que es fundamental dominarlos completamente.

### `pwd` - Print Working Directory (Mostrar directorio actual)

El comando `pwd` te muestra la ruta absoluta del directorio donde te encuentras actualmente. Es muy útil cuando no estás seguro de tu ubicación en el sistema de archivos.

```bash
pwd
```

**Ejemplo de salida:**
```
/c/Users/Maria/Proyectos
```

Este comando no acepta parámetros y simplemente devuelve la ruta completa de tu ubicación actual. Úsalo siempre que necesites confirmar dónde estás antes de ejecutar comandos que modifiquen archivos.

### `ls` - List (Listar contenido)

El comando `ls` muestra el contenido del directorio actual (archivos y carpetas). Es uno de los comandos más utilizados y tiene varias opciones útiles que te permiten ver información adicional.

```bash
ls                  # Lista básica del contenido
ls -l               # Lista con información detallada (permisos, tamaño, fecha)
ls -a               # Lista incluyendo archivos ocultos (que empiezan con .)
ls -la              # Combina -l y -a para ver todo con detalle
ls -lh              # Lista con tamaños en formato legible (KB, MB, GB)
ls carpeta/         # Lista el contenido de una carpeta específica
```

**Ejemplo de salida de `ls -la`:**
```
total 24
drwxr-xr-x 1 Maria 197121 0 mar 20 10:30 .
drwxr-xr-x 1 Maria 197121 0 mar 20 09:15 ..
-rw-r--r-- 1 Maria 197121 256 mar 20 10:30 index.html
drwxr-xr-x 1 Maria 197121 0 mar 20 10:25 css
drwxr-xr-x 1 Maria 197121 0 mar 20 10:22 js
```

La primera letra de cada línea indica el tipo: `d` para directorio (carpeta) y `-` para archivo. Los permisos se muestran como `rwx` (lectura, escritura, ejecución) para usuario, grupo y otros respectivamente.

### `cd` - Change Directory (Cambiar directorio)

El comando `cd` te permite navegar entre carpetas. Es probablemente el comando que más utilizarás, así que practica sus diferentes usos hasta que te resulten naturales.

```bash
cd Proyectos           # Entra a la carpeta "Proyectos" (ruta relativa)
cd /c/Users/Maria      # Va a la ruta absoluta especificada
cd ~                   # Va al directorio personal (home)
cd ..                  # Sube un nivel (al directorio padre)
cd ../..               # Sube dos niveles
cd -                   # Va al directorio anterior (útil para alternar)
cd                     # Sin argumentos, va al directorio personal
```

**Consejo práctico:** Puedes escribir las primeras letras de una carpeta y presionar **Tab** para que la terminal complete automáticamente el nombre. Esto ahorra tiempo y evita errores de escritura.

### Ejercicios prácticos de navegación

1. Abre Git Bash y ejecuta `pwd` para ver dónde estás
2. Ejecuta `ls` para ver qué carpetas hay en tu ubicación actual
3. Usa `cd` para entrar a una carpeta, luego `pwd` para confirmar
4. Usa `cd ..` para volver atrás
5. Prueba `cd ~` para ir a tu carpeta personal
6. Experimenta con `ls -la` y observa la información detallada

---

## Comandos de Manipulación de Archivos y Carpetas

Una vez que sabes navegar por el sistema de archivos, el siguiente paso es aprender a crear, copiar, mover y eliminar archivos y carpetas. Estos son comandos esenciales para cualquier desarrollador, ya que constantemente necesitarás organizar tus proyectos y gestionar archivos de código.

### `mkdir` - Make Directory (Crear carpeta)

El comando `mkdir` crea nuevas carpetas (directorios). Puedes crear una o varias carpetas a la vez, e incluso crear estructuras completas de carpetas anidadas con una sola instrucción.

```bash
mkdir mi-proyecto              # Crea una carpeta llamada "mi-proyecto"
mkdir css js images            # Crea tres carpetas a la vez
mkdir -p src/components/Header # Crea toda la estructura de carpetas
                               # (-p crea las carpetas padre si no existen)
```

La opción `-p` (parents) es particularmente útil cuando quieres crear una estructura de carpetas anidada. Sin esta opción, si intentas crear `src/components/Header` y la carpeta `src` no existe, obtendrás un error. Con `-p`, la terminal crea automáticamente todas las carpetas necesarias en la ruta.

### `touch` - Crear archivos vacíos

El comando `touch` crea archivos vacíos. Es muy útil para crear rápidamente la estructura básica de un proyecto web con sus archivos HTML, CSS y JavaScript.

```bash
touch index.html               # Crea un archivo HTML vacío
touch styles.css script.js     # Crea dos archivos a la vez
touch css/styles.css           # Crea un archivo en una carpeta específica
```

El nombre "touch" viene de la función original del comando, que era "tocar" un archivo para actualizar su fecha de modificación. Si el archivo no existe, lo crea vacío como comportamiento secundario que se ha vuelto su uso principal.

### `cp` - Copy (Copiar)

El comando `cp` copia archivos y carpetas. Es importante dominar sus opciones para poder realizar copias de manera eficiente y segura.

```bash
cp archivo.txt copia.txt           # Copia un archivo
cp archivo.txt carpeta/            # Copia un archivo a una carpeta
cp archivo.txt carpeta/nuevo.txt   # Copia y renombra al mismo tiempo
cp -r carpeta1 carpeta2            # Copia una carpeta completa (-r = recursivo)
cp *.html backup/                  # Copia todos los archivos HTML
```

La opción `-r` (recursive) es necesaria para copiar carpetas, ya que sin ella el comando solo copia archivos individuales. Ten en cuenta que al copiar carpetas, todos los archivos y subcarpetas que contengan también se copian.

### `mv` - Move (Mover/Renombrar)

El comando `mv` tiene doble función: mover archivos a otra ubicación y renombrar archivos. El comportamiento depende de los argumentos que uses.

```bash
mv archivo.txt carpeta/            # Mueve el archivo a la carpeta
mv archivo.txt nuevo-nombre.txt    # Renombra el archivo
mv carpeta1 carpeta2               # Mueve/renombra una carpeta
mv *.js scripts/                   # Mueve todos los archivos JS
```

Es importante entender que en los sistemas de archivos, mover y renombrar son técnicamente la misma operación: cambiar la ruta del archivo. Si cambias solo el nombre del archivo, es un renombrado; si cambias la carpeta, es un movimiento.

### `rm` - Remove (Eliminar)

El comando `rm` elimina archivos y carpetas. **¡Cuidado!** Los archivos eliminados con `rm` no van a la papelera de reciclaje, se eliminan permanentemente. Este comando requiere precaución y es buena práctica verificar siempre el directorio actual antes de usarlo.

```bash
rm archivo.txt                 # Elimina un archivo
rm archivo1.txt archivo2.txt   # Elimina varios archivos
rm -i archivo.txt              # Pide confirmación antes de eliminar
rm -r carpeta                  # Elimina una carpeta y todo su contenido
rm -rf carpeta                 # Elimina sin pedir confirmación (¡usar con cuidado!)
rm *.log                       # Elimina todos los archivos con extensión .log
```

La opción `-i` (interactive) es muy recomendada para principiantes, ya que pide confirmación antes de cada eliminación. Esto puede salvarte de borrar archivos importantes por error. La opción `-f` (force) evita confirmaciones y debe usarse con extrema precaución.

### Ejercicio práctico: Crear estructura de proyecto web

Vamos a crear la estructura típica de un proyecto web:

```bash
# 1. Crear la carpeta principal
mkdir mi-sitio-web

# 2. Entrar a la carpeta
cd mi-sitio-web

# 3. Crear subcarpetas
mkdir css js images

# 4. Crear archivos principales
touch index.html
touch css/styles.css
touch js/script.js

# 5. Verificar la estructura creada
ls -la
ls -la css/
ls -la js/

# 6. Crear una copia de seguridad
mkdir backup
cp index.html backup/
cp -r css backup/
cp -r js backup/
```

---

## Comandos de Visualización de Contenido

A menudo necesitarás ver el contenido de archivos sin abrir un editor de texto completo. Los comandos de visualización te permiten inspeccionar archivos rápidamente, lo cual es especialmente útil para archivos de configuración, logs o código fuente.

### `cat` - Concatenate (Mostrar contenido completo)

El comando `cat` muestra el contenido completo de un archivo en la terminal. Es ideal para archivos pequeños que puedes leer de una vez.

```bash
cat index.html             # Muestra el contenido del archivo
cat archivo1.txt archivo2.txt   # Muestra varios archivos en secuencia
cat -n archivo.txt         # Muestra con números de línea
```

El nombre "cat" viene de "concatenate" (concatenar), porque originalmente se usaba para unir archivos. Sin embargo, su uso más común hoy en día es simplemente mostrar el contenido de un archivo.

### `head` y `tail` - Ver inicio y final

Estos comandos son útiles para archivos grandes donde solo necesitas ver el principio o el final. `head` muestra las primeras líneas y `tail` muestra las últimas.

```bash
head archivo.txt           # Muestra las primeras 10 líneas
head -n 20 archivo.txt     # Muestra las primeras 20 líneas
tail archivo.txt           # Muestra las últimas 10 líneas
tail -n 20 archivo.txt     # Muestra las últimas 20 líneas
tail -f log.txt            # Muestra las últimas líneas y actualiza en tiempo real
```

La opción `-f` (follow) de `tail` es especialmente útil para monitorear archivos de log que se actualizan constantemente, como los logs de un servidor web. La terminal se queda "escuchando" y muestra cada nueva línea que se añade al archivo.

### `less` - Navegar por archivos grandes

Para archivos muy extensos, `less` permite navegar por el contenido de forma interactiva, usando las flechas del teclado o las teclas de navegación.

```bash
less archivo-grande.txt
```

Dentro de `less`, puedes usar:
- **Flechas arriba/abajo**: Navegar línea por línea
- **Espacio**: Avanzar una página
- **b**: Retroceder una página
- **/texto**: Buscar "texto" en el archivo
- **n**: Ir a la siguiente coincidencia de búsqueda
- **q**: Salir de less

### `wc` - Word Count (Contar)

El comando `wc` cuenta líneas, palabras y caracteres de un archivo. Es útil para obtener estadísticas rápidas de archivos de código o texto.

```bash
wc archivo.txt             # Muestra líneas, palabras y caracteres
wc -l archivo.txt          # Solo cuenta líneas
wc -w archivo.txt          # Solo cuenta palabras
wc -c archivo.txt          # Solo cuenta caracteres
wc *.html                  # Cuenta todos los archivos HTML
```

---

## Permisos y el Comando `chmod`

En sistemas Unix/Linux, cada archivo tiene permisos que determinan quién puede leerlo, escribirlo o ejecutarlo. Aunque Windows maneja permisos de forma diferente, Git Bash emula este sistema, y es importante conocerlo porque muchos servidores web usan Linux.

### Entendiendo los permisos

Los permisos se dividen en tres categorías:
- **Usuario (u)**: El propietario del archivo
- **Grupo (g)**: Usuarios del mismo grupo
- **Otros (o)**: Todos los demás usuarios

Y tres tipos de acceso:
- **Lectura (r)**: Ver el contenido del archivo
- **Escritura (w)**: Modificar el archivo
- **Ejecución (x)**: Ejecutar el archivo como programa

### Sintaxis de `chmod`

```bash
chmod +x script.sh         # Da permiso de ejecución a todos
chmod u+x script.sh        # Da permiso de ejecución solo al usuario
chmod g-w archivo.txt      # Quita permiso de escritura al grupo
chmod 755 script.sh        # Permisos con notación numérica
chmod 644 archivo.txt      # Permisos comunes para archivos de texto
```

### Notación numérica de permisos

La notación numérica usa tres dígitos donde cada uno representa una suma:
- **4** = lectura (r)
- **2** = escritura (w)
- **1** = ejecución (x)

Por ejemplo, `755` significa:
- **7** (4+2+1) = rwx para el usuario
- **5** (4+0+1) = r-x para el grupo
- **5** (4+0+1) = r-x para otros

Esta notación es muy común en servidores Linux y es importante entenderla para configurar correctamente los permisos de archivos en producción.

---

## Atajos de Teclado Esenciales

Dominar los atajos de teclado de la terminal acelerará significativamente tu flujo de trabajo. Estos atajos funcionan en Git Bash y en la mayoría de terminales Unix/Linux, por lo que te servirán en cualquier entorno de desarrollo.

### Navegación y edición

| Atajo | Función |
|-------|---------|
| `Tab` | Autocompleta nombres de archivos y carpetas |
| `Ctrl + A` | Mueve el cursor al inicio de la línea |
| `Ctrl + E` | Mueve el cursor al final de la línea |
| `Ctrl + U` | Borra desde el cursor hasta el inicio de la línea |
| `Ctrl + K` | Borra desde el cursor hasta el final de la línea |
| `Ctrl + W` | Borra la palabra anterior al cursor |
| `Ctrl + L` | Limpia la pantalla (equivale a `clear`) |
| `Ctrl + C` | Cancela el comando actual o proceso en ejecución |

### Historial de comandos

| Atajo | Función |
|-------|---------|
| `Flecha arriba` | Navega hacia atrás en el historial de comandos |
| `Flecha abajo` | Navega hacia adelante en el historial |
| `Ctrl + R` | Búsqueda inversa en el historial |
| `history` | Muestra el historial completo de comandos |
| `!n` | Ejecuta el comando número n del historial |
| `!!` | Repite el último comando ejecutado |

El autocompletado con `Tab` es probablemente el atajo más útil. Si escribes `cd Pro` y presionas Tab, la terminal completará a `cd Proyectos` si es la única carpeta que empieza con "Pro". Si hay varias coincidencias, presiona Tab dos veces para ver todas las opciones.

---

## Wildcards (Comodines)

Los comodines son caracteres especiales que permiten seleccionar múltiples archivos con un solo patrón. Son extremadamente útiles para operaciones en lote y pueden ahorrarte mucho tiempo.

### El asterisco `*`

El asterisco coincide con cualquier cantidad de caracteres (incluyendo ninguno):

```bash
ls *.html              # Lista todos los archivos HTML
rm *.log               # Elimina todos los archivos .log
cp *.css backup/       # Copia todos los archivos CSS
mv proyecto-* backup/  # Mueve todos los archivos que empiezan con "proyecto-"
```

### El signo de interrogación `?`

El signo de interrogación coincide con exactamente un carácter:

```bash
ls imagen?.jpg         # Lista imagen1.jpg, imagen2.jpg, imagenA.jpg, etc.
ls archivo?.txt        # Coincide con archivo1.txt pero no archivo10.txt
```

### Corchetes `[]`

Los corchetes coinciden con uno de los caracteres especificados:

```bash
ls archivo[123].txt    # Coincide con archivo1.txt, archivo2.txt o archivo3.txt
ls imagen[A-Z].jpg     # Coincide con cualquier letra mayúscula
ls *[aeiou].txt        # Archivos que terminan en vocal
ls archivo[!0-9].txt   # Archivos que NO terminan en número
```

### Ejemplos prácticos combinados

```bash
# Copiar todos los archivos de código fuente
cp *.{html,css,js} src/

# Eliminar archivos temporales
rm *.tmp *.bak *.log

# Listar imágenes
ls *.{jpg,png,gif,svg}

# Mover archivos numerados
mv foto[0-9][0-9].jpg imagenes/
```

---

## Redirección y Pipes

Una de las características más poderosas de la terminal es la capacidad de redirigir la salida de un comando a otro, o a un archivo. Esto te permite crear "cadenas" de procesamiento de datos muy sofisticadas.

### Redirección de salida

```bash
# Guardar salida en un archivo (sobrescribe)
ls > lista-archivos.txt

# Añadir salida a un archivo existente
echo "Nueva línea" >> notas.txt

# Redirección de errores
comando 2> errores.log

# Redirección de salida y errores
comando > salida.log 2>&1
```

### Pipes (Tuberías)

El símbolo `|` permite conectar la salida de un comando con la entrada de otro, creando flujos de procesamiento de datos:

```bash
# Contar archivos en una carpeta
ls | wc -l

# Buscar en el historial
history | grep "git"

# Ver archivos que contienen cierta palabra
ls -la | grep "css"

# Ordenar y eliminar duplicados
cat datos.txt | sort | uniq

# Procesamiento complejo
cat log.txt | grep "ERROR" | wc -l
```

### El comando `grep`

`grep` es un comando de búsqueda extremadamente potente que busca patrones de texto en archivos:

```bash
grep "function" script.js       # Busca "function" en el archivo
grep -i "html" archivo.txt      # Búsqueda insensible a mayúsculas/minúsculas
grep -n "import" *.js           # Muestra número de línea
grep -r "TODO" src/             # Búsqueda recursiva en carpetas
grep -v "comentario" archivo    # Muestra líneas que NO coinciden
grep -c "error" log.txt         # Cuenta líneas que coinciden
```

---

## Introducción a Git desde la Terminal

Ya que tienen Git instalado, es fundamental conocer los comandos básicos de control de versiones. Git se usa exclusivamente desde la terminal en entornos profesionales, así que familiarizarse con sus comandos es esencial para cualquier desarrollador web.

### Configuración inicial

Antes de usar Git por primera vez, debes configurar tu identidad:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
git config --list                    # Verificar configuración
```

### Comandos básicos de Git

```bash
# Inicializar un repositorio
git init

# Ver estado del repositorio
git status

# Agregar archivos al área de preparación
git add archivo.txt
git add .                    # Agregar todos los archivos

# Crear un commit (guardar cambios)
git commit -m "Mensaje descriptivo del cambio"

# Ver historial de commits
git log
git log --oneline           # Historial compacto

# Ver diferencias
git diff                    # Cambios no preparados
git diff --staged           # Cambios preparados para commit

# Crear y cambiar ramas
git branch nombre-rama      # Crear rama
git checkout nombre-rama    # Cambiar a rama
git checkout -b nueva-rama  # Crear y cambiar en un paso

# Conectar con repositorio remoto
git remote add origin https://github.com/usuario/repo.git
git push -u origin main     # Subir cambios
git pull                    # Descargar cambios
```

### Flujo de trabajo típico

```bash
# 1. Crear proyecto y entrar
mkdir mi-proyecto
cd mi-proyecto

# 2. Inicializar Git
git init

# 3. Crear archivos
touch index.html styles.css script.js

# 4. Verificar estado
git status

# 5. Agregar archivos
git add .

# 6. Crear primer commit
git commit -m "Commit inicial: estructura básica del proyecto"

# 7. Ver historial
git log --oneline
```

---

## Casos Prácticos para Desarrolladores Web

### Caso 1: Crear un nuevo proyecto web

```bash
# Crear estructura completa
mkdir -p mi-portfolio/{css,js,images,assets}
cd mi-portfolio
touch index.html css/styles.css js/main.js

# Inicializar Git
git init
git add .
git commit -m "Estructura inicial del portfolio"
```

### Caso 2: Organizar archivos de un proyecto existente

```bash
# Crear carpetas de organización
mkdir src dist

# Mover archivos fuente
mv *.html src/
mv *.css src/
mv *.js src/

# Verificar estructura
ls -R
```

### Caso 3: Buscar y corregir errores en logs

```bash
# Buscar errores en logs del servidor
grep -i "error" server.log

# Ver los últimos errores
tail -f server.log | grep --color "ERROR"

# Contar errores por tipo
grep "ERROR" server.log | wc -l
```

### Caso 4: Backup de proyecto antes de cambios importantes

```bash
# Crear backup con fecha
mkdir ../backup-$(date +%Y%m%d)
cp -r . ../backup-$(date +%Y%m%d)/

# O usando compresión
tar -czf ../backup-$(date +%Y%m%d).tar.gz .
```

---

## Ejercicios Prácticos para Clase

### Ejercicio 1: Navegación básica
1. Abre Git Bash y determina tu ubicación actual con `pwd`
2. Lista el contenido de tu carpeta personal con `ls -la`
3. Navega a tu carpeta de Documentos usando `cd`
4. Crea una carpeta llamada "practica-terminal" y entra en ella
5. Vuelve a tu carpeta personal usando `cd ~`

### Ejercicio 2: Gestión de archivos
1. En tu carpeta de práctica, crea la siguiente estructura:
   ```
   proyecto/
   ├── index.html
   ├── css/
   │   └── styles.css
   ├── js/
   │   └── app.js
   └── images/
   ```
2. Lista la estructura completa con `ls -R`
3. Copia `index.html` a una carpeta llamada `backup`
4. Renombra `styles.css` a `main.css`
5. Elimina la carpeta `backup` con todo su contenido

### Ejercicio 3: Búsqueda y filtros
1. Crea un archivo de texto con varias líneas de contenido
2. Usa `grep` para buscar una palabra específica
3. Usa `head` y `tail` para ver solo partes del archivo
4. Cuenta las líneas del archivo con `wc`

### Ejercicio 4: Git básico
1. Inicializa un repositorio Git en tu proyecto
2. Configura tu nombre y email si no lo has hecho
3. Crea tu primer commit con todos los archivos
4. Consulta el historial con `git log`
5. Haz un cambio en un archivo y crea un nuevo commit

---

## Recursos Adicionales

### Comandos para consultar ayuda
```bash
comando --help             # Ayuda básica del comando
man comando                # Manual completo (presiona q para salir)
```

### Documentación en línea recomendada
- **Git Documentation**: https://git-scm.com/doc
- **Linux Command Library**: https://linuxcommandlibrary.com/
- **explainshell.com**: Explica comandos de forma interactiva

### Consejos finales para principiantes

1. **No temas experimentar**: La mejor forma de aprender es probando. Crea una carpeta de pruebas y experimenta libremente.

2. **Usa Tab constantemente**: El autocompletado no solo ahorra tiempo, también previene errores tipográficos en nombres de archivos.

3. **Verifica antes de eliminar**: Siempre ejecuta `pwd` antes de usar `rm` para confirmar que estás en el directorio correcto.

4. **Lee los mensajes de error**: La terminal suele dar información útil sobre qué salió mal. No los ignores.

5. **Practica el historial**: Usa las flechas y `Ctrl+R` para reutilizar comandos anteriores. Esto acelera enormemente el trabajo.

6. **Empieza con Git desde el principio**: Aunque parezca complejo al inicio, el control de versiones es indispensable en desarrollo web profesional.

---

## Resumen de Comandos Esenciales

| Categoría | Comando | Descripción |
|-----------|---------|-------------|
| Navegación | `pwd` | Muestra directorio actual |
| | `ls` | Lista contenido |
| | `cd` | Cambia de directorio |
| Archivos | `touch` | Crea archivo vacío |
| | `mkdir` | Crea carpeta |
| | `cp` | Copia archivos/carpetas |
| | `mv` | Mueve/renombra |
| | `rm` | Elimina archivos |
| Contenido | `cat` | Muestra contenido |
| | `head` | Muestra inicio del archivo |
| | `tail` | Muestra final del archivo |
| | `less` | Navega por archivo grande |
| Búsqueda | `grep` | Busca patrones en archivos |
| | `find` | Busca archivos por nombre |
| Git | `git init` | Inicializa repositorio |
| | `git status` | Ver estado |
| | `git add` | Agrega cambios |
| | `git commit` | Guarda cambios |
| | `git log` | Ver historial |

---

*Documento creado para uso educativo en clases de desarrollo web*
