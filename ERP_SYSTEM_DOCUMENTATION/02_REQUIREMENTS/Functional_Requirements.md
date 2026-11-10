# Functional Requirements

The repository is a framework-plus-addon system, so functional requirements are grouped by implementation surface:

1. **Bootstrap and CLI:** command dispatch, configuration parsing, database/server lifecycle.
2. **Module lifecycle:** manifest parsing, dependency graph resolution, installation/update/uninstallation hooks, migrations.
3. **ORM and data:** model declarations, fields, computed fields, constraints, onchange behavior, access rules, transactions, cache, and registry.
4. **HTTP and client:** route registration, dispatch, sessions, JSON/HTTP responses, web assets, XML templates, browser modules.
5. **Business addons:** each manifest-backed addon is a separately traceable functional unit; see the module catalog and per-addon pages.
6. **Cross-cutting services:** mail, bus, scheduled actions, reporting, translations, attachments, authentication, and integrations where their addons are installed.

Detailed source-backed behavior is intentionally not generalized across addons because Odoo uses inheritance and configuration-dependent extension points. The per-addon artifact pages and machine inventory are the authoritative traceability anchors.
