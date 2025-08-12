# WeedGO Platform 🌿

[![Platform Status](https://img.shields.io/badge/Status-Active%20Development-green)](https://github.com/WeedGo-Platform)
[![Services](https://img.shields.io/badge/Services-8%2F16%20Migrated-orange)](https://github.com/WeedGo-Platform)
[![Repositories](https://img.shields.io/badge/Repositories-27-blue)](https://github.com/WeedGo-Platform)

**Enterprise-grade cannabis delivery and dispensary management platform** built with microservices architecture, designed for scalability, compliance, and operational excellence.

## 🎯 Platform Overview

WeedGO is a comprehensive platform that powers cannabis businesses with:
- **Multi-tenant architecture** supporting dispensaries and delivery services
- **Real-time inventory management** with compliance tracking
- **Advanced analytics** and business intelligence
- **Mobile applications** for customers, drivers, and employees
- **Payment processing** with multiple gateway support
- **Automated compliance** reporting and audit trails

## 🏗️ Architecture

Our platform follows **Clean Architecture** principles with **Domain-Driven Design** patterns:

### Core Services
- 🔐 **[Identity Service](https://github.com/WeedGo-Platform/weedgo-identity-service)** - Authentication, authorization, and user management
- 💬 **[Communication Service](https://github.com/WeedGo-Platform/weedgo-communication-service)** - Messaging, notifications, and real-time communication
- 📊 **[Analytics Service](https://github.com/WeedGo-Platform/weedgo-analytics-service)** - Business intelligence and predictive analytics
- 🛍️ **[Product Catalog Service](https://github.com/WeedGo-Platform/weedgo-product-catalog-service)** - Product management and catalog operations
- 📦 **[Inventory Service](https://github.com/WeedGo-Platform/weedgo-inventory-service)** - Real-time stock tracking and warehouse management
- 💳 **[Payment Service](https://github.com/WeedGo-Platform/weedgo-payment-service)** - Secure payment processing and financial transactions

### Platform Components
- 🖥️ **[Admin Portal](https://github.com/WeedGo-Platform/weedgo-admin-portal)** - Management dashboard for operators
- 📈 **[Platform Dashboard](https://github.com/WeedGo-Platform/weedgo-platform-dashboard)** - Service monitoring and system health

### Mobile Applications
- 📱 **Driver Mobile App** - Delivery management and route optimization
- 📱 **Customer Mobile App** - Product browsing and order placement
- 📱 **Employee Mobile App** - Point-of-sale and internal operations

## 🚀 Migration Status

**Current Phase**: Service-Oriented Architecture Migration

| Category | Progress | Status |
|----------|----------|---------|
| **Backend Services** | 8/16 | 🟡 50% Complete |
| **Platform Components** | 2/4 | 🟡 50% Complete |
| **Mobile Applications** | 0/3 | 🔴 Pending |
| **Overall Progress** | 10/27 | 🟡 37% Complete |

### ✅ Completed Services
- [x] Identity & Access Management
- [x] Communication & Messaging
- [x] Analytics & Intelligence
- [x] Product Catalog Management
- [x] Inventory Management
- [x] Payment Processing
- [x] Admin Portal
- [x] Platform Dashboard

### 🔄 In Progress
- [ ] Order Management Service
- [ ] Customer Service
- [ ] Driver Management Service
- [ ] Store Operations Service
- [ ] Notification Service
- [ ] Compliance Service
- [ ] Reporting Service
- [ ] Integration Service

## 🛠️ Technology Stack

### Backend Services (.NET 8)
- **Framework**: ASP.NET Core 8
- **Architecture**: Clean Architecture + DDD
- **Database**: PostgreSQL 14+
- **Cache**: Redis 7
- **Message Queue**: RabbitMQ / Azure Service Bus
- **Search**: Elasticsearch
- **Analytics**: ClickHouse

### Frontend Applications (React 18)
- **Framework**: React 18 + TypeScript
- **UI Library**: Material-UI / Ant Design
- **State Management**: Redux Toolkit / Zustand
- **Build Tool**: Vite / Create React App

### Mobile Applications
- **Framework**: React Native + Expo
- **Navigation**: React Navigation
- **State**: Redux Toolkit + RTK Query
- **Push Notifications**: Expo Notifications

### Infrastructure & DevOps
- **Containers**: Docker + Docker Compose
- **CI/CD**: GitHub Actions
- **Cloud**: Azure / AWS (Multi-cloud ready)
- **Monitoring**: Application Insights / New Relic
- **Security**: Trivy vulnerability scanning

## 📋 Development Guidelines

### Code Standards
- **Clean Architecture** with clear separation of concerns
- **Domain-Driven Design** patterns and bounded contexts
- **SOLID principles** and dependency inversion
- **Comprehensive testing** with unit, integration, and E2E tests
- **Security-first** approach with OWASP compliance

### Branching Strategy
We follow **GitFlow** with environment-specific branches:

- `release` - **Production environment** - Stable, production-ready code
- `test` - **Staging/UAT environment** - Release candidates and final testing
- `dev` - **Development environment** - Integration branch for ongoing development
- `feature/*` - **Feature development** - Individual feature branches (merge to `dev`)
- `hotfix/*` - **Production hotfixes** - Critical fixes (merge to `release` and `dev`)
- `bugfix/*` - **Bug fixes** - Non-critical fixes (merge to `dev`)

#### Branch Flow
```
feature/user-auth → dev → test → release
                     ↑     ↑       ↑
                   merge  deploy  deploy
```

#### Environment Deployments
- **Development**: Auto-deploy from `dev` branch
- **Staging**: Auto-deploy from `test` branch  
- **Production**: **Manual approval required** from `release` branch

#### Production Deployment Security
🔒 **Manual Approval Process:**
- Must trigger via GitHub Actions "Run workflow"
- Requires explicit confirmation text: "DEPLOY"
- Environment protection rules enforced
- Full audit trail maintained

### Commit Conventions
```
feat: add new feature
fix: bug fix
docs: documentation updates
style: formatting changes
refactor: code refactoring
test: test additions
chore: maintenance tasks
```

## 🔒 Security & Compliance

- **RBAC** (Role-Based Access Control) with fine-grained permissions
- **JWT** authentication with refresh token rotation
- **PCI DSS** compliance for payment processing
- **Cannabis regulations** compliance tracking
- **Data encryption** at rest and in transit
- **Audit logging** for all critical operations
- **Vulnerability scanning** in CI/CD pipelines

## 📊 Monitoring & Observability

- **Real-time dashboards** for system health
- **Application Performance Monitoring** (APM)
- **Distributed tracing** across microservices
- **Custom metrics** and business KPIs
- **Alerting** for critical issues
- **Log aggregation** and analysis

## 🤝 Contributing

We follow strict development standards and security practices:

1. **Fork** the repository
2. **Create** a feature branch
3. **Implement** with comprehensive tests
4. **Ensure** all security scans pass
5. **Submit** a pull request

## 📞 Support

- **Technical Issues**: Create an issue in the relevant repository
- **Security Concerns**: Contact the security team privately
- **General Questions**: Use GitHub Discussions

## 📄 License

This project is proprietary software. All rights reserved.

---

<div align="center">

**🌿 Built with passion for the cannabis industry 🌿**

[Platform Dashboard](https://github.com/WeedGo-Platform/weedgo-platform-dashboard) | [Documentation](https://github.com/WeedGo-Platform) | [Migration Status](https://github.com/WeedGo-Platform/.github)

</div>