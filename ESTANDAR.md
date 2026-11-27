# Estándar de codificación Equipo 4

Lenguaje(s) del proyecto formativo:

## 1. Nombrado
(pendiente)

## 2. Formato
(pendiente)

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
(pendiente)