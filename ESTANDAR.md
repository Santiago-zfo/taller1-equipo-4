# Estándar de codificación Equipo 4

Lenguaje(s) del proyecto formativo:

## 1. Nombrado

En el proyecto Velora utilizaremos nombres claros, descriptivos y
consistentes para que cualquier integrante del equipo pueda comprender
el código y la estructura de la base de datos.

### 1.1. Idioma

Los nombres de variables, funciones, clases, constantes, archivos,
carpetas y elementos de la base de datos se escribirán en **inglés**.
La documentación y los comentarios podrán escribirse en español.

No se deben mezclar idiomas en un mismo nombre:

- Correcto: `userProfile`
- Incorrecto: `perfilUser`

Los nombres no deben contener espacios, tildes, la letra ñ ni caracteres
especiales. Se usarán únicamente letras, números y los separadores
permitidos por la convención de cada elemento.

### 1.2. Variables

Las variables se escribirán en `camelCase`: la primera palabra comienza
en minúscula y las siguientes comienzan con mayúscula.

Sus nombres deben indicar qué información almacenan:

- `userName`: nombre de usuario.
- `birthDate`: fecha de nacimiento.
- `profilePhoto`: foto del perfil.
- `matchCount`: cantidad de coincidencias.

Se deben evitar nombres poco descriptivos como `x`, `dato` o `variable1`,
salvo en casos muy breves donde su significado sea evidente.

Las variables que contienen valores verdaderos o falsos deben expresar
una condición, preferiblemente con prefijos como `is`, `has` o `can`:

- `isActive`
- `hasProfilePhoto`
- `canSendMessage`

### 1.3. Funciones y métodos

Las funciones y los métodos se escribirán en `camelCase` y comenzarán
preferiblemente con un verbo que describa la acción que realizan.

Ejemplos:

- `createProfile()`: crea un perfil.
- `updateProfile()`: actualiza la información de un perfil.
- `validateEmail()`: valida una dirección de correo.
- `findMatches()`: busca coincidencias.
- `sendMessage()`: envía un mensaje.

El nombre debe describir la tarea principal de la función. Se evitarán
nombres generales como `doStuff()` o `processData()` cuando sea posible
describir con mayor precisión lo que hace.

### 1.4. Clases

Las clases se escribirán en `PascalCase`: cada palabra comienza con
mayúscula, sin espacios ni separadores.

Se utilizarán sustantivos que representen claramente la responsabilidad
o entidad de la clase.

Ejemplos:

- `User`
- `UserProfile`
- `MatchService`
- `MessageController`

En Java, el archivo que contiene una clase pública debe tener exactamente
el mismo nombre de la clase. Por ejemplo, la clase `UserProfile` se
guardará en `UserProfile.java`.

### 1.5. Constantes

Las constantes que no cambian durante la ejecución se escribirán en
`UPPER_SNAKE_CASE`: todas las letras en mayúscula y las palabras separadas
por guiones bajos.

Ejemplos:

- `MAX_PROFILE_PHOTOS`
- `MIN_PASSWORD_LENGTH`
- `DEFAULT_PAGE_SIZE`

Su nombre debe describir el valor o límite que representan.

### 1.6. Archivos y carpetas

Los nombres de los archivos y carpetas deben indicar su contenido o
responsabilidad.

Para archivos generales se utilizarán nombres en minúscula y con guiones
cuando tengan varias palabras:

- `profile-card.css`
- `user-profile.html`
- `database-config.json`

Las carpetas seguirán la misma regla:

- `user-profiles`
- `profile-photos`
- `database-config`

Se respetarán los nombres exigidos por el lenguaje o el framework.
Por ejemplo, en Java se usará `UserProfile.java` para la clase pública
`UserProfile`.

### 1.7. Tablas y campos de la base de datos

Las tablas y los campos se escribirán en `snake_case`: letras minúsculas
y palabras separadas por guiones bajos.

Las tablas tendrán nombres descriptivos en plural:

- `users`
- `user_profiles`
- `matches`
- `messages`

Los campos tendrán nombres descriptivos que indiquen el dato almacenado:

- `first_name`
- `birth_date`
- `profile_photo`
- `created_at`

La clave primaria de cada tabla se llamará `id`. Las claves foráneas
utilizarán el nombre de la entidad en singular seguido de `_id`:

- `user_id`
- `profile_id`
- `match_id`

### 1.8. Reglas de consistencia

- Un mismo concepto debe conservar el mismo nombre en todo el proyecto.
  Por ejemplo, si se utiliza `user`, no se alternará con `usuario` o
  `person` para referirse a la misma entidad.
- Se evitarán abreviaturas que puedan generar confusión.
- No se usarán nombres demasiado generales si existe una alternativa
  más clara y específica.
- Antes de crear un nombre nuevo, se revisará si ya existe uno para el
  mismo concepto.
- Cuando el lenguaje o framework tenga una convención obligatoria,
  se respetará y se aplicará de forma consistente.

## 2. Formato

Al tratarse de una práctica de simulación para aprender Git y GitHub, definimos reglas sencillas y consistentes para todo el equipo:

* **Indentación:** Usar **2 espacios** (nunca mezclar espacios y tabulaciones en el mismo archivo), alineado con la configuración de `.editorconfig`.
* **Comillas:** Usar **comillas dobles (`"..."`)** en textos y cadenas por defecto, salvo cuando el contexto del lenguaje o archivo requiera comillas simples (`'...'`).
* **Largo máximo de línea:** Mantener las líneas idealmente en un máximo de **80 a 100 caracteres** en código y documentación para facilitar la lectura en diffs y revisiones de Pull Request.
* **Llaves (`{}`):** Abrir la llave en la misma línea de la declaración/condicional (estilo K&R / *same-line*), dejar un espacio antes de `{` y cerrar en una línea nueva.
* **Saltos de línea y espacios finales:** Usar salto de línea LF (`\n`), mantener una línea vacía al final de cada archivo y evitar espacios en blanco al final de las líneas (excepto en archivos `.md` donde se requiera salto de línea explícito).

## 3. Comentarios y documentación

### Cuándo comentar
** **Explicar el *porqué*, no el *qué*:** El código limpio debe ser autoexplicativo mediante buenos nombres de variables y funciones. Solo se comenta la lógica compleja, decisiones técnicas no evidentes, reglas de negocio específicas o soluciones temporales.
* **Evitar comentarios obvios o redundantes:** No comentar acciones triviales (ejemplo incorrecto: `# Suma 1 al contador` sobre `contador += 1`).
* **Marcadores estándar:** Usar etiquetas en mayúsculas cuando quede trabajo pendiente o haya alertas técnicas:
  * `TODO:` funcionalidad o mejora pendiente por implementar.
  * `FIXME:` error conocido que requiere corrección.
* **Idioma:** Todos los comentarios y la documentación se redactan en **español**, con buena ortografía y redacción clara.

### Cómo documentar funciones
* Toda función, método o clase pública debe incluir un bloque de documentación (**Docstring** en Python o **JSDoc** en JavaScript) inmediatamente en su definición.
* **Estructura obligatoria:**
  1. **Descripción breve:** Qué hace la función en una oración clara.
  2. **Parámetros (`Args` / `@param`):** Nombre, tipo de dato y descripción de cada entrada.
  3. **Retorno (`Returns` / `@returns`):** Tipo de dato y significado del valor devuelto.
  4. **Excepciones (`Raises` / `@throws`):** Errores que puede lanzar (si aplica).

### Qué debe tener el README
El archivo `README.md` en la raíz del repositorio es la carta de presentación del proyecto y debe contener las siguientes secciones mínimas:

1. **Título y descripción:** Nombre del proyecto formativo y resumen claro del problema que resuelve.
2. **Tecnologías utilizadas:** Lenguajes, frameworks, bases de datos y herramientas principales con sus versiones.
3. **Requisitos previos e instalación:** Pasos exactos para clonar el repositorio, instalar dependencias y configurar variables de entorno (`.env`).
4. **Instrucciones de ejecución:** Comandos para levantar el proyecto en entorno local y ejecutar pruebas.
5. **Estructura del proyecto:** Breve explicación de las carpetas principales y enlace al estándar de codificación (`ESTANDAR.md`).
6. **Integrantes del equipo:** Nombres completos y roles de cada miembro del equipo.
## 4. Estructura de carpetas
(pendiente)

## 5. Git: ramas, commits y pull requests

### Ramas
- **Rama principal:** `main` (mantiene el código estable y revisado; no se hacen commits directos).
- **Convención de nombres:** `tipo/descripcion-corta` en minúsculas y separada por guiones (`kebab-case`).
  - Ejemplos: `feat/login-usuario`, `fix/error-validacion`, `docs/estandar-git`, `chore/config-editorconfig`.

### Commits
- **Formato:** `tipo: descripción breve en presente` (siguiendo convención similar a Conventional Commits, sin punto final).
- **Tipos comunes:**
  - `feat:` nueva funcionalidad.
  - `fix:` corrección de errores.
  - `docs:` cambios en documentación.
  - `chore:` tareas de configuración, dependencias o mantenimiento.
  - `refactor:` cambios internos de código sin alterar su comportamiento externo.
- **Cierre de issues:** cuando un commit o PR resuelve un issue, se incluye `Closes #N` (donde `N` es el número del issue)[cite: 2].
  - Ejemplo: `docs: agrega sección de git al estándar. Closes #5`[cite: 2].

### Pull Requests (PR)
- Todo cambio de una rama hacia `main` debe pasar por un Pull Request[cite: 2].
- El título del PR debe ser claro y descriptivo (similar al commit principal).
- En la descripción se debe indicar qué se hizo y, si aplica, incluir `Closes #N` para vincular y cerrar el issue al fusionar[cite: 2].
- Antes de fusionar (`merge`), al menos otro integrante revisa los cambios y, si hay conflictos, se resuelven actualizando la rama con los últimos cambios de `main` antes de fusionar[cite: 2, 4].