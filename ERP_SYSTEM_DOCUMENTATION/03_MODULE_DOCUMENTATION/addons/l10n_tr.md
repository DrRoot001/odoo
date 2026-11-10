# Module: l10n_tr

- **Module ID:** MOD-326
- **Path:** `addons/l10n_tr`
- **Manifest:** `addons/l10n_tr/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Türkiye in Odoo
==========================================================================

Türkiye accounting basic charts and localizations
-------------------------------------------------
Activates:

- Chart of Accounts
- Taxes
- Tax Report
    

Declared dependencies: `account`, `contacts`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "contacts"
  ],
  "data": [
    "security/ir.access.csv",
    "data/account_tax_report_data.xml",
    "data/account_tax_report_stamp_tax.xml",
    "data/l10n_tr.tax.office.csv",
    "views/l10n_tr_tax_office_views.xml",
    "views/res_company_views.xml",
    "views/res_partner_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_tr/static/src/js/dynamic_list.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_tr/__init__.py` (2 lines)
- `addons/l10n_tr/__manifest__.py` (44 lines)
- `addons/l10n_tr/data/account_tax_report_data.xml` (530 lines)
- `addons/l10n_tr/data/account_tax_report_stamp_tax.xml` (175 lines)
- `addons/l10n_tr/data/l10n_tr.tax.office.csv` (1,047 lines)
- `addons/l10n_tr/data/template/account.account-tr.csv` (348 lines)
- `addons/l10n_tr/data/template/account.fiscal.position-tr.csv` (9 lines)
- `addons/l10n_tr/data/template/account.tax-tr.csv` (135 lines)
- `addons/l10n_tr/data/template/account.tax.group-tr.csv` (15 lines)
- `addons/l10n_tr/demo/demo_company.xml` (88 lines)
- `addons/l10n_tr/i18n/l10n_tr.pot` (157 lines)
- `addons/l10n_tr/i18n/tr.po` (161 lines)
- `addons/l10n_tr/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_tr/migrations/1.2/end-migrate_update_package.py` (8 lines)
- `addons/l10n_tr/migrations/1.3/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_tr/models/__init__.py` (8 lines)
- `addons/l10n_tr/models/account_journal.py` (26 lines)
- `addons/l10n_tr/models/account_move_line.py` (36 lines)
- `addons/l10n_tr/models/ir_http.py` (14 lines)
- `addons/l10n_tr/models/l10n_tr_tax_office.py` (21 lines)
- `addons/l10n_tr/models/product.py` (22 lines)
- `addons/l10n_tr/models/res_company.py` (12 lines)
- `addons/l10n_tr/models/res_partner.py` (48 lines)
- `addons/l10n_tr/models/template_tr.py` (57 lines)
- `addons/l10n_tr/security/ir.access.csv` (3 lines)
- `addons/l10n_tr/static/src/js/dynamic_list.js` (10 lines)
- `addons/l10n_tr/tests/__init__.py` (1 lines)
- `addons/l10n_tr/tests/test_sales_return_account.py` (34 lines)
- `addons/l10n_tr/views/l10n_tr_tax_office_views.xml` (49 lines)
- `addons/l10n_tr/views/res_company_views.xml` (13 lines)
- `addons/l10n_tr/views/res_partner_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
