# Multi-Environment CI/CD Deployment with GitHub Actions & AWS EC2

This project demonstrates a complete multi-environment CI/CD pipeline using:

- GitHub Actions
- AWS EC2
- Nginx Virtual Hosts
- GitHub Environments
- SSH-based deployment

The same application is automatically deployed to different environments based on the Git branch.

---

# Architecture

```text
GitHub Repository
├── dev branch      → Development Environment
├── staging branch  → Staging Environment
└── main branch     → Production Environment

GitHub Actions
        ↓
SSH/SCP Deployment
        ↓
AWS EC2 Instance
        ↓
Nginx Virtual Hosts
        ↓
Multiple Environments on a Single Server