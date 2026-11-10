# Module: sale_project_stock

- **Module ID:** MOD-526
- **Path:** `addons/sale_project_stock`
- **Manifest:** `addons/sale_project_stock/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Adds a full traceability of inventory operations on the profitability report.

Adds a full traceability of inventory operations on the profitability report.

Declared dependencies: `sale_project`, `sale_stock`, `project_stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 10 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 0 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "sale_project",
    "sale_stock",
    "project_stock_account"
  ]
}
```

### Representative source files

- `addons/sale_project_stock/__init__.py` (4 lines)
- `addons/sale_project_stock/__manifest__.py` (12 lines)
- `addons/sale_project_stock/i18n/ar.po` (115 lines)
- `addons/sale_project_stock/i18n/az.po` (104 lines)
- `addons/sale_project_stock/i18n/bg.po` (104 lines)
- `addons/sale_project_stock/i18n/bs.po` (106 lines)
- `addons/sale_project_stock/i18n/ca.po` (110 lines)
- `addons/sale_project_stock/i18n/cs.po` (106 lines)
- `addons/sale_project_stock/i18n/da.po` (113 lines)
- `addons/sale_project_stock/i18n/de.po` (123 lines)
- `addons/sale_project_stock/i18n/el.po` (105 lines)
- `addons/sale_project_stock/i18n/es.po` (117 lines)
- `addons/sale_project_stock/i18n/es_419.po` (121 lines)
- `addons/sale_project_stock/i18n/et.po` (112 lines)
- `addons/sale_project_stock/i18n/fa.po` (104 lines)
- `addons/sale_project_stock/i18n/fi.po` (114 lines)
- `addons/sale_project_stock/i18n/fr.po` (120 lines)
- `addons/sale_project_stock/i18n/he.po` (105 lines)
- `addons/sale_project_stock/i18n/hi.po` (104 lines)
- `addons/sale_project_stock/i18n/hr.po` (105 lines)
- `addons/sale_project_stock/i18n/hu.po` (114 lines)
- `addons/sale_project_stock/i18n/id.po` (114 lines)
- `addons/sale_project_stock/i18n/it.po` (120 lines)
- `addons/sale_project_stock/i18n/ja.po` (120 lines)
- `addons/sale_project_stock/i18n/kab.po` (105 lines)
- `addons/sale_project_stock/i18n/ko.po` (114 lines)
- `addons/sale_project_stock/i18n/ku.po` (104 lines)
- `addons/sale_project_stock/i18n/lo.po` (104 lines)
- `addons/sale_project_stock/i18n/lt.po` (106 lines)
- `addons/sale_project_stock/i18n/lv.po` (105 lines)
- `addons/sale_project_stock/i18n/mn.po` (104 lines)
- `addons/sale_project_stock/i18n/my.po` (105 lines)
- `addons/sale_project_stock/i18n/nb.po` (105 lines)
- `addons/sale_project_stock/i18n/nl.po` (120 lines)
- `addons/sale_project_stock/i18n/pl.po` (107 lines)
- `addons/sale_project_stock/i18n/pt.po` (113 lines)
- `addons/sale_project_stock/i18n/pt_BR.po` (124 lines)
- `addons/sale_project_stock/i18n/ro.po` (114 lines)
- `addons/sale_project_stock/i18n/ru.po` (116 lines)
- `addons/sale_project_stock/i18n/sale_project_stock.pot` (102 lines)
- `addons/sale_project_stock/i18n/sk.po` (104 lines)
- `addons/sale_project_stock/i18n/sl.po` (106 lines)
- `addons/sale_project_stock/i18n/sr@latin.po` (105 lines)
- `addons/sale_project_stock/i18n/sv.po` (113 lines)
- `addons/sale_project_stock/i18n/th.po` (116 lines)
- `addons/sale_project_stock/i18n/tr.po` (116 lines)
- `addons/sale_project_stock/i18n/uk.po` (107 lines)
- `addons/sale_project_stock/i18n/uz.po` (128 lines)
- `addons/sale_project_stock/i18n/vi.po` (113 lines)
- `addons/sale_project_stock/i18n/zh_CN.po` (118 lines)
- `addons/sale_project_stock/i18n/zh_TW.po` (113 lines)
- `addons/sale_project_stock/models/__init__.py` (7 lines)
- `addons/sale_project_stock/models/account_analytic_line.py` (29 lines)
- `addons/sale_project_stock/models/project_project.py` (18 lines)
- `addons/sale_project_stock/models/stock_move.py` (77 lines)
- `addons/sale_project_stock/models/stock_picking.py` (62 lines)
- `addons/sale_project_stock/tests/__init__.py` (4 lines)
- `addons/sale_project_stock/tests/test_analytic_line.py` (70 lines)
- `addons/sale_project_stock/tests/test_reinvoice.py` (86 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
