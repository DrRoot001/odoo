# Business Rules

## Verified rule mechanisms

- Addon dependency declarations control module graph ordering (`__manifest__.py`, `odoo/modules/module_graph.py`).
- ORM constraints are implemented through model decorators and field definitions; static scan found 573 `constrains` usages.
- Computed/onchange dependencies are implemented through ORM decorators; static scan found 3,750 `depends` and 583 `onchange` usages.
- Access rights and record rules are declared in addon security files and enforced by the ORM/security layer.
- Localization, company, currency, tax, inventory, sales, accounting, HR, and other domain rules are distributed across addon inheritance chains.

Exact rule text is module/model specific and must be read from the cited model methods, XML rules, and tests. No business rule is inferred from a module name alone.
