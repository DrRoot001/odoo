# Security Architecture

The security model combines HTTP/session handling, authentication addons, ORM access rights, record rules, model constraints, and deployment configuration. Static evidence includes 279 access/security files and security-focused test modules.

```mermaid
flowchart LR
  REQ[Request] --> AUTH[Authentication/session]
  AUTH --> ACL[Model access rights]
  ACL --> RULE[Record rules / data domain]
  RULE --> ORM[ORM operation]
  ORM --> DB[(PostgreSQL)]
```
