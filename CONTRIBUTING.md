# Contributing to Nodiki

Thank you for considering contributing to **Nodiki**!  
This document will help you get started and stay aligned with the project's philosophy and standards.

***

## 🚀 Project Setup

### Backend

```bash
cd backend
./gradlew bootRun
```

- Requires Java 17+
- API runs at: `http://localhost:8080`
- Swagger: `http://localhost:8080/swagger-ui.html`

### Frontend

```bash
cd frontend
npm install
npm run dev
```

- Runs at: `http://localhost:5173`

***

## 🧠 Development Principles

- Keep code clean, simple, and well-documented.
- Follow established architectural patterns (e.g., service/controller separation).
- Prefer readability over cleverness.
- Think in terms of logic, meaning, and connections — just like the project’s purpose.

***

## 📝 Making Contributions

1. **Fork the repository** (if you're an external contributor).
2. Create a branch from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes.
4. Test your code locally.
5. Commit with a meaningful message:
   ```
   git commit -m "Add: user authentication feature"
   ```
6. Push your branch:
   ```
   git push origin feature/your-feature-name
   ```
7. Open a Pull Request.

***

## 🔍 Code Style & Documentation

- Java: Use `@Operation`, `@Tag` (Swagger), and `@Service`, `@Repository`, etc.
- TypeScript: Use JSDoc for all exports, functions, and components.
- Keep styles in `.css` files, not inline.

***

## 🧪 Testing (WIP)

- Backend: Spring Boot Test
- Frontend: Coming soon — Jest / Playwright

***

## 🧭 Philosophy Reminder

Nodiki is about **thought**, **structure**, and **clarity**.  
Every line of code should help bring clarity to the world of information chaos.

***

Happy contributing! 🧠
