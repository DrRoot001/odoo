# Module: l10n_us

- **Module ID:** MOD-336
- **Path:** `addons/l10n_us`
- **Manifest:** `addons/l10n_us/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


    

Declared dependencies: `base`, `base_address_extended`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "base",
    "base_address_extended"
  ],
  "data": [
    "security/ir.access.csv",
    "data/l10n_us.res.county.csv",
    "data/res.city.csv",
    "data/res_company_data.xml",
    "views/res_city_views.xml",
    "views/res_partner_bank_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_us/__init__.py` (4 lines)
- `addons/l10n_us/__manifest__.py` (26 lines)
- `addons/l10n_us/data/l10n_us.res.county.csv` (3,173 lines)
- `addons/l10n_us/data/res.city.csv` (31,278 lines)
- `addons/l10n_us/data/res_company_data.xml` (6 lines)
- `addons/l10n_us/demo/demo_company.xml` (33 lines)
- `addons/l10n_us/i18n/es_419.po` (115,337 lines)
- `addons/l10n_us/i18n/l10n_us.pot` (115,300 lines)
- `addons/l10n_us/models/__init__.py` (6 lines)
- `addons/l10n_us/models/l10n_us_res_county.py` (16 lines)
- `addons/l10n_us/models/res_city.py` (13 lines)
- `addons/l10n_us/models/res_partner_bank.py` (15 lines)
- `addons/l10n_us/security/ir.access.csv` (3 lines)
- `addons/l10n_us/views/res_city_views.xml` (24 lines)
- `addons/l10n_us/views/res_partner_bank_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
