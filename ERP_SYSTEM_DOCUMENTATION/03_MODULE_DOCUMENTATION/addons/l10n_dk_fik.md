# Module: l10n_dk_fik

- **Module ID:** MOD-165
- **Path:** `addons/l10n_dk_fik`
- **Manifest:** `addons/l10n_dk_fik/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Use FIK Number as Payment reference


Support Danish FIK number as payment references on customer invoices.


Declared dependencies: `l10n_dk`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 0 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_dk"
  ],
  "data": [
    "views/account_journal_view.xml"
  ]
}
```

### Representative source files

- `addons/l10n_dk_fik/__init__.py` (1 lines)
- `addons/l10n_dk_fik/__manifest__.py` (17 lines)
- `addons/l10n_dk_fik/i18n/da.po` (105 lines)
- `addons/l10n_dk_fik/i18n/l10n_dk_fik.pot` (96 lines)
- `addons/l10n_dk_fik/models/__init__.py` (2 lines)
- `addons/l10n_dk_fik/models/account_journal.py` (53 lines)
- `addons/l10n_dk_fik/models/account_move.py` (34 lines)
- `addons/l10n_dk_fik/views/account_journal_view.xml` (15 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
