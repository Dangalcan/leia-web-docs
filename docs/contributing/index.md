---
sidebar_position: 1
---

# Contributing to LEIA Documentation

Thank you for your interest in contributing to the LEIA documentation! This guide will help you get started with the technical setup and our preferred contribution workflow.

---

## 🚀 Getting Started

To contribute to this documentation, you'll need a local development environment.

### Prerequisites
- **Node.js**: Version 18.0 or higher.
- **npm**: Usually comes with Node.js.

### Local Development Setup

Please fork the official repository and clone your fork.

1. **Clone the repository**:
   ```bash
   git clone <your-fork-url>
   cd your-fork-name
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Start the development server**:
   ```bash
   npm start
   ```
   The site will be available at `http://localhost:3000`.

---

## 📂 Project Structure

We follow a clean and categorized architecture for our documentation.

### Documentation Files
All documentation lives in the `docs/` folder, organized by category:
- `docs/introduction/`: Core concepts and general workflow.
- `docs/tutorials/`: Step-by-step guides for users.
- `docs/contributing/`: This guide and other meta-docs.

### Centralized Asset Management
We use **Asset Mirroring**. Do not store images inside the corresponding `docs/` folder. Instead:
1. Place images in `docs/img/`.
2. Mirror the folder structure of the documentation.
   - Example: Image for `docs/tutorials/create-leia/` goes into `docs/img/tutorials/create-leia/`.
3. Reference images using absolute paths: `![Alt Text](/img/tutorials/create-leia/image.png)`.

---

## ✍️ Contribution Workflow

1. **Create a branch**: Use a descriptive name like `feat/new-tutorial` or `fix/typo`.
2. **Write your content**:
   - Use **Markdown** for formatting.
   - Include **Frontmatter** at the top of new files (e.g., `sidebar_position`).
   - Use `slug: /` if you want a file to be the home page of a category.
3. **Formatting & Style**:
   - We use **Tailwind CSS** for custom components.
   - Design follows a **Glassmorphism** aesthetic (use `.glass-card` and `.glass-panel` classes).
4. **Versioning**:
   - If you are making changes for a specific version, locate it in `versioned_docs/`.
   - To create a new version of the entire documentation, run:
     ```bash
     npm run docusaurus docs:version <version_name>
     ```
5. **Submit a Pull Request**: Provide a clear description of your changes and wait for review.

---

## 🎨 Styling Guidelines

The LEIA brand uses a vibrant, modern palette:
- **Primary Color**: Vibrant Violet (`#7c3aed`).
- **Secondary Colors**: Sleek Slate and Gradient Blues.
- **Components**: Prefer using pre-defined utility classes in `src/css/custom.css`.

---

Happy coding! If you have any questions, feel free to reach out to the team at Github Issues panel.
