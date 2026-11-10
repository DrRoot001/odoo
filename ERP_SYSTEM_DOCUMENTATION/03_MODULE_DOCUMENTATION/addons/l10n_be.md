# Module: l10n_be

- **Module ID:** MOD-128
- **Path:** `addons/l10n_be`
- **Manifest:** `addons/l10n_be/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the base module to manage the accounting chart for Belgium in Odoo.
==============================================================================

After installing this module, the Configuration wizard for accounting is launched.
    * We have the account templates which can be helpful to generate Charts of Accounts.
    * On that particular wizard, you will be asked to pass the name of the company,
      the chart template to follow, the no. of digits to generate, the code for your
      account and bank account, currency to create journals.

Thus, the pure copy of Chart Template is generated.

Wizards provided by this module:
--------------------------------
    * Partner VAT Intra: Enlist the partners with their related VAT and invoiced
      amounts. Prepares an XML file format.

        **Path to access:** Invoicing/Reporting/Legal Reports/Belgium Statements/Partner VAT Intra
    * Periodical VAT Declaration: Prepares an XML file for Vat Declaration of
      the Main company of the User currently Logged in.

        **Path to access:** Invoicing/Reporting/Legal Reports/Belgium Statements/Periodical VAT Declaration
    * Annual Listing Of VAT-Subjected Customers: Prepares an XML file for Vat
      Declaration of the Main company of the User currently Logged in Based on
      Fiscal year.

        **Path to access:** Invoicing/Reporting/Legal Reports/Belgium Statements/Annual Listing Of VAT-Subjected Customers

    

Declared dependencies: `account`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/l10n_be_sequence_data.xml",
    "data/menuitem_data.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_be/__init__.py` (3 lines)
- `addons/l10n_be/__manifest__.py` (53 lines)
- `addons/l10n_be/data/account_tax_report_data.xml` (689 lines)
- `addons/l10n_be/data/l10n_be_sequence_data.xml` (12 lines)
- `addons/l10n_be/data/menuitem_data.xml` (4 lines)
- `addons/l10n_be/data/template/account.account-be.csv` (430 lines)
- `addons/l10n_be/data/template/account.account-be_asso.csv` (44 lines)
- `addons/l10n_be/data/template/account.account-be_comp.csv` (69 lines)
- `addons/l10n_be/data/template/account.depreciation.model-be.csv` (7 lines)
- `addons/l10n_be/data/template/account.fiscal.position-be.csv` (14 lines)
- `addons/l10n_be/data/template/account.tax-be.csv` (453 lines)
- `addons/l10n_be/data/template/account.tax.group-be.csv` (5 lines)
- `addons/l10n_be/demo/__init__.py` (1 lines)
- `addons/l10n_be/demo/account_demo.py` (18 lines)
- `addons/l10n_be/demo/demo_company.xml` (42 lines)
- `addons/l10n_be/i18n/de.po` (217 lines)
- `addons/l10n_be/i18n/fr.po` (182 lines)
- `addons/l10n_be/i18n/l10n_be.pot` (152 lines)
- `addons/l10n_be/i18n/nl.po` (220 lines)
- `addons/l10n_be/models/__init__.py` (8 lines)
- `addons/l10n_be/models/account_journal.py` (12 lines)
- `addons/l10n_be/models/account_move.py` (50 lines)
- `addons/l10n_be/models/account_tax.py` (9 lines)
- `addons/l10n_be/models/res_company.py` (67 lines)
- `addons/l10n_be/models/template_be.py` (125 lines)
- `addons/l10n_be/models/template_be_asso.py` (44 lines)
- `addons/l10n_be/models/template_be_comp.py` (45 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
