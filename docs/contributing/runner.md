---
sidebar_position: 5
---

# Runner (LEIA Customer API)

**Repository:** [leia-org/leia-runner](https://github.com/leia-org/leia-runner)

The LEIA Runner is the AI session execution engine. It exposes a REST API that manages LEIA instances, handles student–AI conversations, and integrates with LLM providers.

---

## Prerequisites

- **Node.js** >= 16.x
- **PNPM**
- **Redis**

---

## Local Development

1. Fork and clone the repository:
   ```bash
   git clone <your-fork-url>
   cd leia-runner
   ```
2. Install dependencies:
   ```bash
   pnpm install
   ```
3. Start the server:
   ```bash
   pnpm start
   ```
   Or in development mode with hot-reloading:
   ```bash
   pnpm run dev
   ```

---

## Key API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/leia` | Create a new LEIA instance |
| `POST` | `/leia/:id/message` | Send a message to a LEIA instance |
| `GET` | `/models` | List available LLM models |

See the full API documentation in the repository README.

---

## Contributing

1. Fork and clone the repository.
2. Ensure Redis is running locally before testing.
3. Add or update tests for any new API endpoints.
4. Open a Pull Request describing the changes to the session execution logic.
