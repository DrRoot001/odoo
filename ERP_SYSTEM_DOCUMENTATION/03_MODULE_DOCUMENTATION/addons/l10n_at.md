# Module: l10n_at

- **Module ID:** MOD-125
- **Path:** `addons/l10n_at`
- **Manifest:** `addons/l10n_at/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

Austrian Standardized Charts & Tax



Austrian charts of accounts (Einheitskontenrahmen 2010).
==========================================================

    * Defines the following chart of account templates:
        * Austrian General Chart of accounts 2010
    * Defines templates for VAT on sales and purchases
    * Defines tax templates
    * Defines fiscal positions for Austrian fiscal legislation
    * Defines tax reports U1/U30

    

Declared dependencies: `account`, `account_edi_ubl_cii`, `l10n_din5008`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "account_edi_ubl_cii",
    "l10n_din5008"
  ],
  "data": [
    "data/account_account_tag.xml",
    "data/account.account.tag.csv",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_at/__init__.py` (2 lines)
- `addons/l10n_at/__manifest__.py` (39 lines)
- `addons/l10n_at/data/account.account.tag.csv` (951 lines)
- `addons/l10n_at/data/account_account_tag.xml` (649 lines)
- `addons/l10n_at/data/account_tax_report_data.xml` (839 lines)
- `addons/l10n_at/data/template/account.account-at.csv` (239 lines)
- `addons/l10n_at/data/template/account.fiscal.position-at.csv` (14 lines)
- `addons/l10n_at/data/template/account.tax-at.csv` (261 lines)
- `addons/l10n_at/data/template/account.tax.group-at.csv` (8 lines)
- `addons/l10n_at/demo/demo_company.xml` (43 lines)
- `addons/l10n_at/i18n/de.po` (481 lines)
- `addons/l10n_at/i18n/l10n_at.pot` (476 lines)
- `addons/l10n_at/migrations/3.2/post-migrate.py` (14 lines)
- `addons/l10n_at/models/__init__.py` (3 lines)
- `addons/l10n_at/models/account_journal.py` (22 lines)
- `addons/l10n_at/models/template_at.py` (55 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
