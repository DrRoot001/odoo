# Module: l10n_br_sales

- **Module ID:** MOD-140
- **Path:** `addons/l10n_br_sales`
- **Manifest:** `addons/l10n_br_sales/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Sale modifications for Brazil

Declared dependencies: `l10n_br`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_br",
    "sale"
  ],
  "data": [
    "views/sale_portal_templates.xml",
    "report/sale_order_templates.xml",
    "report/report_invoice_templates.xml"
  ]
}
```

### Representative source files

- `addons/l10n_br_sales/__init__.py` (3 lines)
- `addons/l10n_br_sales/__manifest__.py` (18 lines)
- `addons/l10n_br_sales/i18n/l10n_br_sales.pot` (41 lines)
- `addons/l10n_br_sales/i18n/pt_BR.po` (46 lines)
- `addons/l10n_br_sales/models/__init__.py` (3 lines)
- `addons/l10n_br_sales/models/sale_order.py` (15 lines)
- `addons/l10n_br_sales/report/report_invoice_templates.xml` (6 lines)
- `addons/l10n_br_sales/report/sale_order_templates.xml` (23 lines)
- `addons/l10n_br_sales/views/sale_portal_templates.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
