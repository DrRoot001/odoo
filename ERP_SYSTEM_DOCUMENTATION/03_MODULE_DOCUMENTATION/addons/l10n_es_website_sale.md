# Module: l10n_es_website_sale

- **Module ID:** MOD-182
- **Path:** `addons/l10n_es_website_sale`
- **Manifest:** `addons/l10n_es_website_sale/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `l10n_es`, `website_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 2 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 1 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_es",
    "website_sale"
  ],
  "data": [
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_es_website_sale/__init__.py` (2 lines)
- `addons/l10n_es_website_sale/__manifest__.py` (10 lines)
- `addons/l10n_es_website_sale/controllers/__init__.py` (1 lines)
- `addons/l10n_es_website_sale/controllers/main.py` (14 lines)
- `addons/l10n_es_website_sale/i18n/es.po` (91 lines)
- `addons/l10n_es_website_sale/i18n/l10n_es_website_sale.pot` (87 lines)
- `addons/l10n_es_website_sale/models/__init__.py` (5 lines)
- `addons/l10n_es_website_sale/models/account_chart_template.py` (32 lines)
- `addons/l10n_es_website_sale/models/res_config_settings.py` (12 lines)
- `addons/l10n_es_website_sale/models/res_partner.py` (39 lines)
- `addons/l10n_es_website_sale/models/sale_order.py` (14 lines)
- `addons/l10n_es_website_sale/models/website.py` (30 lines)
- `addons/l10n_es_website_sale/tests/__init__.py` (1 lines)
- `addons/l10n_es_website_sale/tests/test_simplified_invoice.py` (124 lines)
- `addons/l10n_es_website_sale/views/res_config_settings_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
