# Module: l10n_hr_edi

- **Module ID:** MOD-217
- **Path:** `addons/l10n_hr_edi`
- **Manifest:** `addons/l10n_hr_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


e-invoicing for Croatia
    

Declared dependencies: `l10n_hr`, `account_edi_ubl_cii`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 26 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 14 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 20 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 6 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_hr",
    "account_edi_ubl_cii"
  ],
  "data": [
    "data/cron.xml",
    "data/l10n_hr.kpd.category.csv",
    "data/l10n_hr_tax_category.xml",
    "views/account_journal_views.xml",
    "views/account_move_views.xml",
    "views/account_tax_views.xml",
    "views/l10n_hr_kpd_category_views.xml",
    "views/product_views.xml",
    "views/report_invoice_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "wizard/l10n_hr_edi_mojeracun_reject_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_hr_edi/__init__.py` (16 lines)
- `addons/l10n_hr_edi/__manifest__.py` (33 lines)
- `addons/l10n_hr_edi/data/cron.xml` (29 lines)
- `addons/l10n_hr_edi/data/l10n_hr.kpd.category.csv` (3,359 lines)
- `addons/l10n_hr_edi/data/l10n_hr_tax_category.xml` (111 lines)
- `addons/l10n_hr_edi/data/neutralize.sql` (8 lines)
- `addons/l10n_hr_edi/data/template/account.tax-hr.csv` (16 lines)
- `addons/l10n_hr_edi/demo/demo_company.xml` (13 lines)
- `addons/l10n_hr_edi/i18n/hr.po` (1,293 lines)
- `addons/l10n_hr_edi/i18n/l10n_hr_edi.pot` (1,290 lines)
- `addons/l10n_hr_edi/models/__init__.py` (13 lines)
- `addons/l10n_hr_edi/models/account_chart_template.py` (11 lines)
- `addons/l10n_hr_edi/models/account_edi_xml_ubl_hr.py` (420 lines)
- `addons/l10n_hr_edi/models/account_journal.py` (49 lines)
- `addons/l10n_hr_edi/models/account_move.py` (297 lines)
- `addons/l10n_hr_edi/models/account_move_line.py` (21 lines)
- `addons/l10n_hr_edi/models/account_move_send.py` (131 lines)
- `addons/l10n_hr_edi/models/account_tax.py` (19 lines)
- `addons/l10n_hr_edi/models/l10n_hr_edi_addendum.py` (84 lines)
- `addons/l10n_hr_edi/models/product_template.py` (25 lines)
- `addons/l10n_hr_edi/models/res_company.py` (391 lines)
- `addons/l10n_hr_edi/models/res_config_settings.py` (27 lines)
- `addons/l10n_hr_edi/models/res_partner.py` (46 lines)
- `addons/l10n_hr_edi/models/sequence_mixin.py` (118 lines)
- `addons/l10n_hr_edi/security/ir.access.csv` (8 lines)
- `addons/l10n_hr_edi/tests/__init__.py` (5 lines)
- `addons/l10n_hr_edi/tests/flows/in_invoice.xml` (345 lines)
- `addons/l10n_hr_edi/tests/flows/out_invoice.xml` (186 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice.xml` (182 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice_cash_basis.xml` (183 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice_exemption_e.xml` (188 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice_exemption_k.xml` (185 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice_multiple.xml` (275 lines)
- `addons/l10n_hr_edi/tests/test_files/test_invoice_refund.xml` (181 lines)
- `addons/l10n_hr_edi/tests/test_flows.py` (397 lines)
- `addons/l10n_hr_edi/tests/test_hr_edi_common.py` (78 lines)
- `addons/l10n_hr_edi/tests/test_mer_api.py` (291 lines)
- `addons/l10n_hr_edi/tests/test_payment_unreported.py` (26 lines)
- `addons/l10n_hr_edi/tests/test_ubl_hr.py` (367 lines)
- `addons/l10n_hr_edi/tools/__init__.py` (1 lines)
- `addons/l10n_hr_edi/tools/api.py` (301 lines)
- `addons/l10n_hr_edi/views/account_journal_views.xml` (53 lines)
- `addons/l10n_hr_edi/views/account_move_views.xml` (206 lines)
- `addons/l10n_hr_edi/views/account_tax_views.xml` (13 lines)
- `addons/l10n_hr_edi/views/l10n_hr_kpd_category_views.xml` (28 lines)
- `addons/l10n_hr_edi/views/product_views.xml` (13 lines)
- `addons/l10n_hr_edi/views/report_invoice_views.xml` (46 lines)
- `addons/l10n_hr_edi/views/res_config_settings_views.xml` (69 lines)
- `addons/l10n_hr_edi/views/res_partner_views.xml` (14 lines)
- `addons/l10n_hr_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_hr_edi/wizard/l10n_hr_edi_mojeracun_reject_wizard.py` (65 lines)
- `addons/l10n_hr_edi/wizard/l10n_hr_edi_mojeracun_reject_wizard_views.xml` (27 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
