# Entity Relationship Diagram

A complete static ERD for all possible Odoo addons would be misleading because the schema is generated from the installed module graph. The following runtime-level ERD shows verified platform relationships:

```mermaid
erDiagram
  MODULE_MANIFEST ||--o{ MODULE_DEPENDENCY : declares
  MODULE_MANIFEST ||--o{ ORM_MODEL : contributes
  ORM_MODEL ||--o{ ORM_FIELD : defines
  ORM_MODEL ||--o{ ACCESS_RULE : governs
  ORM_MODEL ||--o{ VIEW_OR_DATA_RECORD : loads
  ORM_MODEL }o--|| POSTGRESQL_TABLE : materializes_as
```

`MODULE_MANIFEST`, `ORM_MODEL`, and related nodes are documentation abstractions, not literal database tables. Use `Entity_Dictionary.csv` and a live registry inspection for a deployment-specific ERD.
