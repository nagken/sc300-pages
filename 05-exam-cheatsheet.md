# SC-300 Exam Decision Reference

> Compressed decision table covering the entire exam. Use 1 day before the test.

| Scenario | Pick | Why |
|---|---|---|
| Hybrid sync (light) | Cloud Sync | Agent only |
| Hybrid sync (full) | Entra Connect | Multi-forest, write-back |
| On-prem MFA path | Federation or PTA + cloud MFA | PHS not on-prem MFA |
| Phishing-resistant MFA | Auth strength = phishing-resistant | WHfB / FIDO2 / cert |
| Block legacy auth | Single most impactful CA | Always do this |
| MI for Azure resource | System-assigned + RBAC | No secret |
| Daemon to MS Graph | Client credentials + cert | App-only token |
| SPA to MS Graph | Auth code + PKCE | No secret in browser |
| API calls downstream API | OBO flow | Token exchange |
| On-prem web app SSO | Application Proxy | No VPN |
| JIT admin | PIM eligible + activation | Reduce standing privilege |
| Self-service access | Entitlement mgmt package | + access reviews |
| JML automation | Lifecycle Workflows | HR-driven |

---

[Master Index](00-MASTER-INDEX.md)
