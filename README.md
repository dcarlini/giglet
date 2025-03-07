# 🚀 Giglet - Small Jobs Marketplace

Welcome to **Giglet** — a fully cloud-native, microservices-based marketplace for small jobs like babysitting, lawn mowing, and cleaning.

---

## 🌟 Overview
**Giglet** is designed as a **portfolio project**, showcasing:
- Mobile-first UI (React Native + Typescript)
- Polyglot microservices (Java + Node.js)
- Cloud-native deployment (Azure AKS + Terraform + Helm)
- End-to-end observability (OpenTelemetry + Prometheus + Grafana)
- Full test coverage (Unit, Integration, E2E)
- Automated CI/CD (GitHub Actions)
- Production-ready documentation (mkdocs)

---

## 🛠️ Tech Stack
| Layer | Tech Used |
|---|---|
| **Frontend (Mobile)** | React Native + Typescript + React Query |
| **Backend Microservices** | React - NestJS (GraphQL) + JavaSpring Boot (gRPC) + Express (REST) |
| **Data & Storage** | Supabase (PostgreSQL + Auth) + Redis (Caching) |
| **Infrastructure** | Docker Compose (local) + Kubernetes (MicroK8s/AKS) + Terraform |
| **CI/CD** | GitHub Actions (Click to Deploy) |
| **Observability** | OpenTelemetry + Prometheus + Grafana |


## 📥 Getting Started
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/dcarlini/giglet.git
cd giglet
```

### 2️⃣ Run Locally (Docker Compose)
```bash
docker-compose up
```

### 3️⃣ Run Mobile App
```bash
cd frontend-mobile
npm install
npm run ios   # for iOS
npm run android  # for Android
```

---

## ☁️ Deploying to Azure AKS
### Provision Infrastructure
```bash
cd terraform
tf apply
```

### Deploy to Kubernetes
```bash
kubectl apply -f k8s/
helm upgrade --install giglet ./helm/
```

---

## 🔗 Documentation
Giglet has a full **mkdocs documentation site**. To preview it locally:
```bash
pip install mkdocs-material
mkdocs serve
# Visit http://localhost:8000
```

---

## 📊 Observability
- Grafana: [http://localhost:3000](http://localhost:3000)
- Prometheus: [http://localhost:9090](http://localhost:9090)

---

## 🧪 Testing
| Test Type | Tool |
|---|---|
| Unit (Node) | Jest |
| Unit (Java) | JUnit 5 |
| Integration (Node) | Supertest |
| Integration (Java) | RestAssured |
| End-to-End | Cypress |

---
