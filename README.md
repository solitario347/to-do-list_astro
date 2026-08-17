# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).


# Sistema de Gestión de Citas - Astro

Aplicación web desarrollada con **Astro** para la gestión y agendamiento de citas en línea, con control de navegación y redirección por roles.

## 🚀 Vista General y Rutas

- **Página Principal (`/`):** Presentación del sistema con acceso directo al inicio de sesión y vista previa al Dashboard (Demo).
- **Inicio de Sesión (`/login`):** Formulario con redirección inteligente según el usuario:
  - **Cliente:** Redirige a `/dashboard`.
  - **Administrador:** Redirige a `/admin` (para correos que contengan `admin`).
- **Panel del Cliente (`/dashboard`):** Consulta de citas activas, estados (Confirmada/Pendiente) y acceso al botón para agendar.
- **Agendar Cita (`/agendar`):** Formulario para seleccionar servicio, fecha, hora y agregar notas adicionales.
- **Panel Administrativo (`/admin`):** Tabla general para la gestión, aprobación y rechazo de citas registradas.

## 🛠️ Tecnologías

- **Framework:** Astro
- **Lenguajes:** TypeScript, HTML5, CSS3
- **Control de Versiones:** Git & GitHub

## 🔧 Ejecución en Local

1. Instalar dependencias:
   ```bash
   npm install