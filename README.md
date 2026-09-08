# SYMBOLE GLOBAL / SIMBA PLATFORM

**A unified, enterprise-scale platform with clear domain separation, security controls, and progressive scaffolding.**

## 🎯 Mission

Transform the official SYMBOLE GLOBAL architecture into a real, structured, versionable, testable software project prepared for GitHub, Docker, Kubernetes, and CI/CD.

## 📋 Table of Contents

1. [Architecture Overview](#architecture-overview)
2. [Core Domains](#core-domains)
3. [Technical Centers](#technical-centers)
4. [Project Structure](#project-structure)
5. [Installation](#installation)
6. [Environment Variables](#environment-variables)
7. [Development](#development)
8. [Testing](#testing)
9. [Docker](#docker)
10. [Kubernetes](#kubernetes)
11. [CI/CD](#cicd)
12. [Security](#security)
13. [Deployment](#deployment)
14. [Contributing](#contributing)
15. [License](#license)

---

## 🏗️ Architecture Overview

SYMBOLE GLOBAL is organized as a **monorepo** with the following principal architecture:

```
SYMBOLE GLOBAL
├── 0. NOYAU GLOBAL SYMBOLE (Core)
├── 1. GLOBAL SOCIAL
├── 2. GLOBAL COMMERCIAL
├── 3. BUREAU DE LIVREUR (Delivery Bureau)
├── 4. JEUX GLOBAL (Global Games)
├── 5. FONDS GLOBAL (Global Funds)
└── 6. CENTRE D'ADMINISTRATEUR (Admin Center)
```

### Architectural Rules (Absolute)

- **Domain Separation**: Each domain is independent. No domain may bypass central controls.
- **Data Isolation**: No direct table access between domains. All exchange via API, Events, or Authorized Services.
- **Financial Authority**: GLOBAL FUNDS is the sole financial authority.
- **Identity Independence**: Download ≠ Registration ≠ Activation ≠ Authorization. Each domain has its own registration and activation state.
- **AI Control**: Domain AIs remain controlled. No IA may establish direct communication with another IA without system rules and permissions.

---

## 🎮 Core Domains

### 0. Noyau Global (Core)

The core layer provides:
- Identity & Global ID
- Accounts & Profiles
- Authentication & Authorization
- Security & Encryption
- API Gateway with full pipeline
- Notifications & Communication
- Media Management
- Search Infrastructure
- Localization & Timezone
- Resilience & Failover
- SDK & Client Libraries
- Telemetry, Logs & Audit
- Data Governance & Onboarding
- Visual Identity
- Application Management

**Location**: `backend/src/core/`

### 1. Global Social

Social networking platform.

**Modules**:
- Profile & Relationships
- Publications & Interactions
- Messaging & Communities
- Search & Discovery
- Notifications
- Social IA
- Moderation & Privacy
- Security & Data

**Location**: `backend/src/modules/global-social/`

**Events**: `PublicationCreated`, `ReactionCreated`, `MessageSent`, `RelationshipCreated`, `CommunityUpdated`

### 2. Global Commercial

E-commerce and marketplace.

**Modules**:
- Catalog & Products
- Merchants & Customers
- Carts & Orders
- Stock & Inventory
- Promotions & Reviews
- Search
- Commercial IA
- Security & Data

**Location**: `backend/src/modules/global-commercial/`

**Flow**:
```
Order → Payment Request → GLOBAL FUNDS → Verification → Authorization → Transaction → Ledger
```

**Delivery Integration**:
```
Order → Delivery Request → BUREAU DE LIVREUR
```

### 3. Bureau de Livreur (Delivery)

Logistics and delivery management.

**Modules**:
- Drivers & Profiles
- Availability & Missions
- Collection & Transport
- Delivery & Tracking
- Communication & Incidents
- Remuneration & Evaluation
- Delivery IA
- Security & Data

**Location**: `backend/src/modules/delivery/`

**Mission Lifecycle**:
```
CREATED → SEARCHING_DRIVER → ASSIGNED → ACCEPTED → COLLECTING →
COLLECTED → IN_TRANSIT → ARRIVING → DELIVERED → COMPLETED
```

### 4. Jeux Global (Games)

Gaming platform with enigma-based architecture.

**Specification**:
- **30 ENIGMA** × **40 distinct games** = **1,200 games**
- All ENIGMA belong to **MORTAL KOMBAT** branch

**Modules**:
- Players & Games
- Enigma Engine
- Modes & Matchmaking
- Sessions & Matches
- Tournaments & Scheduling
- Arbitration & Rankings
- Progression & Rewards
- Tokens & News
- Polls & Live
- Media Generation
- Communication
- Games IA
- Security & Data

**Location**: `backend/src/modules/games/`

**Capabilities**:
- 3D Worlds, Characters, Arenas
- Movements, Effects, Audio
- Cinematics & Dynamic Events
- Matchmaking & Progression
- Rankings & Rewards
- News & Polling
- Tournament Arbitration
- IA Player Architecture (MISTER DAME)

### 5. Fonds Global (Funds)

Financial authority and payment processing.

**Modules**:
- Accounts & Wallets
- Payment Methods & Virtual Accounts
- Transactions & Transfers
- Settlements & Refunds
- Fees & Reconciliation
- Ledger & Controls
- Anomaly Detection
- Guardian (Specialized Service)
- Token Sales
- Payment Gateway
- External Settlement
- Funds IA
- Security & Data

**Location**: `backend/src/modules/funds/`

**Token Sales**:
- Maximum 3 requests per day
- Scheduled slots: 09:00, 12:00, 16:00
- Quota validation → FONDS GLOBAL → Financial Gateway → Transaction → Ledger → Receipt

**Guardian Service**:
- Surveillance & Anomaly Detection
- Alerts & Reports
- Defensive Controls
- No critical financial decisions without system controls

### 6. Centre d'Administrateur (Admin)

Administration & Governance Center.

**Modules**:
- Dashboard & User Management
- Roles & Permissions
- Domain Administration (Social, Commercial, Delivery, Games, Funds)
- Security & Telemetry
- Audit & Configuration
- IA Admin
- Reports & Governance
- Responsible Officers Management
- Visual Identity
- Communication
- Security & Data

**Location**: `backend/src/modules/admin/`

**Human Governance** (5 binomes):
```
GLOBAL SOCIAL          → Director + Assistant
GLOBAL COMMERCIAL      → Director + Assistant
BUREAU DE LIVREUR      → Director + Assistant
JEUX GLOBAL            → Director + Assistant
FONDS GLOBAL           → Director + Assistant

Total: 10 Human Governors
```

---

## 🏢 Technical Centers

The platform supports specialized technical centers (BUILDs 53–87):

- **BUILD 53**: IAM Global
- **BUILD 54**: Document Platform
- **BUILD 55**: Communication Platform
- **BUILD 56**: Time & Scheduling
- **BUILD 57**: Global Workflow Engine
- **BUILD 58**: Global Service Center
- **BUILD 59**: Global Trust & Quality
- **BUILD 60**: Global Quality & Certification
- **BUILD 61**: Global Risk Center
- **BUILD 62**: Global Strategy & Performance
- **BUILD 63**: Global Project & Portfolio Center
- **BUILD 64**: Global Technology Asset Center
- **BUILD 65**: Global IT Service Center
- **BUILD 66**: Global Network Center
- **BUILD 67**: Cybersecurity Center
- **BUILD 68**: Global Cloud Center
- **BUILD 69**: Global Data Center
- **BUILD 70**: Global AI Center
- **BUILD 71**: Digital Trust
- **BUILD 72**: Global API Center
- **BUILD 73**: Global Device Center
- **BUILD 74**: Global POS Center
- **BUILD 75**: Global Supply Chain & Logistics Center
- **BUILD 76**: Global Facility Management Center
- **BUILD 77**: Global Mobility & Transport Center
- **BUILD 78**: Global Real Estate Center
- **BUILD 79**: Global Energy Center
- **BUILD 80**: Global Water Center
- **BUILD 81**: Global Environment Center
- **BUILD 82**: Global Agriculture & Agrifood Center
- **BUILD 83**: Global Industry & Manufacturing Center

---

## 📁 Project Structure

```
symbole-simba-platform/
│
├── backend/
│   ├── src/
│   │   ├── core/
│   │   │   ├── identity/
│   │   │   ├── accounts/
│   │   │   ├── authentication/
│   │   │   ├── authorization/
│   │   │   ├── security/
│   │   │   ├── api-gateway/
│   │   │   ├── communication/
│   │   │   ├── database/
│   │   │   ├── events/
│   │   │   ├── notifications/
│   │   │   ├── media/
│   │   │   ├── search/
│   │   │   ├── localization/
│   │   │   ├── telemetry/
│   │   │   ├── audit/
│   │   │   ├── ai/
│   │   │   └── index.ts
│   │   │
│   │   ├── modules/
│   │   │   ├── global-social/
│   │   │   ├── global-commercial/
│   │   │   ├── delivery/
│   │   │   ├── games/
│   │   │   ├── funds/
│   │   │   └── admin/
│   │   │
│   │   ├── services/
│   │   ├── workers/
│   │   ├── events/
│   │   ├── ai/
│   │   ├── main.ts
│   │   └── index.ts
│   │
│   ├── tests/
│   │   ├── unit/
│   │   ├── integration/
│   │   ├── api/
│   │   ├── security/
│   │   └── permissions/
│   │
│   ├── migrations/
│   ├── Dockerfile
│   ├── package.json
│   ├── tsconfig.json
│   ├── .env.example
│   └── jest.config.js
│
├── mobile/
│   ├── flutter/
│   └── README.md
│
├── web/
│   ├── src/
│   └── README.md
│
├── admin/
│   └── README.md
│
├── infrastructure/
│   ├── docker/
│   │   ├── backend.Dockerfile
│   │   ├── worker.Dockerfile
│   │   └── docker-compose.yml
│   └── kubernetes/
│       ├── namespace.yaml
│       ├── backend-deployment.yaml
│       ├── backend-service.yaml
│       ├── configmap.yaml
│       ├── secrets.yaml
│       ├── ingress.yaml
│       ├── workers-deployment.yaml
│       ├── autoscaling.yaml
│       └── health-checks.yaml
│
├── scripts/
│   ├── build.sh
│   ├── deploy.sh
│   ├── validate.sh
│   └── generate-zip.sh
│
├── docs/
│   ├── architecture/
│   │   ├── overview.md
│   │   ├── domains.md
│   │   ├── security.md
│   │   └── data-flow.md
│   ├── api/
│   │   ├── identity.md
│   │   ├── social.md
│   │   ├── commercial.md
│   │   ├── delivery.md
│   │   ├── games.md
│   │   ├── funds.md
│   │   └── admin.md
│   ├── security/
│   │   ├── authentication.md
│   │   ├── authorization.md
│   │   ├── encryption.md
│   │   └── incident-response.md
│   ├── deployment/
│   │   ├── installation.md
│   │   ├── docker.md
│   │   ├── kubernetes.md
│   │   └── troubleshooting.md
│   ├── database/
│   │   ├── schema.md
│   │   ├── migrations.md
│   │   └── indexing.md
│   ├── development/
│   │   ├── setup.md
│   │   ├── testing.md
│   │   └── debugging.md
│   ├── operations/
│   │   ├── monitoring.md
│   │   ├── logging.md
│   │   └── alerting.md
│   └── governance/
│       ├── admin-roles.md
│       └── audit.md
│
├── .github/
│   └── workflows/
│       ├── lint.yml
│       ├── test.yml
│       ├── security-scan.yml
│       ├── build.yml
│       ├── docker-build.yml
│       └── deploy.yml
│
├── .gitignore
├── .env.example
├── LICENSE
├── CONTRIBUTING.md
├── SECURITY.md
├── CHANGELOG.md
├── package.json
└── README.md (this file)
```

---

## 🚀 Installation

### Prerequisites

- **Node.js** 18+ (LTS recommended)
- **npm** or **yarn**
- **Docker** & **Docker Compose** (for containerized development)
- **PostgreSQL** 14+ (or configured database)
- **Redis** (for caching & sessions)

### Clone & Setup

```bash
# Clone the repository
git clone https://github.com/baraabdoulaziz/symbole-simba-platform.git
cd symbole-simba-platform

# Install dependencies
npm install

# Copy environment template
cp .env.example .env

# Run database migrations
npm run migrate

# Start development server
npm run dev
```

---

## 🔧 Environment Variables

Create a `.env` file based on `.env.example`:

```env
# Application
NODE_ENV=development
APP_NAME=symbole-simba-platform
APP_VERSION=0.1.0

# Server
PORT=3000
HOST=localhost

# Database
DB_HOST=localhost
DB_PORT=5432
DB_NAME=symbole_dev
DB_USER=postgres
DB_PASSWORD=postgres

# Redis
REDIS_HOST=localhost
REDIS_PORT=6379

# Authentication
JWT_SECRET=your-secret-key-here
JWT_EXPIRY=24h

# Security
CORS_ORIGIN=http://localhost:3000
SESSION_SECRET=your-session-secret

# External Services
PAYMENT_GATEWAY_URL=https://sandbox.payment-provider.com
PAYMENT_API_KEY=

# Storage
STORAGE_BUCKET=symbole-bucket
STORAGE_REGION=us-east-1

# Logging & Telemetry
LOG_LEVEL=info
TELEMETRY_ENABLED=true

# Sensitive: Never commit actual values
# These should be supplied by deployment environment
```

**⚠️ NEVER commit actual secrets to Git. Use `.env.example` as template.**

---

## 👨‍💻 Development

### Local Development

```bash
# Start with nodemon (auto-restart on changes)
npm run dev

# Run linter
npm run lint

# Fix linting issues
npm run lint:fix

# Type checking
npm run typecheck

# Build
npm run build
```

### Project Structure in Backend

Each module follows this pattern:

```
module/
├── api/              # Route handlers
├── services/         # Business logic
├── models/           # Data models
├── events/           # Event definitions
├── middleware/       # Module-specific middleware
├── types/            # TypeScript types
├── errors/           # Error handling
├── constants/        # Constants
├── ai/               # Module-specific AI logic
├── __tests__/        # Module tests
└── index.ts          # Module exports
```

---

## 🧪 Testing

### Run Tests

```bash
# Unit tests
npm run test:unit

# Integration tests
npm run test:integration

# API tests
npm run test:api

# Security tests
npm run test:security

# Permission tests
npm run test:permissions

# All tests
npm run test

# Coverage report
npm run test:coverage
```

### Test Strategy

- **Unit Tests**: Service & utility functions
- **Integration Tests**: Cross-module interactions
- **API Tests**: Endpoint validation
- **Security Tests**: Authentication, authorization, encryption
- **Permission Tests**: Role-based access control
- **Workflow Tests**: Complex business processes
- **Data Tests**: Migrations, integrity, validation
- **Regression Tests**: Critical features

**⚠️ Financial operations use sandbox/mock until real provider configured.**

---

## 🐳 Docker

### Build Docker Image

```bash
cd backend
docker build -t symbole-backend:latest .
```

### Run with Docker Compose

```bash
docker-compose up -d
```

### Dockerfile Structure

```dockerfile
# Multi-stage build
FROM node:18-alpine AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY --from=builder /app/dist ./dist
EXPOSE 3000
CMD ["node", "dist/main.js"]
```

---

## ☸️ Kubernetes

### Deploy to Kubernetes

```bash
# Create namespace
kubectl apply -f infrastructure/kubernetes/namespace.yaml

# Deploy backend
kubectl apply -f infrastructure/kubernetes/

# Check status
kubectl get pods -n symbole-platform

# View logs
kubectl logs -f deployment/backend -n symbole-platform

# Port forward (local testing)
kubectl port-forward svc/backend 3000:3000 -n symbole-platform
```

### Kubernetes Manifests

- **Namespace**: Isolate resources
- **Deployment**: Backend pods with replicas
- **Service**: Internal & external access
- **ConfigMap**: Non-secret configuration
- **Secret**: Secrets (injected from environment)
- **Ingress**: Public HTTP/HTTPS routing
- **HPA**: Auto-scaling based on metrics
- **Health Checks**: Readiness & liveness probes

---

## 🔄 CI/CD

### GitHub Actions Workflow

Located in `.github/workflows/`:

```yaml
1. Checkout
2. Install dependencies
3. Lint
4. Type check
5. Test
6. Security scan
7. Build
8. Docker build
9. Docker test
10. Publish
11. Deploy
12. Health check
```

### Trigger Events

- **Push** to `main` / `master`: Auto-deploy
- **Pull Request**: Run tests & lint
- **Schedule**: Nightly security scans

### Buildkite Alternative

Alternative CI/CD via Buildkite for complex pipelines.

---

## 🔐 Security

### Implementation Checklist

- ✅ Input validation
- ✅ Authentication (JWT, Sessions)
- ✅ Authorization (RBAC)
- ✅ Session management
- ✅ Secret protection
- ✅ Rate limiting
- ✅ CORS configuration
- ✅ Security headers
- ✅ Error handling (no leaks)
- ✅ Audit logging
- ✅ Access controls
- ✅ Environment separation

### Secrets Management

**NEVER commit**:
- Passwords
- API tokens
- Private keys
- Certificates
- Cloud credentials
- Financial secrets

**Use**:
- Environment variables
- Secret managers (Vault, AWS Secrets Manager)
- `.env` (local only, .gitignored)
- Deployment provider secrets

### Authentication

- **Global ID**: Unique identifier across platform
- **JWT**: Stateless authentication
- **Sessions**: Stateful authentication option
- **MFA**: Multi-factor authentication support

### Authorization

Model: `User + Role + Permission + Domain + Resource + Action + Context`

- All permission checks on server
- UI is NOT a security boundary
- Domain-specific authorization

---

## 📊 Observability

### Logging

```bash
npm run logs      # View application logs
npm run logs:tail # Follow logs in real-time
```

Structured logging with context:
- User ID
- Request ID
- Domain
- Action
- Timestamp
- Level (info, warn, error)

### Metrics

- Request rate
- Response time
- Error rate
- Database performance
- Cache hit ratio
- Queue depth

### Traces

- Distributed tracing
- Cross-domain calls
- Performance profiling

### Health Checks

```bash
GET /health          # Basic health
GET /health/ready    # Readiness probe (K8s)
GET /health/live     # Liveness probe (K8s)
```

---

## 🚀 Deployment

### Production Checklist

- [ ] All tests passing
- [ ] Security scan passing
- [ ] Database migrations verified
- [ ] Environment variables configured
- [ ] Secrets in secure store
- [ ] Monitoring enabled
- [ ] Alerts configured
- [ ] Rollback plan ready
- [ ] Documentation updated
- [ ] Changelog updated

### Deployment Flow

```
Git Push
  ↓
CI/CD Pipeline
  ↓
Tests & Security Scan
  ↓
Docker Build & Push
  ↓
Kubernetes Apply
  ↓
Health Checks
  ↓
Monitor & Alert
```

### Rolling Deployments

- Zero-downtime updates
- Gradual pod replacement
- Automatic rollback on failure

---

## 📝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for:
- Development guidelines
- Code style
- Commit conventions
- Pull request process
- Domain-specific rules
- Testing requirements

---

## 🛡️ Security Policy

See [SECURITY.md](SECURITY.md) for:
- Vulnerability reporting
- Security best practices
- Incident response
- Third-party dependencies
- Compliance

---

## 📄 License

[Specify license - MIT, Apache 2.0, etc.]

---

## 📞 Support

- **Issues**: GitHub Issues
- **Discussions**: GitHub Discussions
- **Docs**: `/docs` directory
- **Email**: support@symbole-global.com

---

## 🗂️ Additional Documentation

- [Architecture Overview](docs/architecture/overview.md)
- [API Documentation](docs/api/)
- [Security Guide](docs/security/)
- [Deployment Guide](docs/deployment/)
- [Database Schema](docs/database/)
- [Development Setup](docs/development/)
- [Operations Guide](docs/operations/)
- [Governance & Admin](docs/governance/)

---

**Last Updated**: 2026-09-08  
**Version**: 0.1.0-alpha  
**Status**: In Development

---

*This README reflects the Master Architecture Document for SYMBOLE GLOBAL / SIMBA PLATFORM. For detailed architecture specifications, see the official architecture document.*
