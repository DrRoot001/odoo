# Module: l10n_account_withholding_tax

- **Module ID:** MOD-115
- **Path:** `addons/l10n_account_withholding_tax`
- **Manifest:** `addons/l10n_account_withholding_tax/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Allows users to manage withholding taxes on invoices, bills, and payments.

Declared dependencies: `account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 9 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 8 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 2 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
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
    "views/account_move_views.xml",
    "views/account_payment_views.xml",
    "views/account_tax_views.xml",
    "views/report_payment_receipt_templates.xml",
    "views/res_config_settings.xml",
    "wizards/account_payment_register_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "l10n_account_withholding_tax/static/src/helpers/*.js",
      "l10n_account_withholding_tax/static/src/components/**/*"
    ],
    "web.assets_frontend": [
      "l10n_account_withholding_tax/static/src/helpers/*.js"
    ]
  }
}
```

### Representative source files

- `addons/l10n_account_withholding_tax/__init__.py` (13 lines)
- `addons/l10n_account_withholding_tax/__manifest__.py` (30 lines)
- `addons/l10n_account_withholding_tax/demo/__init__.py` (1 lines)
- `addons/l10n_account_withholding_tax/demo/demo.py` (82 lines)
- `addons/l10n_account_withholding_tax/i18n/en_IN.po` (260 lines)
- `addons/l10n_account_withholding_tax/i18n/es_419.po` (759 lines)
- `addons/l10n_account_withholding_tax/i18n/id.po` (774 lines)
- `addons/l10n_account_withholding_tax/i18n/l10n_account_withholding_tax.pot` (735 lines)
- `addons/l10n_account_withholding_tax/i18n/th.po` (755 lines)
- `addons/l10n_account_withholding_tax/models/__init__.py` (10 lines)
- `addons/l10n_account_withholding_tax/models/account_move.py` (133 lines)
- `addons/l10n_account_withholding_tax/models/account_payment.py` (159 lines)
- `addons/l10n_account_withholding_tax/models/account_payment_withholding_line.py` (115 lines)
- `addons/l10n_account_withholding_tax/models/account_tax.py` (82 lines)
- `addons/l10n_account_withholding_tax/models/account_withholding_line.py` (555 lines)
- `addons/l10n_account_withholding_tax/models/product_template.py` (67 lines)
- `addons/l10n_account_withholding_tax/models/res_company.py` (16 lines)
- `addons/l10n_account_withholding_tax/models/res_config_settings.py` (15 lines)
- `addons/l10n_account_withholding_tax/security/ir.access.csv` (3 lines)
- `addons/l10n_account_withholding_tax/static/src/components/account_payment.xml` (8 lines)
- `addons/l10n_account_withholding_tax/static/src/components/withhold_selector/withhold_selector.js` (28 lines)
- `addons/l10n_account_withholding_tax/static/src/helpers/account_tax.js` (12 lines)
- `addons/l10n_account_withholding_tax/tests/__init__.py` (4 lines)
- `addons/l10n_account_withholding_tax/tests/test_account_withholding_amounts.py` (558 lines)
- `addons/l10n_account_withholding_tax/tests/test_account_withholding_flows.py` (1,390 lines)
- `addons/l10n_account_withholding_tax/views/account_move_views.xml` (30 lines)
- `addons/l10n_account_withholding_tax/views/account_payment_views.xml` (78 lines)
- `addons/l10n_account_withholding_tax/views/account_tax_views.xml` (39 lines)
- `addons/l10n_account_withholding_tax/views/report_invoice.xml` (7 lines)
- `addons/l10n_account_withholding_tax/views/report_payment_receipt_templates.xml` (37 lines)
- `addons/l10n_account_withholding_tax/views/res_config_settings.xml` (20 lines)
- `addons/l10n_account_withholding_tax/wizards/__init__.py` (4 lines)
- `addons/l10n_account_withholding_tax/wizards/account_payment_register.py` (339 lines)
- `addons/l10n_account_withholding_tax/wizards/account_payment_register_views.xml` (69 lines)
- `addons/l10n_account_withholding_tax/wizards/account_payment_register_withholding_line.py` (130 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
