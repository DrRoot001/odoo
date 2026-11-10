# Module: l10n_in_ewaybill_irn

- **Module ID:** MOD-231
- **Path:** `addons/l10n_in_ewaybill_irn`
- **Manifest:** `addons/l10n_in_ewaybill_irn/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Indian - E-waybill thru IRN
====================================
This module enables to generate E-waybill through IRN.
    

Declared dependencies: `l10n_in_ewaybill`, `l10n_in_edi`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 6 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
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
    "l10n_in_ewaybill",
    "l10n_in_edi"
  ],
  "data": [
    "views/l10n_in_ewaybill_views.xml",
    "report/ewaybill_report.xml"
  ]
}
```

### Representative source files

- `addons/l10n_in_ewaybill_irn/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill_irn/__manifest__.py` (22 lines)
- `addons/l10n_in_ewaybill_irn/i18n/hi.po` (84 lines)
- `addons/l10n_in_ewaybill_irn/i18n/l10n_in_ewaybill_irn.pot` (80 lines)
- `addons/l10n_in_ewaybill_irn/models/__init__.py` (3 lines)
- `addons/l10n_in_ewaybill_irn/models/l10n_in_ewaybill.py` (152 lines)
- `addons/l10n_in_ewaybill_irn/report/ewaybill_report.xml` (10 lines)
- `addons/l10n_in_ewaybill_irn/tests/__init__.py` (1 lines)
- `addons/l10n_in_ewaybill_irn/tests/test_ewaybill_irn.py` (144 lines)
- `addons/l10n_in_ewaybill_irn/views/l10n_in_ewaybill_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
