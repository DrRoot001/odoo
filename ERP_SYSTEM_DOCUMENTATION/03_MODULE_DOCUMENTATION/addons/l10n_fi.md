# Module: l10n_fi

- **Module ID:** MOD-187
- **Path:** `addons/l10n_fi`
- **Manifest:** `addons/l10n_fi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the Odoo module to manage the accounting in Finland.
============================================================

After installing this module, you'll have access to:
    * Finnish chart of account
    * Fiscal positions
    * Invoice Payment Reference Types (Finnish Standard Reference & Finnish Creditor Reference (RF))
    * Finnish Reference format for Sale Orders

Set the payment reference type from the Sales Journal.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 4 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
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
    "data/account_account_tag_data.xml",
    "data/account_tax_report_line.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fi/__init__.py` (4 lines)
- `addons/l10n_fi/__manifest__.py` (35 lines)
- `addons/l10n_fi/data/account_account_tag_data.xml` (684 lines)
- `addons/l10n_fi/data/account_tax_report_line.xml` (294 lines)
- `addons/l10n_fi/data/template/account.account-fi.csv` (972 lines)
- `addons/l10n_fi/data/template/account.fiscal.position-fi.csv` (7 lines)
- `addons/l10n_fi/data/template/account.tax-fi.csv` (240 lines)
- `addons/l10n_fi/data/template/account.tax.group-fi.csv` (7 lines)
- `addons/l10n_fi/demo/demo_company.xml` (43 lines)
- `addons/l10n_fi/i18n/fi.po` (111 lines)
- `addons/l10n_fi/i18n/l10n_fi.pot` (94 lines)
- `addons/l10n_fi/migrations/13.0.2/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_fi/models/__init__.py` (4 lines)
- `addons/l10n_fi/models/account_journal.py` (12 lines)
- `addons/l10n_fi/models/account_move.py` (88 lines)
- `addons/l10n_fi/models/template_fi.py` (45 lines)
- `addons/l10n_fi/tests/__init__.py` (5 lines)
- `addons/l10n_fi/tests/test_get_reference.py` (42 lines)
- `addons/l10n_fi/tests/test_references.py` (62 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
