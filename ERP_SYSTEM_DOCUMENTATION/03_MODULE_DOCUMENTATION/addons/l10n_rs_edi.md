# Module: l10n_rs_edi

- **Module ID:** MOD-308
- **Path:** `addons/l10n_rs_edi`
- **Manifest:** `addons/l10n_rs_edi/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

E-Invoice implementation for Serbia


eFaktura E-invoice implementation for Serbia
    

Declared dependencies: `account_edi_ubl_cii`, `l10n_rs`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 7 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "account_edi_ubl_cii",
    "l10n_rs"
  ],
  "data": [
    "views/res_config_settings_views.xml",
    "views/account_move.xml",
    "views/res_partner_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_rs_edi/__init__.py` (2 lines)
- `addons/l10n_rs_edi/__manifest__.py` (21 lines)
- `addons/l10n_rs_edi/data/neutralize.sql` (3 lines)
- `addons/l10n_rs_edi/i18n/l10n_rs_edi.pot` (348 lines)
- `addons/l10n_rs_edi/i18n/sr@latin.po` (362 lines)
- `addons/l10n_rs_edi/models/__init__.py` (6 lines)
- `addons/l10n_rs_edi/models/account_edi_xml_ubl_21_rs.py` (60 lines)
- `addons/l10n_rs_edi/models/account_move.py` (179 lines)
- `addons/l10n_rs_edi/models/account_move_send.py` (50 lines)
- `addons/l10n_rs_edi/models/res_company.py` (8 lines)
- `addons/l10n_rs_edi/models/res_config_settings.py` (8 lines)
- `addons/l10n_rs_edi/models/res_partner.py` (31 lines)
- `addons/l10n_rs_edi/tests/__init__.py` (1 lines)
- `addons/l10n_rs_edi/tests/test_files/export_credit_note.xml` (234 lines)
- `addons/l10n_rs_edi/tests/test_files/export_invoice.xml` (236 lines)
- `addons/l10n_rs_edi/tests/test_xml_ubl_rs.py` (90 lines)
- `addons/l10n_rs_edi/views/account_move.xml` (51 lines)
- `addons/l10n_rs_edi/views/res_config_settings_views.xml` (27 lines)
- `addons/l10n_rs_edi/views/res_partner_views.xml` (14 lines)
- `addons/l10n_rs_edi/wizard/__init__.py` (1 lines)
- `addons/l10n_rs_edi/wizard/account_move_send_wizard.py` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
