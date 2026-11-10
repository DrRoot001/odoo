# Module: l10n_jo_edi

- **Module ID:** MOD-246
- **Path:** `addons/l10n_jo_edi`
- **Manifest:** `addons/l10n_jo_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_jo']`
- **License:** `LGPL-3`

## Purpose and dependencies

Electronic Invoicing for Jordan UBL 2.1


       Allows the users to integrate with JoFotara.
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_jo`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 14 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 5 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_jo"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/report_invoice.xml",
    "views/report_templates.xml",
    "views/res_config_settings_views.xml"
  ],
  "demo": [
    "demo/demo_company.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_jo_edi/static/src/**/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_jo_edi/__init__.py` (8 lines)
- `addons/l10n_jo_edi/__manifest__.py` (28 lines)
- `addons/l10n_jo_edi/data/neutralize.sql` (4 lines)
- `addons/l10n_jo_edi/demo/demo_company.xml` (12 lines)
- `addons/l10n_jo_edi/i18n/ar.po` (619 lines)
- `addons/l10n_jo_edi/i18n/l10n_jo_edi.pot` (581 lines)
- `addons/l10n_jo_edi/models/__init__.py` (7 lines)
- `addons/l10n_jo_edi/models/account_edi_xml_ubl_21_jo.py` (488 lines)
- `addons/l10n_jo_edi/models/account_move.py` (311 lines)
- `addons/l10n_jo_edi/models/account_move_send.py` (120 lines)
- `addons/l10n_jo_edi/models/account_tax.py` (11 lines)
- `addons/l10n_jo_edi/models/ir_attachment.py` (20 lines)
- `addons/l10n_jo_edi/models/res_company.py` (64 lines)
- `addons/l10n_jo_edi/models/res_config_settings.py` (11 lines)
- `addons/l10n_jo_edi/static/src/jo_edi_error_dialog/jo_edi_error_dialog.js` (30 lines)
- `addons/l10n_jo_edi/static/src/jo_edi_error_dialog/jo_edi_error_dialog.xml` (23 lines)
- `addons/l10n_jo_edi/tests/__init__.py` (3 lines)
- `addons/l10n_jo_edi/tests/jo_edi_common.py` (102 lines)
- `addons/l10n_jo_edi/tests/test_files/type_1.xml` (97 lines)
- `addons/l10n_jo_edi/tests/test_files/type_2.xml` (108 lines)
- `addons/l10n_jo_edi/tests/test_files/type_3.xml` (115 lines)
- `addons/l10n_jo_edi/tests/test_files/type_4.xml` (137 lines)
- `addons/l10n_jo_edi/tests/test_files/type_5.xml` (124 lines)
- `addons/l10n_jo_edi/tests/test_files/type_6.xml` (135 lines)
- `addons/l10n_jo_edi/tests/test_files/type_7.xml` (96 lines)
- `addons/l10n_jo_edi/tests/test_files/type_8.xml` (94 lines)
- `addons/l10n_jo_edi/tests/test_jo_edi_invoice_codes.py` (68 lines)
- `addons/l10n_jo_edi/tests/test_jo_edi_precision.py` (437 lines)
- `addons/l10n_jo_edi/tests/test_jo_edi_types.py` (363 lines)
- `addons/l10n_jo_edi/views/account_move_views.xml` (72 lines)
- `addons/l10n_jo_edi/views/report_invoice.xml` (34 lines)
- `addons/l10n_jo_edi/views/report_templates.xml` (44 lines)
- `addons/l10n_jo_edi/views/res_config_settings_views.xml` (46 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
