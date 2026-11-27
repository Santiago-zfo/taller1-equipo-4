# Estándar de codificación Equipo 4

Lenguaje(s) del proyecto formativo:

## 1. Nombrado
(pendiente)

## 2. Formato
(pendiente)

## 3. Comentarios y documentación
(pendiente)

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