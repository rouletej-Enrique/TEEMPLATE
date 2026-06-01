# Project Creation Boilerplate

Usa este boilerplate cada vez que quieras crear un proyecto nuevo.

## 1. Clonar el proyecto

Primero, definí el nombre del proyecto:

```bash
PROJECT_NAME="NOMBRE_DE_TU_PROYECTO"
```

Después cloná este repositorio en tu escritorio:

```bash
git clone https://github.com/rouletej-Enrique/TEEMPLATE ~/Desktop/${PROJECT_NAME}
```

Ejemplo:

```bash
PROJECT_NAME="XDS"
git clone https://github.com/rouletej-Enrique/TEEMPLATE ~/Desktop/${PROJECT_NAME}
```

Eso va a clonar este boilerplate en:

```bash
~/Desktop/XDS
```

> Si el nombre del repositorio `TEEMPLATE` es un typo o lo modificas despues, corregilo antes de usar el comando.

## 2. Preparar el proyecto

Antes de pedirle al agente que empiece a trabajar, agregá el contexto necesario.

### Opción A: Tenés un template descargado

Colocá el template, assets, imágenes, referencias o recursos dentro de:

```text
.samples/assets/
```

### Opción B: Tenés una idea y empezás desde cero

Abrí Claude Web, no Claude Code desde la terminal, y pedile que genere un PRD.

Usá este prompt como base:

```text
I want you to create a PRD document for [TOPIC]. The project will be called [NAME].

The project should do the following:

[STEPS]

Make the PRD clear, structured, and ready for an implementation agent to use.
```

Reemplazá `[TOPIC]`, `[NAME]` y `[STEPS]` con los datos reales del proyecto.

Cuando tengas el PRD u otros documentos de contexto, colocalos en:

```text
.samples/docs/
```

## 3. Iniciar el trabajo

Abrí el proyecto desde la terminal, usando VS Code, Cursor, Antigravity o el editor que prefieras.

Desde la raíz del proyecto, pedile al agente:

```text
Start working on the project.
```

También podés hacerlo en español:

```text
Empezá a trabajar en el proyecto.
```

El agente debe detectar `.agents/BOOT.md`, leer el contexto disponible en `.samples/`, preparar el proyecto y eliminar el archivo de bootstrap cuando termine.

> [!IMPORTANT]
> Si queres que claude haga todo sin estar preguntandote cada 2 segundos de aprovar cualquier comando, podes correrlo con `claude --allow-dangerously-skip-permissions`
