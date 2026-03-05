---
sidebar_position: 4
---

# Designer Backend

**Repository:** [leia-org/leia-designer-backend](https://github.com/leia-org/leia-designer-backend)

The backend service powering the LEIA Designer, providing REST APIs for managing LEIAs, personas, problems, and experiments.

---

## Prerequisites

Check the repository's README for the required Node.js version and any environment variables needed.

---

## Local Development

1. Fork and clone the repository:
   ```bash
   git clone <your-fork-url>
   cd leia-designer-backend
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
2. Ensure new endpoints have appropriate validation and error handling.
3. Write or update tests for your changes.
4. Open a Pull Request with a clear description of the API changes.
