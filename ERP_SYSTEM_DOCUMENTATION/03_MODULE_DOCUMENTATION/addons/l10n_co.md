# Module: l10n_co

- **Module ID:** MOD-152
- **Path:** `addons/l10n_co`
- **Manifest:** `addons/l10n_co/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Colombian Accounting and Tax Preconfiguration

Declared dependencies: `account_debit_note`, `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 8 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_debit_note",
    "account"
  ],
  "data": [
    "data/account_chart_template_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_co/__init__.py` (12 lines)
- `addons/l10n_co/__manifest__.py` (22 lines)
- `addons/l10n_co/data/account_chart_template_data.xml` (6 lines)
- `addons/l10n_co/data/template/account.account-co.csv` (802 lines)
- `addons/l10n_co/data/template/account.depreciation.model-co.csv` (6 lines)
- `addons/l10n_co/data/template/account.tax-co.csv` (269 lines)
- `addons/l10n_co/data/template/account.tax.group-co.csv` (46 lines)
- `addons/l10n_co/demo/demo_company.xml` (36 lines)
- `addons/l10n_co/i18n/es_419.po` (192 lines)
- `addons/l10n_co/i18n/l10n_co.pot` (166 lines)
- `addons/l10n_co/migrations/1.0/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_co/models/__init__.py` (3 lines)
- `addons/l10n_co/models/res_partner.py` (63 lines)
- `addons/l10n_co/models/template_co.py` (62 lines)
- `addons/l10n_co/tools/__init__.py` (2 lines)
- `addons/l10n_co/tools/partner_identifiers.py` (71 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
