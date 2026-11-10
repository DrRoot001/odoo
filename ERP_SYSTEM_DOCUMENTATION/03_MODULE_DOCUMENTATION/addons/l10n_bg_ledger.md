# Module: l10n_bg_ledger

- **Module ID:** MOD-134
- **Path:** `addons/l10n_bg_ledger`
- **Manifest:** `addons/l10n_bg_ledger/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Report ledger for Bulgaria
    

Declared dependencies: `l10n_bg`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 5 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
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
    "l10n_bg"
  ],
  "data": [
    "views/account_journal_views.xml",
    "views/account_move_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_bg_ledger/__init__.py` (2 lines)
- `addons/l10n_bg_ledger/__manifest__.py` (20 lines)
- `addons/l10n_bg_ledger/i18n/bg.po` (141 lines)
- `addons/l10n_bg_ledger/i18n/l10n_bg_ledger.pot` (126 lines)
- `addons/l10n_bg_ledger/models/__init__.py` (3 lines)
- `addons/l10n_bg_ledger/models/account_journal.py` (26 lines)
- `addons/l10n_bg_ledger/models/account_move.py` (58 lines)
- `addons/l10n_bg_ledger/views/account_journal_views.xml` (17 lines)
- `addons/l10n_bg_ledger/views/account_move_views.xml` (40 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
