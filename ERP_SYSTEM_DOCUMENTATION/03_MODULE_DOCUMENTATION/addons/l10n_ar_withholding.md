# Module: l10n_ar_withholding

- **Module ID:** MOD-124
- **Path:** `addons/l10n_ar_withholding`
- **Manifest:** `addons/l10n_ar_withholding/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `not declared`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

Allows to register withholdings during the payment of an invoice.

Declared dependencies: `l10n_ar`, `l10n_latam_check`, `l10n_account_withholding_tax`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 19 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 10 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 5 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "l10n_ar",
    "l10n_latam_check",
    "l10n_account_withholding_tax"
  ],
  "data": [
    "data/earnings_table_data.xml",
    "security/ir.access.csv",
    "views/account_tax_views.xml",
    "views/res_partner_view.xml",
    "views/l10n_ar_earnings_scale_view.xml",
    "wizards/account_payment_register_views.xml"
  ]
}
```

### Representative source files

- `addons/l10n_ar_withholding/__init__.py` (5 lines)
- `addons/l10n_ar_withholding/__manifest__.py` (22 lines)
- `addons/l10n_ar_withholding/data/earnings_table_data.xml` (115 lines)
- `addons/l10n_ar_withholding/data/template/account.account-ar_base.csv` (2 lines)
- `addons/l10n_ar_withholding/data/template/account.tax-ar_base.csv` (126 lines)
- `addons/l10n_ar_withholding/data/template/account.tax-ar_ex.csv` (279 lines)
- `addons/l10n_ar_withholding/data/template/account.tax-ar_ri.csv` (5 lines)
- `addons/l10n_ar_withholding/data/template/account.tax.group-ar_base.csv` (26 lines)
- `addons/l10n_ar_withholding/data/template/account.tax.group-ar_ex.csv` (3 lines)
- `addons/l10n_ar_withholding/demo/__init__.py` (3 lines)
- `addons/l10n_ar_withholding/demo/account_demo.py` (54 lines)
- `addons/l10n_ar_withholding/i18n/es_419.po` (706 lines)
- `addons/l10n_ar_withholding/i18n/l10n_ar_withholding.pot` (467 lines)
- `addons/l10n_ar_withholding/models/__init__.py` (11 lines)
- `addons/l10n_ar_withholding/models/account_chart_template.py` (41 lines)
- `addons/l10n_ar_withholding/models/account_payment.py` (24 lines)
- `addons/l10n_ar_withholding/models/account_payment_withholding_line.py` (8 lines)
- `addons/l10n_ar_withholding/models/account_tax.py` (89 lines)
- `addons/l10n_ar_withholding/models/account_withholding_line.py` (72 lines)
- `addons/l10n_ar_withholding/models/l10n_ar_earnings_scale.py` (26 lines)
- `addons/l10n_ar_withholding/models/l10n_ar_earnings_scale_line.py` (53 lines)
- `addons/l10n_ar_withholding/models/l10n_ar_partner_tax.py` (38 lines)
- `addons/l10n_ar_withholding/models/res_partner.py` (84 lines)
- `addons/l10n_ar_withholding/security/ir.access.csv` (9 lines)
- `addons/l10n_ar_withholding/tests/__init__.py` (1 lines)
- `addons/l10n_ar_withholding/tests/test_withholding_ar_ri.py` (1,405 lines)
- `addons/l10n_ar_withholding/views/account_tax_views.xml` (51 lines)
- `addons/l10n_ar_withholding/views/l10n_ar_earnings_scale_view.xml` (60 lines)
- `addons/l10n_ar_withholding/views/res_partner_view.xml` (24 lines)
- `addons/l10n_ar_withholding/wizards/__init__.py` (4 lines)
- `addons/l10n_ar_withholding/wizards/account_payment_register.py` (189 lines)
- `addons/l10n_ar_withholding/wizards/account_payment_register_views.xml` (17 lines)
- `addons/l10n_ar_withholding/wizards/account_payment_register_withholding_line.py` (44 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
