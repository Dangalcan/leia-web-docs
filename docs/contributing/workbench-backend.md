---
sidebar_position: 7
---

# Workbench Backend

**Repository:** [leia-org/leia-workbench-backend](https://github.com/leia-org/leia-workbench-backend)

The backend API powering the LEIA Workbench, managing experiments, student sessions, submissions, and evaluation results.

---

## Prerequisites

Check the repository's README for the required runtime version and any environment variables needed.

---

## Local Development

1. Fork and clone the repository:
   ```bash
   git clone <your-fork-url>
   cd leia-workbench-backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure environment variables (see `.env.example`).
4. Start the server:
   ```bash
   npm run dev
   ```

---

## Contributing

1. Fork the repository and branch off `main`: `feat/my-feature`.
2. Ensure new endpoints have proper validation, authentication, and error handling.
3. Write or update tests for your changes.
4. Open a Pull Request with a clear description of the API changes made.
