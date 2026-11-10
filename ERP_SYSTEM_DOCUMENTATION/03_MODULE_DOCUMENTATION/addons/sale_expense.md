# Module: sale_expense

- **Module ID:** MOD-512
- **Path:** `addons/sale_expense`
- **Manifest:** `addons/sale_expense/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Quotation, Sales Orders, Delivery & Invoicing Control


Reinvoice Employee Expense
==========================

Create some products for which you can re-invoice the costs.
This module allow to reinvoice employee expense, by setting the SO directly on the expense.


Declared dependencies: `sale_management`, `hr_expense`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 15 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 8 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 6 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 1 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 1 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_management",
    "hr_expense"
  ],
  "data": [
    "data/sale_expense_data.xml",
    "views/product_view.xml",
    "views/hr_expense_views.xml",
    "views/sale_order_views.xml",
    "wizard/expense_attachment_selection_wizard_views.xml",
    "security/ir.access.csv"
  ],
  "assets": {
    "web.assets_backend": [
      "sale_expense/static/src/views/*"
    ]
  }
}
```

### Representative source files

- `addons/sale_expense/__init__.py` (5 lines)
- `addons/sale_expense/__manifest__.py` (31 lines)
- `addons/sale_expense/data/sale_expense_data.xml` (25 lines)
- `addons/sale_expense/i18n/ar.po` (266 lines)
- `addons/sale_expense/i18n/az.po` (262 lines)
- `addons/sale_expense/i18n/bg.po` (258 lines)
- `addons/sale_expense/i18n/bs.po` (262 lines)
- `addons/sale_expense/i18n/ca.po` (273 lines)
- `addons/sale_expense/i18n/cs.po` (264 lines)
- `addons/sale_expense/i18n/da.po` (268 lines)
- `addons/sale_expense/i18n/de.po` (283 lines)
- `addons/sale_expense/i18n/el.po` (268 lines)
- `addons/sale_expense/i18n/es.po` (279 lines)
- `addons/sale_expense/i18n/es_419.po` (266 lines)
- `addons/sale_expense/i18n/et.po` (273 lines)
- `addons/sale_expense/i18n/fa.po` (264 lines)
- `addons/sale_expense/i18n/fi.po` (282 lines)
- `addons/sale_expense/i18n/fr.po` (274 lines)
- `addons/sale_expense/i18n/gu.po` (210 lines)
- `addons/sale_expense/i18n/he.po` (266 lines)
- `addons/sale_expense/i18n/hi.po` (258 lines)
- `addons/sale_expense/i18n/hr.po` (264 lines)
- `addons/sale_expense/i18n/hu.po` (266 lines)
- `addons/sale_expense/i18n/id.po` (268 lines)
- `addons/sale_expense/i18n/is.po` (210 lines)
- `addons/sale_expense/i18n/it.po` (279 lines)
- `addons/sale_expense/i18n/ja.po` (265 lines)
- `addons/sale_expense/i18n/kab.po` (259 lines)
- `addons/sale_expense/i18n/km.po` (206 lines)
- `addons/sale_expense/i18n/ko.po` (265 lines)
- `addons/sale_expense/i18n/ku.po` (258 lines)
- `addons/sale_expense/i18n/lo.po` (258 lines)
- `addons/sale_expense/i18n/lt.po` (266 lines)
- `addons/sale_expense/i18n/lv.po` (262 lines)
- `addons/sale_expense/i18n/mn.po` (263 lines)
- `addons/sale_expense/i18n/my.po` (259 lines)
- `addons/sale_expense/i18n/nb.po` (262 lines)
- `addons/sale_expense/i18n/nl.po` (281 lines)
- `addons/sale_expense/i18n/pl.po` (275 lines)
- `addons/sale_expense/i18n/pt.po` (271 lines)
- `addons/sale_expense/i18n/pt_BR.po` (285 lines)
- `addons/sale_expense/i18n/ro.po` (265 lines)
- `addons/sale_expense/i18n/ru.po` (269 lines)
- `addons/sale_expense/i18n/sale_expense.pot` (254 lines)
- `addons/sale_expense/i18n/sk.po` (263 lines)
- `addons/sale_expense/i18n/sl.po` (265 lines)
- `addons/sale_expense/i18n/sr@latin.po` (263 lines)
- `addons/sale_expense/i18n/sv.po` (271 lines)
- `addons/sale_expense/i18n/th.po` (264 lines)
- `addons/sale_expense/i18n/tr.po` (272 lines)
- `addons/sale_expense/i18n/uk.po` (267 lines)
- `addons/sale_expense/i18n/uz.po` (290 lines)
- `addons/sale_expense/i18n/vi.po` (268 lines)
- `addons/sale_expense/i18n/zh_CN.po` (271 lines)
- `addons/sale_expense/i18n/zh_TW.po` (263 lines)
- `addons/sale_expense/models/__init__.py` (9 lines)
- `addons/sale_expense/models/account_move.py` (22 lines)
- `addons/sale_expense/models/account_move_line.py` (58 lines)
- `addons/sale_expense/models/hr_expense.py` (96 lines)
- `addons/sale_expense/models/hr_expense_split.py` (26 lines)
- `addons/sale_expense/models/product_template.py` (40 lines)
- `addons/sale_expense/models/sale_order.py` (79 lines)
- `addons/sale_expense/models/sale_order_line.py` (14 lines)
- `addons/sale_expense/security/ir.access.csv` (2 lines)
- `addons/sale_expense/static/src/views/attachment_selector.js` (38 lines)
- `addons/sale_expense/static/src/views/attachment_selector.xml` (18 lines)
- `addons/sale_expense/tests/__init__.py` (5 lines)
- `addons/sale_expense/tests/test_reinvoice.py` (564 lines)
- `addons/sale_expense/tests/test_sale_expense.py` (248 lines)
- `addons/sale_expense/views/hr_expense_views.xml` (69 lines)
- `addons/sale_expense/views/product_view.xml` (48 lines)
- `addons/sale_expense/views/sale_order_views.xml` (50 lines)
- `addons/sale_expense/wizard/__init__.py` (1 lines)
- `addons/sale_expense/wizard/expense_attachment_selection_wizard.py` (49 lines)
- `addons/sale_expense/wizard/expense_attachment_selection_wizard_views.xml` (20 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
