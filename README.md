# ASI Mercury Geospatial Node API

### Arybit Super Intelligence · Geospatial Intelligence Infrastructure

**ASI Mercury Geospatial Node API** is a FastAPI-based geospatial processing service developed as part of the **Arybit Super Intelligence Mercury** ecosystem.

It provides an independent API and worker execution environment for Earth-observation processing, geospatial intelligence, environmental evidence analysis, mission workflows, dataset integrations, and private mission artifacts.

The service is designed to support scalable geospatial operations while maintaining modularity, independent testability, and integration with the wider Arybit Intelligence infrastructure.

---

## Production & Development

| Environment | Endpoint |
|---|---|
| Production | https://asi-mercury-geospatial-node-api.arybit.co.ke |
| Local | http://127.0.0.1:8000 |
| Interactive API Documentation | `/docs` |
| Alternative API Documentation | `/redoc` |
| OpenAPI Schema | `/openapi.json` |

**Local endpoint:** The service binds to loopback (`127.0.0.1:8000`) for standalone local development.

---

## Core Capabilities

### 1. Earth Observation Processing
- Earth-observation processing entry points.
- Geospatial dataset ingestion and processing.
- Remote-sensing workflow integration.
- Spatial evidence preparation and analysis.

### 2. Geospatial Intelligence
- Geospatial processing services.
- Environmental evidence analysis.
- Spatial data integration.
- Mission-oriented geospatial workflows.

### 3. Dataset & Provider Integrations
- Dataset integration interfaces.
- External geospatial provider connectivity.
- Data processing orchestration.
- Extensible provider architecture.

### 4. Mission Workflows
- Mission execution workflows.
- Background processing jobs.
- Asynchronous task orchestration.
- Private mission artifact management.

### 5. API Infrastructure
- FastAPI application architecture.
- Independent API execution.
- Worker execution environment.
- Modular service integration.
- OpenAPI-compatible documentation.

---

## Architecture

ASI Mercury Geospatial Node API operates as an independent processing component within the broader Arybit Intelligence ecosystem.

```text
ARYBIT SUPER INTELLIGENCE
          |
          v
     ASI MERCURY
          |
          v
 GEOSPATIAL NODE API
          |
    +-----+------+
    |            |
    v            v
  REST API    WORKERS
    |            |
    +------+-----+
           |
           v
  GEOSPATIAL PROCESSING
           |
    +------+------+ 
    |      |      |
    v      v      v
 EARTH  DATASET  ENVIRONMENTAL
 OBS.   PROVIDERS EVIDENCE
    |      |      |
    +------+------+
           |
           v
    MISSION WORKFLOWS
           |
           v
   PRIVATE ARTIFACTS
```

---

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application language |
| FastAPI | API framework |
| REST | Service communication |
| OpenAPI | API specification |
| Background Workers | Asynchronous processing |
| Geospatial Tooling | Spatial data processing |

---

## Local Development

### Prerequisites

- Python 3.10+
- pip
- Git

### Clone the repository

```bash
git clone https://github.com/asi-mercury-geospatial-node-api/asi-mercury-geospatial-node-api.git

cd asi-mercury-geospatial-node-api
```

### Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the application

The application entry point should match the actual FastAPI module in the project.

Example:

```bash
uvicorn app.main:app --host 127.0.0.1 --port 8000 --reload
```

Open:

```text
http://127.0.0.1:8000/docs
```

---

## Production Deployment

Production service:

https://asi-mercury-geospatial-node-api.arybit.co.ke

The production deployment is intended to operate independently while integrating with the wider Arybit Intelligence ecosystem.

Recommended operational practices:

- HTTPS-enabled service access.
- Environment-based configuration.
- Secure secrets management.
- Controlled mission artifact storage.
- Background worker isolation.
- API monitoring and structured logging.
- Health checks and service availability monitoring.

---

## Security & Data Governance

Security is an important architectural consideration.

The service is designed to support:

- Protected mission artifacts.
- Secure provider integrations.
- Environment-managed credentials.
- Controlled access to operational resources.
- Separation of application code and sensitive configuration.

Never commit API keys, passwords, access tokens, private datasets, or mission-sensitive artifacts to the public repository.

---

## Project Positioning

**ASI Mercury Geospatial Node API** is an infrastructure component of Arybit Super Intelligence Mercury.

Its role is to provide dedicated geospatial processing and environmental intelligence capabilities through an independently deployable API and worker environment.

The architecture emphasizes modularity, integration, extensibility, and operational independence.

---

## Organization

**Arybit Super Intelligence (ASI)**

**Platform:** Mercury  
**Service:** Geospatial Node API  
**Category:** Geospatial Intelligence Infrastructure  
**Framework:** FastAPI  
**Deployment:** Production and standalone local environments

---

## License

No license has currently been specified.

All rights are reserved by the respective project owner unless otherwise stated.

---

*ASI Mercury · Geospatial Intelligence Infrastructure · Arybit Super Intelligence*
