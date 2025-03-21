# Roadmap — Nodiki

This document outlines the current progress and planned features for https://nodiki.com.
It serves as a living reference and development compass.

---

## ✅ Phase 1 — MVP (Completed)

- [x] Add, move, and delete nodes
- [x] Create and edit edges between nodes
- [x] Editable labels for nodes and edges
- [x] Node positions persist after reload
- [x] REST API (Spring Boot)
- [x] React frontend with React Flow
- [x] Swagger + Lombok + TypeScript

---

## 🔄 Phase 2 — Internal Structuring

- [x] Frontend/backend refactoring (feature folders, services, DTOs)
- [x] TypeScript conversion and cleanup
- [x] Move styles to external CSS files
- [x] API documentation
- [x] Project documentation in `/docs`
- [ ] Introduce basic validation (backend + frontend)

---

## 🔐 Phase 3 — User & Board System

- [ ] Add authentication (JWT + Spring Security)
- [ ] User accounts and roles
- [ ] User-specific boards
- [ ] Public and private board modes
- [ ] Board switcher in UI
- [ ] **Prepare internal test environment (private beta group)**

---

## 🌐 Phase 4 — Content Integration & Prediction

- [ ] **Add node from external URL**
  - [ ] Parse title, summary, and source
  - [ ] Fetch via OpenGraph, readability or AI
- [ ] Add prediction node type
- [ ] Link logical connections to predictions
- [ ] User reputation/karma based on prediction outcomes
- [ ] Public ratings on predictions

---

## 🧠 Phase 5 — Advanced Features

- [ ] AI-assisted pattern suggestion system
- [ ] Real-time collaboration (WebSocket or polling)
- [ ] Version history for boards
- [ ] Filtering/tagging for large boards
- [ ] Markdown support in node content

---

## 🌍 Phase 6 — Launch & Community

- [ ] Landing page at https://nodiki.com
- [ ] Public documentation access
- [ ] Invite-only beta access for early users
- [ ] Feedback collection system (manual or AI)
- [ ] Prepare for open public launch

---

This roadmap evolves as we do.

