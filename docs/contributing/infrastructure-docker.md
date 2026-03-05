---
sidebar_position: 2
---

# Infrastructure Docker

**Repository:** [leia-org/leia-infrastructure-docker](https://github.com/leia-org/leia-infrastructure-docker)

Docker Compose configurations for orchestrating the complete LEIA system infrastructure, including all 5 microservices, databases (MongoDB and Redis), and network configuration for local development and deployment.

---

## System Overview

The LEIA stack consists of 5 services:

| Service | Role |
|---|---|
| `leia-designer-backend` | REST API for the Designer |
| `leia-designer-frontend` | Web UI for instructors |
| `leia-workbench-backend` | REST API for the Workbench |
| `leia-workbench-frontend` | Web UI for workbench users |
| `leia-runner` | AI session execution engine |

---

## Prerequisites

- **Docker** and **Docker Compose** installed.
- Docker images of all 5 services published to the GitHub Container Registry (done automatically via GitHub Actions).

---

## Quick Start

1. Copy the example `.env` file and fill in your values:
   ```bash
   cp .env.example .env
   ```
2. Start the full system:
   ```bash
   docker-compose up -d
   ```
3. To run only the Designer services:
   ```bash
   docker-compose -f docker-compose.designer.yml up -d
   ```
4. To run only the Workbench services:
   ```bash
   docker-compose -f docker-compose.workbench.yml up -d
   ```

---

## Key Environment Variables

| Variable | Description |
|---|---|
| `MONGO_URI` | MongoDB connection string |
| `REDIS_URL` | Redis connection string |
| `JWT_SECRET` | Secret for auth tokens |
| `OPENAI_API_KEY` | AI/ML provider key |

See the README in the repository for the full list.

---

## Contributing

1. Fork the repository.
2. Clone your fork and create a `.env` from `.env.example`.
3. Make your changes to `docker-compose.yml` or service configs.
4. Test locally with `docker-compose up`.
5. Open a Pull Request describing your changes.
