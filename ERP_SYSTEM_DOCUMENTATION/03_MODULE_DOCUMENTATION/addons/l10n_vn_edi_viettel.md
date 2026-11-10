# Module: l10n_vn_edi_viettel

- **Module ID:** MOD-342
- **Path:** `addons/l10n_vn_edi_viettel`
- **Manifest:** `addons/l10n_vn_edi_viettel/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

E-invoicing using SInvoice by Viettel


Vietnam - E-invoicing
=====================
Using SInvoice by Viettel
    

Declared dependencies: `l10n_vn`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 16 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_vn"
  ],
  "data": [
    "views/account_move_views.xml",
    "views/account_journal_views.xml",
    "views/sinvoice_views.xml",
    "views/res_config_settings_views.xml",
    "wizard/account_move_reversal_view.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_vn_edi_viettel/__init__.py` (8 lines)
- `addons/l10n_vn_edi_viettel/__manifest__.py` (28 lines)
- `addons/l10n_vn_edi_viettel/data/neutralize.sql` (4 lines)
- `addons/l10n_vn_edi_viettel/i18n/l10n_vn_edi_viettel.pot` (678 lines)
- `addons/l10n_vn_edi_viettel/i18n/vi.po` (683 lines)
- `addons/l10n_vn_edi_viettel/models/__init__.py` (10 lines)
- `addons/l10n_vn_edi_viettel/models/account_journal.py` (13 lines)
- `addons/l10n_vn_edi_viettel/models/account_move.py` (668 lines)
- `addons/l10n_vn_edi_viettel/models/account_move_send.py` (143 lines)
- `addons/l10n_vn_edi_viettel/models/res_company.py` (80 lines)
- `addons/l10n_vn_edi_viettel/models/res_config_settings.py` (31 lines)
- `addons/l10n_vn_edi_viettel/models/res_partner.py` (9 lines)
- `addons/l10n_vn_edi_viettel/models/sinvoice.py` (160 lines)
- `addons/l10n_vn_edi_viettel/models/sinvoice_service.py` (307 lines)
- `addons/l10n_vn_edi_viettel/security/ir.access.csv` (4 lines)
- `addons/l10n_vn_edi_viettel/tests/__init__.py` (4 lines)
- `addons/l10n_vn_edi_viettel/tests/test_edi.py` (821 lines)
- `addons/l10n_vn_edi_viettel/tests/test_sinvoice.py` (120 lines)
- `addons/l10n_vn_edi_viettel/views/account_journal_views.xml` (17 lines)
- `addons/l10n_vn_edi_viettel/views/account_move_views.xml` (91 lines)
- `addons/l10n_vn_edi_viettel/views/res_config_settings_views.xml` (45 lines)
- `addons/l10n_vn_edi_viettel/views/sinvoice_views.xml` (68 lines)
- `addons/l10n_vn_edi_viettel/wizard/__init__.py` (3 lines)
- `addons/l10n_vn_edi_viettel/wizard/account_move_reversal.py` (77 lines)
- `addons/l10n_vn_edi_viettel/wizard/account_move_reversal_view.xml` (17 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
