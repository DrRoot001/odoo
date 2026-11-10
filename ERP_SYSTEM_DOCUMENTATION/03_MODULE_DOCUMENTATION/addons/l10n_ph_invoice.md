# Module: l10n_ph_invoice

- **Module ID:** MOD-293
- **Path:** `addons/l10n_ph_invoice`
- **Manifest:** `addons/l10n_ph_invoice/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

Apply Philippine SC/PWD discount privileges on customer invoices and credit notes.

No manifest description declared.

Declared dependencies: `l10n_ph`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 12 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 4 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ph"
  ],
  "data": [
    "security/ir.access.csv",
    "wizard/l10n_ph_discount_privilege_wizard_views.xml",
    "views/l10n_ph_discount_privilege_views.xml",
    "views/account_move_views.xml",
    "data/menuitem_data.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ph_invoice/__init__.py` (4 lines)
- `addons/l10n_ph_invoice/__manifest__.py` (21 lines)
- `addons/l10n_ph_invoice/data/menuitem_data.xml` (10 lines)
- `addons/l10n_ph_invoice/i18n/l10n_ph_invoice.pot` (472 lines)
- `addons/l10n_ph_invoice/i18n/tl.po` (472 lines)
- `addons/l10n_ph_invoice/models/__init__.py` (7 lines)
- `addons/l10n_ph_invoice/models/account_move.py` (30 lines)
- `addons/l10n_ph_invoice/models/account_move_line.py` (121 lines)
- `addons/l10n_ph_invoice/models/l10n_ph_discount_privilege.py` (85 lines)
- `addons/l10n_ph_invoice/models/l10n_ph_discount_privilege_line_mixin.py` (164 lines)
- `addons/l10n_ph_invoice/models/template_ph.py` (34 lines)
- `addons/l10n_ph_invoice/security/ir.access.csv` (7 lines)
- `addons/l10n_ph_invoice/tests/__init__.py` (3 lines)
- `addons/l10n_ph_invoice/tests/test_discount_privilege_wizard.py` (1,328 lines)
- `addons/l10n_ph_invoice/views/account_move_views.xml` (37 lines)
- `addons/l10n_ph_invoice/views/l10n_ph_discount_privilege_views.xml` (48 lines)
- `addons/l10n_ph_invoice/wizard/__init__.py` (3 lines)
- `addons/l10n_ph_invoice/wizard/l10n_ph_discount_privilege_wizard.py` (437 lines)
- `addons/l10n_ph_invoice/wizard/l10n_ph_discount_privilege_wizard_views.xml` (65 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
