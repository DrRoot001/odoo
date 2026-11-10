# Module: l10n_se

- **Module ID:** MOD-314
- **Path:** `addons/l10n_se`
- **Manifest:** `addons/l10n_se/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Swedish Accounting
------------------

This is the base module to manage the accounting chart for Sweden in Odoo.
It also includes the invoice OCR payment reference handling.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
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
    "data/account.account.tag.csv",
    "data/account_tax_report_data.xml",
    "data/res_country_data.xml",
    "views/partner_view.xml",
    "views/account_journal_view.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_se/__init__.py` (3 lines)
- `addons/l10n_se/__manifest__.py` (33 lines)
- `addons/l10n_se/data/account.account.tag.csv` (42 lines)
- `addons/l10n_se/data/account_tax_report_data.xml` (403 lines)
- `addons/l10n_se/data/res_country_data.xml` (32 lines)
- `addons/l10n_se/data/template/account.account-se.csv` (333 lines)
- `addons/l10n_se/data/template/account.account-se_K2.csv` (857 lines)
- `addons/l10n_se/data/template/account.account-se_K3.csv` (27 lines)
- `addons/l10n_se/data/template/account.fiscal.position-se.csv` (21 lines)
- `addons/l10n_se/data/template/account.tax-se.csv` (177 lines)
- `addons/l10n_se/data/template/account.tax.group-se.csv` (5 lines)
- `addons/l10n_se/data/template/account.tax.group-se_K2.csv` (5 lines)
- `addons/l10n_se/data/template/account.tax.group-se_K3.csv` (5 lines)
- `addons/l10n_se/demo/demo_company.xml` (44 lines)
- `addons/l10n_se/i18n/l10n_se.pot` (627 lines)
- `addons/l10n_se/i18n/sv.po` (645 lines)
- `addons/l10n_se/migrations/1.1/end-migrate.py` (7 lines)
- `addons/l10n_se/models/__init__.py` (8 lines)
- `addons/l10n_se/models/account_journal.py` (25 lines)
- `addons/l10n_se/models/account_move.py` (77 lines)
- `addons/l10n_se/models/res_company.py` (22 lines)
- `addons/l10n_se/models/res_partner.py` (21 lines)
- `addons/l10n_se/models/template_se.py` (36 lines)
- `addons/l10n_se/models/template_se_K2.py` (26 lines)
- `addons/l10n_se/models/template_se_K3.py` (26 lines)
- `addons/l10n_se/views/account_journal_view.xml` (15 lines)
- `addons/l10n_se/views/partner_view.xml` (18 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
