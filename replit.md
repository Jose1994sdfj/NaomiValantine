# replit.md

## Overview

This is a personal, single-page romantic/gift website titled "Para Naomi 💛" (For Naomi). It's a static frontend-only project built with HTML, CSS, and JavaScript, using Vite as the development server and build tool. The page features a visually rich, animated card-style layout with floating background elements, gradient backgrounds, and decorative animations — designed as a heartfelt digital message or love letter.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Pure HTML/CSS/JS**: No frontend framework (no React, Vue, etc.). The entire app is a single `index.html` file with inline `<style>` blocks for styling. There is also a `style.css` and `script.js` file, though the primary styles are currently embedded in the HTML.
- **Vite Dev Server**: Vite is used solely as a development server with hot module reloading (HMR) for live preview during development. It also handles production builds via `vite build`.
- **Google Fonts**: The project imports custom fonts (Pacifico, Nunito, Dancing Script) from Google Fonts CDN for decorative typography.
- **CSS Animations**: Heavy use of CSS keyframe animations (`rise`, `popIn`, `rainbow`) for floating background elements and entrance effects. CSS custom properties (variables) define the color palette.

### File Structure
- `index.html` — Main (and only) page. Contains all HTML structure and most CSS styles inline.
- `style.css` — Additional/base CSS reset styles (currently has generic resets and layout, appears to be from the template and partially unused).
- `script.js` — JavaScript file (currently empty). Available for adding interactivity.
- `vite.config.js` — Vite configuration. Sets up dev server on `0.0.0.0` with HMR enabled.
- `package.json` — Only dependency is Vite itself.

### Design Decisions
- **Inline styles in HTML**: The main styling lives inside `<style>` tags in `index.html` rather than in `style.css`. This is intentional for this type of simple, single-page personal project. When modifying styles, check `index.html` first.
- **No build-time CSS processing**: No Tailwind, PostCSS, or SASS. All CSS is vanilla.
- **No backend**: This is a purely static site with no server-side logic, API endpoints, or database.

## External Dependencies

### NPM Packages
- **Vite v5.4.8** — The only npm dependency. Used for development server (with HMR) and production builds. No other libraries or frameworks are installed.

### CDN Resources
- **Google Fonts** — Pacifico, Nunito (weights 400–900), and Dancing Script (weight 700) are loaded via the Google Fonts CDN.

### Databases & APIs
- None. This is a fully static, client-side-only project with no backend services, databases, or API integrations.