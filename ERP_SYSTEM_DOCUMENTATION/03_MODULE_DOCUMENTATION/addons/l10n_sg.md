# Module: l10n_sg

- **Module ID:** MOD-315
- **Path:** `addons/l10n_sg`
- **Manifest:** `addons/l10n_sg/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Singapore accounting chart and localization.
=======================================================

This module add, for accounting:
 - The Chart of Accounts of Singapore
 - Field UEN (Unique Entity Number) on company and partner
 - Field PermitNo and PermitNoDate on invoice

    

Declared dependencies: `account_qr_code_emv`, `account`, `account_edi_ubl_cii`, `account_peppol`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_qr_code_emv",
    "account",
    "account_edi_ubl_cii",
    "account_peppol"
  ],
  "data": [
    "data/account.account.tag.csv",
    "data/l10n_sg_chart_data.xml",
    "data/account_tax_report_data.xml",
    "views/account_invoice_view.xml",
    "views/report_invoice.xml",
    "views/report_templates.xml",
    "views/res_bank_views.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_sg/__init__.py` (16 lines)
- `addons/l10n_sg/__manifest__.py` (43 lines)
- `addons/l10n_sg/data/account.account.tag.csv` (5 lines)
- `addons/l10n_sg/data/account_tax_report_data.xml` (278 lines)
- `addons/l10n_sg/data/l10n_sg_chart_data.xml` (4 lines)
- `addons/l10n_sg/data/template/account.account-sg.csv` (224 lines)
- `addons/l10n_sg/data/template/account.depreciation.model-sg.csv` (7 lines)
- `addons/l10n_sg/data/template/account.fiscal.position-sg.csv` (3 lines)
- `addons/l10n_sg/data/template/account.tax-sg.csv` (150 lines)
- `addons/l10n_sg/data/template/account.tax.group-sg.csv` (6 lines)
- `addons/l10n_sg/demo/demo_company.xml` (36 lines)
- `addons/l10n_sg/migrations/2.1/end-migrate_update_tax.py` (8 lines)
- `addons/l10n_sg/migrations/2.2/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_sg/migrations/2.3/end-reactivate_rc_child_taxes.py` (17 lines)
- `addons/l10n_sg/migrations/9.0.2.0/pre-set_tags_and_taxes_updatable.py` (6 lines)
- `addons/l10n_sg/models/__init__.py` (9 lines)
- `addons/l10n_sg/models/account_edi_proxy_user.py` (21 lines)
- `addons/l10n_sg/models/account_move.py` (61 lines)
- `addons/l10n_sg/models/account_tax.py` (49 lines)
- `addons/l10n_sg/models/base_document_layout.py` (7 lines)
- `addons/l10n_sg/models/res_bank.py` (68 lines)
- `addons/l10n_sg/models/res_company.py` (24 lines)
- `addons/l10n_sg/models/res_partner.py` (26 lines)
- `addons/l10n_sg/models/template_sg.py` (75 lines)
- `addons/l10n_sg/tests/__init__.py` (3 lines)
- `addons/l10n_sg/tests/test_l10n_sg_customer_accounting.py` (83 lines)
- `addons/l10n_sg/tests/test_l10n_sg_emv_qr.py` (80 lines)
- `addons/l10n_sg/tests/test_l10n_sg_reverse_charge_tax.py` (53 lines)
- `addons/l10n_sg/views/account_invoice_view.xml` (16 lines)
- `addons/l10n_sg/views/report_invoice.xml` (63 lines)
- `addons/l10n_sg/views/report_templates.xml` (10 lines)
- `addons/l10n_sg/views/res_bank_views.xml` (17 lines)
- `addons/l10n_sg/views/res_config_settings_views.xml` (25 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
