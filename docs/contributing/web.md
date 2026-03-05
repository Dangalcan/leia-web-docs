---
sidebar_position: 8
---

# Web (Documentation)

**Repository:** [leia-org/web](https://github.com/leia-org/web)

This is the repository for the LEIA documentation website — the site you are reading right now. Built with **Docusaurus 3**, **React**, and **TailwindCSS**.

---

## Prerequisites

- **Node.js** >= 18.x
- **npm**

---

## Local Development

1. Fork and clone the repository:
   ```bash
   git clone <your-fork-url>
   cd web
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
   The site will be available at `http://localhost:3000`.

---

## Project Structure

```
web/
├── docs/                  # Documentation content (Markdown)
│   ├── img/               # Versioning-sensitive images, mirrored by category
│   ├── introduction/      # Getting started docs
│   ├── tutorials/         # Step-by-step guides
│   └── contributing/      # This section
├── static/                # Brand assets (logo, favicon, social card)
├── src/                   # React components and custom pages
│   ├── components/        # Landing page components
│   ├── css/               # Global styles (TailwindCSS + custom)
│   └── pages/             # Custom pages (landing, versions)
└── docusaurus.config.js   # Site configuration
```

---

## Adding or Updating Documentation

### New Pages
1. Create a `.md` file inside the appropriate `docs/` category folder.
2. Add frontmatter:
   ```md
   ---
   sidebar_position: 2
   ---
   ```
3. Images go in `docs/img/<category>/` and are referenced with relative paths (e.g., `../img/introduction/image.png`).

### Versioning
To snapshot the current docs as a new version:
```bash
npm run docusaurus docs:version <version>
```

### Styling
- Global styles live in `src/css/custom.css`.
- Use predefined Tailwind classes and custom utilities like `.glass-card` and `.glass-panel`.
- Follow the LEIA brand: **Vibrant Violet** primary (`#7c3aed`), dark slate backgrounds.

---

## Contributing

1. Fork and clone the repository.
2. Follow the project structure above when adding new documentation.
3. Run `npm start` and verify your changes locally.
4. Open a Pull Request — include screenshots for any visual changes.
