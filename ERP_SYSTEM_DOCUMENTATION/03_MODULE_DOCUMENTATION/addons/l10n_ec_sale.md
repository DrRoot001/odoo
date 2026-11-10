# Module: l10n_ec_sale

- **Module ID:** MOD-169
- **Path:** `addons/l10n_ec_sale`
- **Manifest:** `addons/l10n_ec_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Ecuador Sale

Declared dependencies: `l10n_ec`, `sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ec",
    "sale"
  ],
  "data": [
    "views/payment_method_views.xml",
    "views/sale_order_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ec_sale/__init__.py` (4 lines)
- `addons/l10n_ec_sale/__manifest__.py` (18 lines)
- `addons/l10n_ec_sale/controllers/__init__.py` (3 lines)
- `addons/l10n_ec_sale/controllers/portal.py` (19 lines)
- `addons/l10n_ec_sale/i18n/es_419.po` (73 lines)
- `addons/l10n_ec_sale/i18n/l10n_ec_sale.pot` (68 lines)
- `addons/l10n_ec_sale/models/__init__.py` (4 lines)
- `addons/l10n_ec_sale/models/payment_method.py` (32 lines)
- `addons/l10n_ec_sale/models/sale_order.py` (29 lines)
- `addons/l10n_ec_sale/tests/__init__.py` (1 lines)
- `addons/l10n_ec_sale/tests/test_l10n_ec_account_sale.py` (66 lines)
- `addons/l10n_ec_sale/views/payment_method_views.xml` (18 lines)
- `addons/l10n_ec_sale/views/sale_order_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
