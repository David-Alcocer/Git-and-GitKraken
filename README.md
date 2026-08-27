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
&nbsp;&nbsp;&nbsp;&nbsp;
</a>

</div>

---

<div align="center">
  <img src="images/Negativo blanco.png" width="400" alt="Wewolf" />
  <br><br>
  <em>Curso organizado por Wewolf x Vinculacion FMAT</em>
</div>

---

## <font color="#179287">Herramientas y recursos</font>

| Recurso | Enlace |
|---|---|
| Presentación del curso (Canva) | [Abrir presentación](https://canva.link/wh9mf15zqpmq94i) |
| Descargar Git | [git-scm.com/install](https://git-scm.com/install/) |
| Crear cuenta en GitHub | [github.com](https://github.com) |
| Descargar Github Desktop | [Github Desktop](https://desktop.github.com/download/) |



## <font color="#179287">Antes de empezar — Requisitos</font>

- [ ] Laptop con Git instalado
- [ ] VS Code instalado
- [ ] Cuenta de GitHub creada y correo verificado
- [ ] Cuenta de GitHub Desktop vinculada

---

## <font color="#179287">Guía paso a paso para el alumno</font>

### <font color="#F05032">Bloque 1 — Introducción *(teoría)*</font>

Esta parte es solo de escuchar y observar. El instructor explicará:

- Qué problema resuelve el control de versiones (Qué pasa sin Git?)
- La diferencia entre **Git** (la herramienta local) y **GitHub** (la plataforma en la nube)
- Por qué usamos **GitKraken**: para ver gráficamente lo que Git hace "por dentro"

---

### <font color="#F05032">Bloque 2 — Setup e interfaz *(teoría)*</font>

El instructor hará un tour en vivo. Observa dónde están:

- El **gráfico de commits** (centro de la pantalla)
- El **panel de cambios** (derecha)
- La **barra lateral** (ramas, remotos, stash)

> Si aún no conectaste tu cuenta de GitHub a GitKraken: ve a **Preferences → Integrations → GitHub** y autentícate.

---

### <font color="#F05032">Bloque 3 — Conceptos fundamentales *(teoría)*</font>

Tres ideas clave antes de tocar código:

| Concepto | Qué es |
|---|---|
| **Repositorio (repo)** | Una carpeta que Git vigila y registra su historial |
| **Commit** | Una fotografía del proyecto en un momento dado (tiene autor, mensaje y un código único llamado *hash*) |
| **Grafo de commits** | La línea de tiempo visual de todos los commits; cada punto es un commit |

---

### <font color="#F05032">Bloque 4 — Primer repositorio + commits *(individual)*</font>

**Paso 1 — Crea una carpeta para tu proyecto**
1. En tu computadora, crea una carpeta nueva (ejemplo: `mi-proyecto-git`)

**Paso 2 — Inicia el repositorio en GitKraken**
1. Abre GitKraken → `File` → `Init Repo`
2. Selecciona la carpeta que creaste → `Initialize`
3. Verás el gráfico vacío con un commit inicial

**Paso 3 — Modifica archivos en VS Code**
1. Abre la carpeta en VS Code (`File` → `Open Folder`)
2. Crea un archivo (ejemplo: `index.txt`) y escribe algo
3. Guarda el archivo (`Ctrl+S` / `Cmd+S`)

**Paso 4 — Haz tu primer commit en GitKraken**
1. En GitKraken verás el archivo en el panel derecho como cambio pendiente
2. Haz clic en `Stage All Changes` (o arrastra el archivo al área de staged)
3. Escribe un mensaje descriptivo (ejemplo: `Agrego archivo index.txt`)
4. Haz clic en `Commit changes`

**Ejercicio:** repite los pasos 3 y 4 hasta tener **3 o 4 commits**. Observa cómo el gráfico crece con cada uno.

---

### <font color="#F05032">Bloque 5 — Ramas (branches) *(individual)*</font>

Una **rama** es como una línea de tiempo alterna: puedes hacer cambios sin afectar `main`.

**Paso 1 — Crea una rama nueva**
1. En GitKraken, haz clic derecho sobre el último commit → `Create branch here`
2. Ponle un nombre (ejemplo: `feature/mi-cambio`) → `Enter`
3. Verás que ahora estás en la nueva rama (el ícono de rama activa se mueve)

**Paso 2 — Haz cambios en la rama nueva**
1. Edita o crea un archivo en VS Code
2. Guarda, haz stage y commit en GitKraken (igual que antes)

**Paso 3 — Fusiona (merge) la rama a main**
1. Haz doble clic en `main` en la barra lateral para regresar a esa rama
2. Haz clic derecho sobre tu rama (`feature/mi-cambio`) → `Merge into current branch`
3. Observa cómo el gráfico une las dos líneas en un solo punto

---

### ☕ Descanso — 10 minutos

---

### <font color="#F05032">Bloque 6 — Push y Pull *(individual)*</font>

Ahora subiremos el repositorio local a GitHub.

**Paso 1 — Publica tu repositorio**
1. En GitKraken, haz clic en `Push` (botón superior)
2. Si es la primera vez, te pedirá crear un repositorio remoto en GitHub → acepta
3. Una vez publicado, verás `origin/main` en el gráfico

**Paso 2 — Simula un cambio remoto (Pull)**
1. Ve a tu repositorio en [github.com](https://github.com) y edita un archivo directamente desde el navegador
2. Guarda el cambio haciendo commit desde GitHub
3. En GitKraken haz clic en `Pull` para traer ese cambio a tu computadora
4. Verás el nuevo commit aparecer en el gráfico

---

### <font color="#F05032">Bloque 7 — Fork + Pull Request *(equipos)*</font>

**Fork:** copiar un repositorio ajeno a tu cuenta para poder modificarlo.

**Paso 1 — Haz fork del repo del instructor**
1. Ve al repositorio del instructor en GitHub
2. Haz clic en el botón `Fork` (esquina superior derecha)
3. Clona tu fork desde GitKraken: `File` → `Clone` → pega la URL de tu fork

**Paso 2 — Haz un cambio y manda un Pull Request**
1. Crea una rama nueva en GitKraken (ejemplo: `feature/mi-aportacion`)
2. Edita un archivo en VS Code, haz commit y push
3. Ve a GitHub → verás un banner `Compare & pull request` → haz clic
4. Describe el cambio y haz clic en `Create pull request`

**Paso 3 — Revisa el PR de otro equipo**
1. Ve a la pestaña `Pull requests` del repo del instructor
2. Abre el PR de otro equipo, revísalo y deja un comentario

---

### <font color="#F05032">Bloque 8 — Resolviendo conflictos *(equipos)*</font>

Un **conflicto** ocurre cuando dos personas modifican la misma línea del mismo archivo en ramas distintas.

**Paso 1 — Provoca un conflicto (en equipo)**
1. Los dos integrantes parten del mismo commit en `main`
2. Cada uno crea su propia rama y modifica **la misma línea** del mismo archivo
3. El primero hace merge a `main` sin problema
4. El segundo intenta hacer merge → GitKraken le avisa del conflicto

**Paso 2 — Resuelve el conflicto con GitKraken**
1. GitKraken mostrará el archivo en conflicto con un ícono de advertencia
2. Haz clic en el archivo → `Open in merge tool`
3. Verás tres columnas: versión A (tuya), resultado final (centro), versión B (del compañero)
4. Elige qué líneas conservar haciendo clic en las flechas
5. Guarda y haz clic en `Mark as resolved` → luego commit

---

### <font color="#F05032">Bloque 9 — Mini proyecto integrador *(equipos)*</font>

**Reto final en equipos:**

1. Clona el repositorio del instructor desde GitKraken
2. Crea una rama con el nombre de tu equipo (ejemplo: `equipo-dinamita`)
3. Abre el archivo `box-answers/equipo-dinamita.md` en VS Code
4. Completa las siguientes preguntas **en equipo**:
   - ¿Qué es la ingeniería de software?
   - ¿Qué son las soft skills?
   - ¿Cómo puedes implementar la IA en tu carrera sin perder el protagonismo?
5. Agrega tu foto de perfil a la carpeta `images/` con el formato `nombre-apellido.png` y regístrala en la tabla de integrantes del archivo
6. Guarda los cambios, haz commit y push de tu rama
7. Manda un Pull Request al repositorio del instructor
8. Revisa y aprueba el PR de otro equipo

---

## <font color="#179287">Recursos para seguir practicando</font>

- [GitHub Learning Lab](https://github.com/apps/github-learning-lab) — tutoriales interactivos directamente en GitHub
- [Oh My Git!](https://ohmygit.org/) — juego visual para aprender Git
- [Pro Git Book](https://git-scm.com/book/es/v2) — libro oficial de Git en español (gratuito)
