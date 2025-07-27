BugInsight is a smart, scalable issue & error tracking platform built with NestJS Microservices, designed for developers and teams to efficiently manage bugs, logs, and notifications in real-time.

✨ Features
🔐 Authentication (JWT + Refresh Token, Redis session)
🐛 Issue Management (Create, track, update status)
📁 Project Management (Multi-project support)
📬 Notification System (Email, Discord, Slack via queue)
⚡ Event-Driven Microservices using Redis Pub/Sub
📊 Pluggable AI Analyzer (predict recurring bugs & log patterns)
🧱 Modular Monorepo architecture
🐳 Dockerized for easy deployment

🏗️ Tech Stack
NestJS (Microservices mode)
Redis (Queue + Event communication)
PostgreSQL (Per-service DB)
Prisma ORM
BullMQ (Job Queue)
Docker & Docker Compose
(Optional) gRPC & WebSocket Gateway

📁 Project Structure (Monorepo)
buginsight/
├── apps/
│   ├── api-gateway/
│   ├── auth-service/
│   ├── issue-service/
│   ├── notification-service/
├── libs/
│   ├── dto/
│   ├── common/
│   ├── logger/
├── prisma/
├── .env
└── docker-compose.yml

🚀 Getting Started
# Clone this repo
git clone https://github.com/ariefprasetyo939/nestjs-buginsight.git
cd buginsight

# Install dependencies
npm install

# Start services (local dev)
npm run start:dev auth-service
npm run start:dev issue-service
npm run start:dev api-gateway
Requires PostgreSQL & Redis running locally

📦 Deployment
Use Docker Compose (coming soon)
Compatible with Kubernetes, Fly.io, or Render

🧪 Status
🟡 In development — currently working on:

 Monorepo setup
Auth Service (register, login, JWT)
Issue Service (CRUD + events)
Notification Service (event listener + email)
Docker & CI/CD setup

🙌 Contribution
Feel free to fork, improve, and contribute via PRs. BugInsight is made for learning and building real-world backend architecture.
