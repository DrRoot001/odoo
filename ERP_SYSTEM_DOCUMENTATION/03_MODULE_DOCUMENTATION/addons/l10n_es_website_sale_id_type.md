# Module: l10n_es_website_sale_id_type

- **Module ID:** MOD-183
- **Path:** `addons/l10n_es_website_sale_id_type`
- **Manifest:** `addons/l10n_es_website_sale_id_type/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Let customers pick the type of their identification document at checkout

No manifest description declared.

Declared dependencies: `l10n_es_website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_es_website_sale"
  ],
  "data": [
    "views/address_form_templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_es_website_sale_id_type/static/src/interactions/l10n_es_id_type.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_es_website_sale_id_type/__init__.py` (3 lines)
- `addons/l10n_es_website_sale_id_type/__manifest__.py` (17 lines)
- `addons/l10n_es_website_sale_id_type/controllers/__init__.py` (2 lines)
- `addons/l10n_es_website_sale_id_type/controllers/main.py` (98 lines)
- `addons/l10n_es_website_sale_id_type/i18n/l10n_es_website_sale_id_type.pot` (67 lines)
- `addons/l10n_es_website_sale_id_type/models/__init__.py` (2 lines)
- `addons/l10n_es_website_sale_id_type/models/res_partner.py` (52 lines)
- `addons/l10n_es_website_sale_id_type/static/src/interactions/l10n_es_id_type.js` (34 lines)
- `addons/l10n_es_website_sale_id_type/tests/__init__.py` (1 lines)
- `addons/l10n_es_website_sale_id_type/tests/test_checkout_identification.py` (261 lines)
- `addons/l10n_es_website_sale_id_type/views/address_form_templates.xml` (58 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
