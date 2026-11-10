# Module: l10n_gcc_invoice_stock_account

- **Module ID:** MOD-200
- **Path:** `addons/l10n_gcc_invoice_stock_account`
- **Manifest:** `addons/l10n_gcc_invoice_stock_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Adds Arabic as a secondary language for the lots and serial numbers
    

Declared dependencies: `l10n_gcc_invoice`, `stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 2 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 0 | Files under `models/` or `models.py`. |
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
    "l10n_gcc_invoice",
    "stock_account"
  ],
  "data": [
    "views/report_invoice.xml"
  ]
}
```

### Representative source files

- `addons/l10n_gcc_invoice_stock_account/__init__.py` (2 lines)
- `addons/l10n_gcc_invoice_stock_account/__manifest__.py` (17 lines)
- `addons/l10n_gcc_invoice_stock_account/views/report_invoice.xml` (17 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
