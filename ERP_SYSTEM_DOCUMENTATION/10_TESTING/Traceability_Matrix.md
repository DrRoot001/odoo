# Traceability Matrix

| Requirement | Module/system surface | Source evidence | Test case |
|---|---|---|---|
| FR-001 | CLI/server | `odoo-bin`, `odoo/cli/`, `odoo/service/` | TC-001 |
| FR-002 | Module lifecycle | `odoo/modules/` and manifests | TC-002 |
| FR-003 | ORM/database | `odoo/orm/`, `odoo/sql_db.py` | TC-003 |
| FR-004 | HTTP/API | `odoo/http/`, Route_Inventory.csv | TC-004 |
| FR-005 | Security | addon security artifacts, ORM security | TC-005 |
| FR-007 | UI/assets | XML and JS/TS inventories | TC-006 |
| FR-008 | Testing | addon tests | TC-007 |

Addon-specific traceability is one-to-one from `Module_Catalog.md` to each `addons/<module>.md`; runtime-level UI/API/database/test links remain deployment-specific where static source cannot prove them.
