# Module: l10n_fr_pdp_penalty_rate

- **Module ID:** MOD-195
- **Path:** `addons/l10n_fr_pdp_penalty_rate`
- **Manifest:** `addons/l10n_fr_pdp_penalty_rate/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `['l10n_fr_pdp']`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Adds the mandatory late payment penalty information to French invoices.


Declared dependencies: `l10n_fr_pdp`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_fr_pdp"
  ],
  "data": [
    "security/ir.access.csv",
    "views/account_invoice_report_templates.xml",
    "views/res_config_settings_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_fr_pdp_penalty_rate/__init__.py` (1 lines)
- `addons/l10n_fr_pdp_penalty_rate/__manifest__.py` (18 lines)
- `addons/l10n_fr_pdp_penalty_rate/i18n/l10n_fr_pdp_penalty_rate.pot` (179 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/__init__.py` (5 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/account_edi_common.py` (11 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/account_move.py` (79 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/late_payment_penalty_rate.py` (78 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/res_company.py` (43 lines)
- `addons/l10n_fr_pdp_penalty_rate/models/res_config_settings.py` (17 lines)
- `addons/l10n_fr_pdp_penalty_rate/security/ir.access.csv` (2 lines)
- `addons/l10n_fr_pdp_penalty_rate/tests/__init__.py` (2 lines)
- `addons/l10n_fr_pdp_penalty_rate/tests/test_late_payment_penalties.py` (472 lines)
- `addons/l10n_fr_pdp_penalty_rate/tests/test_pdp_notes.py` (26 lines)
- `addons/l10n_fr_pdp_penalty_rate/views/account_invoice_report_templates.xml` (13 lines)
- `addons/l10n_fr_pdp_penalty_rate/views/res_config_settings_views.xml` (35 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
