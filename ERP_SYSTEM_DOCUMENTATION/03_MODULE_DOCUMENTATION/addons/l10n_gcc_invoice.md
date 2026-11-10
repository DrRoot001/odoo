# Module: l10n_gcc_invoice

- **Module ID:** MOD-199
- **Path:** `addons/l10n_gcc_invoice`
- **Manifest:** `addons/l10n_gcc_invoice/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.


Adds Arabic as a secondary language on your invoice, credit note, debit note, vendor bill, and refund bill


Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
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
    "account"
  ],
  "data": [
    "views/report_invoice.xml",
    "views/res_config_settings_views.xml"
  ],
  "assets": {
    "web.report_assets_common": [
      "l10n_gcc_invoice/static/src/scss/styles.scss"
    ]
  }
}
```

### Representative source files

- `addons/l10n_gcc_invoice/__init__.py` (5 lines)
- `addons/l10n_gcc_invoice/__manifest__.py` (21 lines)
- `addons/l10n_gcc_invoice/i18n/ar.po` (110 lines)
- `addons/l10n_gcc_invoice/i18n/l10n_gcc_invoice.pot` (103 lines)
- `addons/l10n_gcc_invoice/models/__init__.py` (7 lines)
- `addons/l10n_gcc_invoice/models/account_move.py` (78 lines)
- `addons/l10n_gcc_invoice/models/product.py` (24 lines)
- `addons/l10n_gcc_invoice/models/res_company.py` (13 lines)
- `addons/l10n_gcc_invoice/models/res_config_settings.py` (8 lines)
- `addons/l10n_gcc_invoice/static/src/scss/styles.scss` (3 lines)
- `addons/l10n_gcc_invoice/tests/__init__.py` (3 lines)
- `addons/l10n_gcc_invoice/tests/test_gcc_invoice.py` (33 lines)
- `addons/l10n_gcc_invoice/views/report_invoice.xml` (319 lines)
- `addons/l10n_gcc_invoice/views/res_config_settings_views.xml` (19 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
