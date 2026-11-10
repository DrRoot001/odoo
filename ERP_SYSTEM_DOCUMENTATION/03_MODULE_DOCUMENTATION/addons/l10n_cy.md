# Module: l10n_cy

- **Module ID:** MOD-155
- **Path:** `addons/l10n_cy`
- **Manifest:** `addons/l10n_cy/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Basic package for Cyprus that contains the chart of accounts, taxes, tax reports,...
    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
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

- `addons/l10n_cy/__init__.py` (1 lines)
- `addons/l10n_cy/__manifest__.py` (23 lines)
- `addons/l10n_cy/data/account_tax_report_data.xml` (204 lines)
- `addons/l10n_cy/data/menuitem_data.xml` (4 lines)
- `addons/l10n_cy/data/template/account.account-cy.csv` (171 lines)
- `addons/l10n_cy/data/template/account.fiscal.position-cy.csv` (6 lines)
- `addons/l10n_cy/data/template/account.tax-cy.csv` (125 lines)
- `addons/l10n_cy/data/template/account.tax.group-cy.csv` (6 lines)
- `addons/l10n_cy/demo/demo_company.xml` (42 lines)
- `addons/l10n_cy/i18n/el.po` (162 lines)
- `addons/l10n_cy/i18n/l10n_cy.pot` (157 lines)
- `addons/l10n_cy/i18n/tr.po` (166 lines)
- `addons/l10n_cy/models/__init__.py` (1 lines)
- `addons/l10n_cy/models/template_cy.py` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
