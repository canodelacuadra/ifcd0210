
# Guía de Uso de IA para Desarrollo Web: Aprende a Preguntar, no a Copiar

## 1. Introducción: El nuevo compañero de equipo

La Inteligencia Artificial (IA) ha llegado para quedarse en el mundo del desarrollo web. Herramientas como ChatGPT, Claude o GitHub Copilot son increíblemente potentes, pero hay una regla de oro que debes recordar siempre:

> **"Si tú no entiendes el código que la IA genera, ese código te pertenece a la IA, no a ti."**

El objetivo de esta guía no es que la IA haga tu trabajo, sino que te ayude a **aprender más rápido**, a **entender mejor** y a **resolver dudas** cuando te quedes atascado. Queremos que seas un desarrollador que *piensa*, no un robot que *copia*.

## 2. La Filosofía: Prompting con Criterio

"Prompting" es el arte de escribir instrucciones a la IA. Si escribes instrucciones vagas, obtendrás respuestas vagas o incorrectas.

Cuando uses la IA, evita decir simplemente: *"Hazme una página web"*. En su lugar, úsala para:

1.  **Entender código:** Que te explique línea a línea lo que hace un script.
2.  **Orientarte:** Pedir pistas cuando te atascas, sin pedir la solución directa.
3.  **Debuguear:** Entender por qué falla tu código.

## 3. Los 3 Roles Principales de la IA

### Rol A: El Explicador (Para cuando ves código y no lo entiendes)
A veces encontramos código en internet o en ejemplos que parece magia negra. La IA es perfecta para traducirlo a lenguaje humano.

*   **Mal prompt:** "¿Qué es esto?" (pegar código).
*   **Buen prompt:**
    > "Soy estudiante de desarrollo web. Por favor, explica el siguiente código **línea por línea**. Usa analogías sencillas para explicar conceptos complejos. Al final, dame un resumen de qué problema resuelve este código."

### Rol B: El Orientador (Para cuando no sabes cómo seguir)
Estás programando y te bloqueas. No sabes qué función usar. Pide una guía, no la solución.

*   **Mal prompt:** "Escribe el código para validar este formulario".
*   **Buen prompt:**
    > "Estoy intentando validar un formulario en JavaScript para que el email sea correcto. He intentado usar `indexOf` pero no funciona bien. **No me des la solución en código todavía.** Solo dime qué método o expresión regular debería investigar para resolver esto."

### Rol C: El Mentor de Errores (Para cuando algo falla)
La consola escupe errores rojos que dan miedo. La IA te ayuda a traducirlos.

*   **Mal prompt:** "Arregla este error".
*   **Buen prompt:**
    > "Estoy recibiendo este error en mi consola: `[TypeError: undefined is not a function]`. Te pego mi código abajo. ¿Puedes explicarme **por qué** se produce este error conceptualmente? Dime qué línea está causando el problema y por qué, pero déjame intentar arreglarlo a mí mismo."

## 4. La Fórmula Maestra del Prompt

Para obtener las mejores respuestas, intenta estructurar tus preguntas con estos cuatro ingredientes:

1.  **Contexto:** ¿Quién eres y qué estás haciendo? (Ej: "Estoy aprendiendo HTML/CSS y haciendo mi primer portfolio").
2.  **El Problema:** ¿Qué pasa? (Ej: "El menú hamburguesa no se abre al hacer clic").
3.  **Lo que has intentado:** Muestra que has trabajado. (Ej: "He revisado la clase en el evento `onclick` pero parece estar bien").
4.  **La Petición:** ¿Qué quieres exactamente? (Ej: "¿Qué conceptos debo repasar para entender por qué el evento no se dispara?").

## 5. Advertencia: Las Alucinaciones

La IA no es perfecta. A veces inventa librerías que no existen o da soluciones que funcionan hoy pero son "malas prácticas" para el futuro.

**Regla de Oro:** Si la IA te da un código que no has visto en clase o no entiendes, pregúntale: *"¿Por qué usas esta librería? ¿Es estándar o hay una forma nativa de hacerlo?"*. Nunca confíes ciegamente; **verifica siempre** en la documentación oficial (MDN, W3Schools).

---

## 6. Ejercicios Prácticos

A continuación, realiza los siguientes ejercicios usando la herramienta de IA que tengas disponible (ChatGPT, Claude, Gemini, etc.).

### Ejercicio 1: Reverse Engineering (Ingeniería Inversa)
**Objetivo:** Aprender a leer código que no has escrito tú.

1.  Copia el siguiente fragmento de código (que quizás no hayas visto aún o te parezca confuso):
    ```javascript
    const usuarios = ['Ana', 'Luis', 'Carlos'];
    const saludos = usuarios.map(usuario => `Hola, ${usuario}`);
    console.log(saludos);
    ```
2.  **Tarea:** Abre la IA y escribe un prompt usando el **Rol A (El Explicador)**.
3.  **Entregable:** Copia la explicación que te dio la IA y escribe con tus propias palabras si entendiste qué hace la función `.map()`.

### Ejercicio 2: El Detective de Bugs
**Objetivo:** Aprender a diagnosticar errores sin que te den la solución.

1.  Imagina que escribes este CSS para centrar un div, pero no funciona:
    ```css
    .contenedor {
      width: 200px;
      height: 200px;
      background-color: red;
      margin: 0 auto;
    }
    body {
      width: 100%;
    }
    ```
    *Nota: El problema es que el `body` no tiene altura o el contenedor padre no está definido, pero simularemos que no sabemos por qué no se ve bien.*
2.  **Tarea:** Escribe un prompt a la IA explicando que quieres centrar el div verticalmente y que con `margin: 0 auto` no lo logras. Pídele que te oriente sobre qué conceptos de CSS debes buscar para centrar elementos verticalmente.
3.  **Entregable:** ¿Qué conceptos te sugirió la IA? (Ejemplo: Flexbox, Grid, Position). Intenta aplicar la solución basándote en la pista.

### Ejercicio 3: Comparativa de Prompts
**Objetivo:** Entender la diferencia entre un prompt "vago" y un prompt "con criterio".

1.  Tienes la siguiente tarea: "Quiero hacer una galería de imágenes que se muestren en una cuadrícula de 3 columnas".
2.  **Parte A:** Escribe un prompt perezoso (ej: "Dame código para galería de fotos").
3.  **Parte B:** Escribe un prompt detallado usando la **Fórmula Maestra** (Contexto, Problema, Intento, Petición). Pide que te explique qué propiedades de CSS son vitales para lograr la cuadrícula.
4.  **Entregable:** Reflexiona brevemente: ¿Cuál de las dos respuestas te sirvió más para aprender? ¿Por qué?

---

### Conclusión 

Al finalizar estos ejercicios, recuerda: **La IA es tu copiloto, pero tú llevas el volante.** Si sabes preguntar, aprenderás el doble rápido; si solo copias, aprenderás la mitad.