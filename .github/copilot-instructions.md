<!-- Copilot instructions for AI coding agents -->
# Quick Agent Guide for this repo

This is a small static portfolio site. The guidance below focuses on concrete, discoverable patterns so an AI can be immediately productive.

**Project Overview**
- **Type:** Static HTML site (no build system). Entry: [index.html](index.html).
- **Content folders:** Images in `images/`. Page stubs live in `pages/` (currently empty).

**Key Files**
- **Entry:** [index.html](index.html) — single-page structure with header, `nav`, `main` sections and footer.
- **Assets:** `images/` — keep image filenames relative and update `src` paths accordingly.

**Conventions & Patterns (observable in repo)**
- **No package manager or build step:** Do not add or assume `package.json`, `npm`, or other tooling unless the user explicitly asks to introduce them.
- **Structure:** The site uses semantic sections (e.g., `<section id="services">`). When adding content, preserve IDs to avoid breaking internal anchors.
- **Navigation:** The header nav is a simple `<ul><li><a>` list in [index.html](index.html). Edit items in that single file rather than scattering navigation across multiple files.
- **Assets referencing:** Use relative paths (e.g., `images/logo.png`) — keep folder names lowercase and match existing names.

**Safety & Scope for Agents**
- **Do not scaffold backend code** (Express, Flask, etc.) — this repo has no backend and the user did not request one.
- **Avoid adding heavy toolchains** (Webpack, Vite) without explicit permission.

**Common Tasks Examples**
- **Add a new page file:** create `pages/about.html` and link it from the nav in [index.html](index.html). Keep the same header/nav/footer markup so navigation remains consistent.
- **Add an image:** put file in `images/` and reference as `<img src="images/your.png" alt="...">`.
- **Add a section block:** follow the existing pattern: `<section id="portfolio"></section>` and populate inner semantic HTML.

**Developer workflow notes**
- **Preview:** open `index.html` directly in a browser to verify layout and links.
- **Testing / Linting:** none provided in repo. If adding tooling, explain changes to the user and provide minimal setup steps.

**Commit & PR Guidance for AI changes**
- **Scope commits narrowly:** one logical change per commit (e.g., "Add about page and nav link").
- **Include short human-facing PR description** explaining why the change was needed and how to preview it.

If any parts of this guidance are unclear or you want the agent to follow a different convention (add CSS framework, introduce a build tool, or scaffold multiple pages), say so and I will adapt the instructions.
