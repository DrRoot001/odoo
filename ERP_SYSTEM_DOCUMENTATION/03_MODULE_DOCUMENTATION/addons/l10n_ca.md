# Module: l10n_ca

- **Module ID:** MOD-142
- **Path:** `addons/l10n_ca`
- **Manifest:** `addons/l10n_ca/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the Canadian accounting chart in Odoo.
===========================================================================================

Canadian accounting charts and localizations.

Fiscal positions
----------------

When considering taxes to be applied, it is the province where the delivery occurs that matters.
Therefore we decided to implement the most common case in the fiscal positions: delivery is the
responsibility of the vendor and done at the customer location.

Some examples:

1) You have a customer from another province and you deliver to his location.
On the customer, set the fiscal position to his province.

2) You have a customer from another province. However this customer comes to your location
with their truck to pick up products. On the customer, do not set any fiscal position.

3) An international vendor doesn't charge you any tax. Taxes are charged at customs
by the customs broker. On the vendor, set the fiscal position to International.

4) An international vendor charge you your provincial tax. They are registered with your
position.
    

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 7 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account"
  ],
  "data": [
    "data/tax_report.xml",
    "views/res_partner_view.xml",
    "views/res_company_view.xml",
    "views/res_config_settings_views.xml",
    "views/report_invoice.xml",
    "views/report_template.xml"
  ],
  "demo": [
    "demo/demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ca/__init__.py` (5 lines)
- `addons/l10n_ca/__manifest__.py` (53 lines)
- `addons/l10n_ca/data/tax_report.xml` (966 lines)
- `addons/l10n_ca/data/template/account.account-ca_2023.csv` (150 lines)
- `addons/l10n_ca/data/template/account.depreciation.model-ca_2023.csv` (6 lines)
- `addons/l10n_ca/data/template/account.fiscal.position-ca_2023.csv` (15 lines)
- `addons/l10n_ca/data/template/account.tax-ca_2023.csv` (102 lines)
- `addons/l10n_ca/data/template/account.tax.group-ca_2023.csv` (9 lines)
- `addons/l10n_ca/demo/demo.xml` (80 lines)
- `addons/l10n_ca/i18n/fr.po` (243 lines)
- `addons/l10n_ca/i18n/l10n_ca.pot` (226 lines)
- `addons/l10n_ca/migrations/1.1/end-migrate-update_taxes.py` (11 lines)
- `addons/l10n_ca/models/__init__.py` (5 lines)
- `addons/l10n_ca/models/res_company.py` (30 lines)
- `addons/l10n_ca/models/res_config_settings.py` (9 lines)
- `addons/l10n_ca/models/res_partner.py` (7 lines)
- `addons/l10n_ca/models/template_ca.py` (87 lines)
- `addons/l10n_ca/tests/__init__.py` (1 lines)
- `addons/l10n_ca/tests/test_fiscal_position.py` (34 lines)
- `addons/l10n_ca/views/report_invoice.xml` (22 lines)
- `addons/l10n_ca/views/report_template.xml` (26 lines)
- `addons/l10n_ca/views/res_company_view.xml` (15 lines)
- `addons/l10n_ca/views/res_config_settings_views.xml` (28 lines)
- `addons/l10n_ca/views/res_partner_view.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
