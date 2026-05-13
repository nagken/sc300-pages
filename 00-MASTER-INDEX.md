# SC-300 - Microsoft Identity and Access Administrator - Visual Study Guide

> Concept-only study aid. No exam questions reproduced. Source PDF (if any) stays local + gitignored.

**Skills outline:** https://learn.microsoft.com/en-us/credentials/certifications/exams/sc-300/

## Master mind map

```mermaid
mindmap
  root((SC-300))
    Implement Identities in Microsoft Entra
      Configure and manage a Microsoft Entra tenant custom domains, brand...
      Create, configure, and manage Entra users, groups, devices, and adm...
      Implement and manage external identities B2B collaboration, Externa...
      Implement and manage hybrid identity Entra Connect, Cloud Sync, PHS...
    Implement Authentication and Access Management
      Plan and implement Conditional Access policies
      Plan and implement Entra MFA and passwordless Authenticator passkey...
      Configure and manage authentication strengths e.g. require phishing...
      Manage Identity Protection sign-in risk, user risk policies, risky ...
      Implement Continuous Access Evaluation CAE
    Plan and Implement Workload Identities
      Plan, implement, and manage app registrations single-tenant, multi-...
      Manage service principals, managed identities system + user-assigned
      Implement OAuth 2.0 flows auth code + PKCE, client credentials, OBO
      Manage application proxy for on-prem apps
      Manage Workload ID Conditional Access P2
    Plan and Implement Identity Governance
      Plan and implement entitlement management catalogs, access packages...
      Plan and implement access reviews
      Plan and implement Privileged Identity Management PIM for Entra and...
      Monitor and maintain Entra ID audit, sign-in logs, workbooks, Entra...
      Plan and implement Lifecycle Workflows joiner/mover/leaver
```

## Domain map

```mermaid
flowchart LR
    Master["SC-300 Master Index"]
    D01["Implement Identities in Microsoft Entra"]
    Master --> D01
    D02["Implement Authentication and Access Management"]
    Master --> D02
    D03["Plan and Implement Workload Identities"]
    Master --> D03
    D04["Plan and Implement Identity Governance"]
    Master --> D04
```

## Domain weights

```mermaid
pie showData
    title SC-300 domain weights
    "Implement Identities in Microsoft Entra" : 23
    "Implement Authentication and Access Management" : 27
    "Plan and Implement Workload Identities" : 25
    "Plan and Implement Identity Governance" : 25
```

> Click a slice / legend label to jump to that chapter.

## Recommended study order

```mermaid
gantt
    title Suggested study plan
    dateFormat X
    axisFormat Day %d
    section Plan
    Implement Identities in Microsoft Entra :t1, 0, 2d
    Implement Authentication and Access Management :t2, after t1, 2d
    Plan and Implement Workload Identities :t3, after t2, 2d
    Plan and Implement Identity Governance :t4, after t3, 2d
```

---

**Next:** open [01-entra-identities.md](01-entra-identities.md)

<!-- TODO: fill remaining sections via Copilot chat. Target structure mirrors c:\az305\study-guide\00-MASTER-INDEX.md. -->
