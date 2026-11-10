# Module: l10n_gr_edi

- **Module ID:** MOD-208
- **Path:** `addons/l10n_gr_edi`
- **Manifest:** `addons/l10n_gr_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Connect to myDATA API implementation for Greece


        myDATA is a platform created by Greece's tax authority,
        The Independent Authority for Public Revenue (IAPR),
        to digitize business tax and accounting information declaration.
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_gr`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 21 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 13 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 16 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_gr"
  ],
  "data": [
    "data/ir_cron.xml",
    "data/template.xml",
    "views/account_fiscal_position_views.xml",
    "views/account_move_views.xml",
    "views/account_tax_views.xml",
    "views/product_template_views.xml",
    "views/report_invoice.xml",
    "views/res_company_views.xml",
    "views/res_config_settings_views.xml",
    "views/res_partner_views.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_gr_edi/__init__.py` (2 lines)
- `addons/l10n_gr_edi/__manifest__.py` (29 lines)
- `addons/l10n_gr_edi/data/ir_cron.xml` (15 lines)
- `addons/l10n_gr_edi/data/neutralize.sql` (3 lines)
- `addons/l10n_gr_edi/data/template.xml` (143 lines)
- `addons/l10n_gr_edi/i18n/el.po` (2,345 lines)
- `addons/l10n_gr_edi/i18n/l10n_gr_edi.pot` (2,347 lines)
- `addons/l10n_gr_edi/models/__init__.py` (12 lines)
- `addons/l10n_gr_edi/models/account_edi_xml_ubl_gr.py` (156 lines)
- `addons/l10n_gr_edi/models/account_fiscal_position.py` (11 lines)
- `addons/l10n_gr_edi/models/account_move.py` (703 lines)
- `addons/l10n_gr_edi/models/account_move_line.py` (222 lines)
- `addons/l10n_gr_edi/models/account_move_send.py` (85 lines)
- `addons/l10n_gr_edi/models/account_tax.py` (26 lines)
- `addons/l10n_gr_edi/models/l10n_gr_edi_document.py` (219 lines)
- `addons/l10n_gr_edi/models/preferred_classification.py` (981 lines)
- `addons/l10n_gr_edi/models/product_template.py` (16 lines)
- `addons/l10n_gr_edi/models/res_company.py` (127 lines)
- `addons/l10n_gr_edi/models/res_config_settings.py` (10 lines)
- `addons/l10n_gr_edi/models/res_partner.py` (58 lines)
- `addons/l10n_gr_edi/security/ir.access.csv` (4 lines)
- `addons/l10n_gr_edi/tests/__init__.py` (2 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/grcius_out_invoice.xml` (178 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/grcius_out_refund.xml` (176 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/mydata_cls_expense.xml` (22 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/mydata_invoice.xml` (71 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/mydata_invoice_11_2.xml` (48 lines)
- `addons/l10n_gr_edi/tests/test_files/from_odoo/mydata_multi_invoices.xml` (98 lines)
- `addons/l10n_gr_edi/tests/test_mydata_invoice.py` (312 lines)
- `addons/l10n_gr_edi/tests/test_xml_ubl_gr.py` (116 lines)
- `addons/l10n_gr_edi/utils.py` (29 lines)
- `addons/l10n_gr_edi/views/account_fiscal_position_views.xml` (33 lines)
- `addons/l10n_gr_edi/views/account_move_views.xml` (189 lines)
- `addons/l10n_gr_edi/views/account_tax_views.xml` (15 lines)
- `addons/l10n_gr_edi/views/product_template_views.xml` (36 lines)
- `addons/l10n_gr_edi/views/report_invoice.xml` (32 lines)
- `addons/l10n_gr_edi/views/res_company_views.xml` (23 lines)
- `addons/l10n_gr_edi/views/res_config_settings_views.xml` (42 lines)
- `addons/l10n_gr_edi/views/res_partner_views.xml` (17 lines)
- `addons/l10n_gr_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_gr_edi/wizard/account_move_reversal.py` (12 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
