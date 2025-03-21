# API Overview — Nodiki

This document provides a high-level overview of the REST API available in Nodiki.

The full interactive documentation is available at:

👉 [https://nodiki.com/swagger-ui.html](https://nodiki.com/swagger-ui.html)

---

## 📌 Base URL

```
https://nodiki.com/api
```

---

## 🧠 Nodes

- `GET /nodes` — get all nodes
- `POST /nodes` — create new node
- `PUT /nodes/{id}/label` — update node label
- `PUT /nodes/{id}/position` — update node position
- `DELETE /nodes/{id}` — delete a node

### Node Object
```json
{
  "id": "string",
  "label": "string",
  "position": {
    "x": 0,
    "y": 0
  }
}
```

---

## 🔗 Edges

- `GET /edges` — get all edges
- `POST /edges` — create new edge
- `PUT /edges/{id}/label` — update edge label
- `DELETE /edges/{id}` — delete an edge

### Edge Object
```json
{
  "id": "string",
  "source": "nodeId",
  "target": "nodeId",
  "label": "string"
}
```

---

## 🔐 Planned Endpoints

- `POST /auth/register` — user registration
- `POST /auth/login` — login with JWT
- `GET /boards` — list user boards
- `POST /boards` — create board
- `GET /boards/{id}` — get board with nodes/edges

---

## 🧪 Testing the API

Use Swagger at [https://nodiki.com/swagger-ui.html](https://nodiki.com/swagger-ui.html) to try out the endpoints.

This document provides a static summary — Swagger stays live and up to date.
