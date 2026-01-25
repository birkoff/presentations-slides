# CI/CD
 **Continuous Integration** / **Continuous Delivery/Deployment**... 
 
....What's the point of it? 
 


Its primary goal is to streamline and accelerate the software development lifecycle (SDLC) through automation.

---

### Continuous Integration (CI)

The practice of **automatically** and frequently integrating code changes into a shared source code repository....

...How does it helps?


This helps identify bugs early by running automated builds and tests every time a developer commits code.

---

## Continuous Delivery/Deployment (CD)

A two-part process focused on the testing and release of code

---

### Continuous Delivery

Ensures code is always in a deployable state !!

> It automates the integration and testing phases but requires a **manual trigger** to push the code into production.

---

#### Continuous Deployment

Takes automation a step further by **automatically releasing** every change that passes the testing pipeline directly into the production environment without human intervention.

---

### The CI/CD Pipeline

Taken together, these connected practices form what is known as a **"CI/CD pipeline."** This workflow is supported by development and operations teams working together in an **Agile** framework, typically utilizing one of two cultural approaches:

1. **DevOps:** Focusing on collaboration between development and operations to shorten the development life cycle.
2. **Site Reliability Engineering (SRE):** Using software engineering signals and automation to create scalable and highly reliable software systems.

> **Key takeaway:** While CI focuses on the "build and test" phase, CD focuses on the "release and deploy" phase.

---

### API Main Workflows

- Dev Integration Pipeline (PR) => Dev
- Release Integration Pipeline (Main) => Staging
- Release Deployment Pipeline (Tag) => Production



#### API Workflows Pipelines
- Unit Tests

- Deploy to Dev
- Verify API Deployment Dev
- Run E2E Tests Dev

- Deploy to Staging
- Verify API Deployment Staging
- Run E2E Tests Staging

- Notify
---

### Platform Workflows Pipelines
- Terraform Infra Pipeline
- API Mappings Pipeline
- Alembic DB Migrations Pipeline
- Create Release Tag Pipeline
- Run E2E Tests Pipeline
- Remove Ticket Dev Environments Pipeline
