# Module: l10n_fr_account

- **Module ID:** MOD-190
- **Path:** `addons/l10n_fr_account`
- **Manifest:** `addons/l10n_fr_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


This is the module to manage the accounting chart for France in Odoo.
========================================================================

This module applies to companies based in France mainland. It doesn't apply to
companies based in the DOM-TOMs (Guadeloupe, Martinique, Guyane, Réunion, Mayotte).

This localisation module creates the VAT taxes of type 'tax included' for purchases
(it is notably required when you use the module 'hr_expense'). Beware that these
'tax included' VAT taxes are not managed by the fiscal positions provided by this
module (because it is complex to manage both 'tax excluded' and 'tax included'
scenarios in fiscal positions).

This localisation module doesn't properly handle the scenario when a France-mainland
company sells services to a company based in the DOMs. We could manage it in the
fiscal positions, but it would require to differentiate between 'product' VAT taxes
and 'service' VAT taxes. We consider that it is too 'heavy' to have this by default
in l10n_fr_account; companies that sell services to DOM-based companies should update the
configuration of their taxes and fiscal positions manually.

**Credits:** Sistheo, Zeekom, CrysaLEAD, Akretion and Camptocamp.


Declared dependencies: `account`, `account_edi_ubl_cii`, `l10n_fr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 23 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "account_edi_ubl_cii",
    "l10n_fr"
  ],
  "data": [
    "data/account_chart_template_data.xml",
    "data/account_data.xml",
    "data/tax_report_data.xml",
    "views/report_invoice.xml",
    "wizard/account_fr_fec_export_wizard_view.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "data/l10n_fr_account_demo.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fr_account/__init__.py` (24 lines)
- `addons/l10n_fr_account/__manifest__.py` (51 lines)
- `addons/l10n_fr_account/data/account_chart_template_data.xml` (17 lines)
- `addons/l10n_fr_account/data/account_data.xml` (27 lines)
- `addons/l10n_fr_account/data/l10n_fr_account_demo.xml` (9 lines)
- `addons/l10n_fr_account/data/tax_report_data.xml` (2,931 lines)
- `addons/l10n_fr_account/data/template/account.account-fr.csv` (236 lines)
- `addons/l10n_fr_account/data/template/account.account-fr_asso.csv` (270 lines)
- `addons/l10n_fr_account/data/template/account.account-fr_comp.csv` (437 lines)
- `addons/l10n_fr_account/data/template/account.depreciation.model-fr_comp.csv` (7 lines)
- `addons/l10n_fr_account/data/template/account.fiscal.position-fr.csv` (11 lines)
- `addons/l10n_fr_account/data/template/account.tax-fr.csv` (227 lines)
- `addons/l10n_fr_account/data/template/account.tax.group-fr.csv` (7 lines)
- `addons/l10n_fr_account/i18n/fr.po` (460 lines)
- `addons/l10n_fr_account/i18n/l10n_fr_account.pot` (430 lines)
- `addons/l10n_fr_account/migrations/2.2/pre-migrate-add-bank-xmlid.py` (30 lines)
- `addons/l10n_fr_account/models/__init__.py` (14 lines)
- `addons/l10n_fr_account/models/account_move.py` (29 lines)
- `addons/l10n_fr_account/models/base_document_layout.py` (16 lines)
- `addons/l10n_fr_account/models/res_company.py` (13 lines)
- `addons/l10n_fr_account/models/res_partner.py` (55 lines)
- `addons/l10n_fr_account/models/template_fr.py` (63 lines)
- `addons/l10n_fr_account/models/template_fr_asso.py` (42 lines)
- `addons/l10n_fr_account/models/template_fr_comp.py` (149 lines)
- `addons/l10n_fr_account/models/template_gf.py` (18 lines)
- `addons/l10n_fr_account/models/template_gp.py` (18 lines)
- `addons/l10n_fr_account/models/template_mc.py` (19 lines)
- `addons/l10n_fr_account/models/template_mq.py` (18 lines)
- `addons/l10n_fr_account/models/template_re.py` (18 lines)
- `addons/l10n_fr_account/models/template_yt.py` (18 lines)
- `addons/l10n_fr_account/security/ir.access.csv` (2 lines)
- `addons/l10n_fr_account/tests/__init__.py` (3 lines)
- `addons/l10n_fr_account/tests/test_fec_export.py` (181 lines)
- `addons/l10n_fr_account/tests/test_fr_tax_report.py` (49 lines)
- `addons/l10n_fr_account/tests/test_res_partner.py` (48 lines)
- `addons/l10n_fr_account/views/report_invoice.xml` (77 lines)
- `addons/l10n_fr_account/wizard/__init__.py` (4 lines)
- `addons/l10n_fr_account/wizard/account_fr_fec_export_wizard.py` (409 lines)
- `addons/l10n_fr_account/wizard/account_fr_fec_export_wizard_view.xml` (122 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
