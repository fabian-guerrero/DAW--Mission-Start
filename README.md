# NextGen Web Solutions — Microservice Starter

Este repositorio contiene la configuración inicial del entorno de desarrollo y la base para un microservicio desarrollado como parte del proceso técnico interno de NextGen Web Solutions.

El objetivo del proyecto es:

- Configurar un entorno de desarrollo profesional
- Detectar problemas de rendimiento en un e-commerce existente
- Crear la base de un microservicio escalable

---

# ⚙️ Configuración del Entorno

Este proyecto utiliza **configuración local de herramientas** para evitar modificar configuraciones globales del sistema o afectar otros proyectos.

Todas las configuraciones se encuentran dentro del repositorio.

---

# 📋 Requisitos Previos

Antes de comenzar asegúrate de tener instalado:

- **Node.js** (versión 18 o superior recomendada)
- **npm**
- **Visual Studio Code**
- **Git**

Puedes verificarlo con:

```bash
node -v
npm -v
git --version
```

---

# 🚀 Instalación del Proyecto

Clona el repositorio e instala las dependencias.

```bash
git clone <repository-url>
cd <project-folder>
npm install
```

---

# 🧩 Extensiones Recomendadas de VS Code

Este proyecto utiliza algunas extensiones para garantizar calidad y consistencia en el código.

| Extensión | Propósito                                       |
| --------- | ----------------------------------------------- |
| ESLint    | Detectar errores y aplicar estándares de código |
| Prettier  | Formateo automático del código                  |

Cuando abras el proyecto en VS Code se recomendarán automáticamente gracias al archivo:

> .vscode/extensions.json

---

# 🛠️ Configuración Local de VS Code

La configuración del editor está definida en:

> .vscode/settings.json

Esta configuración permite:

- Formateo automático al guardar
- Corrección automática de ESLint
- Reglas de formato consistentes

\
Importante:\
Estas configuraciones solo aplican a este proyecto y no modifican tu configuración global de VS Code.

---

# 🔍 Configuración de ESLint

ESLint se utiliza para mantener la calidad del código y detectar problemas comunes.

Archivo de configuración:

> .eslintrc.json

Para ejecutar el análisis manualmente:

```bash
npm run lint
```

Esto analizará todo el proyecto y mostrará posibles errores o advertencias.

---

# 🎨 Configuración de Prettier

Prettier se utiliza para asegurar un formato consistente del código en todo el proyecto.

Archivo de configuración:

> .prettierrc

Para formatear todo el proyecto manualmente:

```bash
npm run format
```

---

# 📦 Scripts Disponibles

| Comando        | Descripción                     |
| -------------- | ------------------------------- |
| npm install    | Instala dependencias            |
| npm run lint   | Ejecuta ESLint                  |
| npm run format | Formatea el código con Prettier |

---

# 🔒 Pre-commit Hooks (Husky + lint-staged)

Este proyecto utiliza **pre-commit hooks** para garantizar la calidad del código antes de que cualquier cambio sea confirmado en el repositorio.

Antes de cada `git commit`, se ejecutan automáticamente herramientas de análisis y formateo.

Herramientas utilizadas:

| Herramienta | Propósito                                     |
| ----------- | --------------------------------------------- |
| Husky       | Permite ejecutar scripts en hooks de Git      |
| lint-staged | Ejecuta comandos solo en archivos modificados |
| ESLint      | Detecta errores de código                     |
| Prettier    | Formatea automáticamente el código            |

---
