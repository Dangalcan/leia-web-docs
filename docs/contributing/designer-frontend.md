---
sidebar_position: 3
---

# Designer Frontend

**Repository:** [leia-org/leia-designer-frontend](https://github.com/leia-org/leia-designer-frontend)

The web interface used by instructors to create, configure, and test LEIAs. Built with **React**, **TypeScript**, and **Vite**.

---

## Prerequisites

- **Node.js** >= 18.x
- **npm** or **pnpm**

---

## Local Development

1. Fork and clone the repository:
   ```bash
   git clone <your-fork-url>
   cd leia-designer-frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:5173`.

---

## Tech Stack

| Technology | Purpose |
|---|---|
| React + TypeScript | UI framework |
| Vite | Build tool and dev server |
| TailwindCSS | Styling |
| ESLint | Code quality |

---

## Contributing

1. Fork the repository and create your branch: `feat/my-feature`.
2. Follow the ESLint configuration in the project — do not disable rules without justification.
3. Make sure the app builds correctly: `npm run build`.
4. Open a Pull Request with screenshots if you changed any UI elements.
