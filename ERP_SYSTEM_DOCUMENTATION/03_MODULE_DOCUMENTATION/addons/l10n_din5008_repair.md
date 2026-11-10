# Module: l10n_din5008_repair

- **Module ID:** MOD-161
- **Path:** `addons/l10n_din5008_repair`
- **Manifest:** `addons/l10n_din5008_repair/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

No manifest description declared.

Declared dependencies: `l10n_din5008`, `repair`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 4 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 2 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 2 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_din5008",
    "repair"
  ],
  "data": [
    "report/din5008_repair_templates.xml",
    "report/din5008_repair_order_layout.xml"
  ]
}
```

### Representative source files

- `addons/l10n_din5008_repair/__init__.py` (1 lines)
- `addons/l10n_din5008_repair/__manifest__.py` (17 lines)
- `addons/l10n_din5008_repair/i18n/de.po` (72 lines)
- `addons/l10n_din5008_repair/i18n/fr.po` (71 lines)
- `addons/l10n_din5008_repair/i18n/it.po` (72 lines)
- `addons/l10n_din5008_repair/i18n/l10n_din5008_repair.pot` (67 lines)
- `addons/l10n_din5008_repair/models/__init__.py` (1 lines)
- `addons/l10n_din5008_repair/models/repair.py` (7 lines)
- `addons/l10n_din5008_repair/report/din5008_repair_order_layout.xml` (18 lines)
- `addons/l10n_din5008_repair/report/din5008_repair_templates.xml` (32 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
