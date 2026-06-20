# SaaS vs PaaS vs IaaS

### Simple Analogy

- **SaaS:** Use the car.
- **PaaS:** Drive the car.
- **IaaS:** Build and maintain the car.

---

## SaaS (Software as a Service)

You only use the application.

Examples:
- Microsoft 365
- Gmail
- Salesforce

Provider manages:
- Infrastructure
- Platform
- Application
- Updates

You manage:
- Users
- Configuration

**Key Idea:** Just use the software.

---

## PaaS (Platform as a Service)

You build and deploy applications.

Examples:
- Azure App Service
- OpenShift
- Google App Engine

Provider manages:
- Infrastructure
- Operating System
- Runtime
- Platform services

You manage:
- Code
- Containers
- Deployments

**Key Idea:** Focus on the application, not the infrastructure.

---

## IaaS (Infrastructure as a Service)

You manage servers and operating systems.

Examples:
- Azure Virtual Machines
- AWS EC2
- Google Compute Engine

Provider manages:
- Physical hardware
- Datacenter
- Virtualization

You manage:
- Operating System
- Applications
- Security configuration
- Middleware

**Key Idea:** More control, more responsibility.

---

# Responsibility Summary

| Role | SaaS | PaaS | IaaS |
|--------|--------|--------|--------|
| Business User | Use software | N/A | N/A |
| Developer | Integrations | Code & deployments | Applications |
| DevOps Engineer | Integrations | CI/CD & automation | CI/CD & infrastructure automation |
| Platform Engineer | N/A | Platform management | N/A |
| Cloud Engineer | N/A | Cloud foundation | Infrastructure management |

---

# Quick Comparison

| Layer | SaaS | PaaS | IaaS |
|----------|----------|----------|----------|
| Application | Provider | Customer | Customer |
| Runtime | Provider | Provider | Customer |
| Operating System | Provider | Provider | Customer |
| Virtualization | Provider | Provider | Provider |
| Servers | Provider | Provider | Provider |
| Storage | Provider | Provider | Provider |
| Networking | Provider | Provider | Provider |
| Customer Control | Low | Medium | High |
| Operational Effort | Low | Medium | High |