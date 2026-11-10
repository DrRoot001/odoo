# Module: l10n_lb_account

- **Module ID:** MOD-261
- **Path:** `addons/l10n_lb_account`
- **Manifest:** `addons/l10n_lb_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Lebanon in Odoo.
==============================================================================
Lebanon accounting basic charts,taxes and localization.
Activates:
* Chart of Accounts
* Taxes
* Fiscal Positions
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_lb_account/__init__.py` (1 lines)
- `addons/l10n_lb_account/__manifest__.py` (21 lines)
- `addons/l10n_lb_account/data/template/account.account-lb.csv` (586 lines)
- `addons/l10n_lb_account/data/template/account.fiscal.position-lb.csv` (3 lines)
- `addons/l10n_lb_account/data/template/account.tax-lb.csv` (33 lines)
- `addons/l10n_lb_account/data/template/account.tax.group-lb.csv` (4 lines)
- `addons/l10n_lb_account/demo/demo_company.xml` (43 lines)
- `addons/l10n_lb_account/i18n/ar.po` (63 lines)
- `addons/l10n_lb_account/i18n/fr.po` (53 lines)
- `addons/l10n_lb_account/i18n/l10n_lb_account.pot` (49 lines)
- `addons/l10n_lb_account/models/__init__.py` (2 lines)
- `addons/l10n_lb_account/models/template_lb.py` (41 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
