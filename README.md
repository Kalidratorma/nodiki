# Nodiki

Welcome to the monorepo of **Nodiki.com** — a platform for visual thinking, structured analysis, and collaborative forecasting.

## 📂 Repository Structure

```
nodiki/
├── backend/           # Spring Boot REST API (Java)
├── frontend/          # React + TypeScript + ReactFlow
├── project-docs/      # Documentation for architecture, planning, vision
```

## 🚀 Getting Started

### Backend
```bash
cd backend
./gradlew bootRun
```
App runs on: `http://localhost:8080`

### Frontend
```bash
cd frontend
npm install
npm run dev
```
App runs on: `http://localhost:5173`

Make sure both servers are running simultaneously.

## 📖 Documentation
Full documentation is located in [`project-docs/`](./docs):

- `vision.md` — purpose, philosophy, audience
- `architecture.md` — full-stack architecture
- `tech-decisions.md` — rationale for stack choices
- `api.md` — API structure + Swagger link
- `roadmap.md` — current and planned features

## 🧩 Core Concepts
- Cards (nodes) = facts, events, thoughts
- Edges (connections) = logic, causality, prediction links
- Prediction nodes = forecast outcomes
- Boards = user-owned logical spaces
- Public/Private sharing + rating predictions

## 🔐 Auth (planned)
- JWT-based authentication (Spring Security)
- User-specific boards

## 🛣️ Road Ahead
Check [`roadmap.md`](./docs/roadmap.md) for what's next!

## 🤝 Contributing

We welcome contributions!  
Check out [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to help.

---

Made with 🧠 and ❤️ by Vladimir & Алексей
