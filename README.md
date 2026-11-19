# Zero-Trust DevSecOps Pipeline



A CI/CD pipeline built around Zero-Trust security principles — combining policy-as-code enforcement, container security scanning, and automated vulnerability checks into the software delivery process.







## Overview



This project implements a DevSecOps pipeline that enforces security controls at every stage of the CI/CD process rather than treating security as an afterthought. Key components include:



- **Policy-as-code** — OPA (Open Policy Agent) rules that gate deployments based on defined security policies

- **Container security scanning** — automated vulnerability checks on container images before deployment

- **Infrastructure as Code** — Terraform-managed infrastructure with security guardrails baked in

- **CI automation** — GitHub Actions workflows that run security checks, tests, and audits on every change



## Tech Stack



- **CI/CD:** GitHub Actions

- **Policy Enforcement:** Open Policy Agent (OPA)

- **IaC:** Terraform (HCL)

- **Languages:** Go, Python

- **Security:** Semgrep (SAST), container/dependency scanning



## Repository Structure



```

.github/workflows/   → CI pipeline definitions

app/                 → Application code

build/               → Build scripts and configuration

docs/architecture/   → Architecture documentation

infra/               → Infrastructure as Code (Terraform)

policy/              → OPA policy-as-code rules

scripts/             → Automation/utility scripts

security/            → Security scanning configuration

tests/audit/         → Audit and compliance tests

```




