# Module: project_stock_account

- **Module ID:** MOD-489
- **Path:** `addons/project_stock_account`
- **Manifest:** `addons/project_stock_account/__manifest__.py`
- **Implementation status:** Implemented artifacts present
- **Application flag:** `not declared`
- **Installable flag:** `not declared`
- **Auto install:** `True`
- **License:** `LGPL-3`

## Purpose and dependencies

Handle analytics in Stock pickings with Project

No manifest description declared.

Declared dependencies: `stock_account`, `project_stock`.

## Static implementation surface

| Artifact | Count | Evidence / interpretation |
|---|---:|---|
| Python files | 9 | ORM, services, controllers, wizards, reports, or tests; inspect file inventory below. |
| Model-path Python files | 5 | Files under `models/` or `models.py`. |
| Controller-path Python files | 0 | Files under `controllers/` or `controllers.py`. |
| XML files | 1 | Views, actions, menus, templates, data, reports, or tests. |
| JavaScript/TypeScript | 0 | Client behavior/assets. |
| Tests | 2 | Test files found by path/name convention. |
| Security artifacts | 0 | Access CSV and/or security XML. |
| Route declarations | 0 | Static decorator matches. |

## Evidence inventory

### Manifest-declared data and assets

```text
{
  "depends": [
    "stock_account",
    "project_stock"
  ],
  "data": [
    "views/stock_picking_type_views.xml"
  ]
}
```

### Representative source files

- `addons/project_stock_account/__init__.py` (3 lines)
- `addons/project_stock_account/__manifest__.py` (14 lines)
- `addons/project_stock_account/i18n/ar.po` (113 lines)
- `addons/project_stock_account/i18n/az.po` (105 lines)
- `addons/project_stock_account/i18n/bg.po` (105 lines)
- `addons/project_stock_account/i18n/bs.po` (107 lines)
- `addons/project_stock_account/i18n/ca.po` (111 lines)
- `addons/project_stock_account/i18n/cs.po` (107 lines)
- `addons/project_stock_account/i18n/da.po` (107 lines)
- `addons/project_stock_account/i18n/de.po` (112 lines)
- `addons/project_stock_account/i18n/el.po` (106 lines)
- `addons/project_stock_account/i18n/es.po` (113 lines)
- `addons/project_stock_account/i18n/es_419.po` (113 lines)
- `addons/project_stock_account/i18n/et.po` (111 lines)
- `addons/project_stock_account/i18n/fa.po` (105 lines)
- `addons/project_stock_account/i18n/fi.po` (112 lines)
- `addons/project_stock_account/i18n/fr.po` (112 lines)
- `addons/project_stock_account/i18n/he.po` (106 lines)
- `addons/project_stock_account/i18n/hi.po` (105 lines)
- `addons/project_stock_account/i18n/hr.po` (106 lines)
- `addons/project_stock_account/i18n/hu.po` (106 lines)
- `addons/project_stock_account/i18n/id.po` (113 lines)
- `addons/project_stock_account/i18n/it.po` (112 lines)
- `addons/project_stock_account/i18n/ja.po` (111 lines)
- `addons/project_stock_account/i18n/kab.po` (106 lines)
- `addons/project_stock_account/i18n/ko.po` (111 lines)
- `addons/project_stock_account/i18n/ku.po` (105 lines)
- `addons/project_stock_account/i18n/lo.po` (105 lines)
- `addons/project_stock_account/i18n/lt.po` (107 lines)
- `addons/project_stock_account/i18n/lv.po` (106 lines)
- `addons/project_stock_account/i18n/mn.po` (105 lines)
- `addons/project_stock_account/i18n/my.po` (105 lines)
- `addons/project_stock_account/i18n/nb.po` (106 lines)
- `addons/project_stock_account/i18n/nl.po` (112 lines)
- `addons/project_stock_account/i18n/pl.po` (114 lines)
- `addons/project_stock_account/i18n/project_stock_account.pot` (102 lines)
- `addons/project_stock_account/i18n/pt.po` (111 lines)
- `addons/project_stock_account/i18n/pt_BR.po` (114 lines)
- `addons/project_stock_account/i18n/ro.po` (112 lines)
- `addons/project_stock_account/i18n/ru.po` (113 lines)
- `addons/project_stock_account/i18n/sk.po` (105 lines)
- `addons/project_stock_account/i18n/sl.po` (107 lines)
- `addons/project_stock_account/i18n/sr@latin.po` (106 lines)
- `addons/project_stock_account/i18n/sv.po` (113 lines)
- `addons/project_stock_account/i18n/th.po` (111 lines)
- `addons/project_stock_account/i18n/tr.po` (115 lines)
- `addons/project_stock_account/i18n/uk.po` (106 lines)
- `addons/project_stock_account/i18n/uz.po` (131 lines)
- `addons/project_stock_account/i18n/vi.po` (112 lines)
- `addons/project_stock_account/i18n/zh_CN.po` (111 lines)
- `addons/project_stock_account/i18n/zh_TW.po` (114 lines)
- `addons/project_stock_account/models/__init__.py` (6 lines)
- `addons/project_stock_account/models/account_analytic_line.py` (9 lines)
- `addons/project_stock_account/models/analytic_applicability.py` (14 lines)
- `addons/project_stock_account/models/stock_move.py` (43 lines)
- `addons/project_stock_account/models/stock_picking_type.py` (19 lines)
- `addons/project_stock_account/tests/__init__.py` (3 lines)
- `addons/project_stock_account/tests/test_analytics.py` (159 lines)
- `addons/project_stock_account/views/stock_picking_type_views.xml` (13 lines)

## Functional behavior classification

Static artifacts establish that the module is present and wired into Odoo's addon system. Exact screens, fields, access rules, state transitions, response payloads, and side effects require reading the referenced implementations and/or executing the module in a configured database. No behavior is inferred solely from the module name.
