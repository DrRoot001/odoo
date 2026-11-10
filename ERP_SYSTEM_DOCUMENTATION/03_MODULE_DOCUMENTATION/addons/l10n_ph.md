# Module: l10n_ph

- **Module ID:** MOD-292
- **Path:** `addons/l10n_ph`
- **Manifest:** `addons/l10n_ph/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['account']`
- **License:** `LGPL-3`

## Purpose and dependencies

This is the module to manage the accounting chart for The Philippines.

No manifest description declared.

Declared dependencies: `account`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 12 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 4 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/account_tax_report_data.xml",
    "data/menuitem_data.xml",
    "views/res_config_settings_views.xml",
    "views/account_tax_views.xml",
    "views/res_company_views.xml",
    "views/res_partner_views.xml",
    "views/report_disbursement_voucher_template.xml",
    "views/report_disbursement_voucher_internal_template.xml",
    "views/account_report.xml",
    "views/report_templates.xml",
    "views/report_invoice.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ph/__init__.py` (3 lines)
- `addons/l10n_ph/__manifest__.py` (33 lines)
- `addons/l10n_ph/data/account_tax_report_data.xml` (1,082 lines)
- `addons/l10n_ph/data/menuitem_data.xml` (4 lines)
- `addons/l10n_ph/data/template/account.account-ph.csv` (167 lines)
- `addons/l10n_ph/data/template/account.fiscal.position-ph.csv` (6 lines)
- `addons/l10n_ph/data/template/account.tax-ph.csv` (376 lines)
- `addons/l10n_ph/data/template/account.tax.group-ph.csv` (8 lines)
- `addons/l10n_ph/demo/demo_company.xml` (35 lines)
- `addons/l10n_ph/i18n/l10n_ph.pot` (847 lines)
- `addons/l10n_ph/i18n/tl.po` (851 lines)
- `addons/l10n_ph/migrations/1.1/end-migrate_update_taxes.py` (8 lines)
- `addons/l10n_ph/models/__init__.py` (9 lines)
- `addons/l10n_ph/models/account_move.py` (76 lines)
- `addons/l10n_ph/models/account_payment.py` (52 lines)
- `addons/l10n_ph/models/account_tax.py` (9 lines)
- `addons/l10n_ph/models/base_document_layout.py` (9 lines)
- `addons/l10n_ph/models/res_company.py` (14 lines)
- `addons/l10n_ph/models/res_config_settings.py` (14 lines)
- `addons/l10n_ph/models/res_partner.py` (145 lines)
- `addons/l10n_ph/models/template_ph.py` (58 lines)
- `addons/l10n_ph/tests/__init__.py` (5 lines)
- `addons/l10n_ph/tests/common.py` (84 lines)
- `addons/l10n_ph/tests/test_cas_invoice_report.py` (152 lines)
- `addons/l10n_ph/tests/test_partner_name.py` (90 lines)
- `addons/l10n_ph/views/account_report.xml` (21 lines)
- `addons/l10n_ph/views/account_tax_views.xml` (19 lines)
- `addons/l10n_ph/views/report_disbursement_voucher_internal_template.xml` (66 lines)
- `addons/l10n_ph/views/report_disbursement_voucher_template.xml` (141 lines)
- `addons/l10n_ph/views/report_invoice.xml` (160 lines)
- `addons/l10n_ph/views/report_templates.xml` (20 lines)
- `addons/l10n_ph/views/res_company_views.xml` (15 lines)
- `addons/l10n_ph/views/res_config_settings_views.xml` (30 lines)
- `addons/l10n_ph/views/res_partner_views.xml` (33 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
