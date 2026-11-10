# Module: test_translation

- **Module ID:** MOD-664
- **Path:** `odoo/addons/test_translation`
- **Manifest:** `odoo/addons/test_translation/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

A module to test translation.

Declared dependencies: `base`, `web_tour`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 7 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "web_tour"
  ],
  "data": [
    "view.xml",
    "data/test_translation_data.xml",
    "data/test.translation.model1.csv",
    "data/test.translation.model1-translated.csv",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "test_translation/static/tests/tours/constraint.js",
      "test_translation/static/src/xml/js_templates.xml"
    ]
  }
}
```

### Representative source files

- `odoo/addons/test_translation/__init__.py` (1 lines)
- `odoo/addons/test_translation/__manifest__.py` (22 lines)
- `odoo/addons/test_translation/data/files/test_spreadsheet_dashboard.json` (174 lines)
- `odoo/addons/test_translation/data/files/test_spreadsheet_v16_dashboard.json` (146 lines)
- `odoo/addons/test_translation/data/test.translation.model1-translated.csv` (2 lines)
- `odoo/addons/test_translation/data/test.translation.model1.csv` (2 lines)
- `odoo/addons/test_translation/data/test_translation_data.xml` (30 lines)
- `odoo/addons/test_translation/i18n/dot.csv` (5 lines)
- `odoo/addons/test_translation/i18n/fr.po` (777 lines)
- `odoo/addons/test_translation/i18n/fr_BE.po` (775 lines)
- `odoo/addons/test_translation/i18n/fr_CA.po` (775 lines)
- `odoo/addons/test_translation/i18n/test_translation.pot` (775 lines)
- `odoo/addons/test_translation/i18n/tlh.po` (775 lines)
- `odoo/addons/test_translation/models/__init__.py` (2 lines)
- `odoo/addons/test_translation/models/models.py` (99 lines)
- `odoo/addons/test_translation/models/test_related_translation.py` (58 lines)
- `odoo/addons/test_translation/security/ir.access.csv` (6 lines)
- `odoo/addons/test_translation/static/src/js/js_codefile.js` (60 lines)
- `odoo/addons/test_translation/static/src/xml/js_templates.xml` (13 lines)
- `odoo/addons/test_translation/static/tests/tours/constraint.js` (31 lines)
- `odoo/addons/test_translation/tests/__init__.py` (5 lines)
- `odoo/addons/test_translation/tests/test_export_wizard.py` (26 lines)
- `odoo/addons/test_translation/tests/test_load_manifest_translations.py` (27 lines)
- `odoo/addons/test_translation/tests/test_related_translation.py` (780 lines)
- `odoo/addons/test_translation/tests/test_term_count.py` (515 lines)
- `odoo/addons/test_translation/tests/test_ui.py` (21 lines)
- `odoo/addons/test_translation/view.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
