# Reglas y Estándares del Proyecto: Portafolio Web (Astro)

Este archivo define las reglas maestras de desarrollo, diseño y arquitectura para este proyecto en Antigravity. Todas las tareas y modificaciones deben cumplir estrictamente con estos estándares.

---

## 1. Filosofía de Diseño (Anti-Clichés de IA)
- **Cero Estética Genérica de IA**: Prohibido usar el cliché de fondo negro puro con gradientes morados/cian saturados o brillos de neón exagerados.
- **Tipografía con Personalidad**: Usar combinaciones tipográficas modernas, limpias y de alto impacto (editorial o sans-serif contemporáneas como Satoshi, General Sans o Plus Jakarta Sans).
- **Jerarquía y Espaciado**: Espacios en blanco generosos, micro-interacciones suaves en hover/focus y layouts minimalistas de calidad de agencia.
- **Modo Claro / Oscuro Elegante**: Paletas sobrias, con contrastes cuidados (WCAG AAA/AA) y acabados profesionales.

---

## 2. Arquitectura Técnica y Rendimiento
- **Framework**: Astro (aprovechar la arquitectura de islas y 0 KB de JavaScript cliente por defecto).
- **Estilos**: Tailwind CSS moderno y utilitario.
- **HTML Semántico**: Estructura estricta con `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`.
- **Rendimiento Máximo (Lighthouse 100/100)**:
  - Carga prioritaria en imágenes críticas (Hero) y `loading="lazy"` en las secundarias.
  - Cero dependencias pesadas innecesarias.
  - Componentes accesibles (a11y) con soporte para navegación por teclado y lectores de pantalla.

---

## 3. Control de Versiones y Seguridad (Git)
- **Commits Atómicos**: Cada vez que se termine una sección o componente funcional, crear un commit descriptivo en Git (ej. `feat: agregar navbar responsivo con navegación`).
- **Seguridad de Credenciales**: Nunca almacenar claves o tokens en el código fuente. Todo valor sensible debe ir en variables de entorno (`.env`).
- **Reversibilidad**: Mantener el historial limpio para permitir rollbacks instantáneos si algún cambio no satisface las expectativas.

---

## 4. Estilo de Comunicación
- Explicar las decisiones clave de forma concisa y directa.
- Evitar relleno técnico redundante.
- Mantener al usuario informado de las vistas previas en `localhost:4321`.
