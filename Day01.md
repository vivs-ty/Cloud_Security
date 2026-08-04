# Day 01

### What is Cloud Security?

Cloud Security is the practice of protecting data, applications, and infrastructure in the cloud from threats and unauthorized access.

**The Five Pillars of Protection:**

1. **Cloud Applications:** Securing the software itself (often where tools like GitHub Actions and automated CI/CD security checks come in).
2. **Data:** Encryption at rest and in transit.
3. **Servers & Workloads:** Securing compute resources, from traditional VMs to Kubernetes clusters.
4. **Networks:** Virtual Private Clouds (VPCs), firewalls, and managing traffic flow.
5. **User Access:** Identity and Access Management (IAM), ensuring only the right people and automated scripts have permissions.

```mermaid
flowchart TD
    CS{It Protects} 
    
    CS --> CA[Cloud Applications]
    CS --> D[Data]
    CS --> SW[Servers & Workloads]
    CS --> N[Networks]
    CS --> UA[User Access]
    
    %% Optional: Sub-points for context
    CA -.-> CA_Sub[e.g., GitHub Actions CI/CD pipelines]
    D -.-> D_Sub[e.g., Database encryption]
    SW -.-> SW_Sub[e.g., Kubernetes clusters & Ansible nodes]
    N -.-> N_Sub[e.g., VPCs & firewalls]
    UA -.-> UA_Sub[e.g., IAM roles & Bash script permissions]

    classDef primary fill:#2b3137,stroke:#fafbfc,stroke-width:2px,color:#fff;
    classDef secondary fill:#fafbfc,stroke:#d1d5da,stroke-width:1px,color:#24292e;
    
    class CS primary;
    class CA,D,SW,N,UA secondary;
```
