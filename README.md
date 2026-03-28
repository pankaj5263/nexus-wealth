# 🏛️ Nexus Wealth Intelligence
**Autonomous Multi-Agent Financial Operating System**

Nexus is a stateful, agentic platform designed to provide real-time financial analysis. Built with a "human-in-the-loop" philosophy, it scales to 100,000+ users using an asynchronous, event-driven architecture.

---

## 🚀 Tech Stack
- **Frontend:** React 19, Vite, [HeroUI v3](https://heroui.com/), Tailwind CSS v4
- **Backend:** Node.js v22 (Fastify), TypeScript, Socket.io (Real-time)
- **AI Orchestration:** LangGraph.js (Stateful Graphs)
- **Inference:** Groq LPU (Llama 3.3 / 3.1) - <500ms latency
- **Data & Memory:** PostgreSQL (pgvector), Redis (Queue & Checkpointing)
- **Infrastructure:** Docker, pnpm Workspaces

---

## 📂 Project Structure
```text
.
├── apps
│   ├── web          # React Dashboard (HeroUI + Generative UI)
│   └── server       # Node.js API & WebSocket Gateway (Fastify)
├── packages
│   ├── agents       # LangGraph Workflows (The "Brain")
│   ├── tools        # LLM Tool Definitions (The "Hands")
│   └── shared       # Common Types & Interfaces (The "Contracts")
├── docker-compose.yml
└── pnpm-workspace.yaml
