# Module: l10n_mt_pos

- **Module ID:** MOD-275
- **Path:** `addons/l10n_mt_pos`
- **Manifest:** `addons/l10n_mt_pos/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Malta Compliance Letter for EXO Number

Declared dependencies: `point_of_sale`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "point_of_sale"
  ],
  "data": [
    "wizards/compliance_letter_view.xml",
    "reports/compliance_letter_report.xml",
    "security/ir.access.csv"
  ]
}
```

### Representative source files

- `addons/l10n_mt_pos/__init__.py` (2 lines)
- `addons/l10n_mt_pos/__manifest__.py` (18 lines)
- `addons/l10n_mt_pos/reports/compliance_letter_report.xml` (49 lines)
- `addons/l10n_mt_pos/security/ir.access.csv` (2 lines)
- `addons/l10n_mt_pos/wizards/__init__.py` (1 lines)
- `addons/l10n_mt_pos/wizards/compliance_letter.py` (32 lines)
- `addons/l10n_mt_pos/wizards/compliance_letter_view.xml` (26 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
