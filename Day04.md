# Day 04: Major Cloud Security Risks

*While the cloud offers immense scalability and operational benefits, it fundamentally changes the threat landscape. Understanding these risks is the first step. The next step is to secure your cloud the right way!*

To make these 12 risks easier to digest and tackle from an engineering perspective, they can be broken down into four core domains:

```mermaid
flowchart TD
    CR{12 Major Cloud Risks}
    
    CR --> IAM[ Identity & Keys]
    CR --> INFRA[ Infrastructure & Workloads]
    CR --> APP[ Data & Apps]
    CR --> OPS[ Operations & Resilience]

    IAM -.-> SC[Stolen Credentials]
    IAM -.-> EP[Excessive Permissions]
    IAM -.-> PKM[Poor Key Management]

    INFRA -.-> PS[Public Storage]
    INFRA -.-> NM[Network Misconfigs]
    INFRA -.-> US[Unpatched Systems]
    INFRA -.-> CKR[Container Risks]

    APP -.-> DB[Data Breaches]
    APP -.-> IA[Insecure APIs]
    APP -.-> IDT[Insecure Transfers]

    OPS -.-> LM[Lack of Monitoring]
    OPS -.-> DA[DDoS Attacks]

    classDef primary fill:#2b3137,stroke:#fafbfc,stroke-width:2px,color:#fff;
    classDef secondary fill:#fafbfc,stroke:#d1d5da,stroke-width:1px,color:#24292e;
    classDef tertiary fill:#ffffff,stroke:#e1e4e8,stroke-width:1px,color:#24292e;
    
    class CR primary;
    class IAM,INFRA,APP,OPS secondary;
    class SC,EP,PKM,PS,NM,US,CKR,DB,IA,IDT,LM,DA tertiary;

```

---

