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
(pendiente)

## 3. Comentarios y documentación
(pendiente)

## 4. Estructura de carpetas
(pendiente)

## 5. Git: ramas, commits y pull requests
(pendiente)