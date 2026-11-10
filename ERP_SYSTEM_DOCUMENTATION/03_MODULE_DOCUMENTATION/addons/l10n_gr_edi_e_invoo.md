# Module: l10n_gr_edi_e_invoo

- **Module ID:** MOD-210
- **Path:** `addons/l10n_gr_edi_e_invoo`
- **Manifest:** `addons/l10n_gr_edi_e_invoo/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_gr_edi']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `account_edi_proxy_client`, `l10n_gr_edi`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
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
    "account_edi_proxy_client",
    "l10n_gr_edi"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/report_invoice.xml"
  ]
}
```

### Representative source files

- `addons/l10n_gr_edi_e_invoo/__init__.py` (1 lines)
- `addons/l10n_gr_edi_e_invoo/__manifest__.py` (18 lines)
- `addons/l10n_gr_edi_e_invoo/data/neutralize.sql` (3 lines)
- `addons/l10n_gr_edi_e_invoo/i18n/el.po` (264 lines)
- `addons/l10n_gr_edi_e_invoo/i18n/l10n_gr_edi_e_invoo.pot` (263 lines)
- `addons/l10n_gr_edi_e_invoo/models/__init__.py` (5 lines)
- `addons/l10n_gr_edi_e_invoo/models/account_edi_proxy_user.py` (56 lines)
- `addons/l10n_gr_edi_e_invoo/models/account_move.py` (325 lines)
- `addons/l10n_gr_edi_e_invoo/models/account_move_send.py` (75 lines)
- `addons/l10n_gr_edi_e_invoo/models/l10n_gr_edi_document.py` (36 lines)
- `addons/l10n_gr_edi_e_invoo/models/res_company.py` (23 lines)
- `addons/l10n_gr_edi_e_invoo/tests/__init__.py` (1 lines)
- `addons/l10n_gr_edi_e_invoo/tests/test_e_invoo.py` (222 lines)
- `addons/l10n_gr_edi_e_invoo/views/account_move_views.xml` (13 lines)
- `addons/l10n_gr_edi_e_invoo/views/report_invoice.xml` (64 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
