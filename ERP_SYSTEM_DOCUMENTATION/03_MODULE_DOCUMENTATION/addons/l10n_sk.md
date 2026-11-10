# Module: l10n_sk

- **Module ID:** MOD-318
- **Path:** `addons/l10n_sk`
- **Manifest:** `addons/l10n_sk/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Slovakia accounting chart and localization: Chart of Accounts 2020, basic VAT rates +
fiscal positions.

Tento modul definuje:
• Slovenskú účtovú osnovu za rok 2020

• Základné sadzby pre DPH z predaja a nákupu

• Základné fiškálne pozície pre slovenskú legislatívu


Pre viac informácií kontaktujte info@26house.com alebo navštívte https://www.26house.com.

    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/tax_report.xml",
    "views/res_company_views.xml",
    "views/report_invoice.xml",
    "views/report_template.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_sk/__init__.py` (2 lines)
- `addons/l10n_sk/__manifest__.py` (39 lines)
- `addons/l10n_sk/data/tax_report.xml` (930 lines)
- `addons/l10n_sk/data/template/account.account-sk.csv` (392 lines)
- `addons/l10n_sk/data/template/account.depreciation.model-sk.csv` (7 lines)
- `addons/l10n_sk/data/template/account.fiscal.position-sk.csv` (6 lines)
- `addons/l10n_sk/data/template/account.tax-sk.csv` (195 lines)
- `addons/l10n_sk/data/template/account.tax.group-sk.csv` (5 lines)
- `addons/l10n_sk/demo/demo_company.xml` (42 lines)
- `addons/l10n_sk/i18n/l10n_sk.pot` (180 lines)
- `addons/l10n_sk/i18n/sk.po` (192 lines)
- `addons/l10n_sk/migrations/1.1/pre-migrate.py` (17 lines)
- `addons/l10n_sk/models/__init__.py` (6 lines)
- `addons/l10n_sk/models/account_move.py` (31 lines)
- `addons/l10n_sk/models/res_bank.py` (126 lines)
- `addons/l10n_sk/models/res_company.py` (22 lines)
- `addons/l10n_sk/models/res_partner.py` (16 lines)
- `addons/l10n_sk/models/template_sk.py` (116 lines)
- `addons/l10n_sk/tests/__init__.py` (2 lines)
- `addons/l10n_sk/tests/test_l10n_sk_qr_code.py` (186 lines)
- `addons/l10n_sk/views/report_invoice.xml` (33 lines)
- `addons/l10n_sk/views/report_template.xml` (31 lines)
- `addons/l10n_sk/views/res_company_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
