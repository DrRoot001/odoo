# Module: l10n_br_website_sale

- **Module ID:** MOD-141
- **Path:** `addons/l10n_br_website_sale`
- **Manifest:** `addons/l10n_br_website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Bridge Website Sale for Brazil

Declared dependencies: `l10n_br`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
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
    "l10n_br",
    "website_sale"
  ],
  "data": [
    "views/templates.xml"
  ]
}
```

### Representative source files

- `addons/l10n_br_website_sale/__init__.py` (1 lines)
- `addons/l10n_br_website_sale/__manifest__.py` (16 lines)
- `addons/l10n_br_website_sale/i18n/l10n_br_website_sale.pot` (26 lines)
- `addons/l10n_br_website_sale/i18n/pt_BR.po` (40 lines)
- `addons/l10n_br_website_sale/views/templates.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
