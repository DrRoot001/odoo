# Module: l10n_no

- **Module ID:** MOD-286
- **Path:** `addons/l10n_no`
- **Manifest:** `addons/l10n_no/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

This is the module to manage the accounting chart for Norway in Odoo.

Updated for Odoo 9 by Bringsvor Consulting AS <www.bringsvor.com>


Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/account_tax_report_data.xml",
    "views/account_tax.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_no/__init__.py` (8 lines)
- `addons/l10n_no/__manifest__.py` (28 lines)
- `addons/l10n_no/data/account_tax_report_data.xml` (556 lines)
- `addons/l10n_no/data/template/account.account-no.csv` (747 lines)
- `addons/l10n_no/data/template/account.tax-no.csv` (149 lines)
- `addons/l10n_no/data/template/account.tax.group-no.csv` (6 lines)
- `addons/l10n_no/demo/demo_company.xml` (44 lines)
- `addons/l10n_no/i18n/l10n_no.pot` (125 lines)
- `addons/l10n_no/i18n/nb.po` (131 lines)
- `addons/l10n_no/migrations/2.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_no/models/__init__.py` (7 lines)
- `addons/l10n_no/models/account_journal.py` (12 lines)
- `addons/l10n_no/models/account_move.py` (29 lines)
- `addons/l10n_no/models/account_tax.py` (7 lines)
- `addons/l10n_no/models/res_company.py` (8 lines)
- `addons/l10n_no/models/res_partner.py` (26 lines)
- `addons/l10n_no/models/template_no.py` (35 lines)
- `addons/l10n_no/views/account_tax.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
