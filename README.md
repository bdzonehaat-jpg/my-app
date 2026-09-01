# 🧠 Open'Ix AI — Intelligence Platform

> **One Intelligence. Infinite Possibilities.**

Open'Ix AI is a premium, futuristic multi-model AI workspace and prompt intelligence platform. Designed with an ultra-sleek glassmorphic dark interface, Open'Ix AI provides unified access to multi-model AI chats, visual workflows, custom agents, and a dedicated prompt studio.

---

## 🎨 Project & Design Identity

- **Theme Mood:** Deep Purple × Graphite Gray × Midnight Black
- **Visual Style:** Premium • Glass UI • Minimal • Professional • Micro-Interactions
- **Color Palette:**
  - **Primary Purple:** `#7C3AED`
  - **Deep Purple:** `#4C1D95`
  - **Electric Violet:** `#A855F7`
  - **Midnight Background:** `#080B14`
  - **Graphite Surface:** `#111522`
  - **Elevated Surface:** `#181D2B`
  - **Border Accent:** `#2A3040`

---

## 🚀 Core Features

* 💬 **Multi-Model AI Chat:** Unified conversational UI supporting streaming, file/image inputs, and web search toggles.
* 🧠 **Open'Ix Model Hub:** Real-time routing across proprietary and provider models filtered by speed, context, and capabilities.
* ✨ **Prompt Intelligence Studio:** Goal-driven prompt enhancer, intent analyzer, and structure optimizer.
* 🤖 **AI Agent Builder:** Custom assistant setup with tool permissions, system prompts, and memory settings.
* ⚡ **Workflow Automation:** Visual node-based workflow pipeline (Triggers → AI Processing → Decisions → Actions).
* 🧪 **Open'Ix AI Lab:** Side-by-side model response comparisons and dynamic parameter tuning.
* 📁 **Prompt Dashboard:** Folder organization, dynamic tagging, list/grid views, and interactive context menus.

---

## 🛠️ Tech Stack & Architecture

### **Frontend**
* Framework: Next.js (App Router) + React + TypeScript
* Styling: Tailwind CSS + Custom Design System Tokens
* Components: Headless UI / Accessible Primitive System
* Animations: Framer Motion

### **Backend & Storage**
* Database: PostgreSQL via Prisma ORM
* Caching & Rate Limiting: Redis
* Authentication: JWT / OAuth2

### **AI Layer**
* Dynamic Provider Abstraction Layer
* Real-Time Server-Sent Events (SSE) Streaming
* Token Usage & Cost Tracking

---

## 🧠 CRTSE Engineering Prompts Library

Production-ready master prompts structured using the **CRTSE Framework**:
* **C** — Context (Project setup & scenario)
* **R** — Role (Expert specialization)
* **T** — Task (Exact operational goal)
* **S** — Standards (Quality guardrails & constraints)
* **E** — Example (Copy-pasteable execution prompt)

---

### Part 1: REST API Endpoint Generator

* **Context:** Building a scalable multi-tenant SaaS backend for Open'Ix AI with strict typing, zero-trust request validation, and standard error envelopes.
* **Role:** Lead Node.js/TypeScript Architect specializing in RESTful API design, defensive programming, and Express ecosystem security.
* **Task:** Generate a complete `POST /api/v1/users` endpoint split cleanly into route definition, controller, schema validation, and middleware layers.
* **Standards:**
  * Must use `Express`, `Zod`, `Prisma`, and `jsonwebtoken`.
  * Fully type-safe; zero usage of `any`.
  * Implements RFC 7807 problem details format for error responses (400, 409, 422, 500).
  * Enforces password complexity (min 12 chars, regex check) and strips sensitive hash fields.

```markdown
You are a Lead Node.js/TypeScript Backend Architect. Create a production-grade POST /api/v1/users endpoint for an enterprise SaaS backend.

Tech Stack: Express, TypeScript, Zod, Prisma ORM, jsonwebtoken.

Output Requirement:
Provide modular code across two clean files with full JSDoc:
1. `src/routes/users.ts` (Route definitions & Controller logic)
2. `src/middleware/auth.ts` (JWT Authentication & Role verification)

Security & Logic Requirements:
- Input Validation: Use Zod to validate body: `email` (valid email format), `password` (min 12 chars, 1 uppercase, 1 symbol, 1 number), `role` (enum: USER, ADMIN).
- Error Handling: Handle duplicate email with 409 Conflict, validation errors with 400 Bad Request (returning targeted field path errors), JWT auth failures with 401/403, and unhandled exceptions with 500 Internal Error.
- Output Security: Return 201 Created with a payload that strips sensitive field `passwordHash` and includes a generated JWT bearer token.
- No third-party dependencies outside express, zod, @prisma/client, and jsonwebtoken.# new-repo
OPEN’IX AI — COMPLETE MASTER DESIGN &amp; BUILD PROMPT  🎯 PROJECT IDENTITY  Brand Name: Open’Ix AI  Product: Open’Ix AI Intelligence Platform  Tagline: One Intelligence. Infinite Possibilities.  Product Type: AI Chatbot + Multi-Model AI Platform + Prompt Intelligence Workspace
