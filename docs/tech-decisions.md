# Technical Decisions — Nodiki

This document outlines the key technologies and architectural choices made for Nodiki.com and the rationale behind them.

---

## 🧱 Project Structure

- **Monorepo**: Combined repository for frontend, backend, and documentation.
- **Directory layout**:
  - `backend/`: Spring Boot REST API
  - `frontend/`: React + TypeScript + ReactFlow client
  - `docs/`: Markdown documentation

---

## 🔧 Backend: Spring Boot

- **Framework**: Spring Boot (Java 17)
- **Why**:
  - Production-ready and mature
  - Excellent support for REST APIs and dependency injection
  - Easy to document using Swagger/OpenAPI
- **Tools**:
  - Lombok — reduce boilerplate
  - Spring Data JPA — database access
  - Gradle — modern build system

---

## 💡 Frontend: React + TypeScript

- **Framework**: React
- **Why**:
  - Strong ecosystem and community
  - Great for building highly interactive UIs
  - Seamless integration with React Flow
- **Enhancements**:
  - TypeScript — type safety, better tooling
  - TailwindCSS — utility-first styling
  - React Flow — graph visualizations with full control

---

## 🧠 UI/UX Philosophy

- Interactive, clear and focused interface
- Prioritizes logic over visual overload
- Designed to feel like a virtual thinking board

---

## ⚙️ API & Communication

- **REST over HTTP** using JSON
- Swagger/OpenAPI for documentation
- Future-ready for transition to GraphQL if needed

---

## 📄 Documentation

- Markdown-first (`docs/`)
- Technical and product-oriented docs
- Public entry point: [https://nodiki.com](https://nodiki.com)

---

## 🔐 Auth & Security (Planned)

- Spring Security with JWT tokens
- User-specific boards
- Private/public board sharing

---

## 🧪 Testing (Planned)

- Frontend: Jest, Playwright
- Backend: Spring Boot Test, Testcontainers

---

## 🌐 Deployment

- Cloud-ready
- Will be deployed to VPS and exposed via [https://nodiki.com](https://nodiki.com)

---

This document evolves along with the project.
