# Module: l10n_fr_hr_holidays

- **Module ID:** MOD-192
- **Path:** `addons/l10n_fr_hr_holidays`
- **Manifest:** `addons/l10n_fr_hr_holidays/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Management of leaves for part-time workers in France

No manifest description declared.

Declared dependencies: `hr_holidays`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "hr_holidays"
  ],
  "data": [
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "data/l10n_fr_hr_holidays_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fr_hr_holidays/__init__.py` (4 lines)
- `addons/l10n_fr_hr_holidays/__manifest__.py` (18 lines)
- `addons/l10n_fr_hr_holidays/data/l10n_fr_hr_holidays_demo.xml` (79 lines)
- `addons/l10n_fr_hr_holidays/i18n/fr.po` (112 lines)
- `addons/l10n_fr_hr_holidays/i18n/l10n_fr_hr_holidays.pot` (98 lines)
- `addons/l10n_fr_hr_holidays/models/__init__.py` (7 lines)
- `addons/l10n_fr_hr_holidays/models/hr_leave.py` (181 lines)
- `addons/l10n_fr_hr_holidays/models/hr_version.py` (66 lines)
- `addons/l10n_fr_hr_holidays/models/res_company.py` (26 lines)
- `addons/l10n_fr_hr_holidays/models/res_config_settings.py` (13 lines)
- `addons/l10n_fr_hr_holidays/tests/__init__.py` (5 lines)
- `addons/l10n_fr_hr_holidays/tests/test_french_leaves.py` (592 lines)
- `addons/l10n_fr_hr_holidays/tests/test_french_work_entries.py` (99 lines)
- `addons/l10n_fr_hr_holidays/views/res_config_settings_views.xml` (28 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
