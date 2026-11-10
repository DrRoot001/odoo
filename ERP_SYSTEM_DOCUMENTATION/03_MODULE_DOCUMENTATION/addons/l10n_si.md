# Module: l10n_si

- **Module ID:** MOD-317
- **Path:** `addons/l10n_si`
- **Manifest:** `addons/l10n_si/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Chart of accounts and taxes for Slovenia.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/res_country_data.xml",
    "data/account_tax_report_data.xml",
    "data/account_tax_report_ir_data.xml",
    "data/account_tax_report_pd_data.xml",
    "data/account_tax_report_pr_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_si/__init__.py` (2 lines)
- `addons/l10n_si/__manifest__.py` (29 lines)
- `addons/l10n_si/data/account_tax_report_data.xml` (524 lines)
- `addons/l10n_si/data/account_tax_report_ir_data.xml` (511 lines)
- `addons/l10n_si/data/account_tax_report_pd_data.xml` (31 lines)
- `addons/l10n_si/data/account_tax_report_pr_data.xml` (277 lines)
- `addons/l10n_si/data/res_country_data.xml` (28 lines)
- `addons/l10n_si/data/template/account.account-si.csv` (608 lines)
- `addons/l10n_si/data/template/account.fiscal.position-si.csv` (18 lines)
- `addons/l10n_si/data/template/account.tax-si.csv` (257 lines)
- `addons/l10n_si/data/template/account.tax.group-si.csv` (9 lines)
- `addons/l10n_si/demo/demo_company.xml` (42 lines)
- `addons/l10n_si/i18n/l10n_si.pot` (114 lines)
- `addons/l10n_si/i18n/sl.po` (121 lines)
- `addons/l10n_si/models/__init__.py` (4 lines)
- `addons/l10n_si/models/account_journal.py` (10 lines)
- `addons/l10n_si/models/account_move.py` (55 lines)
- `addons/l10n_si/models/template_si.py` (33 lines)
- `addons/l10n_si/tests/__init__.py` (1 lines)
- `addons/l10n_si/tests/test_get_reference.py` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
