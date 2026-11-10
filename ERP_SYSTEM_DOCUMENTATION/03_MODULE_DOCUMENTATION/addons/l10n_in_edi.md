# Module: l10n_in_edi

- **Module ID:** MOD-229
- **Path:** `addons/l10n_in_edi`
- **Manifest:** `addons/l10n_in_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Indian - E-invoicing
====================
To submit invoicing through API to the government.
We use "Tera Software Limited" as GSP
Step 1: First you need to create an API username and password in the E-invoice portal.
Step 2: Switch to company related to that GST number
Step 3: Set that username and password in Odoo (Goto: Invoicing/Accounting -> Configuration -> Settings -> Customer Invoices or find "E-invoice" in search bar)
Step 4: Repeat steps 1,2,3 for all GSTIN you have in odoo. If you have a multi-company with the same GST number then perform step 1 for the first company only.
For the creation of API username and password please ref this document: <https://service.odoo.co.in/einvoice_create_api_user>
    

Declared dependencies: `l10n_in`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_in"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/edi_pdf_report.xml",
    "views/res_config_settings_views.xml",
    "views/account_journal_dashboard_views.xml",
    "wizard/l10n_in_edi_cancel_views.xml",
    "security/ir.access.csv"
  ],
  "demo": [
    "demo/demo_company.xml"
  ]
}
```

### Representative source files

- `addons/l10n_in_edi/__init__.py` (2 lines)
- `addons/l10n_in_edi/__manifest__.py` (33 lines)
- `addons/l10n_in_edi/data/neutralize.sql` (6 lines)
- `addons/l10n_in_edi/demo/demo_company.xml` (9 lines)
- `addons/l10n_in_edi/i18n/hi.po` (672 lines)
- `addons/l10n_in_edi/i18n/l10n_in_edi.pot` (661 lines)
- `addons/l10n_in_edi/models/__init__.py` (8 lines)
- `addons/l10n_in_edi/models/account_journal.py` (30 lines)
- `addons/l10n_in_edi/models/account_move.py` (848 lines)
- `addons/l10n_in_edi/models/account_move_line.py` (60 lines)
- `addons/l10n_in_edi/models/account_move_send.py` (65 lines)
- `addons/l10n_in_edi/models/ir_attachment.py` (21 lines)
- `addons/l10n_in_edi/models/res_company.py` (100 lines)
- `addons/l10n_in_edi/models/res_config_settings.py` (52 lines)
- `addons/l10n_in_edi/models/res_partner.py` (56 lines)
- `addons/l10n_in_edi/security/ir.access.csv` (2 lines)
- `addons/l10n_in_edi/tests/__init__.py` (1 lines)
- `addons/l10n_in_edi/tests/test_edi_json.py` (916 lines)
- `addons/l10n_in_edi/views/account_journal_dashboard_views.xml` (19 lines)
- `addons/l10n_in_edi/views/account_move_views.xml` (91 lines)
- `addons/l10n_in_edi/views/edi_pdf_report.xml` (25 lines)
- `addons/l10n_in_edi/views/res_config_settings_views.xml` (28 lines)
- `addons/l10n_in_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_in_edi/wizard/l10n_in_edi_cancel.py` (25 lines)
- `addons/l10n_in_edi/wizard/l10n_in_edi_cancel_views.xml` (29 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
