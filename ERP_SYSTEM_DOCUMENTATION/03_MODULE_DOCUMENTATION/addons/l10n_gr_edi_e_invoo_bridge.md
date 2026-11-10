# Module: l10n_gr_edi_e_invoo_bridge

- **Module ID:** MOD-211
- **Path:** `addons/l10n_gr_edi_e_invoo_bridge`
- **Manifest:** `addons/l10n_gr_edi_e_invoo_bridge/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `l10n_gr_edi`, `l10n_gr_edi_e_invoo`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_gr_edi",
    "l10n_gr_edi_e_invoo"
  ],
  "data": [
    "views/res_company_views.xml",
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_gr_edi_e_invoo_bridge/__init__.py` (2 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/__manifest__.py` (15 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/data/neutralize.sql` (2 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/exceptions.py` (13 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/i18n/el.po` (114 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/i18n/l10n_gr_edi_e_invoo_bridge.pot` (114 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/models/__init__.py` (4 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/models/account_move.py` (139 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/models/account_move_send.py` (68 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/models/res_company.py` (11 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/models/res_config_settings.py` (10 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/tests/__init__.py` (1 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/tests/test_e_invoo_bridge.py` (296 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/views/res_company_views.xml` (13 lines)
- `addons/l10n_gr_edi_e_invoo_bridge/views/res_config_settings_views.xml` (16 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
