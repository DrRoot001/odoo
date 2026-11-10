# Module: l10n_mt

- **Module ID:** MOD-274
- **Path:** `addons/l10n_mt`
- **Manifest:** `addons/l10n_mt/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Malta basic package that contains the chart of accounts, the taxes, tax reports, etc.
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "data/menuitem_data.xml",
    "data/account_tax_report_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_mt/__init__.py` (2 lines)
- `addons/l10n_mt/__manifest__.py` (26 lines)
- `addons/l10n_mt/data/account_tax_report_data.xml` (482 lines)
- `addons/l10n_mt/data/menuitem_data.xml` (4 lines)
- `addons/l10n_mt/data/template/account.account-mt.csv` (482 lines)
- `addons/l10n_mt/data/template/account.fiscal.position-mt.csv` (6 lines)
- `addons/l10n_mt/data/template/account.tax-mt.csv` (89 lines)
- `addons/l10n_mt/data/template/account.tax.group-mt.csv` (5 lines)
- `addons/l10n_mt/demo/demo_company.xml` (42 lines)
- `addons/l10n_mt/migrations/1.1/post-fix-tax-grid-tags.py` (103 lines)
- `addons/l10n_mt/models/__init__.py` (2 lines)
- `addons/l10n_mt/models/template_mt.py` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
