# Module: l10n_ke_edi_tremol

- **Module ID:** MOD-251
- **Path:** `addons/l10n_ke_edi_tremol`
- **Manifest:** `addons/l10n_ke_edi_tremol/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Kenya Tremol Device EDI Integration


This module integrates with the Kenyan G03 Tremol control unit device to the KRA through TIMS.
    

Declared dependencies: `l10n_ke`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 13 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 3 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ke"
  ],
  "data": [
    "views/account_move_view.xml",
    "views/report_invoice.xml",
    "views/res_config_settings_view.xml",
    "views/res_partner_views.xml"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_ke_edi_tremol/static/src/components/*"
    ]
  }
}
```

### Representative source files

- `addons/l10n_ke_edi_tremol/__init__.py` (5 lines)
- `addons/l10n_ke_edi_tremol/__manifest__.py` (24 lines)
- `addons/l10n_ke_edi_tremol/data/neutralize.sql` (3 lines)
- `addons/l10n_ke_edi_tremol/i18n/l10n_ke_edi_tremol.pot` (375 lines)
- `addons/l10n_ke_edi_tremol/i18n/sw.po` (378 lines)
- `addons/l10n_ke_edi_tremol/models/__init__.py` (5 lines)
- `addons/l10n_ke_edi_tremol/models/account_move.py` (308 lines)
- `addons/l10n_ke_edi_tremol/models/account_move_send.py` (45 lines)
- `addons/l10n_ke_edi_tremol/models/res_company.py` (14 lines)
- `addons/l10n_ke_edi_tremol/models/res_config_settings.py` (10 lines)
- `addons/l10n_ke_edi_tremol/models/res_partner.py` (16 lines)
- `addons/l10n_ke_edi_tremol/static/src/components/ke_proxy_action.js` (20 lines)
- `addons/l10n_ke_edi_tremol/static/src/components/ke_proxy_dialog.js` (24 lines)
- `addons/l10n_ke_edi_tremol/static/src/components/ke_proxy_dialog.xml` (38 lines)
- `addons/l10n_ke_edi_tremol/static/src/components/ke_proxy_hook.js` (83 lines)
- `addons/l10n_ke_edi_tremol/tests/__init__.py` (4 lines)
- `addons/l10n_ke_edi_tremol/tests/test_account_move_send.py` (52 lines)
- `addons/l10n_ke_edi_tremol/tests/test_move_export.py` (296 lines)
- `addons/l10n_ke_edi_tremol/views/account_move_view.xml` (72 lines)
- `addons/l10n_ke_edi_tremol/views/report_invoice.xml` (32 lines)
- `addons/l10n_ke_edi_tremol/views/res_config_settings_view.xml` (27 lines)
- `addons/l10n_ke_edi_tremol/views/res_partner_views.xml` (15 lines)
- `addons/l10n_ke_edi_tremol/wizard/__init__.py` (1 lines)
- `addons/l10n_ke_edi_tremol/wizard/account_move_send_wizard.py` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
