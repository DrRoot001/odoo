# Module: l10n_ph_sale

- **Module ID:** MOD-294
- **Path:** `addons/l10n_ph_sale`
- **Manifest:** `addons/l10n_ph_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Apply Philippine SC/PWD discount privileges on quotations and sale orders.

No manifest description declared.

Declared dependencies: `l10n_ph_invoice`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ph_invoice",
    "sale"
  ],
  "data": [
    "security/ir.access.csv",
    "views/sale_order_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ph_sale/__init__.py` (4 lines)
- `addons/l10n_ph_sale/__manifest__.py` (19 lines)
- `addons/l10n_ph_sale/i18n/l10n_ph_sale.pot` (138 lines)
- `addons/l10n_ph_sale/i18n/tl.po` (138 lines)
- `addons/l10n_ph_sale/models/__init__.py` (4 lines)
- `addons/l10n_ph_sale/models/sale_order.py` (30 lines)
- `addons/l10n_ph_sale/models/sale_order_line.py` (70 lines)
- `addons/l10n_ph_sale/security/ir.access.csv` (4 lines)
- `addons/l10n_ph_sale/tests/__init__.py` (3 lines)
- `addons/l10n_ph_sale/tests/test_discount_privilege_wizard.py` (509 lines)
- `addons/l10n_ph_sale/views/sale_order_views.xml` (35 lines)
- `addons/l10n_ph_sale/wizard/__init__.py` (4 lines)
- `addons/l10n_ph_sale/wizard/l10n_ph_discount_privilege_wizard.py` (73 lines)
- `addons/l10n_ph_sale/wizard/sale_order_discount.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
