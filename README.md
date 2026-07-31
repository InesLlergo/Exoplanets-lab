<div align="center">

# Exoplanets Lab

**Aplicación web interactiva sobre exoplanetas: simulador del método de tránsito, exploración y quiz.**

[![Live demo](https://img.shields.io/badge/demo-exoplanetslab.vercel.app-4F46E5?style=for-the-badge)](https://exoplanetslab.vercel.app/lab)
![Astro 5](https://img.shields.io/badge/Astro-5-BC52EE?style=for-the-badge&logo=astro&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

</div>

---

# ENGLISH VERSION

## Overview

**Exoplanets Lab** is an interactive educational web application about exoplanets, built with **Astro**. Its centerpiece is an **interactive transit-method simulator** — the key technique used to detect planets outside our solar system — rendered in real time on HTML canvas, alongside an exoplanet **quiz** and an **exploration** section.

Built as a team project and **deployed at [exoplanetslab.vercel.app](https://exoplanetslab.vercel.app/lab)**.

## Features

- **Interactive transit simulator** (`/lab`): animated visualization of an exoplanet transiting its star, with real-time parameter controls:
  - Simulation speed
  - Planet mass, radius and orbital parameters
  - Play / reset controls
  - Live light-curve plot alongside the system view (HTML canvas)
- **Quiz** (`/quiz`): knowledge questions about exoplanets
- **Explore** (`/explore`): exoplanet analysis results section
- **Menu** (`/menu`): adventure-style navigation
- **Custom UI kit**: `Badge`, `Button`, `Card` (header/title/description/footer/content) and `Dropdown` components
- **Icon set** with `astro-icon` and shared design tokens (`lib/button-variants.ts`)

## Tech Stack

| Technology | Purpose | Official docs |
|---|---|---|
| [Astro 5](https://astro.build) | Static site framework | [Astro Docs](https://docs.astro.build) |
| [astro-icon](https://github.com/natemoo-re/astro-icon) | SVG icon system | [astro-icon docs](https://astro-icon.dev) |
| [TypeScript](https://www.typescriptlang.org) | Typed language | [TypeScript Handbook](https://www.typescriptlang.org/docs/) |
| HTML Canvas API | Real-time simulation rendering | [MDN Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) |

## Project Structure

```text
src/
├── Components/
│   ├── ui/                    # Badge, Button, Card, Dropdown (shadcn-style)
│   ├── astro/                 # Astro-specific components
│   └── WebAppExoplanet.astro
├── assets/                    # Static assets
├── icons/                     # SVG icons (astro-icon)
├── i18n/                      # ui.ts (i18n dictionary)
├── layouts/
│   └── Layout.astro           # Base layout
├── lib/                       # Shared logic (button variants)
├── scripts/                   # Utilities
└── pages/
    ├── index.astro            # Welcome
    ├── menu.astro             # Choose your adventure
    ├── lab.astro              # Transit simulator (canvas + controls)
    ├── explore.astro          # Exoplanet analysis results
    └── quiz.astro             # Exoplanet quiz
```

## Getting Started

### Commands

```bash
npm install     # install dependencies
npm run dev     # dev server on http://localhost:4321
npm run build   # production build to ./dist/
npm run preview # preview the production build locally
npm run astro   # Astro CLI (astro check, astro add...)
```

> See the [Astro CLI reference](https://docs.astro.build/en/reference/cli-reference/) for all available commands.

## Roadmap

- [ ] Complete the i18n dictionary and apply translations
- [ ] Add real exoplanet data from an open catalog (e.g. [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu))
- [ ] Interactive planet classification activity
- [ ] Unit tests (see [Astro testing guide](https://docs.astro.build/en/guides/testing/))

## Official Documentation

- [Astro Docs](https://docs.astro.build) — concepts and guides
- [Astro configuration reference](https://docs.astro.build/en/reference/configuration-reference/)
- [Astro CLI reference](https://docs.astro.build/en/reference/cli-reference/)
- [MDN Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) — rendering the simulator
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)

## Team

- [Inés Llergo](https://github.com/InesLlergo) — repository owner
- [Fernando Rodríguez López](https://github.com/FerLpz55) — development
- [Gomen](https://github.com/Leviakc) — development
- DanDev — development

---

# VERSIÓN EN ESPAÑOL

## Descripción General

**Exoplanets Lab** es una aplicación web educativa e interactiva sobre exoplanetas construida con **Astro**. Su pieza central es un **simulador interactivo del método de tránsito** — la técnica clave para detectar planetas fuera de nuestro sistema solar — renderizado en tiempo real con HTML canvas, además de un **quiz** de exoplanetas y una sección de **exploración**.

Proyecto de equipo, **desplegado en [exoplanetslab.vercel.app](https://exoplanetslab.vercel.app/lab)**.

## Características

- **Simulador de tránsito interactivo** (`/lab`): visualización animada de un exoplaneta transitando frente a su estrella, con controles de parámetros en tiempo real:
  - Velocidad de la simulación
  - Masa, radio y parámetros orbitales del planeta
  - Controles de reproducir / reiniciar
  - Curva de luz en vivo junto a la vista del sistema (HTML canvas)
- **Quiz** (`/quiz`): preguntas de conocimiento sobre exoplanetas
- **Explorar** (`/explore`): sección de resultados de análisis de exoplanetas
- **Menú** (`/menu`): navegación estilo aventura
- **Kit de UI propio**: componentes `Badge`, `Button`, `Card` (header/title/description/footer/content) y `Dropdown`
- **Set de íconos** con `astro-icon` y tokens de diseño compartidos (`lib/button-variants.ts`)

## Stack Tecnológico

| Tecnología | Propósito | Documentación oficial |
|---|---|---|
| [Astro 5](https://astro.build) | Framework de sitio estático | [Astro Docs](https://docs.astro.build) |
| [astro-icon](https://github.com/natemoo-re/astro-icon) | Sistema de íconos SVG | [astro-icon docs](https://astro-icon.dev) |
| [TypeScript](https://www.typescriptlang.org) | Lenguaje tipado | [TypeScript Handbook](https://www.typescriptlang.org/docs/) |
| HTML Canvas API | Renderizado de la simulación en tiempo real | [MDN Canvas API](https://developer.mozilla.org/es/docs/Web/API/Canvas_API) |

## Estructura del Proyecto

```text
src/
├── Components/
│   ├── ui/                    # Badge, Button, Card, Dropdown (estilo shadcn)
│   ├── astro/                 # Componentes específicos de Astro
│   └── WebAppExoplanet.astro
├── assets/                    # Recursos estáticos
├── icons/                     # Íconos SVG (astro-icon)
├── i18n/                      # ui.ts (diccionario i18n)
├── layouts/
│   └── Layout.astro           # Layout base
├── lib/                       # Lógica compartida (button variants)
├── scripts/                   # Utilidades
└── pages/
    ├── index.astro            # Bienvenida
    ├── menu.astro             # Elige tu aventura
    ├── lab.astro              # Simulador de tránsito (canvas + controles)
    ├── explore.astro          # Resultados de análisis de exoplanetas
    └── quiz.astro             # Quiz de exoplanetas
```

## Cómo Empezar

### Comandos

```bash
npm install     # instalar dependencias
npm run dev     # servidor de desarrollo en http://localhost:4321
npm run build   # compilación de producción en ./dist/
npm run preview # previsualizar la compilación de producción
npm run astro   # CLI de Astro (astro check, astro add...)
```

> Consulta la [referencia de CLI de Astro](https://docs.astro.build/es/reference/cli-reference/) para todos los comandos disponibles.

## Mejoras Planeadas

- [ ] Completar el diccionario i18n y aplicar las traducciones
- [ ] Agregar datos reales de exoplanetas de un catálogo abierto (p. ej. [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu))
- [ ] Actividad interactiva de clasificación de planetas
- [ ] Pruebas unitarias (ver [guía de testing de Astro](https://docs.astro.build/en/guides/testing/))

## Documentación Oficial

- [Astro Docs](https://docs.astro.build) — conceptos y guías
- [Referencia de configuración de Astro](https://docs.astro.build/en/reference/configuration-reference/)
- [Referencia de CLI de Astro](https://docs.astro.build/en/reference/cli-reference/)
- [MDN Canvas API](https://developer.mozilla.org/es/docs/Web/API/Canvas_API) — renderizado del simulador
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)

## Equipo

- [Inés Llergo](https://github.com/InesLlergo) — dueña del repositorio
- [Fernando Rodríguez López](https://github.com/FerLpz55) — desarrollo
- [Gomen](https://github.com/Leviakc) — desarrollo
- DanDev — desarrollo
