
# Day 06: Important Cloud Security Tools

*These native tools form the core AWS ecosystem, working together to help engineers **protect**, **detect**, and **respond** to threats while automating compliance.*

When moving from a traditional network operations view to an automated, scalable infrastructure model, these are the primary services used to enforce policies as code and gain deep visibility into your environments.

---

### The AWS Security Ecosystem

```mermaid
flowchart TD
    Main{AWS Security Ecosystem}
    
    Main --> Protect[ Protect]
    Main --> Detect[ Detect]
    Main --> Respond[ Respond & Govern]

    Protect -.-> IAM[IAM: Access Control]
    Protect -.-> WAF[WAF & Shield: Edge Protection]
    
    Detect -.-> GD[GuardDuty: Threat Detection]
    Detect -.-> Insp[Inspector: Vulnerability Scanning]
    Detect -.-> CW[CloudWatch: Logging & Metrics]
    
    Respond -.-> SH[Security Hub: Centralized Alerts]
    Respond -.-> CT[CloudTrail: API Auditing]
    Respond -.-> Conf[AWS Config: Resource Tracking]

    classDef primary fill:#2b3137,stroke:#fafbfc,stroke-width:2px,color:#fff;
    classDef secondary fill:#fafbfc,stroke:#d1d5da,stroke-width:1px,color:#24292e;
    
    class Main primary;
    class Protect,Detect,Respond,IAM,WAF,GD,Insp,CW,SH,CT,Conf secondary;

```

---



###  1. Identity & Network Protection

* **IAM (Identity & Access Management):** Manages user identities, roles, and permissions. Enforcing least privilege access ensures that automated Bash scripts, Python runbooks, or CI/CD workflows only have the exact access required and nothing more.
* **WAF & Shield:** Protects internet-facing web applications from common exploits and scrapers. Shield specifically defends against Distributed Denial of Service (DDoS) threats, ensuring high availability and uptime.


