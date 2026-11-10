# Module: sale_expense_margin

- **Module ID:** MOD-513
- **Path:** `addons/sale_expense_margin`
- **Manifest:** `addons/sale_expense_margin/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

No manifest summary declared.

When re-invoicing the expense on the SO, set the cost to the total untaxed amount of the expense.

Declared dependencies: `sale_expense`, `sale_margin`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 7 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 3 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_expense",
    "sale_margin"
  ]
}
```

### Representative source files

- `addons/sale_expense_margin/__init__.py` (4 lines)
- `addons/sale_expense_margin/__manifest__.py` (10 lines)
- `addons/sale_expense_margin/i18n/ar.po` (61 lines)
- `addons/sale_expense_margin/i18n/az.po` (58 lines)
- `addons/sale_expense_margin/i18n/bg.po` (58 lines)
- `addons/sale_expense_margin/i18n/bs.po` (60 lines)
- `addons/sale_expense_margin/i18n/ca.po` (59 lines)
- `addons/sale_expense_margin/i18n/cs.po` (60 lines)
- `addons/sale_expense_margin/i18n/da.po` (60 lines)
- `addons/sale_expense_margin/i18n/de.po` (62 lines)
- `addons/sale_expense_margin/i18n/el.po` (59 lines)
- `addons/sale_expense_margin/i18n/es.po` (63 lines)
- `addons/sale_expense_margin/i18n/es_419.po` (60 lines)
- `addons/sale_expense_margin/i18n/et.po` (59 lines)
- `addons/sale_expense_margin/i18n/fa.po` (58 lines)
- `addons/sale_expense_margin/i18n/fi.po` (62 lines)
- `addons/sale_expense_margin/i18n/fr.po` (60 lines)
- `addons/sale_expense_margin/i18n/he.po` (59 lines)
- `addons/sale_expense_margin/i18n/hi.po` (58 lines)
- `addons/sale_expense_margin/i18n/hr.po` (59 lines)
- `addons/sale_expense_margin/i18n/hu.po` (59 lines)
- `addons/sale_expense_margin/i18n/id.po` (60 lines)
- `addons/sale_expense_margin/i18n/it.po` (60 lines)
- `addons/sale_expense_margin/i18n/ja.po` (60 lines)
- `addons/sale_expense_margin/i18n/kab.po` (59 lines)
- `addons/sale_expense_margin/i18n/ko.po` (60 lines)
- `addons/sale_expense_margin/i18n/ku.po` (58 lines)
- `addons/sale_expense_margin/i18n/lo.po` (58 lines)
- `addons/sale_expense_margin/i18n/lt.po` (60 lines)
- `addons/sale_expense_margin/i18n/lv.po` (59 lines)
- `addons/sale_expense_margin/i18n/mn.po` (58 lines)
- `addons/sale_expense_margin/i18n/my.po` (58 lines)
- `addons/sale_expense_margin/i18n/nb.po` (59 lines)
- `addons/sale_expense_margin/i18n/nl.po` (60 lines)
- `addons/sale_expense_margin/i18n/pl.po` (61 lines)
- `addons/sale_expense_margin/i18n/pt.po` (59 lines)
- `addons/sale_expense_margin/i18n/pt_BR.po` (63 lines)
- `addons/sale_expense_margin/i18n/ro.po` (60 lines)
- `addons/sale_expense_margin/i18n/ru.po` (63 lines)
- `addons/sale_expense_margin/i18n/sale_expense_margin.pot` (55 lines)
- `addons/sale_expense_margin/i18n/sk.po` (58 lines)
- `addons/sale_expense_margin/i18n/sl.po` (60 lines)
- `addons/sale_expense_margin/i18n/sr@latin.po` (59 lines)
- `addons/sale_expense_margin/i18n/sv.po` (60 lines)
- `addons/sale_expense_margin/i18n/th.po` (60 lines)
- `addons/sale_expense_margin/i18n/tr.po` (59 lines)
- `addons/sale_expense_margin/i18n/uk.po` (59 lines)
- `addons/sale_expense_margin/i18n/uz.po` (71 lines)
- `addons/sale_expense_margin/i18n/vi.po` (60 lines)
- `addons/sale_expense_margin/i18n/zh_CN.po` (61 lines)
- `addons/sale_expense_margin/i18n/zh_TW.po` (63 lines)
- `addons/sale_expense_margin/models/__init__.py` (5 lines)
- `addons/sale_expense_margin/models/account_move_line.py` (14 lines)
- `addons/sale_expense_margin/models/sale_order_line.py` (19 lines)
- `addons/sale_expense_margin/tests/__init__.py` (4 lines)
- `addons/sale_expense_margin/tests/test_so_expense_purchase_price.py` (86 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
