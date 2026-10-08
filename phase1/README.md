# Phase 1: Beginner Single-Stage Docker Build

Phase 1 demonstrates a basic, single-stage Docker setup using a standard Linux base image (`ubuntu:22.04`).

## Characteristics

- **Base Image**: `ubuntu:22.04`
- **Setup**: Manually installs `python3` and `python3-pip` via `apt-get`.
- **Application**: FastAPI microservice serving basic endpoints (`/`, `/health`, `/info`).
- **Purpose**: Ideal for understanding the fundamental building blocks of Docker images before applying image size and build pipeline optimizations in Phase 2.

## How to Run

From the repository root:

```bash
docker build -t api-gateway:phase1 ./phase1
docker run -d -p 8000:8000 --name api-gateway-phase1 api-gateway:phase1
```
