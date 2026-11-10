# Module: project_mrp_account

- **Module ID:** MOD-481
- **Path:** `addons/project_mrp_account`
- **Manifest:** `addons/project_mrp_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Monitor MRP account using project

No manifest description declared.

Declared dependencies: `mrp_account`, `project_mrp`, `project_stock_account`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 11 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 6 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 3 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 3 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "mrp_account",
    "project_mrp",
    "project_stock_account"
  ],
  "data": [
    "data/project_mrp_account_data.xml",
    "views/stock_picking_type_views.xml"
  ],
  "demo": [
    "data/project_mrp_account_demo.xml"
  ]
}
```

### Representative source files

- `addons/project_mrp_account/__init__.py` (3 lines)
- `addons/project_mrp_account/__manifest__.py` (18 lines)
- `addons/project_mrp_account/data/project_mrp_account_data.xml` (9 lines)
- `addons/project_mrp_account/data/project_mrp_account_demo.xml` (38 lines)
- `addons/project_mrp_account/i18n/ar.po` (121 lines)
- `addons/project_mrp_account/i18n/az.po` (111 lines)
- `addons/project_mrp_account/i18n/bg.po` (111 lines)
- `addons/project_mrp_account/i18n/bs.po` (113 lines)
- `addons/project_mrp_account/i18n/ca.po` (114 lines)
- `addons/project_mrp_account/i18n/cs.po` (113 lines)
- `addons/project_mrp_account/i18n/da.po` (112 lines)
- `addons/project_mrp_account/i18n/de.po` (119 lines)
- `addons/project_mrp_account/i18n/el.po` (112 lines)
- `addons/project_mrp_account/i18n/es.po` (118 lines)
- `addons/project_mrp_account/i18n/es_419.po` (120 lines)
- `addons/project_mrp_account/i18n/et.po` (114 lines)
- `addons/project_mrp_account/i18n/fa.po` (111 lines)
- `addons/project_mrp_account/i18n/fi.po` (117 lines)
- `addons/project_mrp_account/i18n/fr.po` (120 lines)
- `addons/project_mrp_account/i18n/he.po` (112 lines)
- `addons/project_mrp_account/i18n/hi.po` (111 lines)
- `addons/project_mrp_account/i18n/hr.po` (112 lines)
- `addons/project_mrp_account/i18n/hu.po` (112 lines)
- `addons/project_mrp_account/i18n/id.po` (116 lines)
- `addons/project_mrp_account/i18n/it.po` (119 lines)
- `addons/project_mrp_account/i18n/ja.po` (115 lines)
- `addons/project_mrp_account/i18n/kab.po` (112 lines)
- `addons/project_mrp_account/i18n/ko.po` (115 lines)
- `addons/project_mrp_account/i18n/ku.po` (111 lines)
- `addons/project_mrp_account/i18n/lo.po` (111 lines)
- `addons/project_mrp_account/i18n/lt.po` (113 lines)
- `addons/project_mrp_account/i18n/lv.po` (112 lines)
- `addons/project_mrp_account/i18n/mn.po` (111 lines)
- `addons/project_mrp_account/i18n/my.po` (111 lines)
- `addons/project_mrp_account/i18n/nb.po` (112 lines)
- `addons/project_mrp_account/i18n/nl.po` (119 lines)
- `addons/project_mrp_account/i18n/pl.po` (119 lines)
- `addons/project_mrp_account/i18n/project_mrp_account.pot` (108 lines)
- `addons/project_mrp_account/i18n/pt.po` (114 lines)
- `addons/project_mrp_account/i18n/pt_BR.po` (121 lines)
- `addons/project_mrp_account/i18n/ro.po` (115 lines)
- `addons/project_mrp_account/i18n/ru.po` (118 lines)
- `addons/project_mrp_account/i18n/sk.po` (111 lines)
- `addons/project_mrp_account/i18n/sl.po` (113 lines)
- `addons/project_mrp_account/i18n/sr@latin.po` (112 lines)
- `addons/project_mrp_account/i18n/sv.po` (115 lines)
- `addons/project_mrp_account/i18n/th.po` (117 lines)
- `addons/project_mrp_account/i18n/tr.po` (121 lines)
- `addons/project_mrp_account/i18n/uk.po` (112 lines)
- `addons/project_mrp_account/i18n/uz.po` (131 lines)
- `addons/project_mrp_account/i18n/vi.po` (115 lines)
- `addons/project_mrp_account/i18n/zh_CN.po` (115 lines)
- `addons/project_mrp_account/i18n/zh_TW.po` (117 lines)
- `addons/project_mrp_account/models/__init__.py` (7 lines)
- `addons/project_mrp_account/models/mrp_production.py` (56 lines)
- `addons/project_mrp_account/models/mrp_workorder.py` (15 lines)
- `addons/project_mrp_account/models/stock_move.py` (36 lines)
- `addons/project_mrp_account/models/stock_picking_type.py` (14 lines)
- `addons/project_mrp_account/models/stock_rule.py` (13 lines)
- `addons/project_mrp_account/tests/__init__.py` (4 lines)
- `addons/project_mrp_account/tests/test_analytic_account.py` (552 lines)
- `addons/project_mrp_account/tests/test_project_stock.py` (20 lines)
- `addons/project_mrp_account/views/stock_picking_type_views.xml` (14 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
