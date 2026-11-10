# Module: l10n_fr

- **Module ID:** MOD-189
- **Path:** `addons/l10n_fr`
- **Manifest:** `addons/l10n_fr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.




Declared dependencies: `base`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base"
  ],
  "data": [
    "data/res_country_data.xml",
    "views/res_company_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fr/__init__.py` (4 lines)
- `addons/l10n_fr/__manifest__.py` (22 lines)
- `addons/l10n_fr/data/res_country_data.xml` (26 lines)
- `addons/l10n_fr/demo/demo_company.xml` (37 lines)
- `addons/l10n_fr/i18n/fr.po` (91 lines)
- `addons/l10n_fr/i18n/l10n_fr.pot` (85 lines)
- `addons/l10n_fr/models/__init__.py` (5 lines)
- `addons/l10n_fr/models/res_company.py` (72 lines)
- `addons/l10n_fr/models/res_partner.py` (23 lines)
- `addons/l10n_fr/tests/__init__.py` (3 lines)
- `addons/l10n_fr/tests/test_res_partner.py` (18 lines)
- `addons/l10n_fr/views/res_company_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
