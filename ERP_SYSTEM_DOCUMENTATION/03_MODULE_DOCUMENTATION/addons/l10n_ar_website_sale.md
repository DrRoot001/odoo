# Module: l10n_ar_website_sale

- **Module ID:** MOD-123
- **Path:** `addons/l10n_ar_website_sale`
- **Manifest:** `addons/l10n_ar_website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Bridge Website Sale for Argentina

Declared dependencies: `website_sale`, `l10n_ar`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "website_sale",
    "l10n_ar"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/templates.xml"
  ],
  "assets": {
    "web.assets_frontend": [
      "l10n_ar_website_sale/static/src/interactions/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ar_website_sale/__init__.py` (1 lines)
- `addons/l10n_ar_website_sale/__manifest__.py` (23 lines)
- `addons/l10n_ar_website_sale/i18n/es_419.po` (75 lines)
- `addons/l10n_ar_website_sale/i18n/l10n_ar_website_sale.pot` (71 lines)
- `addons/l10n_ar_website_sale/models/__init__.py` (3 lines)
- `addons/l10n_ar_website_sale/models/product_template.py` (57 lines)
- `addons/l10n_ar_website_sale/models/res_config_settings.py` (11 lines)
- `addons/l10n_ar_website_sale/models/website.py` (19 lines)
- `addons/l10n_ar_website_sale/static/src/interactions/product_page.js` (25 lines)
- `addons/l10n_ar_website_sale/tests/__init__.py` (1 lines)
- `addons/l10n_ar_website_sale/tests/test_l10n_ar_website_sale.py` (193 lines)
- `addons/l10n_ar_website_sale/views/res_config_settings_views.xml` (18 lines)
- `addons/l10n_ar_website_sale/views/templates.xml` (39 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
