# Architectures - SC-300

> Reference architectures you should be able to draw on a whiteboard for the exam.

## Hybrid identity end-to-end

```mermaid
flowchart LR
    AD[On-prem AD DS] --> Conn[Entra Connect or Cloud Sync]
    Conn --> Entra[Entra ID]
    Entra --> CA{Conditional Access}
    Entra --> PIM[PIM]
    Entra --> EM[Entitlement Mgmt]
    Entra --> APP[Cloud + on-prem apps via App Proxy]
```

## Workload identity flows

```mermaid
flowchart TD
    SPA[Single-page app] -->|auth code+PKCE| Graph[Microsoft Graph]
    Daemon[Daemon] -->|client_credentials+cert| Graph
    API[API] -->|OBO| DownstreamAPI[Downstream API]
    VM[Azure VM] -->|managed identity| KV[Key Vault]
```


---

[Master Index](00-MASTER-INDEX.md)
