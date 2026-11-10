# Module: l10n_in_ewaybill

- **Module ID:** MOD-230
- **Path:** `addons/l10n_in_ewaybill`
- **Manifest:** `addons/l10n_in_ewaybill/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Indian - E-waybill
====================================
To submit E-waybill through API to the government.
We use "Tera Software Limited" as GSP

Step 1: First you need to create an API username and password in the E-waybill portal.
Step 2: Switch to company related to that GST number
Step 3: Set that username and password in Odoo (Goto: Invoicing/Accounting -> Configration -> Settings -> Indian Electronic WayBill or find "E-waybill" in search bar)
Step 4: Repeat steps 1,2,3 for all GSTIN you have in odoo. If you have a multi-company with the same GST number then perform step 1 for the first company only.
    

Declared dependencies: `l10n_in`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 18 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
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
    "data/ewaybill_type_data.xml",
    "views/l10n_in_ewaybill_views.xml",
    "views/account_move_views.xml",
    "views/edi_pdf_report.xml",
    "views/res_config_settings_views.xml",
    "wizard/l10n_in_ewaybill_cancel_views.xml",
    "report/ewaybill_report_views.xml",
    "report/ewaybill_report.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_in_ewaybill/__init__.py` (5 lines)
- `addons/l10n_in_ewaybill/__manifest__.py` (37 lines)
- `addons/l10n_in_ewaybill/data/ewaybill_type_data.xml` (75 lines)
- `addons/l10n_in_ewaybill/data/neutralize.sql` (5 lines)
- `addons/l10n_in_ewaybill/demo/__init__.py` (2 lines)
- `addons/l10n_in_ewaybill/demo/account_demo.py` (47 lines)
- `addons/l10n_in_ewaybill/i18n/hi.po` (3,322 lines)
- `addons/l10n_in_ewaybill/i18n/l10n_in_ewaybill.pot` (3,309 lines)
- `addons/l10n_in_ewaybill/models/__init__.py` (8 lines)
- `addons/l10n_in_ewaybill/models/account_move.py` (58 lines)
- `addons/l10n_in_ewaybill/models/error_codes.py` (337 lines)
- `addons/l10n_in_ewaybill/models/ewaybill_type.py` (32 lines)
- `addons/l10n_in_ewaybill/models/ir_attachment.py` (19 lines)
- `addons/l10n_in_ewaybill/models/l10n_in_ewaybill.py` (790 lines)
- `addons/l10n_in_ewaybill/models/res_company.py` (19 lines)
- `addons/l10n_in_ewaybill/models/res_config_settings.py` (51 lines)
- `addons/l10n_in_ewaybill/report/ewaybill_report.xml` (284 lines)
- `addons/l10n_in_ewaybill/report/ewaybill_report_views.xml` (32 lines)
- `addons/l10n_in_ewaybill/security/ir.access.csv` (6 lines)
- `addons/l10n_in_ewaybill/tests/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill/tests/test_ewaybill_json.py` (544 lines)
- `addons/l10n_in_ewaybill/tools/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill/tools/ewaybill_api.py` (209 lines)
- `addons/l10n_in_ewaybill/views/account_move_views.xml` (47 lines)
- `addons/l10n_in_ewaybill/views/edi_pdf_report.xml` (17 lines)
- `addons/l10n_in_ewaybill/views/l10n_in_ewaybill_views.xml` (182 lines)
- `addons/l10n_in_ewaybill/views/res_config_settings_views.xml` (36 lines)
- `addons/l10n_in_ewaybill/wizard/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill/wizard/l10n_in_ewaybill_cancel.py` (26 lines)
- `addons/l10n_in_ewaybill/wizard/l10n_in_ewaybill_cancel_views.xml` (30 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
