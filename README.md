## Hands-On Projects Worthy of Recruiter Review

### Food Safety and Inspection Service (FSIS) Eligibility Control Tower  
Cloud-native control tower that monitors FSIS establishment eligibility data, detects status changes, computes downstream operational impact, and provides role-based alerts and dashboards for compliance-aware operations.

---

### 1. What This Project Shows

**Problem:**  
Food Safety and Inspection Service (FSIS) is a public health agency within the USDA. 

FSIS is responsible for ensuring that meat, poultry, and egg products are safe, wholesome, and correctly labeled. FSIS maintains inspection and eligibility records that determine which establishments are authorized to process products for domestic and export markets.

Meat export and cold-chain operations lack near-real-time visibility into "FSIS establishment" (ie meat producing farms) eligibility changes, creating downstream compliance risk across inventory, facilities, and shipments.

**Solution:**  
Built an event-driven cloud control tower that ingests FSIS eligibility data, detects eligibility drift, computes operational blast radius, enforces control gates, and surfaces shared situational awareness across teams.

**Impact:**  
Improves compliance awareness for all decision-makers across the supply chain, prevents invalid downstream actions, and enables faster, coordinated responses across quality, operations, and management roles.

---

### 3. Architecture

High-level architecture showing:

- Scheduled ingestion of FSIS eligibility data  
- Snapshot-based change detection  
- Event-driven impact analysis  
- Enforcement of operational control gates  
- Role-based visibility through dashboards and alerts  
- Audit logging and observability  

*(Replace with your architecture diagram in `docs/architecture.png`.)*

---

### 4. Screenshots (Proof of Work)

Add 2–3 screenshots after a single deployment.

**a. AWS Console**  
Example: Serverless services and data stores provisioned  
*(Screenshot placeholder)*

**b. Dashboard View**  
Example: Eligibility changes, impacted entities, and open compliance events  
*(Screenshot placeholder)*

**c. Data or Event View**  
Example: Eligibility change detected and downstream impact recorded  
*(Screenshot placeholder)*

---

### 5. Tech Used

- **AWS Services:** Serverless compute, managed NoSQL storage, event routing, notifications  
- **Infrastructure as Code:** Terraform  
- **Automation:** Ansible (demo and environment resets)  
- **Observability:** Prometheus, Loki, Grafana (self-hosted for demos)  
- **Language:** Python  

---

### 6. Cost Note

This project is designed to be deployed on-demand and destroyed after validation to minimize cloud costs. No always-on infrastructure is required.

Security: [Security Policy](SECURITY.md) • [Security Checklist](docs/security-checklist.md)

---

### 7. Repo Structure

```
fsis-eligibility-control-tower/
├── README.md
├── docs/
│   ├── architecture.md
│   ├── roadmap.md
│   └── screenshots/
├── infra/
│   ├── terraform/
│   └── ansible/
├── services/
│   ├── ingestor/
│   ├── impact-analyzer/
│   ├── notifier/
│   └── api/
└── schemas/
    ├── events/
    └── models/
```

---
### About Me

Created by Techric — a Cloud & DevSecOps Engineer dedicated to building secure, automated, and observable systems on AWS and Linux. Each project reflects my goal of turning technical exploration into clear, reproducible knowledge others can build upon.

This repository documents real-world projects from my home lab and professional experience, showcasing practical problem-solving, infrastructure mastery, and a commitment to continuous learning.
   
   Apply complete! Resources: 12 added, 0 changed, 0 destroyed.
