# Module: l10n_kr_sale

- **Module ID:** MOD-255
- **Path:** `addons/l10n_kr_sale`
- **Manifest:** `addons/l10n_kr_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Bridge module between the Korean localization and Sales, exposing the proof of issuance
(발행 증빙) on sales orders and propagating it to the invoices created from them.
    

Declared dependencies: `sale`, `l10n_kr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale",
    "l10n_kr"
  ],
  "data": [
    "views/sale_order_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_kr_sale/__init__.py` (2 lines)
- `addons/l10n_kr_sale/__manifest__.py` (16 lines)
- `addons/l10n_kr_sale/i18n/ko.po` (81 lines)
- `addons/l10n_kr_sale/i18n/l10n_kr_sale.pot` (81 lines)
- `addons/l10n_kr_sale/models/__init__.py` (2 lines)
- `addons/l10n_kr_sale/models/sale_order.py` (39 lines)
- `addons/l10n_kr_sale/views/sale_order_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
