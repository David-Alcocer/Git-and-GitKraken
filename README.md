<div align="center">

# Curso Básico: Git para Principiantes

Bienvenido al curso. Aquí encontrarás todo lo que necesitas para seguir la sesión y repasar cada paso por tu cuenta.

<br>

<a href="https://git-scm.com/install/" title="Descargar Git">
  <img src="images/git_plain_wordmark_logo_icon_146508.png" width="80" alt="Git" />
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com" title="GitHub">
  <img src="images/25231.png" width="80" alt="GitHub" />
</a>

</div>

---

<div align="center">
  <img src="images/logo-universidad_-_copia-640w.png" width="100" alt="UADY" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="images/Negativo blanco.png" width="320" alt="Wewolf" />
  <br><br>
  <em>Curso organizado por la Facultad de Matemáticas de la UADY · Vinculación FMAT x Wewolf</em>
</div>

---

## <font color="#179287">Herramientas y recursos</font>

| Recurso | Enlace |
|---|---|
| Presentación del curso (Canva) | [Abrir presentación](https://canva.link/wh9mf15zqpmq94i) |
| Descargar Git | [git-scm.com/install](https://git-scm.com/install/) |
| Crear cuenta en GitHub | [github.com](https://github.com) |
| Descargar GitHub Desktop | [desktop.github.com](https://desktop.github.com/download/) |
| Descargar VS Code | [code.visualstudio.com](https://code.visualstudio.com/) |
| Extensión GitLens | Buscar `GitLens` en VS Code → Extensions (`Ctrl+Shift+X`) |
| Extensión Git Graph | Buscar `Git Graph` en VS Code → Extensions (`Ctrl+Shift+X`) |

---

## <font color="#179287">Antes de empezar — Requisitos</font>

- [ ] Laptop con Git instalado
- [ ] VS Code instalado
- [ ] Cuenta de GitHub creada y correo verificado
- [ ] GitHub Desktop instalado y cuenta vinculada
- [ ] Extensiones de VS Code instaladas: **GitLens** y **Git Graph**

---

## <font color="#179287">Guía paso a paso para el alumno</font>

### <font color="#F05032">Bloque 1 — Introducción *(teoría)*</font>

Esta parte es solo de escuchar y observar. El instructor explicará:

- Qué problema resuelve el control de versiones (¿Qué pasa sin Git?)
- La diferencia entre **Git** (la herramienta local) y **GitHub** (la plataforma en la nube)
- Por qué usamos **GitHub Desktop**: para ver gráficamente lo que Git hace "por dentro"

---

### 📝 Actividad Markdown #1 — Tu primer archivo

> Antes de tocar Git, practica Markdown. Abre VS Code, crea un archivo llamado `mi-perfil.md` en tu escritorio y escribe lo siguiente:

```markdown
# Mi nombre aquí

## Sobre mí
- Carrera:
- Semestre:
- Una cosa que espero aprender hoy:

## Mi frase favorita
> Escribe aquí una frase que te guste.
```

**Elementos que practicaste:** `#` encabezados, `-` listas, `>` citas en bloque.

> Guarda el archivo. Lo usarás durante todo el curso.

---

### <font color="#F05032">Bloque 2 — Setup e interfaz *(teoría)*</font>

El instructor hará un tour en vivo de GitHub Desktop. Observa dónde están:

| Zona | Qué hace |
|---|---|
| **Current Repository** (arriba izquierda) | Muestra el repo activo; desde aquí cambias entre proyectos |
| **Current Branch** (arriba centro) | Indica la rama donde estás trabajando |
| **Changes** (panel izquierdo) | Lista los archivos modificados listos para hacer commit |
| **History** (pestaña izquierda) | Muestra el historial de commits del proyecto |
| **Publish / Push origin** (arriba derecha) | Sube tus cambios a GitHub |

> Si aún no conectaste tu cuenta: ve a **File → Options → Accounts** y haz clic en **Sign In** con GitHub.

---

### 📝 Actividad Markdown #2 — Negritas, cursiva y código

> Abre `mi-perfil.md` en VS Code y agrega una nueva sección al final:

```markdown
## Herramientas del curso

| Herramienta | Para qué sirve |
|---|---|
| **Git** | Control de versiones local |
| **GitHub** | Plataforma en la nube |
| **GitHub Desktop** | Interfaz gráfica para Git |
| **VS Code** | Editor de archivos |

Hoy aprenderé a usar `git commit` por primera vez.
```

**Elementos que practicaste:** `**negritas**`, tablas con `|`, código en línea con `` ` ``.

---

### <font color="#F05032">Bloque 3 — Conceptos fundamentales *(teoría)*</font>

Tres ideas clave antes de empezar:

| Concepto | Qué es |
|---|---|
| **Repositorio (repo)** | Una carpeta que Git vigila y registra su historial |
| **Commit** | Una fotografía del proyecto en un momento dado (tiene autor, mensaje y un código único llamado *hash*) |
| **Rama (branch)** | Una línea de tiempo alterna donde puedes hacer cambios sin afectar `main` |

---

### 📝 Actividad Markdown #3 — Listas de tareas

> Agrega al final de `mi-perfil.md` esta sección y ve marcando cada casilla conforme avances en el curso:

```markdown
## Mi progreso en el curso

- [ ] Cree mi primer repositorio
- [ ] Hice mi primer commit
- [ ] Cree una rama nueva
- [ ] Hice un merge
- [ ] Subí mi repo a GitHub
- [ ] Mandé un Pull Request
- [ ] Resolví un conflicto
```

**Elemento que practicaste:** listas de tareas con `- [ ]` y `- [x]`.

---

### <font color="#F05032">Bloque 4 — Primer repositorio + commits *(individual)*</font>

**Paso 1 — Crea una carpeta para tu proyecto**
1. En tu computadora, crea una carpeta nueva (ejemplo: `mi-proyecto-git`)
2. Mueve tu archivo `mi-perfil.md` dentro de esa carpeta

**Paso 2 — Inicia el repositorio en GitHub Desktop**
1. Abre GitHub Desktop → `File` → `New Repository`
2. En **Local Path**, selecciona la carpeta que creaste → clic en `Create Repository`
3. GitHub Desktop mostrará el repositorio listo en el panel principal

**Paso 3 — Haz tu primer commit**
1. En el panel **Changes** verás `mi-perfil.md` como archivo nuevo
2. Activa la casilla junto al archivo (debe quedar con ✓)
3. En el campo **Summary** (abajo a la izquierda) escribe: `Agrego mi perfil`
4. Haz clic en **Commit to main**
5. Verás el commit en la pestaña **History**

**Ejercicio:** agrega contenido nuevo a `mi-perfil.md` y repite los pasos 1–4 hasta tener **3 o 4 commits**. Observa cómo el historial crece con cada uno.

> **Así se ve tu historial hasta ahora:**

```mermaid
gitGraph
   commit id: "Agrego mi perfil"
   commit id: "Agrego sección sobre mí"
   commit id: "Agrego frase favorita"
   commit id: "Actualizo mi progreso"
```

---

### <font color="#F05032">Bloque 5 — Ramas (branches) *(individual)*</font>

Una **rama** es como una línea de tiempo alterna: puedes hacer cambios sin afectar `main`.

**Paso 1 — Crea una rama nueva**
1. En GitHub Desktop, haz clic en **Current Branch** → **New Branch**
2. Escribe el nombre (ejemplo: `feature/nueva-seccion`) → `Create Branch`
3. Verás que la rama activa cambia en la barra superior

> **Así se ve la bifurcación en el historial:**

```mermaid
gitGraph
   commit id: "commit en main"
   commit id: "otro commit en main"
   branch feature/nueva-seccion
   checkout feature/nueva-seccion
   commit id: "cambio 1 en la rama"
   commit id: "cambio 2 en la rama"
   checkout main
```

**Paso 2 — Haz cambios en la rama nueva**
1. Abre `mi-perfil.md` en VS Code
2. Agrega una nueva sección (ver actividad abajo)
3. Guarda, activa la casilla en **Changes**, escribe un mensaje y haz commit

**Paso 3 — Fusiona (merge) la rama a main**
1. En GitHub Desktop, ve a **Current Branch** → selecciona `main`
2. Desde el menú: `Branch` → `Merge into Current Branch`
3. Selecciona tu rama (`feature/nueva-seccion`) → `Create a merge commit`
4. En **History** verás cómo se unieron los dos caminos

> **Así se ve el merge:**

```mermaid
gitGraph
   commit id: "commit en main"
   branch feature/nueva-seccion
   checkout feature/nueva-seccion
   commit id: "cambio 1"
   commit id: "cambio 2"
   checkout main
   merge feature/nueva-seccion id: "Merge"
```

---

### 📝 Actividad Markdown #4 — Links e imágenes

> Mientras estás en tu rama nueva, agrega esta sección a `mi-perfil.md`:

```markdown
## Recursos que quiero explorar

- [GitHub Learning Lab](https://github.com/apps/github-learning-lab) — tutoriales interactivos
- [Oh My Git!](https://ohmygit.org/) — juego para aprender Git
- [Pro Git Book en español](https://git-scm.com/book/es/v2) — libro oficial gratuito

## Mis dudas hasta ahora

1. 
2. 
3. 
```

**Elementos que practicaste:** `[texto](url)` links y listas numeradas `1.`.

> Haz commit de este cambio en tu rama antes de fusionar.

---

### ☕ Descanso — 10 minutos

---

### <font color="#F05032">Bloque 6 — Push *(individual)*</font>

Ahora subiremos el repositorio local a GitHub.

**Paso 1 — Publica tu repositorio**
1. En GitHub Desktop, haz clic en **Publish repository** (botón superior derecho)
2. Elige si quieres que sea público o privado → `Publish Repository`
3. Una vez publicado, el botón cambia a **Push origin**

**Paso 2 — Verifica en GitHub**
1. Ve a [github.com](https://github.com) y abre tu repositorio
2. Confirma que `mi-perfil.md` aparece con todo tu contenido
3. Regresa a GitHub Desktop: cada vez que hagas cambios nuevos, haz clic en **Push origin** para sincronizar

> **Push, Fetch y Pull — la calle en dos direcciones:**

| Acción | Qué hace | Cuándo usarla |
|---|---|---|
| **Push** | Envía tus commits locales a GitHub | Cuando quieres subir tus cambios |
| **Fetch** | Revisa si hay cambios en GitHub, sin traerlos aún | Para asomarte sin modificar nada local |
| **Pull** | Trae los cambios de GitHub a tu computadora | Cuando quieres recibir lo que otros subieron |

> Fetch = "mirar el buzón". Pull = "meter las cartas a tu escritorio".

---

### 📝 Actividad Markdown #5 — Separadores y énfasis

> En VS Code, agrega al final de `mi-perfil.md` una sección de cierre antes de hacer push:

```markdown
---

## Reflexión del bloque

Lo que más me costó entender fue:

Lo que me quedó más claro fue:

---

*Archivo creado y editado con VS Code + GitHub Desktop*
```

**Elementos que practicaste:** `---` separador horizontal, texto en cursiva con `*`.

---

### <font color="#F05032">Bloque 7 — Viajando en el historial *(individual)*</font>

Git guarda cada commit como un punto en el tiempo. Puedes visitar cualquiera de ellos sin romper el presente.

**Ver el historial en GitHub Desktop**
1. Ve a la pestaña **History**
2. Haz clic en cualquier commit para ver exactamente qué cambió (verde = agregado, rojo = quitado)

**Ver quién escribió cada línea con GitLens**
1. Abre `mi-perfil.md` en VS Code
2. Pasa el cursor sobre cualquier línea — aparecerá quién la escribió y cuándo
3. Esto se llama **blame** y es muy útil para entender por qué está ese texto ahí

**Ver el árbol de ramas con Git Graph**
1. En VS Code, abre la paleta de comandos (`Ctrl+Shift+P` / `Cmd+Shift+P`)
2. Escribe `Git Graph: View Git Graph` y selecciónalo
3. Verás un mapa visual de todos tus commits y ramas

> **Mirar el historial no cambia nada.** Es como pausar un video en un minuto exacto: puedes ver ese fotograma y después seguir desde donde estás.

```mermaid
gitGraph
   commit id: "C1 — puedes verlo"
   commit id: "C2 — puedes verlo"
   commit id: "C3 — puedes verlo"
   commit id: "C4 — aquí estás ahora (HEAD)"
```

---

### <font color="#F05032">Bloque 8 — Si algo sale mal *(individual)*</font>

Antes de trabajar en equipo, conoce los botones de "deshacer". Git tiene uno para cada situación:

| Situación | Qué usar | Dónde está |
|---|---|---|
| Guardaste el archivo pero **no hiciste commit** | **Discard changes** | Clic derecho sobre el archivo en *Changes* → GitHub Desktop |
| Hiciste commit pero **no hiciste push** | **Undo commit** | Botón "Undo" que aparece justo después de comitear en GitHub Desktop |
| Estás en medio de un merge conflictivo y quieres cancelar todo | **Abort merge** | Botón visible en GitHub Desktop durante el conflicto |
| Ya hiciste push y el commit está en GitHub | **Revert commit** | Clic derecho sobre el commit en *History* → Revert |

> **Revert no borra la historia** — crea un commit nuevo que deshace el anterior. Es la opción más segura cuando ya compartiste tus cambios con otros.

---

### <font color="#F05032">Bloque 9 — Fork + colaboración en equipo + Pull Request *(equipos)*</font>

**Fork:** copiar un repositorio ajeno a tu cuenta para poder modificarlo junto con tu equipo.

---

#### 👑 Solo el líder del equipo

**Paso 1 — Haz fork del repo del instructor**
1. Ve al repositorio del instructor en GitHub
2. Haz clic en `Fork` (esquina superior derecha) → `Create fork`
3. Ahora tienes una copia del repo en tu cuenta: `tu-usuario/GitBasic`

**Paso 2 — Agrega a tus compañeros como colaboradores**
1. En tu fork en GitHub, ve a **Settings** → **Collaborators** → **Add people**
2. Busca el usuario de GitHub de cada compañero y agrégalos
3. Ellos recibirán un correo de invitación — avísales que lo acepten antes de continuar

**Paso 3 — Clona tu fork en GitHub Desktop**
1. Abre GitHub Desktop → `File` → `Clone Repository`
2. Busca tu fork (`tu-usuario/GitBasic`) → selecciona carpeta destino → `Clone`

---

#### 👥 El resto del equipo (después de aceptar la invitación)

**Paso 4 — Clona el fork del líder**
1. Abre GitHub Desktop → `File` → `Clone Repository` → pestaña **URL**
2. Pega la URL del fork del líder (el líder se las comparte)
3. Selecciona carpeta destino → `Clone`

---

#### 🤝 Todo el equipo

**Paso 5 — Practiquen Push y Pull en equipo**
1. El líder crea una rama: **Current Branch** → **New Branch** → `equipo-[nombre]`
2. El líder abre VS Code, crea el archivo `answers-box/equipo-[nombre].md` y escribe algo
3. El líder hace commit y **Push origin** desde GitHub Desktop
4. El resto del equipo hace clic en **Fetch origin** → **Pull origin** en GitHub Desktop
5. Verán el archivo del líder aparecer en su VS Code — eso es un **Pull real**

**Paso 6 — Manda el Pull Request al instructor**
1. En GitHub Desktop, haz clic en **Create Pull Request** — se abrirá el navegador
2. Verifica que el PR va desde tu rama en el fork → hacia el repo del instructor
3. Escribe un título descriptivo → `Create pull request`

> El instructor tiene `main` protegido con revisión de **codeowner** obligatoria. Solo él puede aprobar y hacer merge — ustedes no verán ese botón disponible.

**Paso 7 — Deja feedback en el PR de otro equipo**
1. Ve a la pestaña `Pull requests` del repo del instructor en GitHub
2. Abre el PR de otro equipo, léelo y deja un comentario constructivo

---

### <font color="#F05032">Bloque 10 — Resolviendo conflictos *(equipos)*</font>

Un **conflicto** ocurre cuando dos personas modifican la misma línea del mismo archivo en ramas distintas.

**Paso 1 — Provoca un conflicto (en equipo)**
1. Los dos integrantes parten del mismo commit en la rama `equipo-[nombre]` del fork
2. Cada uno crea su propia rama desde ahí y modifica **la misma línea** del archivo `answers-box/equipo-[nombre].md`
3. El primero hace commit, push y merge a la rama del equipo — sin problema
4. El segundo hace commit y push — GitHub Desktop le avisa del conflicto al intentar hacer merge

> **Por qué ocurre el conflicto:**

```mermaid
gitGraph
   commit id: "Base compartida"
   branch rama-persona-B
   checkout main
   commit id: "Persona A edita línea X"
   checkout rama-persona-B
   commit id: "Persona B edita la misma línea X"
   checkout main
   merge rama-persona-B id: "Conflicto aquí"
```

**Paso 2 — Resuelve el conflicto**
1. GitHub Desktop mostrará un mensaje de conflicto con un botón **Open in Visual Studio Code**
2. VS Code abrirá el archivo con marcas como estas:

```
<<<<<<< HEAD
Esta es mi versión del texto
=======
Esta es la versión de mi compañero
>>>>>>> feature/rama-compañero
```

3. Borra las marcas (`<<<<<<<`, `=======`, `>>>>>>>`) y deja solo el texto final que quieran conservar
4. Guarda el archivo en VS Code
5. Regresa a GitHub Desktop → haz clic en **Continue Merge** → luego commit

> **Si el conflicto da pánico**, recuerda el Bloque 8: puedes hacer **Abort merge** y volver al estado anterior sin perder nada.

---

### <font color="#F05032">Bloque 11 — Mini proyecto integrador *(equipos)*</font>

**Reto final en equipos:**

> Continúan en el mismo fork del Bloque 9 — no necesitan clonar nada nuevo. El líder ya tiene el fork y todos los compañeros ya lo tienen clonado.

1. En GitHub Desktop, asegúrate de estar en la rama `equipo-[nombre]` del fork
2. En VS Code, completa (o termina de completar) el archivo `answers-box/equipo-[nombre].md`
3. Divídanse las secciones: cada integrante escribe una parte, hace commit y push — los demás hacen **Fetch + Pull** para recibir los cambios
4. Completen todas las secciones **en equipo**:

```markdown
# Equipo [Nombre]

## Integrantes

| Nombre | Carrera | Semestre |
|---|---|---|
| | | |
| | | |

## Preguntas del reto

### ¿Qué es la ingeniería de software?


### ¿Qué son las soft skills?


### ¿Cómo puedes usar la IA en tu carrera sin perder el protagonismo?


## Lo más valioso que aprendimos hoy

> 

## Una pregunta que nos quedó pendiente

> 
```

5. Haz stage y commit en GitHub Desktop con el mensaje: `Reto final: equipo-[nombre]`
6. Haz clic en **Push origin**
7. En GitHub Desktop, haz clic en **Create Pull Request** — se abrirá el navegador
8. Verifica que el PR apunta al repo del instructor → `Create pull request`
9. Deja un comentario en el PR de otro equipo en GitHub (lectura y feedback solamente)

> El instructor revisará y mergeará los PRs. Una vez aceptados, pueden entrar al repositorio del instructor en GitHub para ver los archivos de **todos los equipos** juntos en `answers-box/` — esa es la visualización final del trabajo colectivo.

---

## <font color="#179287">Referencia rápida de Markdown</font>

| Sintaxis | Resultado |
|---|---|
| `# Título` | Encabezado grande |
| `## Subtítulo` | Encabezado mediano |
| `**texto**` | **negrita** |
| `*texto*` | *cursiva* |
| `- elemento` | lista con viñeta |
| `1. elemento` | lista numerada |
| `- [ ] tarea` | casilla sin marcar |
| `- [x] tarea` | casilla marcada |
| `[texto](url)` | link |
| `> texto` | cita en bloque |
| `` `código` `` | código en línea |
| `---` | línea divisoria |

---

## <font color="#179287">Recursos para seguir practicando</font>

- [GitHub Learning Lab](https://github.com/apps/github-learning-lab) — tutoriales interactivos directamente en GitHub
- [Oh My Git!](https://ohmygit.org/) — juego visual para aprender Git
- [Pro Git Book](https://git-scm.com/book/es/v2) — libro oficial de Git en español (gratuito)
- [Markdown Guide](https://www.markdownguide.org/) — referencia completa de Markdown
