# Architecture — Nodiki

This document describes the high-level system design of Nodiki.
It reflects how the frontend, backend, database, and API interact.

---

### 🏗️ System Overview

```
+-------------+         REST API         +-------------+         +-------------+
|  Frontend   |  <-------------------->  |  Backend    |  <----> |  Database   |
| (React + TS)|                         | (Spring Boot)|         | (PostgreSQL)|
+-------------+                         +-------------+         +-------------+
```

---

### 🧩 Frontend

- Framework: React + TypeScript
- Styling: TailwindCSS
- Diagram library: React Flow
- Features:
  - Interactive board with draggable nodes
  - Connectable edges with descriptions
  - Editable content
  - Communication with backend via REST API (using fetch)

#### File Structure (plan)
```
frontend/
├── features/
│   ├── nodes/
│   └── edges/
├── shared/
│   ├── api/
│   ├── hooks/
│   ├── ui/
│   └── types/
```

---

### 🔧 Backend

- Framework: Spring Boot (Java 17)
- Documentation: Swagger (OpenAPI 3)
- Boilerplate: Lombok
- Persistence: Spring Data JPA
- Features:
  - REST API for nodes and edges
  - Swagger-generated interactive API docs
  - Position, label, and connection editing

#### Layered structure
```
backend/
├── controller/
├── service/
├── repository/
├── model/
├── dto/
```

---

### 💾 Database

- Current: In-memory (H2 or similar) during development
- Future: PostgreSQL (or another persistent relational DB)
- Entities:
  - Node (id, label, x, y)
  - Edge (id, sourceId, targetId, description)
  - Future: User, Board, Prediction, Rating

---

### 🌐 API Layer

- REST over HTTP (JSON)
- Swagger UI: `https://nodiki.com/swagger-ui.html`
- Endpoints:
  - `GET /api/nodes`, `POST`, `PUT`, `DELETE`
  - `GET /api/edges`, `POST`, `PUT`, `DELETE`

---

### 📌 Planned Improvements

- Auth & Users
- Boards (public/private)
- Roles and access control
- WebSocket for live sync (optional)
- GraphQL (future)
- Testing & validation

Architecture evolves as we grow. This doc stays in sync.
